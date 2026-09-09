# Q010 — Measurement Invariance of Evolutionary Accessibility

Theoretical research pass, 2026-09-07. Scope: whether resource-normalized first-passage distributions over novelty classes remain comparable when evolutionary representation, organization, or level changes. This pass evaluates coherence and prior art; it does not propose an OEE metric or mechanism.

## 1. Problem statement

Q009 replaced existential reachability with a stronger, conditional object: the probability distribution for first reaching a specified novelty under a specified evolutionary process and resource budget. That move exposes a second problem. A first-passage distribution is not determined by dynamics alone. It requires at least:

\[
(\text{state process},\ \text{initial ensemble},\ \text{target set},\ \text{clock or cost}).
\]

All four may change during OEE. Evolution can alter genotype representation, the genotype–phenotype map, heredity, population structure, ecological interaction, reproduction rate, and the entities treated as evolutionary individuals. The question is therefore not simply whether two distributions can be calculated, but whether their events and resource axes denote commensurate scientific quantities.

Three problems must be separated:

1. **Coordinate invariance:** two encodings describe the same causal process.
2. **Coarse-graining invariance:** one description groups states or histories of another.
3. **Evolutionary-level invariance:** the causal organization itself changes, potentially introducing new hereditary entities, reproductive relations, or selectable units.

The first has a clean solution. The second has exact and approximate mathematical conditions. The third need not admit a total correspondence at all. Treating them as one “representation problem” hides the main boundary.

## 2. Existing OEE comparability frameworks

### Evolutionary activity and neutral shadows

