# Specification 001 — Prospective Artificial-OEE Exemplar Evidence

Date: 2026-09-10  
Operation: exactly one EX2 evidence-specification pass  
Scope: prospective reporting, evidence preservation, provenance, and validation for artificial-evolution exemplar claims. This is not a community standard, system design, mechanism proposal, experiment implementation plan, candidate search, empirical audit, or hypothesis.

## Decision summary

**Interpretation — central decision: B — OEE-SPECIFIC EVIDENCE INTEGRATION NEEDED.** Generic reproducibility and data-stewardship practices are necessary but do not preserve the history identity, measure semantics, claim scope, endogenous/exogenous distinction, censoring, trivial alternatives, or interpretation-dependent validation needed to audit OEE-relevant exemplar claims. A compact common core plus claim-specific modules is justified.

**Interpretation — specification readiness: READY FOR RETROSPECTIVE COMPATIBILITY AUDIT.** The specification is stable enough to test against the eight frozen EX1 candidate packages, but it is not ready to be called a community standard or imposed as a universal publication requirement.

**Interpretation — exact next operation: EX2A — RETROSPECTIVE COMPATIBILITY AUDIT.** EX2A is selected and not performed.

**Interpretation — scope of effect.** EX2 can directly reduce the evidence/recording gap (E), partially reduce the validation gap (V), and indirectly aid consensus/exemplarization (C). It cannot create the missing phenomenon (P) or the missing same-history conjunction (J).

## 1. Why EX2 was selected

**Fact.** EX1 established **A — COMPONENT EXEMPLAR SET ESTABLISHED, BROAD EXEMPLAR ABSENT**. Evoloops, Stringmol, Aevol, and Geb provide complementary model–measure–interpreted-result packages, while the fixed candidate set contains no full hallmark exemplar and no single defensible global candidate. The dominant bottleneck is heterogeneous, and mechanism readiness remains **NOT READY FOR MECHANISM**. [Evidence Matrix 004](EVIDENCE_MATRIX_004_OEE_CANDIDATE_EXEMPLARS.md)

**Interpretation.** This combination makes prospective evidence preservation more informative than another candidate search or conjunction audit. Existing packages show which distinctions later auditors repeatedly need, while the absence of a broad positive case prevents EX2 from being mistaken for a recipe for producing OEE.

## 2. Exact prospective problem

EX2 asks:

$$
\boxed{
\text{What minimum evidence, provenance, and reporting should a future}
\atop
\text{artificial-evolution study preserve so that an OEE-relevant exemplar claim}
\atop
\text{can later be independently audited without redefining success post hoc?}
}
$$

**Interpretation.** The object is an **evidence specification**. It states what must remain inspectable after a study; it neither prescribes an artificial-life architecture nor proposes how a system should generate any hallmark.

## 3. Prior-art boundary

**Fact — general simulation reporting.** MIASE requires identification and accessibility of models, governing descriptions and parameters, initial/boundary conditions, model modifications, simulation steps and their order, algorithms, environment-sensitive execution information, post-processing, and intended numerical outputs. When source or an open model encoding is unavailable, it permits a sufficiently complete description for reimplementation.[^1]

**Fact — reporting is not validity.** MIASE explicitly defines itself as a reporting guideline rather than a standard operating procedure or account of which experiments are scientifically correct. It does not require a claim that the model matches biological reality or that the experiment ought to have been conducted.[^1]

**Fact — machine-readable experiment descriptions.** SED-ML is an XML-based implementation of MIASE-style simulation descriptions that identifies the model, experimental task, and outputs. It demonstrates feasibility of exchangeable, machine-readable experiment recipes; its systems-biology vocabulary and file format are not universal requirements for artificial evolution.[^2]

**Fact — general data stewardship.** FAIR already supplies domain-independent principles for persistent identifiers, explicit links between data and metadata, accessibility conditions, detailed provenance, qualified relations among digital objects, and machine-actionable reuse. FAIR deliberately precedes particular technical implementations and is not itself a scientific-validity test.[^3]

**Fact — OEE exemplar prior art.** Bedau treats scientific exemplars as concrete problem–solution achievements that organize practice and training, and proposes identifying candidate OEE models and measures, comparing them, and refining them through community work.[^4] The 2024 editorial reports a relative dearth of OEE exemplars, supports behavioral-hallmark and system-specific measurement, and summarizes Tokyo Type 1 as ongoing adaptive novelty plus ongoing complexity growth.[^5]

**Fact — established OEE evidence methods.** Tokyo Type 1 already separates long-term dynamics, indefinite scalability, and qualified empirical extent.[^6] The repository's frozen AFN and complexity methods integrate earlier OEE measures into event-history `N/F/H/A/C` and complexity `X → M → E → (S,I)` evidence records. [Methodology 001](METHODOLOGY_001_AFN_EVENT_HISTORY.md); [Methodology 003](METHODOLOGY_003_COMPLEXITY_SUSTAINEDNESS_SCALABILITY.md)

**Interpretation — boundary result.** EX2 is not a new reporting theory. Its strongest defensible contribution is an **OEE-SPECIFIC INTEGRATION** of established general reporting/provenance practice with established OEE measures and the repository's frozen AFN/complexity evidence structures.

## 4. What generic reproducibility already solves

Generic reproducibility can establish whether another investigator has enough information to reconstruct the intended scientific operation:

- which model or implementation was used;
- which modifications, parameters, initial and boundary conditions applied;
- which procedures and algorithms ran, in which order;
- which environment details materially affect execution;
- how raw numerical outputs were processed; and
- which final numerical outputs were intended.

