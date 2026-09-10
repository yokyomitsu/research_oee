# DESIGN 001 — Evoloops fixed versus relocating refuge matched experiment design

Date: 2026-09-11. Scope: one prospective experimental-design pass; no implementation, model execution, or experimental data generation.

**Decision: D2 — DESIGN VALID BUT ONE BOUNDED ISSUE REMAINS.** The unresolved issue is a scientifically justified minimum meaningful difference in incumbent-majority residence. The policy contrast, identity, endpoint, horizon, sampling target, extinction safeguards, and conditional inference rules are specified below. No numerical equivalence margin is supported well enough to authorize feasibility sizing. This is not D1 or a completed confirmatory protocol.

Labels: **Fact** denotes inspected primary evidence or existing repository results; **Design decision** denotes a prospective choice; **Interpretation/deduction** denotes its justification or mathematical consequence. Proposed outcomes are not observations or admitted hypotheses.

## 1. Exact scientific question

**Design decision.** Under otherwise matched periodic-disturbance conditions, does relocating the refuge alter finite-horizon persistence of an incumbent genotype-defined species' dominance relative to a fixed refuge?

**Primary inference target: CAUSAL DEPENDENCE / CLOSURE DYNAMICS**, conditional on one ancestor, one world size, one pre-intervention evolutionary history, and a declared distribution of spatial registrations. The causal variable is the **refuge-location policy**. The outcome is persistence of the pre-treatment incumbent's majority, not diversity, any-genotype monopoly, or OEE.

This retains [Synthesis 009](SYNTHESIS_009_ORIGINAL_EMPIRICAL_FRONTIER_SELECTION.md)'s incumbent-residence target. Its phrase “genotype dominance/pseudo-equilibrium” is narrowed operationally here: neither fixed-area stagnation nor pseudo-equilibrium is assumed equivalent to this observable. The Evoloops boundaries in [Synthesis 001, M1](SYNTHESIS_001_Q001_Q012.md), [Synthesis 003](SYNTHESIS_003_Q022_Q027.md), [Synthesis 007](SYNTHESIS_007_GLOBAL_OEE_EXEMPLAR_GAP.md), and [Synthesis 008](SYNTHESIS_008_GLOBAL_OEE_RESEARCH_BOUNDARY.md) remain intact. Historical artifacts and the retrospective archive do not activate further operations.

## 2. Historical antecedent

**Fact — primary-source ledger.** The two journal articles describe different numerical examples; their settings must not be merged.

