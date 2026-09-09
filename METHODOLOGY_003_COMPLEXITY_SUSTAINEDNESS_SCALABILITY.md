# Methodology 003 — Complexity Sustainedness and Scalability

Date: 2026-09-09  
Operation: exactly one CG3 methodology/formalization pass  
Scope: evidence warranted by finite histories and finite resource-scaling experiments; no Q028, mechanism search, hypothesis creation, system execution, raw-data reanalysis, or retrospective method application

## Decision summary

The central methodology decision is:

\[
\boxed{\textbf{B — INTEGRATION GAP}}
\]

Tokyo Type 1 analysis, long-term evolutionary-dynamics classification, MODES, and Geb already supply the principal ingredients. What was missing was one explicit evidence workflow that keeps the following claims separate:

\[
\boxed{
\text{realized temporal growth}
\neq
\text{no saturation detected within a finite window}
\neq
\text{resource-scalable attained frontier}.
}
\]

The methodology is:

\[
\boxed{\textbf{READY FOR RETROSPECTIVE USE}}
\]

Its output is an ordered pair of categorical records, \((S,I)\), not a numerical OEE score. It supports graded operational claims from finite evidence; it never proves infinite growth. The exact next operation is **CG3A — RETROSPECTIVE METHOD APPLICATION**, selected in §42 and not performed here.

## 1. Why CG3 was selected

**Fact.** [Evidence Matrix 002](EVIDENCE_MATRIX_002_COMPLEXITY_GROWTH.md) found that Avida supplies the strongest reviewed time-resolved realized complexity-growth evidence, while Geb supplies the strongest reviewed resource-scalability evidence. No reviewed system closes both evidence chains, and higher-order complexity growth is not established.[^1][^2]

**Interpretation.** The highest-information gap is therefore not another complexity metric or positive-case search. It is the evidential relation between finite temporal growth, saturation, and a frontier evaluated across resource configurations. CG3 freezes E1's object and metric judgments and formalizes only that relation.

AFN remains **PAUSED — EXTERNAL INDEPENDENT VALIDATION REQUIRED**. Its postponed event-ongoingness analysis is not imported: complexity supplies a measured process, potentially dense time series, and resource-scaling axis that the sparse AFN event record did not.

## 2. Exact methodological problem

The question is:

\[
\boxed{
\text{What evidence can a finite artificial-evolution experiment legitimately provide for}
\atop
\text{sustained complexity growth, indefinite scalability, and higher-order complexity growth?}
}
\]

Every experiment is finite in time and resources. The method must nevertheless distinguish direct observation from warranted finite-range inference and from claims made only about an architecture. It must also remain usable with system-specific complexity measures.

## 3. Prior-art boundary

**Fact.** Channon's Tokyo Type 1 procedure already orders five analyses: evolutionary activity, component-normalized activity, long-term dynamics classification, indefinite scalability in diversity and complexity, and the order of indefinite scalability.[^3][^4] It explicitly recommends qualifying empirical scalability by the time and physical-limit range over which it has been demonstrated. Ackley and Small's underlying architectural concept concerns open-ended computational growth without substantial reengineering; it does not by itself demonstrate an evolved complexity frontier.[^13]

**Fact.** Bedau, Snyder, and Packard classify long-term evolutionary dynamics from diversity, new activity, and cumulative activity, initially at the level of one run and more generically only when runs and parameter regions agree.[^5] MODES supplies system-portable hallmark measures, a persistence filter, and the recommendation to compare plausible bounded and unbounded models instead of visually declaring a plateau.[^6]

**Fact.** Geb operationalizes indefinite scalability as a sequence of higher evolved maxima when two co-limiting resource bounds are increased together; scaling either alone yields an asymptote over the tested range.[^7] Hintze demonstrates why a formally extensible, increasing compression proxy cannot pass unless complexity validity has already been defended.[^8]

**Interpretation.** CG3 is not a replacement for these methods. Its contribution is an explicit joined audit trail for two independent evidence records, their censoring, their regime and scaling-path contracts, and the transitions among observed, model-supported, and in-principle claims.

## 4. Frozen complexity-validity assumptions

CG3 begins only after E1's first three links have passed at a declared level:

\[
X\rightarrow M\rightarrow E.
\]

- **X:** the complexity bearer and object are declared.
- **M:** the metric has a system-specific scientific interpretation and survives the bloat, inactive-capacity, and arbitrary-accumulation controls.
- **E:** the measured change is located within evolutionary dynamics, with external optimization and designer interventions disclosed.

CG3 does not compare complexity magnitudes across unlike metrics and does not reopen a universal definition of complexity. If **M** fails, as in the Hintze control, no temporal or scaling category can rescue the hallmark claim.

## 5. Realized temporal complexity

Use the simplest adequate notation:

