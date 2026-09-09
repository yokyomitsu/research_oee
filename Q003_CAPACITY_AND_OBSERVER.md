# Q003 — Capacity for novelty and the observer

2026-09-07. Exactly one theoretical research pass, following [Q002](Q002_CLOSURE.md). No implementation or new OEE hypothesis.

**Result / Interpretation:** Realized novelty is evidence about a history; generative capacity concerns possible continuations under specified dynamics. Existing theory makes the latter precise for specified outcomes. Causal and evolutionary accounts constrain what counts as significant, but the literature examined does not supply a unique, observer-independent definition of all future evolutionary possibilities. Conditional objectivity is available; a universal intrinsic OEE criterion remains unresolved.

## 1. Problem statement

Let $\Gamma_t=(X_0,\ldots,X_t)$ be the observed history. Absence of an outcome class $N$ from this history is a statement about realization. Inability to generate $N$ quantifies over admissible future continuations. These statements have different logical strength.

**Fact / deduction:** Finite non-detection alone cannot generally distinguish a zero-probability transition from an arbitrarily rare transition. Both models can assign positive probability to the same finite record. A later occurrence establishes generability from the earlier starting conditions under that protocol; it does not establish indefinite innovation, or continued accessibility from every subsequent state.

Repeated assays can bound probabilities under assumptions. For example, zero successes in $m$ independent, identically distributed replays of a fixed duration gives the one-sided 95% binomial upper confidence bound $q\leq1-0.05^{1/m}$. This elementary calculation bounds the specified assay's success probability, not the probability of eventual novelty across all futures. A single evolving population does not automatically provide independent trials.

**Interpretation:** “Not observed,” “improbable within this horizon,” and “excluded by these dynamics” should replace an undifferentiated diagnosis of closure.

## 2. Existing formal distinctions

**Fact:** Evolvability already distinguishes existing phenotype from capacity to produce variants. Wagner distinguishes the alternative phenotypes available around a genotype from those accessible across a phenotype's neutral network. Neutral movement can change access to alternatives while preserving the focal phenotype. This is an existing distinction, not a new capacity variable. RNA secondary structure in that analysis is a specified phenotype proxy. [Wagner 2008](https://pmc.ncbi.nlm.nih.gov/articles/PMC2562401/)

The following separates objects that the proposed list partly mixes:

| Object | What it can specify | What it leaves out |
|---|---|---|
| Genotype or current phenotype | Local mutational alternatives under a specified mapping | Population supply, competition, ecological context, longer paths |
| Population/genotype distribution | Standing variation, frequencies, mutation supply | Future outcomes without reproduction, variation, and environmental dynamics |
| Genotype–phenotype mapping | Which phenotypes variants express in specified conditions | Their arrival rates and selective establishment |
| Transition law plus current system–environment state | A distribution over future trajectories, if the state is sufficient | Which outcomes qualify as novelty |
| Reachable-state graph | Possible transitions and paths | Rates, meaningful labels, unless supplied separately |
| Interaction network | Relations among current entities | Hidden capacities and responses to changed partners unless modeled |
| History | Which outcomes have already occurred; path-dependent information absent from a reduced state | Unobserved possibilities by itself |
| Description/coarse-graining | Which differences an analysis records | A guarantee that discarded differences are evolutionarily irrelevant |

**Interpretation:** These are complementary levels, not competing locations of a single intrinsic scalar. For a complete Markov description, physical future probabilities depend on the present state and law; historical novelty still requires a historical baseline. With incomplete observations, history can contain predictive information missing from the present description.

The environment must either be included or governed by an explicit boundary protocol. Capacity under a changed laboratory environment is a different conditional claim from capacity under the original autonomous dynamics. A system with deterministic dynamics and an exactly specified complete state has one future trajectory; multiple counterfactual futures require a stated source of variation or uncertainty.

## 3. Reachability

**Fact / existing formalism:** For a discrete time-homogeneous Markov model with complete state $x$ and transition kernel $K$, standard positive-probability reachability and finite-horizon hitting probability are:

