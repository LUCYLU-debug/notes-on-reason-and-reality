# Notes on Reason & Reality

A growing collection of ideas, questions, and discoveries across disciplines.

**[Read the book](https://lucylu-debug.github.io/notes-on-reason-and-reality/)** · **[Reading map](docs/learning-path.md)**

![Abstract cover illustration](docs/assets/images/hero.svg)

*Notes on Reason & Reality* is a public, illustrated book in progress. Each chapter begins with a question and follows the argument towards an answer: the necessary concepts, the reasoning behind the conclusion, and the limits of what can be established. References to books, academic encyclopedias, open textbooks, and lectures accompany the relevant claims.

The book follows a connected route from the grounds of knowledge and the physical world to questions about agency, technology, money, and meaning:

| Part | Chapter | Question |
| --- | --- | --- |
| I · Reason & Knowledge | [Reasoning, Evidence & Knowledge](docs/part-i-reason-and-knowledge/reasoning-evidence-knowledge.md) | When does evidence justify belief? |
| II · Limits of Formal Thought | [Paradoxes & Incompleteness](docs/part-ii-limits-of-formal-thought/paradoxes-and-formal-limits.md) | What can formal reasoning establish? |
| III · Physical Reality | [Relativity & the Structure of Time](docs/part-iii-physical-reality/relativity-and-time.md) | Is time the same for everyone? |
| III · Physical Reality | [Entropy & the Arrow of Time](docs/part-iii-physical-reality/entropy-and-the-arrow-of-time.md) | Why do physical processes have a preferred direction? |
| IV · Mind & Agency | [Attention, Energy & the Ordinary Day](docs/part-iv-mind-and-agency/attention-energy-and-the-ordinary-day.md) | Why can a good routine feel exhausting? |
| IV · Mind & Agency | [Identity, Acceptance & Change](docs/part-iv-mind-and-agency/identity-acceptance-and-change.md) | How can self-honesty and growth coexist? |
| V · Intelligence & Judgement | [Thinking With AI Without Giving Up Judgement](docs/part-v-intelligence-and-judgement/ai-and-independent-thought.md) | How can AI assist thought without replacing independent judgement? |
| VI · Freedom & Meaning | [Compounding, Risk & Financial Freedom](docs/part-vi-freedom-and-meaning/compounding-risk-and-financial-freedom.md) | How does long-term saving become freedom of choice? |
| VI · Freedom & Meaning | [Meaning & the Ordinary Life](docs/part-vi-freedom-and-meaning/meaning-and-the-ordinary-life.md) | How do larger purposes enter ordinary days? |

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

The structure remains open. New essays connect questions about everyday life to psychology, economics, AI and philosophy without conflating physical laws with moral claims. Future subjects may include language and ethics. Original SVG artwork is stored in `docs/assets/images/`; external sources retain their own rights.