\[
C_R(t)=\text{the predeclared realized-complexity statistic at time }t
\]

under a declared regime with relevant resource bounds `R`. Here `C_R(t)` need not be an individual measurement: it may be a mean, quantile, instantaneous maximum, established frontier, or lineage statistic. The definition of `C_R` must say which.

The fixed-regime contract also records the metric, environmental specification, evolutionary rules, sampling schedule, and observation protocol. Subscript `R` highlights resource conditioning without pretending that resources are the whole regime.

**Interpretation.** This object represents realized history. It contains no claim about unvisited states or latent platform capacity.

The accessibility boundary remains:

\[
\boxed{
\text{not observed}\neq\text{not possible}
\qquad\text{and}\qquad
\text{large formal state space}\neq\text{evolutionarily accessed complexity}.
}
\]

## 6. Complexity frontier under resource scaling

For cross-configuration evidence define:

\[
K_{\Pi}(R)=\text{the attained established-complexity frontier under resources }R
\]

where \(\Pi\) is the frozen run protocol: metric, temporal/frontier statistic, observation budget, replication design, initialization rule, and establishment criterion. Including \(\Pi\) prevents a larger or longer search from being mistaken for a resource effect without disclosure.

`K_Π(R)` is empirical. A formal maximum permitted by the substrate is a separate architectural ceiling, not `K_Π`. A theoretical or fitted extension beyond tested `R` is an extrapolation, not an observation.

## 7. Resource vectors and scaling paths

Resources are a vector when several limits can bind:

\[
R=(R_1,\ldots,R_m).
\]

Only limits with a system-specific route to capping the declared complexity object belong in `R`. Examples include world/population capacity, genome limit, neural capacity, memory, or available environmental information. This is not a universal resource ontology.

A scalability claim must declare an ordered path:

\[
R(\lambda),\qquad \lambda_1<\cdots<\lambda_k,
\]

including which components are fixed and co-scaled. Different paths can expose different bottlenecks; one failed single-coordinate path cannot establish global nonscalability when another declared hard bound remains fixed.

## 8. Temporal statistics

The statistic must match the claim:

| Statistic | Scientific claim represented | Principal caution |
| --- | --- | --- |
| \(\bar C_R(t)\) | Central tendency of realized population complexity | Can saturate while rare frontiers advance; can rise without a new maximum. |
| \(Q_p(C_R(t))\) | Declared population quantile | Choice of `p` controls sensitivity to rare versus typical complexity. |
| \(C_{\max,R}(t)\) | Largest observed bearer at a time | Vulnerable to error, bloat, and nonreproducing outliers. |
| Lineage statistic | Complexity along a declared ancestry path | One lineage supplies existence evidence, not system typicality. |
| Established frontier \(C_R^\dagger(t)\) | Highest historical complexity meeting an establishment rule | Depends on a declared, domain-appropriate establishment criterion. |

Mean and frontier saturation are logically independent. Reports may include both, but neither can substitute for the other. Because the hallmark concerns continued production of higher complexity, an established frontier is often the most direct statistic; it is not mandatory when another statistic expresses the scientific target better.

## 9. Finite increase versus sustained growth

One or several transitions with:

\[
C_R(t_2)>C_R(t_1)
\]

establish **FINITE COMPLEXITY INCREASE** only. Retention of the higher value after one transition does not turn that event into continuing production.

Sustainedness concerns repeated or extended advancement of the declared statistic within one sufficiently stable exogenous regime. The regime may contain endogenous ecological, population, and organizational change. Designer changes to resources, tasks, environment, rules, metric, or observation protocol terminate or stratify the within-regime claim.

## 10. Right censoring

Every history ends at `T_max`. Therefore the canonical rule is:

\[
\boxed{
\text{growth through }T_{\max}
\Rightarrow
\text{no saturation established before }T_{\max},
\text{ not indefinite growth}.
}
\]

No finite observation establishes:

\[
\lim_{t\to\infty}C_R(t)=\infty.
\]

The report must state the observed interval, sampling scheme, whether the last record is close to the endpoint, and any extrapolation. “No saturation detected” is an observed-window status, not the negation of all bounded models.

## 11. Saturating alternatives

A claim of continuation must be assessed against principal system-plausible bounded alternatives, including an asymptotic ceiling, bounded fluctuation, a long plateau followed by rare steps, or a metric/substrate ceiling. MODES explicitly recommends model comparison because visual plateau judgments can mislead.[^6]

No universal parametric family is required. A linear slope may describe a window but cannot alone establish ongoingness: autocorrelation, punctuated change, path dependence, and bounded curves can all produce a positive finite-window slope. Wiser, Ribeck, and Lenski provide a useful methodological example—not a complexity result here—of comparing a bounded hyperbola and unbounded power law and testing predictions on later observations.[^9]

