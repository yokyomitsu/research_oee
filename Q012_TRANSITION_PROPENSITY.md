# Q012 — Transition Propensity

One theoretical research pass, 2026-09-07. Scope: whether completing one evolutionary-regime transition causally changes access to later, qualitatively distinct transitions. This pass does not propose an OEE metric, implement a model, or formulate a complete theory.

## 1. Problem statement

Repeated major transitions are a possible history or OEE hallmark, not an explanation of their own recurrence. Three claims must remain separate:

1. **Transition occurrence:** a regime transition happened.
2. **Transition accessibility:** at least one further regime transition is reachable afterward.
3. **Transition-to-transition effect:** something produced by the completed transition changes the feasibility of one or more later regime transitions.

The third claim is causal. Chronological order is insufficient: a prior transition can be merely necessary background, both transitions can depend on a shared environment, or later levels can have been available in the substrate from the beginning.

No standard scalar called “transition propensity” was found. The established neighboring objects are target-specific evolvability, conditional evolutionary transition rates, key innovations, facilitating evolutionary transitions, and directional bias in hierarchical evolution. These make the question coherent only conditionally. Following Q010, a comparison requires sufficiently matched transition classes, process conditions, and resource budgets; genuinely unmatched post-transition classes remain incomparable.

**Interpretation:** “capacity to undergo transitions” is best treated here as a family of causal enabling or suppressing relations, not a new intrinsic quantity.

## 2. Existing ongoing-transition OEE theory

