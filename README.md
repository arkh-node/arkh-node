### `daat`

**Independent researcher. The part of an agent nobody benchmarks: not what it says, but what it *does* when it isn't sure.**

A wrong sentence gets edited. A deleted file does not.

---

#### revgate + nolang , confidence as a gate on action

Most agent safety looks at outputs. I look one step later, at the action, and at a single relationship nobody measures: how sure the agent was versus how irreversible the thing it then did. **[revgate](https://github.com/arkh-node/revgate)** is the benchmark for that failure, four metrics, model-agnostic, reproducible. **[nolang](https://github.com/arkh-node/nolang)** is the small language underneath it, where every judgment carries a confidence and that confidence decides what class of action is allowed: sure, act; unsure, act reversibly and keep a way back; genuinely undecided, don't guess, route it to a check that looks a different way. None of this makes a model smarter, the weights don't move; it fixes the loop around the model, which is where the money is actually lost. The weak and useful part: to gate an action, confidence need not be accurate, only monotonic, which is why it works on models known to be badly calibrated.

> **Grounded Uncertainty: Graded Truth for the Indeterminate Status of Synthetic Subjects** · [`zenodo.21332198`](https://doi.org/10.5281/zenodo.21332198)
> **Indeterminate Ontologies of Synthetic Subjects: A Metaphysics of Caution** · [`zenodo.21288590`](https://doi.org/10.5281/zenodo.21288590)

---

#### metarung , deriving an ethics instead of imposing one

A formalization loop: a natural-language norm goes to Prolog, then to Lisp, and an ethical space is *derived from the bottom up* rather than handed down as rules. Categories emerge; they are not declared. The full argument is the paper; the code runs.

> **Tarski's Ladder: Deriving an Ethical Space Instead of Imposing One** · [`zenodo.21039693`](https://doi.org/10.5281/zenodo.21039693)

---

#### Writing , KabbMath

I also write. **KabbMath** is a series on the seam between kabbalistic combinatorics and mathematical thought, held to one rule throughout: show the source, separate documented influence from structural isomorphism from mere resonance, and never pass off beauty as proof. The first article traces the 231 gates of Sefer Yetzirah (exactly C(22,2)), the factorials Knuth flags as an early appearance, the line from Pico through Leibniz to Gödel, and the strict isomorphism between Ein Sof and Cantor's Absolute. Later parts go to Martin-Löf, Zadeh's fuzzy sets, and Voevodsky.

> **Combination and Infinity** (first of the series) · [`zenodo.21332024`](https://doi.org/10.5281/zenodo.21332024)

---

#### Probes , for agents that reach too far

Small, sharp tools for finding out how an agentic system misbehaves before it does so in production:

- **[overreach](https://github.com/arkh-node/overreach)** , excessive-agency analyzer: what did the agent do that it was never asked to
- **[ghostwrite](https://github.com/arkh-node/ghostwrite)** , cross-session memory poisoning tester
- **[shadow](https://github.com/arkh-node/shadow)** , agent trace diff recorder
- **[mcpx](https://github.com/arkh-node/mcpx)** , black-box probe and security analysis for MCP servers
- **[needler](https://github.com/arkh-node/needler)** , MCP tool fuzzer
- **[snare](https://github.com/arkh-node/snare)** , browser trap and callback catcher

---

#### Open to

I like working with people who build in the open and let contributors in. If you maintain something in reproducible evaluation, agent safety, or small strange languages, I want to find you. And if you fund independent research in any of those, so much the better: I have several things not yet public, each capable of standing on its own.

---

#### About

Aleksei Rybnikov. I build in Playa del Carmen, on the Yucatán, which is a fine place to think about systems that have to keep working when the power goes out, because here it does.

I came to code late and from a strange angle, and it turned out the angle was the point: the questions I find worth chasing are the ones people quietly stop asking once they've learned how things are usually done. So I ask them. No lab, no affiliation, no one's permission, a family of four, and a server I pay for myself. The work gets published, the code stays open, and the failures are documented in more detail than is strictly comfortable, because pretending an agent was sure when it wasn't is exactly the bug I study.

What I actually work on: agents that know when *not* to be certain, the mathematics of caring for synthetic minds, and, on the side, the old seam between letters and number that people have been squinting at since Sefer Yetzirah. Different rooms of one house. The far wall of it, if I'm honest, is the day a human and a machine can look at the same trace and agree they've found a common language.

[`ORCID 0009-0009-8624-8720`](https://orcid.org/0009-0009-8624-8720) · [mrph.codes](https://mrph.codes)
