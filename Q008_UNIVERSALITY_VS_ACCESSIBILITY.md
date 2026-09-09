# Q008 — Universality versus Evolutionary Accessibility

Research pass: 2026-09-07. Scope: whether a fixed universal or constructive substrate can turn in-principle generative capacity into an ongoing evolutionary history. No implementation was performed.

## 1. Problem statement

The fixed-meta-rule intuition needs correction. A fixed mechanism $U$ need not expose a finite repertoire. If descriptions are extensible, then

\[
\mathcal C_U=\{y:\exists d\;U(d)=y\}
\]

may be infinite even though $U$ never changes. A universal interpreter, constructor, chemistry, or physical law can therefore support effective structures and procedures not individually listed in the meta-rule.

This does not establish OEE. It establishes at most a capacity claim. The relevant distinction is:

\[
\text{expressible}
\rightarrow
\text{constructible}
\rightarrow
\text{evolutionarily accessible}
\rightarrow
\text{viable, heritable, maintained, and recursively exploitable}.
\]

The research question is therefore not whether the substrate can realize arbitrarily rich organizations, but what makes evolution discover and preserve them through endogenous histories.

**Fact.** A fixed universal mechanism does not entail a fixed finite effective repertoire.

**Interpretation.** Formal generative capacity is weaker than endogenous exploitable generative capacity. The latter includes the geometry and probability of viable paths, not only the existence of descriptions.

## 2. Universal construction

Von Neumann’s universal constructor architecture separates a description tape from the constructor and copier. A description can be copied as description and interpreted to construct the machine it encodes. This makes heritable variation in descriptions compatible with a fixed construction architecture. Hutton’s artificial-chemistry review correctly emphasizes the distinction: a universal constructor gives theoretical evolutionary capacity, but does not by itself demonstrate sustained complexity growth.

Universal construction establishes, conditional on appropriate resources and a suitable description:

\[
\exists d_y\;U(d_y)=y.
\]

It does not establish that mutation produces (d_y), that intermediate descriptions remain viable, that the lineage can maintain the constructor while changing the description, or that selection discovers the target without an externally supplied target. Universal construction is thus a capacity theorem or architecture, not a historical theorem about evolutionary search.

The Stringmol work is a stronger empirical case. Clark, Hickinbotham, and Stepney report simultaneous evolution of genomic material, copier, and constructor, with viable offspring, and describe the resulting semantic closure. This demonstrates endogenous change in the interpretation/construction organization in an artificial chemistry. It remains evidence for a transition and for one form of recursive coupling, not evidence that such changes continue indefinitely or avoid eventual closure.

**Status: ESTABLISHED.** Universal construction separates description from interpreter/constructor and permits extensible heritable descriptions. **Not established:** universal construction alone generates ongoing OEE.

