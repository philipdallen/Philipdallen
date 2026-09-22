# Philip Allen

I design and run AI-assisted engineering projects — and the program-level workflows,
guardrails, and delivery tracking that keep them honest.

**Saratoga Springs, NY** · Open to **AI Operations**, **AI Workflow Designer**, and
**AI Technical Program Manager** roles.

[LinkedIn](https://linkedin.com/in/allenpd) · philip.d.allen@gmail.com

---

## What I actually do

I build research projects where AI agents produce most of the code, and I treat the
hard part as making that output *trustworthy* rather than merely fast. That means gates
that tell a real result apart from a broken instrument, metrics that housekeeping cannot
move, and a decision log that survives review.

Five public repositories, all built in 2026 under my direction with agentic AI tooling.
Each one solves a different part of the same problem: **how do you run work that an agent
mostly executes, and still be able to stand behind its results?**

---

## The projects

### Maith — [philipdallen/Maith](https://github.com/philipdallen/Maith)

A Lean 4 pipeline that extracts a canonical semantic intermediate representation from
formal mathematics, and tests whether training language models on it helps. It is also my
longest-running experiment in directing agentic coding workflows.

The pipeline and corpus builder are the mature parts; the axiom-discovery search on top is
the active frontier. When an earlier round of results did not survive stricter gates, I
withdrew them under a documented reset notice rather than let them stand — that retraction
is part of the repository's history, on purpose.

### PleaNP — [philipdallen/PleaNP](https://github.com/philipdallen/PleaNP)

A Lean 4 / Mathlib formalization of the P vs NP barrier landscape, and the integrity gates
that keep AI-assisted proof search honest.

The oracle substrate (`P^A ⊆ NP^A`, both directions) and the BGS diagonalization module are
machine-checked with zero `sorry`. Relativization is rendered as a frozen statement with two
tracked `sorry`s, and natural proofs exists as statement specifications — scoped, not claimed
as complete. The gates exist because a proof assistant will happily accept a proof of the
wrong statement, and an agent will happily produce one.

### ephapse — [philipdallen/ephapse](https://github.com/philipdallen/ephapse)

Probing open-weight model internals — activations and sparse-autoencoder features — for
cross-domain co-activation, as a candidate generator for mathematical hypotheses.

Its distinguishing feature is a two-tier validation layer built to separate **instrument
failure from phenomenon absence**. When the probe returned a clean null at 70M parameters,
that layer is what made the null reportable instead of ambiguous. A rigorous negative
result is a result.

### rubato — [philipdallen/rubato](https://github.com/philipdallen/rubato)

An executable, AI-native music format: a score, an interpretive prompt, and a plaintext
rights manifest. A deterministic player is the free baseline; an LLM player performs the
work inside the authored interpretive space.

The design point is that "interpretation" is a first-class, authorable object rather than
something left to a model's discretion — and that the deterministic path always exists as
a reproducibility anchor.

---

## Delivery and operations

### HuB — [philipdallen/HuB](https://github.com/philipdallen/HuB) · [live dashboard](https://philipdallen.github.io/HuB/)

A read-only static dashboard that aggregates cross-repo delivery status from the four
research repositories above, with a documented readiness framework and scheduled per-repo
automation.

This is the operations artifact: it reads each project's status log, renders readiness and
flow, and is checked daily by a monitoring job that files an issue when the public artifact
breaks. Field definitions live in a versioned contract, because I learned the hard way that
a metric without a stated definition will eventually be moved by something that has nothing
to do with the project it claims to measure.

---

## How I work

**Definitions before measurement.** Every published metric has a written definition, an
owner, and a change process. If a definition changes, it is recorded and the discontinuity
is visible — history is append-only and never edited to look better.

**A check that cannot fail is not a check.** Monitoring and validation code ships with a
self-test that proves each check fails on deliberately broken input.

**Negative results are published.** A rigorous null is a finding. So is a retraction.

**Honest about the tooling.** These repositories were built with agentic AI doing most of
the code production, under my direction and review. I think that is the interesting part,
not something to obscure: the skill on display is designing the workflow, the guardrails,
and the verification — not typing every line.

---

*All five repositories are 2026 – present.*