Use these separate saturation statements:

- **OBSERVED SATURATION SUPPORTED:** a declared statistic stops advancing over an evidentially substantial later interval, and a bounded/plateau account is supported relative to principal continuing alternatives under the frozen regime.
- **NO SATURATION DETECTED WITHIN WINDOW:** records or trend continue through the observed interval, but later behavior is censored.
- **SATURATION UNRESOLVED:** the record is too short, insensitive, punctuated, or phase-dependent to discriminate.

The cause is then annotated as **EXTERNAL CEILING REACHED**, **SATURATION BELOW KNOWN CEILING**, **BOUNDED FLUCTUATION**, **MEASUREMENT-LIMITED**, or **CAUSE UNRESOLVED**. A flat final segment alone is insufficient.

## 12. Punctuated and nonmonotonic growth

A method for complexity OEE must admit smooth, punctuated, branch-specific, and upper-envelope growth with local losses. It must not require `C_R(t+Δt) ≥ C_R(t)` at every step.

Stringmol supplies the calibration: active replication organization can be gained, lost when costly defenses cease to be maintained, and regained under renewed ecological pressure.[^10] Local loss does not erase prior complexity-generating capacity. Repeated movement among already reached levels, however, does not establish an advancing frontier.

## 13. Record/frontier complexity

The raw record process is:

\[
C_R^*(t)=\max_{\tau\le t}C_R(\tau).
\]

**Interpretation.** It is a useful optional summary when the chosen `C_R(t)` is itself frontier-bearing. It preserves historical advances despite later loss and makes record times explicit. It is inadequate as the central object because a single bloat event, measurement error, or nonreproducing outlier raises it permanently and because it says nothing about establishment or record frequency.

The method therefore prefers the established frontier below when an individual-maximum claim is used.

## 14. Establishment and outlier control

Define `C_R†(t)` as the highest historical complexity whose bearer passed a predeclared establishment rule. The weakest common rule is:

> A record must enter evolutionary history beyond instantaneous appearance through at least one domain-valid continuity channel—reproduction or descendant contribution, persistence through a declared interval, lineage continuation, or repeated independent attainment.

The selected channel and threshold must be justified before inspecting candidate records. No adaptive advantage is required. Activity/nontriviality remains part of **M**, while establishment only controls whether the observed extreme became part of the evolving population history.

One nonreproducing outlier can raise `C_R*(t)` but not `C_R†(t)`. A heritable rare lineage can support an existence claim; it does not establish typicality.

## 15. Waiting-time evidence

For successive established records (r_n) at times (t_n), record:

\[
\tau_n=t_{n+1}-t_n.
\]

Waiting times are descriptive evidence about how frequently the frontier advances. Stable or shortening intervals strengthen finite-window continuation; rapidly increasing intervals weaken it and motivate bounded, slowing, or heavy-tailed alternatives.

But:

\[
\boxed{\tau_n\uparrow\not\Rightarrow\text{eventual saturation}.}
\]

Few records cannot distinguish extremely slow unbounded growth, a true ceiling, heavy-tailed waiting, or regime change. No stationary waiting-time distribution is assumed.

## 16. Replicate histories

Replicates answer two different questions:

- **Existence evidence:** at least one honestly selected, provenance-complete trajectory establishes that the system realized the recorded pattern under `R` and \(\Pi\). A post hoc exceptional run must be labeled exploratory and cannot stand for the system generically.
- **Typicality/robustness evidence:** independently initialized histories support a distribution of `S` outcomes, ceilings, record counts, and waiting times. Consistency strengthens a generic system claim; heterogeneity is itself a result.

Do not average away a rare expanding frontier. Conversely, do not call a hand-picked run typical. The run-selection rule, failed/extinct runs, and per-run classifications must be retained alongside any aggregate.

## 17. Scalability semantics

Scalability asks:

\[
\boxed{
\text{As scientifically relevant external bounds are relaxed, does the attained evolutionary}
\atop
\text{complexity frontier continue to increase across the tested family of experiments?}
}
\]

It is not a time-series claim. It concerns `K_Π(R(λ))`, with resource path, levels, observation protocol, and frontier statistic declared.

Architectural absence of a fixed maximum is recorded separately as **IN-PRINCIPLE EXTENSIBILITY**. It is neither observed scalability nor evidence that evolution accesses higher complexity.

## 18. Multi-resource bottlenecks

Before interpreting a scaling plateau, identify the externally imposed bounds plausibly capable of limiting the declared complexity object. Bounds included in the scaling test must be justified from system structure or prior results, not added indefinitely after every negative outcome.

If a known unscaled hard limit becomes dominant, classify:

`RESIDUAL EXTERNAL BOTTLENECK`.