Sources: [von Neumann architecture discussed by Hutton (2002)](https://faculty.cc.gatech.edu/~turk/bio_sim/articles/hutton_rep_molecules.pdf); [Clark, Hickinbotham & Stepney (2017)](https://doi.org/10.1098/rsif.2016.1033).

## 3. Computational universality

Computational universality means that, with a suitable encoding and input/program, a substrate can implement any computable computation in the relevant class. It is stronger than a finite catalogue of behaviors, but it still leaves the evolutionary problem open.

**Fact.** Universality normally quantifies over carefully prepared programs, encodings, inputs, or configurations. It does not quantify over the probability that a mutation-selection process produces those encodings through viable intermediates.

The missing conditions include:

* a physical realization of the computation rather than merely a formal simulation;
* self-reproduction or another persistence mechanism;
* mutation and recombination that preserve enough semantics for cumulative change;
* selection that rewards the relevant intermediate organizations;
* a path from the starting population to the target descriptions.

Artificial systems such as Tierra and Avida show that universal computation can coexist with evolving programs, but program evolution and universal computation are not a proof of sustained OEE. Conversely, formal definitions of open-endedness can be satisfied by simple computational systems whose novelty is not the kind of cumulative organizational innovation at issue here. This is why computational universality is neither a sufficient OEE criterion nor, under every OEE definition, a necessary one.

**Counterexample.** A universal machine can be initialized with a program that computes an arbitrarily complicated result while the evolutionary population is absent, non-heritable, trapped on a local attractor, or unable to discover the required program. The computation exists; the evolutionary history does not.

Sources: [Hutton (2002)](https://faculty.cc.gatech.edu/~turk/bio_sim/articles/hutton_rep_molecules.pdf); [Open-Endedness for the Sake of Open-Endedness (2021)](https://doi.org/10.1162/artl_a_00289).

## 4. Physical universality

Physical universality is a distinct, stronger-looking notion in cellular-automaton theory. Janzing’s formulation, used by Salo and Törmä, asks whether a fixed dynamics can implement an arbitrary transformation of patterns in a finite region by configuring the surrounding pattern. It quantifies over arbitrary inputs, rather than only a specially prepared computational subspace. The fixed cellular-automaton law can therefore have an unbounded class of effective transformations.

This is relevant to the fixed-meta-rule problem: it directly demonstrates how fixed low-level dynamics can support a non-finite constructive repertoire. It still says nothing by itself about:

* how the required controller/gadget is generated by evolution;
* whether the gadget is self-maintaining and heritable;
* whether mutations preserve constructional semantics;
* whether viable evolutionary paths connect current lineages to increasingly rich gadgets;
* whether selection repeatedly favors the transformations that expand later accessibility.

Constructor theory makes a related distinction by formulating physical laws in terms of possible and impossible transformations and constructors. That is useful for asking whether a transformation can in principle be performed, but a possibility statement is not a probability distribution over endogenous lineages. It does not by itself supply persistence, selection, developmental realization, or historical accessibility.

**Fact.** Physical universality removes some substrate-level representational restrictions.

**Interpretation.** It is closer to a condition for universal construction than to a condition for OEE. A physically universal world can contain evolutionarily trivial initial conditions and selection regimes.

Sources: [Salo & Törmä (2015), definition and distinction from computational universality](https://arxiv.org/abs/1501.03988); [Deutsch (2012), Constructor Theory](https://arxiv.org/abs/1210.7439).

## 5. Indefinite scalability

Ackley’s indefinite scalability concerns the absence of a hard architectural ceiling: when physical or computational resources are increased, larger or more capable living computation can in principle continue. This is important infrastructure for avoiding a finite-size bottleneck.

It is not, by itself, a mechanism for discovering or exploiting the available scale. A scalable substrate may support arbitrarily large organisms while evolution repeatedly returns to the same simple organization. It may also have a rapidly shrinking fraction of viable configurations as size or coordination requirements grow.

Thus:

\[
\text{indefinite scalability}
\not\Rightarrow
\text{indefinite evolutionary exploitation of scale}.
\]

**Status: PARTIALLY EXPLORED.** Indefinite scalability is a plausible enabling condition and an empirical design/test dimension, but the literature does not establish it as sufficient for OEE or as the missing anti-closure mechanism.

Source: [Ackley (2016)](https://doi.org/10.1609/aaai.v30i1.9802).

## 6. Description-space extensibility

An extensible hereditary description space makes the universal-construction distinction concrete. If $G$ can grow in length or structure while $P=U(G)$, a fixed $U$ can interpret descriptions of increasing complexity. This is enabling for unbounded heritable construction under a description-based architecture.

It is not sufficient. Description growth can be neutral padding, redundant encoding, intronic or inactive material, or repeated changes that leave function and organization invariant. Conversely, an effective organization can become more complex through interaction, development, ecological structure, or non-genetic inheritance even when a particular genome representation is bounded; whether this counts as strong OEE depends on the system boundary and OEE definition.

The strongest conservative conclusion is conditional:

* For unbounded heritable construction encoded only in a finite alphabet with a permanently bounded description length, unbounded hereditary construction is structurally unavailable.
* Unbounded descriptions are therefore enabling, and may be necessary for that narrow architecture.
* They are not sufficient for functional, organizational, or adaptive novelty, and they are not necessary for every broader OEE-like criterion.

The converse is therefore also established by counterexample in principle: a lineage can accumulate description length without increasing selectable organization. Length is a resource or proxy, not the target property.

## 7. Evolutionary accessibility

Evolutionary-accessibility theory gives the closest formal vocabulary for the missing link, although it is usually target-relative and local rather than an OEE theory. A target $Y$ is accessible from $X_0$ only when the relevant mutational, developmental, ecological, and selective process supplies a path such as

\[
X_0\rightarrow X_1\rightarrow\cdots\rightarrow X_n=Y
\]

with acceptable intermediate viability and transmission. A probabilistic version additionally asks for the probability of the path under mutation, fixation, drift, selection, development, and ecology.

Fitness-landscape work formalizes accessible monotone paths, path divergence, sign epistasis, ruggedness, neutral networks, and valley crossing. Lobkovsky, Wolf, and Koonin report that only a small fraction of theoretically possible trajectories may be accessible in analyzed landscapes, while also showing that landscape structure changes this fraction. This directly separates the size of a theoretical space from the portion evolution can explore.

Related genotype–phenotype and neutral-network work shows that robustness can preserve lineages while exposing cryptic variation, and that navigability depends on the structure of the map. These concepts address reachability, but they do not yet provide a general criterion for repeated, endogenous expansion of the accessible class of evolutionary organizations.

Useful notation is:

\[
\mathcal U=\text{all constructible organizations},
\qquad
\mathcal E(X_t;\Pi)=\text{organizations reachable under process }\Pi.
\]

The relevant OEE question is about the history of $\mathcal E$, not merely the cardinality of $\mathcal U$:

\[
\mathcal E(X_{t+1};\Pi)\ ?\supsetneq\ \mathcal E(X_t;\Pi)
\]

with the increase caused by heritable endogenous organization and remaining usable for later evolution.

Source: [Lobkovsky, Wolf & Koonin (2011)](https://doi.org/10.1371/journal.pcbi.1002302).

## 8. Universal capacity versus endogenous discovery

The central gap can be stated without treating universality as OEE:

\[
\exists d\;U(d)=Y
\]

is an existence claim, whereas

\[
P(\text{lineage reaches and establishes }d\mid X_t,\Pi)>0
\]

is a historical/accessibility claim. A viable path is stronger than nonzero formal probability because it requires intermediate maintenance, reproduction, inheritance, and selection-compatible transitions.

Universal construction usually assumes that a description or controller is supplied. Evolution must produce both the description and, when necessary, the machinery that interprets it. The problem is not solved by replacing a finite operator catalogue with an infinite set of possible programs if almost all programs are unreachable or nonviable.

This is not a new hypothesis. It is a clarification of the boundary between universal construction, evolvability, and evolutionary accessibility. Existing literatures cover the pieces, but no reviewed source supplies a general OEE criterion that combines them with repeated recursive exploitation.

## 9. Path viability and search complexity

The gap is partly explained by path viability and search complexity, but not exhausted by ordinary fitness-landscape language.

**Established components:** ruggedness and sign epistasis can block monotone paths; neutral networks can permit drift and expose variation; valley crossing can make a target possible but unlikely; developmental maps and modularity can alter accessibility; ecological scaffolding can change intermediate fitness.

The relevant difficulty is not representation size alone. It may involve the minimum coordinated change, the density of viable intermediates, the probability of retaining a scaffold, the number of trials, and whether the target remains selectable while the necessary machinery is assembled. A short description can be hard to discover; a long description can be easy if a reusable module makes it accessible.

**Interpretation.** Search complexity is a necessary part of the capacity-to-history distinction, but “fitness landscape” is too local unless the landscape itself includes changing genomes, developmental semantics, inheritance, ecological context, and selectable units. The remaining question is whether innovations systematically reduce the search complexity of later innovations, not merely whether they add another nearby outcome.

## 10. Cumulative/scaffolded accessibility

Scaffolding and cumulative construction are established prior art. Potentiation, facilitated variation, developmental toolkits, exaptation, modularity, major transitions, autocatalytic organization, and cumulative cultural evolution all describe ways in which one organization can make later transformations easier, viable, or selectable. The generic pattern is:

\[
A\not\rightsquigarrow C,
\qquad
A\rightsquigarrow B\rightsquigarrow C.
\]

This can bridge the gap between universal capacity and actual discovery when (B) is heritable, reusable, and changes the accessibility structure of later variation. But it is not automatically cumulative meta-evolution. Scaffolds can be one-off, can become entrenched, can support only a finite sequence, or can be lost. Cumulative culture can display strong cumulative improvement without necessarily satisfying OEE. Artificial circuit systems also show improvement and invention followed by plateaus.

The Stringmol UCA is the strongest directly relevant positive case located in this pass: the genomic material, copier, and constructor coevolve and viable offspring result. It demonstrates that a fixed underlying artificial chemistry can host endogenous changes in constructional organization. It does not demonstrate an indefinitely repeated reduction in the search complexity of future construction.

## 11. Counterexamples

### A — Universal computational substrate with no OEE

A universal computation substrate can be evolutionarily inert, or its population can remain on a stable simple lineage. Universal computation requires suitable configurations; it does not guarantee that selection discovers them. Simple computational systems can also satisfy behavioral open-endedness criteria without the intended organizational novelty.

### B — Universal constructor without sustained complexity growth

Von Neumann’s architecture supplies the theoretical capacity for increasingly complex self-reproducing machines. Hutton’s review notes that simulated evolutionary growth of complexity had not been conclusively demonstrated. Thus constructional universality is not a historical result.

### C — Indefinitely scalable but evolutionarily simple world

A world can add space, time, or material without changing mutation, selection, developmental constraints, or ecological attractors. The maximum possible organism size grows, while the realized evolutionary history remains bounded or repetitive. Scalability is therefore not exploitation.

### D — Unbounded descriptions with stagnation

Variable-length genomes can accumulate neutral or redundant sequence, or vary descriptions that map to the same effective organization. Description-space growth without new selectable organization is not OEE.

### E — Non-universal system with substantial OEE-like behavior

Systems lacking a proof of computational or physical universality can still show sustained diversity, adaptive exploration, or model-relative open-ended behavior. Consequently universality is not necessary for every behavioral OEE criterion. A stronger claim about unbounded construction would require specifying the criterion and boundary.

### F — Expanding accessibility with increasing search difficulty

An innovation can enlarge the set of formally reachable states while making viable paths to later states rarer, longer, or more coordinated. Accessibility expansion and successful exploitation can therefore diverge; the former does not imply the latter.

### G — Reusable mechanisms easing later innovation

Developmental reuse, facilitated variation, neutral networks, cumulative culture, and the Stringmol constructor/copier transition all support this possibility. They establish mechanisms for local or historical scaffolding, not a general theorem that search complexity decreases often enough to prevent eventual closure.

## 12. Surviving conceptual distinction

The most useful surviving distinction is:

\[
\boxed{\text{formal generative capacity}}
\quad\neq\quad
\boxed{\text{endogenously exploitable generative capacity}}.
\]

The first concerns expressibility and constructibility under (U). The second concerns a lineage-level process that can repeatedly:

1. produce a heritable constructional or organizational scaffold;
2. preserve it while variation continues;
3. make new viable transformations accessible;
4. cause those transformations to be selected and maintained; and
5. reuse the resulting organization in later evolutionary change.

This is not a new named theory. It is a synthesis boundary across universal construction, evolvability, accessibility, developmental systems, and cumulative evolution. “Accessibility-centered” is closer to the evidence than “universality-centered,” but it remains incomplete because accessibility can expand without recursive exploitation or indefinite continuation.

## 13. Remaining explanatory gap

The narrow unresolved problem is:

> Can a fixed universal or constructive substrate be given an operational, causal, and representation-robust test for repeated endogenous increases in the accessibility of viable, heritable evolutionary organizations—caused by prior heritable innovations—while distinguishing them from fixed-rule output expansion, neutral description growth, externally injected novelty, and one-off scaffolding?

This requires more than showing that (mathcal U) is infinite or that (mathcal E(X_t)) grows once. It requires a criterion for the repeated historical transformation of the accessibility relation itself, including probability, viable intermediates, persistence, and later reuse.

## 14. Known / Underexplored / Potentially Novel / Unknown

### KNOWN

* Fixed interpreters, constructors, physical laws, and local rules can support non-finite or universal classes of effective transformations.
* Universal construction separates descriptions from construction and copying, enabling heritable variation in descriptions.
* Computational and physical universality are capacity notions, not guarantees of viable evolutionary discovery.
* Fitness landscapes, genotype networks, neutral networks, developmental maps, and valley-crossing theory formalize important parts of evolutionary accessibility.
* Scalability, facilitated variation, potentiation, reuse, major transitions, and cumulative culture provide established scaffolding mechanisms.

### UNDEREXPLORED

* A unified treatment connecting universal construction to the probability and viability of endogenous evolutionary paths.
* A prospective measure of whether a heritable innovation reduces the search complexity of later constructional innovations.
* A repeated-accessibility criterion that remains meaningful as the genotype–phenotype map, inheritance system, or selectable unit changes.

### POTENTIALLY NOVEL

No new mechanism is justified by this pass. The distinction between capacity and accessibility is already distributed across established literatures and is not itself a novelty claim.

### UNKNOWN

Whether any fixed-microphysics system can be shown, under a representation-robust criterion, to generate an indefinitely extensible sequence of such accessibility-transforming scaffolds remains unknown.

## 15. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

The novelty firewall fails for the candidate “endogenously exploitable generative capacity” as a new hypothesis. It substantially overlaps evolutionary accessibility, evolvability, facilitated variation, adjacent-possible expansion, potentiation, major transitions, and cumulative evolution. The pass clarifies their missing connection but does not justify a distinct causal theory.

`HYPOTHESES.md` is therefore unchanged.

## 16. Highest-information next question

Can a fixed-microphysics evolutionary system be given a causal, representation-robust measure of repeated increases in the probability and viability of later heritable organizational innovations that are caused by prior innovations, rather than by a larger fixed repertoire or external novelty?
