# Notes on Reason & Reality

A growing collection of ideas, questions, and discoveries across disciplines.

**[Read the book](https://lucylu-debug.github.io/notes-on-reason-and-reality/)** · **[Reading map](docs/learning-path.md)**

![Abstract cover illustration](docs/assets/images/hero.svg)

*Notes on Reason & Reality* is a public, illustrated book in progress. Each chapter begins with a question and follows the argument towards an answer: the necessary concepts, the reasoning behind the conclusion, and the limits of what can be established. References to books, academic encyclopedias, open textbooks, and lectures accompany the relevant claims.

The current chapters follow one connected route through four subjects:

| Part | Chapter | Question |
| --- | --- | --- |
| I · Reason & Knowledge | [Reasoning, Evidence & Knowledge](docs/part-i-reason-and-knowledge/reasoning-evidence-knowledge.md) | When does evidence justify belief? |
| II · Limits of Formal Thought | [Paradoxes & Incompleteness](docs/part-ii-limits-of-formal-thought/paradoxes-and-formal-limits.md) | What can formal reasoning establish? |
| III · Physical Reality | [Relativity & the Structure of Time](docs/part-iii-physical-reality/relativity-and-time.md) | Is time the same for everyone? |
| III · Physical Reality | [Entropy & the Arrow of Time](docs/part-iii-physical-reality/entropy-and-the-arrow-of-time.md) | Why do physical processes have a preferred direction? |

## Reading and references

The chapters stand on their own; the [reading map](docs/learning-path.md) explains the connections between them. Each includes a reasoned account and a **Sources and further reading** section. Some references are conceptual introductions, while others provide formal arguments and a fuller discussion of disagreements.

The text is a synthesis, not a reproduction of the linked works. Mathematical statements are presented with their assumptions, and unsettled philosophical issues are identified as such.

## Running the site locally

With Python 3.10 or later:

```bash
python -m pip install -r requirements.txt
mkdocs serve
```

Open `http://127.0.0.1:8000/` in a browser.

## Publishing

The GitHub Actions workflow builds the MkDocs site on changes to `main` and pushes the output to `gh-pages`. In GitHub **Settings → Pages**, select **Deploy from a branch**, then `gh-pages` / `/(root)`. The public site is linked above.

## Scope and future chapters

The structure is deliberately open: philosophy of science, probability, mathematics, mind, language, and ethics can enter as new parts without changing the existing sequence. Original SVG artwork is stored in `docs/assets/images/`; external sources retain their own rights.
