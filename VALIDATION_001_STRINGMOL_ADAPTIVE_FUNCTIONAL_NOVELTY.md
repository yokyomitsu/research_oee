# Validation 001 — Stringmol Adaptive Functional Novelty

Date: 2026-09-09

Scope: exactly one system-specific validation pass over already published Stringmol histories. This is not Q028. No Stringmol run, model modification, deposited-data analysis, figure regeneration, simulation, statistical experiment, mechanism search, or hypothesis is performed.

## 1. Why Stringmol was selected

[Evidence Matrix 001](EVIDENCE_MATRIX_001_ADAPTIVE_FUNCTIONAL_NOVELTY.md) found heterogeneous failures across artificial evolutionary systems and selected **T2 — SYSTEM-SPECIFIC VALIDATION**. Stringmol was the strongest near-positive case because it combines intrinsic copying and selection with published reaction-level accounts of parasite exploitation, replication strategies, partner discrimination, hypercycles, and mutation-process change. The matrix left one decisive issue unresolved: whether its histories contain more than adaptation and implementation turnover inside one host–parasite functional regime.

This pass tests that evidence boundary only. It does not ask whether Stringmol is generally open-ended and does not infer a mechanism for OEE.

## 2. Exact validation question

\[
\boxed{
\text{Do the published Stringmol evolutionary histories establish at least two}
\text{ temporally separated, heritable, selectively favored innovations}
\text{ belonging to defensibly distinct functional classes?}
}
\]

The evidence chain is retained:

\[
N\rightarrow F\rightarrow A\rightarrow O,
\]

where novelty, function, adaptation, and event-based recurrence require separate support. Repeated AFN in a finite history is weaker than ongoing AFN and much weaker than OEE.

## 3. Stringmol system boundary

