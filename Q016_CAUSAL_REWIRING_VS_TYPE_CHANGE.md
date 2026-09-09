# Q016 — Causal Rewiring versus Organizational-Type Change

One theoretical research pass, 2026-09-08. Scope: the identity criterion required by [Q015](Q015_CONSTRUCTION_VS_LATENT_CAPACITY.md). This pass does not propose a general OEE mechanism.

Epistemic convention: descriptions of published theories and results are **Fact**. Cross-framework judgments and the repository decision are **Interpretation**. No scientific **Hypothesis** or unsupported **Speculation** is introduced.

## 1. Problem statement

The question is:

> What distinguishes heritable causal rewiring that preserves an existing organizational type from causal rewiring that creates a genuinely new organizational type?

Q015 established that genetic distance, component age, and mechanistic change do not settle this question. The target contrast is provisionally:

\[
M_A\rightarrow M_B,
\qquad
\mathcal O(M_A)\sim_K\mathcal O(M_B)
\]

for type-preserving rewiring, versus

\[
M_A\rightarrow M_C,
\qquad
\mathcal O(M_A)\not\sim_K\mathcal O(M_C)
\]

for type-changing rewiring. Here \(K\) cannot mean “all causes.” It must identify the causal relations relevant to the scientific claim. If every molecular cause and intervention is included, ordinary evolutionary divergence almost always produces a different type. If only a narrow phenotype or fitness output is included, distinct developmental and reproductive organizations collapse into one type.

The required discriminator must therefore occupy a middle position:

\[
\boxed{
\text{identity-bearing causal relation}
\;<\;
\text{complete microcausal description}
}
\]

while being richer than limited input–output agreement. The prior-art question is whether biology supplies one such invariant across domains or only claim-specific invariants.

## 2. Developmental System Drift

