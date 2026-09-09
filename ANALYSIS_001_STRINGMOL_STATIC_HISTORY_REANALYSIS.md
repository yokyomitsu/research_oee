# Analysis 001 — Stringmol Static-History Re-analysis

Date: 2026-09-09  
Operation: exactly one **T2A — STATIC HISTORY RE-ANALYSIS** pass  
Evidential object: already generated, deposited Stringmol processed histories only

## 1. Why T2A was selected

**Fact.** [Validation 001](VALIDATION_001_STRINGMOL_ADAPTIVE_FUNCTIONAL_NOVELTY.md) froze a two-event finite result:

\[
e_1=\text{nonreciprocal parasitic exploitation before/by }90{,}000
\]

followed in run 2 by

\[
e_2=\text{partner-contingent replication discrimination by }680{,}000.
\]

Both were classified as heritable and selectively favored, and their functional classes were judged distinct. The unresolved question was whether the later portions of the deposited histories contain an additional adaptive functional novelty (AFN) event rather than further change within exploitation, discrimination/defense, replication optimization, or variation production.

**Interpretation.** T2A was the highest-information operation because the 2024 processed deposit contains event-indexed species and reaction tables for all eight surviving long runs. It permits a new deterministic query of old evidence without model execution or regeneration of the authors' preprocessing pipeline.

## 2. Policy boundary

This pass performed read-only analysis of deposited files. It downloaded the authors' processed archive and documentation, verified and extracted the archive in a temporary directory, read every processed run table, deterministically aggregated declared fields, and inspected selected recorded reaction rows.

It did **not** run or compile Stringmol, generate an evolutionary history, change a parameter, modify source code, rerun an experiment, regenerate the processed data from 2021 logs, execute RStringmol, reproduce the paper's figure pipeline, conduct an intervention, search for a mechanism, formulate an OEE theory, or create a hypothesis.

\[
\boxed{\text{evidence}=\text{already generated historical Stringmol data}}
\]

## 3. Data provenance

