# Q018 — Frozen Q017 equivalence transfer

Theoretical research pass, 2026-09-08. This pass tests a specification frozen before inspection of the Fernandes–Vroomans–Colizzi target system. It uses published evidence only; it does not run or modify the model and does not perform Q019.

## 1. Research question

> Does the Q017 collective-reproducer equivalence transfer unchanged to the Fernandes–Vroomans–Colizzi level-blind multicellularity model?

The critical constraint is **NO RETUNING**: neither numerical tolerances nor the meanings of parent, offspring, collective, multiplication, life cycle, or closure may be changed after inspecting the target. Mapping target observables onto the frozen concepts is permitted; criterion modification is not.

## 2. FROZEN Q017 SPECIFICATION

This section was extracted from [Q017](Q017_SNOWFLAKE_COLLECTIVE_REPRODUCER_EQUIVALENCE.md) before examining Fernandes et al. It is fixed for the remainder of Q018.

### 2.1 Entity-identification rule

The candidate collective unit \(U\) is:

> a maximal, physically cohesive clonal assembly produced by continuing genealogical association of daughter cells and capable of becoming physically separate from another such assembly.

Cohesion may be realized by intact bonds or entanglement; exact bond topology is not identity-bearing. The fixed stage variables are \(S=\{J,A\}\): a juvenile collective not yet reproduction-competent and an adult collective capable of producing a propagule. Cell number, radius, toughness, exact geometry, and stage duration are state variables, not identity variables.

### 2.2 Parentage relation

Collective parentage \(P\) holds when a separated offspring assembly derives by material and genealogical continuity from one parent assembly, rather than by an observer grouping independent cells.

### 2.3 Multiplication criterion

The collective-level stage graph must contain a multiplicative transition: one candidate collective gives rise to more than one causally descendant candidate collective. Growth of one assembly, cell proliferation alone, or spatial separation without the frozen parentage relation does not satisfy multiplication.

### 2.4 Life-cycle closure criterion

The declared collective-stage graph must recurrently connect juvenile, adult, and offspring stages. In Q017's formal statement, the relevant collective-level projection/support graph must be irreducible and must contain a multiplicative edge. A materially and genealogically descended offspring collective must reconstruct the juvenile-to-adult-to-offspring cycle.

### 2.5 Intervention family

The three identity-relevant intervention classes \(I\) are fixed:

1. abolish persistent post-budding association without abolishing cell division;
2. isolate a newly separated propagule and test reconstruction;
3. alter size or mechanics while testing whether parentage and closure persist.

No target-specific substitute intervention may be added during Q018.

### 2.6 Numerical thresholds and tolerances

The fixed tolerance schema \(\tau\) requires:

- collective offspring contain at least two clonally related cells **at separation**;
- multiplicative and reconstruction probabilities exceed one prespecified detection threshold;
- both are evaluated within one common budget measured in yeast cell-division or transfer opportunities;
- transition probabilities, sizes, timings, and mechanics may vary above that threshold without changing type.

Q017 explicitly did **not** supply a numerical value for the common detection threshold: it said the value could not be recovered from the published snowflake comparisons and must be fixed before a decisive new experiment or reanalysis. Q018 therefore freezes the absence of a number; it may not invent or fit one from Fernandes data. Q017's budget is expressed generically as cell-division or transfer opportunities, not in a snowflake-specific dimensional unit.

### 2.7 Equivalence conditions

Two cases \(X\sim_{CR}Y\) exactly when a mapping between their juvenile and adult stages preserves:

1. the candidate-unit rule \(U\);
2. the existence and direction of collective parentage \(P\);
3. a multiplicative edge;
4. irreducibility of the relevant stage graph;
5. the fixed qualitative intervention outcomes in \(I\), within \(\tau\).

Rates and magnitudes on graph edges may differ. The equivalence preserves which lineage reproduces and which stages recur, not every mechanism or rate.

### 2.8 Exclusion conditions

The rule excludes:

- independently assembled or observer-grouped cells that lack continuing clonal genealogy;
- a single cell as a collective offspring, because offspring must contain at least two clonally related cells at separation;
- growth without production of multiple causally descendant collectives;
- temporary, non-recurrent clustering;
- stage cycles manufactured only by arbitrary size bins;
- collective-looking persistence without material/genealogical parentage and closed multiplication;
- declaring a new reproducer type solely from changes in size, duration, geometry, mechanics, exact bond topology, propagule size distribution, or rates when \(U\), \(P\), and \(L\) persist.