This status blocks a global nonscalability inference but does not count as positive scalability. Path comparisons can localize co-limitation; they do not identify a mechanism of complexity growth.

## 19. Fixed-limit saturation versus scalable frontier

Four evidence cases are logically possible:

| Case | Realized sustainedness | Resource scalability | Permissible interpretation |
| --- | --- | --- | --- |
| A | Strong | Weak | Long realized growth is observed, but a known or untested ceiling prevents a scalability claim. Avida is the E1 calibration, not a full exemplar. |
| B | Weak | Strong | Larger configurations attain higher established frontiers, while fixed runs saturate or lack continuing histories. Geb is the E1 calibration. |
| C | Strong | Strong | Desired strongest operational evidence: extended established-frontier growth plus continued scaling across relevant tested bounds. Still finite and conditional. |
| D | Weak | Weak | Neither continuing realized growth nor a resource-scaled frontier is supported. |

External resource enlargement can move a frontier from one experiment to another. It does not retroactively make a fixed-run history ongoing.

## 20. Scaling relation and resource cost

The observed relation is reported without prescribing its form:

\[
K_\Pi(R(\lambda))\sim f(\lambda).
\]

Candidate bounded, logarithmic, power-law, or other relations must come from system-specific evidence. No universal slope, significance threshold, or preferred law is valid across metrics and resource paths.

The report must expose the resource cost of frontier improvement: the values of `R`, run duration, population/exposure, and computational budget associated with each attained frontier. If `K ~ log R`, mathematical unboundedness coexists with exponentially growing resource cost per linear complexity increment. Efficiency is not an OEE gate, but feasibility cannot be hidden by the word “unbounded.”

This supports a descriptive distinction between **formal/operational scalability** and **effective continuation over a declared scientifically relevant scale**. No universal “interesting enough” threshold is introduced; the observed frontier and its resource cost are reported so readers can judge practical reach without altering the formal category.

Finite-size scaling offers only a structural analogy: both inspect how finite-system observables shift with system size. Physics finite-size scaling is tied to a specified critical model, scaling ansatz, and controlled limit; those assumptions are not established for heterogeneous evolutionary systems.[^11] CG3 therefore borrows the discipline of explicit size paths and finite-range qualification, not critical exponents or universality.

## 21. Geb operational meaning of indefinite scalability

**Fact.** Channon reports that maximum individual complexity is asymptotically bounded when either world length/population capacity or maximum neural capacity is scaled alone, but increases across the tested range when both are scaled together. The relation is approximately logarithmic in the lower limiting resource, with runs lasting years and billions of reproductions.[^7]

Tokyo Type 1 gives the operational semantics: an increasing sequence of greater upper bounds continues to an unknown tested length, and every claim should quantify the time or physical-limit extent reached.[^3][^4] Hence the warranted phrase is:

`INDEFINITELY SCALABLE IN THE PUBLISHED OPERATIONAL SENSE, TO THE EXTENT TESTED`.

This is strong finite-range `I` evidence plus a model-supported interpretation. It is not proof that `K(R) → ∞`, not a fixed-world temporal result, and not higher-order growth.

## 22. Avida calibration

**Fact.** In the E1 calibration, Avida's information-based genomic complexity rises through a fixed-environment, fixed-length history. The genome length and finite environmental task information provide known candidate ceilings; no matched multi-resource scaling study was reviewed.[^2][^12]

Methodologically, Avida is **Case A**: direct finite within-history growth, an extended observed trend, and no detected plateau within the focal window, but a known finite capacity and no `I` result. “Ongoing upward trajectory” in MODES remains an observed-window description, not an indefinite claim.[^6]

## 23. Hintze triviality calibration

**Fact.** Hintze's path genomes become longer and less compressible over five million generations in a formally extensible setup, yet the fixed behavior language and rarity-driven path construction do not establish increased organized capability.[^8]

CG3 therefore has a strict entry condition:

\[
M\text{ fails}\Rightarrow S\text{ and }I\text{ are not hallmark classifications}.
\]

The time trend may still be described as a property of the proxy, and architecture may be called extensible. Neither is meaningful OEE-complexity evidence. This prevents counterexample G without subjective, post hoc exclusion.

## 24. MODES relation

**Fact.** MODES's complexity metric is the maximum informative-site count among persistent population components. Its forward persistence filter controls short-lived components, and its NK demonstration recovers saturation at the finite genome-length ceiling. The paper recommends selecting among plausible bounded and unbounded mathematical models rather than judging graphs by eye.[^6]

MODES therefore supplies three CG3 ingredients:

1. an establishment-like persistence filter;
2. an explicit maximum-complexity time series; and
3. bounded-versus-unbounded trend comparison.