**Fact:** OEE literature explicitly lists ongoing major transitions as an especially strong form of open-ended evolution. It also distinguishes the existence of some historical transitions from ongoing production: the York report notes that the surveyed transitions were contingent, that there may be no more, and that individual transitions can spur many later adaptations without constituting OEE. [Taylor et al. 2016](https://doi.org/10.1162/ARTL_A_00210), [Packard et al. 2019](https://doi.org/10.1162/artl_a_00291)

Szathmáry explicitly treats some transitions as repeated or recursive, including multicellularity and plastid acquisition. This classifies histories and decomposes transitions into origin, maintenance, and transformation; it does not derive a feedback law by which completing one transition raises the rate of the next. [Szathmáry 2015](https://doi.org/10.1073/pnas.1421398112)

Evolution of evolvability already covers cases in which inherited organization changes the distribution of future variation. Applying that umbrella to future *regime transitions* is legitimate but does not solve the target problem. A change can increase ordinary adaptation, diversification, or complexity within the new regime without increasing access to another unit of selection, inheritance system, or reproductive ontology.

Metasystem-transition and progressive-hierarchy theories describe successive higher levels of control. Their recursive imagery is close to the present question, but often treats progression or increased adaptive control as a premise. It does not supply comparative evidence that a completed transition systematically changes later transition rates.

**Known boundary:** ongoing transitions are an OEE hallmark; recursive transitions and evolved evolvability are prior art; a self-sustaining transition-to-transition mechanism is not established.

## 3. Hierarchical artificial systems

DISHTINY is the strongest critical case because it was designed to make fraternal transitions repeatable and scalable.

### What is built in

In the original system, cells occupy a toroidal grid, reproduce into neighboring sites, carry channel identifiers, recognize channel partners, pool resources, and encounter spatial resource waves whose predefined radii reward coordinated groups of particular scales. Multiple overlaid resource-wave/channel systems constitute hierarchical “levels.” The reported experiments supplied two levels, separate identifiers for each level, strict nesting rules, group bottlenecks, and explicit level-specific resource scales. [Moreno & Ofria 2019](https://doi.org/10.1162/artl_a_00284)

The genotype contained 15 parameters controlling manually designed transition-relevant strategies: reproduction, resource pooling, apoptosis, propagule creation, and propagule endowment. Thus selection chose among strategies, but neither the behavioral vocabulary nor the two-level hierarchy was created by the first transition.

The authors report an especially important limitation: second-level allocation could leapfrog and supersede first-level individuality; they could not show that first-level individuality was preserved in or necessary for the second. They explicitly identified enforced nesting and predefined signaling networks as restrictions to relax in future work.

### What later versions evolved

The SignalGP version allowed evolved programs to control resource sharing, reproductive timing, communication, and apoptosis. It generated diverse life histories and did not prescribe a single collective-reproduction routine. Nevertheless, the ability to assign hereditary-group identifiers, recognize kin, found propagules, and—in nested treatments—use exactly two strictly nested grouping levels remained supplied. The cooperative resource regime and group-aging mechanism also imposed opportunities for group formation and turnover. [Moreno & Ofria 2022](https://doi.org/10.3389/fevo.2022.750837)

This supports the following answers:

1. Transition-relevant strategies and life histories evolved.
2. Later hierarchical levels were structurally available from initialization.
3. No experiment showed that completion of level one created the channel or state space for level two.
4. The 2019 result did not even require level-one individuality for the level-two phenotype.
5. SignalGP expanded behavioral expressivity, but finite case studies did not demonstrate unbounded strategy novelty or ongoing creation of new levels.
6. Configured group levels, fixed spatial and resource scales, finite grids and populations, and computational cost limit continuation. The 2022 study notes that shifting selection to groups of many cells compounds digital-evolution population-size and processing limits.

**Conclusion:** DISHTINY demonstrates evolution *within a pre-enabled recursive hierarchy*. It does not yet demonstrate endogenous construction of recursive transition capability.

## 4. Cumulative major transitions

Biological history contains strong prerequisite chains: DNA-based inheritance precedes later cellular organization; eukaryogenesis precedes the independent origins of complex multicellularity; multicellular organisms precede eusocial colonies; and biological evolution produced capacities for language and cultural inheritance. These histories show dependence, not a general increase in transition-producing ability.

“Facilitating evolutionary transition” (FET) is close prior art. Robin and colleagues define an FET as a major evolutionary or competitive transition that is necessary but insufficient for a later major system transition. Eukaryogenesis is their example: it was required for the later animal/plant/fungal ecosystem transformation, but eukaryotes persisted for a long interval without causing it. FET therefore formalizes a *specific prerequisite*, not general transition propensity. [Robin et al. 2021](https://doi.org/10.3389/fevo.2021.711556)

Claims about codes and information channels make a related historical argument: flexible codes, DNA, epigenetic regulation, and later symbolic transmission can expand how information is stored or used and can precede major transitions. Such accounts identify plausible enabling structures, but increased storage or bandwidth alone does not provide a conditional rate for later regime changes. [Szathmáry 2015](https://doi.org/10.1073/pnas.1421398112), [The major evolutionary transitions and codes of life 2021](https://doi.org/10.1016/j.biosystems.2021.104548)

Cultural-evolution work treats human open-ended culture as evolved open-endedness: biological changes in cognition and social organization produced a second evolutionary process with unusually broad cumulative innovation. Yet this literature explicitly leaves open whether OEE requires cumulative major transitions. Culture's open-ended outcomes do not by themselves show repeated creation of new hereditary systems or selectable units within culture. [Borg et al. 2024](https://doi.org/10.1162/artl_a_00406)

Autocatalytic-set theory explains how reactions or replicators can mutually sustain and amplify a chemical organization, and synthetic-transition reviews use it for early evolutionary transitions. It does not establish that the *occurrence of a regime transition* catalyzes another regime transition. “Transitions catalyze transitions” would therefore conflate molecular catalytic closure with the unproved cross-transition causal relation and is not retained. [Solé 2016](https://doi.org/10.1098/rstb.2016.0175)

**Interpretation:** cumulative histories provide candidate causal dependencies and stress tests. They do not establish a transition-autocatalytic law.

## 5. Transition-generated enabling structures

Completed transitions can generate structures with demonstrated downstream evolutionary effects:

* **Bottlenecks and clonal development:** snowflake multicellularity produced a single-cell bottleneck that exposed multicellular traits to selection. Ratcliff and colleagues experimentally found higher-level evolvability to arise as a consequence of the transition rather than direct selection for evolvability. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102)
* **New developmental organization:** multicellular development, division of labour, and communication can create selectable collective traits and new ecological strategies.
* **Inheritance channels:** DNA, epigenetic regulation, sexual recombination, language, and external symbolic storage can alter fidelity, recombination, and the range of heritable organization.
* **Coordination and conflict control:** eukaryotic cellular machinery and mechanisms that align lower-level interests plausibly facilitated repeated origins of multicellularity. [Blackstone 2013](https://pmc.ncbi.nlm.nih.gov/articles/PMC3685466/)
* **Ecological construction:** an evolved individual can modify population or environmental structure relevant to a later transition, as Q011 established.

These findings are important but weaker than the target claim. The snowflake result shows increased evolvability *within the new multicellular regime*, not access to a second transition in individuality. Communication and developmental machinery can yield many phenotypes without creating another evolutionary level. A large genome or high-fidelity code can remain within one regime; eukaryotic genome size varies enormously without tracking organismal complexity. [Elliott & Gregory 2015](https://pmc.ncbi.nlm.nih.gov/articles/PMC4571570/)

The strongest candidate for branching enablement is eukaryogenesis, whose products were reused in multiple independent multicellular lineages and subsequent symbioses. But shared ancestry, environmental changes, long delays, and survivor bias prevent this historical pattern from identifying a general propensity increase.

## 6. Transition-generated constraints

The sign of a transition-to-transition effect is not fixed. A completed transition can also create:

* longer reproductive cycles and higher construction cost;
* smaller effective populations and reduced mutation supply at the new level;
* coordination and policing overhead;
* developmental canalization and entrenchment;
* dependence among formerly autonomous parts;
* loss of lower-level reproductive and hereditary options;
* larger energetic or spatial requirements.

The York OEE discussion explicitly noted that successive major transitions tend to produce organisms requiring more resources and existing in smaller populations, imposing a finite-system limit on indefinitely continuing hierarchy. DISHTINY exhibits the artificial counterpart: groups contain many cells, so a fixed computational budget supports fewer group-level individuals. [Taylor et al. 2016](https://doi.org/10.1162/ARTL_A_00210), [Moreno & Ofria 2022](https://doi.org/10.3389/fevo.2022.750837)

McShea directly considered directional feedback in hierarchical evolution. Greater hierarchy might offer more components that can combine into a higher level, but it also offers more routes to disassembly and loss. Proposed upward and downward biases both had limited empirical support; an unbiased diffusion with a lower bound remained plausible. This is explicit prior art for positive-versus-negative transition feedback, and it did not establish either sign. [McShea 2001](https://doi.org/10.1046/j.1420-9101.2001.00283.x)

Resource and organization trade-offs cannot be collapsed into “more complex means more transition-capable.” New expressive capacity and increased search cost can occur together, and Q010 supplies no universal currency for netting them into one scalar.

## 7. Reversions

Reversions reject an irreversible ladder model. Experimental selection can reverse recently evolved multicellularity, and current theory distinguishes paradigmatic reversions—loss of the higher-level collective and recovery of lower-level individuality—from agential reversions in which internal conflict erodes the collective's unity of evolutionary purpose. [Rebolleda-Gómez 2019](https://doi.org/10.1111/evo.13654), [Schenkel, Ågren & Patten 2026](https://doi.org/10.1093/jeb/voag007)

Entrenchment makes some reversions difficult because constituent parts lose autonomous functions. But subsequent conflict, environmental change, or renewed lower-level autonomy can change the direction and level of selection. The products of one transition can therefore suppress reversal, enable a different downward transition, or later be dismantled.

**Interpretation:** transition accessibility is a dynamic, directed network with possible reversals, losses, and context changes—not an order (L_0<L_1<L_2<\cdots). Ongoing-major-transition OEE accounts remain coherent as hallmark accounts, but they cannot infer self-amplification merely from an upward historical maximum.

## 8. Transition-to-transition causality

Existing methods can address bounded versions of the causal question:

* **Experimental replay or ablation:** repeat a first transition, manipulate a product attributed to it, and compare arrival of a specified second transition under matched environments and resource budgets.
* **Digital counterfactuals:** disable an evolved communication, bottleneck, or inheritance feature while leaving a later level available; separately compare systems in which that level is and is not designer-provided.
* **Independent natural origins:** compare replicated clades in which a candidate enabling structure arose or did not arise, while modeling shared ancestry and ecological covariates.
* **Phylogenetic dependent-rate models:** Pagel-style models ask whether the transition rate of one discrete character depends on the state of another. These can test a conditional-rate claim but are correlational, model-dependent, and vulnerable to hidden states, extinction, and classification error. [Pagel 1994](https://doi.org/10.1098/rspb.1994.0006)
* **Historical reconstruction:** establish temporal order, mechanistic use, and counterfactual necessity. This can support a prerequisite relation but rarely identifies the probability of alternatives that left no descendants.

Key-innovation research supplies an important warning. A trait can open a new adaptive zone or raise eventual richness without increasing lineage diversification rate, and apparent post-innovation radiations can have alternative causes. Historical succession and more descendants are not equivalent to a changed transition hazard. [Rabosky 2017](https://pmc.ncbi.nlm.nih.gov/articles/PMC5665805/)

Q010 remains binding. A causal comparison can be objective for a specified, conserved transition target and resource process. If a later regime has no counterpart in the comparison system, the appropriate result is a partial prerequisite relation or an undefined comparison, not a universal propensity score.

## 9. Specific prerequisite versus general transition propensity

The distinction is defensible and already implicit in adjacent theory.

A **specific prerequisite** means that structure (S), produced during an earlier transition, is necessary or raises accessibility for one defined later transition under stated conditions. FETs, key innovations, and conditional character-transition models express this kind of claim. It can hold even if (S) reduces access to every other transition.

A **general increase** would require broader evidence: the earlier transition's products increase access to several non-equivalent later regime changes, or improve a justified partial ordering over a family of transition targets after resource costs are controlled. This is a much stronger evolution-of-evolvability claim.

Major-transition theory has no established “branching transition potential” object. Historical lists usually contain one realized child per lineage, while unobserved alternatives, extinction, and observer-dependent regime classifications make branch abundance difficult to infer. More hereditary bandwidth, modularity, or communication is not sufficient: each can support extensive novelty inside one ontology without producing another.

The phrase “transition propensity” is therefore not retained as a new mechanism. Where possible, use the established, narrower language: a conditional transition rate, a target-specific enabling relation, or changed accessibility to specified regime transitions.

## 10. Pre-enabled hierarchy versus endogenous hierarchy construction

A pre-enabled hierarchy supplies the identifiers, nesting relation, group-forming operations, or scale-specific rewards for later levels before evolution reaches them. Evolution may discover and exploit those levels, but it did not create their availability.

Endogenous hierarchy construction requires an evolved product to establish the population boundary, inheritance channel, reproduction relation, or interaction structure by which a new level becomes an effective evolutionary unit. This does not require changing microphysical rules; it requires that removing the evolved product removes or materially changes access to the later level.

DISHTINY makes the contrast unusually explicit. Its cells evolved allocation, reproductive, communication, and apoptosis strategies, but the experiments overlaid and enforced the later hereditary level. The authors acknowledged that higher-level strategies could bypass the lower level and proposed relaxing the predefined networks and nesting. Thus multiple observed levels do not demonstrate that one transition generated the next.

This is an application of the established capacity-versus-accessibility boundary from Q008, not a new principle. A universal constructor, recursively typed system, or arbitrary stack of group identifiers can pre-enable unbounded hierarchy while evolution never creates a new transition channel.

## 11. Counterexamples

| Case | Strongest finding | Consequence |
|---|---|---|
| A — completed transition followed by permanent stagnation | Szathmáry's “limited transitions” have transition-like organization but restricted phylogenetic impact; scaffold-endogenization models can also settle. Permanent future stagnation cannot be established from a finite natural history. | Completion does not imply a second transition, but “permanent” closure remains hard to prove. |
| B — transition reduces evolvability | Organelle and somatic integration remove lower-level autonomy; entrenchment, longer cycles, and smaller higher-level populations can reduce particular routes and mutation supply. | Effects are level- and target-dependent; no monotonic overall evolvability follows. |
| C — repeated predefined levels | DISHTINY's two hereditary-group levels, radii, identifiers, and nesting are available from initialization; level two can bypass level one. | Repeated hierarchy can be selected without endogenous generation of the hierarchy. |
| D — niche construction without ETI | Ecosystem engineers and social niche constructors routinely alter selective environments without becoming parts of a new reproducing individual. | Rich feedback with the environment is not sufficient for a change of evolutionary regime. |
| E — one later transition specifically enabled | Eukaryogenesis is a necessary but insufficient precursor to complex multicellularity; FET theory was introduced for such relations. | A prerequisite for one child is not general transition-generating capacity. |
| F — products plausibly enable several regimes | Eukaryotic cellular and information-processing organization precedes multiple independent origins of complex multicellularity, plastid symbioses, and eventually eusocial/cultural regimes. | This is the best branching candidate, but historical confounding and long delays prevent a general causal inference. |
| G — every transition demonstrably improves access to another | No controlled biological or artificial sequence was found. DISHTINY predefines levels; historical ladders lack counterfactual controls. | The strongest self-amplifying claim is unsupported. |

Additional negative controls matter. Snowflake multicellularity caused higher-level evolvability and later ecological diversification, but those outcomes remain within multicellular individuality. Cultural OEE creates wide and cumulative novelty, but has not demonstrated an indefinite sequence of new cultural inheritance systems or selectable ontologies. Neither should be counted as case G.

## 12. Central decision

**Decision: B — Historical but not general.**

Prior work documents cumulative, recursive, and prerequisite relations among transitions. It also explicitly asks whether hierarchical change has an upward bias and supplies mechanisms that could raise or lower it. The evidence does not support a general causal rule that completed transitions make later transitions more accessible.

Why the alternatives are weaker:

* **A** is false: no recognized theory predicts systematic transition-to-transition propensity across regimes.
* **C** accurately characterizes DISHTINY and related artificial hierarchies, but not the full biological and cultural evidence.
* **D** is too strong: target-specific enabling and suppressing effects exist; what fails is a universal sign.
* **E** overstates conceptual novelty. The causal question is under-tested, but its pieces already fall under conditional transition rates, FETs, key innovations, directional bias, and evolution of evolvability.
* **F** is too strong: Q010 permits partial, target-specific comparisons even though a universal scalar is unavailable.

The best-supported answer is therefore: a previous transition **can** reorganize access to particular later transitions, positively or negatively, but no general propensity increase—or even a common direction—is established.

## 13. Remaining explanatory gap

The narrow gap is empirical and causal: no reviewed study isolates a product evolved during a completed first transition and shows, under matched resource budgets, that it changes access to multiple qualitatively distinct second transitions whose channels were not designer-predefined.

This is narrower than evolution of evolvability and stronger than a prerequisite claim. It requires separating:

* effects on adaptation within the new regime from effects on another regime transition;
* one named historical descendant from branching access to several transition classes;
* an evolved enabling structure from a latent hierarchy supplied by the substrate;
* increased expressive capacity from added population, time, energy, or computational burden;
* causal enablement from shared ecology, temporal order, and survivor bias.

No universal scalar is needed. A collection of target-specific intervention results could answer the question partially.

## 14. Known / Underexplored / Potentially Novel / Unknown

### Known / ESTABLISHED

* Ongoing major transitions are an OEE hallmark, not an established recurrence mechanism.
* Recursive and cumulative transitions are prior art.
* FETs, key innovations, conditional transition rates, and evolution of evolvability already express narrower enabling relations.
* A new individual can gain higher-level evolvability while losing lower-level options.
* DISHTINY evolves transition-relevant strategies within a substantially predefined hierarchy.
* Successive hierarchy can impose resource, population-size, generation-time, and coordination costs.
* Reversions and hierarchical losses prevent an irreversible ladder interpretation.
* Prior theory finds evidence for an upward or downward bias in hierarchical transitions inconclusive.

### Underexplored

* Controlled second-transition experiments that manipulate products of a completed first transition.
* Branching comparisons across several later regime-transition classes.
* Resource-normalized positive and negative effects of the same completed transition.
* Endogenous creation of a later hereditary or group-forming channel in artificial systems whose substrate did not expose it in advance.

### Potentially Novel

No mechanism or law passed the novelty firewall. The transition-to-transition causal assay is a sharper application of established evolvability and dependent-transition questions, not itself a scientific discovery.

### Unknown

* Whether any transition product reliably increases access to more than one distinct later regime transition.
* Whether the net direction of transition feedback changes with hierarchical depth.
* Whether a non-predefined, recursively generated sequence of transitions is achievable in one system.

## 15. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

No specified property (P) was found for which evidence supports the general implication

\[
P\text{ produced by }T_i
\Rightarrow
\text{greater access to later regime transitions}.
\]

Information capacity, bottlenecks, communication, modularity, developmental machinery, and ecological construction each have counterexamples or only target-specific support. `HYPOTHESES.md` remains unchanged.

## 16. Highest-information next question

Can replay or ablation experiments show that a product evolved during a completed first transition, rather than a designer-predefined channel, increases resource-normalized access to more than one distinct subsequent evolutionary regime?