Bedau-style evolutionary activity compares the realized use or persistence of components against an adaptively neutral shadow. It enabled comparisons among artificial systems and the fossil record, but only after defining component identity, activity, thresholds, sampling intervals, and a shadow that preserves chosen background dynamics. It measures realized historical activity, not the latent distribution of resources required to reach a future target. A shadow is not automatically invariant when the component ontology, reproduction process, or selectable level changes; the matching intervention that defines the shadow must then be specified again. [Bedau, Snyder & Packard 1998](https://sfi-edu.s3.amazonaws.com/sfi-edu/production/uploads/sfi-com/dev/uploads/filer/b3/e9/b3e9317b-5798-485b-8bb1-3465cd336e0e/98-03-025.pdf)

### MODES

MODES aims to make change, novelty, complexity, and ecological metrics implementable and comparable across systems. Its units are deliberately generic “components,” which may be genotypes, phenotypes, or higher taxa. That agnosticism is useful, but it is not ontological invariance: each application must supply component identity, a distance or complexity interpretation where required, relevance filtering, fitness or reproductive-output information, and measurement time. MODES notes that its time variable must be strictly increasing and permits tracking generation plus another clock when generation does not increase reliably. It also identifies measurement of potential for major transitions in individuality as future work. [Dolson et al. 2019](https://doi.org/10.1162/artl_a_00280)

Consequently, MODES solves a within-definition standardization problem: given operational components and filters, it summarizes realized histories in a common metric family. It does not estimate latent first-passage accessibility, derive a class mapping when the components become parts of a higher-level individual, or make pre- and post-transition “generations” equivalent.

### Formal innovation and unbounded-evolution measures

Adams et al. define innovation and unbounded evolution relative to a specified organism–environment partition, update steps, and isolated counterfactual system. Those definitions are rigorous within that dynamical model, but changing the partition, rule space, state dimension, or isolated comparator changes the proposition being measured. They do not provide cross-ontology first-passage normalization. [Adams et al. 2017](https://pmc.ncbi.nlm.nih.gov/articles/PMC5430523/)

Taylor's exploratory, expansive, and transformational novelty is explicitly relative to a model and meta-model. Transformational novelty introduces a new concept and therefore requires a meta-model change; a major transition in individuality is a candidate case. This directly recognizes the vocabulary change that creates the present comparability problem, but the framework does not provide a numerical transport rule between old and new concepts. [Taylor 2019](https://www.tim-taylor.com/papers/taylor2019evolutionary.preprint.pdf)

**Boundary:** existing OEE frameworks support cross-system comparison only after system-specific semantic choices. None reviewed supplies a representation- and resource-normalized accessibility invariant across changes in evolutionary ontology.

## 3. First-passage theory

For a stochastic process \(X\), initial law \(\mu\), target \(N\), and increasing resource process \(R\), define the first target time and its resource cost by

\[
\tau_N=\inf\{t:X_t\in N\},
\qquad
R_N=R_{\tau_N}.
\]

The distribution \(F_N(r)=P_\mu(R_N\le r)\) is well defined even when the observed process is non-Markovian, provided the path law, target event, and resource functional are specified. Markov assumptions are computational conveniences, not prerequisites for defining first passage.

For an invertible relabeling \(h:X\to Y\), the law is exactly coordinate invariant if the process, initial law, target, and resource functional are all pushed forward:

\[
N\mapsto h(N),\qquad
\mu\mapsto h_*\mu,
\qquad
R\mapsto h_*R.
\]

Then corresponding sample paths have identical hitting events and resource costs. An accessibility score that changes under such a relabeling is measuring encoding-dependent features such as raw Hamming distance, not first passage of the same event.

Noninvertible projection is different. Let \(q:X\to Z\). If \(N\) is **saturated** by the partition—\(N=q^{-1}(B)\) for some macro-target \(B\)—then along every path

\[
\inf\{t:X_t\in N\}
=
\inf\{t:q(X_t)\in B\}.
\]

Thus the exact projected path process preserves the complete hitting-time distribution for that target. No Markov assumption is needed for this pathwise identity. What may fail is the attempt to replace that projected, potentially history-dependent process by an autonomous low-order Markov model.

## 4. Coarse-graining and lumpability

For a finite discrete-time Markov chain with transition matrix \(P\) and partition \(\{B_i\}\), strong lumpability requires

\[
\sum_{z\in B_j}P(x,z)
=
\sum_{z\in B_j}P(x',z)
\quad
\text{for every }x,x'\in B_i\text{ and every }B_j.
\]

This is the Kemeny–Snell condition: the next-block distribution is independent of the hidden microstate within the present block. It makes the quotient a Markov chain for every initial distribution. Weak lumpability yields a Markov quotient only for restricted initial distributions; higher-order lumpability permits a finite-memory quotient. These qualifications matter because an OEE comparison should not silently depend on an unreported microstate mixture. [Jernigan & Baran 2003, overview and statistical test](https://doi.org/10.1016/S0167-7152(03)00126-3), [Geiger & Temmel 2014](https://arxiv.org/abs/1212.4375)

With a saturated target and matching initial law, a strongly lumpable quotient preserves finite-horizon reachability and hence the full discrete hitting-time distribution, not only its mean. Probabilistic bisimulation provides the corresponding labeled behavioral equivalence and is known to preserve reachability probabilities. [Givan, Dean & Greig 2003](https://cs.brown.edu/people/tdean/publications/archive/GivanetalAIJ-03.pdf), [Doberkat 2007](https://research.utwente.nl/en/publications/bisimulation-logic-and-reachability-analysis-for-markovian-system/)

Failure modes are precise:

- If the target is not a union of blocks, reaching its block is not equivalent to reaching the target.
- If the projection is not lumpable, the macro trajectory generally retains hidden-state memory. A fitted first-order quotient can therefore change hitting probabilities and distributions.
- Weak lumpability can preserve results for one starting ensemble while failing for another.
- Metastable aggregation is normally approximate and depends on timescale separation; preserving slow modes or a mean does not guarantee preservation of tails.
- If the original evolutionary dynamics are history dependent, the state must be enlarged to include sufficient history, or a semi-Markov/higher-order/path-space model must retain the memory.

Milestoning shows that coarse first-passage calculations can remain exact or controlled under specified assumptions. Exact Milestoning maps a time-homogeneous strong Markov process into a Markov or semi-Markov milestone process and supplies an exact mean-first-passage equation plus error bounds. Coarse-memory Milestoning improves passage estimates by enlarging the macrostate with recent-history information when the ordinary memory-loss assumption fails. These are preservation methods for selected endpoints, not universal coarse-graining invariants. [Aristoff et al. 2016](https://pmc.ncbi.nlm.nih.gov/articles/PMC4879838/), [Hawk 2013](https://doi.org/10.1063/1.4795838)

## 5. Novelty-class equivalence

Novelty classes require an equivalence relation. Three established approaches constrain such relations:

- **Predictive causal states** group histories that induce the same conditional distribution over specified futures. They are minimal sufficient predictive states for the observed process. [Shalizi & Crutchfield 2001](https://arxiv.org/abs/cond-mat/9907176)
- **Probabilistic bisimulation** groups states with matching labels/rewards and matching transition probabilities into equivalence blocks. It preserves the specified behavioral properties, not every possible interpretation.
- **Intervention-respecting causal abstractions** require a mapping between low- and high-level variables and a compatible mapping between allowed interventions. Exact transformations can justify using the high-level model for high-level intervention effects. [Rubenstein et al. 2017](https://is.mpg.de/uploads/publication_attachment/attachment/427/UAI_2017_Rubensteinetal.pdf)

These methods can make novelty classification less arbitrary, but not uniquely intrinsic. Predictive causal states depend on the observed variables and future distinctions; causal abstractions depend on macrovariables and intervention sets; bisimulation depends on labels or rewards chosen for preservation. Shalizi and Moore make the boundary explicit: dynamics constrain the refinement once observables are chosen, but do not select the initial observables. [Shalizi & Moore 2003](https://arxiv.org/abs/cond-mat/0303625)

Hoel et al.'s causal emergence compares intervention-based effective information across coarse-grainings and can identify a macro-description that is more causally informative than a given micro-description. Yet the result presupposes a micro transition model, a coarse-graining, and an intervention distribution; it does not choose evolutionarily meaningful novelty classes or transport them through a change of individuality. [Hoel, Albantakis & Tononi 2013](https://pmc.ncbi.nlm.nih.gov/articles/PMC3856819/)

Therefore causal grounding supplies constraints, not a universal class system. An equivalence relation can change as reproduction, heredity, interaction, or the relevant prediction target changes. If a post-transition class has no defensible predecessor, its pre-transition first-passage distribution is undefined rather than infinite or zero.

## 6. Resource normalization

Evolutionary theory routinely uses several clocks or opportunity measures, each appropriate to a particular question:

| Normalizer | What it controls | Why it can fail across transitions |
|---|---|---|
| Physical time | elapsed duration | does not equalize reproductive or mutational opportunity |
| Generations | lineage turnover | depends on the reproducing entity and life cycle |
| Birth or lineage-reproduction events | reproductive trials | event identity changes when individuality changes |
| Mutation events/opportunities | variation supply | depends on the hereditary channel and mutation operator |
| Population turnovers / population-time | parallel sampling | requires a stable population and individual count |
| Evaluated variants | search work in digital systems | ignores unequal development, ecology, and physical cost |
| Energy or metabolic expenditure | a physical budget | energetic equivalence need not imply equal evolutionary opportunity |
| Update or causal events | computational/causal work | event granularity and causal decomposition are model choices |

Population-genetic waiting times already depend on population-wide mutation supply and demographic history; changing population size can alter first-arrival time without changing the per-lineage landscape. Evolutionary rescue makes the dependence especially clear because population decline reduces the supply of new mutations through time. [Orr & Unckless 2014](https://pmc.ncbi.nlm.nih.gov/articles/PMC4133041/)

Markov reward models and reward-bounded reachability give established mathematics for accumulated cost rather than elapsed time. They show that \(P(R_N\le r)\) is coherent after a reward/cost function has been specified. They do not make that function representation independent or evolutionarily canonical.

No reviewed theory supplies a universal evolutionary resource measure invariant under changes in heredity, life cycle, ecology, and individuality. Energy and physical time are comparatively ontology-stable but scientifically answer different questions from mutation opportunity or lineage turnover. A normalizer cannot eliminate observer choice; it must be causally justified for the comparison being claimed.

## 7. Changing evolutionary clocks

Major transitions in individuality are a decisive stress test. They reorganize fitness and shift its reference from formerly independent lower-level entities to a higher-level individual. The lower and higher levels may coexist and reproduce on different schedules during the transition. [Michod 2007](https://doi.org/10.1073/pnas.0701489104), [West et al. 2015](https://pmc.ncbi.nlm.nih.gov/articles/PMC4547252/)

Multilevel selection and multilevel Price-equation formalisms can attribute change to within- and between-collective processes once particles, collectives, traits, descendants, and a census interval are specified. They do not derive a canonical conversion between one lower-level generation and one higher-level generation. Discrete-generation versions make that assumption explicit; overlapping or nested life cycles require additional bookkeeping.

Hence

\[
1\ \text{generation before}
\not\equiv
1\ \text{generation after}
\]

when the bearer of reproduction changes. Physical time can span the transition, but then a gain in access may merely reflect more births, greater population size, or faster metabolism. Counting all births can span levels, but weighting a cell division against collective reproduction is not supplied by multilevel selection theory. No evolutionary clock found both survives every transition and equalizes the opportunity relevant to every accessibility claim.

## 8. Representation versus causal change

A principled but conditional distinction is available:

- **Epistemic representation change:** an invertible relabeling, or an exact abstraction preserving the specified interventions and outcomes. Correctly transported first-passage claims should be invariant.
- **Information-losing redescription:** a coarse-graining. Invariance is property-relative and requires target saturation plus an adequate projected dynamics—lumpable, bisimilar, memory-aware, or accompanied by explicit approximation error.
- **Endogenous causal change:** the transition law, hereditary relation, organism–environment partition, reproduction process, or selectable unit changes. Differences in accessibility can be real, but only conserved targets and resources can be quantitatively compared.

Exact causal transformations and probabilistic bisimulation can test proposed correspondences. They do not prove that a particular macrovariable is the newly relevant evolutionary individual. That empirical and theoretical identification still requires criteria such as heritable variation in collective fitness, integration, conflict control, or intervention effects on future reproduction.

This reconnects with Q003: dynamics can reject bad representations and show that two descriptions preserve chosen consequences, but they cannot provide an observer-free catalogue of all meaningful evolutionary distinctions.

## 9. Full distributions versus scalar metrics

The full first-passage distribution is the right established object when finite budgets and tail risk matter. The survival function \(S(r)=P(R_N>r)\) equivalently characterizes a single-target first-passage problem, and its hazard describes conditional arrival propensity. This applies to Markovian and non-Markovian processes. [Levernier et al. 2019](https://pmc.ncbi.nlm.nih.gov/articles/PMC6611868/)

A mean discards decisive information. For example, a process that reaches at resource 10 with probability one and a process that reaches at resources 1 and 19 with equal probabilities have the same mean, yet their probabilities of access under budgets below 10 and between 10 and 19 differ sharply. A divergent mean can also coexist with substantial finite-budget probability under a heavy tail.

If target and resource semantics are already matched, first-order stochastic dominance provides a useful partial order:

\[
F_B(r)\ge F_A(r)\quad\text{for all }r
\]

means that \(B\) reaches the target with at least as much probability under every resource budget. Crossing distributions remain incomparable under this order. Dominance adds a budget-uniform comparison, but it cannot establish that the two distributions concern the same target or resource. Distributional richness repairs scalar information loss, not ontological mismatch.

## 10. Cross-ontology comparison

Complete pre/post comparison requires a relation between novelty-class systems and resource processes. Existing mathematics supports several conditional cases:

- an isomorphism for the same process in different coordinates;
- a lumpable or bisimilar quotient for preserved labeled behaviors;
- a refinement/coarsening relation for nested classes;
- an intervention-preserving causal abstraction between levels;
- a partial correspondence restricted to conserved functions or causal consequences.

It does not require a total one-to-one map. If \(\mathcal N_{t+1}\) contains a class that cannot be expressed in \(\mathcal N_t\), then targetwise comparison for that class has no pre-transition argument. Forcing it into an old class would erase the very distinction that makes the novelty transformational. Taylor's model/meta-model account makes this tension explicit conceptually: transformational novelty requires a new concept, while quantitative transport would require enough prior vocabulary to identify the same event.

This is not fundamental non-comparability of the entire transition. Conserved observables—physical persistence, material flux, some reproductive consequences, or lower-level dynamics—may still support comparisons. New higher-level classes may be related to old states by a many-to-one causal abstraction or emergence process without being equivalent to any old novelty class. The scientifically defensible result is therefore a family of matched comparisons plus explicitly undefined entries, not a universal scalar ordering.

## 11. Counterexamples

### A — Encoding-dependent scores under identical dynamics

Encode the same finite Markov chain bijectively using bit strings of different lengths. Hitting-time distributions are unchanged after transporting the target, but Hamming distance and “fraction of genotype space searched” can change arbitrarily under the encoding. Such scores fail coordinate invariance even though first passage itself does not.

### B — A coarse target that is not saturated

Let microstates \(a\) and \(b\) be placed in one macrostate, with novelty defined as reaching \(a\). A trajectory at \(b\) has already reached the macro-block but has not reached \(a\). Macro hitting time can be zero while micro novelty remains unobserved. Coarse-graining has changed the event.

### C — Generation changes meaning

During a unicellular-to-multicellular transition, cell divisions and collective reproduction are distinct event series. “Ten generations” can mean ten cell cycles or ten collective life cycles and therefore cannot normalize access without specifying the reproductive level.

### D — Parallel search masquerading as accessibility

For \(n\) independent lineages with individual first-passage survival \(S(r)\), the first arrival among them has survival \(S(r)^n\). Increasing population size shortens the observed first-arrival distribution even when each lineage's mutation map and accessibility are unchanged. Raw first-passage time therefore confounds organization with sampling resources.

### E — Equal means, different tails

The deterministic resource cost 10 and the equal mixture of costs 1 and 19 both have mean 10, but neither gives the same finite-budget claim. Mean first-passage time cannot identify accessibility distributions.

### F — No old predecessor for a new class

If novelty is “heritable variation in collective reproductive success,” a pre-transition collection with no collective reproduction may supply precursor microstates but no instance of that target class. Assigning a pre-transition waiting time requires retroactively imposing the later individuality criterion.

### G — Exact preservation despite microscopic difference

In a strongly lumpable chain or probabilistically bisimilar transition system, microstates within a block have identical transition probability into every labeled block. For any block-saturated target, the quotient preserves all finite-horizon reachability probabilities and therefore the hitting-time distribution. This is a positive witness for representation-robust comparison under explicit conditions.

Cases A–G are mathematical or conceptual counterexamples, not claims that a particular historical transition realizes them.

## 12. Candidate comparability conditions

Prior art supports the following conditions for a *particular* cross-description accessibility claim. They are an audit checklist, not a new metric:

1. **Process relation:** state whether the descriptions are isomorphic, one is a projection of the other, or the causal dynamics genuinely differ.
2. **Target relation:** provide an exact, refinement, or partial mapping and show that targets are saturated when quotient hitting times are used.
3. **Initial-condition relation:** transport or justify the initial ensemble; weak lumpability and metastable estimates can depend on it.
4. **Dynamics preservation:** establish lumpability/bisimulation, retain necessary semi-Markov or higher-order memory, or report approximation error for the specific passage statistic.
5. **Resource relation:** use a common additive clock/cost with causal justification, or give an explicit conversion; do not equate generations at different levels by name alone.
6. **Distributional claim:** compare the full CDF/survival curve or justified quantiles when tails matter; use a scalar only for the stated question.
7. **Null relation:** if a shadow or randomized control is used, show how both the observed and null processes map across the transition. A newly redesigned null is not automatically the same baseline.
8. **Undefined cases:** report unmatched new classes as incomparable, rather than assigning zero, infinity, or an observer-chosen predecessor.

When these conditions hold only for a subset of classes and resources, comparison is correspondingly partial. They make claims reproducible without pretending that a universal evolutionary currency has been found.

## 13. Central decision

**C — Partial comparability.**

Outcome B, conditional invariance, is correct for a fixed target semantics and a justified coordinate, quotient, causal, and resource mapping. It is not the best overall decision because genuinely transformational novelty can add classes with no old counterpart, and a transition in individuality can remove the shared generation clock. Some conserved causal consequences remain comparable, but the entire pre/post accessibility structure need not admit a total ordering.

A is rejected because no universal invariant was found. D is too strong because lumpability, bisimulation, exact causal transformations, and pathwise target-saturated projection provide positive cases. E is too strong because first-passage distributions remain coherent conditional scientific objects; what fails is unconditional cross-ontology transport.

This is a **measurement/formalization boundary**, not an OEE mechanism.

## 14. Remaining explanatory gap

The narrow gap is an empirically defensible procedure for constructing and validating **partial** correspondences among novelty classes, resource clocks, and initial ensembles around a real or artificial transition in evolutionary individuality—while allowing genuinely new classes to remain unmatched.

The required mathematics already exists in pieces: first-passage path laws, lumpability and bisimulation, semi-Markov memory, causal abstractions, stochastic ordering, and multilevel evolutionary bookkeeping. What is missing is not a scalar formula but evidence that proposed cross-transition mappings preserve the reproductive and hereditary causal consequences used to define the comparison, without prespecifying the higher-level individual or silently carrying forward an obsolete clock.

No reviewed OEE metric performs that validation. This is a bounded literature conclusion, not a proof that such a method cannot be constructed.

## 15. Known / Underexplored / Potentially Novel / Unknown

### Known / ESTABLISHED

- Invertible relabeling preserves first-passage distributions when process, target, initial law, and resource functional are transported together.
- Target-saturated projection preserves the hitting event pathwise; lumpability is needed for an autonomous first-order Markov quotient valid across initial distributions.
- Non-lumpable coarse-graining generally creates memory; semi-Markov, higher-order, milestoning, or history-augmented models can retain selected kinetics under explicit assumptions.
- Complete first-passage distributions contain finite-budget and tail information lost by a mean.
- Predictive, bisimulation, and intervention-based equivalences constrain coarse-grainings relative to specified observables, labels, outcomes, or interventions.
- MODES and evolutionary activity standardize realized-history measures after system-specific component, filter, and clock choices; they do not measure latent cross-transition accessibility.
- Major transitions change the reference of fitness and reproduction, so a generation is not a universal cross-level resource unit.

### Underexplored

- Validation of partial first-passage correspondences across observed changes in heredity or evolutionary individuality.
- How to transport matched neutral/shadow processes when the component ontology and selectable level change.
- Reporting standards that distinguish preserved comparisons, approximation error, and genuinely undefined new-class comparisons in OEE experiments.

### Potentially Novel

No scientific claim is retained. Combining established preservation conditions into an OEE-specific comparability protocol may be methodologically new after a dedicated methods review, but a missing protocol is not a hypothesis and this pass does not design one.

### Unknown

- Whether interventionally conserved evolutionary observables can be identified without prespecifying the post-transition individual.
- Whether any physically grounded resource relation is informative across several distinct transitions rather than one chosen case.
- How much of an accessibility structure remains comparable during, rather than only before and after, a transition with overlapping selective levels.

## 16. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

The result concerns conditions for measurement invariance and the domain of defined comparisons. It makes no new falsifiable claim about evolutionary dynamics. `HYPOTHESES.md` should therefore remain unchanged.

## 17. Highest-information next question

Can interventionally conserved reproductive and hereditary consequences identify a partial pre/post mapping through a transition in individuality without prespecifying the emergent higher-level individual?
