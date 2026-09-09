# Q017 — Snowflake collective-reproducer equivalence

Theoretical research pass, 2026-09-08. Scope: one predeclared identity model for collective reproduction in snowflake yeast. This is not a universal organizational taxonomy, a claim that snowflake yeast completed an evolutionary transition in individuality, or an OEE mechanism.

## 1. Research question

> Can a predeclared equivalence over collective parentage and life-cycle closure classify the `ACE2` snowflake transition as a new reproducer type while classifying later snowflake size and toughness evolution as type-preserving, without changing the variables, interventions, or tolerances between the two comparisons?

This is the exact highest-information question from [Q016](Q016_CAUSAL_REWIRING_VS_TYPE_CHANGE.md), and it agrees with the pre-pass [STATUS](STATUS.md) and [FRONTIER](FRONTIER.md).

The answer has two strengths:

1. **Structural answer: yes.** One parentage-and-life-cycle equivalence separates the unicellular ancestor from early snowflake yeast and groups early and macroscopic snowflake yeast together.
2. **Full causal answer: not yet demonstrated.** The published studies did not apply one matched intervention protocol and one prespecified statistical tolerance to all three genotypes. The structural classification is supported; its richer intervention-preserving version remains an empirical validation target.

## 2. Domain under study

The domain is **collective reproduction in clonally developing budding yeast**. The identity claim is deliberately restricted to this question:

> Does a multicellular, genealogically organized parent–offspring cycle exist, and is it the same kind of cycle across subsequent changes in size and mechanics?

It is not a claim about:

- morphological character identity;
- every kind of multicellular organization;
- organismality or completed evolutionary individuality;
- autopoietic or constraint closure;
- a universal hierarchy of evolutionary levels.

Three comparisons are fixed before defining equivalence:

| Case | Relevant condition | Role in the test |
|---|---|---|
| Unicellular ancestor | Functional `ACE2`; daughters separate after budding | Different-type control |
| Early snowflake | `ACE2` loss; persistent mother–daughter attachment; growth and fracture | Candidate origin of a collective reproducer |
| Macroscopic snowflake | Later evolved elongation, packing relief, and branch entanglement | Same-type control despite major implementation change |

The ancestral cell cycle remains present in all three cases. The proposed transition adds an embedding collective cycle; it does not replace cell reproduction.

## 3. Identity-bearing relation

Reproduction theory identifies causal parent–offspring lineages, rather than material similarity alone, as the common relation among simple, collective, and scaffolded reproduction. A collective reproducer has components that reproduce while the collective also forms a parent–offspring lineage. Godfrey-Smith explicitly treats the distinction between substantial collective reproduction and a mere by-product such as a herd as graded. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112)

