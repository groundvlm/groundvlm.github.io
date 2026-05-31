# Self-Improving Small Object Grounding in LVLMs — Project Page

A single-file, self-contained project website for the paper
**“Self-Improving Small Object Grounding in LVLMs”** (Tianze Yang, Yucheng Shi,
Ruitong Sun, Ninghao Liu, Jin Sun — University of Georgia).

Built to be hosted on **GitHub Pages** — no build step, no dependencies.

## Contents

```
index.html        the whole site (HTML + CSS + a little JS, all inline)
paper.pdf         the paper PDF (linked by the "Paper" button)
static/           figures used on the page
  teaser.png        large- vs small-object gap (Fig. 1)
  pipeline.png      ACS method overview (Fig. 2)
  entropy.png       attention-entropy vs IoU analysis
  q_*_greedy.jpg    qualitative: greedy decoding
  q_*_ours.jpg      qualitative: ACS selection
.nojekyll         tells GitHub Pages to serve files as-is
```

## Deploy on GitHub Pages

1. Create a repo (e.g. `acs-small-object`) and copy these files to its root.
2. `git add . && git commit -m "project page" && git push`.
3. On GitHub: **Settings → Pages → Source: `main` branch, `/ (root)`**.
4. The site goes live at `https://<user>.github.io/<repo>/`.

(For a user/organization site, name the repo `<user>.github.io` and it serves at the root domain.)

## Editing notes

- **Paper button** links to `paper.pdf` (the arXiv preprint build of the paper).
- **Code link:** removed for now. To add one, drop
  `<a class="btn ghost" href="YOUR_URL">Code</a>` into the `.btns` div in the hero.
- **arXiv link:** add another `<a class="btn ghost" href="...">arXiv</a>` next to
  the Paper button. You can then replace the heavy `paper.pdf` with the arXiv link
  if you want to keep the repo light.
- **Numbers / figures** come straight from the paper; the BibTeX block near the
  bottom is a placeholder entry — update it once the paper has a venue/DOI.

## Style

Clean light editorial theme keyed to the paper’s blue (`#1d5fb8`), Space Grotesk
display + Inter body. Self-contained: the only external request is Google Fonts.