| Source/status | Verified relevant content | Limit |
|---|---|---|
| Salzberg & Sayama, *Complex Genetic Evolution of Artificial Self-Replicators in Cellular Automata*, Complexity 10(2), 33–39, 2004, **peer-reviewed**; [DOI](https://doi.org/10.1002/cplx.20060), [author manuscript, note 20 and Fig. 4](https://bingdev.binghamton.edu/sayama/papers/Complexity-preprint.pdf) | Cells outside a preserved corner are reset to quiescence. The corner varies to avoid fixed-area stagnation. Fig. 4(c)'s refuge is described as approximately 40% of the space, with 5,000 updates between resets; Fig. 4 uses a periodic 500×500 grid. | The wording does not supply exact mask coordinates or an ordered corner schedule. Stagnation has no frozen genotype-majority threshold. |
| Salzberg, Antony & Sayama, *Evolutionary dynamics of cellular automata-based self-replicators in hostile environments*, BioSystems 78, 119–134, 2004, **peer-reviewed**; [DOI](https://doi.org/10.1016/j.biosystems.2004.07.004), [author manuscript, §§2.2.2, 3.1, 3.3](https://bingdev.binghamton.edu/sayama/papers/BioSystems-preprint.pdf) | Localized removal preserves 285×285 cells on a 750×750 periodic grid at 8,000-update intervals, beginning at 1.5 million updates. A distributed-removal comparison is also reported. The surviving location changes between events. The founder is a specified size-12 loop with a long conserved subsequence. | No exact fixed-versus-relocating control or ordered corner cycle is reported in the inspected methods/results. The manuscript is dated 2005; the journal article is 2004. |
| Salzberg, *Emergent Evolutionary Dynamics of Self-Reproducing Cellular Automata*, 2003, **M.Sc. thesis**; [university-hosted PDF, Chapters 3–6](https://uva.computationalscience.nl/papers/archive/Salzberg2003a.pdf) | Describes deterministic collision-driven variation, birth/structural-death detection, a noninteracting observation layer, genotype-plus-dimensions species identity, and genealogy. Different periodic world sizes can change evolutionary paths. | Documentation does not verify the behavior of an executable available today or its handling of direct reset operations. |

**Design decision.** Use the more explicitly specified localized BioSystems regime as the numerical baseline. The 40%/5,000 example is verified historical context, not the chosen treatment dose. From the selected dimensions, refuge area is 81,225 cells, or 14.44% of the 562,500-cell world. This arithmetic concerns area, not mortality; the article's approximate population-loss rationale cannot be treated as a guaranteed dose.

The [2025 Sayama–Nehaniv review, §4](https://arxiv.org/html/2402.03961v2), published in [Artificial Life](https://doi.org/10.1162/artl_a_00451), retains eventual dominance/pseudo-equilibrium as an open boundary. It does not validate the present endpoint or establish that this comparison has been performed.

## 3. Fixed-refuge regime

**Design decision.** Coordinates are integer pairs `(x,y)` with `0 ≤ x,y < 750`; CA boundaries wrap periodically. Define four 285×285 rectangular masks using intervals `L={0,…,284}` and `H={465,…,749}`:

- NW: `L×L`;
- NE: `H×L`;
- SE: `H×H`;
- SW: `L×H`.

At a reset, retain cell states inside the selected mask exactly, and set every cell outside it to the quiescent state. No translation, rotation, reseeding, repair, or selection of surviving organisms occurs. Apply resets atomically between synchronous CA updates, never during a partial grid update.

In **F**, preserve NW at every reset. “Corner” names locate masks on a displayed fundamental domain of a torus; they do not introduce absorbing world edges. Observation bookkeeping is updated to represent the same physical reset, but may never write back to the CA layer.

## 4. Relocating-refuge regime

**Design decision.** In **R**, preserve masks in the infinite, prospectively fixed sequence `NW → NE → SE → SW → NW → …`, one mask per reset. The rules, cells, and organisms are not rotated with the mask. The cycle is clockwise in the stated coordinate display, including its direction relative to the founder's orientation.

Both arms use NW for their first reset. Their first post-reset trajectory must therefore agree exactly. Policy divergence begins at the second reset, when F retains NW and R retains NE. This supplies a built-in procedural comparison without adding a third scientific regime.

## 5. Relocation-policy choice

| Option | Assessment |
|---|---|
| Exact historical ordered schedule | Not recoverable from the inspected prose. Describing the proposed cycle as an exact historical reproduction would overclaim. |
| Independent random corner choice | Adds avoidable schedule variation, permits repeats, and mixes relocation with variable refuge residence time. Reject. |
| Pre-generated balanced random schedule | Reproducible but introduces order variation unrelated to the first question. Reject for this experiment. |
| Deterministic four-corner cycle | **Select.** Equal visitation counts over complete cycles, no population feedback, one explicit direction, and exact reproducibility. |

**Interpretation.** The effect concerns this particular cyclic relocation policy, not all possible moving refuges. A reverse cycle is not assumed equivalent in a directional replicator system and is not an additional treatment. No schedule parameter may be optimized against observed dominance.

## 6. What remains matched

**Design decision.** Exactly two principal regimes share cell-rule table, synchronous update semantics, periodic boundaries, world dimensions, founder configuration/orientation, pre-intervention state, mask area and shape, reset interval, reset count, first mask, census phase, observation horizon, species semantics, and evidence retention. Neither uses a pathogen, imposed random mutation, novelty objective, genotype-dependent intervention, or replenishment.

Equal instantaneous masks do not equate their cumulative spatial exposure: persistent protection versus periodically changing protection is the intervention itself. Equal reset area also does not equate realized killing, occupied-cell loss, regrowth, collisions, or mutation supply. These differences are recorded and interpreted as potential consequences of the assigned policy, not removed through post-treatment matching.

**Sham decision:** no third regime. In future instrumentation validation, observation-on/off replay and identical-mask replay must preserve CA states. Such engineering checks test noninterference; they are not new experimental arms or evidence for the scientific claim. No checks are executed here.

## 7. Counterfactual pairing

**Design decision.** Each selected pre-intervention world `W_i` branches into exact copies `(F_i,R_i)`, including physical state, observation state, timestamps and ancestry identifiers. No observations from one arm influence the other. The branch histories share their first reset and first regrowth interval. A mismatch before the first differing mask invalidates that pair's execution.

**Fact/limit.** The published CA and collision-generated variation are deterministic. The chosen reset cycle is deterministic too. No externally stochastic biological operation is part of this design. Source-level claims do not establish that a later recovered executable has no random options, asynchronous updates, race conditions, or hidden state. Verifying those is a future feasibility obligation, not accomplished by reading the papers.

**Interpretation.** Both potential outcomes can in principle be observed for each selected world. A within-pair difference therefore identifies a model counterfactual policy effect, assuming implementation fidelity. It does not need to be inferred by comparing unrelated organisms.

## 8. Experimental unit

**Design decision.** The paired world/history is the analysis unit. The population to which the average effect refers is deliberately narrow: **all spatial registrations of one fixed pre-intervention colony world relative to the fixed environmental mask coordinates**.

Let `W*` be the frozen world after the pre-period in §14. Define `W_u` by toroidally translating every physical cell and associated observation record by `u ∈ {0,…,749}²`, leaving the refuge coordinates unchanged. This gives a finite registration population of size `M=562,500`, with equal weights. Uniform spatial registration expresses lack of a privileged founder-to-refuge origin; it does not change genotype, density, world size, or ancestry. Translating both world and masks together would instead be a redundant replay and is excluded as a replication strategy.

Select registrations by a prospectively recorded simple random sample without replacement, independently of their outcomes. Randomness enters this sampling operation only. The selected manifest is then fixed for both deterministic policies. Run count remains unassigned until the meaningful-effect issue is resolved and later feasibility/pilot information supports it.

**Qualification.** These are different initial registrations of one ancestral ecological history, not independent evolutionary origins. The sample has known finite-population sampling dependence, not iid biological histories. Different registrations can yield identical outcomes; retain their stated sampling weights rather than search for “interesting” ones. Exact symmetry-equivalent states may share an execution only if their weights and equivalence are verified; they do not become additional independent evidence through rerunning.

This design separates a policy effect from an accidentally favorable single spatial placement. It does **not** establish robustness to different founder genotypes or independently assembled colony mosaics. The latter would require another experiment. Adding arbitrary noise or extra founders merely to manufacture variance would change this target and is rejected.

## 9. Genotype identity

**Design decision.** Use the historical **birth-defined species** object: the ordered genotype sequence traced from the birth landmark, together with inner-sheath length and width in the parent-arm-relative convention. The complete state sequence is authoritative; G/T/C or hexadecimal forms are reversible labels, not a license to discard spacing or dimensions. Run-local numeric species IDs must map to the same complete identity across arms.

**Fact.** The thesis, §5.3.1, defines species jointly through genotype and phenotype; §4 describes the detection records. A genotype-only pooling could conflate distinct configurations. Spatial orientation and current ecological performance are not newly added species criteria. [Salzberg 2003](https://uva.computationalscience.nl/papers/archive/Salzberg2003a.pdf)

**Interpretation.** “Genotype dominance” here abbreviates dominance of this established genotype–phenotype species class. It is not dominance of a sequence after discarding shape, nor a claim of one ecological role. Counts follow birth identity until structural death; they do not silently reclassify a living loop at arbitrary phases of its circulating sequence. Terminal/transitional recognized loops are retained under the historical structural convention, with reproduction status diagnostic only.

Direct deletion must unregister destroyed structures even if it bypasses the usual dissolver transition. Boundary-damaged but still registered structures require explicit flags and audit states. If damage makes the historical class/living count indeterminate, report it as unresolved measurement and bound its contribution; do not invent a new genotype equivalence or count it as absence. A material inability to retain this identity is a later instrumentation failure, not permission to substitute size or color classes.

## 10. Primary dominance observable

**Design decision.** For recognized living species counts define, where `N(t)>0`,

\[
p_g(t)=N_g(t)/N(t),\qquad D(t)=\max_g p_g(t).
\]

Freeze `g0` as the unique species with `p_g(B−)>1/2` in the common pre-intervention world. If there is no majority, or fewer than two recognized living loops, the predeclared incumbent-persistence experiment lacks its starting target and must stop before policy comparison; do not select a later favorable checkpoint. Translation leaves these counts unchanged.

The primary state indicator is `Z(t)=1` when a living population has `p_g0(t)>1/2`, and `0` when a classifiable living population does not. Zero population is separately coded, as detailed in §21.

`D(t)` is retained diagnostically, not substituted for `p_g0(t)`. Alternating complete monopolies by different species can keep `D(t)=1` while the incumbent loses dominance. Conversely, incumbent return contributes to incumbent residence without establishing continuous dominance. The endpoint makes those limits explicit.

## 11. Persistence definition

**Design decision — one primary statistic.** For `K=1000` post-divergence disturbance cycles, observe each arm immediately before the next reset, after a full interval of regrowth. Define **incumbent-majority census occupancy**:

\[
Y_a(W_i)=\frac1K\sum_{j=1}^{K} Z_a(c_j),\quad a\in\{F,R\}.
\]

Where zero population is confirmed, `Z=0` by a structural bookkeeping convention, accompanied by the separate zero-population record and mandatory inference bounds in §21. Unclassifiable measurements yield bounds rather than a fabricated point value.

The paired effect is `d_i=Y_R(W_i)−Y_F(W_i)`; the primary estimand is the mean `μ` over the declared finite registration population. Negative values mean less incumbent occupancy under relocation.

**Interpretation.** This freezes Synthesis 009's restricted residence concept as a **cycle-end occupancy** statistic, not continuous-time duration. Longest episode is rejected because one exceptional episode can dominate it and it discards repeated incumbent return. Mean `D(t)` changes the target to concentration irrespective of identity. Richness and genealogy remain diagnostics. No composite OEE score is constructed.

## 12. Threshold policy if required

**Design decision.** Primary threshold is **strict majority, `p_g0>1/2`**. Exact half is not dominance: no tie-breaker is needed. Majority has an interpretable population meaning and at most one species can satisfy it.

**Fact/limit.** No canonical fractional dominance threshold was found in the inspected Evoloops methods, thesis definitions, or population-plot captions. Absolute plotting cutoffs are display choices and cannot be imported as dominance criteria.

Freeze two diagnostic sensitivity thresholds, `p_g0>2/3` and `p_g0>0.9`, representing supermajority and near-monopoly. They do not compete to become primary. Report all three, including sign changes or failures of robustness. Sensitivity analyses support narrower threshold-specific interpretation; they cannot rescue a failed primary result or multiply independent tests. These conventions are prospective choices, not historical standards.

## 13. Finite horizon

**Design decision.** Set pre-period `B=1,500,000` updates and reset interval `τ=8,000`. Resets occur after updates `B+jτ` for `j=0,…,1000`. Reset `j=0` is common. Differential-policy cycles are `j=1,…,1000`, and the primary censuses are at `c_j=(B+(j+1)τ)−`, immediately before a next reset would occur.

Stop after the final census at update **9,508,000**, without applying an additional reset. Each arm receives **1,001 resets**, including the common reset, and contributes **1,000 primary cycle-end censuses**. The differential interval is **8,000,000 updates** and contains 250 complete four-corner circuits in R. These numbers define exposure, not independent replication.

**Interpretation.** This prospective horizon is near the historical ten-million-update study scale, expressed as complete relocation circuits; it is not chosen at a visually apparent plateau. It does not reproduce a particular published trajectory exactly. The shared first regrowth census is diagnostic and excluded from the primary sum because policies have not yet diverged. Record both update count and disturbance count. No outcome-dependent extension, early success stopping, or longer-run rescue is allowed.

If a later pilot shows that cycle-end observations predominantly sample unrecovered remnants, the specified regime fails its intended post-regrowth interpretation. That requires an explicit design amendment or rejection, not quietly extending intervals or dropping early cycles.

## 14. Ancestor/initial-condition policy

**Design decision.** Use the BioSystems size-12 founder `GGGGGGGGGGTCCCCCCCCCCTGG/12×12`, with one intact ancestor and its published birth-state configuration, in an otherwise quiescent periodic world. Define +x along its initial reproductive-arm direction and +y clockwise perpendicular to it; retain the original chirality. Place its birth-reference landmark at (375,375) for the canonical pre-period. This fixes the mask cycle relative to the ancestor without treating reflection as an equivalent orientation. Its exact cell configuration must be recovered and verified later, not reconstructed from the sequence in this pass.

**Ancestor classification: USEFUL CALIBRATION.** It is not essential to the abstract dominance question. It is useful because the selected environmental setting already has a documented baseline with that founder. Its engineered conserved subsequence is also a **potential bias for generalization**, conditioning accessible variation and competition. The experiment will say nothing about an unmodified “typical” Evoloop ancestor. Choosing a simpler ancestor now would introduce a second substantive departure from the documented regime; choosing the engineered one does not make its expected diversification a discovery.

The common pre-period allows a colony and endogenous interaction history to establish before clearing; it is not evidence that equilibrium was reached. Generate one canonical `W*` at fixed `B`, then obtain the registration family in §8. There is no pre-treatment search for a particularly stable, diverse, or treatment-responsive world. Failed establishment is recorded and stops this design. Pre-period generation is future work and has not occurred.

## 15. Prior-art exact-match audit

**Fact — bounded search through 2026-09-11.** Inspected the two required journal manuscripts; the 2003 thesis's contents, detection/identity sections, evolutionary experiments and conclusions; the directly related [ALIFE IX conference paper](https://bingdev.binghamton.edu/sayama/papers/alife9-evoloop.pdf); and [ECAL 2003 genealogy paper](https://bingdev.binghamton.edu/sayama/papers/ecal2003.pdf). The latter two are **conference proceedings**, not independent replications of the new contrast. The former develops genetic identification/conserved-sequence experiments; the latter develops graph-based genealogy and includes an environmental example.

Targeted searches used the exact fixed/refuge/safe-area/corner contrast and the thesis title. Within the thesis, relevant searches included `safe`, `stagnation`, `reset`, `removal`, `corner`, `fixed`, and associated experimental sections. The 2005-dated BioSystems manuscript was distinguished from a separate 2005 experiment. A cited “A closer look…” manuscript was not recovered as an independently identifiable direct-comparison report; no unseen result is attributed to it.

**Decision: APPARENTLY UNPERFORMED AFTER BOUNDED SEARCH.** The inspected journal antecedents contain relocation and a rationale for it, but not the direct fixed-versus-relocating genotype-persistence contrast. Thesis and directly linked conference material did not supply that contrast. This is not a universal absence claim; unreported trials or inaccessible material remain possible. A later adequate direct match would invalidate the originality claim rather than justify changing parameters to preserve a project.

## 16. Originality boundary

**Interpretation.** The prospective contribution is **matched comparative evidence on incumbent genotype–phenotype species dominance persistence under fixed versus cyclically relocating refuge policy**, with explicit finite exposure, sampling scope, and extinction accounting.

The operations, biological ideas of refuges/disturbance, and genotype-level Evoloops evolution are prior art. The study is not the first proof that moving refuges prevent closure. It does not merely repeat localized versus distributed clearing or disturbance versus no disturbance. An informative result would concern the previously unverified consequence of refuge persistence, under the new declared endpoint. Originality is provisional until the full protocol survives its remaining gate.

## 17. Positive-result interpretation

**Design decision.** A meaningful reduction requires an uncertainty interval for `μ` wholly below `−δ`, where `δ` is the unresolved meaningful-effect margin in §20, plus the extinction/low-count robustness requirement in §21.

If those conditions are met, the admissible claim is: **within the specified ancestral history, registration population, environmental regime and finite horizon, cyclic relocation reduces incumbent-majority occupancy relative to fixed protection**. This weakens invariance to the policy at that scale.

It does not identify a microscopic pathway, establish ongoing polymorphism, show that every registration benefits, or imply that all genotype dominance disappears. Inspect the effect distribution and diagnostic `D(t)` to distinguish heterogeneous responses and replacement by another monopoly. A reduction confined to immediate deletion is not the intended population-persistence result.

## 18. Null-result interpretation

**Design decision.** A meaningful null requires an interval wholly within `(-δ,+δ)`, not `p>0.05`. It bounds the **registration-average** policy effect under the declared horizon; heterogeneous positive and negative pair effects can cancel, so it does not establish equivalence for every world. Wide intervals, measurement failure, or unresolved extinction effects are inconclusive.

The primary statistical framework is **design-based finite-population inference**. Both deterministic potential outcomes are available at sampled registrations. Sampling uncertainty concerns the unsampled registrations; it is not random genetic evolution, random treatment assignment between unrelated worlds, or independence of time points.

For a fixed simple random sample of `n` registrations, bounded differences `d_i∈[-1,1]` admit a conservative 95% interval `mean(d) ± sqrt(2 log(40)/n)`, intersected with `[-1,1]`. This follows the without-replacement Hoeffding bound, not a normality assumption. A complete census has no registration sampling uncertainty. [Bardenet & Maillard 2015, Proposition 1.2, peer-reviewed Bernoulli reprint](https://arxiv.org/pdf/1309.4029)

This conservative framework shows how a finite null could be interpretable. It does **not** show that sufficient precision is affordable. A tighter validated finite-population bound may be preregistered in a later protocol, but must not be selected after seeing which produces significance/equivalence. No paired t-test or label-swap permutation distribution is assumed automatically valid. Run count and fixed stopping must be frozen before confirmatory outcomes; an interval cannot legitimate repeated optional stopping.

Subject to the safeguards, a null would weaken a substantial **average** contribution of permanent refuge location to incumbent persistence in this regime. It would not refute all explanations of spatial stagnation, assert exact equality, or exclude changes beyond the horizon.

## 19. Reversal interpretation

**Design decision.** An interval wholly above `+δ`, with the same interpretability safeguards, supports increased incumbent-majority occupancy under relocation. It rejects the naive directional expectation that moving protection necessarily disrupts the incumbent. Spatial recolonization, survival filtering, and changed interaction opportunities become diagnostic questions, not automatically confirmed mechanisms.

Greater extinction under R is a different adverse outcome. Reduced incumbent occupancy with `D(t)` remaining high can indicate replacement by another dominant species. Neither outcome is hidden support for ongoing openness. An uncertain or threshold-sensitive sign remains qualified rather than relabeled success.

## 20. Meaningful-effect criterion

**Interpretation — the sole unresolved design gate.** `δ` must mean a scientifically consequential difference in cycle-end incumbent residence, expressed as **m cycle-equivalents over K**, so `δ=m/K`. It must be fixed independently of confirmatory separation, detector convenience, and affordable sample size.

Candidate anchors were attacked:

- One census gives `1/K`; this is measurement granularity, not scientific importance.
- One complete refuge circuit gives `4/K`; it removes dependence on a single corner phase but does not establish that four fewer majority censuses over a thousand-cycle window are consequential. It is an aggregate residence equivalent, not necessarily four consecutive nondominant cycles.
- A conventional five- or ten-percentage-point margin is unsupported here.
- Published population plots establish temporal structure but do not provide a validated distribution of this incumbent-residence statistic or a minimum important difference.
- Pilot variance can determine precision and sample size, not scientific relevance. Inflating the margin until a null becomes attainable would defeat the research objective.

**Decision.** Do not assign a numerical margin. The bounded follow-up must determine one defensible `m` from the meaning of dominance persistence on the declared horizon, using directly relevant historical episode/regrowth timescales or an explicit scientific loss criterion; otherwise reject the promise of an informative confirmatory null. It must not become a parameter sweep, a new literature review, or a simulation pass.

A later separately authorized instrumentation pilot would still need to quantify classification ambiguity under resetting, its contribution to `Y`, regrowth relative to the census phase, and paired sampling variance for planning `n`. Pilot cases must be prospectively separated from confirmatory evidence. Those measurements can show that a scientifically chosen margin is measurable; they cannot choose its importance. Because the current gap is scientific meaning, not merely unknown instrument variance, deferring it automatically to a pilot is not justified. This is why the decision is D2 rather than D1.

## 21. Extinction handling

**Design decision.** Never discard an assigned history because it loses its population. Keep the planned horizon and denominator. At each census, separately record living population, zero recognized population, and unresolved measurement. Zero recognized loops is not automatically irreversible extinction: residual structures can potentially produce a later birth. Continue the prescribed history unless permanent quiescence or another absorbing state is actually established; do not stop merely because the event counter reaches zero.

For the structural statistic, a confirmed zero-population census contributes `Z=0`, but its interpretation is **no living incumbent majority**, not successful coexistence. Record its count separately. Near-extinction diagnostics include the exact minimum population, one-loop censuses, and cases where one individual could change the majority classification. Do not silently import historical figure display cutoffs as viability thresholds.

**Mandatory interpretability bound.** At zero- or one-loop censuses, and at censuses with unresolved identity/counts, temporarily allow the indicator either value `0` or `1`. This yields per-arm bounds `[Y_a^lo,Y_a^hi]` and paired bounds `[d_i^lo,d_i^hi]=[Y_R^lo−Y_F^hi, Y_R^hi−Y_F^lo]`. For two bounded finite-population means, a simultaneous 95% envelope is conservatively `[mean(d^lo)−h, mean(d^hi)+h]`, with `h=sqrt(2 log(80)/n)`, truncated to `[-1,1]`. This uses a union bound on the two endpoint intervals.

These are conservative robustness bounds, **not** imputations of hypothetical evolution after extinction or a second optimized endpoint. A living-population positive, null, or reversal claim must survive this envelope as well as the primary interval. If it does not, report the actual structural endpoint and population-loss/measurement limitation without the stronger claim. This prevents extinction cancellation from manufacturing equivalence and avoids conditioning on survivors. Larger low-population episodes and failure to regrow can still require a restricted interpretation; the bounds do not certify population health.

## 22. Mortality/regrowth diagnostics

**Design decision.** For each reset retain the immediately preceding and immediately following physical states, live-count reconciliation, recognized species counts, and reset mask. Report `N−`, `N+`, and `(N−−N+)/N−` when the denominator is positive. Record occupied-cell loss separately from lost loops. A loop intersecting the cleared region is not assumed dead solely from its centroid; structural destruction must be reconciled with the identity convention. If an immediate count cannot be resolved, record bounds and preserve the relevant state.

Retain births, structural deaths, direct-reset losses, population counts at event times where feasible, and the entire between-reset count trajectory through those events. This distinguishes immediate killing, delayed damage, and regrowth. Parent–offspring identity changes can identify reproductive transitions; they are not automatically a count of all collisions. No new collision classifier is required for the primary claim. Inability to obtain a validated collision count limits pathway discussion rather than invalidating a measured total policy effect.

## 23. Spatial diagnostics

**Design decision.** Minimum spatial evidence comprises initial and pre-branch worlds; before/after-reset states; cycle-end states; mask location; and positions/footprints associated with recorded births and deaths. All records retain species IDs linked to complete identities. Lossless state differences or exact deterministic replay from validated checkpoints may substitute for full repeated arrays only if the same audit states remain reconstructable.

These records support inspection of persistent sanctuary occupancy, recolonization fronts, spatial monopoly/mixing, boundary damage and treatment-induced population loss. No entropy, clustering, or spatial-complexity index is primary. Visual impressions alone cannot establish which process caused an effect. Record enough location history to test whether persistent counts are merely sheltered old individuals rather than their descendants; no elaborate spatial metric is invented here.

## 24. Genealogical diagnostics

**Design decision.** Preserve birth/death times, individual identity where available, species identity, parent references, and multiple contributing parents where the existing method detects them. A lineage is not a species: recurrent production of one species from another must remain distinct from survival of the same individuals.

The original [ECAL 2003 method](https://bingdev.binghamton.edu/sayama/papers/ecal2003.pdf) concerns graph-based genealogy; the thesis documents handling parent contributions and parents that die before offspring completion. **Feasibility must distinguish species-level links from individually resolved ancestry** rather than assume the historical software supplies both at the required fidelity.

Continued lineage coexistence, replacement among species, and recurrent mutation from one lineage are diagnostic alternatives. If only species-level parent links can be retained, the primary abundance comparison may remain possible, but claims distinguishing these individual-lineage histories remain unresolved. No forced single-parent tree, inference of parentage from spatial proximity alone, or claim that genotype richness proves lineage independence is allowed.

## 25. Mediator/confound audit

| Threat or difference | Classification | Treatment in inference |
|---|---|---|
| Different ancestral state, initial density, orientation, observation state, or branch time between paired arms | **PRE-TREATMENT CONFOUND** | Prevent with exact copies; any mismatch is execution failure. |
| Different rule table, wrap behavior, update order or unrecorded external randomness | **FATAL AMBIGUITY** for the assigned contrast | Must be excluded by future model audit; do not attribute such differences to refuge policy. |
| Equal area but unequal actual killing | **CAUSAL MEDIATOR** | Record direct/indirect losses; estimate total policy effect, not a mortality-controlled effect. |
| Changed regrowth geometry | **CAUSAL MEDIATOR** | Diagnose from state/event histories; no post-treatment matching. |
| Changed collision opportunity | **CAUSAL MEDIATOR** | May explain a total effect; no unvalidated collision causal claim. |
| Changed mutation supply through interactions | **CAUSAL MEDIATOR** | Retain birth/genotype transitions and exposure; no normalization that changes the primary estimand. |
| Permanent versus changing protected spatial region | **PART OF THE INTERVENTION** | Intentionally different environmental boundary condition within an unchanged CA world. |
| Population richness, turnover and observed spatial mixing | **DIAGNOSTIC CONSEQUENCE** | Explain observed patterns descriptively; not alternative primary endpoints. |
| Differential extinction or observation loss | **DIAGNOSTIC CONSEQUENCE**, potentially **FATAL AMBIGUITY** for stronger claims | Keep all histories, preserve terminal/uncertain status and apply §21 bounds. |

**Interpretation.** The treatment is sufficiently isolated at policy level, not at a single microscopic pathway. Mortality matching, adjusting for offspring count, or selecting survivors after treatment could remove genuine policy effects or induce selection bias. Covariate analysis cannot restore a failed exact pairing. This corrects any reading of Synthesis 009's “strongest confound” as automatically a pre-treatment confound.

## 26. Pseudoreplication audit

**Design decision.** One pair contributes one `d_i`. Its 1,000 censuses, reset events, loops, births, and genotype observations are within-history measurements, not independent sample size. Rerunning identical states verifies determinism but adds no scientific replicate.

The registration-sampling distribution, not a hypothetical independent-evolution distribution, supports the interval in §18. Shared ancestry and the shared pre-period are explicitly conditioned on. Uniform sampling without replacement is frozen before outcomes; choosing separated-looking or effect-rich registrations afterward invalidates it. A single pair permits a state-specific deterministic contrast only, not the proposed registration-average null.

## 27. Evidence-retention requirements

**Design decision.** Preserve the trace:

`source/rules + founder → common pre-period → W* → registration manifest → exact F/R branches → mask/update history → birth/death/species records → p_g0(t) and diagnostic D(t) → Y and paired effects → uncertainty/extinction bounds → scoped claim`.

Each arrow needs identifiable input/output versions, transformation conventions, and failure flags. Retain all selected registrations, runs attempted, aborted runs, exclusions fixed before treatment, missing measurements and the reason for any lossy retention. Execution ordering must not change world state. Event records must reconcile with population snapshots; a plausible figure is not an audit.

The source and initial-world hashes, complete species dictionary, reset schedule and sampled registration seed/manifest are indispensable. A hash alone is insufficient without the recoverable object. Model data remain separate from observation metadata. No schema, event-detection code, or simulation infrastructure is created in this pass.

## 28. Protocol-freeze boundary

| Item | Status after DESIGN 001 |
|---|---|
| Question, scope, two policies and chosen cycle | **FROZEN CONCEPTUALLY**, including direction and no feedback. |
| World/mask dimensions, interval, common reset, pre-period and horizon | **FROZEN DESIGN CHOICES**; not executed or certified affordable. |
| Founder identity, historical birth-defined species object, majority threshold, primary statistic | **FROZEN**; exact source-state recovery and faithful measurement remain future verification tasks. |
| Initial-condition population and inferential unit | **FROZEN** as uniform spatial registrations of one common history. |
| Positive/null/reversal rules, diagnostics, extinction safeguards and provenance | **FROZEN CONDITIONALLY ON δ**. |
| Minimum meaningful effect `δ=m/K` | **UNRESOLVED SCIENTIFIC GATE**; sole issue blocking the next stage. |
| Confirmatory sample size `n`, chosen registrations, compute/storage budget | **DEFERRED**, dependent on δ and later instrumentation/feasibility information; not permission to choose them from final outcomes. |
| Pilot sample allocation and maximum instrumentation error acceptable relative to δ | **DEFERRED TO A SEPARATELY AUTHORIZED PILOT PROTOCOL**, after the scientific margin exists. |
| Actual source/version, initial configuration file/hash, replay/detection certification | **FUTURE FEASIBILITY EVIDENCE**, not unperformed design choices to be inferred from attractive outcomes. |

No empirical success is asserted. The next bounded design operation succeeds only if it justifies a nontrivial margin and preserves a credible null claim; it fails if the margin can be defended only through convenience, variance, or favorable treatment separation. Later model mismatch, unidentifiable counts, non-regrowing remnants, insufficient precision or unaffordable evidence retention can still stop the program. They are audit conditions, not silently completed passes.

## 29. Destructive objections O1–O10

| Objection | Classification | Resolution or remaining threat |
|---|---|---|
| O1: fixed-area stagnation is not genotype dominance | **RESOLVED WITH QUALIFICATION** | No equivalence is claimed. The experiment measures only incumbent-majority census occupancy. It may leave the historical phrase unexplained. |
| O2: relocation merely changes mortality dose | **RESOLVED WITH QUALIFICATION** | Realized mortality is a possible mediator of the assigned policy. Total effect remains interpretable; a mortality-independent pathway claim is excluded and extinction has explicit safeguards. |
| O3: non-comparable spatial boundary conditions | **RESOLVED WITH QUALIFICATION** | Physical CA boundaries remain identical; protected-location persistence is the intentional treatment. No claim of equal realized environments follows. |
| O4: arbitrary dominance metric | **RESOLVED WITH QUALIFICATION** | Historical species counts, strict majority, fixed census phase and one incumbent-residence endpoint have clear semantics. Numerical meaningfulness of its change remains the specific issue in §20, not a reason to shop for another metric. |
| O5: genotype dominance is not an OEE closure proxy | **RESOLVED WITH QUALIFICATION** | It is a limited population-dynamics target relevant to a component boundary, not a validated surrogate for OEE. |
| O6: finite horizon makes the null uninterpretable | **MATERIAL THREAT** | Finite registration-average equivalence is mathematically possible, but its scientific margin is unresolved. This is the single remaining design blocker. Precision/feasibility must subsequently support that margin. |
| O7: determinism prevents meaningful replication | **RESOLVED WITH QUALIFICATION** | Exact counterfactual pairs and probability sampling over a declared finite registration population support the scoped effect. They do not supply independent evolutionary origins. |
| O8: initial genotype/placement dominates treatment | **RESOLVED WITH QUALIFICATION** | Genotype/history are fixed and conditioned on; placement is sampled with equal weights and matched within pair. No generalization beyond that background is claimed. |
| O9: exact comparison already exists | **RESOLVED WITH QUALIFICATION** | No adequate direct match was found in the bounded primary audit, including the recovered thesis. Originality remains provisional against inaccessible/unreported work. |
| O10: merely reproduces disturbance-induced diversity | **RESOLVED** | Both arms are disturbed; instantaneous geometry/dose schedule match. The endpoint concerns one incumbent, and richness cannot replace it. |

No objection is protected by an OEE label. D2 records incomplete readiness; it is not evidence that the expected sign or scientific payoff will survive.

## 30. What the experiment cannot establish

Even a well-measured effect cannot establish OEE, AFN, indefinite diversity, indefinite complexity growth, a universal anti-closure mechanism, or an explanation of natural evolution. Incumbent replacement can lead to another monopoly; low occupancy can reflect extinction; unchanged average occupancy can conceal opposing effects across registrations. A loop's birth-defined species class is not its ecological function. The experiment isolates an environmental policy, not mortality, regrowth or mutation as a separate cause.

The repository retains finite versus ongoing AFN, `N∧F∧H∧A∧C`, `S≠I`, Aevol `(S2,I0)`, Geb `(S1,I4)`, the absence of a strong same-object S/I conjunction in the reviewed space, and component versus broad exemplar distinctions. Closed Q001–Q027 families are not reactivated.

## 31. Central decision D1–D7

**D2 — DESIGN VALID BUT ONE BOUNDED ISSUE REMAINS.**

**Exact unresolved issue:** What minimum change, expressed in cycle-equivalents of incumbent-majority residence over the fixed 1,000-cycle window, is scientifically meaningful enough to support the proposed equivalence/null inference?

The contrast is causally coherent at policy level and its endpoint is interpretable. A numerical meaningful-effect margin is not justified by the inspected evidence, and cannot be manufactured from sampling variance. Therefore D1 is premature. No adequate direct prior-art answer was found (not D3); the structural endpoint itself survives (not D4); mediator differences do not invalidate the total effect (not D5); a useful finite null is possible in principle but not yet scientifically specified (not D6); no other specific fatal failure is established (not D7).

## 32. Implementation readiness

**IMPLEMENTATION NOT YET JUSTIFIED — DESIGN MARGIN UNRESOLVED.**

The repository is not yet **READY FOR FEASIBILITY AUDIT**, because D2 rather than D1 was selected. Resolving the one scientific issue could permit a later decision to authorize feasibility. No model/source audit, source modification, clone, compile, event-detection implementation or pilot is activated by this artifact.

## 33. Mechanism readiness

**NOT READY FOR MECHANISM.** No original empirical result exists. HYPOTHESES.md remains byte-for-byte unchanged. This is a prospective causal question, not an admitted general mechanism hypothesis.

## 34. Exact next operation

**DESIGN_001A — EVOLOOPS DOMINANCE-RESIDENCE MEANINGFUL-EFFECT MARGIN**

Resolve only the issue in §31, or reject the current promise of a scientifically meaningful null. Do not change the system, endpoint, spatial policy or horizon merely to obtain an easy margin. No feasibility work is part of that next design operation.

## 35. Stop condition

Stop after this artifact, compact current-state/navigation updates, and integrity checks. Do not perform the next design operation, feasibility audit, model implementation, pilot or full experiment. No simulation data, source code, clone, build, commit, or push is authorized by this pass. Historical synthesis/evidence/methodology artifacts, AGENTS.md and HYPOTHESES.md remain untouched.

**Validation record — Fact.** Whitespace checks passed for tracked edits and this new file. All 35 required sections are ordered correctly; local links resolve. There is one ACTIVE frontier and one identical next-operation declaration in each current-state/navigation document and this design. HYPOTHESES.md, AGENTS.md and Synthesis 009 retain their beginning-of-pass SHA-256 hashes. This pass changed only this artifact, STATUS.md, FRONTIER.md, KNOWN.md and README.md; prior working-tree changes were preserved. No simulation code was created or executed, external source repository cloned, experimental data generated, commit created, or push performed.