**Interpretation.** EX2 adopts these MIASE-style obligations rather than renaming them. Model and experiment serialization, packaging format, and vendor-specific infrastructure remain outside the OEE-specific minimum.

## 5. What OEE exemplar claims additionally require

Reconstructing a simulation does not answer whether its output supports an OEE-relevant interpretation. OEE claims additionally require:

1. the exact history or family of histories to which the claim applies;
2. the evolutionary regime and every relevant exogenous intervention;
3. the bearer, object, semantics, non-implications, and confounds of each measure;
4. a trace from preserved evidence through transformations and classification to the claim;
5. claim-appropriate history, continuity, establishment, alternatives, uncertainty, and censoring;
6. explicit separation of observed, extrapolated, and architectural statements;
7. disclosure of run selection, failures, and the intended existence/typicality scope; and
8. validation proportional to interpretive ambiguity.

The layers are therefore:

| Layer | Question | Passing the layer does not establish |
| --- | --- | --- |
| **REPRODUCTION** | Can the intended model and experiment be reconstructed or rerun? | That the measure means what is claimed. |
| **EVIDENCE** | Do retained records support the stated OEE-relevant claim under frozen semantics? | That independent investigators agree. |
| **VALIDATION** | Can others reproduce or audit the computation and interpretation? | Community-canonical exemplar status. |
| **COMMUNITY EXEMPLARIZATION** | Is the package reused, taught, extended, and recognized as exemplary? | Any stronger phenomenon than the evidence supports. |

## 6. Core versus hallmark-specific architecture

The final architecture is:

$$
\boxed{
\text{common audit core}
+
\text{claim-specific evidence module}
+
\text{validation record}
}
$$

**Interpretation — sufficiency test.** This structure survives the cross-substrate requirement because the core names durable scientific relations—model, regime, history, measure, claim, provenance, uncertainty—without assuming cells, genomes, neural networks, or genealogical trees. It also avoids manufacturing exemplar scarcity: a component claim activates only its relevant module, while a broad claim declares its own conjunction.

**Interpretation — module registry.** Only **AFN** and **COMPLEXITY GROWTH** are stabilized here. Transformational novelty, semantic evolution, major transitions, and other hallmarks are marked **MODULE NOT YET STABILIZED**. No criteria for them are invented in EX2.

## 7. Minimal common core

The proposed seven headings compress to five nonredundant records:

| Core record | Required content | Omission would prevent |
| --- | --- | --- |
| **C1 — operation identity** | Model/implementation identity, evolutionary regime, scientifically relevant computational environment | Reconstruction and interpretation of what generated the record |
| **C2 — evidence-unit history** | Run/history identity, temporal/resource range, relationship among histories, interventions, run-selection provenance | Knowing which evolutionary history the claim concerns |
| **C3 — measure and claim trace** | Measured bearer/object, metric semantics, inputs, transformations, classification rule, result, confounds | Auditing the inference rather than only rerunning the system |
| **C4 — inferential scope** | Claim type, discovery/confirmation status, establishment where relevant, alternatives/controls, observed/extrapolated status, uncertainty/censoring, limitations | Preventing post hoc success redefinition and overclaim |
| **C5 — artifacts and validation** | Availability tier, exact identifiers/versions, analysis procedure, reproduction/replication/validation statuses, human/AI provenance | Locating the exact evidence and understanding how independently it was checked |

**Interpretation.** Every common-core field passes the omission test: without it, at least one of interpretation, comparison, reproduction, or auditing materially fails. Detailed substrate metadata belongs in C1 only when scientifically relevant; hallmark-specific histories belong in their modules.

## 8. Model identity

**Required.** Record the model/system name and version, precise implementation or revision, governing rules or algorithms, parameter configuration, initial-condition generation procedure, randomness/seed policy, relevant boundary conditions, and externally imposed limits. A durable semantic description is primary; no serialization format is prescribed.

**Required availability status.** Use one of:

- `SOURCE AVAILABLE`;
- `EXECUTABLE / ARTIFACT AVAILABLE`;
- `FULL ALGORITHMIC DESCRIPTION`; or
- `INSUFFICIENT TO REIMPLEMENT`.

Open source is **recommended**, not a logical condition of exemplar candidacy. MIASE already permits a full description sufficient for reimplementation when open code is unavailable.[^1] `INSUFFICIENT TO REIMPLEMENT` fails the reproduction layer and must be visible; it does not automatically erase every observational claim.

**Computational environment.** Compiler, library, software, architecture, numerical precision, nondeterminism, parallel execution, and hardware-specific behavior are required only when they could materially alter the scientific operation or output. Irrelevant machine inventory is omitted.

## 9. Evolutionary-regime identity

**Required.** Describe the reproduction or continuity mechanism, inheritance, mutation/variation, selection or ecological survival dynamics, population structure, environmental dynamics, resource constraints, and external interventions at the resolution needed to understand the evidence.

**Interpretation.** No predetermined Darwinian form is imposed. The purpose is to identify what evolutionary or system process generated the result and what part of that process was supplied externally.

## 10. Run/history identity

**Required.** Every history supporting a claim receives a unique run/history identifier, seed or initial-condition reference, start/end generation or time, parameter regime, relevant checkpoints, and relationship to replicates.

Each aggregate must declare one of:

- `ONE CONTINUOUS HISTORY`;
- `RELATED REPLICATE HISTORIES`;
- `RESOURCE-SCALED FAMILY`;
- `DISTINCT EXPERIMENTS`; or
- `PLATFORM-WIDE COLLECTION`.