It does not collapse CG3. Its “complexity potential” is a hallmark-measure label for realized filtered maximum complexity, not `K_Π(R)`; it does not provide a multi-resource scaling-path record, residual-bottleneck audit, or a required separation among observed, extrapolated, and architectural claims. Its model-fitting recommendation is incorporated conditionally, not universalized.

## 25. Tokyo Type 1 relation

**Fact.** Tokyo Type 1 already separates qualitative long-term trend classification (step 3), indefinite scalability in diversity and complexity (step 4), and the order of indefinite scalability (step 5). It explicitly treats finite empirical claims as qualified by the tested time or parameter extent.[^3][^4]

This is the strongest absorption result:

\[
\text{CG3}
=
\text{Tokyo Type 1 trend analysis}
+
\text{Geb-style resource scaling}
+
\text{explicit censoring/triviality controls},
\]

with MODES supplying persistence and bounded-alternative comparison. The ingredients are established. CG3 contributes their minimal, two-record integration and does not claim a new theory of ongoingness.

## 26. Higher-order complexity growth

**Fact.** In Channon's procedure, “order of complexity growth” refers to the scaling of attained complexity with limiting resources. Geb's maximum individual complexity scales approximately logarithmically with the lower of maximum population and neural capacity. A “higher order” means a stronger complexity-versus-resource scaling order than this logarithmic result, sought within a system already exhibiting indefinite scalability so that substantially more complex artifacts or behavior may be reachable on feasible scales.[^3][^7]

The article does not declare one universal target function or threshold. Therefore:

`HIGHER-ORDER GROWTH NOT ESTABLISHED`.

No method may equate higher absolute complexity, a steeper time slope, larger population, higher-dimensional metric, hierarchy, or major transition with higher-order scaling unless the resource-frontier relation itself supports that reading.

## 27. Time-growth versus scaling-order distinction

The two derivatives, when they are meaningful at all, concern different objects:

\[
\frac{dC_R(t)}{dt}
\qquad\text{versus}\qquad
\frac{dK_\Pi(R(\lambda))}{d\lambda}.
\]

The first is a temporal trend within a regime. The second is a cross-configuration scaling relation. Channon's “order” concerns the latter. Neither derivative is required by the method, and neither receives a universal positive threshold.

## 28. Evidence versus extrapolation

Every conclusion must carry one of three inference tags:

| Tag | Meaning | Maximum warranted language |
| --- | --- | --- |
| **OBSERVED** | Directly present within tested histories or resource levels | “Growth observed through `T_max`” or “frontier rises across tested levels.” |
| **MODEL-SUPPORTED EXTRAPOLATION** | A declared fitted or theoretical relation extends beyond observations | “The selected relation supports continuation beyond the observed range,” with alternatives and uncertainty stated. |
| **IN-PRINCIPLE CLAIM** | Architecture has no identified formal bound or can be enlarged without redesign | “No formal architectural ceiling is identified,” not “evolution will realize growth.” |

Claims can carry more than one tag for different clauses. They cannot be promoted from architectural possibility to realized evidence or from finite observation to literal infinity.

## 29. Sustainedness evidence vocabulary

The provisional S hierarchy survives with refined meanings:

- **S0 — NO GROWTH ESTABLISHED:** the declared statistic has no supported increase, or the evidence is inadequate.
- **S1 — FINITE COMPLEXITY INCREASE:** one or several established increases occur, without an extended advancing trend.
- **S2 — EXTENDED REALIZED GROWTH:** the declared statistic advances across a substantial stated interval under one exogenous regime. “Substantial” is justified relative to system generations, turnover, and earlier record intervals, not a universal duration.
- **S3 — GROWTH WITHOUT DETECTED SATURATION:** an established frontier or other matching statistic continues to advance through the observation window, while principal bounded alternatives have been examined and no plateau is supported. This remains right-censored.
- **S4 — STRONG FINITE-WINDOW CONTINUATION EVIDENCE:** S3 recurs across independently initialized histories, prespecified sequential windows, or both, and the principal bounded/saturating alternatives are disfavored under transparent system-appropriate analyses.

S4 is the strongest empirical sustainedness category, not proof of indefinite temporal growth. Pair it with a separate saturation statement and inference tag.

## 30. Scalability evidence vocabulary

- **I0 — NO SCALABILITY EVIDENCE:** no relevant resource comparison exists, or active complexity fails to increase.
- **I1 — FINITE CAPACITY EXPANSION:** at least one justified increase in relevant bounds yields higher attained established complexity under a comparable protocol.
- **I2 — REPEATED FRONTIER SCALING:** higher established frontiers occur across several ordered resource configurations on a declared path.
- **I3 — NO SCALING SATURATION DETECTED:** I2 continues across the tested range, principal bounded scaling alternatives are examined, and no known unscaled external bottleneck invalidates the path-level inference.
- **I4 — INDEFINITELY SCALABLE IN THE PUBLISHED OPERATIONAL SENSE:** an extensible sequence of greater bounds is supported to a quantified tested extent, with relevant co-limitations addressed and the operational term explicitly qualified.

