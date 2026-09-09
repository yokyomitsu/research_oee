# Q024 — Broad-scope evolvability

Theoretical research pass, 2026-09-08. Scope: one prior-art and counterexample audit of the exact frontier selected by Q023. This pass does not implement or simulate anything and does not perform Q025.

Epistemic convention: literature-supported claims are **Fact**. Cross-literature conclusions are **Interpretation**. Provisional notation is an analysis aid, not a new biological object or hypothesis.

## 1. Research question

> Can indirect selection retain a costly evolvability modifier across a change in the developmental or hereditary organization that determines which future variants it can generate, or must retention be supplied by recurrent environmental structure or tight linkage?

The question is read broadly enough to include a modifier embodied in regulatory, developmental, mutational, recombinational, or inheritance organization, but not so broadly that every organismal trait becomes a universal object called \(G_t\).

## 2. Prior-art boundary

The strongest boundary is the conjunction of three established research programs:

1. **Evolution of evolvability.** Mutation and recombination rates, pleiotropy, modularity, robustness, development, and genotype–phenotype maps can evolve and can alter the distribution of future heritable variation. Selection on a modifier may be direct or indirect through statistical association with the variants it helps produce. [Wagner & Altenberg 1996](https://doi.org/10.1111/j.1558-5646.1996.tb02339.x), [Hansen 2006](https://doi.org/10.1146/annurev.ecolsys.37.091305.110224), [Payne & Wagner 2019](https://doi.org/10.1038/s41576-018-0069-z)
2. **Facilitated variation.** Conserved core processes, weak regulatory linkage, compartmentation, exploratory processes, and robustness permit regulatory redeployment and reduce the chance that variation is globally disruptive. These properties can be favored for present developmental and physiological performance, with future evolvability as a by-product. [Gerhart & Kirschner 2007](https://doi.org/10.1073/pnas.0701035104)
3. **Evolutionary generalization.** Selection histories with recurring compositional structure can produce developmental organizations that respond well to unencountered combinations of familiar subproblems. Evolution-as-learning explains this as acquisition of inductive bias from environmental regularity. [Parter, Kashtan & Alon 2008](https://doi.org/10.1371/journal.pcbi.1000206), [Kouvaris et al. 2017](https://doi.org/10.1371/journal.pcbi.1005358), [Watson & Szathmáry 2016](https://doi.org/10.1016/j.tree.2015.11.009)

Modifier theory also supplies a destructive baseline. In broad classes of equilibrium models, selection tends to reduce mutation, recombination, dispersal, or other transformation rates; departures require features such as fluctuating selection, disequilibrium, association with selected backgrounds, or direct effects. Fluctuating environments can favor particular mutation/recombination regimes, but the outcome remains conditional on the fluctuation process and genetic association. [Carja, Liberman & Feldman 2014](https://doi.org/10.1073/pnas.1417664111), [Altenberg, Liberman & Feldman 2017](https://doi.org/10.1073/pnas.1619655114)

Therefore Q024 does not ask whether evolvability, its genetic architecture, or its generator can evolve. All three are prior art. It asks whether selection supplies a target-independent retention principle when the regularities and transmission relations that made an earlier generator useful no longer apply.

## 3. Parter-style generalization

Parter, Kashtan, and Alon trained networks on modularly varying goals composed from recurring subgoals. Networks evolved modularity and could solve previously unseen goals. Their operative condition was that varying goals shared a common “language”: new challenges recombined recurring building blocks. [Parter, Kashtan & Alon 2008](https://doi.org/10.1371/journal.pcbi.1000206)

Kouvaris and colleagues make the learning interpretation explicit. Their training and test phenotypes are drawn from one class of modular patterns; evolution internalizes correlations among phenotypic features, while environmental noise or connection costs regularize the learned architecture. Generalization succeeds when past environments are representative of structural relations in the larger class and can fail through underfitting or overfitting. [Kouvaris et al. 2017](https://doi.org/10.1371/journal.pcbi.1005358)

Thus the results are stronger than memorizing selected phenotypes but weaker than preparation for an arbitrary new task decomposition:

\[
E_i=f_i(s_1,\ldots,s_k)
\quad\Longrightarrow\quad
\text{generalization to new }f_j(s_1,\ldots,s_k).
\]

Some experiments include a subgoal not itself previously selected. This does not eliminate the boundary: the input variables, logic operations, developmental representation, fitness interpretation, and modular task-generating rule remain supplied. “Held out” is relative to that declared family.

## 4. Evolution-as-learning theory

Evolution-as-learning is the strongest attempted absorption. Watson and Szathmáry identify formal correspondences between selection and learning and argue that learning theory can organize questions about evolvability, development, ecological organization, and major transitions. Evolutionary connectionism further treats developmental, ecological, and reproductive relations as malleable association structures: recurrent selected correlations can become internalized as causal organization, including higher-level units during evolutionary transitions. [Watson & Szathmáry 2016](https://doi.org/10.1016/j.tree.2015.11.009), [Watson et al. 2016](https://doi.org/10.1007/s11692-015-9358-z)

This theory already contains representation change in an important sense. The learned interaction matrix is not merely a phenotype parameter; it changes which variants are generated together. Its scope nevertheless remains conditional on:

- a supplied state/representation space and update process;
- statistical regularity connecting selective history to later demands;
- a timescale on which the association structure can be learned;
- transmission sufficient for selected associations to persist.

Valiant's formal evolvability makes the conditionality particularly clear: evolvability is stated for a representation class, concept class, distribution, neighborhood relation, and performance criterion. Kanade, Valiant, and Vaughan prove robustness to gradually drifting targets, but every target remains in the same concept class, the distribution is fixed, and per-step drift is bounded. This is meaningful ongoing adaptation, not invariance to replacement of the representational language. [Valiant 2009](https://doi.org/10.1145/1462153.1462156), [Kanade, Valiant & Vaughan 2010](https://arxiv.org/abs/1005.3566)

## 5. Frank 2026

Frank distinguishes evolutionary memorization from generalization: a selected regulatory solution may fit historical challenges narrowly or capture structure that transfers across an abstract class. He proposes that overparameterized regulatory systems may generalize better, translating double-descent arguments into predictions that greater regulatory dimensionality and older circuits should associate with broader performance. The article explicitly maps regulatory connections to parameters, selective history to training data, selection to an optimizer, and novel environments to test data. [Frank 2026](https://doi.org/10.1093/evolut/qpag111)

The contribution is a concrete, comparative proposal about **within-class generalization**. Its limits for Q024 are decisive:

1. The class is the unspecified “potential set of environments” over which test performance is evaluated.
2. Increased parameterization supplies capacity and an implicit bias; it does not guarantee generalization under arbitrary distribution or concept shift.
3. The input–output circuit interpretation presupposes a correspondence between old and new tasks.
4. The account does not model replacement of the regulatory variables, developmental primitives, inheritance channel, or modifier–descendant association.
5. The article supplies predictions, not evidence that lineages retain evolvability through repeated evolutionary-regime changes; it reports no new data or model test.

**Interpretation.** Frank strengthens the challenge that Q023's residual may simply be generalization, but does not cross the relevant boundary. Regulatory dimensionality may improve performance over a broader declared class while remaining target/distribution relative. More parameters do not encode information about an unrelated future task language.

## 6. Fixed regularity family versus changing regularity structure

The distinction is defensible only conditionally. Let a task/environment sequence be generated by \(\mathcal D_t\), and let \(G_t\) denote a domain-specific organization of heritable variation. A fixed-family study holds stable enough structure that performance learned from earlier samples predicts later samples. A structural-shift study changes one or more independently declared components—relevant variables, task decomposition, developmental primitives, inheritance channel, or neighborhood of heritable changes—so that the old predictive relation is no longer adequate.

The inequality

\[
\mathcal D_t\not\approx\mathcal D_{t+1}
\]

is not self-interpreting. A shift that is arbitrary at one description can be regular at a richer description. Conversely, grouping two regimes into one “meta-distribution” can conceal the very representational change under study. The scientific content must therefore be stated through explicit train/test histories, admissible mappings, interventions on \(G\), and performance criteria.

This does not make the distinction empty. It prevents it from functioning as a universal binary. Developmental-system drift demonstrates that underlying developmental mechanisms may change while a phenotype is conserved; major-transition theory demonstrates local changes in inheritance and individuality. Neither fact guarantees higher evolvability after the change. [True & Haag 2001](https://doi.org/10.1046/j.1525-142x.2001.003002109.x), [Szathmáry 2015](https://doi.org/10.1073/pnas.1421398112)

## 7. Variation-generator change

Existing theory already explains numerous changes in \(G_t\):

- modifier alleles alter mutation and recombination;
- duplication, deletion, and regulatory rewiring change available molecular variation;
- genotype–phenotype maps and pleiotropic organization evolve;
- plastic responses can expose cryptic variation and undergo genetic accommodation;
- developmental mechanisms can drift beneath conserved phenotypes;
- major transitions can reorganize reproduction, inheritance, and selectable individuality.

Consequently, “structural reorganization” is not a missing phenomenon. Nor must \(G_t\) remain identifiable by a universal invariant. A domain-specific study can compare mutation kernels, developmental causal maps, or inheritance relations before and after a transition.

The exact Q024 modifier question has a simpler answer than Q023 anticipated. Selection does not retain a costly modifier because of an abstract capacity called broad-scope evolvability. It changes modifier frequency through current direct effects and through covariance with selected descendants. Tight physical linkage is one way to preserve that covariance, but not the only one: clonal descent, assortment, population structure, cotransmission, recurrent selection, and present functional benefits can do so. When developmental or hereditary organization changes, the old modifier may be lost, transformed, or reassociated with the new organization. No general law requires preservation of the same modifier identity.

## 8. No-free-lunch / conditionality boundary

No finite selection history supports systematic preparedness for every possible unrelated future. An evolutionary analogue of the learning no-free-lunch boundary follows without claiming that biological evolution samples all mathematical functions uniformly:

\[
\text{systematic test advantage}
\Longrightarrow
\text{some restriction or relation connecting history and test cases}.
\]

Wolpert's result shows that without a priori distinctions among possible learning problems, no learning algorithm has a universal off-training-set advantage. Domain-adaptation theory similarly requires assumptions connecting source and target domains. These are formal learning results, not direct biological mechanisms, but they expose the missing premise in “universal broad-scope evolvability.” [Wolpert 1996](https://doi.org/10.1162/neco.1996.8.7.1341), [Ben-David et al. 2010](https://doi.org/10.1007/s10994-009-5152-4)

The biological consequence is limited but firm. If later demands are entirely independent of every transmitted feature and recurrent environmental relation, indirect selection cannot preferentially retain a costly present modifier for those demands. If a larger-scale regularity links regimes, selection or learning may exploit it—but the claim is then conditional generalization over that larger process, not target-free preparedness.

Therefore:

\[
\boxed{\text{OEE cannot require preparedness for arbitrary future novelty.}}
\]

It may instead require repeated discovery and reconstruction of locally useful variational organization as structured opportunities arise. That is compatible with temporary specialization, loss of old competence, bottlenecks, and nonmonotonic evolvability.

## 9. Generalization under structural shift

Closest theory covers three increasingly demanding cases:

1. **Novel samples/combinations under a stable family:** established by Parter-style and Kouvaris-style models.
2. **Gradual target drift within a fixed concept and representation class:** formally tractable in evolvability-with-drifting-targets theory.
3. **Change of representation, developmental map, or inheritance process:** established as a biological phenomenon and modeled in domain-specific evolution-of-evolvability and transition theories.

No reviewed theory guarantees predictive continuity when the task class, representation, and transmission relation all change without bounded correspondence. That absence is not by itself a mechanism gap, because without such correspondence there is nothing selection could systematically learn or retain. With a declared correspondence, the problem becomes a domain-specific instance of modifier dynamics, adaptation under nonstationarity, developmental evolution, or transition theory.

The term “second-order generalization” is therefore unnecessary. Evolution of evolvability already covers change in the variational basis; generalization covers transfer justified by shared structure; drifting-target theory covers one formal kind of changing demand. Their union leaves a requirement to state the cross-regime regularity, not evidence for a further evolutionary force.

## 10. Current utility and future evolvability

Facilitated variation provides the best non-foresight mechanism:

\[
\text{present robustness, regulation, or physiological utility}
\longrightarrow
\text{organization with incidental future versatility}.
\]

Weak linkage and exploratory processes work now: they stabilize development, coordinate response, and reduce harmful coupling. Their future benefits need not be directly anticipated. This can maintain properties that later increase accessibility. [Gerhart & Kirschner 2007](https://doi.org/10.1073/pnas.0701035104)

The mechanism can also recur after an architectural change whenever analogous present benefits favor new weak linkages, redundancy, exploratory control, or modular organization. What does not follow is that the same modifier persists, that every reorganization exposes the same design principle, or that current utility is positively correlated with every distant novelty family. The principle explains repeated **local rebuilding under recurring functional pressures**, not universal retention across arbitrary regime changes.

Modifier results reinforce this point. Environmental fluctuation can favor increased rates of mutation or recombination, whereas stable equilibrium conditions often favor their reduction. Natural selection has no general obligation to maximize future adaptability, and long-term benefits can lose to short-term load. [Earl & Deem 2004](https://doi.org/10.1073/pnas.0404656101), [Clune et al. 2008](https://doi.org/10.1371/journal.pcbi.1000187), [Altenberg, Liberman & Feldman 2017](https://doi.org/10.1073/pnas.1619655114)

## 11. Conserved cores and changing primitives

Facilitated variation's conserved core processes supply versatile primitives whose internal conservation permits freer regulatory recombination. This is not a logical commitment to an eternally fixed vocabulary: duplication, divergence, co-option, developmental-system drift, and transitions in inheritance can create or replace components. Yet conservation creates genuine path dependence. A core can enable many recombinations precisely because changes to it would disrupt many dependent processes.

Thus “today's core becomes tomorrow's evolvable substrate” is possible in particular histories but not a general requirement. Change may occur by:

- duplication followed by divergence, retaining an old copy while a new one changes;
- regulatory co-option, altering context before internal mechanism;
- compensatory developmental drift under stabilizing selection;
- hierarchical incorporation of lower-level units;
- replacement of transmission mechanisms during a major transition.

These are established routes to new primitives or new organization. None guarantees an endless sequence or monotonic increase in evolvability. The constraint–freedom relation is a trade-off, not an anti-closure theorem.

## 12. Candidate mechanisms

The labels below concern evidence for crossing at least one explicitly defined change in task or variational organization. **ESTABLISHED CROSS-STRUCTURAL** does not mean sufficient for OEE.

| Candidate | Classification | Boundary |
|---|---|---|
| Modularity | **FIXED-LANGUAGE ONLY** | Strong generalization demonstrations recombine a supplied module vocabulary; modules can later constrain novelty. |
| Weak regulatory linkage | **POSSIBLY CROSS-STRUCTURAL** | Permits redeployment across contexts, but repeated efficacy after replacement of core organization is not established. |
| Robustness | **POSSIBLY CROSS-STRUCTURAL** | Can preserve cryptic variation through environmental change; its effect can reverse with population and landscape conditions. |
| Exploratory processes | **POSSIBLY CROSS-STRUCTURAL** | Adaptive state-finding can buffer novel contexts, but relies on conserved process organization. |
| Developmental plasticity / genetic accommodation | **POSSIBLY CROSS-STRUCTURAL** | Novel environments can expose variation and reorganize regulation; no general retention across inheritance changes follows. |
| Overparameterization / regulatory dimensionality | **INSUFFICIENT EVIDENCE** | Frank supplies a prediction; comparative and cross-shift biological tests are not yet supplied. |
| Hierarchy | **POSSIBLY CROSS-STRUCTURAL** | Major transitions establish local changes in level; repeated predefined levels do not explain OEE. |
| Gene duplication and divergence | **ESTABLISHED CROSS-STRUCTURAL** | Can create new molecular components and alter the variational vocabulary in domain-specific cases. |
| Evolution of genotype–phenotype maps | **ESTABLISHED CROSS-STRUCTURAL** | Map architecture can change which phenotypes mutations produce; sustained broad performance is not guaranteed. |
| Changing inheritance mechanisms | **ESTABLISHED CROSS-STRUCTURAL** | Major transitions and inheritance-system evolution establish local replacement/addition of channels; they do not guarantee future transitions. |

No row establishes a target-independent retention process. Several establish that structural crossing happens, so Q024 cannot classify the phenomenon itself as unknown.

The classifications rely on scoped results rather than labels: quantitative-genetic theory shows that plasticity can rise after an extreme environmental shift and later be genetically assimilated, while duplication theory supplies multiple routes by which a retained copy can diverge or partition ancestral functions. Both cross a local organizational change; neither predicts general performance after unrelated later changes. [Lande 2009](https://doi.org/10.1111/j.1420-9101.2009.01754.x), [Innan & Kondrashov 2010](https://doi.org/10.1038/nrg2689)

## 13. Strong counterexamples

| Case | Counterexample | Consequence |
|---|---|---|
| **A** | Networks generalize to unseen combinations of subgoals sampled from the same supplied modular language. | Excellent generalization can fail to test a changed decomposition. |
| **B** | An architecture's modules become highly integrated dependencies and constrain changes not expressible by the old vocabulary. | Modularity can improve local access while narrowing later routes. |
| **C** | An overparameterized learner performs well in-distribution but fails after unsupported concept or distribution shift. | Parameter count alone does not supply cross-regime information. |
| **D** | A mutator hitchhikes during adaptation, then loses association or is selected against through deleterious load, recombination, or environmental stabilization. | High short-term evolvability does not ensure retention. |
| **E** | A major transition creates a new inheritance or individuality regime while producing dependence, conflict-control costs, or loss of lower-level autonomy. | Generator reorganization has no universally positive effect on later evolvability. |
| **F** | Developmental-system drift and evolution of genotype–phenotype maps change mechanisms repeatedly while phenotypes remain viable. | Structural generator change exists without proving broadening or OEE. |
| **G** | Evolvability with drifting targets supports indefinite tracking by a finite fixed process when targets drift slowly inside a fixed concept/representation class. | Sustained adaptation does not require changing primitives, while the formal guarantee ends at the class boundary. |

Two further negative controls sharpen the modifier question. A costless modifier can persist neutrally without causing future adaptation, so persistence is insufficient. A useful variational organization can disappear and later be independently rebuilt, so retention of the same component is not necessary for continued evolution.

## 14. Prior-art absorption test

Adversarial claim:

\[
\text{Q023 gap}
=
\text{evolution of evolvability}
+
\text{generalization}
+
\text{facilitated variation}.
\]

The conjunction absorbs the scientifically coherent target:

- evolution-of-evolvability theory explains changes in the production and transmission of variation;
- modifier theory specifies how direct effects and associations with selected descendants determine retention;
- facilitated variation explains how present utility can incidentally maintain versatile organization without foresight;
- evolutionary generalization explains transfer when environmental histories share learnable structure;
- drifting-target theory proves that ongoing tracking is possible under an explicit bounded change process;
- developmental and major-transition theories establish local replacement of maps, components, and inheritance organization.

The conjunction does **not** guarantee success after arbitrary replacement of the regularities, representation, and transmission relations. But that remainder cannot be demanded of any adaptive process: it removes the information and causal association required for systematic selection. Calling its absence a mechanism gap would turn lack of a premise into a missing biological force.

**Conclusion.** F3 does not survive as a general OEE mechanism frontier. Its coherent cases are conditional instances of established theory; its unconditional form violates a no-free-lunch boundary. A useful research program may compare specified structural shifts, but it must declare the continuity or regularity being exploited.

## 15. Deep-learning contribution

\[
\boxed{\textbf{ANALOGY ONLY}}
\]

Distribution shift, representation learning, meta-learning, and continual-learning language clarify why within-family holdout performance differs from performance after a structural shift. Modern learning theory also makes the no-free-lunch premise conspicuous. It adds no evolutionary mechanism beyond evolution-as-learning, evolution of genotype–phenotype maps, plasticity, and modifier theory. Meta-learning remains relative to a task/meta-distribution; continual learning adds a stability–plasticity problem already represented biologically by robustness, plasticity, and entrenchment; no neural architecture is imported.

## 16. Central decision

\[
\boxed{\textbf{E — NO-FREE-LUNCH LIMIT}}
\]

Broad-scope evolvability beyond every fixed or higher-order regularity family is not a coherent general requirement. Systematic transfer requires some shared restriction, correspondence, environmental recurrence, present utility, or transmission association. Once that structure is declared, the problem is conditional evolvability/generalization rather than an independent OEE mechanism.

## 17. Mechanism readiness

\[
\boxed{\textbf{NOT READY}}
\]

The unconditional target is incoherent; the conditional target is a family of already recognized, domain-specific problems. A new mechanism would require a stable scope, a specified regime-change process, and a causal prediction not absorbed by modifier, developmental, transition, or learning theory. None emerged in this pass.

## 18. Remaining explanatory gap

The narrow residue is a formalization question:

> For a specified sequence of developmental or hereditary regimes, what transmitted correspondence or environmental regularity makes performance before a regime change informative about resource-feasible adaptation after it?

This is not a demand that the same costly modifier persist. Recurrent environmental structure and tight linkage are sufficient routes in some models, but neither is individually necessary. Some continuing causal/statistical association—through descent, cotransmission, structure, direct current utility, or recurrence—is necessary for systematic indirect selection. Without it, retention can occur only neutrally, by drift, or accidentally, not because of future evolvability.

## 19. Problem classification

\[
\boxed{\textbf{FORMALIZATION}}
\]

The remaining work is to specify the relation between regimes, not to posit an unexplained generator. A domain may then expose a validation or mechanism problem, but Q024 found no general mechanism gap.

## 20. Known / Underexplored / Potentially Novel / Unknown

- **ESTABLISHED:** evolvability and genotype–phenotype maps evolve; indirect modifier selection depends on direct effects and association with selected backgrounds; recurring environments can select generalizable organization; facilitated variation can make future versatility a by-product of present utility; developmental and inheritance organization can change.
- **PARTIALLY EXPLORED:** adaptation to gradual target drift; plasticity and genetic accommodation in novel environments; developmental-system drift; evolution of inheritance during major transitions; comparative scope of broad versus narrow evolvability determinants.
- **UNDEREXPLORED:** matched, domain-specific comparisons of retained or rebuilt evolvability across an explicitly defined change in developmental or hereditary representation.
- **POTENTIALLY NOVEL:** none. No new causal relation survives the firewall.
- **UNKNOWN:** which regularities and transmission relations account for particular long natural histories; whether any empirical lineage repeatedly crosses independently defined structural shifts while maintaining resource-feasible adaptive access.

## 21. Hypothesis decision

\[
\boxed{\textbf{NO HYPOTHESIS JUSTIFIED}}
\]

Claims that fixed-language generalization has limits or that modifiers require association are prior art or logical boundary conditions. No specific new dynamical relation passes the novelty and counterexample tests. `HYPOTHESES.md` remains unchanged.

## 22. Highest-information next question

> Is maintaining evolutionary identity while altering the organization that generates heritable variation a mechanism problem beyond established robustness–evolvability, facilitated-variation, plasticity, canalization, and developmental-system-drift theory?

This question is recorded only as the next frontier. It is not investigated here.