$$
\mathcal R_K^+(x)=\{y:\exists n\geq0,\ K^n(x,y)>0\},
\qquad
q_N(x,T)=\Pr_x(\tau_N\leq T).
$$

Here $\tau_N$ is the first hitting time of a specified target set. Probabilistic verification distinguishes probability-zero/one reachability, quantitative probabilities, bounded horizons, and temporal path properties. These are existing tools for capacity questions, not OEE definitions. [Forejt et al. 2011, §§4–6](https://www.prismmodelchecker.org/papers/sfm11.pdf)

**Fact / deductions under stated assumptions:**

- A complete finite transition graph can establish that no path reaches $N$. An invariant set $I$ containing $x$, disjoint from $N$, and satisfying $K(y,I)=1$ for every $y\in I$ establishes probability-zero escape to $N$. Such proofs need structural knowledge beyond the observed history.
- An exact full-state recurrence, together with a known autonomous deterministic law, fixes the subsequent periodic orbit. Recurrence of a phenotype or a stochastic state does not do this.
- A finite irreducible Markov chain reaches each state almost surely, although waiting times can be enormous. Aperiodicity concerns convergence of distributions, not whether states can be reached. Infinite irreducible chains need not have the same almost-sure hitting property. None of these conditions identifies adaptive novelty.
- In continuous spaces, an individual point can have probability zero despite lying in the support. Logical admissibility, support reachability, and positive probability of a measurable target event must therefore be distinguished.

For huge finite systems, exact analysis can be computationally impractical without becoming undecidable merely because of size. Sound overapproximations and invariants can prove exclusion without listing every state; an apparent path in an overapproximation can be spurious. A witnessed path proves a possibility under the modeled conditions, whereas unsuccessful sampling is not an exclusion proof.

**Fact:** Day studies a stronger limitation for computable evolution over unbounded population types. Decidability of which states ever occur is connected to existence of a computable progressive recoding. Known update rules therefore need not provide a general decision procedure for eventual occurrence/non-occurrence. “Progressive” here is a formal coding property, not necessarily increasing fitness or biological complexity. The result does not prohibit specific predictions or make every finite-state problem undecidable. [Day 2012, theorem and limitations](https://arxiv.org/pdf/1110.2982)

**Interpretation:** Projecting reachability through $\phi:X\rightarrow Z$ gives reachable descriptions $\phi(\mathcal R_K^+(x))$. It does not make those descriptions functional, adaptive, or novel. Adaptive establishment and heredity may be properties of trajectories and lineages, requiring path events or augmented states rather than a target defined by instantaneous morphology.

Thus finite evidence can support a closure conclusion only conditional on additional constraints that exclude alternatives. Closure relative to a specified $N$ is also weaker than exhaustion of every possible meaningful novelty class.

## 4. Observer dependence

**Fact:** OEE's descriptive dependence is explicit in model-relative novelty classifications: exploratory, expansive, and transformational novelty depend on the reference model. This is distinct from whether generation, evaluation, and reproduction operate internally to the evolving system. Internally determined selection does not by itself determine an observer's phenotype vocabulary. [Taylor 2019, §§2–4](https://www.tim-taylor.com/papers/taylor2019evolutionary.preprint.pdf)

MODES makes component identity, historical baseline, and persistence duration explicit. Its optional genome filter measures fitness effects of null substitutions; it is an operational attempt to remove noise. The paper acknowledges epistasis and residual distinctions between functionally equivalent genomes. A causal assay therefore improves a metric without making it a complete account of future potential. [Dolson et al. 2019, §3.1](https://cse.msu.edu/~dolsonem/pdfs/modes_paper.pdf)

**Fact:** Computational mechanics defines causal states by equality of conditional distributions of future observations given past observations. Its minimality and uniqueness results concern a specified stochastic process and observed variables. “Causal state” here denotes predictive equivalence; it is not automatically equivalence under arbitrary replacement interventions. [Shalizi & Crutchfield 2001](https://arxiv.org/pdf/cond-mat/9907176)

Shalizi and Moore address the objectivity question directly: initial observables reflect measurement choices, while dynamics constrain a sufficient predictive refinement. Their account supplies objective restrictions after that choice, not a unique initial choice of what should be predicted. [Shalizi & Moore, 2003 preprint / 2025 publication, §§III, VI](https://arxiv.org/pdf/cond-mat/0303625)

**Interpretation:** Observer dependence is not equivalent to arbitrary labeling. Two analysts can obtain reproducible, constrained answers after specifying the same boundary, outcomes, and interventions. Mere invertible relabeling need not change an answer; losing distinctions through coarse-graining can. A projected process can also lose the Markov property, hiding relevant memory.

No reviewed framework establishes that every reasonable description must agree about OEE. Nor does their dependence on observables prove that an intrinsic account is impossible.

## 5. Function and endogenous significance

**Fact / distinctions among existing accounts:**

| Sense of function | Grounding | Limitation for future novelty |
|---|---|---|
| Observer-assigned | Performance on a chosen task or assay | Fixes the task vocabulary externally |
| Selected-effect | An effect helps explain the trait's presence through its selection history | A newly available effect can precede selection for that effect |
| Causal-role | Contribution to a specified capacity of a containing system | Neither historical selection nor reproductive benefit follows |
| Ecological | Effects or relational roles among organisms and environmental processes | Network similarity is not automatically identical future dynamics |
| Reproductive consequence | Contextual effect on survival/reproduction or lineage growth | A fitness difference need not identify a new kind of function |
| Organism-internal | Contribution to maintaining the organization that sustains the component | Requires an account of the organism, organization, and maintenance |

The historical/causal-role distinction is developed in [Wright 1973](https://mechanism.ucsd.edu/~bill/teaching/w10/wright.functions.%201973.pdf) and [Cummins 1975](https://joelvelasco.net/teaching/3334/cummins75-functional_analysis.pdf). An explicit organizational proposal grounds function in contribution to, and dependence on, differentiated self-maintaining organization; it is one theoretical account, not an agreed universal definition. [Mossio, Saborido & Moreno 2009](https://www.ias-research.net/wp-content/uploads/2019/02/Mossio_25592036.pdf)

Ecological role has existing relational formalizations. For example, trophic regular equivalence compares organisms by the roles of their interaction partners. It does not prove interchangeability under mutation, environmental change, or unobserved future interactions. [Luczkovich et al. 2003](https://pubmed.ncbi.nlm.nih.gov/12468282/)

**Interpretation:** The proposed replacement test has substantial prior art, but “relevant endogenous causal difference” still requires specification. Equal current reproductive effects can conceal different descendant possibilities. Conversely, requiring equality of every microscopic consequence preserves irrelevant noise or chaotic differences. A harmful causal effect is not adaptive novelty. An experimental replacement can reveal consequences without showing that endogenous evolution can generate the replacement.

Functional novelty need not be arbitrarily assigned: historical selection and causal interventions offer empirical constraints. They do not select one universal vocabulary. OEE does not require function under every definition; Q002's dynamical definitions provide a counterexample. An adaptive-functional claim, however, needs evidence beyond a new physical state.

## 6. Generation vs accessibility vs maintenance

**Interpretation grounded in the following studies:** The suggested categories are useful distinctions, but neither a universal sequence nor independent summands.

| Question | Appropriate distinction |
|---|---|
| Is the configuration consistent with the model? | Logical admissibility |
| Is there an allowed route from the specified starting conditions? | Dynamical reachability |
| Does that route/event have positive probability? | Probabilistic reachability, with the measure specified |
| Is arrival plausible on the stated horizon? | First-passage probability/time and mutational supply |
| Can evolutionary dynamics traverse the route? | Adaptive accessibility under a stated mutation–selection–drift regime |
| Can the generated entity operate or survive? | Viability |
| Can its relevant differences be transmitted? | Heritability |
| Can selection amplify the differences in this context? | Selectability/establishment |
| Do the entity, lineage, or function remain? | Persistence, specifying object and duration |
| Does it change subsequent access to other outcomes? | Further generativity/evolvability, a separate comparison |

**Fact:** Genotype–phenotype bias changes arrival probabilities. Schaper and Louis show that frequently generated phenotypes can dominate rarer, fitter alternatives; possible and favored-if-present need not mean likely to appear. Their first-arrival analysis supplies a timescale concept rather than a universal probability cutoff for OEE. [Schaper & Louis 2014](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0086635)

Weinreich et al. distinguish selectable paths in a restricted five-mutation landscape from the complete set of mutation orders. Their accessibility restriction is model-dependent; it is not proof that all other routes are physically impossible. [Weinreich et al. 2006](https://pubmed.ncbi.nlm.nih.gov/16601193/)

Generation and establishment also differ. A reconstructed citrate-use innovation gave the ancestral LTEE background a small measured benefit. Leon et al. interpret its early failure to establish in terms of competition with larger-effect beneficial mutations, and document backgrounds where the same innovation was detrimental. This separates biochemical capability, contextual benefit, and successful spread. The reconstruction was engineered, so it does not alone measure spontaneous arrival rates. [Leon et al. 2018](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1007348)

Maintenance of every intermediate is unnecessary: stochastic tunneling permits an advantageous descendant to arise through a neutral or deleterious intermediate without that intermediate fixing. [Iwasa, Michor & Nowak 2004](https://pmc.ncbi.nlm.nih.gov/articles/PMC1470783/)

**Interpretation:** Heritability is not fixation; persistence is not proof of selection; transient structures can matter through descendants. No single timescale or probability threshold found in the reviewed OEE work makes accessibility universally meaningful. Thresholds can nevertheless be declared and empirically compared.

The proposed sum “openness = capacity + accessibility + endogenous significance + heritability/persistence” is **not retained as an equation or sufficient definition**. It mixes modal properties, probabilities, causal criteria, and lineage outcomes. They help diagnose a specified heritable adaptive novelty, but all can hold for one innovation followed by permanent closure. Whether innovations alter later potential requires an additional comparison; requiring every innovation to do so is not established.

## 7. Counterexamples

Evidence strengths are separated deliberately.

| Case | Evidence | What it defeats—and what it does not show |
|---|---|---|
| **A: long absence, later realization** | Aerobic citrate use arose after roughly 31,500 LTEE generations. Replay experiments found increased propensity in later historical backgrounds. [Blount, Borland & Lenski 2008](https://doi.org/10.1073/pnas.0803151105) | Long non-detection is not a closure proof. Historical propensity changed; this does not show constant ancestral probability. |
| **A: cryptic capacity** | RNA populations accumulated variation with little measured change in the original phenotype, then adapted more rapidly under a new substrate condition. [Hayden, Ferrada & Wagner 2011](https://www.nature.com/articles/nature10083) | Current phenotype can hide potential. The changed environment is part of the capacity claim, not evidence of autonomous novelty under the old environment. |
| **B: many identities, weak significance** | The evolutionary-activity neutral shadow produces genotype identities without genotype-specific adaptive significance (Q002, K010). MODES explicitly filters some noncoding differences (§4 above). | Identity counts do not establish adaptive novelty. Neither result licenses treating all neutral variation as irrelevant to future evolution. |
| **C: descriptive novelty without causal novelty** | **Constructed logical counterexample:** append an independently changing inert label to a reproducing system, stipulating that it affects neither reproduction, mutation of functional traits, nor ecological interactions. | A label-sensitive description reports novelty; a behavioral description need not. Causal irrelevance is stipulated here, not inferred from a short neutral assay. |
| **D: adaptive behavior within assigned functions** | Avida's EQU experiments evolved a complex rewarded logic behavior using simpler features as stepping stones. The reward menu was specified in advance. [Lenski et al. 2003](https://cse.msu.edu/~ofria/pubs/2003LenskiEtAl.pdf) | New adaptive behavior does not by itself establish new kinds of evolutionary possibility. This experiment does **not** prove that subsequent mutational potential stayed unchanged. |
| **E: metric disagreement** | MODES reports treatments where meaningful change and ecological diversity increase without corresponding final novelty increase; it also cannot distinguish every evolutionary-activity class. [Dolson et al. 2019, §§3.1, 5](https://cse.msu.edu/~dolsonem/pdfs/modes_paper.pdf) | Different measurements can support different conclusions about ongoing activity. This is not a matched demonstration of two validated universal OEE tests giving opposite verdicts. |

**Interpretation / limits:** A strong empirical D—proving that an adaptive innovation creates no additional future possibilities under every relevant description—was not found. A simple logical counterexample suffices against sufficiency: a stipulated two-type evolutionary system allows an advantageous replacement and then has an absorbing derived state. Adaptation occurs; no further types are generable. This is a deduction from imposed rules, not a discovered biological mechanism.

For E, Q002 additionally establishes definitional disagreement about fixed-model exploration. That is disagreement over the target, not experimental error.

## 8. Existing candidate solutions

**Fact / published proposals, with Interpretation of their limits:**

| Approach | Existing contribution | Remaining choice or limitation |
|---|---|---|
| Probabilistic bisimulation/state aggregation | Groups states with matched outputs/rewards and transition probabilities into equivalence classes | Preserves supplied distinctions; does not choose evolutionary significance |
| Computational mechanics | Minimal predictive equivalence of histories for a specified process | Observables remain specified; predictive equivalence is not automatically intervention equivalence |
| Input–output causal states | Compares future outputs conditional on future inputs and pasts | Input/output boundaries and relevant responses must be supplied |
| Behavioral novelty search | Compares behaviors rather than raw genotypes | Behavioral descriptors and distance measures remain selected |
| Intrinsic emergence | Requires emergent organization to matter to the system's own behavior/evolution | A conceptual target, not a complete capacity decision procedure |
| Semantic information | Tests which system–environment information is causally necessary for maintaining viability | Boundary, viability measure, interventions, and horizon remain explicit choices |
| Functional information | Measures rarity of configurations achieving a performance threshold | Function, ensemble, and threshold are given; rarity is not evolutionary arrival probability |
| Causal emergence | Compares effective information across micro/macro descriptions | Interventional conventions matter; causal strength is not adaptive novelty |

For finite Markov dynamics, the standard aggregation condition is that equivalent states have equal transition probability into every equivalence block, while preserving relevant labels. Such a quotient preserves target-hitting probabilities when targets are unions of blocks. The action-dependent version requires matching for each action. This supplies a rigorous existing analogue of behavioral interchangeability. Without labels or outcomes to preserve, even a one-block partition can satisfy the transition condition, so the condition alone cannot identify evolutionary functions. [Givan, Dean & Greig 2003, §§2–4](https://cs.brown.edu/people/tdean/publications/archive/GivanetalAIJ-03.pdf)

Input–output computational mechanics supplies a richer response-based equivalence than passive current phenotype. It still starts with defined input/output processes. [Barnett & Crutchfield 2015](https://arxiv.org/pdf/1412.2690)

Novelty search makes the genotype/behavior distinction operational and can discover outcomes missed by objective-driven search. Its behavioral distance is still specified by the experimenter; removing a task objective does not remove representation dependence. [Lehman & Stanley 2011](https://gwern.net/doc/reinforcement-learning/exploration/2011-lehman.pdf)

Crutchfield already connects intrinsic emergence to structures being used within the system, with evolutionary significance through fitness and persistence. The proposed endogenous-significance idea therefore has prior art and should not be renamed as a new hypothesis. [Crutchfield 2001, intrinsic emergence discussion](https://csc.ucdavis.edu/~cmg/papers/EvRevInno.pdf)

Kolchinsky and Wolpert operationalize semantic information by interventions on system–environment correlations and resulting viability. They explicitly allow researcher choices of viability function and intervention class. This is a causal account of significance, not a hereditary innovation inventory or proof of OEE. [Kolchinsky & Wolpert 2018](https://artemyk.github.io/assets/pdf/papers/Kolchinsky_Wolpert_2018_Semantic%20information,%20autonomous%20agency%20and%20non-equilibrium%20statistical%20physics.pdf)

Hazen et al.'s functional information is the negative logarithm of the fraction of configurations meeting a specified function threshold. It quantifies performance rarity conditional on those choices, not access under a biased evolutionary process. [Hazen et al. 2007](https://pmc.ncbi.nlm.nih.gov/articles/PMC1876432/)

Hoel et al. provide an intervention-based sense in which macro descriptions can have higher effective information. Subsequent criticism identifies ambiguities in macro interventions and the order of abstraction and marginalization. This debate does not establish or refute an intrinsic OEE criterion. [Hoel et al. 2013](https://pmc.ncbi.nlm.nih.gov/articles/PMC3856819/), [Eberhardt & Lee 2022](https://www.mdpi.com/2409-9287/7/2/30)

## 9. Remaining explanatory gap

**Interpretation:** The missing bridge is precise. Reachability answers whether a **specified** event can occur. Predictive/causal equivalence constrains which distinctions can be discarded while preserving **specified** consequences. Evolutionary and semantic accounts offer grounds for selecting consequential outcomes. The reviewed work does not combine these into a generally accepted rule selecting all future evolutionarily meaningful outcomes without presupposing their catalogue.

Two opposite errors must be avoided:

1. Discarding variation because it has no present measured effect loses cryptic future potential.
2. Retaining every microscopic distinction—or treating every causal effect as evolutionary significance—admits inert detail, nonadaptive effects, or consequences irrelevant to the evolutionary claim.

“Any possible causal difference” and “any difference in current fitness” therefore do not resolve the problem. A comparison must specify which contexts are reachable endogenously, not merely imaginable or engineerable, and which lineage consequences must be preserved.

**Answer to the strongest question:** Future physical continuations can be properties of a specified system–environment dynamics independent of anyone observing them. Existing theory also supports objective, conditional tests of evolutionary consequences. What is not established is a unique intrinsic partition of those continuations into meaningful evolutionary possibilities. No satisfactory general solution was found in this search; this is a bounded literature finding, not an impossibility theorem.

## 10. Known / Underexplored / Unknown

**Known / ESTABLISHED, within cited scopes**

- Realization, mutational potential, arrival probability, and establishment are distinct.
- Neutral/cryptic variation can preserve current measured phenotype while changing subsequent adaptation.
- Structural models can establish specified reachability or exclusion; finite non-detection alone generally cannot.
- Existing predictive equivalences and causal significance measures constrain descriptions but retain specified observables, outcomes, or interventions.
- Current phenotype, fitness, novelty count, and persistence alone are insufficient summaries of future potential.

**PARTIALLY EXPLORED**

- Using endogenous consequences to identify significance: intrinsic emergence, semantic information, organizational function, and fitness-based filters already address parts of this.
- Preserving future distributions under coarse-graining: causal states and probabilistic bisimulation already supply formal tools.

**UNDEREXPLORED status not established**

The exact intersection with hereditary adaptive capacity remains unresolved in the sources examined. This pass does not establish that it has received little research overall, or justify a novelty claim.

**UNKNOWN**

- Whether a sufficiently general intrinsic criterion can select relevant evolutionary outcomes while preserving cryptic potential and excluding irrelevant differences.
- Whether such a criterion can support useful closure diagnoses in non-enumerable or computationally intractable systems.
- Whether further generativity is required by a defensible stronger OEE account, beyond being a separate property of some innovations.

No genuinely new falsifiable hypothesis is justified by this decomposition; [HYPOTHESES.md](HYPOTHESES.md) remains unchanged.

## 11. Highest-information next question

**Can an existing causal or predictive coarse-graining retain cryptic evolutionary potential while removing causally inert variation, without prespecifying a catalogue of future functions?**

This targets the unresolved choice of consequential outcomes; preserving probabilities for an already supplied target is an existing result. No additional pass is undertaken here.