Life-cycle theory supplies the temporal criterion. Doulcier, Takacs, and Bourrat require (i) a multiplicative transition and (ii) closure: under a declared stage coarse-graining, each relevant stage is reachable again along the lineage. In their matrix formulation, closure is irreducibility of the collective-level projection matrix. They use incomplete cell separation and cluster fragmentation as the snowflake-yeast example. [Doulcier, Takacs & Bourrat 2024](https://doi.org/10.1017/psa.2023.162)

For this pass, predeclare a collective-reproducer model

\[
K_{CR}=(U,S,P,L,I,\tau).
\]

- \(U\), the candidate-unit rule: a maximal, physically cohesive clonal assembly produced by continuing genealogical association of daughter cells and capable of becoming physically separate from another such assembly. Cohesion may be realized by intact bonds or entanglement; exact bond topology is not identity-bearing.
- \(S=\{J,A\}\), the stage variables: a juvenile collective not yet reproduction-competent and an adult collective capable of producing a propagule. Cell number, radius, toughness, exact geometry, and stage duration are state variables, not identity variables.
- \(P\), collective parentage: a separated offspring assembly derives by material and genealogical continuity from one parent assembly, rather than by an observer grouping independent cells.
- \(L\), life-cycle closure: the stage graph contains a multiplicative transition and recurrently connects juvenile, adult, and offspring stages.
- \(I\), identity-relevant intervention classes: abolish persistent post-budding association without abolishing cell division; isolate a newly separated propagule and test reconstruction; and alter size or mechanics while testing whether parentage and closure persist.
- \(\tau\), fixed tolerances: collective offspring contain at least two clonally related cells at separation; multiplicative and reconstruction probabilities exceed one prespecified detection threshold within one common budget measured in yeast cell-division or transfer opportunities; and transition probabilities, sizes, timings, and mechanics may vary above that threshold without changing type.

Two cases are equivalent in this domain when a mapping between their juvenile and adult stages preserves \(U\), \(P\), the support of the multiplicative closed cycle \(L\), and the qualitative response classes in \(I\), all under the same \(\tau\). This equivalence deliberately preserves **which lineage reproduces and which stages recur**, not every mechanism or rate.

The numerical detection threshold in \(\tau\) cannot be recovered from the published comparisons because they were not designed as one preregistered assay. It must be fixed before a decisive new experiment or reanalysis. This is a measurement limitation, not permission to tune the criterion retrospectively.

## 4. Type-preserving variation

Early snowflake clusters reproduce by physical fracture: daughter cells remain attached to mothers, clusters grow, internal stress breaks a connection, and a multicellular branch becomes a propagule. The propagule develops into another reproduction-competent cluster. Cluster size at reproduction is highly heritable, yet the growth form remained stable through substantial early evolution. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102)