Developmental System Drift (DSD) is the strongest negative case. In DSD, an ancestral or homologous character is conserved while the morphogenetic, regulatory, or genetic processes producing it diverge. The phenomenon is reported across distant and closely related taxa and can include different gene-expression patterns, different regulatory dependencies, and different loss-of-function phenotypes. [True & Haag 2001](https://doi.org/10.1046/j.1525-142x.2001.003002109.x), [Verster et al. 2014](https://doi.org/10.1371/journal.pone.0090258)

In *C. elegans* and *C. briggsae*, broad RNAi screens found many orthologues with different loss-of-function effects despite near-identical development and morphology. More recent work reports substantial differences in mutant relationships in the heterochronic pathway despite essentially the same anatomy and life history. Thus even a moderately rich intervention profile can drift while comparative biologists retain character identity. [Verster et al. 2014](https://doi.org/10.1371/journal.pone.0090258), [Ivanova & Moss 2023](https://doi.org/10.1093/genetics/iyad177)

What is preserved is not one universal molecular invariant. Depending on the case, it includes:

- historical continuity and homology of the character;
- recognizable anatomy, developmental outcome, or position in the life cycle;
- an identity-bearing causal profile at a coarser level than individual molecular edges;
- integration with the same surrounding character system.

What may change includes particular genes, regulatory connections, expression levels, compensatory pathways, developmental trajectories, robustness, and responses to molecular perturbation.

**Interpretation:** DSD defeats both “different mechanism means different type” and “complete intervention equivalence defines same type.” The conserved explanandum—usually a homologous character—licenses ignoring some causal changes. Which changes are ignorable is learned from comparative, phylogenetic, developmental, and intervention evidence together; it is not read directly from network edit distance.

## 3. Character identity mechanisms

Character Identity Mechanism (ChIM) theory is the closest established account of implementation change versus identity change for morphological characters. Earlier character-identity-network proposals grounded homology in historical continuity of regulatory networks rather than individual genes. The later ChIM model allows homologues to have diverse etiological organization while retaining a recognizable, cohesive causal profile. It explicitly proposes level-specific ChIMs for cell types, tissues, and organs. [Wagner 2007](https://doi.org/10.1038/nrg2099), [DiFrisco, Love & Wagner 2020](https://doi.org/10.1007/s10539-020-09762-2)

Character identity and character state have different explanatory roles. An identity mechanism individuates the character—such as a particular appendage or cell type—whereas downstream “realizer” processes can vary its shape, size, physiology, or function. Selection can alter character states while identity persists. Conversely, co-option of a conserved gene or module does not make the resulting structures homologous; shared components can be redeployed into a new character context. [Wagner 2014](https://doi.org/10.23943/princeton/9780691156460.001.0001), [DiFrisco, Love & Wagner 2023](https://doi.org/10.1016/j.semcdb.2022.03.030)

ChIM theory supplies three lessons for Q016:

1. Identity is attached to a scientifically individuated character, not to the whole causal history producing it.
2. Identity can tolerate replacement or reorganization of lower-level realizers.
3. Outcome-function alone cannot individuate identity; historical continuity, parts, activities, organization, and intervention evidence jointly constrain the causal profile.

It does **not** supply a general “organizational identity mechanism.” Collective reproduction, heredity, a life cycle, and evolutionary individuality are not automatically anatomical characters. Their identity-bearing relations are specified by other theories. Generalizing the phrase without supplying those relations would merely rename the problem.

## 4. Network/topological rewiring

A graph edit is neither necessary nor sufficient for organizational-type change. Regulatory networks with different edges can produce the same equilibrium expression pattern. In model genotype spaces, many such networks form connected neutral networks, so lineages can accumulate extensive topological change while preserving a phenotype. Importantly, locations within that same phenotype-neutral network can have different mutational neighborhoods and innovative potential. [Ciliberti, Martin & Wagner 2007](https://doi.org/10.1073/pnas.0705396104)

This yields four distinct comparisons:

| Change | What follows |
|---|---|
| Same topology, changed weights or kinetics | Dynamics and attractors may change |
| Changed topology, same tested attractor/output | Phenotype may be preserved |
| Changed topology and new attractor | A new dynamical state or capacity exists under the model |
| Changed identity-bearing relation | A domain-specific type claim may be justified |

Only the fourth is a type criterion, and it cannot be inferred from the first three without a theory identifying the relevant relation. A new attractor can be another state of an existing developmental system. A small edge or parameter change can instead establish persistent cell attachment and a collective growth–fracture cycle. Syntax such as \(f_{\theta_1}\to f_{\theta_2}\) versus \(f\to g\) is therefore not decisive.

Bisimulation, state aggregation, and dynamical equivalence can rigorously preserve specified trajectories, labels, or control responses. They remain relative to state variables, observations, inputs, tolerances, and time resolution. They can test a proposed equivalence; they do not identify the biological type to be preserved.

## 5. Causal equivalence

Structural-causal-model abstraction formalizes agreement between descriptions by requiring that mapped interventions produce compatible outcomes. Exact transformations, strong abstractions, and approximate abstractions differ in which distributions and interventions must be preserved. [Rubenstein et al. 2017](https://arxiv.org/abs/1707.00819), [Beckers & Halpern 2019](https://arxiv.org/abs/1812.03789), [Beckers, Eberhardt & Halpern 2020](https://proceedings.mlr.press/v115/beckers20a.html)

For Q016, this provides a useful **meta-criterion**. Let

\[
K=(V,I,Y,\tau)
\]

specify biologically interpreted variables \(V\), admissible interventions \(I\), identity-relevant outcomes or relations \(Y\), and tolerances or temporal resolution \(\tau\). Two implementations are equivalent when a mapping between them preserves the relevant intervention–response structure under \(K\).

Every term has a role:

- \(V\) represents entities or stages such as cells, collectives, parents, offspring, or anatomical units;
- \(I\) represents feasible perturbations relevant to their causal role;
- \(Y\) represents the claimed identity-bearing relation, not every observable output;
- \(\tau\) makes graded biological and finite-measurement claims explicit.

This notation does not solve the biological problem. It exposes it. The formalism cannot determine whether \(Y\) should be a homologous character, life-cycle closure, parentage, inherited reconstruction, policing and demarcation, or constraint closure.

Complete micro-intervention equivalence is too strong because it classifies DSD as type-changing. Limited input–output equivalence is too weak because systems with different reproductive dependencies or robustness can match on a narrow assay. The relevant intervention family must be justified by an independently identified biological role and must predict withheld perturbations. Equivalence is consequently conditional and partly observer/model dependent, but not arbitrary when constrained by domain theory and controls.

## 6. Reproduction relations

“Who reproduces whom?” is a strong boundary for claims about reproducers. Reproduction theory distinguishes simple, collective, and scaffolded reproduction and emphasizes parent–offspring lineage formation, material overlap, development, and propagation. Collective reproduction can arise while constituent cells continue reproducing. A herd, by contrast, can be a by-product of its members’ reproduction without itself being a plausible bearer of fitness. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112)

Life-cycle theory adds temporal organization. On one account, a collective becomes an individual when its coarse-grained stages form a closed multiplicative cycle; formally, all relevant stages recurrently connect within the collective-level projection. This can separate a genuine collective cycle from a gerrymandered grouping or a population that merely grows. [Doulcier, Takacs & Bourrat 2024](https://doi.org/10.1017/psa.2023.162)

A changed reproduction relation is therefore:

- **necessary** for the specific claim that a new kind of reproducer or collective life cycle arose;
- **not necessary** for new morphological, physiological, regulatory, or autonomous organization within an existing reproducer;
- **not sufficient** for a new Darwinian individual, because parent–offspring production may lack adequate inherited variation, fitness differences, or internally generated individuation;
- **not sufficient** for a universal organizational type, because reproduction itself has plural and borderline realizations.

Mechanisms can drift while the same parent–offspring and stage relations persist. Conversely, a small heritable change can create persistent attachment and fracture reproduction without introducing new molecular components. Thus reproduction supplies one domain-specific identity relation, not the cross-domain invariant.

## 7. Heredity and developmental reconstruction

Heredity theories likewise privilege a relation rather than an immutable material carrier. Evolutionary individuality requires enough trait-transmission fidelity for selection, but different individuals can achieve it through different reproductive and inheritance mechanisms. Organizational accounts describe heredity as cross-generational conservation of functional constraints under organizational closure, explicitly extending beyond genes without treating every persistent similarity as heredity. [Ereshefsky & Pedroso 2015](https://doi.org/10.1073/pnas.1421377112), [Mossio & Pontarotti 2022](https://doi.org/10.1093/bjps/axz031)

The identity-bearing target can be represented as a developmental reconstruction relation:

\[
\text{offspring resources and environment}
\longrightarrow
\text{reconstructed reproducer or character}.
\]

The relation may remain invariant while genes, cellular routes, ecological inputs, and timing change. DSD is already a developmental example. “Reconstitutor” accounts make the same logical point for heredity: the material basis grounding a recurrent phenotypic variant can change across generations without necessarily changing what is inherited. [Charbonneau 2022](https://doi.org/10.1007/s11229-022-03810-y)

A new inheritance or reconstruction relation is necessary only for a claim about a new hereditary organization. It is not necessary for every character novelty, and recurrence is not sufficient: similar phenotypes can be independently induced by a persistent environment. Parentage, cross-generational causation, developmental resources, and the level bearing variation must be declared.

## 8. Closure / autonomy

Closure-of-constraints theory characterizes biological organization through mutually dependent constraints that maintain one another at specified timescales. It distinguishes process from constraint, provides a way to investigate self-maintaining boundaries, and permits hierarchical or nested closure. [Mossio & Moreno 2010](https://pubmed.ncbi.nlm.nih.gov/21162371/), [Montévil & Mossio 2015](https://doi.org/10.1016/j.jtbi.2015.02.029)

The appearance of a new closure can therefore mark a new autonomous organization **under that theory**, provided:

- the constraint set and system boundary are fixed independently of the desired result;
- mutual maintenance is established causally rather than inferred from co-occurrence;
- the new closure persists on the timescale relevant to the claim;
- alternative descriptions do not recover the same closure by merely relabeling components.

Closure is not a universal type criterion. Its proponents state that closure underdetermines the full requirements of a paradigmatic organism. A self-sustaining autocatalytic network can possess mutually enabling organization yet lack sufficiently rich heredity or Darwinian evolution. Nested closures also make the “new level” depend on selected system boundaries and timescales. [Mossio & Moreno 2010](https://pubmed.ncbi.nlm.nih.gov/21162371/), [Vasas, Szathmáry & Santos 2010](https://doi.org/10.1073/pnas.0912628107)

Accordingly, new closure is neither necessary for every organizational novelty nor sufficient for a new evolutionary individual. It is an identity candidate for autonomy claims only.

## 9. Causal emergence and multilevel organization

Causal-emergence frameworks compare causal descriptions across scales. Effective information can be higher in a macrodescription than in a complete microdescription because coarse-graining reduces degeneracy or indeterminism relative to a chosen state space and intervention distribution. The result is formally important: macro causal models can outperform micro models even when fully realized by them. [Hoel, Albantakis & Tononi 2013](https://doi.org/10.1073/pnas.1314922110)

It does not establish organizational-type creation:

1. the standard examples are simple state-transition systems with no heredity, reproduction, or evolutionary history;
2. the preferred macrolevel depends on the coarse-graining and intervention distribution;
3. a newly evolved individual can be causally noisy and need not maximize effective information;
4. a causally informative macrostate can be transient and non-heritable;
5. the metric compares explanatory scales at a time, not ancestral and descendant identities through history.

Causal emergence can support the claim that a macrodescription is consequential rather than merely convenient. It cannot by itself identify a reproducer, date a novelty, or distinguish a new type from a better description of an old system.

Nested individuality creates the same warning. Cells can remain reproducers inside a multicellular individual, and lower- and higher-level selection can overlap. A new effective level need not replace the old one, and coarse-graining alone can manufacture a level. ETI theory requires historical change in Darwinian or individuating relations, not just macro-predictive advantage. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112), [West et al. 2015](https://doi.org/10.1073/pnas.1421402112)

## 10. Relational novelty

The claim that old parts can form new relations is established prior art. Co-option and exaptation separate component ancestry from current developmental or functional role. ChIM research makes co-option experimentally meaningful by asking which identity mechanism, module, or activity was redeployed and whether the resulting character has a new identity. [Gould & Vrba 1982](https://doi.org/10.1017/S0094837300004310), [DiFrisco, Love & Wagner 2023](https://doi.org/10.1016/j.semcdb.2022.03.030)

Evo-devo work on pregnancy supplies an explicit relational case: eutherian pregnancy has been analyzed as a historically individuated reproductive relation integrating maternal and embryonic processes, not merely as a novel component. Placenta research likewise describes new signaling dynamics and regulatory organization arising from interactions between ancestral tissues. [Nuño de la Rosa, Pavličev & Etxeberria 2021](https://doi.org/10.3389/fpsyg.2020.572106), [Griffith 2021](https://doi.org/10.1002/jmor.21322)

“Relational novelty” is therefore not a missing general explanation. A new edge, dependency, or interaction is scientifically significant only when theory and evidence show that it individuates a character, life-cycle stage, reproducer, inheritance channel, or autonomous organization. Otherwise it is network rewiring with an unspecified explanandum.

## 11. Evolutionary consequences

It is tempting to define type by future evolutionary consequences:

\[
\mathcal T(O)=
\{\text{heritable transformations supported by }O\}.
\]

This does not supply an independent invariant. Regulatory networks with the same phenotype can occupy different locations on a neutral network and expose different mutational neighborhoods. DSD can therefore preserve character identity while changing robustness, accessibility, and evolvability. [Ciliberti, Martin & Wagner 2007](https://doi.org/10.1073/pnas.0705396104)

If every change in \(\mathcal T(O)\) is a type change, ordinary evolution of developmental bias and evolvability fragments one character into many “organizational types.” If only qualitative changes count, the criterion again requires a prior identity relation stating which transformation differences matter.

Evolutionary consequences remain important evidence in the appropriate domain:

- a new parent–offspring relation changes which entities can form lineages;
- a new inheritance relation changes what can recur with fidelity;
- a new individuation mechanism changes the balance of within- and between-entity selection;
- a new developmental character changes the units whose states can vary;
- a new closure changes which constraints jointly maintain an autonomous system.

But no one relation is necessary for all types of organization. If two implementations preserve all relations relevant to the stated evolutionary claim, a difference in their remaining mutation neighborhoods is evolution of evolvability within that type, not sufficient evidence of another type.

The narrow deep-learning analogy—same function under changed internal representation versus access to a new function class—adds no criterion beyond multiple realization, causal abstraction, and evolvability. It is therefore not used as evidence.

## 12. Candidate invariants

No single invariant survives all domains. The supported result is a family indexed to the kind of identity being claimed.

| Domain claim | Candidate identity-bearing invariant | Type-preserving rewiring | Evidence of type change | Principal limit |
|---|---|---|---|---|
| Morphological character | Homology plus a level-specific ChIM causal profile | DSD changes etiological realization while the character remains traceable | Origin, duplication, or co-option of a distinct character identity | Historical and mechanistic inference; ChIM profiles are not universal checklists |
| Developmental character state | Same individuated character and reconstruction role | Shape, size, expression, route, or robustness changes | A new individuated character rather than another state | Character individuation remains method-dependent |
| Reproducer / life cycle | Parent–offspring relation and closure of the declared stage cycle | Growth rate, stage duration, mechanics, or propagule size changes | A new closed multiplicative cycle or parentage relation | Competing reproduction concepts and coarse-grained stages |
| Hereditary organization | Cross-generational reconstruction of type-relevant functional organization | Material carriers and developmental routes change | A new transmissible or reconstructive relation at the claimed level | Environment, ancestry, trait, and fidelity are conditional |
| Evolutionary individual | Entity-level Darwinian capacity plus mechanisms that demarcate and police it | Implementations of bottlenecks, conflict mediation, or boundary maintenance change | A new entity acquires internally supported between-entity selection and controlled within-entity conflict | Individuality is multidimensional and graded |
| Autonomous organization | Closure among constraints at a declared boundary and timescale | Component or pathway replacement preserves mutual maintenance | A new causally demonstrated closure | Closure alone underdetermines heredity, reproduction, and organismality |

The common logical form is:

\[
\boxed{
\text{same type relative to domain }D
\iff
\text{the identity-bearing role/relation }K_D
\text{ is preserved under admissible replacements}
}
\]

This is a family resemblance among criteria, not a universal biological invariant. “Admissible replacements” must be tested with withheld interventions and same-type/different-type controls. Historical continuity matters for homology; functional causal roles matter for individuality; cycle structure matters for reproduction; cross-generation reconstruction matters for heredity. These cannot be collapsed without losing the reason each type is scientifically useful.

Ellen Clarke’s account of individuality is instructive: different mechanisms can realize common policing and demarcation roles. It supplies multiple realization at the level of evolutionary individuality, analogous in logical form to ChIMs but with different identity-bearing roles. It does not make policing and demarcation the identity criteria for organs or life cycles. [Clarke 2013](https://doi.org/10.5840/jphil2013110817)

## 13. Counterexamples

### A — Massive rewiring with conserved character identity

DSD directly supplies this case. Closely related nematodes retain near-identical development and anatomy while many orthologues acquire different expression or perturbation effects. A complete molecular intervention profile would split accepted homologues and is therefore too fine-grained. [Verster et al. 2014](https://doi.org/10.1371/journal.pone.0090258)

### B — A small molecular change can create an accepted higher-level organization

Disrupting `ACE2` in yeast prevents mother–daughter separation and yields clonally developing snowflake clusters with high broad-sense heritability of collective traits. The primary study describes this single mutation as creating a new level of biological organization. Mutation count and graph-edit magnitude therefore cannot define type. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102)

### C — A new causal macrostructure can lack heredity and reproduction

Causal-emergence results are demonstrated in abstract Markov systems. A macrolevel can have greater effective information without any lineage, inherited variation, or selection. Macro causal advantage is therefore insufficient for evolutionary novelty. [Hoel, Albantakis & Tononi 2013](https://doi.org/10.1073/pnas.1314922110)

### D — A new evolutionary individual can be assembled from ancestral mechanisms

Snowflake yeast reuses cell division, mother–daughter adhesion, clonal inheritance, physical fracture, and a unicellular bottleneck. The novelty claim concerns their new collective relation and life cycle, not physically new primitives. Co-option and ETIs defeat component-newness requirements. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102)

### E — A reproduction relation need not identify a new developmental character

Collective and scaffolded reproduction can establish parent–offspring lineages by propagation or aggregation even when no new anatomical character is identified. Conversely, character novelties arise within unchanged reproductive relations. Reproduction is an invariant only for reproducer or individuality claims. [Godfrey-Smith 2015](https://doi.org/10.1073/pnas.1421378112), [Ereshefsky & Pedroso 2015](https://doi.org/10.1073/pnas.1421377112)

### F — New closure need not create a selectable unit

Autocatalytic and compositional systems can exhibit self-sustaining organization or growth-and-fission dynamics while lacking the hereditary capacity required for sustained Darwinian evolution. Closure and self-maintenance are not sufficient for a new evolutionary individual. [Vasas, Szathmáry & Santos 2010](https://doi.org/10.1073/pnas.0912628107)

### G — Equally defensible abstractions can disagree

The `ACE2` change can be represented as a parameter or threshold change in cell separation, or as the origin of a collective growth–fracture cycle. Both descriptions can be causally adequate for different interventions. Causal-abstraction theory does not choose between them; the stated explanandum does. This defeats observer-free type identity but not conditional objectivity.

### H — Accepted transitions can lack a sharp causal instant

ETIs commonly pass through overlapping lower- and higher-level reproduction and selection. Individuality is multidimensional, and group formation, life-cycle closure, conflict mediation, heredity, and fitness reorganization need not coincide. A scientifically meaningful transition can therefore be graded even when a particular life-cycle relation has a sharp threshold under a model. [Godfrey-Smith 2009](https://doi.org/10.1093/acprof:osobl/9780199552047.001.0001), [West et al. 2015](https://doi.org/10.1073/pnas.1421402112)

The counterexamples jointly destroy a universal rule based on amount of rewiring, graph topology, phenotype, intervention profile, reproduction, closure, causal emergence, or future variation alone.

## 14. Central decision

**B — DOMAIN-SPECIFIC INVARIANTS**

Different biological domains possess defensible identity criteria, but no general organizational invariant was found.

- Morphological homology and ChIM theory explain why DSD can preserve character identity.
- Reproduction and life-cycle theories identify parentage and cycle closure for claims about reproducers.
- Heredity theories identify cross-generational transmission or reconstruction relations.
- Individuality theories identify Darwinian and individuating roles such as demarcation and policing.
- Closure theories identify autonomous mutual maintenance at a specified boundary and timescale.
- Causal abstraction supplies the formal structure for testing preservation of any chosen relation, but does not select it.

**Qualification toward C:** a conditional family of intervention-preserving equivalences is a defensible general *methodological structure*. It is not a biological type criterion until a domain theory supplies the identity-bearing variables, interventions, and relations.

**Qualification toward F:** all useful classifications retain declared model, scale, historical, and tolerance choices. They achieve conditional objectivity through independent theory, comparative continuity, intervention validation, and controls; they do not escape observer dependence completely.

**Why not D:** changes in reproduction, heredity, or selectable-unit structure provide strong boundaries for evolutionary-individuality claims, but they are unnecessary for new anatomical, regulatory, physiological, or autonomous organizations. They cannot serve as the universal organizational criterion.

Thus type-preserving rewiring changes realizers while preserving the domain’s identity-bearing relation. Type-changing rewiring changes that relation itself. This statement is not circular only when the relation is independently motivated and the same equivalence classifies known positive and negative controls.

## 15. Remaining explanatory gap

The broad conceptual question is narrowed to a formal validation problem:

> Can one predeclared domain-specific equivalence over collective parentage and life-cycle closure distinguish the origin of a collective reproducer from large subsequent changes within that reproducer, without changing variables, interventions, or tolerances between comparisons?

Snowflake yeast supplies a demanding paired case. `ACE2` disruption establishes persistent clonal attachment and a growth–fracture cycle; later evolution produced approximately \(2\times10^4\)-fold larger and \(10^4\)-fold tougher clusters while retaining that clonal multicellular life cycle. If one declared equivalence cannot classify the first as a new reproducer relation and the second as within-type refinement, it is either too weak, too fine, or fitted retrospectively. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102), [Bozdag et al. 2023](https://doi.org/10.1038/s41586-023-06052-1)

This is not yet a general mechanism question. Only after a domain-specific boundary survives positive/negative controls would it be meaningful to ask which evolutionary dynamics recurrently cross that boundary. Failure would warrant retiring “organizational type” in favor of separate character, reproduction, heredity, individuality, and autonomy claims.

## 16. Problem classification

| Problem type | Q016 result |
|---|---|
| **Definition** | **Primary.** “Organizational type” has no universal identity bearer. The claim must name a character, reproducer, inheritance relation, evolutionary individual, or autonomous closure. |
| **Measurement** | Comparative development, lineage reconstruction, perturbation, life-cycle observation, and multilevel assays can test declared invariants, but finite intervention coverage and graded thresholds remain. |
| **Formalization** | **Primary.** Causal abstraction can formalize preservation only after a domain-specific relation and intervention family are fixed. A controlled worked application remains missing. |
| **Mechanism** | Deferred. The dynamics generating a type change cannot be isolated before the relevant type equivalence is validated. |

The unresolved issue is not evidence for a missing OEE mechanism.

## 17. Known / Underexplored / Potentially Novel / Unknown

### ESTABLISHED / KNOWN

- DSD allows substantial genetic, regulatory, and intervention-response divergence while a homologous character remains conserved.
- Character identity and character state are distinct; ChIMs are level-specific causal profiles, not complete molecular implementations.
- Network topology, attractor structure, and limited input–output behavior do not independently determine biological identity.
- Exact, approximate, and dynamical causal equivalences are relative to variables, interventions, mappings, and tolerances.
- Reproduction, heredity, individuality, and closure theories privilege different relations and admit multiple realizations.
- Co-option and relational novelty show that old components can form new characters or reproductive organizations.
- Causal emergence does not entail heredity, evolutionary novelty, or a new individual.
- Evolvability and mutational neighborhoods can change while a character identity is preserved.

### PARTIALLY EXPLORED

- The shared logical form in which diverse mechanisms realize a stable character, reproducer, hereditary relation, or individual-level role.
- Intervention-based validation of identity profiles in comparative biology.
- Life-cycle closure as a formal boundary for particular ETIs, alongside graded individuality criteria.

### UNDEREXPLORED

- Applying one predeclared reproduction/life-cycle equivalence to an ancestor, a transition, and a major within-type refinement.
- Sensitivity analysis across biologically plausible variable sets and intervention families without retuning the desired classification.
- Explicit negative controls in claims that evolutionary experiments create new organizational types.

### POTENTIALLY NOVEL

None. The domain-indexed equivalence family composes established homology, individuality, reproduction, heredity, closure, and causal-abstraction concepts. It is not a new natural kind or dynamical theory.

### UNKNOWN

- Whether a single reproduction/life-cycle equivalence can pass the snowflake-yeast positive/negative-control test.
- Whether any minimal cross-domain core beyond “preserve the independently chosen identity-bearing relation” has empirical content.
- Where to place thresholds in graded transitions without tailoring them to historical exemplars.

## 18. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

Q016 establishes a definition/formalization boundary. DSD, multiple realization, causal abstraction, co-option, life-cycle closure, and relational novelty are prior art. “Domain-specific invariants exist” is a methodological conclusion, not a falsifiable dynamical relation. [HYPOTHESES.md](HYPOTHESES.md) remains unchanged.

## 19. Highest-information next question

Can a predeclared equivalence over collective parentage and life-cycle closure classify the `ACE2` snowflake transition as a new reproducer type while classifying later snowflake size and toughness evolution as type-preserving, without changing the variables, interventions, or tolerances between the two comparisons?
