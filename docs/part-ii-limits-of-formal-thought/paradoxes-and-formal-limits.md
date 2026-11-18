<div class="chapter-kicker">Part II / Limits of Formal Thought · Chapter 02</div>

# Paradoxes, Self-Reference & Incompleteness

<img class="chapter-cover" src="../../assets/images/paradox.svg" alt="A circular self-referential form with a central question mark">

<div class="chapter-lede">The difficulty with a paradox is not that we have found a complicated question. It is that assumptions which initially seem harmless can, together, entail a contradiction.</div>

<div class="chapter-info"><span>Foundations of mathematics</span><span>Self-reference</span><span>Proof and provability</span></div>

## 1. Why is the liar sentence a problem?

Consider the sentence:

> This sentence is false.

Call it \(L\). In an ordinary two-valued interpretation, where a sentence must be either true or false, its apparent content leads to the equivalence

\[
L \text{ is true} \;\Longleftrightarrow\; L \text{ is false}.
\]

If \(L\) is true, what it asserts holds, so it is false. If it is false, what it asserts fails to hold, so it is true. Neither straightforward assignment is stable.

The difficulty rests on more than **self-reference alone**. A sentence such as “This sentence has five words” refers to itself without generating the same contradiction. The liar combines self-reference with a truth predicate and apparently unrestricted principles linking a sentence's truth to what it says.

Philosophers and logicians have proposed different responses. **Tarski's approach** distinguishes a language from a richer *metalanguage* in which truth about the first language can be expressed. On this approach, the relevant truth predicate is not allowed to apply unrestrictedly to sentences of its own language. Other approaches modify the treatment of truth values or the logic governing contradictions. There is no universally accepted resolution to the full family of semantic paradoxes.[^liar]

The important point is not that ordinary language is worthless; it is that a rigorous theory of truth must specify **which sentences can express what about which language**.

## 2. How did Russell's paradox challenge set theory?

The problem can be derived rather than merely described. In naïve set theory, an unrestricted comprehension principle says that for any well-defined condition \(P(x)\), there is a set containing exactly the objects satisfying \(P\).

Now imagine the collection

\[
R=\{x \mid x\notin x\}.
\]

It is supposed to contain precisely the sets that are **not** members of themselves. Ask whether \(R\in R\).

- **Suppose \(R\in R\).** By the rule defining \(R\), it contains only sets that are not members of themselves. Therefore \(R\notin R\).
- **Suppose \(R\notin R\).** Then \(R\) satisfies the defining condition for membership in \(R\). Therefore \(R\in R\).

Either assumption produces its opposite. The contradiction does not show that the argument is badly executed. It shows that the unrestricted set-existence principle cannot be maintained alongside the usual classical reasoning about membership.[^russell]

### What changed after Russell?

One response is to **restrict which collections count as sets**. In standard Zermelo–Fraenkel set theory (ZF, or ZFC with the axiom of choice), separation forms subsets of an already given set; it does not license the existence of an unrestricted set of *all* objects meeting an arbitrary condition. This blocks Russell's construction as a universal set.

Other foundational approaches, including type theories, restrict the kinds of objects that may stand in membership-like relations. The variety of responses matters: the paradox does not uniquely dictate one replacement foundation.[^russell]

<div class="chapter-callout"><strong>A distinction worth keeping</strong>Russell's paradox exposes inconsistency in a particular unrestricted principle of set formation. It does not establish that modern axiomatic set theory is inconsistent.</div>

## 3. What did Gödel actually prove?

A **formal theory** specifies a language, axioms, and rules for deriving theorems. It is *consistent* if it does not prove a contradiction. It is *complete* in the relevant syntactic sense if, for every sentence \(\varphi\) in its language, it proves either \(\varphi\) or its negation.

Gödel's **first incompleteness theorem**, in a standard modern formulation, concerns theories that meet three central conditions:

1. They are **consistent**.
2. Their axioms are **effectively enumerable**: there is a computable procedure for listing them.
3. They can express enough elementary arithmetic (for example, they extend a system at least as strong as Robinson arithmetic \(Q\)).

Such a theory cannot decide every arithmetical sentence. There is a sentence \(\varphi\) for which neither \(\varphi\) nor \(\neg\varphi\) is provable within the theory. This is a limitation of what can be simultaneously secured by those conditions, not a claim that mathematical proof as such has failed.[^goedel]

### Why does arithmetic allow a statement about proofs?

The surprising move is **arithmetisation**. Symbols, formulas, and finite proofs can be encoded by natural numbers, so that claims about formal proofs become arithmetical claims. Through a diagonal or fixed-point construction, a sentence \(G\) can be made to express, in effect, that \(G\) is not provable in the theory.

A simplified line of reasoning is instructive:

- If a consistent theory proved \(G\), the encoded claim of unprovability would be false in the way the construction describes; this creates a contradiction.
- Establishing that the theory also cannot prove \(\neg G\) requires additional care. Gödel's original argument used a stronger consistency condition; later refinements, including Rosser's, obtain the familiar incompleteness conclusion from ordinary consistency under the standard effective and arithmetic assumptions.

This is a sketch of the architecture, **not** a substitute for the formal proof. The precise arithmetical predicates and assumptions are indispensable to a rigorous theorem statement.[^goedel]

### Does the theorem mean that truth exceeds proof?

For a fixed, sound formal arithmetic theory, there are true statements of arithmetic not provable **in that theory**. But the qualifiers matter. The theorem does not provide a mechanical way to recognise every arithmetical truth, nor does it license the unqualified claim that “humans can see truths no machine can”.

It is also important to separate Gödel's **incompleteness theorem for arithmetic theories** from his **completeness theorem for first-order logic**. The latter states that every logically valid first-order formula is derivable in an appropriate sound and complete proof calculus. These theorems answer different questions: one about logical consequence across models, the other about what a particular theory can decide.[^goedel]

## 4. Can a system prove its own consistency?

Gödel's **second incompleteness theorem** strengthens the result. Under suitable conditions on a consistent, effectively axiomatised theory capable of representing enough arithmetic and its own proof relation, the theory cannot prove a suitably formalised statement of its **own consistency**.[^goedel]

This does **not** mean that consistency can never be studied or supported by mathematics. A stronger theory can sometimes prove the consistency of a weaker one. Such a proof carries assumptions from the stronger theory; it does not make those assumptions disappear.

The result speaks to Hilbert's programme of grounding mathematics in secure formal procedures. It shows that an especially ambitious version of the programme cannot succeed in the simple form originally hoped for, while leaving a broad and productive role for formal proof.

## 5. Where do these results stop?

Three popular conclusions do **not** follow:

**“Everything in mathematics is undecidable.”** False. Countless mathematical statements are provable or refutable. Gödel's result guarantees *some* undecidable sentences in theories meeting the conditions above, not that ordinary calculation is impossible.

**“Self-reference always causes contradiction.”** False. It is the conjunction of specific self-referential constructions and logical or semantic assumptions that matters. Self-reference is also a powerful tool used in legitimate mathematical proofs.

**“Gödel proved that artificial intelligence or human reason has an absolute limit.”** Too broad. The incompleteness theorems address precisely specified formal theories. Arguments extending them to minds, intelligence, or computation need further philosophical and mathematical premises; the theorems alone do not establish such claims.

<div class="chapter-callout"><strong>Where the argument leads</strong>Formal rigour reveals both extraordinary power and precise limits. Paradoxes teach why the rules of a system matter. Incompleteness teaches why consistency, effective axiomatisation, expressive strength, and deductive completeness cannot all be demanded together in the relevant arithmetical setting.</div>

## Sources and further reading

- **“Liar Paradox,” *Stanford Encyclopedia of Philosophy*.** [Read the entry](https://plato.stanford.edu/entries/liar-paradox/). The semantic difficulty and major approaches to truth.
- **“Self-Reference and Paradox,” *Stanford Encyclopedia of Philosophy*.** [Read the entry](https://plato.stanford.edu/entries/self-reference/). The connections between semantic paradox, diagonalisation, and proof theory.
- **“Russell's Paradox,” *Stanford Encyclopedia of Philosophy*.** [Read the entry](https://plato.stanford.edu/entries/russell-paradox/). The contradiction and its foundational significance.
- **“Gödel's Incompleteness Theorems,” *Stanford Encyclopedia of Philosophy*.** [Read the entry](https://plato.stanford.edu/entries/goedel-incompleteness/). The theorem statements, assumptions, history, and philosophical interpretations.
- **“Set Theory,” *Stanford Encyclopedia of Philosophy*.** [Read the entry](https://plato.stanford.edu/entries/set-theory/). Axiomatic approaches to sets and logical completeness.

**Optional lecture:** [MIT OpenCourseWare — Recursion Theorem and Logic](https://ocw.mit.edu/courses/18-404j-theory-of-computation-fall-2020/resources/lecture-11-recursion-theorem-and-logic/). A more technical account of the relationship between computability and incompleteness.

[^liar]: [*Liar Paradox*](https://plato.stanford.edu/entries/liar-paradox/) and [*Self-Reference and Paradox*](https://plato.stanford.edu/entries/self-reference/), *Stanford Encyclopedia of Philosophy*.
[^russell]: [*Russell's Paradox*](https://plato.stanford.edu/entries/russell-paradox/) and [*Set Theory*](https://plato.stanford.edu/entries/set-theory/), *Stanford Encyclopedia of Philosophy*.
[^goedel]: [*Gödel's Incompleteness Theorems*](https://plato.stanford.edu/entries/goedel-incompleteness/), *Stanford Encyclopedia of Philosophy*, especially the qualified theorem statements and Rosser's refinement.