Later anaerobic lineages evolved approximately \(2\times 10^4\)-fold larger size and \(10^4\)-fold greater toughness. Elongated cells first reduced packing strain and later enabled branch entanglement, allowing clusters to remain cohesive after many bonds broke. Despite these large molecular, cellular, topological, and biomechanical changes, the study explicitly reports retention of the clonal multicellular life cycle. [Bozdag et al. 2023](https://doi.org/10.1038/s41586-023-06052-1)

Under \(K_{CR}\), these later changes are type-preserving because they alter:

- stage duration and size;
- propagule and parent size distributions;
- mechanical strength and fragmentation thresholds;
- cell aspect ratio, packing, and the physical realization of cohesion;
- quantitative collective fitness and accessible phenotypes;

while retaining a clonally developing collective that matures, separates material descendants, and reconstructs the same collective cycle. The case is a direct analogue of Developmental System Drift only in logical form: substantial realizer change can preserve the selected domain relation. It is not itself a case of morphological homology or ChIM identity.

## 5. Type-changing variation

The unicellular ancestor buds and separates into individual cells. It has a cellular parent–offspring cycle, but under the same \(U\) it lacks persistent multicellular units, collective propagule parentage, and a juvenile-to-adult collective growth–fragmentation cycle.

Early snowflake yeast changes all three facts. The original evolution experiment observed multicellular propagules, a juvenile phase, determinate collective growth, and selection responses in collective life-history traits. [Ratcliff et al. 2012](https://doi.org/10.1073/pnas.1115323109)

Reverse genetics strengthens the causal contrast. Knocking out `ACE2` in the unicellular ancestor was sufficient to yield the snowflake phenotype, whereas functional complementation of an early snowflake strain restored unicellularity. The causal route is incomplete mother–daughter separation followed by growth and mechanically induced fragmentation. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102)

Thus the strongest supported statement is:

\[
\boxed{
\text{cellular reproduction only}
\longrightarrow
\text{cellular reproduction embedded in a collective growth–fracture cycle}
}
\]

This is a new **collective-reproducer relation** under \(K_{CR}\), not merely a larger value of cluster size. The molecular change is small; the identity-bearing relation changes. Conversely, later molecular and biomechanical change is large; that relation persists.

The result remains bounded in the Q015 sense. It contrasts the assayed `ACE2`-functional ancestor with its engineered and evolved descendants under the reported environments. It does not prove that no ancestral yeast genotype, environment, or longer evolutionary route could produce any collective cycle.

## 6. Closest established theory

The result is substantially absorbed by established reproduction and ETI theory.

1. **Collective reproduction:** parent–offspring lineage formation distinguishes a reproducing collective from recurring structures or incidental groups. Reproduction alone does not guarantee strong Darwinian individuality. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112)
2. **Nascent multicellular life cycles:** clonal development and genealogical bottlenecks partition variation among snowflake clusters, reduce within-cluster conflict, and enable collective adaptation. [Ratcliff et al. 2017](https://doi.org/10.1098/rstb.2016.0420)
3. **Biological construction:** a mutation causing daughters to remain attached can generate a group life cycle in which growth and fracture supply reproduction and heritable variation. [van Gestel & Tarnita 2017](https://doi.org/10.1073/pnas.1704631114)
4. **Life-cycle closure:** a new collective level is characterized by a multiplicative, closed cycle over declared collective stages. [Doulcier, Takacs & Bourrat 2024](https://doi.org/10.1017/psa.2023.162)
5. **Multilevel selection and individuality:** a life cycle can create collective heritability and selection before a transition is complete; levels of individuality are graded and multidimensional. [Shelton & Michod 2020](https://doi.org/10.1098/rstb.2019.0364)

Accordingly, “new organizational type” adds no distinct scientific category here. The defensible term is **origin of a collective growth–fragmentation reproducer**. Whether that reproducer is already an evolutionary individual, and how far the ETI has progressed, are further claims.

## 7. Formal equivalence framework

Let \(G_K(X)\) be the directed support graph estimated for case \(X\) under \(K_{CR}\). Vertices are the fixed stage classes \(J,A\); directed edges are supported developmental or multiplicative transitions; parentage labels distinguish transformation of one unit from production of a materially descended unit.

Define

\[
X\sim_{CR}Y
\]

when there is a stage mapping that preserves:

1. the candidate-unit rule \(U\);
2. the existence and direction of collective parentage \(P\);
3. a multiplicative edge;
4. irreducibility of the relevant stage graph;
5. the fixed qualitative intervention outcomes in \(I\), within \(\tau\).

Rates and magnitudes attached to graph edges are allowed to differ. This is why evolved size, strength, propagule size, or generation time can change without producing another reproducer type. A transition that removes collective parentage or breaks cycle closure changes type even if morphology remains similar.

Applied without retuning:

| Comparison | \(U\) | Collective \(P\) | Multiplication + closure | Matched intervention evidence | Classification |
|---|---:|---:|---:|---:|---|
| Ancestor | Absent at collective level | Absent | Absent | Cell separation and absence of clustering established | Different from snowflake |
| Early snowflake | Present | Present | Present | `ACE2` knockout/complementation plus propagule observation | Collective reproducer |
| Macroscopic snowflake | Present | Reported as retained clonal life cycle | Present by reported retention | No fully matched `ACE2`/association intervention series located | Structurally equivalent; causally provisional |

This table prevents two overclaims. First, the evidence is adequate for the support-graph classification but incomplete for full intervention equivalence. Second, graph isomorphism is not sufficient by itself: its vertices and parentage labels receive their meaning from reproduction theory.

## 8. Domain theory versus causal abstraction

Domain theory does the indispensable scientific work:

- reproduction theory says why material/genealogical parentage matters;
- life-cycle theory says why multiplication plus recurrent stage reconstruction matters;
- snowflake developmental biology identifies persistent attachment and fracture as the causal realization.

Causal abstraction then asks whether interventions on these variables commute across descriptions. It can test whether early and late snowflake models preserve the declared higher-level relation even though lower-level mechanisms differ. It cannot decide that parentage and life-cycle closure, rather than morphology or autonomy, should bear identity.

Thus \(\sim_{CR}\) is not discovered by causal abstraction. It is a domain-motivated relation checked with abstraction machinery. Complete molecular intervention equivalence would be too strong; gross input–output equivalence under settling selection would be too weak.

## 9. Same-domain versus cross-domain transitions

The two comparisons have different logical forms.

- **Ancestor to early snowflake:** a new embedding domain becomes evolutionarily relevant. Cell parentage continues, but persistent cell genealogy now realizes collective parentage and a collective cycle. This is a cross-level addition, not a replacement of cellular identity.
- **Early to macroscopic snowflake:** the same collective-reproducer domain persists while quantitative life-history, morphology, mechanics, and evolvability change. This is same-domain variation.

The transition therefore can be represented as a change in **which relation carries an additional evolutionary identity**: a cell lineage alone versus cell lineages nested inside a collective lineage. Major-transition theory already describes this pattern. No new “evolutionary ontology” is required.

The nesting matters. New collective possibilities coexist with losses or restrictions at the cellular level; the event is a reorganization, not monotonic set inclusion.

## 10. Relation to transformational novelty

Taylor's transformational novelty concerns changes that require a new concept in the descriptive meta-model; major transitions in individuality are candidate examples. The addition of a collective reproducer can therefore instantiate transformational novelty **under a model whose relevant concepts include levels of reproduction**. [Taylor 2019](https://doi.org/10.1162/artl_a_00290)

The relation is neither equivalence nor mechanism:

- transformational novelty is broader than changes in reproduction;
- a new collective cycle supplies domain evidence for changing the description rather than merely asserting a new macrostate;
- later macroscopic evolution may be a major morphological and biomechanical innovation while remaining within the same collective-reproducer domain;
- one transformation does not establish ongoing transformational novelty or OEE.

Thus \(K_{CR}\) operationalizes one candidate instance of transformational novelty; it neither defines the whole category nor explains its recurrence.

## 11. Relation to major transitions

The collective-reproducer classification is a restricted part of ETI theory, not an alternative to it. Snowflake yeast is a fraternal transition: related cells remain associated, collective propagules reproduce, a genealogical bottleneck limits conflict, and collective traits become heritable and selectable.

Life-cycle-closure theory argues that a new embedding closed cycle is enough to characterize an ETI. Other accounts treat individuality as multidimensional or graded and additionally emphasize heritable fitness variation, bottlenecks, integration, germ–soma differentiation, conflict control, or transfer in the balance of selection. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112), [Shelton & Michod 2020](https://doi.org/10.1098/rstb.2019.0364)

Q017 therefore supports a weaker, less controversial conclusion:

\[
\boxed{
\text{new collective reproducer}
\not\Rightarrow
\text{completed ETI or fully consolidated evolutionary individual}
}
\]

The early transition supplies a new unit capable of collective parentage and heritable life-history variation. Later evolution strengthens collective size, toughness, and adaptation without necessarily marking another transition in reproducer identity.

## 12. Counterexamples

### A. Large implementation change with conserved identity

Macroscopic snowflake yeast is the intended negative control. Orders-of-magnitude changes in size and toughness plus a shift from bond-limited packing to branch entanglement do not abolish the clonal collective cycle. Any criterion that declares a new reproducer solely from molecular distance, graph topology, size, or biomechanics fails this control.

### B. A small change creates a new relation

Loss of `ACE2` is sufficient for persistent attachment and the growth–fracture cycle, and complementation restores unicellularity in the early strain. Genetic edit distance cannot be the type boundary.

### C. The by-product objection

Cell division generates both wild-type cells and snowflake biomass, so one can describe clusters as by-products of cellular reproduction. That description misses the observed multicellular propagules, juvenile/adult differentiation, recurrent cluster parentage, heritable cluster size at reproduction, and response of collective life-history traits to selection. These relations distinguish snowflake clusters from arbitrary cell aggregates or herds. They do not, by themselves, prove completed individuality.

### D. Stage gerrymandering

Arbitrary size bins can manufacture cycles. Multiplication, irreducibility, lineage-based parentage, preregistered stages based on reproductive competence, and sensitivity analysis constrain this freedom but do not eliminate model choice. This is the strongest observer-dependence counterexample.

### E. A different domain gives a different answer

Macroscopic snowflake yeast may count as a new biomechanical or morphological organization because entanglement creates a new cohesion regime. Q017 calls it type-preserving only in the reproducer/life-cycle domain. The disagreement is not inconsistency unless both claims purport to use the same identity bearer.

### F. Reproduction is graded

Godfrey-Smith's distinction between marginal and definite collective reproduction has no universal cutoff. A minimal closed cycle can precede integration, germ–soma specialization, or strong suppression of lower-level selection. \(K_{CR}\) identifies the existence and structural kind of a collective cycle, not a scalar degree of organismality.

### G. The same intervention family is not yet fully observed

The early lineage has direct `ACE2` knockout and complementation evidence. The macroscopic study establishes retained clonal life cycle but does not report the same full association-removal, propagule-isolation, and reconstruction protocol used as a matched three-way causal test. Treating its intervention profile as proven would exceed the evidence.

### H. Alternative but defensible boundaries

A bond-graph model could declare entanglement a new type, while a genealogical parentage model treats it as another cohesive realization. Both may be useful for different explananda. The reproducer claim survives because its boundary is fixed by parentage and life-cycle theory, but it remains explicitly domain-relative.

Together these attacks reject a universal invariant while preserving a conditional, biologically motivated equivalence.

## 13. Central decision

**B — CONDITIONAL DOMAIN MODEL**

A scientifically useful distinction exists under an explicitly declared theory of collective reproduction. The same structural criterion classifies:

\[
\text{ancestor}\not\sim_{CR}\text{early snowflake}
\]

and

\[
\text{early snowflake}\sim_{CR}\text{macroscopic snowflake}.
\]

The positive classification is supported by parentage, developmental stage, and life-cycle evidence. The complete intervention-preserving equivalence remains provisional because no located study subjected all three cases to the same intervention family and statistical tolerances.

**Why not A:** established reproduction and life-cycle theories identify the right relation, but they do not uniquely fix candidate units, stages, thresholds, or all empirical interventions. The worked classification is conditional.

**Why not C:** cross-level addition is conceptually captured by collective reproduction and ETI theory. Its universal formalization remains unavailable, but that is outside this declared domain.

**Why not D:** the target is defined well enough for a domain-specific causal test, but the snowflake mechanism itself is already known and the matched validation is incomplete. A new general mechanism question would be premature.

**Why not E:** the workspace's generic term dissolves into established theory in this case, but a genuine empirical/formal gap remains in applying one causal equivalence without retuning.

**Why not F:** observer-free classification fails, yet parentage, multiplicative closure, controls, and interventions constrain the model enough for conditional objectivity.

## 14. Remaining explanatory gap

Q017 resolves the structural positive/negative-control problem but narrows the causal gap to:

> Does the same preregistered collective-unit rule, reproductive-stage partition, association intervention, propagule-isolation assay, and detection threshold recover the predicted ancestor/early/macroscopic classification across replicate lineages?

Published evidence supports the expected answer but does not constitute that matched test. More importantly for the OEE project, the result has so far been validated only in a system whose collective benefit was externally selected and whose biological substrate makes clonal attachment readily available. It remains unknown whether the same relation identifies an unprescribed collective reproducer in a level-blind artificial model without importing model-native group labels.

This is a **causal-validation and measurement gap**, not an unexplained dynamical mechanism. The specific snowflake causal sequence—`ACE2` loss, persistent attachment, growth, stress, and fracture—is already established.

## 15. Problem classification

| Problem type | Q017 result |
|---|---|
| **Definition** | Narrowly resolved for the collective-reproducer claim by \(K_{CR}\); remains conditional on its candidate-unit and stage rules. |
| **Measurement** | **Primary remaining gap.** A common assay, sampling design, and numerical detection tolerance have not been applied across all three controls. |
| **Formalization** | Structural graph equivalence is available; intervention-preserving equivalence is specified but not fully estimated. |
| **Mechanism** | No new mechanism gap in snowflake origin: the `ACE2` attachment–growth–fracture route is known. Recurrence or generality is not yet a well-validated target. |

## 16. Mechanism readiness

**NOT READY**

The domain and identity-bearing relation are now explicit, and structural type-preserving versus type-changing cases can be distinguished. Two mechanism-gate conditions nevertheless fail:

1. the richer equivalence has not passed a matched intervention-and-tolerance test across the three controls;
2. the mechanism producing the specific snowflake transition is already explained by prior art, so asking for it again would not expose a new gap.

The next high-information step is transfer validation in a level-blind system. Only if the same domain relation identifies a collective reproducer there without designer group labels should the project ask which dynamics generate or recurrently transform that relation.

## 17. Known / Underexplored / Potentially Novel / Unknown

### ESTABLISHED / KNOWN

- Snowflake yeast evolved multicellular propagules, juvenile/adult collective stages, and selectable collective life-history traits from a unicellular ancestor.
- `ACE2` loss is sufficient for early snowflake organization, and functional complementation restores unicellularity in an early strain.
- Snowflake propagules are clonal branches produced by fracture and carry genealogical bottlenecks that support collective heritability.
- Later anaerobic lineages became macroscopic and much tougher through cell elongation and branch entanglement while retaining a clonal multicellular life cycle.
- Reproduction theory privileges parent–offspring lineage formation; life-cycle-closure theory privileges multiplication and recurrent connection among declared stages.
- A new collective reproducer is weaker than a completed transition in individuality and does not establish OEE.
- Deep learning contributes no useful additional abstraction to this frontier; multiple realization and implementation drift are already captured by the biological and causal literature.

### PARTIALLY EXPLORED

- Life-cycle closure as a sufficient marker for an ETI; other theories treat individuality as graded and require additional dimensions.
- Intervention-based comparison of parentage and cycle identity across evolved biological implementations.
- The boundary between incidental group propagation and substantial collective reproduction.

### UNDEREXPLORED

- A single preregistered intervention-and-tolerance protocol applied to unicellular, early snowflake, and macroscopic snowflake genotypes.
- Sensitivity of the classification to alternative biologically defensible candidate-unit and stage partitions.
- Transfer of the same equivalence to a level-blind model with no operative group identifier or predefined collective cycle.

### POTENTIALLY NOVEL

None. The proposed equivalence composes established collective-reproduction, life-cycle, intervention, and causal-abstraction concepts. The paired-control application is useful validation, not a new natural kind or mechanism.

### UNKNOWN

- Whether macroscopic snowflake lineages retain the predicted intervention profile under direct matched perturbation rather than structural observation alone.
- Whether a non-retuned collective-reproducer equivalence remains stable across different plausible coarse-grainings.
- Whether the closest level-blind model contains an internally reconstructed collective parent–offspring cycle under this external domain model.

## 18. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

The pass supplies a conditional empirical classifier and identifies missing validation. The causal origin of snowflake clusters is established prior art; the proposition that one equivalence will transfer to another system is a test-design question until the target variables and data are analyzed. [HYPOTHESES.md](HYPOTHESES.md) remains unchanged.

## 19. Highest-information next question

Under the Q017 collective-reproducer equivalence, do propagule-forming lineages in Fernandes, Vroomans, and Colizzi's level-blind model acquire an internally reconstructed collective parent–offspring cycle outside matched ancestors' bounded capacity, without retuning the entity rule, intervention family, or tolerance?