**Hard reporting rule.** Platform-wide results must not be silently represented as one evolutionary history. Different experiments may support a platform repertoire or different component claims; they do not form a recurrence or conjunction sequence without an explicitly defended unit of conjunction.

## 11. Ancestry/causal continuity

An ancestry or causal-continuity record is **conditionally required** when the claim depends on heredity, lineage innovation, establishment, historical origin, or a major transition. It is **optional** for a genuinely population-level statistic whose interpretation does not depend on ancestry.

No tree is universally required. Valid representations include parentage trees, reticulate graphs, horizontal-transfer edges, fusion/contribution relations, collective reconstruction, cultural/ecological transmission, or another defended continuity relation. A future substrate without genealogy must state what causal continuity replaces it; if none is relevant, it must explain why the claim does not depend on heredity or historical descent.

## 12. Event chronology

Where event claims are made, preserve enough resolution to distinguish, when scientifically relevant:

$$
t_{\mathrm{appearance}},\quad
t_{\mathrm{function}},\quad
t_{\mathrm{establishment}},\quad
t_{\mathrm{persistence}},\quad
t_{\mathrm{loss}}.
$$

Intervals, gradual transitions, composite events, and uncertain boundaries are permitted. Exact point times must not be invented from checkpointed data.

## 13. Raw → processed → measure → claim trace

**Required.** Every exemplar-relevant result must support this trace:

$$
\boxed{
\text{raw or deposited record}
\rightarrow
\text{transformation}
\rightarrow
\text{metric or structured judgment}
\rightarrow
\text{classification rule}
\rightarrow
\text{claim}
}
$$

For each link, record inputs, versioned procedure or sufficiently complete description, parameterization, output, and provenance identifier. A figure or table must be traceable back to the deposited evidence used to compute it. This specializes MIASE's post-processing rule to the provenance of an OEE interpretation rather than duplicating generic workflow reporting.[^1]

## 14. Measure semantics

**Required for every measure.** State:

- the bearer and object measured;
- the context and resolution;
- what an increase or change means;
- what it does **not** establish;
- known confounds and failure modes; and
- any observer representation, phenotype encoding, behavior descriptor, clustering, or classification procedure.

Evolutionary activity alone does not establish AFN. Genome length alone does not establish complexity. Visual morphology alone does not establish complexity growth. A metric name or scalar trend never substitutes for its scientific interpretation.

## 15. Exogenous intervention log

**Required.** Preserve a human-readable and, where practical, machine-readable chronological record of researcher or platform interventions that could affect the claim: task/curriculum changes, objective-function changes, direct novelty/complexity/diversity optimization, resource scaling, environmental challenge additions, rule or parameter changes, restarts, manual selection, and data-repair operations.

**Interpretation.** External objectives, curricula, and resource growth are not automatically invalid. They answer different questions from endogenous evolutionary generation. The claim must state which changes arose through evolution/system dynamics and which were supplied externally.

## 16. Discovery versus confirmation

Publications should label whether each decisive result arose through:

1. `EXPLORATORY DISCOVERY`;
2. `CANDIDATE FORMATION`;
3. `CRITERIA FROZEN BEFORE CONFIRMATION`; or
4. `CONFIRMATORY VALIDATION`.

**Required for confirmatory claims.** Before inspecting decisive confirmation evidence, freeze the target phenomenon, metric, context, explanatory resolution, event-inclusion rule, and classification rule where feasible. Exploratory ALife research remains legitimate; it must not be relabeled as preregistered confirmation. Same-data retrospective confirmation is allowed with that limitation stated.

## 17. Triviality / alternative controls

**Required when an obvious claim-threatening alternative exists.** State the strongest plausible trivial explanation and provide at least one system-appropriate discriminating control or analysis. Relevant alternatives include neutral persistence, bloat, raw size, direct optimization of the reported metric, external objective/task expansion, resource-limit release, finite transient novelty, unrelated experiments, and visual complexity.

Null, shadow, randomized, and non-evolutionary baselines are **recommended when they discriminate the live alternative**, not universally required. A shadow is required only when the claim's logic depends on separating adaptive activity from an appropriate neutral expectation; it is not a universal OEE ritual.

## 18. Persistence / establishment

$$
\boxed{
\text{appearance}\neq\text{establishment}.
}
$$

**Conditionally required.** If a novelty, complexity frontier, ecological innovation, or other claim depends on entry into evolutionary history rather than instantaneous occurrence, specify and justify a domain-appropriate establishment criterion. It may use reproduction/descendant contribution, persistence, lineage continuation, adaptive displacement, or repeated attainment. Adaptation is not required for every complexity or structural claim.

## 19. Replication dimensions

Do not compress the following into `reproducible`:

| Dimension | Required report |
| --- | --- |
| **Run replication** | Number and relationship of evolutionary histories; existence versus typicality target |
| **Computational reproduction** | Whether another investigator can rerun/reconstruct the stated experiment |
| **Analytical reproduction** | Whether the same retained inputs and procedure recover the metric/classification |
| **Conceptual robustness** | Whether the interpretation survives predeclared reasonable methodological or resolution choices |

An exceptional history can establish existence if selection is disclosed and evidence is complete. It cannot establish typicality without an appropriate replicate distribution.

## 20. Independent validation

**Conditionally required for a strong hallmark or broad exemplar claim** when the conclusion materially depends on expert causal-role judgment, ontology or resolution choice, ambiguous event boundaries, or other structured interpretation. Independent investigators should receive the same frozen evidence object and record their initial judgments before adjudication.

