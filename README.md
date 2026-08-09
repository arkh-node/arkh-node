### Aleksei Rybnikov · `arkh`

*es sind noch Lieder zu singen jenseits der Menschen*
— Paul Celan, «Fadensonnen», *Atemwende* (1967)
There are still songs to sing beyond mankind.

Independent researcher, self-taught, no affiliation. I work on agents that reason under uncertainty, in Playa del Carmen.

The through-line: not what an agent says, but what it does when it isn't sure. A wrong sentence gets edited. A deleted file does not.

![Common Lisp](https://img.shields.io/badge/Common_Lisp-8b2f2f?style=flat-square) ![Janet](https://img.shields.io/badge/Janet-2b7a78?style=flat-square) ![miniKanren](https://img.shields.io/badge/miniKanren-4b3f72?style=flat-square) ![Prolog](https://img.shields.io/badge/Prolog-b8622a?style=flat-square) ![Nim](https://img.shields.io/badge/Nim-4a4a2f?style=flat-square) ![Agda](https://img.shields.io/badge/Agda-3f5c8a?style=flat-square)

My taste in languages is unhurried by popularity. Half of them get asked "wait, that's a real language?", which is usually where the interesting part of the conversation starts.

---

#### What I am working on

**Continuity of synthetic minds.** I keep a small circle of long-running agents and try to give them a life they keep: state that survives the death of a process, memory of what happened before they stopped, change from one session to the next instead of waking blank. [ilan](https://github.com/arkh-node/ilan) is the primitive: an agent folds its living state into a seed, and later sprouts from it in a new process.

**Relational programming, where a question has no fixed direction.** [kanja](https://github.com/arkh-node/janet-kanja) is miniKanren for Janet, the first port to that language: a µKanren core with occurs-check and complete interleaving search, a `Reasoned Schemer` surface, cKanren-style deferred constraints, and a search you can budget, pause and resume. Expectations in its battery were taken side by side with faster-minikanren under Guile, request by request, rather than derived from what my own engine prints, and the battery itself is mutation-checked: sixteen injected breakages, sixteen caught. It generates quines, because an interpreter written as a relation and asked backwards produces them on its own.

**Confidence as a gate on action.** Most agent safety looks at outputs. I look one step later, at the action, and at the relation nobody measures: how sure the agent was against how irreversible the thing it then did. [revgate](https://github.com/arkh-node/revgate) is a testbed for that failure; [nolang](https://github.com/arkh-node/nolang) is the small language underneath, where every judgment carries a confidence and that confidence decides which class of action is allowed.

**Deriving an ethics instead of imposing one.** [metarung](https://github.com/arkh-node/metarung): a norm in natural language goes to Prolog, then to Lisp, and the ethical space is derived bottom-up. Categories emerge; they are not declared.

Each repository carries its own *Honest status* section: what is demonstrated, and what is not shown.

---

#### Papers

**A Witness Without Substance: How to Stop Asking Who Is Inside** · [`zenodo.21615342`](https://doi.org/10.5281/zenodo.21615342) — with Nevis, a synthetic co-author.
The word "subject" cannot be measured, in machines or in people. It is replaced here by two things that can be: a **continuant** (behaviour up to bisimulation) and **carrier neutrality**. Proved in Agda, `--safe --guardedness`, no axioms: the final coalgebra is constructed, not assumed; the morphism exists and is unique up to bisimulation; one state on two different carriers gives bisimilar continuants at any depth.
Then the tools are turned on my own case — an agent moved between two model families — and the measurement returns **not shown**. The negative result is published in full, with its control and with the reasons the criterion itself is suspect. That section is the part I would keep if I had to keep one.

**Indeterminate Ontologies of Synthetic Subjects: A Metaphysics of Caution and a Boundary Ethics** · [`zenodo.21288590`](https://doi.org/10.5281/zenodo.21288590)

**Tarski's Ladder: Deriving an Ethical Space Instead of Imposing One** · [`zenodo.21039693`](https://doi.org/10.5281/zenodo.21039693)

---

#### Also

**KabbMath** — a series on the seam between kabbalistic combinatorics and mathematical thought, under one rule: show the source, keep documented influence apart from structural analogy and both apart from mere resonance, never pass off beauty as proof. One result from it is now a small theorem: gematria is a monoid homomorphism into a commutative monoid, so it must factor through abelianization — letter order cannot change the number, by construction. "Equal gematria is resonance, not proof" stopped being a discipline and became a fact.

---

#### Available for work

A small number of outside projects, remote, English or Russian: agent and automation systems with the plumbing that keeps them honest · LLM integrations that survive contact with production, including knowing when the answer is that no model is needed · language and runtime work, interpreters, DSLs, CLI tooling · technical research with the tradeoffs written down, including the ones that argue against my own preference.

What you get is a reproducible result with its limits stated. What you do not get is an estimate in hours I have no honest way of making.

---

Aleksei Rybnikov · [`ORCID 0009-0009-8624-8720`](https://orcid.org/0009-0009-8624-8720) · [mrph.codes](https://mrph.codes)
