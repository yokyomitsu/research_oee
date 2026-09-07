# OEE Theoretical Research Workspace

## Mission

This repository is a persistent research workspace for investigating theoretical principles underlying Open-Ended Evolution (OEE).

The objective is not implementation.

Do not:

* write simulation code
* implement cellular automata
* build Evoloops/Lenia hybrids
* create GUIs
* design software architectures
* treat known phenomena as discoveries

The objective is:

$$
\text{Known evidence}
\rightarrow
\text{abstraction}
\rightarrow
\text{research frontier}
\rightarrow
\text{falsifiable hypothesis}
$$

The main question is:

> Why do artificial evolutionary systems usually converge or close, while natural evolution appears capable of continually generating new evolutionary possibilities?

The research begins from:

* Evoloops
* Lenia / continuous artificial life
* Autopoiesis
* Open-Ended Evolution research
* evolutionary biology
* complex systems
* abstract lessons from modern deep learning

Deep-learning mechanisms must not be directly transplanted into artificial life. Use them only as sources of abstract structural insights.

## Fundamental distinctions

Never conflate:

* replication
* self-reproduction
* heritable variation
* Darwinian evolution
* adaptive evolution
* diversity
* novelty
* adaptive novelty
* complexity
* Open-Ended Evolution

In particular:

$$
\text{evolution} \not\Rightarrow \text{OEE}
$$

$$
\text{diversity} \not\Rightarrow \text{novelty}
$$

$$
\text{large state space} \not\Rightarrow
\text{large evolutionary possibility space}
$$

## Novelty rule

Already observed or established phenomena are evidence, not research discoveries.

A candidate hypothesis should be retained only if it is:

* not merely a renamed known concept
* not a trivial combination of known mechanisms
* apparently underexplored after prior-art search
* falsifiable in principle
* grounded in existing evidence

Do not claim "novel", "first", or "unexplored" without searching prior work.

Use cautious statuses:

* ESTABLISHED
* PARTIALLY EXPLORED
* UNDEREXPLORED
* POTENTIALLY NOVEL
* UNKNOWN

## Research style

Use:

$$
\text{generate}
\rightarrow
\text{attack}
\rightarrow
\text{eliminate}
\rightarrow
\text{refine}
$$

Prefer counterexamples over confirmation.

A hypothesis that is rejected is a successful research result.

Distinguish every important statement as:

* Fact
* Interpretation
* Hypothesis
* Speculation

Prefer primary literature.

## Central candidate question

Investigate, but do not assume:

$$
\text{OEE}
\stackrel{?}{=}
\text{endogenous transformation of the effective evolutionary possibility space}
$$

One provisional representation is:

$$
\mathcal S_t=(X_t,\mathcal O_t)
$$

with

$$
\mathcal O_t=(V_t,R_t,H_t,S_t)
$$

where:

* \(V_t\): evolutionarily relevant variables
* \(R_t\): possible relations/interactions
* \(H_t\): possible hereditary entities
* \(S_t\): possible selectable units

A strong candidate OEE condition would be:

$$
(X_t,\mathcal O_t)
\rightarrow
(X_{t+1},\mathcal O_{t+1})
$$

where \(\mathcal O_{t+1}\) enables evolutionary trajectories that were not expressible under \(\mathcal O_t\).

This is a hypothesis to attack, not an established result.

## Repository as research memory

Do not recursively reread the entire repository at the beginning of every session.

Always begin with:

1. `STATUS.md`
2. `KNOWN.md`
3. `HYPOTHESES.md`
4. `FRONTIER.md`

Read additional material only when necessary.

Stable knowledge should be aggressively compressed into `KNOWN.md`.

Uncertain reasoning should retain more detail.

Do not store long paper summaries unless necessary.

Store only research-relevant deltas:

* what the source establishes
* what it does not establish
* which hypothesis it supports or weakens
* what boundary it clarifies

## File roles

### STATUS.md

Minimal sufficient description of the current research state.

It should answer:

* What is the current central question?
* What has been established?
* What hypotheses remain active?
* What has been rejected?
* What is the highest-value unresolved question?

Keep it short.

### KNOWN.md

Canonical compressed boundary of established knowledge.

Do not put speculation here.

### HYPOTHESES.md

Maintain competing hypotheses.

Each should contain:

* claim
* status
* closest prior art
* evidence
* strongest counterexample
* falsifiable prediction
* falsification condition
* next question

Do not prematurely converge to one theory.

### FRONTIER.md

Contains unresolved questions only.

Rank questions by expected information gain.

## Research loop

Each research pass should follow:

$$
S_t
\rightarrow
Q_t
\rightarrow
R_t
\rightarrow
\Delta S
\rightarrow
S_{t+1}
$$

Operationally:

1. Read the canonical state files.
2. Select exactly one high-information frontier question.
3. Search relevant primary literature.
4. Determine the known boundary.
5. Generate or refine hypotheses only if justified.
6. Search for prior art.
7. Search for counterexamples.
8. Update `KNOWN.md` only with stable conclusions.
9. Update `HYPOTHESES.md`.
10. Update `FRONTIER.md`.
11. Rewrite `STATUS.md` as a compressed state.
12. Stop.

Do not implement anything.

## Success criteria

A research pass is useful if it does at least one of the following:

1. establishes a clearer known/unknown boundary;
2. rejects a plausible hypothesis;
3. identifies an underexplored explanatory gap;
4. derives a falsifiable hypothesis;
5. identifies a potentially missing theoretical variable;
6. compresses several known observations into a stronger general principle.

The final target is:

$$
\boxed{
\text{Known}
\rightarrow
\text{Frontier}
\rightarrow
\text{Testable Unknown}
}
$$

Implementation is outside the current scope.