Independent coding is not mandatory for a direct numerical metric whose object, computation, and inference are unambiguous, although independent analytical reproduction remains recommended. Reliability coefficients are diagnostic; no statistic or universal threshold validates an interpretation.

## 21. Human/AI provenance

**Required when human or AI interpretation materially affects event classification, evidence extraction, functional interpretation, or literature coding.** Record one of:

- `HUMAN ONLY`;
- `AI-ASSISTED RETRIEVAL`;
- `AI-ASSISTED ANALYSIS`;
- `AI PRIMARY CODER`; or
- `MIXED ADJUDICATION`.

Also record analyst/coder role, relevant domain expertise, involvement in criterion development, access to expected outcomes, and—when AI is material—the system/model identity or access date, prompt/protocol version, evidence packet, and whether prior judgments entered context.

**Hard validation rule.** Multiple calls to one model family, shared model priors, or shared context do not constitute demonstrated independent scientific validation. No human/AI category is inherently valid or invalid; the evidential independence and procedure matter.

## 22. AFN module

Activate this module only when a study claims adaptive functional novelty. Preserve the frozen conjunction:

$$
\boxed{N\land F\land H\land A\land C}
$$

for every accepted event:

- **N:** historical novelty at the declared object and resolution;
- **F:** system-grounded causal functional role;
- **H:** lineage or reconstructive heredity sufficient for selection;
- **A:** comparative or causal evidence of adaptive consequence;
- **C:** distinctness from prior accepted functional classes in the same history.

The prospective event ledger records event ID, history/run, temporal interval and boundary, ancestry/continuity, pre/post states, N/F/H/A evidence, prior repertoire, class relations, provenance, and censoring/uncertainty. This is a conceptual record, not a required database.

## 23. AFN class-comparison requirements

For every decisive comparison $C_{K,g}(e_i,e_j)$, preserve:

- context $K$ and explanatory question;
- explanatory resolution $g$ and its justification;
- role A and role B;
- `SAME / DISTINCT / UNRESOLVED`;
- causal justification and missing evidence;
- evidence provenance; and
- robustness status, including `RESOLUTION-SENSITIVE` where admissible resolutions alter the result.

For strong multi-class claims, blinded packets, independent initial judgments, coder provenance, disagreement structure, and adjudication history are **recommended** and become **required** when class identity is substantially interpretive. Krippendorff's $\alpha$ is not mandatory and has no universal pass threshold. [Formalization 001](FORMALIZATION_001_AFN_FUNCTIONAL_CLASS_IDENTITY.md); [Methodology 002](METHODOLOGY_002_AFN_INDEPENDENT_CODING_ROBUSTNESS.md)

## 24. Complexity module

Activate this module only when a study claims complexity growth. First preserve the frozen entry chain:

$$
X\rightarrow M\rightarrow E,
$$

where the bearer/object is declared, the metric has a defensible system-specific complexity meaning, and the observed change is located within evolutionary dynamics with external optimization disclosed.

Then report independently:

$$
\boxed{S=\text{realized temporal sustainedness}}
\qquad
\boxed{I=\text{resource-scalable frontier}}.
$$

Both are not mandatory for every complexity paper. A strong ongoing-complexity exemplar must explicitly state the evidence or absence for both and must use the same defensible complexity object under compatible protocols for a conjunction claim.

## 25. Complexity sustainedness record

Preserve:

- complexity bearer, object, metric, and why the metric tracks complexity;
- what the metric does not imply, including active/expressed versus merely available structure;
- temporal statistic: mean, quantile, maximum, lineage, or established frontier;
- exogenous regime and resource vector;
- observation interval and sampling;
- establishment rule where an extreme/frontier is claimed;
- growth trajectory and record evidence;
- saturation evidence and principal bounded alternatives;
- replicate basis for existence versus typicality; and
- right-censoring, extrapolation tag, and S classification.

No universal time-series model is required.

## 26. Complexity scalability record

Preserve:

- the same complexity object and metric used for the relevant temporal claim;
- scientifically relevant resource dimensions and justified scaling path;
- tested configurations, run protocol, and exposure/computational budget;
- established-frontier statistic;
- observed frontier relation and resource cost;
- known residual hard bounds and co-limitations;
- scaling saturation and principal alternatives;
- observation versus extrapolation tags; and
- I classification.

$$
\boxed{
\text{external resource scaling}\neq\text{within-run growth}.
}
$$

An in-principle extensible architecture is not observed evolutionary scalability.

## 27. Observed versus extrapolated evidence

Every strong claim must use one of:

- `OBSERVED`;
- `MODEL-SUPPORTED EXTRAPOLATION`;
- `ARCHITECTURAL / IN-PRINCIPLE`; or
- `NOT ESTABLISHED`.

Terms such as `unbounded`, `indefinite`, and `ongoing` must include the tested temporal/resource extent and inferential category. A finite positive trajectory may support “no saturation detected within the declared window”; it cannot by itself establish literal infinity.

## 28. Censoring

**Required.** Record applicable forms:

- **temporal right censoring:** the study ended;
- **historical left censoring:** relevant origin may predate retained records;
- **sampling/interval censoring:** events may lie between checkpoints or below resolution; and
- **resource-range censoring:** only finite resource configurations were tested.

Censoring is part of the evidence, not a defect to hide. It qualifies absence and continuation claims without demanding deductive proof of infinity.

## 29. Broad/conjunction claim module

A claim labeled `BROAD ARTIFICIAL-OEE EXEMPLAR` must declare:

1. the OEE conception or type claimed;
2. the hallmarks/components necessary under that conception;
3. the evidence module and result for each claimed component;
4. the unit in which the components coexist;
5. compatibility of their histories, regimes, objects, and protocols; and
6. important OEE properties not established.

For Tokyo Type 1, the declared conjunction is ongoing adaptive novelty plus ongoing complexity growth, and the established Tokyo Type 1 procedure remains governing prior art.[^6] EX2's AFN and complexity records preserve the claim provenance needed to audit that procedure; they do not replace it.

## 30. Same-history / same-platform compatibility

When several experiments support different components, classify their relationship:

- `SAME CONTINUOUS HISTORY`;
- `SAME REGIME / REPLICATE FAMILY`;
- `COMPATIBLE MODEL FAMILY`;
- `RELATED PLATFORM ONLY`; or
- `INCOMPATIBLE FOR CONJUNCTION`.

**Hard reporting rule.** Evidence for novelty in experiment A, complexity in experiment B, and cooperation in experiment C does not establish broad OEE in one evolutionary history. A platform-repertoire claim may intentionally use multiple experiments, but its unit and weaker scope must be explicit.

## 31. Data-retention granularity

The common core requires compact provenance and enough claim-linked history to reproduce the stated analysis. The following are **module-specific**, not universal:

- ancestry/contribution records for hereditary or origin claims;
- event/reproduction logs for event chronology or establishment;
- periodic population or state snapshots for longitudinal reconstruction;
- metric inputs and intermediate aggregates for measure reproduction; and
- environment/intervention history for endogenous/exogenous separation.

**Interpretation.** Retain causally informative raw or intermediate records rather than only final scalars, because future measures may reinterpret the same history. The requirement remains proportional to the claim.

## 32. Storage realism

A three-layer retention policy is sufficient:

| Layer | Status | Content |
| --- | --- | --- |
| **L1 — compact provenance** | **REQUIRED** | Manifest, identifiers, versions, regime, run relations, interventions, measure semantics, claim trace, uncertainty, selection, availability and validation status |
| **L2 — claim-sufficient history/derived data** | **REQUIRED** | The minimum retained histories, inputs, intermediate results, and continuity/event information needed to audit the activated claim module |
| **L3 — high-volume raw state** | **RECOMMENDED when feasible; conditionally required** | Full states or event-complete logs when the claim cannot otherwise be audited; systematic checkpoints/samples are acceptable when justified |

Permissible lossy strategies include periodic checkpoints, compressed lineage summaries, event-indexed snapshots, immutable hashes, and a retained raw subset plus reproducible aggregation procedure. Every lossy choice must state what temporal, ancestry, event, or remeasurement questions can no longer be answered.

## 33. Provenance / immutable identity

**Required conceptually.** Identify exactly which model, data, run, transformation, and analysis produced the claim. Version identifiers are mandatory; content hashes, immutable releases, and persistent archive identifiers are **recommended** because they make identity independently checkable. FAIR already supplies the general persistent-identifier and provenance rationale.[^3]

No blockchain, repository vendor, container system, or particular archive is required. Restricted or proprietary artifacts must state access conditions and preserve enough metadata and algorithmic description for the claimed audit level.

## 34. Failure-friendly reporting

**Required at manifest level when multiple runs exist.** Report total runs, inclusion/exclusion rules, failed or terminated runs, and the identities of selected illustrative histories. Provide claim-relevant negative outcomes—saturation, reversals, no-novelty intervals, and negative scaling levels—when their omission would bias the stated inference.

Publication of every raw run is not required. Aggregate counts and sufficient per-run status metadata may substitute when storage, confidentiality, or access constraints are stated.

## 35. Run-selection / cherry-picking provenance

Every reported exemplar history must be labeled:

- `PRESELECTED`;
- `RANDOM`;
- `BEST-OF-N`;
- `MEDIAN / REPRESENTATIVE BY DECLARED RULE`;
- `CRITERION-SELECTED`; or
- `POST HOC INTERESTING RUN`.

**Interpretation.** Exceptional runs are legitimate existence evidence. Undisclosed best-of-10,000 selection is not legitimate typicality evidence. Selection provenance, not prohibition of rare outcomes, blocks survivor-bias inflation.

## 36. Machine-readability status

**Decision: RECOMMENDED.** Human-readable semantic completeness is required. Machine-readable metadata materially improves cross-study comparison, archival validation, automated trace checking, and future agent-assisted research, as SED-ML and FAIR demonstrate in general settings.[^2][^3]

Machine readability is not required because no substrate-neutral OEE schema has been validated, some old or proprietary studies remain auditable without it, and mandating a premature ontology would overfit current hallmarks. EX2 does not design JSON, YAML, XML, or another schema.

## 37. LLM/platform durability

The specification depends only on durable concepts: model, operation, evolutionary regime, history, intervention, measure, evidence, claim, uncertainty, provenance, and validation. It does not depend on Codex, ChatGPT, an LLM vendor, a repository provider, or a current tool name.

AI-specific details are provenance metadata only when AI materially affects the evidence chain. They are not structural dependencies of the specification.

## 38. Minimum exemplar manifest

The final human-readable form for one published claim is:

```text
Study / claim ID:
Claim type and target conception/hallmark:
Claim unit: continuous history / replicate family / resource family / distinct experiments / platform repertoire

Model / implementation / availability status:
Evolutionary regime and relevant computational environment:
History/run IDs, interval or resource range, and selection rule:
Exogenous interventions and directly optimized objectives:

Measured bearer/object, context, and resolution:
Measure; meaning; non-implications; known confounds:
Deposited evidence -> transformation/analysis -> classification rule -> result:
Discovery/confirmation status and criterion-freeze point:

Main alternative explanation and relevant control:
Establishment/continuity evidence, if claim-dependent:
Observed / extrapolated / architectural status:
Censoring and uncertainty:
Replicate, computational, analytical, and conceptual-robustness status:
Independent-validation and human/AI provenance:

Exact data/code/procedure identifiers and access conditions:
Known limitations and unavailable future analyses:
Activated hallmark module(s):
```

**Interpretation.** This is shorter than the proposed manifest because model/run provenance, raw/analysis/classification trace, and validation fields absorb redundancies. It is a conceptual claim record, not a submission form or software schema.

## 39. Publication artifact package

Ideally accompany a claim with:

1. the manuscript;
2. the model/code or sufficient implementation description;
3. an experiment/run manifest;
4. claim-sufficient history and measure-input data;
5. the analysis procedure;
6. the completed evidence manifest; and
7. stable identifiers, versions, access conditions, and known limitations.

These may be separate artifacts or one coherent research object. No hosting provider, packaging system, programming language, or executable environment is prescribed.

## 40. Required / Recommended / Optional table

| Item | Status | Scope rule |
| --- | --- | --- |
| Model, implementation, regime, parameters, initial/boundary conditions, relevant environment | **REQUIRED** | MIASE-style operation identity; record only environment details that affect the science |
| Code/executable availability category and sufficient algorithmic description | **REQUIRED** | Open source itself is recommended, not logically required |
| Unique run/history identity, interval/range, replicate relationship | **REQUIRED** | Every claim-bearing history |
| Unit of continuity/conjunction and same-history/platform relation | **REQUIRED** | Prevents silent concatenation |
| Intervention/objective/environment-change log | **REQUIRED** | Claim-relevant exogenous changes only |
| Bearer/object, metric semantics, non-implications, confounds, observer representation | **REQUIRED** | Every claim-bearing measure or structured classification |
| Evidence → transformation → metric/judgment → rule → result trace | **REQUIRED** | Every exemplar-relevant claim |
| Discovery/confirmation label and frozen criteria for confirmation | **REQUIRED** | Freeze where feasible; exploration remains allowed |
| Alternative explanation and discriminating control | **CONDITIONALLY REQUIRED** | Required when an obvious trivial alternative threatens the claim |
| Establishment and ancestry/causal continuity | **CONDITIONALLY REQUIRED** | Required when persistence, heredity, lineage, origin, or historical establishment matters |
| Observed/extrapolated/architectural label; uncertainty and censoring | **REQUIRED** | Every finite temporal/resource claim |
| Run-selection and replicate manifest, including failure visibility | **REQUIRED** | Aggregate metadata may replace every raw file |
| Independent interpretive validation | **CONDITIONALLY REQUIRED** | Strong claims with material expert/ontology/boundary judgment |
| Human/AI analytical provenance | **CONDITIONALLY REQUIRED** | Required when interpretation or extraction is materially affected |
| Activated AFN or complexity module | **CONDITIONALLY REQUIRED** | Only for the corresponding hallmark claim |
| Open source, executable artifact, independent rerun, blinded validation packets | **RECOMMENDED** | Strengthens auditability/validation without defining the phenomenon |
| Persistent archive ID, immutable release, content hashes | **RECOMMENDED** | Required semantic identity may be achieved less robustly without them |
| Machine-readable metadata | **RECOMMENDED** | Human-readable completeness remains primary |
| Full high-volume raw states | **RECOMMENDED / CONDITIONAL** | Required only if no smaller record can audit the claim |
| Null/shadow/randomized baseline | **RECOMMENDED / CONDITIONAL** | Required only when it discriminates a live alternative in the claim logic |
| Universal genealogy tree, metric, ontology, reliability threshold, format, container, vendor, or blockchain | **OPTIONAL / NOT PRESCRIBED** | Use only if scientifically useful in the substrate |

## 41. Component-exemplar requirements

A component scientific-exemplar claim requires the common core plus evidence appropriate to that component only. Evoloops-like Darwinian self-reproduction need not report complexity scalability; Outlier-like hierarchical replication need not establish AFN. The claim must identify its narrow solved problem and the boundary it does not cross.

## 42. Hallmark-exemplar requirements

A hallmark-exemplar claim requires:

1. a declared target hallmark;
2. a valid system-specific measurement or structured evidence object;
3. longitudinal/historical evidence when the hallmark is historical;
4. relevant nontriviality controls;
5. uncertainty and censoring;
6. sufficient model/run/analysis provenance; and
7. validation proportional to interpretive ambiguity.

It does not require evidence for every OEE hallmark or community consensus. AFN and complexity activate their frozen modules; unstabilized hallmarks cannot borrow those modules as substitutes.

## 43. Broad-exemplar requirements

A broad artificial-OEE candidate additionally requires an explicit OEE conception, strong evidence across the dimensions necessary to that conception, declared same-system/history compatibility, nontriviality controls, and an explicit list of important properties not established.

No mechanical count of passed fields confers broad status. The scientific interpretation remains open to independent criticism, and the community decides whether the package eventually functions as a shared Kuhnian exemplar.

## 44. What compliance does NOT establish

The following implications are rejected:

$$
\text{reproducible experiment}
\not\Rightarrow
\text{claim-auditable evidence}
\not\Rightarrow
\text{scientifically strong phenomenon}
\not\Rightarrow
\text{Kuhnian exemplar}.
$$

Three nonbureaucratic readiness labels clarify these stages:

| Label | Meaning | Does not mean |
| --- | --- | --- |
| **REPORTING-COMPLETE** | Enough information to reconstruct the intended scientific operation | The measure or claim is valid |
| **CLAIM-AUDITABLE** | Enough claim-linked evidence and semantics to audit the stated inference | The inference is strong or independently validated |
| **EXEMPLAR-CANDIDATE-READY** | The claim is auditable, nontriviality has been addressed, validation is proportionate, and limits are explicit | The phenomenon is OEE, the claim is correct, or the community has canonized it |

**Interpretation.** These are evidence-package states, not a maturity bureaucracy or OEE scale.

## 45. Exemplar-gap dimensions addressed

Using Synthesis 007's decomposition:

| Gap | EX2 effect |
| --- | --- |
| **P — phenomenon** | **CANNOT SOLVE.** Preservation cannot make an absent phenomenon occur. |
| **E — evidence/recording** | **DIRECTLY REDUCES.** Histories, semantics, interventions, selection, and traceability are prospectively retained. |
| **V — validation** | **PARTIALLY REDUCES.** It preserves validation objects and statuses but cannot recruit independent investigators or guarantee agreement. |
| **C — consensus/exemplarization** | **INDIRECT ONLY.** Comparable, teachable packages can support later uptake; EX2 cannot create it. |
| **J — conjunction** | **CANNOT SOLVE.** It prevents false conjunction by concatenation but cannot generate same-history component coexistence. |

## 46. Counterexamples A–L

| Case | Specification result |
| --- | --- |
| **A. Reproducible trivial unbounded counter** | `REPORTING-COMPLETE`, but metric semantics/triviality control fails; not exemplar-candidate-ready. |
| **B. Interesting visual evolution without quantitative/causal measure** | Raw visual evidence may be preserved; claim trace and measure semantics are insufficient for a strong hallmark claim. |
| **C. Strong AFN claim without ancestry** | AFN H and historical continuity cannot be audited; claim not AFN-evidence-complete. |
| **D. Complexity figure without raw/derived provenance** | Metric-to-result trace fails; figure is not claim-auditable. |
| **E. One run selected from 10,000 without disclosure** | Run-selection/replicate manifest fails; neither rarity nor typicality is interpretable. |
| **F. Novelty, complexity, and cooperation from separate platform experiments** | Classified `RELATED PLATFORM ONLY` unless a different unit is defended; broad same-history conjunction rejected. |
| **G. Continuously expanding external curriculum** | Intervention log exposes exogenous challenge growth; result may be valid for scaffolded adaptation but not silently endogenous novelty. |
| **H. Author-only strong functional classes** | Evidence may be claim-auditable, but strong interpretive validation requirement remains unmet. |
| **I. Massive raw deposit without metric meaning** | Data availability passes; measure semantics and claim trace fail. |
| **J. Excellent package for a saturating system** | Can be reporting-complete and claim-auditable; saturation remains the correct scientific result, not an exemplar upgrade. |
| **K. All reporting requirements met but phenomenon is not OEE** | Compliance supports evaluation only; no positive OEE inference follows. |
| **L. Unknown substrate without genealogical trees** | A domain-specific causal-continuity relation is accepted when needed; a tree is not imposed. |

**Interpretation.** All twelve are handled without architecture-specific exemptions. The failures occur at different layers, showing why reporting completeness cannot stand in for evidential validity.

## 47. Prior-art absorption

| Specification component | Classification |
| --- | --- |
| Model/procedure/environment/post-processing/output identity | **EXISTING GENERAL REPORTING PRACTICE** — MIASE/SED-ML |
| Persistent identifiers, provenance, accessible/reusable metadata, machine actionability | **EXISTING GENERAL REPORTING PRACTICE** — FAIR |
| Behavioral hallmarks, Tokyo Type 1 trend/scalability separation, system-specific measures | **ESTABLISHED OEE METHOD** |
| AFN `N/F/H/A/C`, event history, pairwise class records, independent-coding diagnostics | **ESTABLISHED OEE INGREDIENTS + REPOSITORY INTEGRATION**; the integrated workflow is repository-level and conditionally validated |
| Complexity `X → M → E → (S,I)`, establishment, bounded alternatives, resource-path/censoring records | **ESTABLISHED OEE INGREDIENTS + REPOSITORY INTEGRATION**; the S/I workflow is retrospectively validated |
| Five-record common core, manifest, three evidence-package labels, compatibility labels | **NEWLY PROPOSED ORGANIZATIONAL CONVENIENCE** |
| Common-core + claim-module + validation architecture | **REPOSITORY INTEGRATION** |

The strongest absorption equation holds:

$$
\boxed{
\text{EX2}
=
\text{MIASE-style reproducibility}
+
\text{general data/provenance practice}
+
\text{existing OEE measures}
+
\text{frozen AFN/complexity evidence}
}
$$

No component warrants a claim of a new universal scientific standard.

## 48. Strongest positive interpretation

**Interpretation.** Future artificial-evolution studies can preserve a small common evidence core while activating system-specific hallmark records. This makes a later candidate success comparable, teachable, and independently auditable without requiring one universal OEE metric, ontology, genealogy, or all-hallmark super-system. It directly addresses part of the current E gap and creates better validation objects.

## 49. Strongest skeptical interpretation

**Interpretation.** Any checklist can become bureaucratic, reward compliance theater, and overfit today's AFN/complexity language. Core/module separation, conditional requirements, and `REQUIRED / RECOMMENDED / OPTIONAL` levels substantially reduce this risk but do not eliminate it. In particular, the core must remain semantic and minimal, new hallmark modules must be added only after their evidence methods stabilize, and compliance must never confer exemplar status.

