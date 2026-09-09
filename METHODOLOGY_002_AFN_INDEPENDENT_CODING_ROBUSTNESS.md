# Methodology 002 — AFN Independent-Coding Robustness

Date: 2026-09-09  
Operation: exactly one M5 methodology/robustness-protocol pass  
Scope: protocol design for pairwise functional-class judgments only; no coding study, empirical re-analysis, event-count revision, mechanism search, simulation, coder recruitment, or hypothesis creation

## Decision summary

The central decision is:

\[
\boxed{\text{B — AFN-SPECIFIC ROBUSTNESS INTEGRATION NEEDED}}
\]

Standard intercoder reliability is necessary but insufficient. It can test whether independent coders applying the same frozen comparison contract reproduce `SAME / DISTINCT / UNRESOLVED`. It cannot by itself tell whether disagreement reflects incomplete evidence, inconsistent application of the contract, or a legitimate change under another scientifically admissible explanatory resolution. M5 therefore adds no new reliability statistic. It integrates established independent-coding practice with AFN's pairwise causal-role object, frozen context and resolution, separate adaptation evidence, explicit unresolved state, and provenance-preserving sensitivity audit.

Robustness-protocol readiness is:

\[
\boxed{\text{READY FOR PILOT}}
\]

The consequence for M3 is:

\[
\boxed{\text{SUPPORTED WITH ROBUSTNESS REQUIREMENT}}
\]

The protocol can now be piloted, but this workspace has no demonstrated scheme-independent, domain-literate validation coders. Repeated calls to one model family or shared agent context would not supply that independence. The highest-information next operation under current resources is therefore:

\[
\boxed{\text{STOP — INDEPENDENCE RESOURCE BOUNDARY}}
\]

An actual M5A pilot becomes licensed only when genuine independent coders are available. It is not performed here.

---

## 1. Why M5 was selected

[Application 001](APPLICATION_001_AFN_EVENT_HISTORY_CROSS_SYSTEM.md) established **B — METHOD VALIDATED WITH FUNCTIONAL-CLASS LIMIT**. One frozen N/F/H/A/C workflow represented Stringmol, Avida, and Geb without a system-specific logical exception, but important class edges still depended on how analysts described causal roles.

[Formalization 001](FORMALIZATION_001_AFN_FUNCTIONAL_CLASS_IDENTITY.md) then established **B — PAIRWISE CAUSAL-ROLE INTEGRATION SUFFICIENT**. The surviving relation is:

\[
C_{K,g}(e_i,e_j)
\in
\{\mathrm{SAME},\mathrm{DISTINCT},\mathrm{UNRESOLVED}\},
\]

under a frozen comparison contract \(D=(K,Q,g)\), with role signatures of the form:

\[
\Phi_D(e)=\bigl(B,P\xrightarrow{E}Y\bigr).
\]

M3 deliberately retained structured expert judgment. Its highest-value residual was whether different sufficiently informed analysts could apply that structure reproducibly without inheriting the developers' tacit assumptions. M5 addresses exactly that residual and does not reopen event reconstruction or any empirical edge.

## 2. Exact robustness problem

M5 asks:

\[
\boxed{
\text{Can functional-class judgments be subjected to an independent-coding and robustness protocol}
\atop
\text{that distinguishes evidence-supported agreement from agreement produced by shared assumptions?}
}
\]

Three instability sources must be diagnosed separately:

| Source | Fixed during comparison | What varies | Scientific meaning |
|---|---|---|---|
| **Evidence instability** | \(K,g\), coder rule | available or interpretable causal evidence | the record does not stably support a role comparison |
| **Analyst instability** | identical evidence packet and identical \(K,g\) | coder application | the protocol, training, or analyst interpretation is not reproducible |
| **Resolution instability** | evidence and coder procedure | scientifically admissible \(g_1,g_2,\ldots\) | function identity is legitimately question- or scale-sensitive |

These are not interchangeable. In particular:

\[
C_{K,g_1}(e_i,e_j)\neq C_{K,g_2}(e_i,e_j)
\]

can coexist with excellent coder agreement at each resolution.

## 3. What independent coding can and cannot establish