| Item | Inventory result |
|---|---|
| Primary processed-data DOI | [10.15124/88a8bad0-b23f-4afc-80a6-77e6358b7a8f](https://doi.org/10.15124/88a8bad0-b23f-4afc-80a6-77e6358b7a8f) |
| Earlier input-data DOI | [10.15124/305dfdb6-9483-4c5b-8a01-c030570b9c31](https://doi.org/10.15124/305dfdb6-9483-4c5b-8a01-c030570b9c31); not downloaded or regenerated |
| Archive | `rundata.zip`, 42.0 MiB downloaded; SHA-256 `fc78029b8412ca9cace043aef4d791c071c75d3c9100021239576599a8d3d76a` |
| Documentation | `Measuring_Stringmol_code_and_data_documentation.pdf`, 193 KiB; SHA-256 `0075dba7090024c875ba7e0e942fd259210d23ef91abe247c4ed7654b9b23a9b` |
| Archive integrity | `unzip -t` reported every member `OK`; no corrupt or missing member found |
| Archive members | 1,650 members: 1,640 regular files and 10 directories |
| Runs | `run1` through `run8`, exactly eight; no naming discrepancy |
| Files per run | Exactly 205: 100 `oeeRun<N>props<T>.csv`, 101 `sppcounts<T>.csv`, and one each of `species<0N>.csv`, `popdy<0N>.csv`, `qnn<0N>.csv`, `selfself<0N>.csv` |
| Recorded range | Species snapshots: 0–2,000,000; observed-reaction snapshots: 20,000–2,000,000 |
| Sampling interval | 20,000 timesteps; 101 species and 100 reaction snapshots per completed run |
| Processed provenance | The documentation states that the 2021 logs and derived input files were processed with RStringmol to create this output deposit; that preprocessing takes more than 10 hours and should not be repeated |

All 1,640 regular files were read during the schema/integrity audit: 800 observed-reaction tables, 808 species snapshots, eight species catalogues, eight population summaries, eight QNN files, and eight self-self tables. None was empty. Targeted scientific inspection used the same deposited files, especially run-2 epochs 600,000, 680,000, 1,080,000, 1,500,000, and 2,000,000 and every recorded hypercycle row.

The catalogue sizes were: run 1, 36,129 species; run 2, 51,976; run 3, 39,457; run 4, 59,143; run 5, 32,978; run 6, 45,337; run 7, 42,874; run 8, 44,163.

## 4. Frozen AFN criteria

No criterion was changed after candidate inspection. A candidate qualifies only when all five are supported:

- **N — historical novelty:** the relevant capability or relation was absent earlier in the available lineage/history;
- **F — functional consequence:** the state has a system-grounded causal role in the Stringmol ecology;
- **H — heredity:** the organization persists through copying sufficiently for selection to act;
- **A — adaptation:** the function is selectively favored under the relevant conditions;
- **C — functional-class distinctness:** the causal role differs from every already accepted AFN class.

When 20,000-step sampling prevents proof of absence, this report uses `EARLIER EQUIVALENT NOT FOUND`, not `PROVEN ABSENT`.

## 5. Frozen existing functional classes

- **C1 — exploitative replication relation:** nonreciprocal use of another molecule's copying machinery/resources: one partner causes the other to be copied without reciprocal copying.
- **C2 — partner discrimination:** differential interaction or copy behavior conditioned on partner identity or an equivalent interaction state, including defensive gatekeeping that grants or denies copy-loop access.

Different sequences, opcode counts, binding sites, checks, or reaction traces do not create a new class when they retain one of these roles. The classes were neither broadened nor narrowed after candidate discovery.

## 6. Static-data field audit

**Reconstructable facts.** The deposit records sampled species identity, sequence, first/last logged time, logged abundance, active/passive/unbound counts, QNN activity, observed partner sequences, first product, end-state strings, copy/move/overwrite/toggle counts, binding probability, non-mutating in-vitro reaction length, product count, observed-reaction count, and author-defined booleans for replication, self-replication, parasitism, mutual replication, hypercycle membership, jumping, modification, and new products. `selfself` tables provide the in-vitro self-pair reaction for every recorded species.

**Non-reconstructable facts.** The processed archive does not expose spatial coordinates, events between logged snapshots, a complete mutation pedigree, every product beyond the first, a full instruction-by-instruction trace, or trait-ablation competitions. Sequence similarity is not pedigree. `nobs` is a sampled reaction count, not fitness.

**Boundary.** Exact mutational-operator ancestry or recovery of unsampled transitions would require returning to the input logs and rebuilding lineage/event structure. That line is classified `REQUIRES RAW-HISTORY RECONSTRUCTION` and was stopped. It was not necessary for the central decision below.

## 7. Candidate-discovery procedure

Stage A assigned no AFN status. Before inspection, the following deterministic discovery rules were fixed:

1. scan all eight runs and all recorded times;
2. locate the first and every contiguous sampled episode of the author-defined parasite, mutual-replication, hypercycle, jumper, modification, and new-product categories;
3. record discrete changes in the role and toggle count of the most-observed biological replication reaction at each snapshot;
4. separately flag a post-680,000 first occurrence, a later recurrence of an earlier category, and a category that supplies the most-observed biological-replication row;
5. use counts and durations descriptively, never as an AFN threshold.

For run 2, the primary post-event interval is strictly

\[
T_{\mathrm{post}}=\{t:t>680{,}000\},
\]

so its first sampled point is 700,000. The same numerical cutoff was used only as a cross-run reporting convention; clocks in independent runs do not establish lineage ordering relative to run-2 \(e_2\).

## 8. Functional-reconstruction procedure

Stage B inspected each nominated category at reaction and carrier level:

1. identify copied partner and direction from `pp_Repl1`, `pp_Repl2`, product, and end-state fields;
2. test self-sufficiency using the carrier's `selfself` row;
3. place the carrier using catalogue start/end and sampled abundance;
4. compare the causal role with C1, C2, and any earlier equivalent of the same candidate role;
5. assess heredity from persistence of the copied program/reaction organization;
6. assess adaptation from dominance, persistence, displacement, recurrence, or an author-grounded causal comparison, without treating abundance alone as sufficient.

## 9. Positive and negative controls

| Control | Static result | Sanity-check outcome |
|---|---|---|
| Positive C1: exploitation | `np_Parasite` occurs in every reaction snapshot of all eight runs, from 20,000 through 2,000,000 | **RECOGNIZED**; this is recurrence of C1, not a new event |
| Positive C2: run-2 discrimination region | The most observed run-2 replication reaction changes from a 28/28, one-toggle replicator at 600,000 to a 38/38, three-toggle replicator at 680,000; later dominant reactions use five toggles by 1,100,000 and six by 1,240,000. These are the deposited signatures of the already validated gate/check chronology | **RECOGNIZED AS FROZEN ANCHOR**; processed fields locate the region but the prior program-level validation supplies the functional label |
| Negative: replication adjustment | Length, steps, and toggle count change repeatedly while the recorded role remains self/mutual replication | Correctly retained as parameter/implementation change unless tied to C2 |
| Negative: later parasite turnover | Parasite relations occur at every sampled time while carrier sequences turn over | Correctly retained in C1 |
| Negative: mutation-rate/operator variation | `pp_NewProduct` and `pp_SelfMod` are already present at the first reaction snapshot in every run (except one isolated missing `pp_NewProduct` snapshot in runs 6 and 8); the processed fields do not identify a newly selected operator lineage | Correctly not promoted to AFN |

The positive controls show that the archive can recover the declared relational categories and the run-2 strategy-change region. Its resolution is nevertheless inadequate for discovering arbitrary unencoded functions; later negative claims are restricted to what these processed histories expose.

## 10. Full candidate-event ledger

Stage-A status uses only `CANDIDATE`, `DUPLICATE KNOWN CLASS`, `PARAMETER CHANGE`, or `INSUFFICIENT DATA`.

| ID | Run | Earliest supported time | Pre-event state | Post-event state | Candidate causal role | Discovery signal | Evidence source | Initial status |
|---|---:|---:|---|---|---|---|---|---|
| L01 | 1 | 100,000 | no recorded hypercycle at 20–80k | two isolated hypercycle observations at 100k; three at 120k | reciprocal/dependent copying | first author-defined hypercycle category | reaction + species + self-self | CANDIDATE |
| L02 | 1 | 800,000 | dominant one-toggle mutual/self replication | dominant three-toggle mutual/self replication | added partner checking | discrete dominant-program change | reaction table | DUPLICATE KNOWN CLASS |
| L03 | 1 | 920,000 | earlier hypercycle absent since 120k | hypercycle returns and is continuously recorded through 2m; the most-observed biological-replication row is hypercycle-labelled at 40 snapshots from 980k onward | reciprocal/dependent copying | category recurrence and role replacement | reaction + species + self-self | CANDIDATE |
| L04 | 2 | 40,000 | no hypercycle at 20k | sparse hypercycle observations through 360k | reciprocal/dependent copying | first category occurrence | reaction + species | CANDIDATE |
| L05 | 2 | 680,000 | dominant one-toggle replicator at 600k | dominant three-toggle gate at 680k; five/six-toggle descendants later | partner discrimination/refinement | frozen positive-control region | reaction table + Validation 001 | DUPLICATE KNOWN CLASS |
| L06 | 2 | 1,320,000 | no hypercycle since 360k | sparse hypercycle recurrence at 29 later snapshots, maximum 19 of 4,680 reaction observations | reciprocal/dependent copying | category recurrence | reaction + species | CANDIDATE |
| L07 | 3 | 60,000 | no hypercycle at 20–40k | nine sparse hypercycle snapshots ending 660k | reciprocal/dependent copying | first category occurrence | reaction + species | CANDIDATE |
| L08 | 3 | 1,540,000 | dominant one-toggle self/mutual replication | alternating dominant three-toggle implementations | added partner checking | discrete dominant-program change | reaction table | DUPLICATE KNOWN CLASS |
| L09 | 4 | 20,000 | unobserved initial reaction state | one hypercycle observation, followed by sparse later recurrences including 1880–1940k | reciprocal/dependent copying | category presence/recurrence | reaction + species | CANDIDATE |
| L10 | 4 | 1,060,000 | one/three-toggle replication | later two-, four-, five-, and six-toggle dominant implementations | added checking/replication implementation | discrete program changes | reaction table | DUPLICATE KNOWN CLASS |
| L11 | 5 | 160,000 | no hypercycle through 140k | sparse early and post-1.08m hypercycles; maximum 43 of 2,909 observations | reciprocal/dependent copying | first category and later recurrence | reaction + species | CANDIDATE |
| L12 | 5 | post-680k | dominant one-toggle self/mutual replication | same recorded role/toggle class through 2m despite genotype turnover | replication optimization/turnover | lineage replacement without category change | reaction + species | PARAMETER CHANGE |
| L13 | 6 | 100,000; stable regime from 280–320k | no recorded hypercycle at 20–80k | hypercycles recur; from 320k the most-observed biological-replication row is hypercycle-labelled at 84 snapshots through 2m | reciprocal obligate copying/dependence | category onset then dominant-role replacement | reaction + species + self-self | CANDIDATE |
| L14 | 6 | 1,760,000 | hypercycle-dominated replication | one-snapshot parasite-dominated interruption, then hypercycle dominance returns | exploitative copying | dominant-role interruption | reaction table | DUPLICATE KNOWN CLASS |
| L15 | 7 | 140,000 | no earlier hypercycle | early hypercycle cluster peaks at 240k; seven sparse post-680k recurrences | reciprocal/dependent copying | first category and recurrence | reaction + species | CANDIDATE |
| L16 | 7 | 1,240,000 | dominant one-toggle self/mutual replication | three-toggle and then five-toggle dominant implementations | added partner checking | discrete dominant-program change | reaction table | DUPLICATE KNOWN CLASS |
| L17 | 8 | 860,000 | dominant one-toggle self/mutual replication | alternating three-toggle implementations, later returning mainly to one-toggle | added partner checking | discrete dominant-program change | reaction table | DUPLICATE KNOWN CLASS |
| L18 | 8 | 980,000 | no recorded hypercycle through 960k | first hypercycle category, followed by 16 sparse snapshots through 1.74m | reciprocal/dependent copying | first post-cutoff category occurrence | reaction + species + self-self | CANDIDATE |
| L19 | 1–8 | recurrent after 680,000 | extant host/parasite pairs | new parasite carrier sequences with the same one-way copying semantics | exploitation | species turnover within `np_Parasite` | reaction + species | DUPLICATE KNOWN CLASS |
| L20 | 1–8 | unresolved | modification/new-product processes already present at 20k | later quantitative and program changes | mutation-process control or active modification | modification, overwrite, new-product, jumper, and opcode-count changes | processed reaction fields | INSUFFICIENT DATA |

No run was omitted. No deposited parameter-change file or simulation intervention exists in this archive; `PARAMETER CHANGE` in L12 denotes an evolved reaction/program state change, not an analyst or experimenter change.

## 11. Post-second-AFN candidates

| Candidate | Post-680 evidence | Whole-history novelty check | Final AFN audit |
|---|---|---|---|
| Run-1 stable hypercycle regime (L03) | continuous category from 920k–2m; the most-observed biological-replication row is hypercycle-labelled at 40 snapshots; maximum category count 1,529/3,208 observations | equivalent reciprocal hypercycle semantics already recorded at 100k and 120k | F and later ecological establishment supported; N fails for the later transition |
| Run-2 later hypercycles (L06) | 29 snapshots, but only 1–19 observations each | same category already occurs at 40k, 100k, 140k, 220k, and 360k | N fails; A not established |
| Run-4/5/7 recurrences | sparse, non-dominant post-cutoff episodes | same category occurs before/by 160k in each run | N fails; A weak or not established |
| Run-6 continuing hypercycle regime (L13) | dominant throughout the post-cutoff interval except one snapshot | first recorded at 100k and dominant by 320k, before \(e_2\)'s run-2 time | later state is adaptive ecological persistence, not a later new class event |
| Run-8 first hypercycles (L18) | first at 980k; at most two hypercycle observations in any snapshot; focal carrier totals are 1–25 and carrier windows are 0–180k | `EARLIER EQUIVALENT NOT FOUND` in run 8 at 20k resolution | N and F plausible; H at most strongly consistent for a few pairs; A **NOT ESTABLISHED** |
| Later toggle/check programs | several runs acquire new dominant toggle counts | the causal problem remains partner-contingent copying/defense | C2; C fails |
| Later parasites | present at every post-cutoff snapshot | C1 already present from the first reaction snapshot | C1; N and C fail |
| Mutation/operator candidate | processed counts vary post-cutoff | modification/new-product/jumper processes occur earlier; no operator pedigree or selected-current-function field | N/F/H/A alignment unresolved; `REQUIRES RAW-HISTORY RECONSTRUCTION` for lineage-level adjudication |

No post-\(e_2\) candidate satisfies N, F, H, A, and C jointly.

## 12. Later defense evolution

**Fact.** Run 2 moves from the validated three-toggle strategy at 680k to dominant five-toggle replication at 1.10–1.20m and six-toggle replication from 1.24m through 2m. Runs 1, 3, 4, 7, and 8 also show later discrete increases or alternation in the toggle count of the most-observed replication program. Run 5 remains dominated by a one-toggle relation; run 6 is mainly hypercycle-dominated.

**Interpretation.** These are stronger static discriminators of implementation turnover than the publication-only record, but no deposited field assigns a new ecological problem to them. Added or reorganized checks still condition copying on partner state. They are **new defense implementations**, not a new functional relation:

\[
\boxed{\text{later defensive program change}=C2\text{ unless different causal semantics are demonstrated}.}
\]

## 13. Later parasite evolution

**Fact.** `np_Parasite` is present at all 100 reaction snapshots in every run. Sequence catalogues and pair rows show extensive carrier turnover, but the recorded relation remains one-way copying.

**Interpretation.** Later parasite genotypes that evade a current defense still exploit another program's copying machinery. No post-\(e_2\) row establishes active interference, reciprocal dependency, or another role attributable to a parasite carrier beyond that relation. Classification: `SAME FUNCTIONAL CLASS — C1`.

## 14. Mutation-process evolution

**Fact.** Copy, overwrite, toggle, jumping, modification, and new-product fields expose changed reaction mechanics. `pp_NewProduct` and `pp_SelfMod` are not new post-\(e_2\) categories: they occur from the first reaction snapshot in all runs. The archive does not encode a mutation-parent edge or a field saying that an operator-bearing carrier is favored because of current variation control.

**Interpretation.** Quantitative mutation opportunity and emergent rearrangement remain evolution-of-variation evidence, not AFN by default. Outcomes are:

- identifiable changed variation production: **NEW VARIATION MECHANISM** is possible at reaction level;
- selected current modulation of that variation: **FUNCTIONAL STATUS UNRESOLVED**;
- AFN classification: **NOT ESTABLISHED**.

Resolving a particular operator's genealogy from input logs is `REQUIRES RAW-HISTORY RECONSTRUCTION`; that forbidden branch was not performed.

## 15. Other candidate functional changes

The processed ontology additionally marks mutual replication, jumping, active/passive modification, and new products. Mutual replication, modification, new products, and jumping all occur early; no new author-defined relational category first appears after \(e_2\) except run 8's sparse hypercycle records. QNN, species turnover, length, binding probability, reaction steps, and opcode counts locate change but do not specify a causal ecological role.

No cooperative structure beyond author-defined mutual replication/hypercycle semantics can be inferred from topology alone. No spatial-shielding claim can be evaluated because the processed output has no coordinates. Unexplained major QNN or genotype change without reaction semantics is therefore not promoted; it is at most a `MEASUREMENT-ESCAPE CANDIDATE`.

## 16. Event-level heredity

| Candidate | Heredity result | Basis |
|---|---|---|
| C1 parasite turnover | CLEARLY HERITABLE | copied carrier sequences recur as logged populations |
| C2 later checking programs | CLEARLY HERITABLE for program strings | dominant sequence-defined replication programs persist and replace alternatives |
| Run-1 late hypercycle | STRONGLY CONSISTENT WITH HEREDITY | focal non-self-replicating components `sp12349` and `sp12351` persist 180–260k sampled timesteps with total logged instances 3,306 and 3,878; later component lineages persist similarly |
| Run-6 hypercycle regime | STRONGLY CONSISTENT WITH HEREDITY | non-self-replicating components such as `sp4336` (280–720k; 10,932 logged instances) and `sp6382` (480–700k; 5,573) are repeatedly produced only in partner relations |
| Run-8 hypercycles | HEREDITY UNRESOLVED at event level | most carrier species are observed once or briefly; the longest focal pair totals only 23 and 25 logged instances |
| Mutation operator | HEREDITY UNRESOLVED for the operator | successful products can be heritable without the variation-generating relation itself being a stable selected trait |

## 17. Event-level adaptation

| Candidate | Adaptive evidence | Classification |
|---|---|---|
| Later C2 implementations | repeated dominance and persistence in the already validated ecological setting; exact benefits remain implementation-specific | STRONGLY SUPPORTED as adaptation within C2 |
| Later parasite carriers | persistent one-way copying and repeated replacement | PARTIALLY/STRONGLY SUPPORTED within C1; class novelty absent |
| Run-1 late hypercycle regime | the most-observed biological-replication row is hypercycle-labelled at 40 snapshots and the category persists to the observation limit | STRONGLY SUPPORTED for ecological establishment; not a historically new later role |
| Run-6 hypercycle regime | the most-observed biological-replication row is hypercycle-labelled at 84 snapshots from 320k to 2m, with one interruption | STRONGLY SUPPORTED for ecological establishment; temporal condition \(t>t(e_2)\) fails for origin/establishment |
| Run-2/4/5/7 post-cutoff hypercycles | sparse or intermittent reaction records without displacement attributable to the role | NOT ESTABLISHED or PARTIALLY SUPPORTED |
| Run-8 first hypercycles | maximum two of 4,766 reaction observations at onset; low-abundance, short-lived carriers; no sweep or displacement | NOT ESTABLISHED |
| Mutation/operator variation | no comparative advantage attributable to current variation control | NOT ESTABLISHED |

Counts here are descriptive consequences, not a candidate-selection threshold. A population or reaction increase was never used alone to infer AFN.

## 18. Functional-class pairwise matrix

| Candidate | Comparison class | Same causal role? | Same ecological/selective problem? | Same interaction semantics? | Distinct class? | Evidence |
|---|---|---|---|---|---|---|
| Later defense/check programs | C2 partner discrimination | Yes | Yes | Yes at role level; implementation differs | SAME | toggle/check program and copy-gating continuity |
| Later parasite genotypes | C1 exploitation | Yes | Yes | Yes: one-way copying | SAME | `np_Parasite` and directional replication flags |
| Reciprocal hypercycle dependence | C1 exploitation | No | Not exactly | No: reciprocal production rather than one-way exploitation | DISTINCT | paired hypercycle/mutual-replication flags; non-replicating self-self reactions |
| Reciprocal hypercycle dependence | C2 discrimination | No | No | No: productive reciprocal dependency rather than partner exclusion | DISTINCT | partner products and self-self failure |
| Run-1/2/4/5/7 later hypercycle | earlier hypercycle class in same run | Yes | Yes | Yes under the deposited category and reaction direction | SAME | earlier recorded `np_Hypercycle` rows |
| Run-6 post-680 hypercycle persistence | run-6 pre-680 hypercycle regime | Yes | Yes | Yes | SAME | continuous author-defined category and carrier replacement |
| Run-8 hypercycle | C1 and C2 | No | Not exactly | No | DISTINCT, but AFN unresolved | F clear enough; A not established |
| Mutation/operator variation | C1/C2 | No if selected variation control exists | No | No | UNRESOLVED | present fields do not establish selected current control |

Genetic distance was not used as functional distance.

## 19. Cross-run convergence

### Same-class convergence

| Relation/strategy | Cross-run result |
|---|---|
| C1 exploitation | recorded at every sampled reaction time in 8/8 runs |
| Mutual replication | recorded at every sampled reaction time in 8/8 runs |
| Toggle-rich replication implementation | dominant later reactions exceed one toggle in runs 1, 2, 3, 4, 7, and 8; semantic assignment beyond the validated run-2 anchor remains partly author/analyst dependent |
| Hypercycle category | appears at least once in 8/8 runs; supplies the most-observed biological-replication row only in runs 1 and 6 |

This is convergence/recurrence of categories, not a count of new functional classes.

### Across-system repertoire

The deposited histories contain three objectively encoded interaction semantics: one-way exploitation, partner-contingent/checking implementations, and reciprocal hypercycle/dependency. Only C1 and C2 have event-aligned AFN support under the frozen test. The third semantic repertoire item is not thereby a third accepted AFN event.

## 20. Within-lineage AFN recurrence

The strongest accepted within-lineage sequence remains run 2:

\[
e_1\;(\text{C1 exploitation, before/by }90{,}000)
\rightarrow
e_2\;(\text{C2 discrimination, by }680{,}000).
\]

Run-2 post-\(e_2\) hypercycles are sparse recurrences of a class already recorded at 40,000. Run-1 and run-6 hypercycle regimes provide strong evidence that reciprocal dependence can establish, but their class appears earlier in those histories and is not aligned as a novel event after a validated C2 event. Run 8 supplies later first occurrence but not adaptation. Therefore no defensible \(e_3\) can be appended.

## 21. Observation-window censoring

Every run ends at 2,000,000. Non-observation means only:

\[
\boxed{\text{no additional qualifying event recorded before }T_{\max}=2{,}000{,}000.}
\]

The reaction record begins at 20,000 and samples every 20,000 steps. Earlier, shorter, or between-snapshot events can be missed. This right- and interval-censored result does not show that Stringmol lacks capacity for later AFN. No AFN rate is estimated.

## 22. Measurement-escape audit

The archive is unusually rich but deliberately organized around fixed Stringmol measures. It can detect activity and declared reaction/network semantics; it cannot prove that those semantics exhaust functional change. Large sequence/QNN changes without a declared reaction role are `MEASUREMENT-ESCAPE CANDIDATE`, not hidden innovations.

The absence result is consequently bounded:

\[
\text{no post-}e_2\text{ AFN found by reconstructable deposited semantics}
\not\Rightarrow
\text{no later functional innovation occurred}.
\]

No spatial candidate can be semantically reconstructed from this deposit, and no arbitrary functional label was invented to fill that gap.

## 23. Analyst-dependence audit

| Attribution | Objective reaction semantics | Lineage dynamics | Author-defined measure | Retrospective interpretation | Strength |
|---|---:|---:|---:|---:|---|
| C1 recurrence | high | medium | high | low | high |
| C2 run-2 anchor | high once focal rows are fixed | high from Validation 001 | medium (`ctogg`) | medium | frozen positive anchor |
| Later C2 refinements | medium | medium | high | medium | adequate for same-class exclusion, not a new function |
| Run-1/6 reciprocal dependence | high (`Repl` direction + self-self failure) | medium-high persistence | high (`np_Hypercycle`) | low-medium | strong functional/ecological result |
| Run-8 AFN claim | high for interaction semantics | low | high | would be high | too weak; rejected |
| Selected mutation control | low-medium | low | medium | high | too weak; unresolved |

No accepted third event depends mainly on retrospective labeling, because no third event is accepted.

## 24. Strongest positive interpretation

**Fact.** Static histories strengthen the empirical reality of reciprocal dependent replication: in runs 1 and 6, hypercycle-labelled partners do not replicate in self-self tests, copy one another in observed reactions, persist through carrier replacement, and supply the most-observed biological-replication row over long intervals.

**Limit.** This does not extend the frozen AFN sequence. In run 1 the same functional class is already recorded at 100–120k before the later stable regime; in run 6 it arises and dominates before 680k; in run 8 its later first occurrence lacks adaptive establishment.

The strongest defensible AFN sequence is therefore unchanged:

\[
\boxed{e_1\rightarrow e_2;\quad e_3\text{ not supported}.}
\]

## 25. Strongest skeptical interpretation

For the focal run-2 post-\(e_2\) history, the skeptical null survives:

\[
\boxed{\text{two genuine AFN events, followed by adaptation within established roles}.}
\]

Later run-2 changes are absorbed by C1 exploitation, C2 discrimination/defense, replication optimization, or unresolved variation production. Sparse hypercycles are a recurrence of a pre-\(e_2\) role, not a new later class. Across other runs, reciprocal dependence can become ecologically important, but it does not supply the required ordered third event.

This null is evidence about deposited histories, not a claim that the substrate cannot innovate further.

## 26. Central decision

\[
\boxed{\textbf{E — TWO-EVENT AFN RECORD REMAINS THE STRONGEST CLAIM}}
\]

No additional post-\(e_2\) event survives N/F/H/A/C. Later hypercycle regimes either repeat an earlier equivalent role, originate/establish before the validated second-event time, or lack adaptive evidence. Later defenses and parasites remain C2 and C1. Mutation-process candidates lack event-aligned heredity and adaptive function.

This decision does not revise either frozen positive anchor and does not infer incapacity.

## 27. Mechanism-target readiness

\[
\boxed{\textbf{MECHANISM TARGET NOT YET STABLE}}
\]

Stringmol remains a valuable finite two-AFN case, but it lacks three event-aligned distinct AFN classes or strong multi-run within-lineage recurrence. That is insufficient to stabilize a Stringmol-specific mechanism program. No mechanism was investigated.

## 28. Cross-system implication

Stringmol remains the reviewed matrix's strongest finite repeated-AFN case. Its count stays at two supported classes/events. The static pass adds a sharper boundary: reciprocal hypercycle dependence is real and can dominate, yet its deposited timing does not extend the post-discrimination AFN sequence. `Ongoing AFN` and `Stringmol is OEE` remain **NOT ESTABLISHED**.

The historical [Evidence Matrix 001](EVIDENCE_MATRIX_001_ADAPTIVE_FUNCTIONAL_NOVELTY.md) is unchanged.

## 29. Next-operation decision

\[
\boxed{\textbf{RETURN — GLOBAL HALLMARK PROGRAM}}
\]

T1S is not licensed because no third event or multi-run within-lineage AFN recurrence was established. T2B is not selected because class distinctness is not the dominant ambiguity: reciprocal dependence is distinguishable from C1/C2. T2C is not selected because the only later first-origin case (run 8) is sparse and low-information, while the stronger established regimes fail the temporal novelty requirement. T4S is not selected because measurement escape limits the negative result but did not prevent resolution of the deposited high-priority candidates. STOP is unnecessary because raw reconstruction is not decisive for the central decision.

## 30. Highest-information next operation

Exactly one next operation is selected:

> **Return to the global adaptive-functional-novelty hallmark program and select its next cross-system evidence bottleneck; do not begin a Stringmol mechanism contrast.**

That operation is not conducted here.

## 31. Stop condition

The Stringmol-specific branch stops now. It should remain closed unless a future, separately authorized operation has event-aligned deposited evidence that can jointly resolve origin, functional semantics, heredity, and adaptive consequence for a post-discrimination candidate without silently rebuilding the forbidden raw-history pipeline. Otherwise the research returns to the global hallmark program.

Finite recurrence remains finite:

\[
\boxed{\text{two finite AFN events}\neq\text{ongoing AFN}\neq\text{OEE}.}
\]

## Data-analysis provenance

### Downloaded identifiers and checksums

- Processed deposit DOI: `10.15124/88a8bad0-b23f-4afc-80a6-77e6358b7a8f`.
- `rundata.zip`: SHA-256 `fc78029b8412ca9cace043aef4d791c071c75d3c9100021239576599a8d3d76a`.
- `Measuring_Stringmol_code_and_data_documentation.pdf`: SHA-256 `0075dba7090024c875ba7e0e942fd259210d23ef91abe247c4ed7654b9b23a9b`.
- Earlier raw/input DOI recorded but not downloaded: `10.15124/305dfdb6-9483-4c5b-8a01-c030570b9c31`.

### Exact deposited files used

All files under `rundata/runs/run1` through `run8` were inventoried. Analysis read every `oeeRun<N>props<T>.csv`, `sppcounts<T>.csv`, `species<0N>.csv`, `popdy<0N>.csv`, `qnn<0N>.csv`, and `selfself<0N>.csv`. No upstream file was edited.

### Commands and helper scripts

Core commands were `curl -L` from the York archival endpoint, `shasum -a 256`, `unzip -t`, `unzip -l`, `unzip -q`, `find`, `file`, `sed`, `rg`, and Python 3 read-only CSV/JSON queries. The six-page documentation was text-extracted and rendered to PNG for visual verification with temporary `pypdf` and `pymupdf` packages.

Three minimal temporary scripts were used:

- `/private/tmp/stringmol-t2a.B3D4KE/analyze_static.py`, SHA-256 `0666ed1086164f4d69efa64cd969693efd3a611ad1e142902912ad6e8c338bc1`: reads every reaction/species-snapshot/species-catalogue/QNN table and emits deterministic category, time, carrier, population, and activity summaries;
- `/private/tmp/stringmol-t2a.B3D4KE/query_summary.py`, SHA-256 `f5d04ffce91bc348b069131af4cf11f5646fb255ffde4cb23dd051dd69b2d430`: prints hypercycle chronology, focal pair/carrier persistence, and selected category counts;
- `/private/tmp/stringmol-t2a.B3D4KE/top_reactions.py`, SHA-256 `095a6265465d2a965f384beb64450ef52552299754b1c5b65a79a36dc50d158b`: records the most-observed biological-replication role/toggle signature at every snapshot and compresses exact discrete segments.
- `/private/tmp/stringmol-t2a.B3D4KE/audit_all_tables.py`, SHA-256 `a2ccf56be1f62f731b09eea7538cf8fa89d23570497ba9a0ed9f9cd7bb29526d`: reads every CSV and reports file-family counts, physical row counts, and empty files.

The large generated `summary.json` was temporary only (SHA-256 `ed444d668d1e390bd9cb47e2a8d2f5157efdc05f570e984efea81aa9cfe32ef0`) and was not added to the repository.

### Runtime versions and transformation status

- Operating shell: zsh 5.9 (`arm64-apple-darwin25.0`).
- Python: system Python 3.9.6 used for standard-library CSV/JSON analysis and document inspection; `uv 0.12.7` installed temporary PDF tools under `/private/tmp` (`pypdf 6.18.0`, `pymupdf 1.28.2`; package resolution used CPython 3.12.7).
- Archive extraction was lossless. CSV parsing converted R-style integer strings such as `1e+05` to exact integral values via `int(float(value))`; no binning, smoothing, resampling, stochastic operation, or lossy scientific transformation was used.
- Derived summaries are deterministic aggregations of deposited rows. `nobs` counts were preserved as integers.
- No Stringmol executable, simulator, compiler, RStringmol preprocessing pipeline, mutation experiment, or evolutionary model was run.
- No third-party dataset or temporary analysis artifact was committed to this repository.
