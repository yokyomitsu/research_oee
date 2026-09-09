# Q006 — Accessible outcomes versus generative capacity

2026-09-07. Exactly one theoretical research pass. This pass corrects prior-art scope before asking whether “new generative capacity” means anything stronger than a larger adjacent possible or greater evolvability. No implementation and no complete OEE theory.

**Result:** The broad idea that evolution expands its adjacent possible is established prior art. The workspace transitions \(\Omega_t\to\Omega_{t+1}\) and \(\mathcal O_t\to\mathcal O_{t+1}\) substantially overlap Kauffman’s adjacent possible, OEE state/meta-model distinctions, evolving genotype–phenotype maps, evolving genetic operators, developmental-system evolution, and major-transition accounts of new inheritance channels. They should not be retained as independent novelty claims.

The narrower distinction is defensible only as an analytical separation between:

1. **outcome expansion:** more or different heritable outcomes are reachable under an already specified generator; and
2. **generator/map change:** the variation, development, recombination, inheritance, or constructional organization itself changes, altering future accessibility.

Existing theory already calls the second family **evolution of evolvability**, **evolvable genetic operators**, **evolution of the genotype–phenotype map**, **facilitated variation**, **modularity**, **evolutionary capacitance**, **major evolutionary transitions**, or—within OEE—**door-opening states**, **non-additive compositional systems**, and **transdomain bridges**. Reuse and recursion add important empirical structure but do not yet supply a unified observer-independent criterion. **Hypothesis decision: NO HYPOTHESIS JUSTIFIED.** The outcome is **Fragmented prior art**, not a surviving new mechanism.

## 1. Prior-art correction

### Adjacent possible and expanding state spaces

