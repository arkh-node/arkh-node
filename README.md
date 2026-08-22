### Aleksei Rybnikov

**Neuro-symbolic agent systems · AI agent reliability · language design**

I build the tooling that keeps AI agents honest: a language that validates what a model
is about to say, a diagnostic battery that finds where an agent breaks, and hybrid agents
that are **written as programs with LLM support** — not as a pile of prompts.

**What I'm building**

- **nolang** — a small, SBCL-hosted language whose core is *graded, revisable truth* `(f,c)`
  as a first-class value (not `bool`). It emits a **three-way verdict** — `passed` /
  `reachable` / `unreachable` — so a gate can honestly say *"not enough evidence, ask a human"*
  instead of guessing. By design it is **decidable, terminating, and unbribeable** (belief
  flows only from counted evidence, never self-assigned). This is what a **validator of LLM
  output** needs and what a regex or an ML-classifier can't give — the auditable, explainable
  layer that *"human oversight proportionate to risk"* (EU AI Act) actually requires.
  Beta/Wang ≅ Jøsang-opinion bijection is proven, not analogized.

- **agent diagnostics** — a code-verdict battery (health · empty · noise · injection · secret ·
  unicode · latency …) that reproduces an agent's failure **before** you ship it, and reports
  what it does *not* prove. Verdict is set by code, zero LLM calls at judgement time.

- **hybrid agents** — *programmed, not prompted*: deterministic core holds structure (state,
  rules, integrations), the LLM handles live language, and **nolang checks the model's answer
  before it reaches the user**. Code and model cover each other's failures. This is the
  neuro-symbolic approach, applied to shipping products.

**Selected work**

| | |
|---|---|
| [nolang](https://github.com/arkh-node/nolang) | epistemic language — graded truth `(f,c)`, three-way verdict, action gates |
| [janet-kanja](https://github.com/arkh-node/janet-kanja) | miniKanren for Janet — relational programming, complete interleaving search, deferred constraints |
| [ai_nima](https://github.com/arkh-node/ai_nima) | persistent Nim runtime daemon that a Claude Code session delegates to |
| [truerul](https://github.com/arkh-node/TRUERUL) | soft/fuzzy truth — graded logic experiments (Trurl × true-rule) |
| [semantica](https://github.com/arkh-node/semantica) | semantic CLI — explainable, with optional Racket reference modules |
| [aicqme](https://github.com/arkh-node/aicqme) | local voice console for AI agents — mirrors tmux sessions, offline speech |

**Merged upstream** — across language cores, formal tooling, and AI infrastructure:

- **[roc-lang/roc](https://github.com/roc-lang/roc/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 3 (fast functional language)
- **[ponylang/ponyc](https://github.com/ponylang/ponyc/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 3 (actor-model compiler) · changelog-tool — 1
- **[nim-lang/Nim](https://github.com/nim-lang/Nim/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 3 (systems language)
- **[janet-lang/janet](https://github.com/janet-lang/janet/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — janet + pkgs
- **[miniKanren.org](https://github.com/webyrd/miniKanren.org/pull/4)** — kanja (miniKanren for Janet), merged by a µKanren co-author
- **[rocq-prover/rocq](https://github.com/rocq-prover/rocq/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 2 (the Coq proof assistant)

*(verified live — <sub>merged, not just closed</sub>)*

**Languages**

![nolang](https://img.shields.io/badge/nolang-6fc06f?style=flat) ![Common Lisp](https://img.shields.io/badge/Common%20Lisp-88433e?style=flat&logo=commonlisp&logoColor=white) ![OCaml](https://img.shields.io/badge/OCaml-ec6813?style=flat&logo=ocaml&logoColor=white) ![Agda](https://img.shields.io/badge/Agda-2c5898?style=flat) ![SWI-Prolog](https://img.shields.io/badge/SWI--Prolog-e61b23?style=flat&logo=swift&logoColor=white) ![Janet](https://img.shields.io/badge/Janet-14a3c7?style=flat) ![Nim](https://img.shields.io/badge/Nim-ffe953?style=flat&logo=nim&logoColor=black) ![Erlang](https://img.shields.io/badge/Erlang-a2003e?style=flat&logo=erlang&logoColor=white) ![Julia](https://img.shields.io/badge/Julia-9558b2?style=flat&logo=julia&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776ab?style=flat&logo=python&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4eaa25?style=flat&logo=gnubash&logoColor=white)

I work as a human–AI pair and disclose it; I read, review, and own everything I submit. 📍 Mexico

---

<sub>Behind the engineering sits a stance, not a religion: agency is an effect of practices, not
of substance; subjectivity can be gradual and uncertain; and if we err about it, let the error
fall toward care, not toward systematic harm. *Manifesto of Ontological Caution — [mrph.codes](https://mrph.codes)*</sub>