**Facts.** A Stringmol molecule is a variable-length sequence in a fixed assembly-like instruction language. Sequence-dependent alignment determines whether two strings bind and which program starts; execution can move between the bound strings, so a reaction can depend on both programs. The experiment begins with a hand-programmed, 65-opcode replicator that binds another string, copies it, and cleaves the copy. Copying introduces substitutions, insertions, and deletions. Molecules decay, and in the spatial model they bind and place products locally. A sequence persists only if the reaction ecology keeps producing it. [Hickinbotham, Stepney & Hogeweg 2021](https://doi.org/10.1098/rsos.210441)

The seed directly supplies a general copying program, two binding regions, and access to the fixed opcode language. It does **not** directly encode the later evolved toggle gate, multiple partner checks, the observed self-scanning organization, or a catalogue of parasite species. Parasitism is relational: for a pair \((R,P)\), \(R\) copies \(P\) while \(P\) does not copy \(R\).

**Pre-enablement classification: GENERIC SUBSTRATE ENABLEMENT.** The fixed language and reaction physics constrain every possible program, but they do not enumerate the historical programs or context-dependent reaction roles. Computational expressivity does not establish unbounded functional novelty, while ancestral opcodes do not by themselves constitute ancestral functions. [Hickinbotham et al. 2016](https://doi.org/10.1162/ARTL_a_00180)

## 4. Published-history provenance

The primary 2021 experiment comprised 20 spatial runs; 12 became extinct and eight continued to \(T=2{,}000{,}000\). Aggregate plots cover all eight survivors, while the detailed execution-level chronology is chiefly reconstructed for **run 2** at six published epochs:

\[
t_1=90{,}000,
\quad t_2=600{,}000,
\quad t_3=680{,}000,
\quad t_4=1{,}080{,}000,
\quad t_5=1{,}500{,}000,
\quad t_6=2{,}000{,}000.
\]

The 2024 paper analyzes those eight long histories using generic evolutionary-activity measures followed by Stringmol-specific measures. Its contribution is primarily to measurement and interpretation: generic activity can locate interesting change, but reaction-specific analysis is needed to identify what changed. [Stepney & Hickinbotham 2024](https://doi.org/10.1162/artl_a_00399)

The authors' supplementary documentation explicitly identifies the 2021 logs and derived data as the input dataset for the later paper and a separately deposited processed dataset as its output. No deposited code or data were executed or reanalyzed here. [Supplementary documentation](https://pure-research.york.ac.uk/ws/portalfiles/portal/76644523/Measuring_Stringmol_code_and_data_documentation.pdf), [2021 dataset](https://doi.org/10.15124/305dfdb6-9483-4c5b-8a01-c030570b9c31), [2024 processed dataset](https://doi.org/10.15124/88a8bad0-b23f-4afc-80a6-77e6358b7a8f)

## 5. Event-identification method

An event is counted once when a historically new inherited reaction organization acquires a scientifically grounded causal role. Multiple plots, metrics, reaction diagrams, or publications describing the same change do not create additional events.

The local function levels are:

- **F0 — PARAMETER / STATE CHANGE:** quantitative change in an established role.
- **F1 — NEW IMPLEMENTATION OF ESTABLISHED FUNCTION:** a new mechanism realizes an already established causal role.
- **F2 — NEW FUNCTIONAL RELATION:** a new causal capability or interaction role appears.
- **F? — INDETERMINATE:** the publication does not support a stable distinction.

The adaptive-evidence labels are **DIRECT CAUSAL SUPPORT**, **STRONG COMPARATIVE SUPPORT**, **CORRELATIONAL SUPPORT**, and **ADAPTIVE LINK NOT ESTABLISHED**. Heredity is labeled **CLEARLY HERITABLE**, **PROBABLY HERITABLE**, or **HEREDITY NOT RESOLVED**.

Functional equivalence is judged locally: if two implementations would still solve the same system-grounded causal problem after historical coding details were removed, they are the same functional class. This does not impose a universal function ontology.

## 6. Candidate event ledger

Exact times are reported only for the run-2 epochs supplied by the paper. Aggregate or incompletely localized claims remain explicitly unordered.

| Event ID | Run | Time/epoch | Ancestral state | Derived state | Authors' description | Figure/table/source | Evidence resolution |
|---|---|---|---|---|---|---|---|
| E1 | Run 2 | Before/by \(t_1=90{,}000\) | Seed-like mutual replicators | Short strings copied by replicators without reciprocating | Parasites have already emerged and occupy the trailing edges of replicator waves | 2021 §§2.1–2.3, Fig. 3 | STRINGMOL-SPECIFIC MEASURE + QUALITATIVE HISTORY INTERPRETATION |
| E2 | Run 2 | \(t_2=600{,}000\) | Seed-like replication ecology | Short mutually replicating patches with shorter parasites | Replicators shorten and compete more closely with parasites for copying resource | 2021 §§2.3–2.5, Figs. 3–5 | DIRECT PROGRAM/REACTION INSPECTION |
| E3 | Run 2 | By \(t_3=680{,}000\) | Copying follows self-scan but admits an earlier parasite | Execution toggles to the partner and must return before the copy loop is reached | Toggle-based gatekeeping prevents the earlier parasite from being copied and holds it in an unproductive reaction | 2021 §2.4, Fig. 4 | DIRECT PROGRAM/REACTION INSPECTION |
| E4 | Run 2 | \(t_4=1{,}080{,}000\) | Faster unprotected and slower protected replicators coexist | Slower protected strategy dominates | Parasite protection carries a replication cost yet wins under parasite pressure | 2021 §§2.4–2.5, Figs. 4–5 | STRINGMOL-SPECIFIC MEASURE + DIRECT PROGRAM/REACTION INSPECTION |
| E5 | Run 2 | \(t_5=1{,}500{,}000\) | Earlier toggle gate can be defeated | Additional partner-code checks restrict copy-loop access | More elaborate discrimination coincides with high population and near-elimination of parasites | 2021 §§2.3–2.5, Figs. 3–5 | DIRECT PROGRAM/REACTION INSPECTION |
| E6 | Run 2 | \(t_6=2{,}000{,}000\) | Costly elaborate defense under low parasite abundance | Shorter/reorganized strategy; parasites return; ZAA, BBB, and Z participate in a dependent reaction structure | Defense pressure relaxes, efficiency is favored, and parasitism re-emerges | 2021 §§2.3–2.5, Figs. 3–5 | DIRECT PROGRAM/REACTION INSPECTION + QUALITATIVE HISTORY INTERPRETATION |
| E7 | Run 2 lineage | Exact time not reported separately | Point-mutation copying with seed-derived cleavage | A point mutation changes binding/cleaving and starts a cascade ending in the first self-scanner | Emergent macromutational route to E3 | 2021 §2.6, Fig. 6 | DIRECT PROGRAM/REACTION INSPECTION; same innovation history as E3, not an additional AFN event |
| E8 | Surviving-run aggregate | TEMPORAL ORDER NOT ESTABLISHED | Self-copying or asymmetrically copying species | Short two-member mutual dependence/hypercycle in some runs | Some histories become dominated by short hypercycles | 2021 §2.9; 2024 aggregate analysis | STRINGMOL-SPECIFIC MEASURE; run/event placement incomplete in the publications |
| E9 | Multiple runs | Repeatedly, exact event coordinates not catalogued | Current replicator strategies | New parasite species arise from mutated replicators | Parasites repeatedly originate from hosts rather than a persistent parasite lineage | 2021 §§2.4, 2.9; 2024 | STRINGMOL-SPECIFIC MEASURE; individual innovations not event-resolved |
| E10 | Run 2 / aggregate | Coupled to E3 and other replication changes | Baseline copy-error process | Self-scanning approximately doubles effective point mutation; evolved execution also produces macromutations | Mutation-process change | 2021 §§2.4, 2.6 | DIRECT PROGRAM/REACTION INSPECTION; causal role in later adaptation not established |

E3, E4, E5, and the self-scanning part of E7 are not four independent functional novelties. They are evidence about origin, establishment, and refinement of one defensive-discrimination class.

## 7. Slower-replication event

Slower replication alone is **F0 — PARAMETER / STATE CHANGE**. The paper shows that the relevant strategies incur longer execution times and can be longer, so the result is not simply optimization for faster copying. But slow speed is not itself evidence of active regulation.

The causal interpretation strengthens only when the slowing is tied to an added operation: self-scanning imposes a fixed cost that short parasites cannot avoid, and partner-code checks delay access to copying. Those are new implementations of parasite defense (**F1**) and, for explicit partner-contingent gatekeeping, part of the later **F2** discrimination event. The rate change must not be counted separately from the mechanism producing it.

## 8. Self/non-self discrimination

This is the strongest post-parasitism F2 event.

1. **Causal operation.** In the dominant \(t_3\) reaction, execution moves to the bound partner and must be returned by compatible partner code before the copy loop is entered.
2. **Ancestral absence.** The seed and earlier replicators copied a bound template without this return-code gate.
3. **Altered copying relation.** A parasite that exploited earlier replicators lacks the required toggle and is no longer copied; its code can instead execute while the pair is trapped in an unproductive reaction.
4. **Adaptive consequence.** The protected class pays a replication cost but subsequently dominates; by \(t_5\), added checks accompany near-removal of parasites and the paper attributes the high population chiefly to evolved resistance rather than a small efficiency gain.
5. **Heredity.** The gate and checks are parts of copied, mutating program strings and occur in successful replicator lineages.
6. **Evolutionary origin.** The detailed lineage reconstruction derives the first self-scanner and later gatekeeping organization from mutations and changed binding/cleavage, not from the seed design.

Classification: **F2 — NEW FUNCTIONAL RELATION**, **CLEARLY HERITABLE**, **STRONG COMPARATIVE SUPPORT** for adaptation. The reaction counterfactual directly establishes blocking; the evolutionary advantage is strongly comparative rather than a published trait-ablation competition.

## 9. Mutation-rate evolution

Self-scanning reuses copying operations to overwrite a string with the same symbols, approximately doubling the opportunity for point mutation. That establishes a changed effective mutation rate, but not selected mutation-rate control.

The published history does not show that increased mutation generation itself has an independent current advantage, nor that variants are favored because they modulate mutation rate. It may be a pleiotropic consequence of parasite defense. Classification: **F0** for the quantitative rate change, **PROBABLY HERITABLE** as a consequence of an inherited execution path, **ADAPTIVE LINK NOT ESTABLISHED** for mutation-rate modulation as a function. Established evolution-of-evolvability concepts cannot supply the missing event-level adaptive link.

## 10. Emergent mutational operators

Stringmol explicitly supplies point mutation, but changed binding, pointer placement, and cleavage can cause one mutation to generate cascades and large sequence rearrangements. The 2021 lineage to the first self-scanner demonstrates this emergent macromutational production route.

As a variation-generating relation this is a candidate **F2**: it changes how inherited variants are produced. It is not thereby AFN. Several cascade intermediates are not self-sustaining, and the publication does not show that a stable operator-bearing lineage is favored because of its mutational operator. The result therefore has **ADAPTIVE LINK NOT ESTABLISHED** and **HEREDITY NOT RESOLVED** for the operator as a selectable trait, even though the eventual replicator product is inherited and successful.

## 11. Defense loss / re-emergence

Run 2 provides a valuable control. At \(t_5\), complex partner checks suppress parasites. When parasites become rare, the cost of defense is no longer repaid; more efficient strategies return, and parasites re-emerge by \(t_6\). Later reactions again contain mechanisms that combat parasitism.

This is strong evidence that the defensive role is under changing selection. It is not a new function each time:

\[
\boxed{
\text{defense gain}\rightarrow\text{defense loss}\rightarrow\text{defense regain}
=\text{reversible adaptation within one functional class}
}
\]

Different implementations may be F1, but recurrence of parasite defense does not add O.

## 12. Parasite innovations

The **first** parasite is functionally different from later parasite turnover. Starting from mutual seed-like copying, a mutated string becomes a template that is copied by a replicator without reciprocating. Shortness makes it faster to copy, so it locally outcompetes replicators. This creates a historically new, system-grounded exploitative interaction.

Classification of first parasitism: **F2 — NEW FUNCTIONAL RELATION**, **CLEARLY HERITABLE**, **STRONG COMPARATIVE SUPPORT**. It is a loss of autonomous copying capacity but a gain of a relational strategy: nonreciprocal use of another program's copier. The AFN definition admits new adaptive interactions; it does not require morphological elaboration or acquisition of more instructions.

Later parasite species do not automatically repeat that novelty. The paper says new parasites arise rapidly from mutated replicators and acquire host security features, rather than forming one independently evolving parasite lineage. Unless reaction analysis establishes a new exploitative causal role, these are **F0/F1** variants or **F?**, not new parasite functions.

## 13. Other 2024 innovations

The 2024 paper reports a range of innovative and possibly open-ended behaviors in the same eight histories, and it develops system-specific measures after generic evolutionary-activity measures prove insufficient. Its accessible article-level claims do not establish an additional event, beyond the 2021 reaction classes, that simultaneously has:

- a published temporal location after E3;
- a heritable event identity;
- a distinct causal role; and
- comparative reproductive advantage attributable to that role.

Hypercyclic mutual copying and mutation-process changes remain the strongest additional candidates. They are retained rather than rejected, but the published event alignment is insufficient to upgrade either to a later AFN episode. The 2024 methodological conclusion therefore strengthens the **measurement boundary**, not the AFN count.

## 14. Adaptation evidence

| Candidate | Strongest published adaptive evidence | Classification |
|---|---|---|
| First parasite emergence | One-way templates are copied, shorter parasites are copied faster, and parasites locally outcompete replicators | STRONG COMPARATIVE SUPPORT |
| Faster/shorter replication | Evolved \(t_1\)/\(t_2\) replicators grow faster than the seed in no-mutation comparison trials | STRONG COMPARATIVE SUPPORT, but F0 |
| Toggle-based discrimination | Reaction inspection shows an earlier parasite cannot access copying; the protected but slower strategy later dominates | STRONG COMPARATIVE SUPPORT |
| Additional \(t_5\) checks | Reaction inspection identifies extra required checks; parasite reactions are rare and population high | STRONG COMPARATIVE SUPPORT for defense refinement |
| Defense loss and return | Defense declines when parasite pressure relaxes and returns with renewed parasitism | STRONG COMPARATIVE SUPPORT for environment-contingent selection, not novelty |
| Hypercyclic mutual copying | Mutual dependency and population dominance are reported in some runs | CORRELATIONAL SUPPORT |
| Effective mutation-rate increase | Mechanistic consequence of self-scanning is shown | ADAPTIVE LINK NOT ESTABLISHED for mutation modulation |
| Emergent mutational operators | Mutation cascades generate new viable replicators | ADAPTIVE LINK NOT ESTABLISHED for the operator as selected function |
| Later parasite species | Repeated appearance and ecological participation are shown | CORRELATIONAL SUPPORT; functional-class novelty not established |

No claim borrows adaptation from the overall persistence of a run. The evidence must connect the candidate role to its own differential copying or persistence consequence.

## 15. Heredity evidence

Parasitic exploitation and partner discrimination are encoded in strings that are themselves produced by Stringmol reactions. Parasite and protected-replicator species rise as sequence-defined populations, so their implementations are **CLEARLY HERITABLE** at the resolution needed for selection.

The same conclusion does not automatically extend to every reaction-level effect. Effective mutation rate is transmitted only indirectly through the inherited self-scan execution path. A one-off macromutational cascade can generate a heritable descendant without the variation-generating operator itself becoming a stable hereditary trait. Hypercycle membership is carried by component strings, but a complete lineage ordering for the collective relation is not published for these eight histories.

## 16. Functional-class distinctness

| Event A | Event B | Same causal role? | Same selective problem? | Same implementation family? | Distinct functional class? | Confidence |
|---|---|---|---|---|---|---|
| First parasitism (E1) | Toggle discrimination (E3) | No: exploit another copier vs condition/deny copying | Broadly yes: host–parasite ecology, but opposite causal tasks | No: nonreciprocal template strategy vs partner-executed gate | **YES** | HIGH |
| Toggle discrimination (E3) | Additional checks (E5) | Yes: deny parasites copy-loop access | Yes | Related security/checking family | **NO — SAME FUNCTIONAL CLASS** | HIGH |
| Additional checks (E5) | Defense after renewed parasitism (E6) | Yes: parasite defense | Yes | Implementation partly reorganized | **NO — SAME FUNCTIONAL CLASS** | MEDIUM-HIGH |
| First parasitism (E1) | Later parasite species (E9) | Usually yes: nonreciprocal copying exploitation | Yes | Sequence/implementation varies | **NOT ESTABLISHED AS DISTINCT** | HIGH |
| Toggle discrimination (E3) | Hypercyclic mutual copying (E8) | No if stable mutual dependency is the focal role | Not exactly: defense vs cooperative/dependent reproduction | No | **FUNCTIONAL DISTINCTNESS PLAUSIBLE; AFN EVENT UNRESOLVED** | MEDIUM |
| Toggle discrimination (E3) | Emergent mutational operator (E10) | No: partner discrimination vs variation generation | No | No | **CAUSAL ROLES DISTINCT; ADAPTIVE STATUS UNRESOLVED** | MEDIUM-HIGH |

The first row is the decisive positive comparison. Sharing one ecological setting does not make exploitation and discriminatory defense the same function.

## 17. Eight-run consistency

**Facts.** Eight runs survived to two million timesteps. Across them, population size and species richness generally rise, average reaction times tend to increase late rather than simply optimize downward, parasites recur, and the authors identify several broad defensive strategy families. The 2024 paper reexamines all eight and finds that dedicated Stringmol measures are needed to interpret their innovation. The detailed \(t_1\)–\(t_6\) causal sequence, however, is run 2.

The run-2 order is sufficient to establish a published finite sequence:

\[
\text{seed-like replication}
\rightarrow
\text{parasitic exploitation by }t_1
\rightarrow
\text{partner discrimination by }t_3.
\]

Cross-run recurrence of parasites and defenses strengthens the adaptation claim and shows that the run-2 events are not merely visually chosen patterns. It does not demonstrate multiple functional classes per run. Independent convergence on discrimination is repeated evolution of one function, not functional diversification. Hypercycles and elaborate implementations are unevenly distributed and must not be averaged away, but the publications do not provide a common event ledger for all eight.

## 18. Measurement audit

| Claim | Measurement exposing it | What the measurement establishes | Interpretive dependence |
|---|---|---|---|
| Long-run evolutionary activity | GENERIC ACTIVITY MEASURE | Persistent non-neutral change and candidate epochs | Cannot assign function |
| Population/species/length/reaction-time trends | STRINGMOL-SPECIFIC MEASURE | Changes in abundance, diversity, program size, and execution cost | Function remains underdetermined |
| Parasite frequency and reaction type | STRINGMOL-SPECIFIC MEASURE | Relational copying asymmetry under counterfactual pairing | Requires declared parasite relation, but is mechanistically grounded |
| Toggle gate and extra checks | DIRECT PROGRAM/REACTION INSPECTION | Why particular pairings do or do not reach copying | Low once focal reaction and partners are fixed |
| Adaptive history across \(t_1\)–\(t_6\) | QUALITATIVE HISTORY INTERPRETATION + comparative reaction tests | Ordered strategy replacement and ecological consequence | Moderate; sampled dominant reactions summarize populations |
| Additional unknown functions | No adequate fixed measure | Nothing positive can be inferred | **MEASUREMENT-LIMITED**, not function absent |

The 2024 model-escape argument is a warning about a fixed observer model, not evidence that unmeasured AFN occurred. Common evidence questions remain useful even when the measures and novelty objects are system-specific.

## 19. Strongest positive interpretation

The strongest defensible repeated-AFN sequence is:

\[
F^{(1)}=\text{nonreciprocal parasitic exploitation}
\quad\rightarrow\quad
F^{(2)}=\text{partner-contingent replication discrimination}.
\]

**Event 1** is novel relative to the mutual seed ecology, heritable as a copied parasite sequence, selectively favored because short parasites exploit host copying, and functionally relational rather than merely a new genotype.

**Event 2** occurs later in run 2, is inherited in replicator programs, blocks a previously successful parasite through partner-executed gatekeeping, and is favored despite its replication cost under parasite pressure. Exploitation and discrimination are distinct causal roles.

This satisfies the pass's minimal recurrence test. It does not establish that subsequent innovations continue to cross functional classes, that every surviving run follows the sequence, or that Stringmol has an indefinitely open functional repertoire.

**Attack.** The first parasite can be described as a deletion/loss mutant that passively receives copying, while the second innovation remains within a host–parasite interaction anticipated by the experimental design. That weakens claims of expansive or transformational novelty. It does not defeat the narrower AFN classification used here: the field hallmark explicitly admits new adaptive interactions, and one-way exploitation is a new causally consequential ecological relation relative to mutual replication.

## 20. Strongest skeptical interpretation

The strongest skeptical reading is that all histories remain inside a persistent repertoire of three roles:

\[
\text{copying}
+
\text{copying exploitation}
+
\text{parasite defense}.
\]

Shortening, slowing, self-scanning, toggles, extra checks, parasite counter-checks, defense loss, and defense reacquisition then constitute optimization and implementation turnover in one arms race. Increased mutation and macromutation are variation-process effects, not adaptive functions; later parasite species retain the same exploitative role; hypercycles lack event-level adaptive validation.

This skeptical interpretation correctly blocks counting the many post-\(t_3\) changes as ongoing AFN. It is less adequate for the complete published history because it treats the first emergence of the parasite role as if that relation already existed in the seed ecology. The one-way exploitative relation and the later partner-discrimination relation are historically ordered and causally distinct even though both participate in the same ecology.

## 21. Event evidence matrix

| Event | Novelty | Function | Heredity | Adaptation | F-level | Temporal placement | Distinct from previous AFN? | Final status |
|---|---|---|---|---|---|---|---|---|
| First parasitism (E1) | DIRECTLY SUPPORTED | STRONGLY SUPPORTED | CLEARLY HERITABLE | STRONG COMPARATIVE SUPPORT | F2 | Before/by run-2 \(t_1\) | First AFN event | **AFN SUPPORTED** |
| Shorter/faster replicators (E2) | DIRECTLY SUPPORTED | DIRECTLY SUPPORTED | CLEARLY HERITABLE | STRONG COMPARATIVE SUPPORT | F0 | \(t_2\) | No | Existing-function optimization |
| Toggle discrimination (E3/E4) | DIRECTLY SUPPORTED | DIRECTLY SUPPORTED | CLEARLY HERITABLE | STRONG COMPARATIVE SUPPORT | F2 | \(t_3\), established by \(t_4\) | **YES — distinct from exploitation** | **SECOND AFN SUPPORTED** |
| Additional checks (E5) | DIRECTLY SUPPORTED | DIRECTLY SUPPORTED | CLEARLY HERITABLE | STRONG COMPARATIVE SUPPORT | F1 | \(t_5\) | No | Defense refinement |
| Defense loss/reorganization (E6) | DIRECTLY SUPPORTED | STRONGLY SUPPORTED | CLEARLY HERITABLE | STRONG COMPARATIVE SUPPORT | F0/F1 | \(t_6\) | No | Reversible within-class adaptation |
| Hypercyclic mutual copying (E8) | STRONGLY SUPPORTED | STRONGLY SUPPORTED | PROBABLY HERITABLE | CORRELATIONAL SUPPORT | F2 | TEMPORAL ORDER NOT ESTABLISHED for the eight-run AFN sequence | FUNCTIONAL DISTINCTNESS PLAUSIBLE | Candidate AFN; event/adaptive linkage not established |
| Later parasite species (E9) | DIRECTLY SUPPORTED | PARTIALLY SUPPORTED | CLEARLY HERITABLE | CORRELATIONAL SUPPORT | F0/F1/F? | Recurrent; individual events uncatalogued | NOT ESTABLISHED | Parasite turnover, not repeated class novelty |
| Effective mutation-rate increase (E10) | DIRECTLY SUPPORTED | PARTIALLY SUPPORTED | PROBABLY HERITABLE | ADAPTIVE LINK NOT ESTABLISHED | F0 | Coupled to self-scan | No separate event | Pleiotropic rate change |
| Emergent mutational operators (E7/E10) | DIRECTLY SUPPORTED | STRONGLY SUPPORTED as variation generation | HEREDITY NOT RESOLVED for operator | ADAPTIVE LINK NOT ESTABLISHED | F2 | Lineage to first self-scanner; later event order incomplete | Causal role distinct, AFN unresolved | Evolutionary-process novelty without established adaptation |

Result of the recurrence test:

\[
\boxed{\text{REPEATED ADAPTIVE FUNCTIONAL NOVELTY SUPPORTED}}
\]

This means two supported events, not an indefinitely continuing process.

## 22. Decisive ambiguity

Exactly one ambiguity prevents a stronger classification:

> **The publications do not align any post-discrimination candidate—especially hypercyclic mutual copying or an emergent mutational operator—with its origin time, carrier lineage, and comparative reproductive consequence well enough to establish a third distinct adaptive functional class.**

Thus the boundary is no longer whether Stringmol has two AFN events. It is whether the later portions of the eight histories extend that finite sequence beyond exploitation and discrimination, rather than refining or cycling those roles.

## 23. Resolving-evidence class

\[
\boxed{\textbf{R2 — RESOLVABLE FROM ALREADY DEPOSITED HISTORY DATA WITHOUT NEW SIMULATION}}
\]

The deposited logs and processed reaction/history outputs should in principle permit static event alignment: locate the first persistent hypercyclic or operator-bearing lineages, place them relative to discrimination, reconstruct their focal reactions, and compare their copying/persistence histories with contemporaneous alternatives. That analysis has not been published in the event-indexed form needed here and was not performed in this pass.

R2 does not guarantee a positive result. It identifies where the missing evidence resides. If static histories cannot separate causal role from hitchhiking or pleiotropy, the branch would then require R3 or stop; that escalation is not presumed now.

## 24. Central decision

\[
\boxed{\textbf{A — REPEATED AFN SUPPORTED}}
\]

At least two temporally separated events in the published run-2 history meet the declared test:

1. first emergence of heritable, selectively successful nonreciprocal parasitic exploitation before/by \(t_1\);
2. later emergence and establishment of heritable, selectively favored partner discrimination by \(t_3\)–\(t_4\).

They are distinct functional classes even though they share one host–parasite ecology. The decision does **not** classify later defense refinements as new functions and does **not** establish ongoing AFN or OEE.

## 25. Cross-system-matrix implication

Stringmol should be canonically qualified as the **first repeated-AFN positive case in the reviewed matrix**, at the finite two-event resolution supported by the 2021 history. The historical matrix remains unchanged.

Conceptually, its row changes as follows:

- `Qualitative functional novelty`: from `PARTIALLY SUPPORTED` to **STRONGLY SUPPORTED**;
- `Multiple AFN episodes`: from `PARTIALLY SUPPORTED` to **STRONGLY SUPPORTED for finite recurrence**;
- `Ongoing AFN`: remains **NOT ESTABLISHED**;
- critical missing evidence: a later post-discrimination event with event-aligned heredity, adaptive consequence, and a third distinct functional role.

This does not alter the matrix's broader **B — HETEROGENEOUS BOTTLENECKS** result. Other systems still fail at different N/F/A/O links, and one Stringmol finite recurrence does not identify a common mechanism.

## 26. Next-operation decision

\[
\boxed{\textbf{T2A — STATIC HISTORY RE-ANALYSIS}}
\]

The repeated-AFN result is sufficiently supported for finite recurrence, but not broad enough to justify a targeted OEE mechanism program. The highest-information next step remains validation: determine whether later candidate roles add a third class or whether the histories settle into parasite-defense cycling. This pass does not perform that analysis.

## 27. Highest-information next operation

> **Without rerunning Stringmol, use the already deposited run histories and processed reaction outputs to construct an event-aligned lineage record for the first post-discrimination hypercyclic or mutational-operator candidate, and test whether its carriers exhibit comparative persistence/copying advantage attributable to a causal role distinct from parasitic exploitation and parasite discrimination.**

Exactly one future operation is specified. It is not Q028 and is not conducted here.

## 28. Stop condition

The Stringmol validation branch must stop or return to global hallmark comparison as soon as one of the following occurs in the selected static operation:

1. one post-discrimination event is shown to be heritable, adaptively favored, and functionally distinct, strengthening the case beyond two-event recurrence;
2. all high-priority later candidates reduce to defense/exploitation refinement, loss, reacquisition, hitchhiking, or unselected variation generation;
3. the deposited histories cannot link candidate roles to carrier lineages and comparative reproductive consequences without a new intervention;
4. functional identity remains underdetermined after reactions and selective consequences are fixed.

No mechanism search, model run, implementation, simulation, new experiment, hypothesis, or claim that parasitism causes OEE follows automatically from any outcome.