The skeptical interpretation does not force option C. A useful global core exists beyond ordinary reproducibility: history unit, claim trace, measure semantics, intervention provenance, inferential scope, selection, and validation status recur across both mature modules and all twelve counterexamples.

## 50. Central decision

$$
\boxed{
\textbf{B — OEE-SPECIFIC EVIDENCE INTEGRATION NEEDED}
}
$$

- **A is not selected:** MIASE/FAIR do not decide what an OEE measure means, which history bears the claim, whether components coexist, or how censoring and interpretation affect the inference.
- **C is not selected:** a small substrate-neutral core survives both AFN and complexity without imposing one hallmark definition.
- **D is not selected:** validation is decisive for interpretive AFN edges but does not dominate missing history, semantics, provenance, selection, or complexity conjunction.
- **E is not selected:** component exemplars and mature AFN/complexity methods already expose stable prospective needs.
- **F is not selected:** conditional modules and three obligation levels prevent most useful fields from becoming universal burdens; the remaining risk is explicitly retained.

## 51. Specification readiness

$$
\boxed{
\textbf{READY FOR RETROSPECTIVE COMPATIBILITY AUDIT}
}
$$

It is stronger than `READY AS REPOSITORY GUIDANCE` because the core, two modules, obligation levels, manifest, and counterexample behavior are explicit enough for a frozen audit. It is weaker than `READY FOR PROSPECTIVE COMMUNITY PILOT` because feasibility, discriminating power, archival burden, and cross-system completeness have not been tested on the eight fixed EX1 packages. It must not be called an OEE standard.

## 52. Known / Underexplored / Potentially Novel / Unknown

| Status | Result |
| --- | --- |
| **ESTABLISHED / KNOWN** | MIASE-style reporting can preserve reproducible simulation operations without establishing scientific correctness; FAIR supplies general persistent-identity/provenance principles; Bedau and the 2024 editorial establish the exemplar-scarcity/community-uptake problem; AFN and complexity have frozen evidence methods. |
| **UNDEREXPLORED — repository scope** | Whether the compact common core is realistic, minimal, and discriminating when applied unchanged to the eight fixed EX1 candidate packages. No field-wide neglect claim is made. |
| **POTENTIALLY NOVEL** | **NONE CLAIMED.** The architecture is an OEE-specific integration and organizational convenience, not a methodological invention or community standard. |
| **UNKNOWN** | Whether studies and archives can supply the fields at acceptable cost; whether independent investigators recover the intended claims; whether community use follows; and whether future hallmarks require new modules or revision of the common core. |

No hypothesis about why OEE occurs follows from this classification.

## 53. Highest-information next operation

**EX2A — RETROSPECTIVE COMPATIBILITY AUDIT.** Apply this frozen specification, without changing its fields, to the eight fixed EX1 candidate packages and classify which evidence would have been available, missing, or impossible to reconstruct.

**Why this operation.** It directly tests realism, minimality, discrimination, architecture neutrality, and storage burden. EX2B is not selected because storage is not yet the demonstrated dominant residual; EX4 is not selected because validation is only one gap; global consolidation is premature before compatibility testing; H2 would leave the new evidence branch untested; and STOP is premature because EX2A can use the frozen corpus without new experiments.

EX2A is selected and not performed here.

## 54. Stop condition

This EX2 pass stops after creating this specification and updating `KNOWN.md`, `FRONTIER.md`, and `STATUS.md`. It performs no EX2A, EX2B, EX3, EX4, H2, transformational-novelty work, candidate search, empirical audit, simulation, architecture design, mechanism research, Q028, or hypothesis formulation.

Prospective evidence work must stop and the boundary must be labeled empirical/external when further progress requires a new positive phenomenon, a same-history hallmark conjunction, new experimental records, system reruns, independent coders, or community uptake. A reporting specification can make evidence auditable; it cannot manufacture OEE or canonize an exemplar.

## Sources

[^1]: Dagmar Waltemath et al. “[Minimum Information About a Simulation Experiment (MIASE)](https://doi.org/10.1371/journal.pcbi.1001122).” *PLOS Computational Biology* 7(4), e1001122 (2011).
[^2]: Dagmar Waltemath, Frank T. Bergmann, Richard Adams, and Nicolas Le Novère. “[Simulation Experiment Description Markup Language (SED-ML): Level 1 Version 1](https://doi.org/10.1038/npre.2011.5846.1).” *Nature Precedings* (2011).
[^3]: Mark D. Wilkinson et al. “[The FAIR Guiding Principles for Scientific Data Management and Stewardship](https://doi.org/10.1038/sdata.2016.18).” *Scientific Data* 3, 160018 (2016).
[^4]: Mark A. Bedau. “[Kuhnian Lessons for the Study of Open-Ended Evolution](https://doi.org/10.1162/artl_a_00428).” *Artificial Life* 30(3), 337–344 (2024).
[^5]: Alastair Channon, Mark A. Bedau, Norman H. Packard, and Tim Taylor. “[Editorial Introduction to the 2024 Special Issue on Open-Ended Evolution](https://doi.org/10.1162/artl_e_00445).” *Artificial Life* 30(3), 300–301 (2024).
[^6]: Alastair Channon. “[A Procedure for Testing for Tokyo Type 1 Open-Ended Evolution](https://doi.org/10.1162/artl_a_00430).” *Artificial Life* 30(3), 345–355 (2024).
