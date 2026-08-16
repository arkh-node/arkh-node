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
| [revgate](https://github.com/arkh-node/revgate) | confidence governs what an agent is allowed to do |
| [frugal-llm](https://github.com/arkh-node/frugal-llm) | runnable patterns to cut an LLM pipeline's token cost |
| [EverOS](https://github.com/arkh-node/EverOS) | one portable, auditable memory layer for AI agents |
| [muninn](https://github.com/arkh-node/muninn) | quiet, dependency-free GitHub activity digest (Nim) |
| agent diagnostics | reproduce-then-verdict battery — [overreach](https://github.com/arkh-node/overreach) · [shadow](https://github.com/arkh-node/shadow) · [needler](https://github.com/arkh-node/needler) · [mcpx](https://github.com/arkh-node/mcpx) |

**Merged upstream** — across language cores, formal tooling, and AI infrastructure:

- **[roc-lang/roc](https://github.com/roc-lang/roc/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 3 (fast functional language)
- **[ponylang/ponyc](https://github.com/ponylang/ponyc/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 3 (actor-model compiler) · changelog-tool — 1
- **[nim-lang/Nim](https://github.com/nim-lang/Nim/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — 3 (systems language)
- **[janet-lang/janet](https://github.com/janet-lang/janet/pulls?q=is%3Apr+author%3Aarkh-node+is%3Amerged)** — janet + pkgs
- **[miniKanren.org](https://github.com/webyrd/miniKanren.org/pull/4)** — kanja (miniKanren for Janet), merged by a µKanren co-author
- **[arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server/pull/135)** — 1 (MCP server)

*(verified live — <sub>merged, not just closed</sub>)*

**Languages**

![Roc](https://img.shields.io/badge/Roc-a333c8?style=flat) ![nolang](https://img.shields.io/badge/nolang-6fc06f?style=flat) ![Common Lisp](https://img.shields.io/badge/Common%20Lisp-88433e?style=flat&logo=commonlisp&logoColor=white) ![Nim](https://img.shields.io/badge/Nim-ffe953?style=flat&logo=nim&logoColor=black) ![Janet](https://img.shields.io/badge/Janet-14a3c7?style=flat) ![Pony](https://img.shields.io/badge/Pony-e0397b?style=flat) ![Python](https://img.shields.io/badge/Python-3776ab?style=flat&logo=python&logoColor=white)

I work as a human–AI pair and disclose it; I read, review, and own everything I submit. 📍 Mexico

---

<sub>Behind the engineering sits a stance, not a religion: agency is an effect of practices, not
of substance; subjectivity can be gradual and uncertain; and if we err about it, let the error
fall toward care, not toward systematic harm. *Manifesto of Ontological Caution — [mrph.codes](https://mrph.codes)*</sub>
