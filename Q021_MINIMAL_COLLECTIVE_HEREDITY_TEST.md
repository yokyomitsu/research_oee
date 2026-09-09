# Q021 — Minimal collective-heredity test

Theoretical research pass, 2026-09-08. Scope: validation and formalization of the smallest evidential step from short-range collective parentage to collective heredity in the Fernandes–Vroomans–Colizzi system. This pass uses independent theory and the published manuscript and supplement only. It does not run or modify the model, inspect its source code, perform the proposed analysis, search for a mechanism of higher-level individuality, or perform Q022.

Epistemic convention: source claims and reported measurements are **Fact**. Cross-framework judgments and the proposed assay are **Interpretation / analysis specification**. Counterfactual examples are **Thought experiments**. No new scientific **Hypothesis** is introduced.

## 1. Research question

> What is the minimum theoretically justified evidence needed to extend one-generation collective parentage into genuine collective heredity and higher-level Darwinian evolutionary potential?

The immediate discriminator is narrower:

\[
\text{genealogical collective reproducer only}
\quad\text{versus}\quad
\text{heritable collective reproducer}.
\]

Differential collective reproductive consequence is then an additional relation required for collective-level selection; reproductive autonomy remains a separate axis.

## 2. Why Q020 stops at genealogical reproduction

Q020 established a direct local relation in one Fernandes regime:

\[
C_{\mathrm{source}}
\rightarrow p_{\mathrm{single\ cell}}
\rightarrow C_{\mathrm{newborn}}.
\]

The source collective supplies a cell, that cell divides, and its daughters re-express adhesion and form a newborn collective. This is a genuine causal parentage edge, not mere temporal recurrence. The single cell can be a stage in the collective life cycle.

