# Q007 — Meta-evolution closure

2026-09-07. Exactly one theoretical research pass. Research question: what, if anything, prevents the evolution of evolvability from becoming another closed or convergent process? No implementation and no complete OEE theory.

## 1. Known boundary

**Fact / ESTABLISHED:** Evolution of evolvability is already a recognized OEE category. The York classification treated it as one kind of ongoing adaptive novelty; the later Tokyo categories identify **Type 2 OEE** with the ongoing evolution of evolvability, alongside Type 1 new entities/interactions, Type 3 major transitions, and Type 4 semantic evolution. The terminology is not perfectly stable: the first 2019 special-issue editorial used “Type 1d” for evolution of evolvability under the York list, while the Tokyo revision flattened and relabeled the categories. [Taylor et al. 2016](https://doi.org/10.1162/ARTL_A_00210), [Packard et al. 2019](https://doi.org/10.1162/artl_a_00291), [Channon 2024](https://doi.org/10.1162/artl_a_00430)

**Fact:** Existing prior art includes evolution of mutation rates, recombination, genetic operators, genotype–phenotype/developmental maps, modularity, capacitance, regulatory systems, autoconstructive evolution, and major transitions. These mechanisms can alter the production or transmission of heritable variation, the selectable unit, or the distribution of phenotypic outcomes. They establish that evolvability can evolve; they do not establish that evolvability must continue evolving indefinitely.

**Interpretation:** The known boundary is therefore:

\[
\text{one heritable increase or change in evolvability}
\neq
\text{ongoing evolution of evolvability}.
\]

The second is a trajectory-level hallmark, not yet a general generating principle.

## 2. One-off versus ongoing meta-evolution

**Fact:** Taylor et al. explicitly state that one instance of the evolution of evolvability falls short of genuinely open-ended evolution, just as one adaptation or one major transition does. [Taylor et al. 2016](https://doi.org/10.1162/ARTL_A_00210)

**Interpretation:** A one-off event establishes only that the current evolutionary organization can reach a state with altered future variation or adaptation. Ongoing Type 2 requires repeated, historically later changes in the mechanisms that determine future evolvability, with the changes remaining heritable, selectable, and reconstructible at the relevant level.

An operational distinction is:

\[
M_t\to M_{t+1}
\]

for one altered variation/development/inheritance map, versus a sustained sequence

\[
M_t\to M_{t+1}\to M_{t+2}\to\cdots
\]

in which later changes alter the class or organization of transformations available to produce still later changes. The latter is not supplied by a single modifier, a single exaptation, or a single major transition.

## 3. The regress question

**Fact:** The regress is explicitly recognized in meta-genetic programming. Edmonds proposed co-evolving the operators that act on a base population; the operators themselves still require operators for their evolution. His framework allowed additional operator populations, including populations acting on themselves. Spector et al. describe this as a potential regress and distinguish recursive strategies from autoconstructive evolution. [Edmonds 2001](https://journals.tubitak.gov.tr/elektrik/vol9/iss1/2/), [Spector 2001](https://faculty.hampshire.edu/lspector/pubs/ace.pdf)

**Interpretation:** The regress is coherent as a question about the causal organization of variation, but the strong claim

\[
E_n\text{ is bounded unless }E_{n+1}\text{ exists}
\]

is not established. A finite organization can encode an operator that acts on descriptions of operators, or can let organisms construct their own offspring. Conversely, a system can contain self-reference or several meta-levels and still converge.

The literature therefore supports neither an infinite hierarchy as a necessary condition nor a finite recursive closure as a sufficient condition.

## 4. Self-reference

**Fact:** Pavlic et al. define self-referencing cellular automata in which state feedback helps determine the iteration rules. Adams et al. later studied state-dependent rule dynamics of the form

\[
r_o(t+1)=f(s_o(t),r_o(t),s_e(t)).
\]

They report state-dependent dynamics as a scalable mechanism for their formal definitions of unbounded evolution and innovation. [Pavlic et al. 2014](https://arxiv.org/abs/1405.4070), [Adams et al. 2017](https://www.nature.com/articles/s41598-017-00810-8)

**Fact:** In Adams et al.'s framework, the environment is not incidental. Unbounded evolution and innovation are defined relative to an isolated counterfactual and require extrinsic perturbation of the subsystem. The authors explicitly exclude closed self-referential systems studied by Pavlic et al. from their UE result, and state that a non-self-referential external rule modulation can also produce their formal conditions, although it is less scalable under their definition.

**Counterexamples and limits:**

- Self-reference is not sufficient: closed self-referential dynamics can remain recurrent or fail the formal unboundedness criterion.
- Self-reference is not necessary for the Adams et al. UE/innovation criterion: external rule modulation and stochastic rule mutation are alternative cases.
- Self-reference can move closure from the current rule (r_t) to the fixed transformation (f). The state-dependent rule is still generated by a specified meta-function and, in the cellular-automaton study, by a restricted rule space.
- Unbounded state novelty under state-dependent rules is not automatically adaptive meta-evolution; Adams et al. do not show Darwinian selection repeatedly creating new classes of evolutionary operators.

**Conclusion:** Self-reference is a candidate enabling relation for state-dependent dynamics, not a sufficient or necessary theory of ongoing Type 2 OEE.

## 5. Fixed meta-rule problem

Consider:

\[
r_{t+1}=F(r_t,x_t).
\]

**Fact:** Existing formal state-dependent models retain a fixed rule-update scheme (F), and often a fixed finite rule representation. Autoconstructive and meta-genetic-programming systems likewise rely on a fixed programming language, interpreter, selection loop, or code-manipulation substrate even when the encoded reproduction and variation procedures evolve. [Adams et al. 2017](https://www.nature.com/articles/s41598-017-00810-8), [Edmonds 2001](https://journals.tubitak.gov.tr/elektrik/vol9/iss1/2/), [Spector 2001](https://faculty.hampshire.edu/lspector/pubs/ace.pdf)

**Interpretation:** Changing (r_t) under fixed (F) can be genuine evolution of an effective rule, but it does not by itself demonstrate that the meta-space of possible rule changes has changed. It may produce:

\[
r_t\neq r_{t+1},\qquad F_t=F_{t+1},
\]

with ongoing state novelty but no ongoing evolution of the evolutionary machinery. This is a decisive counterexample to the implication:

\[
\text{changing effective rules}\Rightarrow\text{ongoing meta-evolution}.
\]

At the same time, demanding that (F) itself change at every step merely recreates the regress. Existing work avoids that regress pragmatically by embedding variation in the evolving entities or by allowing recursive operator application; it does not provide a generally accepted observer-independent criterion for when the resulting operator is genuinely new.

## 6. Evolved open-endedness

**Fact:** Pattee and Sayama define **evolved open-endedness (EOE)** as treating open-endedness, including its mechanisms, as an outcome of evolution rather than as a pre-existing property of the whole evolutionary system. They identify symbolic genetic control and new organizational hierarchies as historical mechanisms that increased expressive and constructive capacity. They propose taxonomies, quantitative degrees, modeling of meta-level adaptation, and study of selection for or against open-endedness. [Pattee & Sayama 2019](https://doi.org/10.1162/artl_a_00276)

**Fact:** The paper does not give a scalar open-endedness objective or a necessary-and-sufficient criterion for repeated increases. It explicitly notes that all domains and environments have lawful limits, that apparent open-endedness depends on temporal and spatial scope, and that even a highly diverse lichen lineage does not provide evidence of continuous open-ended novelty over its long history.

**Interpretation:** EOE explains the historical transition from a less expressive evolutionary organization to one with more mechanisms for producing novelty. It does not explain why those mechanisms cannot later stabilize, become entrenched, or exhaust their effective operator repertoire. EOE is therefore a research orientation and historical claim, not a solution to the closure problem.

## 7. Fixed microphysics / emergent operators

**Fact:** Existing biological theory permits fixed underlying physical laws while effective evolutionary organization changes. Conserved molecular and cellular core processes can be redeployed through evolved regulatory, developmental, and organizational controls. Pattee and Sayama make the related point that a finite material alphabet can support highly varied constructions through evolved symbolic control. Major-transition theory describes new levels of individuality and inheritance without requiring changes to microphysics. [Gerhart & Kirschner 1998](https://pmc.ncbi.nlm.nih.gov/articles/PMC33871/), [Pattee & Sayama 2019](https://doi.org/10.1162/artl_a_00276), [Szathmáry 2015](https://doi.org/10.1073/pnas.1421398112)

Thus the following is compatible with existing theory:

\[
\text{microphysics fixed},\qquad E_t\neq E_{t+1}.
\]

**Fact:** Autoconstructive evolution makes reproduction and variation part of the evolving program, and major transitions can create new inheritance channels or selectable wholes. These are established forms of endogenous effective-operator change. [Edmonds 2001](https://journals.tubitak.gov.tr/elektrik/vol9/iss1/2/), [Harrington et al. 2012](https://doi.org/10.1145/2330784.2330797), [Szathmáry 2015](https://doi.org/10.1073/pnas.1421398112)

**Remaining boundary:** Existing theories do not settle what makes a new operator emergent rather than merely one member of a fixed operator language. A fixed universal interpreter, grammar, or code-manipulation substrate can generate many effective procedures without changing its own meta-rule. The distinction depends on the chosen causal, hereditary, developmental, and selectable-unit representation.

## 8. Environmental openness

**Fact:** In the formalism of Adams et al., openness to an environment is required for their version of unbounded evolution and innovation: the organism subsystem is compared with an isolated counterfactual, while environmental states perturb its time-dependent rule. Their state-dependent case scales because a larger environment supplies longer or richer perturbation histories while the same coarse-grained update function can be reused. [Adams et al. 2017](https://www.nature.com/articles/s41598-017-00810-8)

**Interpretation:** Environmental openness can prevent recurrence of a subsystem, but it does not by itself explain endogenous Type 2 OEE. It can:

- inject unbounded or effectively unbounded information;
- make the subsystem's rule history non-repeating;
- transfer the open-endedness question to the larger organism–environment system;
- produce novelty without adaptive evolution of the subsystem's own generative organization.

Environmental openness is therefore a sufficient ingredient for a particular extrinsic dynamical criterion, not a sufficient explanation of internally sustained meta-evolution. Pattee and Sayama's finite-domain argument reinforces this boundary: no system is open-ended without a specified scope and constraints.

## 9. Coevolution

**Fact:** Coevolution can promote complexity and evolvability. In an Avida host–parasite system, reciprocal selection produced more complex host traits and favored hosts with more evolvable phenotypes. [Zaman et al. 2014](https://doi.org/10.1371/journal.pbio.1002023)

**Fact:** Coevolution does not generically prevent closure. Predator–prey and host–parasite models admit extinction, stable coexistence with constant phenotypes, or cyclic Red Queen dynamics, depending on parameters. [Marrow, Law & Cooper 1995](https://doi.org/10.1006/jtbi.1995.0179)

**Interpretation:** Mutual modification can keep selection pressures moving and can create conditions favorable to evolvability, but it is a dynamical source of pressure, not a proof of indefinitely new evolutionary operators. Coevolution can converge, cycle within a fixed repertoire, or generate a one-time escalation. Organism–environment, host–parasite, genotype–ecology, and gene–culture feedbacks therefore remain candidate mechanisms, not resolutions.

## 10. Counterexamples

**A — Evolvability evolves once and stabilizes.** Evolving mutation rates can settle near a balance between novelty and memory or near an environment-specific optimum. This demonstrates selection on an evolvability modifier, not ongoing Type 2. [Bedau & Packard 2003](https://doi.org/10.1016/S0303-2647(02)00137-5)

**B — Operators evolve within a fixed repertoire.** Meta-genetic programming can evolve operator trees, but the operator language, encoding, interpreter, and preservation constraints remain specified. Operator change need not imply meta-space change. [Edmonds 2001](https://journals.tubitak.gov.tr/elektrik/vol9/iss1/2/)

**C — Self-reference remains bounded.** Closed self-referencing cellular automata provide a direct counterexample to self-reference as a sufficient condition for unbounded evolution. [Pavlic et al. 2014](https://arxiv.org/abs/1405.4070); the limitation is also stated by [Adams et al. 2017](https://www.nature.com/articles/s41598-017-00810-8).

**D — State novelty without adaptive meta-evolution.** A state-dependent or stochastically changing rule can produce non-repeating trajectories, while the rule-update function and rule representation stay fixed. This satisfies some dynamical novelty criteria without showing repeated heritable changes in evolutionary organization.

**E — Repeated major transitions can still be finite.** Major transitions are historically powerful changes in evolutionary organization, but their occurrence is contingent; the York report explicitly notes that there may be no more major transitions and that finite resources limit successive transitions. [Taylor et al. 2016](https://doi.org/10.1162/ARTL_A_00210)

**F — Coevolution reaches equilibrium.** The same reciprocal-selection architecture that can yield Red Queen cycling can yield extinction or stable coexistence with constant phenotypes. [Marrow, Law & Cooper 1995](https://doi.org/10.1006/jtbi.1995.0179)

**G — Fixed lower-level dynamics generate many effective procedures.** A fixed grammar, interpreter, or constructional alphabet can generate an indefinitely large family of behaviors or constructions. This dissolves the need for a new explicit meta-level in each case, but it does not show that the system has evolved a new effective evolutionary operator. It is a logical counterexample to the necessity of infinite hierarchy, not evidence that fixed generators guarantee Type 2 OEE.

## 11. Candidate resolution classes

| Class | Boundary after prior-art search |
|---|---|
| **A — Infinite hierarchy** | Not necessary. The regress is recognized, but recursive/self-applying and autoconstructive organizations offer finite alternatives. No evidence establishes an indefinitely rising meta-level as required. |
| **B — Recursive closure** | A real structural possibility and established as a design pattern, but not sufficient. Fixed recursive maps can converge, cycle, or generate novelty only within a fixed repertoire. |
| **C — Environmental openness** | Required by one formal dynamical criterion and useful for preventing subsystem recurrence, but it externalizes unboundedness and does not explain endogenous Type 2. |
| **D — Emergent effective hierarchy** | Best description of how fixed microphysics can support new biological organizations, inheritance channels, and selectable levels. Existing major-transition and EOE work covers important instances, but no sufficient criterion for indefinite continuation exists. |
| **E — Question malformed** | Correct against the universal regress claim: “another meta-level must exist” is not a well-supported necessity. The narrower closure question remains meaningful if posed causally and at a specified hereditary level. |

**Decision:** The evidence supports **E for the strong regress framing**, with partial mechanisms resembling B, C, and D. No class currently supplies a complete theory of ongoing Type 2 OEE.

## 12. Remaining explanatory gap

The narrow unresolved question is:

> Can a fixed-microphysics evolutionary system be given a representation-robust, causal assay that distinguishes repeated endogenous changes in its heritable repertoire of reconstructible evolutionary transformations from (i) fixed-rule output expansion, (ii) a one-off evolvability increase, (iii) external novelty injection, and (iv) observer-created relabeling?

This is narrower than “does the adjacent possible expand?” and narrower than “can evolvability evolve?” Existing literature covers those questions. It is also not solved by requiring (F_t) to change, because that merely reinstates the regress.

## 13. Known / Underexplored / Potentially Novel / Unknown

### Known / ESTABLISHED

- Ongoing evolution of evolvability is an established OEE hallmark and Tokyo Type 2 category.
- A single evolvability increase is not ongoing Type 2 OEE.
- The meta-evolution regress is explicitly recognized in meta-genetic programming; recursive and autoconstructive responses already exist.
- Self-reference can generate state-dependent rule dynamics, but self-reference is neither sufficient nor necessary for the relevant formal dynamical criteria.
- Fixed microphysics can support changing effective evolutionary organization through regulation, development, symbolic control, new inheritance channels, and new levels of individuality.
- Coevolution can promote evolvability but can also converge, cycle within a fixed repertoire, or terminate.
- OEE literature explicitly distinguishes behavioral hallmarks from hypothesized mechanisms and recognizes that a single hallmark instance is insufficient.

### Underexplored / PARTIALLY EXPLORED

- A common assay for repeated endogenous changes in evolutionary organization across biological, cultural, and artificial systems.
- A causal equivalence relation for distinguishing a new effective operator from a new output under an old operator.
- Prospective detection of Type 2 before the later adaptive targets are known.
- Empirical separation of internal meta-evolution from novelty supplied by an open environment.

### Potentially Novel

No new hypothesis or terminology is retained. “Recursive meta-evolution,” “generative closure,” and “evolvability of evolvability” overlap existing meta-evolution, autoconstructive evolution, EOE, major-transition, and self-referential-dynamics literatures.

### Unknown

- Whether an observer-robust criterion for ongoing endogenous meta-evolution exists at all.
- Whether ongoing Type 2 OEE is a mechanism, a trajectory-level hallmark, or a model-relative summary of repeated changes across organizational levels.
- Whether a finite recursive organization can sustain indefinitely many *new classes* of heritable evolutionary transformations without an externally enlarging domain.

## 14. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED.**

The novelty firewall fails for the proposed candidates. Infinite hierarchy is not established as necessary; recursive closure is known but not sufficient; environmental openness is an external source or subsystem-relative criterion; and emergent effective hierarchy is already substantially covered by EOE, evolving maps/operators, autoconstructive evolution, and major-transition theory. The unresolved criterion is important but too observer- and boundary-dependent to promote as a new mechanism.

## 15. Highest-information next question

**Can a fixed-microphysics evolutionary system be given a causal, representation-robust test for repeated endogenous changes in its heritable repertoire of reconstructible evolutionary transformations, while excluding fixed-rule output expansion and externally injected novelty?**

### Core references

- [Taylor et al. 2016 — Open-Ended Evolution: Perspectives from the OEE Workshop in York](https://doi.org/10.1162/ARTL_A_00210)
- [Packard et al. 2019 — An Overview of Open-Ended Evolution](https://doi.org/10.1162/artl_a_00291)
- [Pattee & Sayama 2019 — Evolved Open-Endedness, Not Open-Ended Evolution](https://doi.org/10.1162/artl_a_00276)
- [Channon 2024 — A Procedure for Testing for Tokyo Type 1 OEE](https://doi.org/10.1162/artl_a_00430)
- [Adams et al. 2017 — Formal Definitions of Unbounded Evolution and Innovation](https://www.nature.com/articles/s41598-017-00810-8)
- [Pavlic et al. 2014 — Self-referencing cellular automata](https://arxiv.org/abs/1405.4070)
- [Edmonds 2001 — Meta-Genetic Programming](https://journals.tubitak.gov.tr/elektrik/vol9/iss1/2/)
- [Spector 2001 — Autoconstructive Evolution](https://faculty.hampshire.edu/lspector/pubs/ace.pdf)
- [Zaman et al. 2014 — Coevolution Drives the Emergence of Complex Traits and Promotes Evolvability](https://doi.org/10.1371/journal.pbio.1002023)
- [Szathmáry 2015 — Toward Major Evolutionary Transitions Theory 2.0](https://doi.org/10.1073/pnas.1421398112)
- [Borg et al. 2022 — Evolved Open-Endedness in Cultural Evolution](https://arxiv.org/abs/2203.13050)