**Fact / established methodological boundary.** Intercoder agreement measures whether a specified data-making rule is reproducibly applied by independent observers. Reliability is necessary for a strong reproducibility claim but is not sufficient for validity. [Lombard, Snyder-Duch & Bracken 2002](https://doi.org/10.1111/j.1468-2958.2002.tb00826.x), [Krippendorff 2004](https://doi.org/10.1111/j.1468-2958.2004.tb00738.x)

M5 can establish, conditionally:

- reproducibility of a frozen pairwise coding rule;
- whether rationales reconstruct the same causal roles;
- where the protocol, packet, context, or evidence fails;
- sensitivity to predeclared admissible resolutions; and
- an auditable record of unresolved classification.

M5 cannot establish:

- metaphysically correct or unique functional identity;
- accuracy against an unavailable ground truth;
- latent evolutionary capacity;
- independent empirical replication of an event;
- an OEE mechanism; or
- ongoing AFN.

Unanimously wrong coders can attain perfect agreement. Conversely, resolution-sensitive classifications can be scientifically well behaved.

## 4. Prior art on intercoder reliability

The statistical machinery is established prior art:

| Tool | Appropriate role | Principal limitation here |
|---|---|---|
| Raw percentage agreement | transparent descriptive agreement and input to confusion reporting | ignores chance agreement and can look excellent when `SAME` dominates |
| Cohen's \(\kappa\) | two fixed coders assigning nominal categories | not the general design for more than two coders or missing assignments; depends on coder marginals |
| Fleiss' \(\kappa\) | several raters, nominal categories, conventionally with a fixed number of ratings per unit | less flexible than alpha for missingness and changing coder sets |
| Krippendorff's \(\alpha\) | any number of coders, nominal categories, and incomplete coding matrices | still a reproducibility coefficient, sensitive to sparse samples and category prevalence; not a truth measure |

Cohen introduced chance-corrected agreement for a fixed pair of nominal-scale raters. Fleiss generalized nominal agreement to many raters, allowing the raters assigned to different subjects to differ. [Cohen 1960](https://doi.org/10.1177/001316446002000104), [Fleiss 1971](https://doi.org/10.1037/h0031619)

Hayes and Krippendorff recommend \(\alpha\) as a general coding-data coefficient because it accommodates different numbers of observers, measurement levels, sample sizes, and missing values. Artstein and Poesio likewise show that coefficient choice depends on the coding design and the meaning assigned to chance agreement. [Hayes & Krippendorff 2007](https://doi.org/10.1080/19312450709336664), [Artstein & Poesio 2008](https://doi.org/10.1162/coli.07-034-R2)

Content-analysis standards also require independent coding, separate training/pilot material, full reporting of coding procedures, and preservation of reliability measured before reconciliation. [Lombard, Snyder-Duch & Bracken 2002](https://doi.org/10.1111/j.1468-2958.2002.tb00826.x), [Lacy et al. 2015](https://doi.org/10.1177/1077699015607338)

M5 is therefore not a new reliability method. Its domain-specific content is the AFN coding unit and the separation of analyst, resolution, and evidence diagnoses.

## 5. Coding unit

The M5 coding unit is one already reconstructed, within-history event pair:

\[
u_{ij}=(e_i,e_j;K,Q,g).
\]

The variable is nominal:

\[
C_D(e_i,e_j)\in\{\mathrm{SAME},\mathrm{DISTINCT},\mathrm{UNRESOLVED}\}.
\]

M5 evaluates **coding of predefined units**, not **unitizing**. Content-analysis methodology treats identifying the units and assigning categories to already identified units as different data-making processes with different reliability problems. [Krippendorff 2013, ch. 11](https://www.metodos.work/wp-content/uploads/2020/05/content_analysis-kippendorf-book.pdf)

Accordingly, disagreement about whether an AFN event exists, where it starts, or whether two observations are one composite event is an upstream event-reconstruction issue. It must not be counted as functional-class coder disagreement.

Each candidate event carries one upstream flag:

- `EVENT BOUNDARY STABLE`; or
- `EVENT BOUNDARY UNCERTAIN`.

Pairs with uncertain event identity are excluded from the primary class-reliability coefficient unless every admissible boundary reconstruction preserves the same role evidence. Otherwise they form a separately reported event-reconstruction cohort. M5 does not solve them.

## 6. Evidence-packet design

The prompt's proposed packet contains useful fields but duplicates context and risks leaking analyst conclusions. `Relevant system relations` and `Relevant environmental/ecological context` belong inside \(K\); a precomputed `Known implementation relation` or `Known selective challenge relation` can anchor coders toward an earlier interpretation. Those summary judgments are removed. The underlying mechanistic facts may remain when causally necessary.

The minimal standardized packet is:

```text
Packet ID and version:
Pair-local history ID:
Event-boundary status for A/B:

Declared system/domain:
Necessary system semantics:

Comparison contract
- context K:
- explanatory question/target Q:
- primary explanatory resolution g:
- admissibility basis:

Event A
- history/time relation needed for this comparison
- activity/implementation evidence
- causal-pathway evidence
- provenance pointers

Event B
- history/time relation needed for this comparison
- activity/implementation evidence
- causal-pathway evidence
- provenance pointers

Evidence limitations:
Adaptation-information inclusion exception, if any:
```

The packet does **not** contain:

- a previous `SAME / DISTINCT / UNRESOLVED` judgment;
- a normalized role label supplied by the prior analyst;
- an AFN-supported status;
- previous event counts or system rankings;
- a statement that one outcome is scientifically desired;
- later mechanism hypotheses; or
- citations or summaries unavailable to the other coders.

Adaptation evidence remains in the event's separate AFN-validation record, not in the ordinary class packet. Mask fitness differences, selection coefficients, abundance or sweep trajectories, persistence/dominance summaries, labels such as `beneficial` or `adaptive`, prior A-level judgments, and any statement that an event increased reproductive success. These facts can make a class answer appear consequential without identifying its causal role. Include the smallest necessary fragment only when an adaptive fact is constitutive of the role being compared—for example, when the declared target is a reproductive process and its causal operation cannot otherwise be specified. Every such exception is named in the packet, justified before coding, and supplied identically to all coders. Coders are instructed that included adaptation evidence cannot by itself support `SAME` or `DISTINCT`.

Coders reconstruct `Role A` and `Role B` themselves. All coders receive byte-identical packet versions. In strict validation, external lookup is prohibited. If new evidence is necessary, the packet is centrally revised, versioned, and the affected coding round is restarted; one coder may not privately expand the corpus.

Before coding, a packet-quality assessor who will not classify that pair checks for declared \(K,Q,g\), necessary causal-role evidence, provenance, and boundary status. Failure yields `PACKET INCOMPLETE`, not a forced class code. This gate prevents private evidence reconstruction from masquerading as coder judgment.

## 7. Blinding

The principle is:

\[
\boxed{\text{blind to expected classification, not blind to causal evidence}.}
\]

Coders must not know:

- the repository's prior class edge;
- the previous or expected AFN count;
- the strongest-system ranking;
- which answer would increase the count;
- the desired hallmark-program outcome; or
- downstream mechanism proposals.

System identity, domain semantics, local chronology, and ecological relations remain visible when required to understand the causal role. Artificially removing those facts would test domain ignorance rather than classification reproducibility.

Packets use neutral pair IDs and event labels. Benchmark counts and repository conclusions are released only after initial coding is frozen.

## 8. Coder independence

Two coder roles must be distinguished:

- **Scheme developers:** participated in constructing or revising the AFN functional-class rule, comparison contract, packet template, or calibration cases.
- **Independent validation coders:** did not participate in those target decisions and receive only the frozen protocol, calibration material, and target packets.

Lacy et al. warn that protocol developers have more implicit training and that having all coders participate in protocol development can reduce independence; fresh coders permit developer bias to be evaluated. A semantic-coding study drawing on Krippendorff makes the same point: developers who negotiated a taxonomy can agree because of shared clarification unavailable in the written scheme. [Lacy et al. 2015](https://doi.org/10.1177/1077699015607338), [Montefinese et al. 2017](https://doi.org/10.3758/s13428-016-0838-6)

For a **strong robustness claim**, at least two coders must be independent validation coders, and a design with three or more is preferable when resources allow a meaningful confusion structure. Developer-only agreement may be reported as calibration or exploratory consistency but cannot establish independent reproducibility. This requirement is not imposed on every exploratory study; such studies must use a weaker label.

Independence is compatible with expertise. Every coder must have sufficient domain literacy to interpret the supplied system semantics. A completely domain-naive coder is not a stronger validator. A mixed-expertise panel—domain experts plus methodology-trained, less embedded coders—can reveal tacit assumptions if all satisfy a predeclared literacy check; it is optional, not mandatory machinery.

## 9. Context freeze

Before any target pair is coded, \(K\) is registered and justified by system semantics, experimental setup, ecological relations, or established domain theory. It contains the smallest causal background needed for the comparison, not the entire microhistory.

Coders may not redefine \(K\) after encountering a difficult pair. If the supplied context cannot support the comparison, the response is:

`UNRESOLVED — CONTEXT SPECIFICATION INADEQUATE`.

This is initially classified as D4 and may trigger packet/protocol revision only after the independent round is frozen.

## 10. Resolution freeze

The primary round uses one registered explanatory resolution \(g\). Its record states:

- the explicit explanatory question;
- the system/domain justification;
- the causal distinction represented at that resolution; and
- why that distinction matters scientifically.

Coders may not switch between coarse and fine resolution to reach a preferred class. Trivial extremes such as “all reproductive advantages are one function” or “every opcode trace is a different function” are inadmissible unless an explicit scientific question genuinely requires that level.

No universal resolution taxonomy is introduced.

## 11. Primary coding procedure

The frozen procedure is:

1. A noncoding packet assessor verifies packet completeness and event-boundary status.
2. Coders complete calibration cases that are not part of the target sample.
3. The protocol, primary \(K,Q,g\), coder assignments, packet versions, sampling rule, and reporting statistics are frozen.
4. Assigned target pairs are presented in randomized order within history blocks. Pair-local chronology remains visible where causal interpretation requires it.
5. Each coder independently completes all assigned pairs before seeing any other coder's decision, rationale, confidence, event count, or benchmark.
6. Decisions are time-stamped and frozen. No pre-freeze consultation or consensus meeting is allowed.
7. Raw agreement, nominal \(\alpha\), category prevalence, missingness, and confusion structure are computed on the frozen judgments.
8. Disagreements are diagnosed using §16.
9. Only then may adjudication and the separate resolution-robustness stage occur.

The primary question is identical for every coder:

> Under the declared context \(K\) and explanatory resolution \(g\), do these two events instantiate the same relevant causal functional role?

The response form is:

```text
Classification: SAME / DISTINCT / UNRESOLVED

Role A:
Role B:

Decisive comparison:
<difference or invariance in the causal contribution>

Missing evidence if unresolved:
<specific missing evidence>

Confidence, recorded only after the rationale:
HIGH / MODERATE / LOW
```

“They seem different” and semantic labels alone are invalid rationales. The rationale must identify the relevant invariance or change in \(P\), \(E\), or \(Y\), with the bearer and context made clear.

Qualitative confidence is retained as a low-cost secondary diagnostic. It can identify unanimous but fragile-looking judgments and prioritize adjudication or sensitivity analysis. It does not override the classification, receive numerical weight, enter \(\alpha\), or convert `DISTINCT / LOW` into `UNRESOLVED`.

## 12. UNRESOLVED as a legitimate state

`UNRESOLVED` is a nominal outcome, not a midpoint between `SAME` and `DISTINCT` and not coder failure. It is required when:

- the role cannot be reconstructed from the packet;
- missing causal evidence could change the class;
- the frozen context is inadequate;
- the apparent difference cannot be located above implementation level; or
- two role interpretations remain admissible at the same frozen resolution.

The coder must name the missing evidence or contract defect. An unreasoned `UNRESOLVED` is incomplete coding.

## 13. Intercoder reliability statistics

For a future design with more than two coders, nominal categories, and possible missing judgments, M5 preselects:

\[
\boxed{\text{nominal Krippendorff's }\alpha\text{ as the primary chance-corrected diagnostic}.}
\]

This choice is design-based, not conventionality-based. \(\alpha\) accommodates multiple coders and incomplete coder-by-pair matrices. Cohen's \(\kappa\) may be added for an exactly two-coder complete design; Fleiss' \(\kappa\) may be added when a fixed number of ratings exists for every pair. Neither replaces the preselected primary statistic merely because it produces a more favorable value.

Every report also includes:

- number of pairs and coders;
- coder assignment pattern and missingness;
- category prevalence by coder and pooled;
- raw exact agreement;
- nominal \(\alpha\), with an uncertainty interval when the design supports defensible estimation;
- mandatory pairwise confusion structure; and
- counts and rationales for every disagreement type.

With a very small decisive-pair census, coefficients are explicitly descriptive and may be unstable or undefined. The edge-level record then carries more information than the scalar.

## 14. Why no universal coefficient threshold

Published conventions such as .80 or .67 are reporting heuristics, not scientific truths. Lombard et al. and Krippendorff discuss conventional levels, while later best-practice work acknowledges their partial arbitrariness. [Lombard, Snyder-Duch & Bracken 2002](https://doi.org/10.1111/j.1468-2958.2002.tb00826.x), [Lacy et al. 2015](https://doi.org/10.1177/1077699015607338)

M5 therefore rejects:

\[
\alpha\geq\theta\Rightarrow\text{valid AFN edge}.
\]

The coefficient depends on the unit sample, category distribution, coder design, and amount of information in the data. A high coefficient cannot validate the functional interpretation, and a low coefficient does not reveal whether the cause is evidence, context, resolution misuse, or protocol ambiguity. The protocol predeclares how the coefficient will be reported, but edge acceptance follows the transparent qualitative rule in §24 rather than a universal scalar cutoff.

## 15. Confusion structure

A confusion matrix is mandatory regardless of \(\alpha\):

|              | Coder B SAME | Coder B DISTINCT | Coder B UNRESOLVED |
|---|---:|---:|---:|
| **Coder A SAME** |  |  |  |
| **Coder A DISTINCT** |  |  |  |
| **Coder A UNRESOLVED** |  |  |  |

For more than two coders, report each coder-pair matrix or a clearly defined aggregate over unordered coder pairs; do not hide coder-specific asymmetry in one total.

`SAME ↔ DISTINCT` directly threatens the class edge. `SAME/DISTINCT ↔ UNRESOLVED` instead signals a sufficiency threshold or packet problem until diagnosed. The same coefficient can conceal these different structures.

## 16. Disagreement taxonomy

The proposed D1–D5 taxonomy is useful and sufficient for M5's classification scope, with one refinement to D3:

| Code | Diagnosis | Correct response |
|---|---|---|
| **D1 — ROLE DESCRIPTION DISAGREEMENT** | coders reconstruct different \((B,P,E,Y)\) roles | inspect causal evidence and role-language rules |
| **D2 — RESOLUTION APPLICATION DISAGREEMENT** | roles agree, but coders apply the same frozen \(g\) differently | clarify the resolution rule; do not call this resolution sensitivity |
| **D3a — CORPUS EVIDENCE SUFFICIENCY DISAGREEMENT** | one coder commits and another identifies a genuine evidential gap | preserve `UNRESOLVED`; consider `EVIDENCE-UNRESOLVED` |
| **D3b — PACKET COMPLETENESS DISAGREEMENT** | relevant evidence exists in the fixed corpus but was omitted or unevenly exposed | mark `PACKET INCOMPLETE`; revise/version and restart affected coding |
| **D4 — CONTEXT INTERPRETATION DISAGREEMENT** | coders construe the same \(K\) differently | diagnose inadequate or ambiguous context specification |
| **D5 — PROTOCOL AMBIGUITY** | written rules support multiple readings | revise protocol only after freezing the failed round |

Event-boundary disagreement is recorded separately as `U1 — EVENT RECONSTRUCTION / UNITIZING ISSUE`; it is not a sixth class-coding disagreement.

Persistent disagreement is data. It may show a bad role description, inadequate context, unsuitable resolution, missing evidence, or unstable distinction. The protocol's purpose is diagnosis, not compulsory elimination.

## 17. Adjudication

Adjudication occurs only after initial decisions, rationales, confidence, and reliability outputs are frozen. It may clarify evidence, identify a packet/protocol defect, or produce a consensus edge for downstream use.

The archive preserves:

- every original judgment and rationale;
- coder metadata;
- the frozen reliability analysis;
- the disagreement diagnosis;
- every packet/protocol revision; and
- the adjudicated result and rationale.

Adjudication never retroactively changes the measured independent-coding reliability.

A separate senior, domain-literate adjudicator is preferred for decisive edges because it avoids asking the original coders to erase their own disagreement. A small panel is justified only for unusually consequential or cross-domain cases. If resources permit only the original coders, their post-freeze consensus may be used as a final operational classification with that limitation disclosed. It is not independent validation.

## 18. Training/calibration

Training is required because coders need a shared written rule and sufficient domain literacy. It must not train coders on the decisive target pairs.

Calibration material should include non-target conceptual or historical examples of:

- same mechanism / new function;
- different mechanisms / same function;
- same selective challenge / distinct roles;
- same role / different implementation;
- insufficient evidence; and
- resolution-sensitive classification.

The sequence is: practice, discuss misreadings, revise the protocol, freeze it, then code an unused target sample independently. If target-pair evidence influences a protocol revision, those pairs cannot remain an untouched validation set. Agreement created by rehearsing the target answer is training success, not independent reproducibility.

## 19. Sampling decisive pairs

No fixed sample fraction is justified. Sampling follows claim importance and the structure of the history:

1. census all edges whose `DISTINCT` status creates an accepted AFN event;
2. census all important `UNRESOLVED` edges that could change the historical claim;
3. include all `SAME` edges that define a class representative or prevent double counting;
4. add a probability sample of routine comparison edges when the history is long; and
5. document exclusions and the sampling frame.

The reliability sample must contain the hard distinctions, not merely a random set dominated by routine `SAME` cases. A probability component supports generalization to routine edges; complete coverage of decisive edges supports the actual AFN claim.

### Reference repertoire

For a candidate \(e_k\), the auditable default is exhaustive comparison against every earlier accepted **role-origin event** that could defeat the claim of class novelty. It need not compare against every later implementation token or duplicate observation.

Representative-class comparison is allowed only when:

- the representative was frozen before coding \(e_k\);
- the edges linking it to the other class members are themselves audited;
- the selection rule for the representative is recorded; and
- any transitivity assumption uses one common comparison contract.

This hybrid is the weakest scalable design that does not hide circularity. A representative chosen because it makes a new candidate look distinct is invalid.

## 20. Rare-category / prevalence issue

When most edges are `SAME`, raw agreement can be high while chance-corrected coefficients behave counterintuitively or become unstable. The classic high-agreement/low-kappa problem arises from imbalanced marginal totals; prevalence and coder bias can change \(\kappa\) even when observed agreement is similar. [Feinstein & Cicchetti 1990](https://doi.org/10.1016/0895-4356(90)90158-L), [Byrt, Bishop & Carlin 1993](https://doi.org/10.1016/0895-4356(93)90018-V)

Krippendorff's \(\alpha\) is selected for design flexibility, not immunity to sparse categories. Every report therefore presents prevalence, raw agreement, \(\alpha\), sample size, and confusion structure together. A rare `DISTINCT` edge that defines an AFN event receives complete edge-level review even if it contributes little to an aggregate coefficient.

## 21. Analyst robustness

Analyst robustness asks whether independent coders agree under exactly the same packet and frozen \(K,Q,g\). It is assessed at two levels:

- **Study level:** raw agreement, nominal \(\alpha\), category prevalence, missingness, and confusion structure.
- **Edge level:** unanimity pattern, rationales, confidence distribution, and D1–D5 diagnosis.

No scalar \(R_{\text{analyst}}\) is introduced. The qualitative labels `ANALYST-STABLE` and `ANALYST-SENSITIVE` are conditional summaries of the frozen design, not universal properties of a function.

## 22. Resolution robustness

After primary coding is frozen, selected disputed or claim-decisive pairs enter a separate resolution-sensitivity round. Each alternative \(g_r\) must be registered with:

- its explanatory question;
- domain/system justification;
- causal distinction represented;
- scientific relevance of that distinction; and
- confirmation that it is not chosen to manipulate the event count.

Coders then classify each packet independently under each alternative resolution. Results are:

- `ROBUST SAME`;
- `ROBUST DISTINCT`;
- `RESOLUTION-SENSITIVE`; or
- `EVIDENCE-UNRESOLVED`.

If every coder agrees `SAME` at \(g_1\) and `DISTINCT` at \(g_2\), analyst reproducibility is high and the scientific result is resolution sensitivity. It is not coder failure.

## 23. Evidence robustness

A third numerical robustness axis would make the protocol cumbersome and would partly duplicate packet-quality and D3 diagnoses. M5 therefore retains evidence robustness in a minimal form:

1. **Gate:** `PACKET COMPLETE / PACKET INCOMPLETE` before coding.
2. **Outcome:** `EVIDENCE-UNRESOLVED` when the fixed corpus cannot support a stable class.
3. **Targeted sensitivity:** `EVIDENCE-SENSITIVE` when a decisive edge changes across predeclared, provenance-valid packet versions such as publication summary versus complete supplementary evidence.

A leave-one-evidence-source-out probe is optional for decisive edges supported by several genuinely nonessential, partly independent sources. It can reveal that a conclusion rests on one interpretive statement. It is not required when removal would knowingly delete constitutive causal evidence, and it is not a substitute for independent empirical replication.

Thus the minimal diagnostic structure is two orthogonal robustness dimensions—analyst and resolution—plus an evidence-sufficiency gate and targeted evidence sensitivity. No general \(R_{\text{evidence}}\) score is introduced.

## 24. Robustness classification

The predeclared edge-level rule avoids undefined words such as “predominantly”:

### Primary-round diagnosis

- `ANALYST-STABLE SAME`: all eligible independent validation coders assign `SAME` under the same complete packet and frozen \(K,Q,g\).
- `ANALYST-STABLE DISTINCT`: all assign `DISTINCT` under those conditions.
- `ANALYST-SENSITIVE`: at least one eligible coder assigns `SAME` and another assigns `DISTINCT`, or a D1/D2/D4/D5 disagreement remains after diagnosis.
- `EVIDENCE-SUFFICIENCY DISPUTED`: no `SAME ↔ DISTINCT` split exists, but at least one coder commits while another selects `UNRESOLVED`; this is a provisional D3 status pending packet audit.
- `EVIDENCE-UNRESOLVED`: all coders select `UNRESOLVED`, or post-freeze diagnosis confirms that missing corpus evidence prevents a stable judgment.
- `PACKET INCOMPLETE`: the supplied validation object is defective; the pair is excluded from the reliability calculation for that version and must be recoded from a new frozen packet.

Unanimity here is a conservative operational condition for an edge-level “stable” label, not a truth criterion and not a substitute for the study-level statistics. A study may report useful reproducibility even when some individual edges remain sensitive.

### Final robustness status after resolution audit

- `ROBUST SAME`: `ANALYST-STABLE SAME` at the primary resolution and every registered admissible alternative tested.
- `ROBUST DISTINCT`: `ANALYST-STABLE DISTINCT` at the primary resolution and every registered admissible alternative tested.
- `RESOLUTION-SENSITIVE`: at least two admissible resolutions yield different analyst-stable committed classifications.
- `ANALYST-SENSITIVE`: classification varies across coders under the same packet and same \(K,g\).
- `EVIDENCE-UNRESOLVED`: evidence does not support a stable classification after the contract is fixed.

Confidence remains a separate annotation. Adjudication may create an operational consensus edge, but it does not upgrade an analyst-sensitive original result to independently robust.

The two-axis interpretation remains useful if kept qualitative:

| Analyst robustness | Resolution robustness | Interpretation |
|---|---|---|
| stable | stable | strongly reproducible classification within the audited evidence |
| stable | sensitive | scientifically resolution-sensitive |
| sensitive | stable resolutions tested | analyst/protocol ambiguity |
| sensitive | sensitive | unstable classification; do not derive a strong class edge |

## 25. Event-graph uncertainty

The AFN event graph naturally preserves uncertainty:

- event nodes retain reconstruction and boundary status;
- pairwise edges retain `SAME / DISTINCT / UNRESOLVED`;
- each edge carries packet version, \(K,Q,g\), analyst status, resolution status, evidence status, and adjudication provenance.

The graph should not be forced into one partition when edges are unresolved or use different contracts. No probabilistic graph is needed.

If a scalar summary is required, publish at most a predeclared strict count derived only from accepted events whose decisive distinctness edges meet the study's explicit robustness standard:

\[
n_{\mathrm{AFN}}^{\mathrm{strict}}.
\]

Do not publish an “including unresolved” count as though unresolved candidates were partial positives. Publish the graph and candidate list instead. M5 sets no universal acceptance threshold and revises no existing count.

## 26. Cross-system applicability

The same people need not code every system. Each system should use independent, sufficiently domain-literate coders under the common meta-protocol:

\[
\boxed{\text{cross-system comparability comes from procedure, not identical coders or a global function ontology}.}
\]

Primary coding remains within one continuous history. Cross-system pairs such as Stringmol exploitation versus Geb fleeing are unnecessary for AFN counts and are not part of the protocol.

Independent coding is also distinct from independent empirical replication. Coders can reproducibly classify one published event that has never been independently reproduced; multiple experimental runs can reproduce an event while analysts disagree about its functional class. Both dimensions should be reported separately.

## 27. Human / AI assistance provenance

Record for each coder only attributes relevant to methodological provenance:

- domain expertise and literacy check;
- involvement in AFN scheme development;
- access to prior AFN conclusions or target counts;
- human/AI assistance category; and
- any conflict such as authorship of the underlying event study.

AI-assistance categories are:

- `HUMAN ONLY`;
- `HUMAN WITH AI INFORMATION RETRIEVAL`;
- `HUMAN WITH AI DRAFTING`;
- `AI CODER`; and
- `MIXED`.

For AI involvement, report model/provider, version or access date, prompt/protocol version, evidence packet, retrieval access, stochastic settings when available, and whether earlier judgments entered context.

The boundary is mandatory:

\[
\boxed{
\text{multiple outputs from the same model family or shared context}
\neq
\text{demonstrated independent scientific coding}.
}
\]

Repeated stochastic calls share training history, model priors, protocol language, and often conversation context. They may be useful for protocol debugging, sensitivity exploration, or drafting. They must not be presented as statistically independent validation coders. Multiple human coders who all see the same AI-generated recommendation can likewise lose informational independence.

Heterogeneous human/AI panels are a future methodological option, not a validated substitute for scheme-independent human coding and not an M5 result.

## 28. Counterexamples A–J

| Case | Diagnosis under M5 |
|---|---|
| **A — all agree because trained on target cases** | training contamination; agreement does not count as independent validation; recode an untouched sample |
| **B — coarse agreement, fine disagreement** | first determine whether coders disagree at the same fine \(g\); if each \(g\) is internally stable but outcomes differ, `RESOLUTION-SENSITIVE` |
| **C — omitted same-role fact** | `PACKET INCOMPLETE` / D3b; freeze failure, revise packet for all, restart; prior agreement remains archived |
| **D — DISTINCT versus UNRESOLVED only** | D3 evidence-sufficiency disagreement, not direct class opposition; diagnose the specified missing evidence |
| **E — SAME versus DISTINCT despite identical role descriptions** | D2 resolution-application disagreement or D5 rule ambiguity |
| **F — rare DISTINCT misleads statistic** | report prevalence, raw agreement, \(alpha\), and confusion; inspect every AFN-defining edge |
| **G — domain-naive coder misreads semantics** | failed literacy/qualification condition; report coder type and do not treat ignorance as independence |
| **H — experts share weak disciplinary convention** | high social reproducibility but validity unresolved; seek external domain justification or mixed-expertise sensitivity, not a higher coefficient |
| **I — consensus erases disagreement** | archive violation; recover or rerun independent judgments; consensus cannot replace frozen reliability |
| **J — repeated LLM calls agree from common priors** | useful debugging evidence only; no claim of independent-coder validation |

The protocol distinguishes every case without changing the coding categories.

## 29. Strongest prior-art absorption test

The strongest absorption is:

\[
\boxed{\text{M5}=\text{ordinary intercoder reliability applied to AFN functional classes}.}
\]

This is correct for the statistical core. Independent coders, codebook training, frozen judgments, raw agreement, chance-corrected coefficients, prevalence reporting, and adjudication are established content-analysis practice.

The absorption is incomplete only at the integration boundary. AFN requires the coding unit to be a within-history causal-role edge, the comparison contract \((K,Q,g)\) to be frozen, adaptation evidence to remain separate, `UNRESOLVED` to remain substantive, resolution sensitivity to be tested outside intercoder disagreement, and event-graph provenance to preserve uncertainty. These are application constraints, not a new coefficient.

## 30. Strongest positive interpretation

The strongest defensible success is:

\[
\boxed{
\text{functional-class judgment can remain structured expert judgment}
\atop
\text{yet become independently reproducible and sensitivity-audited}.
}
\]

No algorithmic or universal function ontology is required. A strong result is an edge that fresh, domain-literate coders reproduce from a complete blinded packet and that remains stable across the registered admissible resolutions relevant to the scientific question.

## 31. Strongest skeptical interpretation

Independent coding validates social reproducibility under a supplied evidence representation, not functional truth. Coders can share a disciplinary convention, a misleading packet, or an oversimplified but easy-to-apply causal vocabulary. Blinding cannot remove background theory, and the admissible-resolution registry still requires expert judgment.

This skeptical interpretation is correct. M5 narrows the warrant to reproducibility, protocol clarity, sensitivity, and explicit uncertainty. It does not turn agreement into ontology or empirical replication.

## 32. Central decision

\[
\boxed{\textbf{B — AFN-SPECIFIC ROBUSTNESS INTEGRATION NEEDED}}
\]

- **Not A:** ordinary reliability supplies the statistics but does not separate analyst disagreement from admissible resolution change or packet insufficiency.
- **Not C:** resolution choice remains important, but analyst reproducibility has not yet been measured and cannot be treated as straightforward.
- **Not D:** sparse decisive edges make scalar interpretation weak, but confusion matrices, prevalence, and nominal \(\alpha\) still provide useful study-level diagnostics alongside rationales.
- **Not E:** M3's frozen contract and three-valued relation remain testable; interpretiveness alone does not show inevitable failure.
- **Not F:** the coding unit and packet schema are stable enough for a pilot, while packet incompleteness is explicitly gated rather than assumed away.

The decision is B despite strong prior-art absorption because the added value lies in disciplined separation of three instability sources, not in statistical novelty.

## 33. Robustness-protocol readiness

\[
\boxed{\textbf{READY FOR PILOT}}
\]

The packet, blinding rules, coder roles, coding form, ordering, sampling, statistics, disagreement taxonomy, adjudication archive, and resolution round are specified sufficiently to test on a small frozen set. The protocol is not yet `READY FOR RETROSPECTIVE VALIDATION` as an empirically demonstrated procedure because no genuinely independent coder has used it. It is not `READY FOR PROSPECTIVE USE` because no pilot, workflow burden assessment, or prospective packet-generation study exists.

## 34. Consequence for M3

\[
\boxed{\textbf{SUPPORTED WITH ROBUSTNESS REQUIREMENT}}
\]

M5 does not weaken the M3 causal-role rule. It confirms that the rule is the appropriate coding object and adds a requirement for strong retrospective claims: decisive edges should be coded by scheme-independent, domain-literate validators from identical blinded packets, with analyst and resolution robustness reported separately.

The historical M3 artifact and all prior edge judgments remain unchanged.

## 35. Known / Underexplored / Potentially Novel / Unknown

### Known / established

- Independent coding assesses reproducibility of a coding procedure, not truth.
- Scheme developers can share tacit training that fresh coders do not; developer-only agreement is a weaker robustness test.
- Nominal Krippendorff's \(\alpha\) is suitable for multiple coders and missing judgments, while raw agreement and confusion structure remain necessary diagnostics.
- Category prevalence can make one scalar misleading, especially with rare `DISTINCT` outcomes.
- Coding predefined pairs and reconstructing event boundaries are distinct reliability problems.
- Reconciliation after coding cannot replace the reliability measured from frozen independent judgments.

### Underexplored

- Empirical inter-analyst reproducibility of AFN causal-role edges.
- Whether independent coders converge on the same role signatures without developer explanation.
- How often scientifically admissible resolution changes alter AFN edges.
- Whether mixed-expertise panels expose tacit domain assumptions without increasing semantic error.

### Potentially novel

- **Not assigned.** The protocol is an AFN-specific integration of established reliability, blinding, provenance, and sensitivity practices. No new statistic, threshold, or general reliability theory is claimed.

### Unknown

- The actual reliability of any existing repository judgment.
- Whether decisive AFN edges are analyst-stable, resolution-stable, or evidence-sensitive.
- The coder burden and packet-revision rate in a real pilot.
- Whether independent validation would support, weaken, or leave unresolved any current class edge.

## 36. Highest-information next operation

Exactly one operation is selected:

\[
\boxed{\textbf{STOP — INDEPENDENCE RESOURCE BOUNDARY}}
\]

The protocol is ready for a pilot, but the current workspace supplies no demonstrated independent validation coders and this pass is not authorized to recruit them. Repeated agent or model calls would create fake independence. Therefore M5A is not performed or simulated.

If a future research context supplies at least two scheme-independent, domain-literate coders who can receive blinded frozen packets, the next licensed active operation would be M5A on a small set containing all decisive edges and appropriate same/unresolved controls. That conditional future operation is not selected or performed here.

## 37. Stop condition

M5 stops after creating this protocol and updating the canonical repository state. It performs no Stringmol, Avida, Geb, or other empirical coding; calculates no intercoder coefficient; changes no AFN event or count; recruits no coder; makes no repeated-LLM independence claim; conducts no M5A, M4, M2, Q028, mechanism search, simulation, or hypothesis creation.

The permitted result is methodological:

\[
\boxed{
\text{structured expert functional judgment}
\rightarrow
\text{genuinely independent coding}
\rightarrow
\text{separate analyst disagreement from resolution dependence}
}
\]

without treating agreement as functional truth.