I4 is reserved for literature that justifies that terminology. It remains finite-range and does not entail `K(R) → ∞`. A separate **RESIDUAL EXTERNAL BOTTLENECK** annotation blocks I3/I4 until resolved or explicitly bounded.

## 31. Minimal sustainedness record

The proposed record simplifies to:

```text
System / provenance:
Complexity object and metric (frozen X/M result):
Temporal complexity statistic:
Exogenous regime and resource vector:
Observation interval and sampling:
Establishment rule:
Observed growth / record evidence:
Saturation evidence and principal bounded alternatives:
Replicate basis (existence versus typicality):
Right-censoring and extrapolation tag:
S classification:
```

“Alternative bounded explanation” is combined with saturation evidence; robustness is combined with the replicate claim; and provenance is moved to the first line. The record remains human-auditable and does not prescribe software or one statistical test.

## 32. Minimal scalability record

```text
System / provenance:
Complexity object and metric (same frozen X/M result):
Resource dimensions and declared scaling path:
Resource levels and run protocol tested:
Established-frontier statistic:
Observed frontier relation and resource cost:
Known residual hard bounds:
Scaling-saturation evidence and alternatives:
Observation versus extrapolation tags:
I classification:
```

The temporal record and scalability record may cite the same experiments, but neither inherits the other's conclusion.

## 33. Two-axis representation

The pair survives:

\[
\boxed{(S,I)}.
\]

It is categorical and accompanied by the two records, not converted to a score. A full claim must also retain E1's `X/M/E` status. The pair allows Avida-like `(S2 or S3, I0)` evidence and Geb-like `(S unresolved, I4)` evidence without ranking one as universally “more open-ended.”

The strongest operational complexity-hallmark evidence would require a valid (X/M/E) chain, a frontier-matched S3 or S4 record, and I3 or qualified I4 on the same complexity object under compatible protocols. Even then the conclusion is **strong finite evidence consistent with ongoing complexity growth**, not a metaphysical or mathematical proof of infinity.

## 34. Counterexamples A–L

| Case | Methodological result | Why |
| --- | --- | --- |
| **A. Sharp rise, then plateau** | S1; **OBSERVED SATURATION SUPPORTED** if alternatives and window justify it; I separate | One large transition is finite increase, not continuing production. |
| **B. Slow rise throughout a finite run** | S2 or S3; **NO SATURATION DETECTED WITHIN WINDOW** | Positive slope alone is insufficient; the endpoint censors slow unbounded and eventual saturation alike. |
| **C. Oscillation with no new record** | S1 at most after the initial record; **BOUNDED FLUCTUATION** if supported | Local change and regain do not extend the frontier. |
| **D. Repeated records with rising waiting times** | S3 possible; S4 only with replication/alternative checks | Rising \(\tau_n\) weakens continuation evidence but does not prove closure. |
| **E. Fixed runs saturate; scaled runs reach higher ceilings** | Weak S, I2–I4 as evidence warrants; Case B | Scalable capacity and fixed-run ongoingness remain different. |
| **F. Available genome grows; active complexity does not** | S0, I0; latent capacity only | External room without evolved use does not move `K_Π`. |
| **G. Unbounded junk/bloat proxy grows** | **M fails**; no hallmark S/I classification | Hintze firewall applies before CG3. |
| **H. Mean flat; frontier grows** | Mean S0, frontier S2/S3 | The declared statistic determines the claim; mean saturation does not imply frontier saturation. |
| **I. Frontier rises through one nonreproducing outlier** | Raw `C*` rises; established `C†` does not | The establishment rule blocks an instantaneous anomaly without requiring adaptation. |
| **J. Scaling rises but hidden bottleneck remains** | I1/I2 plus **RESIDUAL EXTERNAL BOTTLENECK**; no I3/I4 | Finite gains are observed, but global path-level continuation is unresolved. |
| **K. Only external task complexity expands** | I1/I2 conditional on the environmental path; S not established for an autonomous fixed regime | Designer-supplied complexity is disclosed as exogenous scaling, not within-history evolution. |
| **L. No formal substrate bound, no observed growth** | S0, I0, plus **IN-PRINCIPLE EXTENSIBILITY** | Architectural possibility is not evolutionary accessibility or realization. |

The distinctions follow from frozen contracts rather than ad hoc system exclusions.

## 35. Strongest prior-art absorption test

The strongest absorption attempt succeeds at the ingredient level:

1. Tokyo Type 1 already separates trend, scalability, and order.
2. Geb supplies the operational multi-resource calibration.
3. MODES supplies persistence and model-based boundedness analysis.
4. Bedau-style classifications distinguish single-run evidence from more generic replicated/parameter-region claims.
5. Hintze supplies the metric-validity firewall.

It fails at the workflow level: none of the reviewed sources packages two independent records with a frozen regime/protocol, established frontier, existence-versus-typicality report, resource path, residual-bottleneck status, and observation/extrapolation tags. Therefore the result is **INTEGRATION GAP ONLY**, not a distinct new theory or statistical discovery.

## 36. Strongest positive interpretation

\[
\boxed{
\text{Ongoing-complexity evidence can be represented without one universal metric by separating}
\atop
\text{realized temporal frontier growth from resource-scalability evidence.}
}
\]

**Attack.** The representation still depends on system-specific metric validity, regime choice, establishment rule, resource path, run protocol, and bounded alternatives. `S` and `I` can each be strong while referring to incompatible statistics or complexity objects; pairing them is legitimate only when these contracts align. Censoring prevents the pair from proving infinite continuation.

**Refinement.** The pair is an auditable evidence architecture, not a sufficient definition of OEE. It states exactly which finite observations support which operational claim and where extrapolation begins.

## 37. Strongest skeptical interpretation

The skeptic is correct that finite time and finite resource ranges cannot deductively distinguish extremely slow unbounded growth from eventual saturation in all possible futures. This blocks `UNBOUNDED FOREVER`.

It does not make scientific inference impossible. Other empirical sciences compare bounded and continuing models, test predictions on later windows, replicate histories, and qualify conclusions to observed domains; Wiser et al. provide one example.[^9] The warranted outcome is graded, conditional evidence with explicit censoring—not certainty and not silence.

“Ongoing” and “indefinitely scalable” must therefore remain operational terms. Their evidential force comes from continued successful tests over declared windows and paths, plus failure of principal bounded alternatives, and can be revised by later saturation.

## 38. Central decision

\[
\boxed{\textbf{B — INTEGRATION GAP}.}
\]

Existing prior art contains the necessary substantive ingredients. The missing piece was an explicit joined evidence workflow that:

- freezes the complexity object and metric before CG3;
- separates `C_R(t)` from `K_Π(R)`;
- separates observed, extrapolated, and in-principle claims;
- controls frontier outliers without requiring adaptation;
- distinguishes existence from typicality;
- declares multi-resource scaling paths and residual bottlenecks; and
- keeps higher-order scaling distinct from temporal growth and basic indefinite scalability.

This is not C, D, or E: neither the temporal nor scalability axis alone dominates the gap, and higher-order scaling is already interpretable as the resource-scaling-order challenge even though no positive case exists.

## 39. Methodology readiness

\[
\boxed{\textbf{READY FOR RETROSPECTIVE USE}.}
\]

The two records, vocabularies, inference tags, and counterexample handling are explicit enough to apply to published Geb, Avida, Tierra, and Stringmol reports without redefining success after seeing each result. Prospective readiness is not claimed because the workflow has not yet been tested for whether published evidence can populate every field consistently, and no prospective preregistration or new experiment design has been audited.

## 40. Consequence for E1

\[
\boxed{\textbf{CONFIRMED AS METHODOLOGICALLY DISTINCT}.}
\]

Avida's strength lies on the realized temporal axis: a defensible complexity statistic advances within one fixed-environment history. Geb's strength lies on the resource axis: attained active-component maxima advance along a co-scaled resource path. The two results can share a hallmark program without being collapsed or numerically compared.

The historical E1 artifact remains unchanged.

## 41. Known / Underexplored / Potentially Novel / Unknown

| Status | Boundary after CG3 |
| --- | --- |
| **ESTABLISHED** | Long-term trend analysis, persistence filters, bounded-versus-unbounded model comparison, indefinite-scalability analysis, multi-resource Geb calibration, and separation of scaling order are prior art. |
| **PARTIALLY EXPLORED** | Qualification of finite-time and finite-parameter claims, replicate/parameter-region generality, and resource-cost implications are present but distributed across literatures. |
| **UNDEREXPLORED** | A single auditable two-record workflow joining established-frontier temporal evidence, scaling paths, residual bottlenecks, existence/typicality, and inference tags. This is an integration gap, not yet a novel method claim. |
| **POTENTIALLY NOVEL** | None claimed. The established-frontier notation and record templates are local synthesis devices unless prior-art review and application later show a distinct contribution. |
| **UNKNOWN** | Whether one reviewed system can populate strong compatible `S` and `I` records; whether the workflow survives retrospective use without object-specific exceptions; and which stronger resource-scaling orders are empirically achievable. |

No hypothesis is created.

## 42. Highest-information next operation

Exactly one operation is selected and not performed:

\[
\boxed{\textbf{CG3A — RETROSPECTIVE METHOD APPLICATION}.}
\]

Artifact/operation name:

> **APPLICATION — COMPLEXITY SUSTAINEDNESS / SCALABILITY CROSS-SYSTEM**

Exact evidence target:

> Apply the frozen paired sustainedness/scalability records to the already reviewed Geb, Avida, Tierra, and Stringmol publications, and determine whether their reported observations support internally consistent `(S,I)` classifications without adding new metrics, fitting new models, or reanalyzing raw data.

## 43. Stop condition

The complexity methodology branch must pause, consolidate, or return to evidence when any of the following occurs:

1. retrospective records cannot be completed from published evidence without new simulation, raw-data analysis, or post hoc metric changes;
2. `S` and `I` cannot be paired without referring to incompatible complexity objects or protocols;
3. establishment or bottleneck judgments require unavailable external validation;
4. the evidence architecture needs a universal slope, p-value, stationary process, or complexity scalar;
5. the next question becomes causal—why complexity grows—rather than evidential; or
6. CG3A establishes the stable boundary, at which point the methodology must consolidate before any prospective test or mechanism program.

This artifact stops at CG3. It does not perform CG3A, any other CG3 sub-operation, Q028, mechanism research, model fitting, or hypothesis creation.

## Sources

[^1]: [Synthesis 005 — Selection of the Next OEE Hallmark](SYNTHESIS_005_NEXT_OEE_HALLMARK.md).
[^2]: [Evidence Matrix 002 — Complexity Growth](EVIDENCE_MATRIX_002_COMPLEXITY_GROWTH.md).
[^3]: Channon, A. (2024). [“A Procedure for Testing for Tokyo Type 1 Open-Ended Evolution.”](https://doi.org/10.1162/artl_a_00430) *Artificial Life*, 30(3), 345–355.
[^4]: Channon, A. (2020). [“A Procedure for Testing for Tokyo Type 1 Open-Ended Evolution (Draft Edition).”](https://workshops.alife.org/oee4/papers/channon-oee4-camera-ready.pdf) Fourth Workshop on Open-Ended Evolution. Used to verify the explicit five-step sequence and finite-range qualification; the 2024 journal article is authoritative.
[^5]: Bedau, M. A., Snyder, E., & Packard, N. H. (1998). [“A Classification of Long-Term Evolutionary Dynamics.”](https://people.reed.edu/~mab/papers/alife6.ab.htm) *Artificial Life VI*, 228–237.
[^6]: Dolson, E. L., Vostinar, A. E., Wiser, M. J., & Ofria, C. (2019). [“The MODES Toolbox: Measurements of Open-Ended Dynamics in Evolving Systems.”](https://doi.org/10.1162/artl_a_00280) *Artificial Life*, 25(1), 50–73.
[^7]: Channon, A. (2019). [“Maximum Individual Complexity is Indefinitely Scalable in Geb.”](https://doi.org/10.1162/artl_a_00285) *Artificial Life*, 25(2), 134–144.
[^8]: Hintze, A. (2019). [“Open-Endedness for the Sake of Open-Endedness.”](https://doi.org/10.1162/artl_a_00289) *Artificial Life*, 25(2), 198–206.
[^9]: Wiser, M. J., Ribeck, N., & Lenski, R. E. (2013). [“Long-Term Dynamics of Adaptation in Asexual Populations.”](https://doi.org/10.1126/science.1243357) *Science*, 342(6164), 1364–1367. Used only as a finite-history model-comparison analogy, not as a complexity matrix case.
[^10]: Hickinbotham, S., Stepney, S., & Hogeweg, P. (2021). [“Nothing in Evolution Makes Sense Except in the Light of Parasitism: Evolution of Complex Replication Strategies.”](https://doi.org/10.1098/rsos.210441) *Royal Society Open Science*, 8, 210441. Used only as E1's nonmonotonic calibration.
[^11]: Fisher, M. E., & Barber, M. N. (1972). [“Scaling Theory for Finite-Size Effects in the Critical Region.”](https://doi.org/10.1103/PhysRevLett.28.1516) *Physical Review Letters*, 28, 1516–1519. Used only to delimit the finite-size-scaling analogy.
[^12]: Adami, C., Ofria, C., & Collier, T. C. (2000). [“Evolution of Biological Complexity.”](https://doi.org/10.1073/pnas.97.9.4463) *Proceedings of the National Academy of Sciences*, 97(9), 4463–4468.
[^13]: Ackley, D. H., & Small, T. R. (2014). [“Indefinitely Scalable Computing = Artificial Life Engineering.”](https://doi.org/10.7551/978-0-262-32621-6-ch098) *Artificial Life 14*, 606–613. Used only to delimit architectural indefinite scalability from evolved-frontier evidence.