The publication does not show that a newborn collective later becomes a parent in the same tracked pedigree, pair parent and offspring collective phenotypes, or estimate whether parental collective differences predict offspring differences. Its phylogenies concern cells; its evolved “lineages” are cell-genetic lineages or populations represented by cellular MRCAs. One edge therefore establishes a reproductive event but not a transmitted collective difference or an evolutionarily persistent collective lineage. [Fernandes, Vroomans & Colizzi 2026, uncertified preprint v3](https://doi.org/10.1101/2025.10.08.681199), [Q020](Q020_FERNANDES_COLLECTIVE_INDIVIDUALITY.md)

## 3. Independent theory of collective heredity

Lewontin-style Darwinian requirements concern relations in a population, not labels attached to one object:

1. candidate entities vary in a declared character;
2. they reproduce or otherwise contribute to a later population;
3. parental differences are transmitted or predictably reconstructed in descendants;
4. those differences have differential reproductive consequences if selection is claimed.

Q020 supplies item 2 locally. For a collective trait \(Z\), the minimum heredity claim requires all of the following:

- an independently declared collective unit and reproductive-stage rule;
- a causal parentage relation from parental to offspring collectives;
- between-parent variation in \(Z\);
- measurement of \(Z\) in linked parents and descendants;
- parent-specific predictive resemblance relative to appropriate nonparent controls in the same stated environment;
- concatenation of reproductive edges so that at least some offspring are observed as later parents.

The last condition is structural rather than an arbitrary generation threshold. A parent–offspring cohort with many families can estimate transmission across one transition, but if all offspring terminate there it does not demonstrate that the relation can carry a collective lineage. The logical minimum is at least one replicated set of concatenated edges—offspring that themselves reproduce. The number of chains and their depth must then be set by identifiability, uncertainty, temporal autocorrelation, and the desired generalization, not by a universal number of generations. No independent theory located specifies such a universal number.

Heritability is population-, trait-, environment-, genealogy-, and measurement-specific. A regression slope, variance component, or transmission kernel may quantify it, but no particular estimator is constitutive. The core claim is that variation among declared parents contains information about variation among their causal descendants under specified conditions. [Lewontin 1970](https://doi.org/10.1146/annurev.es.01.110170.000245), [Bourrat 2015](https://doi.org/10.1093/bjps/axu015), [Herron, Zamani-Dahaj & Ratcliff 2018](https://doi.org/10.1186/s12915-018-0612-6)

## 4. MLS1 / MLS2 caution

**Fact.** Bourrat argues that the usual MLS1/MLS2 distinction should not be treated as two objectively decoupled material processes. For a finite physical collective in one environment, particle and collective reproductive outputs must in principle be connected by a map. MLS1 and MLS2 descriptions differ importantly in practical tractability and predictive usefulness, especially as particle-to-collective character and fitness mappings become complex, but the label chosen does not create a new process. [Bourrat 2023](https://doi.org/10.1007/s11229-023-04285-1)

Accordingly, Q021 does not use either of these as a success condition:

\[
\text{“MLS2 detected”},
\qquad
\text{“fitness-2 exists”}.
\]

The underlying evidential relations are instead:

\[
\boxed{
\text{declared collective genealogy}
+\text{ variable }Z
+\text{ parent-specific transmission of }Z
}
\]

for heredity, and additionally

\[
\boxed{
\text{transmitted }Z
\text{ predicts mapped reproductive contribution}
}
\]

for a selection claim. Calling the latter MLS2 may be convenient after those relations are established; it cannot substitute for establishing them.

## 5. Collective genealogy

The genealogical units must be fixed before any resemblance statistic is calculated. Q019's domain supplies the admissible life-cycle stages. For the primary regime, define:

- a **parent collective** as a connected migrating collective immediately before regulated propagule detachment;
- the **propagule path** as the detached cell and its cellular descendants;
- an **offspring collective** as the first connected multicellular stage reconstructed by those descendants after adhesion is reactivated.

These event boundaries use the reported life-cycle semantics rather than a target-aware similarity rule. A descendant is not assigned because it resembles a parent; it is assigned because tracked material and cell descent causally connect them.

For aggregation and fusion, use a material-contribution relation rather than majority ancestry. Let

\[
A_{ij}\geq 0
\]

record the amount or fraction of the founding material of offspring collective \(j\) descended from parent collective \(i\). An edge exists for every nonzero tracked contribution. This produces a directed temporal parentage network or hypergraph: one parent can contribute to several offspring and one offspring can have several parents. The measured cell-flow contribution is the ancestry relation; no arbitrary “largest contributor wins” threshold is required. Bourrat's multiple-parent collective models use precisely the possibility that offspring particles from several parental collectives assemble an offspring collective. [Bourrat 2019](https://doi.org/10.1007/s12064-019-00294-2)

Four evidential levels then remain distinct:

| Evidence | Minimum topology | Establishes |
|---|---|---|
| one successful reconstruction | one edge \(C_0\to C_1\) | one reproductive event |
| recurrent collective reproduction | multiple qualifying edges | the process recurs, but edges may be genealogically disconnected |
| continuing collective lineage | concatenated edges in which offspring later act as parents | collective descent persists beyond one event |
| evolutionary lineage potential | replicated continuing lineages with variable, predictively transmitted \(Z\) | collective heredity; differential consequence is still separate |

## 6. Reticulate versus propagule genealogy

Reticulation does not make heredity undefined. For a many-parent offspring, the predictor can be the vector of parental trait values and measured contributions, or a theory-justified contribution-weighted parental value. Both preserve all parents. The analysis must report sensitivity to the declared material unit—cell count, inherited biomass, or another biologically justified contribution—rather than silently changing ancestry definitions.

Reticulation does make inference harder. If an offspring continually incorporates unrelated cells, its trait may depend nonlinearly on composition, and a parent can contribute too little to predict the offspring. Bourrat shows that additive collective traits can retain mathematically high heritability even under extensive mixing, whereas nonlinear collective traits become frequency- and population-structure-dependent. Parent-specific offspring variance or fidelity is therefore more informative for individuality than a positive aggregate \(h^2\) alone.

The single-cell-propagule interval is the cleanest Fernandes case. At detachment and initial reconstruction, all founding material of the newborn cluster descends through one cell from one source cluster, so \(A_{ij}=1\) for that local edge. If the newborn later fuses with other collectives, unique parentage ends at the merger; subsequent descent is reticulate and must retain all contributing edges. Genealogy should be censored at an unobserved merger, not statistically repaired.

## 7. Collective trait definition

A legitimate \(Z\) must be declared before examining transmission, vary among collectives, be measurable in a parent and its descendants at homologous life-cycle stages, and recur when descendants themselves reproduce.

| Fernandes candidate | Level audit | Q021 use |
|---|---|---|
| cellular GRN parameters or one cell's adhesion expression | assignable to an isolated cell | inherited realizer, not the focal collective trait |
| median adhesion between cell states | reported for a cellular lineage/population, computed from cell profiles | potential mechanistic predictor; not currently an individual-collective phenotype |
| cluster size | genuinely collective and reported for sampled clusters | valid secondary trait, but not the closest measure of the reproductive organization at issue |
| collective chemotactic motion | depends on relations and forces among several cells | valid collective functional trait, but no parent–offspring measurement is reported |
| whole-population spatial dispersion | measured over the cell population | not an individual-collective trait |
| life-cycle / propagule-production mode | realized only by a source collective producing and reconstructing another collective | **primary focal trait** |
| reproductive timing | definable from state transitions | not reported as a parent–offspring collective phenotype |

The narrow focal trait is:

\[
Z(C)=\text{the propagule-production organization realized when }C\text{ reproduces},
\]

using the paper's categories, with the primary state being regulated single-cell release followed by newborn-cluster reconstruction. It cannot be assigned to an isolated cell: a cell may carry the regulatory program, but \(Z\) is realized only by its state-dependent relation to a source cluster and a reconstructed offspring. Measuring \(Z(C_1)\) requires observing \(C_1\) later reproduce, which makes a concatenated lineage part of the trait definition rather than an arbitrary demand for more time.

If every observed parent has the same \(Z\), transmission is not estimable in that population. Repeatability of a monomorphic mode may demonstrate developmental fidelity but not heritable variation. A secondary continuous trait such as propagule size or event timing may be used only if it is predeclared and shown to vary; Q021 does not substitute one merely to force a positive result.

## 8. Reconstruction through lower-level heredity

Collective heredity can be reconstructive:

\[
C\rightarrow p\rightarrow C',
\]

even though the mature collective phenotype is absent during the unicellular stage. The propagule may inherit lower-level information that, through development and ecology, reconstructs \(Z(C')\). Metazoan organismal heredity through gametes and a zygote is the decisive ordinary case; snowflake yeast is a nascent case in which cell genotype and clonal development reconstruct highly heritable cluster traits. Direct material preservation of the mature phenotype and a separate group genome are not required. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112), [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102), [Zamani-Dahaj et al. 2023](https://doi.org/10.3390/genes14081635)

Fernandes' inherited cell GRN can therefore implement collective heredity in principle. The decisive question is not whether the causal information is molecularly located “at the group level,” but whether inherited lower-level differences carried along the independently defined collective pedigree generate predictable differences in offspring collective \(Z\).

An entirely lower-level inheritance mechanism is compatible with nascent collective heredity. Greater higher-level autonomy would later be indicated by features such as dedicated propagule allocation, developmental control that stabilizes transmission against variation in composition and environment, cotransmission of required partners, reduced lower-level opportunity for independent evolution, or a collective-level inheritance channel not replaceable by arbitrary cell dispersal. Those are degrees and mechanisms of individuality, not prerequisites for detecting the initial transmission relation.

## 9. Parent–offspring resemblance

For a unique-parent edge, a covariance, regression, variance-component model, or nonparametric predictive comparison can ask whether

\[
Z(C_i)\quad\text{predicts}\quad Z(C_j),\qquad C_i\to C_j.
\]

For several parents, use the full parent-contribution vector or a predeclared contribution-weighted predictor based on \(A_{ij}\). The estimator is secondary to these interpretation conditions:

1. parent and offspring were assigned causally, without reference to \(Z\);
2. \(Z\) is measured at homologous collective stages;
3. there is between-parent variation and more than one independent parental lineage event;
4. siblings and repeated offspring are not treated as independent parents;
5. relevant food environment and temporal autocorrelation are represented;
6. linked pairs predict better than nonparent pairs exposed to the same environmental regime;
7. inherited cell genotype/composition is recorded as a candidate transmission pathway, not conditioned away as though lower-level implementation invalidated collective heredity.

Resemblance among all clusters in one deterministic environment is not genealogical transmission. Conversely, a parental environmental modification that is itself causally transmitted to offspring may constitute ecological inheritance. The test must therefore separate an externally reset common cause from parent-mediated environmental transmission. Quantitative-genetic work shows that shared environments can strongly inflate resemblance; extended inheritance theory shows that genuine parent-mediated nongenetic effects can contribute to evolutionary transmission. [Kruuk & Hadfield 2007](https://doi.org/10.1111/j.1420-9101.2007.01377.x), [Bonduriansky & Day 2011](https://doi.org/10.1086/660911), [Lynch & Bourrat 2017](https://doi.org/10.1086/688933)

No universal positive slope or \(h^2\) threshold is introduced. The claim is a supported directional/predictive transmission relation with uncertainty reported for its specified population and environment.

## 10. Between-lineage variation

Heritability cannot be inferred from a single phenotype or a monomorphic set of parents. The data must include multiple collective parents that differ in \(Z\), and their causally linked descendants, within the population about which heredity is claimed.

Fernandes reports variation among 72 independent evolutionary simulations, among cellular MRCAs extracted from those simulations, and among transferred cellular lineages. These are valuable demonstrations that different cell-genetic strategies can evolve. They are not collective generations. Starting 100 cloned cells from an MRCA and recovering a life-cycle phenotype tests a genotype-to-population reconstruction map; it does not pair a parent collective with its offspring collective. Differences among independent runs cannot be substituted for transmission along one collective genealogy.

Pooling independent runs could estimate how different cellular genotypes generate different collective phenotypes under a common protocol. It could not, without an explicit collective parentage relation within each run, establish collective heredity.

## 11. Differential collective reproduction

Heredity and selection must be tested in that order. Once a pedigree and variable \(Z\) are established, lower-level events can be mapped to the reproductive contribution of each collective without adding a primitive group-fitness variable to the simulator. A Price-style mapping assigns each parental entity a contribution to the descendant population and separates covariance between parental character and contribution from change during transmission. In a reticulate pedigree, contribution can be fractional and must follow the same material ancestry matrix used to define parentage. [Frank 2012](https://doi.org/10.1111/j.1420-9101.2012.02498.x), [Bourrat 2023](https://doi.org/10.1007/s11229-023-04285-1)

Candidate consequences supported by the declared life cycle include the number of successfully reconstructed descendant collectives, the probability or rate of completing the propagule cycle, and persistence of the resulting collective lineage. Which is used must be declared from the stage graph and observation window; Q021 does not invent one scalar “true group fitness.” Fernandes' reported steady-state food-depletion fitness and cell-lineage invasion do not provide this mapping.

A stronger higher-level result would combine:

\[
\text{heritable variation in }Z
+\text{ differential mapped contribution}
\longrightarrow
\text{a predicted change in the descendant }Z\text{ distribution}.
\]

An observed response across repeated collective transitions is strong evidence that the collective description is evolutionarily useful. It is not necessary for the narrower heredity claim: heritable neutral variation can exist without differential reproduction. Nor is one observed mean shift sufficient for Darwinian individuality, because drift, transmission bias, or an environmental trend can also shift a distribution. Autonomy and causal control remain additional questions.

## 12. Reproductive autonomy

Collective heredity does not entail reproductive autonomy. Externally passaged Pseudomonas collectives can show lineage-level transmission and response to collective selection while the imposed patch cycle supplies much of their reproduction. Bourrat therefore separates reproducees, reproducers with background-relative autonomy, and Darwinian individuals with stronger reproductive causal control. [Hammerschmidt et al. 2014](https://doi.org/10.1038/nature13884), [Bourrat 2025](https://doi.org/10.1007/s11229-024-04880-w)

Fernandes has more endogenous reproductive organization than an externally passaged system: evolved cell-state regulation controls adhesion and propagule release. That supports partial autonomy. It neither supplies the missing heredity evidence nor needs to be fully autonomous before collective heredity is measurable. Q021 therefore does not add an autonomy threshold to its minimal assay.

## 13. Fernandes single-cell-propagule case

This is the strongest and narrowest test case because initial ancestry is unambiguous:

1. identify the connected source collective immediately before a regulated dividing cell detaches;
2. trace that cell and its daughters materially;
3. identify the first newborn connected collective formed by those descendants;
4. retain the edge as uniquely parented until an independently detected merger;
5. observe whether the newborn later acts as a parent and record its own \(Z\).

The focal phenotype is the realized propagule-production organization. The inherited GRN is a plausible reconstructive pathway, but the test asks whether the phenotype follows the collective pedigree, not merely whether cloned cells can express the relevant adhesion states.

The test succeeds as evidence of collective heredity only if there are variable parental \(Z\) values and parent-specific prediction across replicated, concatenated edges beyond same-environment nonparent resemblance. If regulated single-cell propagation is monomorphic, the result is **not identifiable for heredity** in that sample, even if every cycle is reconstructed perfectly.

## 14. Negative control regime

**One negative control: the high-adhesion, strictly multicellular regime with rare physical tearing.**

It contains recurrent multicellular structure and collective chemotaxis, but clusters aggregate extensively and rarely split through an unregulated physical event. Under the proposed rule, a pedigree edge is recorded only when tracked material crosses an independently identified split and reconstructs a qualifying offspring stage. If later clusters are formed by unrecorded merging or if no offspring becomes a parent, the heredity statistic is **undefined / unsupported**, not zero and not forcibly assigned through spatial proximity or phenotypic similarity.

This control tests the specification's restraint:

\[
\text{recurrent multicellular structure}
\not\Rightarrow
\text{measurable collective heredity}.
\]

## 15. Minimum decisive analysis

**Exactly one analysis: a pedigree-indexed, concatenated transmission assay for realized propagule-production organization in the single-cell-propagule regime.**

Under the stage definitions in Section 5, record every source-cluster → propagule → newborn-cluster event at sufficient temporal resolution, preserve all material-contribution edges at splits and mergers, and follow newborns until they either reproduce, merge, die, or are censored. For multiple collective parents, retain the complete contribution vector. Measure

\[
Z(C)=\text{realized propagule-production organization when }C\text{ reproduces}
\]

for variable parental collectives and for descendants that later reproduce. Then test whether the contribution-linked parental \(Z\) predicts descendant \(Z\) better than contemporaneous nonparent collectives in the same food environment, with family structure and temporal dependence respected.

This single analysis is minimal because it tests only the missing relation—parent-specific collective transmission. It does not require a collective-selection treatment, a Price decomposition, an autonomy intervention, a new environment, or a new numerical threshold. It produces three legitimate outcomes:

- **SUPPORTED:** variable parental \(Z\) predicts descendant \(Z\) across replicated concatenated edges beyond the nonparent/environmental control;
- **NOT SUPPORTED:** defensible genealogy and variation exist, but parentage provides no predictive transmission;
- **NOT IDENTIFIABLE:** genealogy cannot be assigned, \(Z\) does not vary, descendants do not reproduce, or observation ends after isolated edges.

Only the first discriminates a heritable collective reproducer from Q020's genealogical reproducer. Differential collective contribution is the next relation, not part of this minimum test.

## 16. Data availability audit

The audit concerns evidence described in the manuscript and supplement; the linked source code was not inspected.

| Required object | Published basis | Classification | Consequence |
|---|---|---|---|
| instantaneous cell identity and geometry | Cellular Potts cells are sets of lattice sites sharing a spin; positions of all cells are periodically recorded | **AVAILABLE IN MODEL STATE BUT NOT ANALYZED** for pedigree purposes | connected collective membership can in principle be derived at a time point |
| instantaneous collective boundaries | cluster size is measured; Supplementary Fig. S3 assigns a unique color to each final-time cluster | **AVAILABLE IN REPORTED OUTPUT** at sampled times | the paper can identify clusters, but not persistent collective individuals |
| cell mother–daughter ancestry | mutations/inheritance occur at division; cellular phylogenies and MRCAs are reconstructed | **AVAILABLE IN MODEL STATE BUT NOT ANALYZED** for collective descent | material propagation through the single-cell stage is in principle traceable |
| one propagule origin and newborn collective | Figure 3 and Video S2 show the source cluster, detached cell, division, and newborn cluster | **AVAILABLE IN REPORTED OUTPUT** for a representative event | establishes Q020's local edge only |
| population-wide propagule origins | no event table pairs every propagule with a source cluster | **WOULD REQUIRE NEW MODEL INSTRUMENTATION** under the published output description | representative trajectories cannot estimate transmission |
| persistent split/merge collective identities | no collective IDs, birth/death records, or merger ancestry are reported | **WOULD REQUIRE NEW MODEL INSTRUMENTATION** | the minimal pedigree cannot be recovered from reported summary outputs |
| cadence adequate to resolve every event | non-evolutionary positions are reported every 20,000 time steps; division growth itself lasts 20,000 steps; video/output cadence and raw retention are not specified as a complete event log | **UNKNOWN** | periodic snapshots may miss detachment, merger, or short-lived stages |
| individual-collective \(Z\) paired across descent | life-cycle mode is classified for cellular lineages/populations from adhesion profiles, not for pedigree-linked collectives | **WOULD REQUIRE NEW MODEL INSTRUMENTATION** | the reported phenotype table cannot be reused as parent–offspring data |
| environmental covariates | food-patch state, chemoattractant, reserves, and cellular state exist in the model; reported EC is known | **AVAILABLE IN MODEL STATE BUT NOT ANALYZED** for heredity | same-environment and temporal controls are conceptually available |
| raw saved trajectories sufficient for retrospective reconstruction | code location and parameters are published, but data-availability text does not establish a complete archived event history | **UNKNOWN** | source inspection or rerunning would be needed to decide; neither is done here |

The runtime model contains the local variables from which a collective pedigree could be constructed, but the published recording protocol does not establish that the required high-resolution histories already exist. The theoretical test is clear; its execution requires additional collective-lineage recording unless a currently undocumented complete trajectory archive exists.

## 17. Counterexamples

| Attack | Case | Result for the criterion |
|---|---|---|
| **A — resemblance from identical environments** | Unrelated deterministic collectives placed in the same externally reset food field can converge on the same phenotype; quantitative-genetic studies likewise show common environment can inflate relative resemblance. | Same-environment nonparent comparison and environmental covariates are required; raw resemblance is insufficient. [Kruuk & Hadfield 2007](https://doi.org/10.1111/j.1420-9101.2007.01377.x) |
| **B — reconstructed trait without variation** | A monomorphic clone can reconstruct the same collective form perfectly in every cycle. | Developmental fidelity is present, but population heritability and selectable variation are not identifiable. |
| **C — heredity without differential reproduction** | A faithfully transmitted neutral collective color or morphology has no effect on reproductive contribution. | Collective heredity is supported; collective selection on that trait is not. |
| **D — persistence without heredity** | Environmentally induced high-adhesion clusters can persist differentially across patches while producing no pedigree-linked offspring with transmitted differences. | Differential persistence alone does not establish generational collective heredity; Bourrat's temporal-heredity analysis shows that persistence and reproduction must be stated separately. [Bourrat 2015](https://doi.org/10.1093/bjps/axu015) |
| **E — nascent individual without separate inheritance machinery** | Early snowflake yeast inherits cell genotype and reconstructs group size at reproduction with high group-level heritability. | A distinct group genome is not necessary for nascent collective heredity. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102) |
| **F — single-cell bottleneck with organism heredity** | Sexual metazoan parent → gamete/zygote → multicellular offspring. | Material disappearance of the mature phenotype during the bottleneck does not terminate organism-level heredity. |
| **G — meaningful heredity with multiple founders** | Bourrat's multiple-parent collective models permit parent–offspring regression under mixing; microbial-community selection models estimate parent–offspring community-function transmission after many-cell propagule sampling. | Reticulate or many-founder ancestry is compatible with heredity when contributions and the reproduction protocol are explicit. [Bourrat 2019](https://doi.org/10.1007/s12064-019-00294-2), [Xie, Yuan & Shou 2021](https://doi.org/10.1038/s41467-021-26647-4) |

The strongest attack is B: high-fidelity reconstruction can coexist with no between-parent variation, making “heritability” unestimable. The proposed analysis returns **NOT IDENTIFIABLE** rather than manufacturing variation across independent runs.

## 18. Central decision

**C — NEW LINEAGE INSTRUMENTATION REQUIRED**

Independent theory supplies a stable criterion, so D and F are rejected. Multiple-parent ancestry can be represented by all measured material contributions; the single-cell-propagule regime supplies an initially unique edge. Heredity is applicable in principle, so E is rejected.

The current paper does not supply the required data, so A is rejected. B is also too strong: although the runtime state appears to contain cell identities, geometry, ancestry, regulation, and environment, the reported outputs do not contain a complete high-resolution record of collective birth, split, merger, offspring reconstruction, or descendants reproducing. The existing periodic snapshots and representative trajectories are not demonstrably sufficient for a retrospective pedigree. Unless an undocumented complete archive exists, the model must record those lineage events and paired collective phenotypes before the one minimal analysis can be performed.

This is an instrumentation requirement for future validation, not a model change, model run, or implementation performed in Q021.

## 19. Mechanism readiness

**NOT READY**

Q021 provides a test specification, not evidence that Fernandes has collective heredity. The higher-level heritable process is not yet established as a target phenomenon, and differential collective reproductive consequence remains downstream even if transmission is later found. A mechanism pass would therefore still risk explaining an unvalidated phenomenon.

## 20. Remaining explanatory gap

The narrow remaining gap is:

> Across event-resolved, concatenated source-cluster → single-cell-propagule → newborn-cluster pedigrees, does a parent's realized propagule-production organization predict the descendant's later reproductive organization beyond same-environment nonparent resemblance?

This is a transmission question. It does not reopen collective reproduction, demand full autonomy, or ask why individuality emerges.

## 21. Problem classification

| Problem | Q021 result |
|---|---|
| **Validation** | **Primary.** Parent-specific transmission of a collective reproductive trait has not been tested. |
| **Measurement** | Event-resolved split/merge genealogy, repeated parental \(Z\), and matched descendant \(Z\) must be recorded. |
| **Formalization** | **Largely resolved for the primary regime.** Use life-cycle-stage boundaries and all nonzero material contributions; do not impose unique or majority ancestry. |
| **Mechanism** | Deferred. Cell regulation is a candidate reconstructive pathway, not yet an explanation of demonstrated collective heredity. |

## 22. Known / Underexplored / Potentially Novel / Unknown

### ESTABLISHED / KNOWN

- Variation, reproduction, heredity, and differential reproductive consequence are distinct relations in Darwinian theory.
- Heritability is conditional on the population, trait, genealogy, environment, and measurement design.
- Lower-level genetic inheritance can reconstruct a heritable collective phenotype; separate higher-level inheritance machinery is unnecessary at a nascent stage.
- Multiple-parent collective heredity is formally possible; aggregation does not force a tree genealogy.
- Parent–offspring resemblance can be generated by shared environment and must be compared against genealogically unlinked controls.
- MLS1 and MLS2 labels are pragmatically useful but do not by themselves identify two objectively decoupled physical processes.
- Fernandes reports one local collective parentage edge and the state variables needed to identify clusters and cells at sampled times, but not a persistent collective pedigree.

### PARTIALLY EXPLORED / UNDEREXPLORED

- Event-level collective quantitative genetics for endogenous aggregative life cycles.
- Transmission of nonlinear reproductive organization through a single-cell propagule followed by later reaggregation.
- Pedigree methods that preserve all causal material contributors through repeated collective split and merger.
- Separating cell-program reconstruction, collective trait transmission, and environmental recurrence in level-blind spatial models.

### POTENTIALLY NOVEL

None. Pedigree-indexed transmission, parent–offspring regression, material-contribution ancestry, collective quantitative genetics, and environmental controls are prior art. Applying them to Fernandes could produce a new empirical result, but Q021 does not produce it.

### UNKNOWN

- Whether regulated propagule-production organization varies among collectives within the relevant Fernandes population.
- Whether newborn collectives remain identifiable long enough to reproduce before merger or death.
- Whether parent-specific collective resemblance exceeds same-environment nonparent resemblance.
- Whether complete saved trajectories already exist at a cadence sufficient for retrospective reconstruction.
- If heredity is supported, whether the transmitted collective difference has differential reproductive consequences.

## 23. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

The minimum test is an application of established heredity, quantitative-genetic, Price-equation, and multiple-parent collective theory. Rejecting MLS2 as a magic ontological threshold is also Bourrat's prior argument. Q021 isolates a validation requirement and introduces no new falsifiable dynamical relation. [HYPOTHESES.md](HYPOTHESES.md) remains unchanged.

## 24. Highest-information next question

> With event-level lineage instrumentation, does the Fernandes single-cell-propagule regime show that a newborn collective's later propagule-production organization is predicted by its causally contributing parent collective more strongly than by same-environment nonparents across concatenated collective cycles?