### 2.9 Missing-data rules

Q017 distinguished structural support from complete intervention-preserving equivalence. Accordingly, the frozen rules for absent evidence are:

- failure to report a required relation or intervention is **evidence unavailable**, not evidence that the criterion fails;
- a case missing evidence required by \(U\), \(P\), multiplication, or closure is **NOT IDENTIFIABLE FROM AVAILABLE DATA**, not “almost” a collective reproducer;
- a structurally supported case lacking the matched intervention family and common threshold may be structurally classified, but full frozen equivalence is not demonstrated;
- because no numerical detection threshold was fixed in Q017, numerical equivalence cannot be certified retrospectively in Q018;
- no target-specific normalization, unit conversion convention, stage definition, entity boundary, or semantic exception may be introduced to rescue classification.

## 3. Fernandes model semantics

### 3.1 Source status

**Fact.** The latest version located is bioRxiv version 3, posted 10 March 2026 under the title *Reproduction emerges from ecological interactions at the onset of multicellularity*. The official bioRxiv metadata lists versions 1–3 and no journal publication; the manuscript itself states that it has not been certified by peer review. Q018 therefore treats it as an **uncertified preprint**, not as a peer-reviewed result. [Fernandes, Vroomans & Colizzi 2026, preprint v3](https://www.biorxiv.org/content/10.1101/2025.10.08.681199v3), [official version metadata](https://api.biorxiv.org/details/biorxiv/10.1101/2025.10.08.681199/na/json)

### 3.2 Predefined substrate

**Fact.** The model explicitly specifies:

- a \(2000\times2000\) two-dimensional Cellular Potts lattice and an explicit cell as a set of lattice sites carrying one spin;
- cell size and shape mechanics, stochastic movement, and contact energy;
- resource patches, a chemoattractant field, food consumption, metabolic reserves, starvation and background death;
- two mutually exclusive cell states, migrating and dividing;
- a fully supplied cell-division operation: growth to twice target area, division into two daughters, and partition of metabolic reserves;
- chemotaxis and persistent migration;
- ligand–receptor adhesion mechanics with 16 adhesion output genes;
- a fixed-topology Boolean gene-regulatory architecture with sensory, regulatory, cell-state, and adhesion outputs;
- mutation of regulatory weights and thresholds in one daughter at cell division;
- six designer-set resource-distribution environments, while GRN parameters and behaviour regulation evolve.

The substrate therefore pre-enables cell reproduction, adhesion, behavioural switching, sensing, and aggregation. It does not predefine no structure at all; that would be impossible. [Fernandes et al. v3, main text and methods](https://doi.org/10.1101/2025.10.08.681199), [Supplementary Information, Model description](https://www.biorxiv.org/content/biorxiv/early/2026/03/10/2025.10.08.681199/DC1/embed/media-1.pdf?download=true)

### 3.3 Predefined evolutionary entities

**Fact.** The dynamically explicit reproducing entities are cells. Each cell has a spin, metabolic state, GRN, adhesion profile, death process, and division event. The model does **not** encode:

- multicellular-individual identifiers;
- collective membership or a privileged collective boundary;
- group parentage or collective offspring identifiers;
- a propagule-production operator;
- collective generations;
- collective genomes;
- a collective fitness variable used by the evolutionary dynamics;
- a hierarchy or fixed nesting channel of cell-to-group levels.

Clusters, life-cycle categories, and “multicellular lineages” are analytical descriptions applied to evolved cell dynamics. The paper's classifier derives three life-cycle categories from median adhesion between migrating and dividing cell states in mutation-free follow-up simulations. Its threshold \(\widetilde\gamma_{\mathrm{mig,mig}}\leq0\) identifies the strictly unicellular category; \(\widetilde\gamma_{\mathrm{div,div}}\leq0\) separates the single-cell-propagule category from strictly multicellular cases. These categories are post-evolution measurements, not group objects consulted by the simulator. [Fernandes et al. v3, Materials and methods](https://doi.org/10.1101/2025.10.08.681199)

### 3.4 What receives reproductive consequences

**Fact.** Cells consume resources, die when reserves are exhausted or stochastically, and divide when their evolved regulatory state permits. Mutation occurs at cell division. Thus differential survival and cell division generate cell-lineage reproductive success.

**Fact.** The quantity called “fitness” in the methods is inferred after evolution for a population in mutation-free simulations from steady-state food depletion. It is not a collective fitness variable assigned during the evolutionary simulations. Competition experiments compare the population persistence of sampled lineages, again without assigning fitness to pre-labelled collectives.

**Interpretation.** Collective chemotaxis, dispersal, cluster persistence, and propagule production can change cell-lineage success. That is an emergent collective consequence under cell-level ecological selection, not an explicit collective-level fitness term or an automatic demonstration of MLS2. This matches the immediate modelling lineage: the 2020 model explicitly made each cell's replication probability depend on cell position and stated that no multicellular fitness advantage was assigned; the 2023 regulated-behaviour model likewise described competition among cells for survival and reproduction inside emergent clusters. [Colizzi, Vroomans & Merks 2020](https://doi.org/10.7554/eLife.56349), [Vroomans & Colizzi 2023](https://doi.org/10.1186/s12862-023-02133-x)

## 4. Meaning of level-blindness

For Q018, “level-blind” is decomposed rather than accepted as a single rhetorical label.

| Blindness | Classification | Evidence and limit |
|---|---|---|
| **Selection blindness** | **YES with respect to collectives** | Evolutionary consequences arise through cell survival and division; no fitness is assigned to a pre-labelled collective. Retrospective population fitness and lineage competitions do not alter this. |
| **Entity blindness** | **YES with respect to collectives** | Cells are explicit, but collective IDs, fixed memberships, parentage, generations, and offspring are absent. Cluster categories are analytical. |
| **Reproduction blindness** | **YES for multicellular modes; NO for cell reproduction** | Cell division is fully predefined. Fragmentation, differential-adhesion propagules, and the reported collective cycles are not enumerated as operations or options. |
| **Scale blindness** | **PARTIAL** | No discrete collective level or nesting hierarchy is encoded above cells. The lattice, cells, intracellular GRN layers, and cell-scale behaviours remain designer-defined; the substrate is not blind to every scale. |

**Interpretation.** “Level-blind” is accurate only as shorthand for the absence of an operative collective level. It must not imply that the simulator lacks predefined cells, reproductive micro-operations, behavioural states, or architectural scale.

The narrow DISHTINY contrast survives: DISHTINY supplies level-specific hereditary identifiers and configured nesting channels, whereas Fernandes supplies neither group IDs nor higher-level reproduction operations. This does not imply that the Fernandes substrate is unconstrained or that its evolved clusters satisfy Q017.

## 5. Reported evolutionary regimes

**Fact.** Across 72 simulations in six food-distribution environments, the paper reports three main life cycles in its own terminology:

1. **strictly unicellular life cycle**;
2. **multicellular + unicellular propagules life cycle**;
3. **strictly multicellular life cycle**.

The strictly multicellular category contains a reported spectrum:

- **multicellular propagules**, in which dividing cells reduce adhesion to migrating cells while continuing to adhere to one another and detach as a group;
- **high-adhesion multicellular** lineages, whose clusters split rarely and do so through physical tearing when different regions move toward different food patches.

Homogeneous resource conditions most often yield strictly unicellular strategies; intermediate conditions favor unicellular or multicellular propagules; heterogeneous conditions favor high-adhesion multicellularity. This is the paper's classification, recorded before applying Q017. [Fernandes et al. v3, Figs. 2–4](https://doi.org/10.1101/2025.10.08.681199)

**Fact.** The evolved clusters are aggregative. Supplementary Figure S3 reports that clusters in both a single-cell-propagule lineage and a high-adhesion lineage contain many distantly related cell lineages and are highly genetically heterogeneous. [Fernandes et al. v3, Supplementary Fig. S3](https://www.biorxiv.org/content/biorxiv/early/2026/03/10/2025.10.08.681199/DC1/embed/media-1.pdf?download=true)

## 6. Entity-rule transfer

### 6.1 Measurement mappings allowed

The following are mappings of observables onto frozen concepts, not modifications:

| Frozen concept | Fernandes observable | Status |
|---|---|---|
| cell | Cellular Potts spin and its occupied lattice sites | Direct |
| physical cohesion | connected cells with positive effective adhesion/contact persistence | Available in model state |
| clonal genealogy | recorded cell ancestry / pairwise time to MRCA | Available; Supplementary Fig. S3 is diagnostic |
| physical separation | loss of contact between an emitted unit and source cluster | Directly visible and model-definable |
| cell count at separation | number of cells in the emitted unit at detachment | Directly visible for illustrated regimes |
| juvenile/adult collective stages | a collective-level reproductive-competence partition | Not supplied as a target-independent measurement |

The last entry is missing rather than licensed for retrospective invention. Migrating and dividing are cell states, not automatically Q017's juvenile and adult collective stages.

### 6.2 Prohibited criterion modifications

The following would rescue apparent biological cases but invalidate frozen transfer:

- dropping clonality or replacing continuing daughter association with aggregation;
- calling any connected cluster a Q017 collective regardless of genealogy;
- allowing a single cell to count as a collective offspring at separation;
- identifying the later reconstructed cluster as the offspring while ignoring that separation occurred one cell earlier;
- replacing a physical parent collective with a genotype, MRCA, or sampled “lineage”;
- substituting the paper's \(\widetilde\gamma\) life-cycle thresholds for Q017's \(\tau\);
- treating author labels such as “propagule” or “life cycle” as satisfaction of frozen parentage and closure.

### 6.3 Unchanged entity-rule results

| Reported regime | Frozen Q017 collective reproducer? | Reason |
|---|---|---|
| strictly unicellular | **NO** | No multicellular candidate unit. |
| multicellular + unicellular propagules | **NO** | The detached propagule is one cell, below the fixed two-cell-at-separation rule; mature clusters are aggregative and genetically heterogeneous rather than clonal assemblies produced by continuing daughter association. |
| strictly multicellular with multicellular propagules | **NO** | Physical cohesive propagules occur, but the reported collectives are aggregative and genetically heterogeneous, so frozen \(U\) has no instance. |
| high-adhesion strictly multicellular | **NO** | Cohesive clusters and rare tearing occur, but the clusters violate frozen clonality/continuing-genealogy requirements. |

These are exactly the permitted YES/NO/NOT IDENTIFIABLE outcomes. Here **NO** is supported for \(U\) because the target positively reports aggregative genetic heterogeneity; it is not inferred from silence.

## 7. Parentage transfer

**Fact.** The paper supports several process-level descent relations:

- in the single-cell-propagule regime, a cell changes adhesion state, detaches from a migrating cluster, divides, and its daughters reactivate adhesion and form a new cluster;
- in the multicellular-propagule regime, a group of dividing cells detaches from a migrating cluster;
- high-adhesion clusters can tear into physically separate parts.

**Interpretation under the frozen rule.**

| Regime | Paper-level material descent | Q017 \(C_{\mathrm{parent}}\rightarrow C_{\mathrm{offspring}}\) |
|---|---:|---:|
| multicellular + unicellular propagules | Supported as cluster \(\rightarrow\) cell \(\rightarrow\) cluster | **NO**: the separated offspring is not a collective under fixed \(\tau\), and the reconstructed aggregate is not a frozen clonal \(U\)-unit. |
| multicellular propagules | Supported as detachment of cells from a source cluster | **NO as a relation between frozen units**: neither parent nor offspring satisfies \(U\). |
| high-adhesion tearing | Supported as material partition of a cluster | **NO as a relation between frozen units**: the aggregative cluster is outside \(U\). |

This is an ontological failure before a dispute about temporal succession arises. The paper-level processes are not denied; they do not instantiate parentage **between Q017 entities**.

## 8. Multiplication transfer

The frozen criterion requires one candidate collective to produce multiple causally descendant candidate collectives.

- **Strictly unicellular:** **NO** collective multiplication; only cell division.
- **Multicellular + unicellular propagules:** **NO** under Q017. Repeated cell emission followed by aggregation/reconstruction is not multiplication into collective offspring containing at least two clonal cells at separation.
- **Multicellular propagules:** process-level group multiplication is supported by detachment, but **NO** under Q017 because the groups are not frozen \(U\)-units.
- **High-adhesion multicellular:** the paper reports rare physical tearing, but the probability is not evaluated under Q017's missing common threshold. Even apart from that evidential problem, multiplication of frozen \(U\)-units is **NO** because \(U\) is absent.

The distinction among cluster growth, cell proliferation, and collective multiplication is therefore preserved. No positive Q017 case is inferred from cluster size.

## 9. Life-cycle closure transfer

### 9.1 Claim B is supported

**Fact.** The paper provides strong evidence for recurrent process cycles in its own categories. Its clearest sequence is:

\[
\text{migrating aggregate}
\rightarrow
\text{detached single cell}
\rightarrow
\text{two daughters that re-adhere}
\rightarrow
\text{new migrating aggregate}.
\]

It also reports recurrent strictly multicellular strategies with group detachment or tearing. Thus Claim B—a recurrent multicellular life cycle under the paper's entity and stage interpretation—is supported.

### 9.2 Claim C does not follow

Under frozen Q017, closure requires recurrence among \(U\)-units plus a multiplicative transition within \(\tau\). The single-cell sequence fails at the fixed offspring boundary, and all evolved aggregates fail frozen clonality. Therefore:

- strictly unicellular: **NO**;
- multicellular + unicellular propagules: **NO**;
- strictly multicellular with multicellular propagules: **NO**;
- high-adhesion strictly multicellular: **NO**, with additional missing probability/intervention evidence.

The existence of a single-cell stage does not logically preclude every collective life cycle. It precludes this transfer because Q017 explicitly required a multicellular clonal offspring **at separation**. Treating post-separation reconstruction as an exception would be semantic and numerical retuning.

## 10. Intervention-family transfer

| Frozen intervention | Status in Fernandes | Assessment |
|---|---|---|
| abolish persistent post-budding association without abolishing cell division | **conceptually undefined at Q017 specificity** | Fernandes cells do not bud, and the model has general, state-dependent ligand–receptor adhesion rather than a separately manipulable post-budding association relation. Replacing the frozen intervention with a post-division daughter-association perturbation would already alter its stated target; globally forcing non-adhesion would be broader still and would affect aggregation among unrelated cells. The v3 target does not perform the exact frozen intervention. |
| isolate a newly separated propagule and test reconstruction | **not evaluated** | The paper tracks naturally detached single-cell propagules that divide and re-form a cluster in the intact ecology. It does not report an isolation intervention under a common assay, and no such test is reported for multicellular propagules or tearing fragments. |
| alter size or mechanics while testing whether parentage and closure persist | **not evaluated** | Environmental transfers and evolved adhesion differences change size, dispersal, and split frequency, but no matched intervention alters size/mechanics while measuring frozen parentage and closure. |

Related observations are not substituted for the interventions. Their absence is **evidence unavailable**, not evidence that the relevant causal response is absent.

The first entry cannot be filled in this target without criterion modification because Fernandes cells do not bud; a post-division or kin-specific analogue would belong to a newly and prospectively specified equivalence, not the frozen transfer. The remaining evidential entries could be filled by isolation and lineage tracking of each emitted unit through reconstruction, and by a controlled size/mechanics perturbation with collective ancestry and cycle outcomes recorded. These are specifications only. Q018 does not implement or run them.

## 11. Numerical-tolerance transfer

Three separate results follow.

1. **Cell-count tolerance transfers and rejects the strongest prospective case.** The “at least two clonally related cells at separation” condition is dimensionless and applies unchanged. The paper's single-cell propagule has one cell at detachment, so it fails.
2. **The common opportunity budget is conceptually transportable but unmeasured.** Q017 permitted cell-division or transfer opportunities, so a cell-division-event budget need not be rescaled from yeast physical units. Fernandes reports time steps and division mechanics, but not Q017 multiplication/reconstruction probabilities within one common opportunity budget.
3. **The detection threshold is non-transportable as currently formulated.** Q017 deliberately left its numerical probability threshold unspecified. Q018 cannot assign one after seeing the target. The paper's adhesion threshold at \(\gamma=0\), its \(25\%\) Hamming cutoff for co-option, and its regime frequencies are different quantities and cannot replace \(\tau\).

The numerical result is therefore:

\[
\boxed{\text{NON-TRANSPORTABLE AS CURRENTLY FORMULATED}}
\]

This is not merely unit incompatibility. It is a prior under-specification of the numerical equivalence, plus absence of the required probability assay.

## 12. Positive cases

### 12.1 Under the frozen Q017 equivalence

**None.**

No reported Fernandes regime satisfies the unchanged conjunction of frozen \(U\), collective parentage, collective multiplication, closure, intervention responses, and \(\tau\).

### 12.2 What this does not erase

**Fact.** The target strongly supports:

- **Claim A:** multicellular spatial structures and collective chemotaxis exist;
- **Claim B:** regulated recurrent multicellular life cycles, including single-cell and multicellular propagule modes, exist under the paper's interpretation.

**Interpretation.** Q018 rejects only Claim C: that the **frozen Q017** equivalence identifies these as its collective-reproducer type. The absence of a frozen positive case is not evidence that the reported transition or life cycles are unreal.

## 13. Negative / type-preserving cases

### 13.1 Negative cases

- The strictly unicellular regime is a direct negative control: cell division occurs without a collective \(U\), collective multiplication, or collective closure.
- High-adhesion aggregates show that spatial cohesion, large cluster size, and collective migration do not alone establish frozen collective reproduction. Their rare tearing cannot be evaluated against the missing Q017 probability threshold, and their aggregation violates \(U\).
- The single-cell-propagule regime is a stronger boundary control: it shows that even a recurrent process naturally described as multicellular reproduction can be excluded by Q017's fixed offspring-count and clonal-development rules.

### 13.2 Reported variations that would be prospective same-type controls

The paper reports quantitative changes in adhesion, cluster size, dispersal, division timing, food response, and persistence across lineages and environmental transfers. It also reports that 35 of 49 initially multicellular lineages retained a multicellular phase after transfer to EC1, all by preserving or evolving a propagule-forming life cycle.

These would be useful controls for a broader aggregative-reproducer equivalence. They cannot validate Q017's type preservation because Q017 identifies no positive Fernandes \(U\)-unit to preserve. Within the strictly multicellular spectrum, the shift from frequent multicellular propagules to rare tearing might be type-preserving if both exceeded one fixed threshold, but Q017 supplied no value and the paper did not estimate the required probabilities. The correct result is **NOT IDENTIFIABLE FROM AVAILABLE DATA**, not retrospective grouping.

## 14. Pre-enabled substrate analysis

**Fact.** Adhesion, environmental sensing, behavioural switching, cell growth/division, mutation, and ecological resources are predefined. The GRN topology is fixed; only its parameters and resulting regulation evolve. These ingredients strongly constrain and enable the accessible dynamics.

**Fact.** The model does not enumerate “single-cell propagule,” “multicellular propagule,” “tearing,” or “high-adhesion life cycle” as reproductive modes. It does not invoke a group ID, group reproduction operator, group generation, or collective fitness term when cells behave.

**Interpretation.** The substrate is generically enabling relative to collective reproduction rather than designer-enumerating the reported modes. The fixed repertoire of cell states and adhesion machinery is still a substantive inductive bias and bounds the result. It establishes that an unlabelled collective process can arise from supplied cell behaviours, not that arbitrary reproductive modes or levels are accessible.

This differs narrowly from DISHTINY: Fernandes does not provide the later collective's ID or nesting channel. It nevertheless predefines the cellular entities and the behavioural primitives from which collectives form.

### 14.1 Co-option is not latent organizational identity

**Fact.** In the paper's EC3 transfer experiment, 7 of 12 strictly unicellular starting lineages and 11 of 12 high-adhesion multicellular starting lineages evolved toward propagule production. Among the lineages that evolved single-cell propagules, the authors' independent homology assay classified 5 of 7 unicellular-origin cases and 7 of 8 high-adhesion-origin cases as co-option of ancestral adhesion profiles. That assay uses a \(25\%\) Hamming-distance ceiling, conserved GRN input combinations, and conserved qualitative adhesion behaviour; these are the paper's co-option criteria, not Q017 tolerances. [Fernandes et al. v3, Fig. 4 and Supplementary Fig. S6](https://doi.org/10.1101/2025.10.08.681199)

**Interpretation.** Preserving Q015, ancestral adhesion profiles, behavioural programs, and GRN architecture do not imply that the later recurrent multicellular process already existed as an ancestral organizational identity. The evolved coupling between cell state and adhesion changes the process relation even though it reuses ancestral programs. Conversely, this evidence cannot rescue Q017: a changed process built from old parts still fails the frozen clonal entity and offspring-size conditions.

## 15. Snowflake–Fernandes comparison

| Feature | Snowflake yeast under Q017 | Fernandes v3 |
|---|---|---|
| group formation | continued clonal mother–daughter attachment | adhesion-mediated aggregation plus cell division |
| within-group genealogy | clonal branching | many distantly related cell lineages in reported clusters |
| emitted unit | multicellular clonal branch at fracture | single cell, multicellular aggregate, or tearing fragment depending on regime |
| identity-bearing implementation | growth and mechanical fracture | state-regulated differential adhesion, dispersal, or tearing |
| collective labels in operative dynamics | absent biologically | absent computationally |
| frozen \(U\) | present in early/later snowflake | absent in all reported Fernandes regimes |
| frozen offspring threshold | satisfied by multicellular fragments | violated by the flagship single-cell-propagule case |

Q016 correctly predicted that different mechanisms could realize the same identity relation. Mechanism difference is not what causes failure here. The failure is that Q017's purported identity-bearing relation contains two implementation/domain restrictions—clonal continued daughter association and a multicellular offspring at separation—that Fernandes does not satisfy.

Thus the same frozen relation coherently gives:

\[
\text{snowflake ancestor}\not\sim_{CR}\text{snowflake collective reproducer},
\]

\[
\text{early snowflake}\sim_{CR}\text{macroscopic snowflake},
\]

but no corresponding positive \(\sim_{CR}\) class in Fernandes. This is not out-of-system support for one common identity domain.

## 16. Transfer failure taxonomy

| Failure class | Result | Explanation |
|---|---|---|
| **A — Ontological failure** | **YES — decisive** | Frozen \(U\) does not identify the target's aggregative, genetically heterogeneous clusters. |
| **B — Relational failure** | **YES** | The single-cell case fails collective-at-separation parentage/multiplication; group detachment relations cannot become Q017 relations because their relata fail \(U\). |
| **C — Evidential failure** | **YES — additional** | The exact intervention family, isolation assay, common-budget probabilities, and a type-preserving control are not reported. |
| **D — Numerical failure** | **YES — additional** | The fixed two-cell cutoff transfers and rejects the flagship case, while Q017's probability threshold has no numerical value and cannot be transported retrospectively. |
| **E — Biological/domain failure** | **YES — central interpretation** | Q017 explicitly models clonal collective reproduction; Fernandes' reported collectives are aggregative and can reproduce through a single-cell phase. |
| **F — Q017 overfitting** | **POSSIBLE, NOT ESTABLISHED** | The two-cell-at-separation and continued-clonal-association clauses look snowflake-specific if Q017 was intended as a broad collective-reproducer model. But Q017 explicitly restricted its domain to clonal budding yeast, so the present result proves non-generality/domain mismatch, not post hoc overfitting within that domain. |

The problem lies primarily in the assumption that both systems instantiate the same frozen identity domain. Secondarily, Q017 is numerically underdefined. The Fernandes evidence is incomplete for interventions but already sufficient to establish the decisive clonal/domain mismatch.

## 17. Anti-circularity audit

Remove the expressions “multicellular reproduction,” “propagule,” and “life cycle,” and retain only process descriptions:

- a cell in an adhering migrating cluster changes state, loses adhesion, separates alone, divides, and its daughters re-adhere while also encountering other lineages;
- several dividing cells can detach together from an aggregate;
- a cohesive aggregate can be pulled apart when regions move toward different resources;
- clusters contain many distantly related cell lineages.

The frozen classifier still returns the same results. The first process fails the two-cell-at-separation rule and frozen clonality. The latter processes have material splitting but fail the entity rule. Author terminology is therefore not doing the classificatory work.

The audit also exposes the converse circularity risk: accepting the first process because it is labelled a propagule life cycle would require changing the frozen boundary. Q018 does not do so.

## 18. Central decision

**SYSTEMS NOT IN SAME IDENTITY DOMAIN**

The Q017 equivalence does not transfer unchanged. Snowflake yeast instantiates clonal collective reproduction through continued daughter association and multicellular fragmentation. Fernandes reports aggregative, genetically heterogeneous collectives and prominently a single-cell propagule at separation. Both may instantiate defensible forms of collective reproduction under a broader theory, but they are not members of the same class under frozen \(K_{CR}\).

This decision is stronger than “evidentially indeterminate” because the decisive entity and offspring-count conflicts are positively reported. It is more precise than generic “frozen transfer failed” because the process-level parentage/multiplication ideas remain meaningful; the frozen domain restrictions prevent common classification. Structural transfer is therefore only partial at the abstract process vocabulary level, not successful at the stated equivalence level.

The no-retuning conditions were met:

- collective boundaries were not redefined;
- no target-specific intervention was substituted;
- no tolerance or threshold was changed;
- parentage was not reassigned from a physical cluster to a genotype or analytical lineage;
- single-cell propagules received no exception;
- author conclusions were not used to override the frozen rule.

## 19. Mechanism readiness

**NOT READY**

The identity target is unstable across the two systems: the frozen equivalence has no Fernandes positive case, its numerical probability threshold is absent, and its intervention profile cannot be evaluated. Proceeding to ask what mechanism generates “the same” collective-reproducer relation would conflate clonal fragmentation with aggregative/single-cell reconstruction under an equivalence that has not yet justified grouping them.

This does not reopen or deny the paper's established model-specific mechanisms of regulated adhesion, ecological dispersal, and co-option. It blocks only a general mechanism analysis using Q017 as a validated cross-system target.

## 20. Remaining explanatory gap

The narrow gap is:

> Is clonality through continuing daughter association, and multicellularity at the moment of offspring separation, genuinely identity-bearing for the intended collective-reproducer domain, or are they snowflake-specific realizers that a broader **prospectively frozen** relation should exclude from identity?

This is a domain-boundary validation question. It must be answered before combining clonal fragmentation and aggregative single-cell-propagule cycles in one mechanism target.

The smallest discriminating test is conceptual and comparative: predeclare two competing domain models—one retaining the Q017 restrictions and one preserving only material/genealogical parentage across a recurrent collective reconstruction cycle—then apply both to established clonal and aggregative positive/negative cases without fitting either to Fernandes. Q018 does not perform that next test.

## 21. Problem classification

| Problem | Q018 result |
|---|---|
| **Definition** | The intended breadth of “collective reproducer” is unresolved: Q017's operational entity is specifically clonal and multicellular at separation. |
| **Measurement** | Exact intervention responses and common-budget multiplication/reconstruction probabilities are unavailable. |
| **Formalization** | The probability threshold has no value, and Q017 provides no prospective cross-domain rule for single-cell reconstruction or aggregative parentage. |
| **Validation** | **PRIMARY.** Frozen cross-system validation fails because the target lies outside the specified identity domain. |
| **Mechanism** | Deferred; the paper's model-specific mechanism is prior evidence, not the cross-system target of this pass. |

## 22. Known / Underexplored / Potentially Novel / Unknown

### ESTABLISHED / KNOWN

- BioRxiv v3 is an uncertified preprint as of the checked 2026 record.
- The model explicitly represents cells, cell division, adhesion mechanics, environmental resources, sensing, behavioural states, mutation, and a fixed GRN architecture.
- It does not use collective IDs, group parentage, collective offspring operations, collective generations, nesting levels, or a collective fitness variable in evolution.
- Cell survival and division receive direct reproductive consequences; group benefits are emergent ecological effects on cell lineages.
- Three author-defined life-cycle regimes evolve, including single-cell and multicellular propagule processes.
- Reported clusters are aggregative and genetically heterogeneous.
- Q017's clonal entity rule and two-cell-at-separation threshold therefore reject every reported Fernandes regime without retuning.
- Ancestral regulatory and adhesion programs can be co-opted into a changed multicellular process; ancestral ingredients do not imply ancestral organizational identity.

### PARTIALLY EXPLORED / UNDEREXPLORED

- Domain models of collective reproduction that cover both clonal development and aggregative reconstruction without collapsing incidental aggregates into reproducers.
- Intervention-based collective ancestry tests in models where clusters merge, exchange cells, and reproduce through a single-cell stage.
- Prospectively specified numerical thresholds and opportunity budgets for comparing collective multiplication across physical and computational systems.

### POTENTIALLY NOVEL

None. The transfer failure reveals a scope error and formal under-specification; it does not supply a new dynamical relation or scientific mechanism.

### UNKNOWN

- Whether Q017's clonality and offspring-size clauses are necessary identity conditions or snowflake-specific realizers.
- Whether a broader, prospectively frozen equivalence can accept established clonal and aggregative reproducer cases while rejecting transient or merely functional aggregates.
- Whether the exact Q017 intervention family can be represented without changing its meaning in an aggregative system.

## 23. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

Q018 is a failed transfer/validation result. It does not establish a new dynamical law. Co-option, adhesion-regulated propagules, ecological selection, and recurrent multicellular cycles are already the target paper's evidence and adjacent prior art. [HYPOTHESES.md](HYPOTHESES.md) remains unchanged.

## 24. Highest-information next question

> Are Q017's clonality-through-continuing-daughter-association and multicellular-at-separation clauses necessary for collective-reproducer identity, or are they snowflake-specific realizers that should be removed in a prospectively frozen cross-domain equivalence tested against independent clonal, aggregative, and non-reproducing controls?