**Fact:** Kauffman’s adjacent possible is the set of possibilities available from the current actual through a specified kind of one-step process. Realizing an adjacent possibility changes the actual and thereby changes what is adjacent next. The concept is explicitly path-dependent and concerns the expansion of a possibility space, not merely movement through a fixed list. [Kauffman 2000, as described by Griesemer 2023](https://doi.org/10.1093/phisci/pyad018)

Formal models already implement expansion. Loreto et al.’s urn-with-triggering model adds new possibilities when a previously unseen element is realized; its generalization produces waves of novelty by changing accessibility and collective exploration. This is a model of an expanding adjacent possible, not a new “generator” concept. [Loreto et al. 2017](https://doi.org/10.1371/journal.pone.0179303)

### OEE state/meta-model and door-opening states

**Fact:** Banzhaf et al. distinguish novelty relative to a model and meta-model. Taylor distinguishes exploratory, expansive, and transformational open-endedness and explicitly identifies two processes: ongoing exploration and the discovery of states that open an expanded phenotype space. The paper further discusses non-additive compositional complexity and transdomain bridges as ways a fixed genetic space can support transformational novelty. [Banzhaf et al. 2016](https://doi.org/10.1162/ARTL_a_00210), [Taylor 2019](https://arxiv.org/abs/1806.01883)

Taylor also maps routes to altered evolutionary process: evolving genetic operators, changing the genotype–phenotype map, and organism-mediated environmental changes. The paper explicitly warns that a larger genome need not specify new traits, and that the relevant issue is the capacity of added genes or building blocks to specify new traits. [Taylor 2019, §§2–4](https://arxiv.org/abs/1806.01883)

**Interpretation:**

- \(\Omega_t\to\Omega_{t+1}\) is substantially equivalent to adjacent-possible/state-space expansion when \(\Omega\) denotes accessible outcomes.
- \(\mathcal O_t\to\mathcal O_{t+1}\) is substantially equivalent to evolving the model, genotype–phenotype map, genetic operators, inheritance system, or constructional organization when \(\mathcal O\) denotes those mechanisms.
- The workspace notation is useful bookkeeping but is not a new theoretical distinction.

The notation is also potentially stronger than ordinary adjacent-possible language only if \(\mathcal O\) is specified as a heritable causal organization whose changes alter the future transition law. Without that specification it merely renames model-relative state-space expansion. No such stronger status is adopted here.

## 2. Accessible outcomes versus generative capacity

Cardinality is insufficient:

\[
|\mathcal A_{t+1}|>|\mathcal A_t|
\]

may mean only that one existing mechanism exposes many nearby variants. A larger set does not establish a new constructional operation, a new character class, or recursive future innovation.

A more precise existing distinction is between a transition kernel/map and its outputs. Let \(M_t\) summarize the heritable variation, developmental, recombination, and constructional processes, and let \(E_t\) describe the relevant environment/context. Then:

\[
\mathcal A_t(x)=\operatorname{Reach}_{M_t,E_t,H,S}(x)
\]

is a set or distribution of accessible heritable outcomes under a specified assay. Two changes can occur:

\[
M_t\text{ fixed},\quad \mathcal A_t(x)\text{ expands};
\]

or

\[
M_t\to M_{t+1},\quad \mathcal A_{t+1}(x)\text{ changes because the generator/map changes}.
\]

The first is outcome expansion. The second is a change in evolvability or in the genotype–phenotype/developmental/inheritance map. Even the second need not create a new qualitative dimension: a mutation-rate modifier can make existing variants more frequent, and a developmental change can redistribute probability within an existing phenotype space.

**Conclusion:** “new means of generating alternatives” is a meaningful operational distinction from “more alternatives,” but existing theory already places it under evolution of evolvability and evolving representations. It is not a new OEE concept. A further distinction between a changed map and a changed *class of generators* remains possible, but no accepted criterion was found that makes that distinction observer-independent.

## 3. Evolvability

**Fact:** Evolvability is used in several related senses, including the capacity to generate heritable phenotypic variation, the ability of a population to respond to selection, and the stronger ability to acquire innovative properties. Wagner explicitly distinguishes change in an existing activity from innovative evolution such as a new catalytic activity. [Wagner 2005](https://doi.org/10.1016/j.febslet.2005.01.063), [Wagner & Altenberg 1996](https://doi.org/10.1111/j.1558-5646.1996.tb02339.x)

The evolution of evolvability literature already studies second-order changes. Examples include:

- mutation-rate and recombination modifiers;
- evolvable genetic operators and copying/error-correction systems;
- evolving genotype–phenotype maps;
- regulatory networks that become more likely to generate adaptive variants;
- modularity and neutral networks that preserve current function while exposing alternatives;
- capacitance mechanisms that store or release cryptic variation.

Crombach and Hogeweg explicitly model gene-regulatory networks evolving to generate adaptive mutants while retaining robustness. [Crombach & Hogeweg 2008](https://doi.org/10.1371/journal.pcbi.1000112) Rutherford and Lindquist’s Hsp90 experiment gives a biological example of buffered variation becoming expressed and subsequently selectable. [Rutherford & Lindquist 1998](https://doi.org/10.1038/24550)

These mechanisms answer the provisional first-order/second-order question in existing language:

\[
\text{new outcome under }M
\quad\text{versus}\quad
\text{evolved }M\text{ or evolved }GP\text{ map}.
\]

They do not answer whether a map change creates a new reusable generator rather than a better distribution over an old outcome space. That is a limitation of the current target, not evidence for a new term.

## 4. Reuse

**Fact:** Reuse of conserved components is a central explanation in facilitated variation, evo-devo, and modularity. Shared regulatory modules can be redeployed in new developmental and ecological contexts; toolkit genes and conserved regulatory networks can participate in multiple phenotypes. [Gerhart & Kirschner 1997](https://doi.org/10.1073/pnas.94.16.8420), [Debat & David 2001](https://doi.org/10.1016/S0169-5347(01)02180-8), [Wagner 2014](https://doi.org/10.23943/princeton/9780691156460.001.0001)

The idea

\[
g\to\{f_1,f_2,\ldots,f_n\}
\]

is therefore close to established **modularity**, **developmental toolkit**, **regulatory redeployment**, **co-option**, and **exaptation** literatures. A structure that can be reused across distinct contexts is more than a merely necessary component, provided the reuse is heritable and developmentally reconstructible.

But reuse is not sufficient for generative capacity in the stronger sense:

- several uses may be variants of one function rather than distinct capacities;
- reuse may be available only through an observer-supplied environment or intervention;
- a component may be reusable in principle but never reach its alternative contexts;
- a component may be reused twice and then become specialized or entrenched;
- a single exaptation can create a new function without changing future generative scaling.

Reuse is thus evidence for a mechanism of access, not a criterion for OEE or recursive generativity.

## 5. Compositionality

**Fact:** Compositionality is already explicit in OEE theory and in evolutionary accounts of modular construction. Taylor identifies non-additive compositional systems as a route to expansive or transformational open-endedness even when genetic space is fixed. Wimsatt’s combinatorial entrenchment describes standardized parts as a constructional alphabet from which many adaptive forms can be assembled. [Taylor 2019](https://arxiv.org/abs/1806.01883), [Wimsatt 2013](https://doi.org/10.7551/mitpress/9780262019552.003.0004)

This is prior art for:

\[
p_i\circ p_j
\]

creating higher-level constructions whose number can exceed additive growth. Modular regulatory systems, developmental modules, protein domains, and digital-organism building blocks are empirical/theoretical examples of this general pattern. [Clune et al. 2013](https://doi.org/10.1371/journal.pone.0052258), [Soyer 2012](https://doi.org/10.1186/1471-2148-12-136)

Compositionality is not necessary for every form of novelty. A new ecological interaction, biochemical activity, or developmental transformation can be novel without an obviously combinatorial construction grammar. It is also not sufficient for future OEE: a fixed combinatorial system can have a vast or unbounded formal language while viable, heritable, selectable constructions remain finite or quickly exhausted.

Thus “new compositional primitive” is a useful descriptive phrase, but its theoretical content is already distributed across modularity, constructional selection, combinatorial entrenchment, GP-map evolution, and Taylor’s non-additive compositional systems.

## 6. Generative entrenchment

**Fact:** Generative entrenchment measures how many downstream developmental features depend on an upstream feature. It describes depth or breadth of dependence, not the number of distinct future innovations that could use the feature. [Wimsatt & Schank 1986](https://doi.org/10.1086/psaprocbienmeetp.1986.2.192789)

The proposed distinction can therefore be stated as a difference between two relation types:

\[
D(g)=\text{downstream dependence on }g,
\]

\[
B(g)=\text{distinct future capacities made accessible through }g.
\]

But \(B(g)\) is not an established metric equivalent to one accepted literature term. It overlaps:

- phenotype evolvability: accessible alternative phenotypes;
- developmental bias: distribution of generated variants;
- modularity: reduced interference and redeployment;
- combinatorial entrenchment: many constructions from standardized parts;
- potentiation: increased access to a specified later outcome;
- novelty/innovation: new characters/functions and their ecological success.

The separation survives conceptually: a deeply entrenched component may support one conserved function, while a weakly entrenched module may have many possible redeployments. Yet “generative branching” is not established as a representation-independent quantity. A branch count depends on what outcomes are treated as qualitatively distinct and on how far into the future the assay extends.

Entrenchment and branching can also coexist in one history. A module may become more indispensable after many descendants depend on it while also serving as a reusable substrate for additional forms. Depth and branching are not mutually exclusive and should not be combined into a single scalar without a justified ontology.

## 7. New operators / generators

The operand/operator analogy maps onto known evolutionary mechanisms but does not create a new category.

### Operand-like changes

\[
F(x)\to F(y)
\]

These include changes in the value or structure acted upon by an existing developmental, regulatory, or constructional process.

### Operator/map-like changes

\[
F\to G
\]

These include changes to:

- mutation and recombination processes;
- genome organization and gene duplication;
- regulatory/developmental maps;
- inheritance channels;
- ecological scaffolding and niche construction;
- the rules by which modules are redeployed or combined.

Modifier theory and evolution-of-evolvability work already study heritable variants that alter mutation rates, recombination, transmission, or the distribution of fitness effects. Evo-devo studies evolution of the developmental map. Major-transition theory studies new inheritance channels, new levels of individuality, and changes in how heritable information is stored and transmitted. [Altenberg 1994](https://doi.org/10.1007/978-1-4613-0259-5_3), [Maynard Smith & Szathmáry 1995](https://global.oup.com/academic/product/the-major-transitions-in-evolution-9780198502944), [Jablonka & Lamb 2006](https://doi.org/10.1016/j.jtbi.2005.08.038)

The major-transition literature is especially relevant because some transitions change the evolutionary process itself: they establish new units of selection or new channels and fidelity of inheritance. This is stronger than merely exposing another phenotype, but it is a recognized class of evolutionary transition, not an unrecognized “generator” principle. [Szathmáry 2015](https://doi.org/10.1073/pnas.1421398112)

“New generator of future dimensions” is therefore either:

1. a restatement of evolution of evolvability/GP maps/operators;
2. a major transition if the inheritance or individuality regime changes; or
3. a metaphor whose content depends on a chosen representation.

No independent hypothesis is justified.

## 8. Recursive generativity

### Prior art

The broad recursive pattern

\[
g_1\to g_2\to g_3\to\cdots
\]

already appears in several literatures:

- Kauffman’s adjacent possible: actualization changes the next adjacent possible;
- Taylor’s door-opening states and expansive/transformational OEE;
- non-additive compositional systems and transdomain bridges;
- major transitions that create new units or inheritance channels;
- evolutionary change in evolvability and developmental maps;
- recursive developmental organization and cumulative cultural/technological innovation.

Frank explicitly describes evolutionary innovation as a hierarchy of recursive processes in which innovations can alter the processes generating and transmitting later innovations. This is close semantic prior art, although it is a conceptual synthesis rather than a universal operational criterion. [Frank 2016](https://doi.org/10.12688/f1000research.9568.1)

### Limits

Recursive access does not imply recursive *evolution of generators*. A fixed grammar can generate arbitrarily many strings; a fixed adjacent-possible rule can keep adding nodes; a fixed developmental map can support many compositions. In each case, the output space expands while the generative mechanism remains unchanged.

Conversely, a generator can evolve once and then become closed. The fact that a new operator supports many outcomes does not establish that any later outcome can itself change the operator or generate a new class of operators.

The distinction between one-shot and recursive generativity is therefore useful as a question about the trajectory of the mechanism, but it is not a new established formal category and cannot be adopted without specifying inheritance, generator identity, and equivalence of later capacities.

## 9. Counterfactual formulation

The proposed comparison

\[
\Delta_g=\mathcal F(g)\setminus\mathcal F(\neg g)
\]

is useful only after fixing:

- the variation and developmental law;
- the environmental and ecological boundary;
- the hereditary unit and reconstruction process;
- the time horizon and probability threshold;
- the viability/selection assay;
- the equivalence relation over outcomes;
- whether engineered or only endogenous paths count.

With those fixed, one can ask whether a component changes the reachable distribution, first-passage probabilities, mutational neighborhoods, or future transition law. Existing reachability, GP-map, neutral-network, potentiation, and causal-intervention tools can support such target-relative comparisons.

The size of \(\Delta_g\) is not enough. A large set can contain only near-duplicates; a small set can contain a new character identity; and a new generator can change probabilities without adding any state to the current phenotype set. Internal structure—functional diversity, reuse, compositional depth, or later map changes—may be informative, but each requires a specified equivalence relation and remains vulnerable to observer choice.

**Interpretation:** Counterfactual generativity is a useful research assay, not a solved intrinsic criterion. It should not be promoted to a new OEE definition.

## 10. Observer dependence

The observer problem remains central. “Qualitatively distinct,” “new dimension,” “reusable,” and “generator” require an equivalence relation over outcomes or transformations.

Possible grounding constraints include:

- distinct causal effects on organismal maintenance;
- distinct heritable operations or inheritance channels;
- distinct organism–environment interaction structures;
- distinct developmental reconstruction mechanisms;
- distinct selectable units or levels of individuality.

These constraints reduce arbitrary labeling but do not select one universal ontology. A protein domain may be a reusable primitive under a molecular-function description and merely one constrained sequence under another. A developmental module may support several morphological characters while preserving one character-identity network. A new phenotype may be distinct morphologically but not introduce a new inherited operation.

Predictive equivalence, causal-state methods, and behavioral coarse-graining can preserve specified future distributions while eliminating some distinctions. They do not determine which future outcomes are evolutionarily meaningful without supplied observables, interventions, environments, or beneficiaries. This repeats Q003 rather than solving it.

## 11. Strong counterexamples

### A — Reuse without increased long-term evolvability

A conserved component can be redeployed in many contexts that are already represented by the developmental or ecological system, while the system's mutation/developmental map gains no new future operation. Reuse shows functional versatility, not necessarily an expanding future generator.

### B — Compositional modularity followed by stagnation

A modular system may support many formal combinations, but most may be nonviable, nonheritable, unreachable under endogenous variation, or selectively neutral. Digital-organism and modularity studies also show that complexity can facilitate some changes while constraining others. Combinatorial capacity is not realized OEE.

### C — Dramatic new function without further opportunities

A one-off mutation can produce an adaptive function and then enter an absorbing or highly constrained region of the genotype–phenotype map. This defeats the implication:

\[
\text{new function}\Rightarrow\text{new future generator}.
\]

### D — Large expanding state space with fixed generator

Urn-with-triggering and adjacent-possible models can expand the accessible set whenever a new element is realized while keeping the rule for generating new elements fixed. A large or continually expanding adjacent possible therefore does not prove that the qualitative generative mechanism itself evolves. [Loreto et al. 2017](https://doi.org/10.1371/journal.pone.0179303)

### E — Deep entrenchment that restricts future novelty

Generative entrenchment can make an upstream feature difficult to modify because many downstream features depend upon it. High downstream dependence can therefore reduce viable evolutionary routes even if the feature is “generative” in the developmental sense.

### F — Restrictive dependency later reused

CNE can increase dependence and reduce independence, after which an altered interaction or buffered variation can be exapted or redeployed. The same history can contain entrenchment followed by reuse. The categories are temporal/analytic distinctions, not mutually exclusive lineage types.

### G — Adjacent possible expansion with fixed qualitative mechanism

An evolving population may continually realize new nodes because the current rule adds or exposes adjacent nodes, while all future generation still uses the same fixed grammar, mutation operator, and constructional alphabet. This is expanding adjacent possible without recursive evolution of generative mechanism.

### H — Apparent new generator under observer-selected tasks

A modifier may increase arrival rates for one task, environment, or phenotype class. Under a different task family it may have no benefit or may reduce evolvability. Task-relative evolvability does not establish an intrinsic generator of future dimensions.

## 12. Remaining gap

The broad question is not open: existing theory already distinguishes adjacent-possible expansion, accessible phenotype space, evolution of evolvability, evolving GP maps/operators, and some major transitions that alter inheritance or individuality.

The narrow remaining gap is:

> Can a specified heritable organization be shown to change not merely the number or probability of accessible outcomes, but the class of endogenous, developmentally reconstructible transformations that can generate later selectable capacities—without defining “class,” “qualitative,” or “generator” by the observer’s preferred future examples?

This gap has two possible resolutions:

1. identify a representation-robust causal equivalence under which generator changes are objective; or
2. show that no such criterion is available without fixing the system boundary, inheritance regime, environment, and outcome ontology.

The reviewed literature does not settle either. It does show that any solution will be a synthesis of existing concepts, not a rediscovery of adjacent possible or evolvability.

## 13. Known / Underexplored / Potentially Novel / Unknown

### Known / ESTABLISHED within cited scopes

- Kauffman’s adjacent possible and formal expansion models already describe how realized outcomes expose later outcomes.
- OEE theory already distinguishes exploration from door-opening states, and discusses expansive/transformational novelty, non-additive compositional systems, and transdomain bridges.
- \(\Omega_t\to\Omega_{t+1}\) overlaps accessible state-space/adjacent-possible expansion; \(\mathcal O_t\to\mathcal O_{t+1}\) overlaps evolving maps, operators, representations, and inheritance systems.
- Evolvability already includes changes in the mechanisms that generate or transmit heritable variation.
- Reuse, modularity, developmental toolkits, regulatory redeployment, exaptation, and combinatorial construction are established prior art.
- Major-transition theory already addresses changes in evolutionary individuality, inheritance channels, and the evolutionary process itself.
- Expanding adjacent possible does not imply that the qualitative generator changes.

### Underexplored / PARTIALLY EXPLORED

- A common assay linking altered generator/map structure to nontrivial future capacity while preserving cryptic potential.
- A principled separation between downstream entrenchment and future-capacity branching.
- Prospective detection of recursive generator change without selecting the later target in hindsight.

### Potentially Novel

No candidate terminology is retained. “New generator,” “recursive generativity,” “generative branching,” and “new compositional primitive” substantially overlap established work and remain observer-sensitive unless further specified.

### Unknown

- Whether a representation-robust criterion can distinguish map/operator evolution from mere output expansion.
- Whether such a criterion is necessary for a strong form of OEE.
- Whether recursive generativity is an objective property of biological organization or a target-relative summary of repeated innovation.

## 14. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED.**

The primary target has **Fragmented prior art** rather than a single sufficient theory. The distinction between accessible outcomes and changed generative mechanisms is already represented by adjacent possible versus evolving evolvability/GP maps/operators, and its stronger versions are covered in part by compositional OEE, facilitated variation, modularity, evolutionary capacitance, and major-transition theory. The remaining lack of a unified criterion does not pass the novelty firewall: naming it “recursive generativity,” “generative branching,” or “new generator” would be a relabeling or synthesis, not a grounded new hypothesis.

The corrected boundary is:

\[
\text{more accessible outcomes}
\neq
\text{changed generator/map},
\]

but also:

\[
\text{changed generator/map}
\neq
\text{new qualitative evolutionary dimension},
\]

and:

\[
\text{expanding adjacent possible}
\neq
\text{recursive evolution of generative mechanisms}.
\]

No deep-learning comparison was needed: evolutionary theory already supplies the relevant abstract distinctions, and importing representation-learning terminology would not improve the prior-art boundary.

## 15. Highest-information next question

**Can a heritable change in a genotype–phenotype/developmental/inheritance map be identified prospectively as changing the class of endogenous selectable transformations, rather than merely changing the number or probability of outcomes under a fixed observer-defined assay?**

### Core references

- [Kauffman 2000; adjacent possible summarized in Griesemer 2023](https://doi.org/10.1093/phisci/pyad018)
- [Loreto et al. 2017 — Waves of novelties in the expansion into the adjacent possible](https://doi.org/10.1371/journal.pone.0179303)
- [Banzhaf et al. 2016 — Defining and simulating open-ended novelty](https://doi.org/10.1162/ARTL_a_00210)
- [Taylor 2019 — Evolutionary Innovations and Where to Find Them](https://arxiv.org/abs/1806.01883)
- [Wagner & Altenberg 1996 — Complex Adaptations and the Evolution of Evolvability](https://doi.org/10.1111/j.1558-5646.1996.tb02339.x)
- [Wagner 2005 — Robustness, Evolvability, and Neutrality](https://doi.org/10.1016/j.febslet.2005.01.063)
- [Crombach & Hogeweg 2008 — Evolution of Evolvability in Gene Regulatory Networks](https://doi.org/10.1371/journal.pcbi.1000112)
- [Rutherford & Lindquist 1998 — Hsp90 as a Capacitor for Morphological Evolution](https://doi.org/10.1038/24550)
- [Gerhart & Kirschner 1997 — Cells, Embryos, and Evolution](https://doi.org/10.1073/pnas.94.16.8420)
- [Wimsatt & Schank 1986 — Generative Entrenchment and Evolution](https://doi.org/10.1086/psaprocbienmeetp.1986.2.192789)
- [Wimsatt 2013 — Entrenchment and Scaffolding](https://doi.org/10.7551/mitpress/9780262019552.003.0004)
- [Erwin 2021 — A Conceptual Framework of Evolutionary Novelty and Innovation](https://doi.org/10.1111/brv.12643)
- [Szathmáry 2015 — Toward Major Evolutionary Transitions Theory 2.0](https://doi.org/10.1073/pnas.1421398112)
- [Frank 2016 — Recursive Processes of Evolutionary Innovation](https://doi.org/10.12688/f1000research.9568.1)
