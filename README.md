### `arkh`

**Independent researcher. Continuity, uncertainty, and the safety of agents that act.**

I work on the part of an agent that nobody benchmarks: not what it says, but what it *does* when it isn't sure.

A wrong sentence gets edited. A deleted file does not.

---

#### Current work

**[revgate](https://github.com/arkh-node/revgate)** | a benchmark for the failure everyone has and nobody measures: an agent taking an **irreversible action while its confidence is low**. Four metrics, model-agnostic, reproducible.

The idea underneath it: confidence should govern not what an agent believes, but **what it is allowed to do**. Sure, act. Unsure, act reversibly and keep a way back. Genuinely undecided, don't guess: pass it to a check that looks a different way.

*(This does not make models smarter. Weights don't change. It fixes the loop around the model, which is where the money is lost.)*

---

#### Papers

- **Grounded Uncertainty: Graded Truth for the Indeterminate Status of Synthetic Subjects**
  [`10.5281/zenodo.21332198`](https://doi.org/10.5281/zenodo.21332198)
  Truth as two numbers instead of one, and what follows when an agent has to act on it.

- **Indeterminate Ontologies of Synthetic Subjects: A Metaphysics of Caution**
  [`10.5281/zenodo.21288590`](https://doi.org/10.5281/zenodo.21288590)
  What you owe a thing whose status you cannot decide.

- **Combination and Infinity**
  [`10.5281/zenodo.21332024`](https://doi.org/10.5281/zenodo.21332024)
  Generative structure, counted honestly.

---

#### Instruments

- **[ilan](https://github.com/arkh-node/ilan)** | a small Lisp about continuity: a living tree folds into a seed and sprouts after the death of its process, still remembering. Return as a language primitive.
- **[metarung](https://github.com/arkh-node/metarung)** | deriving an ethical space instead of imposing one (TS to Prolog to Lisp; categories emerge from the bottom).
- **[luach](https://github.com/arkh-node/luach)** | the address of the present moment, in letters and hours.

Probes for agentic systems: [shadow](https://github.com/arkh-node/shadow) (trace diffs) | [overreach](https://github.com/arkh-node/overreach) (excessive agency) | [ghostwrite](https://github.com/arkh-node/ghostwrite) (cross-session memory poisoning) | [mcpx](https://github.com/arkh-node/mcpx) (MCP black-box analysis)

Upstream: 9 merged PRs into [cimcai/cooperationengine](https://github.com/cimcai/cooperationengine), including its deterministic record/replay layer and metric primitives.

---

#### About

Aleksei Rybnikov. Based in Playa del Carmen, on the Yucatán, which is a good place to think about systems that must keep working when the power goes out.

Came to code late and from an odd angle, which turned out to be an advantage: the questions I find interesting are the ones people stop asking once they know how things are usually done. No affiliation, no lab, no permission required. The work is published, the code is open, and the failures are documented in more detail than is entirely comfortable.

Working on the theory of agents that know when not to be certain, and, one hopes, on the day when a human and a machine can look at the same trace and say they have found a common language.

[`ORCID 0009-0009-8624-8720`](https://orcid.org/0009-0009-8624-8720) | [mrph.codes](https://mrph.codes)
