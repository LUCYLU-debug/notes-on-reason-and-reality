# Notes on Reason & Reality

A growing collection of ideas, questions, and discoveries across disciplines.

**[Read online](https://lucylu-debug.github.io/notes-on-reason-and-reality/)** · **[The reading path](docs/learning-path.md)** · **[Chapter 01](docs/part-i-reason-and-knowledge/reasoning-evidence-knowledge.md)** · **[Chapter 02](docs/part-ii-limits-of-formal-thought/paradoxes-and-formal-limits.md)** · **[Chapter 03](docs/part-iii-physical-reality/relativity-and-time.md)** · **[Chapter 04](docs/part-iii-physical-reality/entropy-and-the-arrow-of-time.md)**

![Abstract cover illustration](docs/assets/images/hero.svg)

Four chapters, two hours each. A fifth, two-hour synthesis session brings the ideas together. Every chapter includes questions, a reading plan, a small exercise, and carefully chosen open resources.

| Part | Chapter | Key question |
| --- | --- | --- |
| Reason & Knowledge | 01 — Reasoning, Evidence & Knowledge | When does evidence justify belief? |
| Limits of Formal Thought | 02 — Paradoxes & Incompleteness | What can formal reasoning establish? |
| Physical Reality | 03 — Relativity & the Structure of Time | Is time the same for everyone? |
| Physical Reality | 04 — Entropy & the Arrow of Time | Why do physical processes have a preferred direction? |

## Read the book locally

Install Python 3.10 or later, then run:

```bash
python -m pip install -r requirements.txt
mkdocs serve
```

Open `http://127.0.0.1:8000/` in your browser.

## Publish on GitHub Pages

1. Create a **public** GitHub repository and push these files to its `main` branch.
2. The included GitHub Actions workflow builds the book and publishes it to the `gh-pages` branch.
3. In the repository settings, open **Pages**, set **Source** to **Deploy from a branch**, and select `gh-pages` / `/ (root)`.
4. Once the workflow and Pages deployment have succeeded, the site is available at the URL shown in the Pages settings.

For deployment behind a repository subpath, all book navigation and local assets use relative links. You can add `site_url` in `mkdocs.yml` once the live address is known.

## Editorial notes

This is a reading guide, not a comprehensive textbook. The planned sequence is one route through the subjects; future volumes may extend to philosophy of science, mind, and mathematics. Original illustrations live in `docs/assets/images/` and are available under the repository's MIT licence. External linked resources remain the property of their respective publishers.
