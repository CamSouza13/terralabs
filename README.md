# Terra Laboratories

Marketing site for [Terra Laboratories](https://terralaboratories.com).
Predictive Bayesian state estimation for closed living systems.

Static. No build step, no dependencies, no framework.

## Layout

```
index.html         the site
terra-team.html    leadership page
assets/img/        hero posters and card stills
assets/video/      hero footage (H.264 MP4, 1920x1080, silent, looping)
DEPLOY.txt         hero swap instructions, system index map, source register notes
```

## Deploy on GitHub Pages

Settings -> Pages -> Source: **Deploy from a branch** -> Branch: `main`, folder: `/ (root)`.

For the custom domain, add a `CNAME` file at the root containing `terralaboratories.com`
and point the DNS A records at GitHub's Pages IPs. Do this only when you are ready to
cut over, since it will take over the apex domain.

## Editing

The HTML is generated. The generator is `build_colossal.py` in the working repo, which
holds all copy, the system index, the validation record and the source register as Python
data structures. Edit there and regenerate rather than editing `index.html` by hand.

## Content rules this site follows

- Every figure carries a reference mark (S1 to S8) resolving to the source register in section 11.
- Terra results resolve to the validation record in section 07, with run counts and conditions stated.
- Simulation results are labelled as simulation.
- No claim of a paid pilot, live deployment, award or press coverage.
- All imagery is real footage under the Pexels licence. No AI generation, no renders.
