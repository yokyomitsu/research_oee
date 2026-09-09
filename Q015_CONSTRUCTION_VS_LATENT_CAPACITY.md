# Q015 — Construction versus Latent Capacity

One theoretical research pass, 2026-09-08. Scope: the bounded ancestral-capacity and causal-equivalence conditions left by [Q014](Q014_EVIDENCE_FOR_ORGANIZATIONAL_TYPE_CREATION.md). This pass does not propose a general OEE mechanism.

Epistemic convention: descriptions of published concepts and results are **Fact**. Cross-framework conclusions and the bounded test below are **Interpretation**. No scientific **Hypothesis** is introduced.

## 1. Problem statement

The question is:

> How can we distinguish evolution constructing a genuinely new organizational capacity from evolution merely actualizing, revealing, or recombining capacity already latent in the ancestor?

An unbounded test cannot answer it. If “latent in ancestor $A$” includes arbitrary mutations, recombination, environmental changes, external manipulations, and indefinitely long evolution, then every descendant reachable from $A$ is latent by definition. “Latency” becomes identical to historical evolvability:

\[
O\text{ is latent in }A
\quad\Longleftrightarrow\quad
\Pr(A\leadsto O)>0
\text{ under some admissible history}.
\]

That statement is a reachability claim, not evidence that $A$'s current developmental or organizational system already has the capacity to construct $O$. Genotype–phenotype map theory explicitly separates possible phenotypes from phenotypes attainable in specified mutational neighborhoods, while first-passage work further separates positive reachability from feasible access. [Fontana & Schuster 1998](https://doi.org/10.1006/jtbi.1998.0771), [Schaper & Louis 2014](https://doi.org/10.1371/journal.pone.0086635), [Chatterjee et al. 2014](https://doi.org/10.1371/journal.pcbi.1003818)

The comparison therefore needs two declarations:

1. a bounded family of environments, inherited variants, perturbations, or transformations allowed when assaying the ancestor; and
2. an equivalence relation stating which causal differences count as the same organizational type.

Without the first, all evolutionary reachability becomes latency. Without the second, any quantitative change can be redescribed as a new type, and any topological change can be embedded as a parameter value of a larger model.

## 2. Meanings of latent capacity

“Latent” covers different empirical claims. They should not be pooled.

| Meaning | Operational ancestral set | What a positive result establishes | What it does not establish |
|---|---|---|---|
| **A. Immediately expressed capacity** | The ancestral population in its usual environment | $A$ already exhibits $O$ | That the capacity was newly constructed; this is realized ancestral organization |
| **B. Environmental plasticity** | Unchanged ancestral genotypes across a stated environmental/intervention range | $O$ lies in the assayed ancestral reaction norm | That $O$ is expressed normally, adaptive, inherited as an induced state, or reachable in every environment |
| **C. Cryptic or standing variation** | Sampled ancestral population, with its existing alleles and developmental responses | Some ancestral genotypes or allele combinations produce or potentiate $O$ when exposed | That a typical ancestral individual has the capacity, or that later integration was already present |
| **D. Recombinational capacity** | Existing ancestral alleles under the population's specified mating and recombination process | $O$ can be assembled without de novo mutation within that population and protocol | Immediate plasticity or individual-level capacity; recombination is a heritable transformation |
| **E. Mutational accessibility** | A declared $k$-step neighborhood, mutation spectrum, population process, and budget | $O$ is locally accessible from $A$ | That the ancestral developmental system already constructs $O$; this is accessibility, not latency in the strict developmental sense |
| **F. Historical evolvability** | Arbitrarily long histories under mutation, recombination, selection, and environmental change | $O$ is evolutionarily reachable from $A$ | A nontrivial construction-versus-latency distinction |

Meanings B and C are established uses in the plasticity and cryptic-variation literatures. D is meaningful but population- and recombination-system-relative. E is standard mutational accessibility. F should not be called latent capacity in this project because it collapses the target distinction.

This produces a nested-looking hierarchy only under fixed assay definitions. Environmental plasticity, standing variation, and mutational accessibility need not be set-theoretically nested when different environments, population samples, or genotype–phenotype maps are used. No monotonic claim is implied.

## 3. Plasticity and genetic accommodation

Phenotypic plasticity is the capacity of one genotype to produce different phenotypes across environments. Plasticity-first accounts propose that an environment can first elicit a phenotype and that selection can subsequently alter its regulation, form, frequency, threshold, or environmental sensitivity through genetic accommodation. Genetic assimilation is the limiting case in which an initially environment-dependent phenotype becomes comparatively environment-independent. [Levis & Pfennig 2016](https://doi.org/10.1016/j.tree.2016.03.012), [Ehrenreich & Pfennig 2016](https://doi.org/10.1093/aob/mcv130)

The established evidential design is already a bounded ancestral-capacity test: identify an ancestor or justified ancestral proxy, rear ancestral and derived lineages in ancestral and derived environments, and compare their reaction norms in a common garden. Let $P_L(E)$ denote the probability that lineage $L$ expresses the focal phenotype in environment $E$. The main alternatives are:

\[
\begin{array}{ll}
P_A(E')>0,\ P_D(E')>0 & \text{the phenotype is ancestrally inducible;}\\
P_A(\cdot)\neq P_D(\cdot) & \text{the reaction norm has evolved;}\\
P_A(E')=0,\ P_D(E')>0 & \text{derived capacity within the tested domain.}
\end{array}
\]

The first appearance of a plastic phenotype can be phenotypically new relative to recorded history while its production capacity is ancestral relative to the assayed reaction norm. These are compatible statements because “new occurrence” and “new generative capacity” have different baselines.

Genetic accommodation can do at least three different things:

- shift the probability or threshold of an ancestral response;
- stabilize or canalize a previously induced phenotype;
- rewire development so that a different causal route reconstructs a similar phenotype.

None of these changes alone settles organizational identity. Rewiring is the clearest candidate for a causal-type change, but stabilization can also matter if it creates an internally reconstructed life cycle or inheritance relation rather than merely changing expression frequency. An apparent loss of plasticity can be a shifted induction threshold that reappears when a broader environmental range is assayed, demonstrating why two-environment tests can overstate assimilation. [Sikkink et al. 2014](https://doi.org/10.1534/g3.114.010553)

**Decision:** plastic origin does not invalidate later organizational construction. If the ancestor already constructs the same reproduction/inheritance organization under $E'$, then that organization is environmentally latent. If evolution later creates a different, inherited reconstruction relation—even while retaining a similar morphology—organizational construction can occur after phenotypic appearance.

## 4. Cryptic variation

Cryptic genetic variation has little or no phenotypic effect in a specified background or environment but becomes consequential after an environmental or genetic change. Hayden, Ferrada, and Wagner experimentally showed that RNA-enzyme populations allowed to accumulate cryptic variants adapted more rapidly to a new substrate: the variants preserved the original phenotype yet occupied genotypes pre-adapted to the changed condition. [Hayden, Ferrada & Wagner 2011](https://doi.org/10.1038/nature10083)

Release of such variation establishes revelation of an ancestral **population's** sampled genetic capacity. It does not show that:

- every ancestral genotype could construct the phenotype;
- the phenotype's later developmental integration was already present;
- the new environment merely revealed, rather than also selected and reorganized, the response;
- all mutational routes to the phenotype were standing in the ancestral population.

The time of variation origin and the time of organizational construction can therefore differ. Existing alleles may supply ingredients or a rudimentary response at $t_0$; later selection can alter their regulatory coupling, developmental reliability, parent–offspring reconstruction, or reproductive consequences at $t_1$. Calling the entire $t_1$ organization latent because some contributing alleles existed at $t_0$ confuses component provenance with organization.

The appropriate assay distinguishes three claims: phenotype inducibility in ancestral genotypes, variance among ancestral genotypes in that inducibility, and evolved change in the descendant reaction norm or causal mechanism. Plasticity-first criteria explicitly make these separate evidential steps. [Levis & Pfennig 2016](https://doi.org/10.1016/j.tree.2016.03.012)

## 5. Co-option and exaptation

Exaptation distinguishes a feature's current effect or use from the selective history for which it arose. Co-option research shows that old genes, pathways, structures, and regulatory modules can be recruited in new spatial, temporal, or functional contexts. [Gould & Vrba 1982](https://doi.org/10.1017/S0094837300004310), [True & Carroll 2002](https://doi.org/10.1146/annurev.cellbio.18.020402.140619)

Facilitated-variation theory makes the same point constructively: conserved core processes, modularity, weak regulatory linkage, and exploratory behavior can allow a small number of regulatory changes to deploy old components in new combinations. This is established prior art, not a new “organizational recombination” hypothesis. [Gerhart & Kirschner 2007](https://doi.org/10.1073/pnas.0701035104)

Three novelty questions must be kept separate:

| Question | Relevant comparison |
|---|---|
| Are any components new? | Molecular or material ancestry |
| Is the effect or function new? | Historical function and current causal contribution |
| Is the organization new? | Identity of relations among components, developmental reconstruction, reproduction, or inheritance |

Old parts can support a new organization. If ancestral $a,b,c$ are redeployed so that new coupling $a\leftrightarrow c$ implements a new reproductive process, the absence of a new component does not make that relation ancestrally instantiated. Conversely, a new component can be inserted as a replaceable realizer while the character or organization remains homologous.

The molecular-exploitation history of steroid receptors supplies both directions of the warning. An ancestral receptor already had affinity for a hormone before that hormone evolved, so the binding capacity was latent as a structural by-product. Later substitutions changed specificity and integrated the receptor into a new functional interaction. Ancestral resurrection can locate these events; the mere age of either molecule cannot. [Bridgham, Carroll & Thornton 2006](https://doi.org/10.1126/science.1123348)

## 6. Character identity and novelty theory

Morphological novelty theory distinguishes a new state of a homologous character from the origin of a new character identity. Character Identity Mechanisms (ChIMs) propose that homologues can retain a recognizable, cohesive causal profile despite turnover in their lower-level etiological realization. [Müller & Wagner 1991](https://doi.org/10.1146/annurev.es.22.110191.001305), [DiFrisco, Love & Wagner 2020](https://doi.org/10.1007/s10539-020-09762-2)

This directly blocks two invalid inferences:

\[
\text{same parts}\Rightarrow\text{same character}
\qquad\text{and}\qquad
\text{different mechanism}\Rightarrow\text{different character}.
\]

Developmental-system drift is the decisive counterexample to the second inference: homologous phenotypes can retain identity while their gene-regulatory or morphogenetic underpinnings diverge. [True & Haag 2001](https://doi.org/10.1046/j.1525-142x.2001.003002109.x)

Character-identity theory therefore supplies a strong model for a construction-versus-state distinction in morphological evolution. It does not fully solve Q015 for three reasons:

1. ChIMs are developed for anatomical units such as cell types, tissues, and organs; a collective parent–offspring cycle or inheritance channel is not automatically an anatomical character.
2. Historical continuity can preserve character identity despite extensive causal drift, whereas Q015 sometimes asks whether reproduction or inheritance relations themselves changed.
3. The causal profile and organizational level used to identify a ChIM still require scientific specification and comparative evidence.

For anatomical claims, use character, homology, and ChIM terminology. For a transition in evolutionary individuality, use ETI theory. For broader changes in reproduction or inheritance that are not either of those, state the specific relation-level change rather than proposing “organizational type” as a new natural kind.

## 7. Developmental constraints

Developmental bias and constraint describe how development shapes the distribution, dimensions, and covariance of phenotypic variation supplied to selection. Hallgrímsson and colleagues proposed that evolutionary novelty can involve both an adaptive-peak transition and breakdown of ancestral developmental constraints so that variation appears in a new direction or dimension. [Hallgrímsson et al. 2012](https://doi.org/10.1002/jez.b.22448)

This supplies a useful operational contrast:

\[
V_A=\text{distribution of heritable phenotypic variation generated by a declared ancestral population, environment, and variation process}.
\]

Moving within $V_A$ is different from an evolved change to the developmental map that changes $V_A$. But neither “outside” nor “new dimension” is intrinsic. $V_A$ depends on population sampling, mutation and recombination operators, environments, trait coordinates, and the detection threshold. A rotation of coordinates can turn an apparently new axis into a combination of old axes, and finite sampling can mistake a low-probability ancestral direction for absence.

The defensible claim is distributional and bounded: the inherited change alters the probability law of organizational variants under the same specified perturbation family, and the change cannot be represented as movement within the ancestral causal-equivalence class. This is evolution of developmental bias or evolvability unless the altered relations also cross a separately justified organizational identity boundary.

“Breaking a constraint” is therefore neither necessary nor sufficient for a new organizational type. Old constraints can be quantitatively relaxed without type change; a small regulatory alteration can introduce a new parent–offspring relation without a large displacement in ordinary trait space.

## 8. Bounded ancestral-capacity comparison

Existing theory does not provide one privileged universal bound. It supplies claim-specific experimental bounds: reaction norms for environmental plasticity, ancestral population samples for standing variation, mutation neighborhoods for local accessibility, replay experiments for historical contingency, and causal abstractions for intervention-preserving comparisons.

A compact representation is useful if its relativity remains explicit. Let

\[
B=(G_A,E,I,T,R)
\]

specify an ancestral genotype or population ensemble $G_A$, environments $E$, developmental interventions $I$, allowed heritable transformations $T$, and a resource or time budget $R$. Let $\sim_K$ be an equivalence preserving the causal relations $K$ relevant to the claim. Then define

\[
\mathcal C_{B,\sim_K}(A)
=
\left\{
[O]_{\sim_K}:
O\text{ is produced from }G_A
\text{ under }(E,I,T,R)
\right\}.
\]

This set represents organizational equivalence classes supported by a declared ancestral assay. It is partly observable through experiments or exhaustive models and partly inferential where sampling is incomplete. It is not an intrinsic catalogue of everything the ancestor “really could” do.

The bound should follow the claim:

| Claim | Principled bound |
|---|---|
| “Environmentally latent” | Hold inherited state fixed; vary preregistered, biologically justified environments and developmental perturbations |
| “Present in standing variation” | Sample the ancestral population and its ordinary recombination process; prohibit de novo mutation |
| “Locally accessible” | Declare mutation spectrum, $k$, population process, and resource budget; call the result accessibility rather than strict latency |
| “New developmental/organizational capacity” | Permit perturbations that preserve the proposed ancestral causal type; test whether the descendant requires an inherited change crossing $\sim_K$ |

For an artificial system, the corresponding bound must distinguish generic enablement from enumeration. Local interaction, matter, communication, mutation, and construction primitives necessarily make many organizations physically possible. They count as generic substrate capacity when the dynamics do not consult the later entity boundary, life-cycle phase, inheritance channel, or organizational label. A group identifier, fixed nesting channel, or menu of organizational modes is different: it places the claimed alternatives in the operative model before evolution. Formal realizability under generic rules is not ancestral expression, while selecting among designer-enumerated modes is not construction of a previously unspecified type.

Evidence for construction within $B$ has the form

\[
[O_D]_{\sim_K}\notin \mathcal C_{B,\sim_K}(A),
\qquad
A+\Delta\longrightarrow O_D,
\]

where $\Delta$ is an evolved inherited change and intervention evidence supports that $\Delta$ changes a $K$-relation rather than merely revealing an unassayed ancestral state. The negative claim remains finite: “not found or not possible under $B$,” never “metaphysically absent from all ancestral futures.”

The displayed non-membership has two evidential strengths. An exhaustive model or invariant can establish exclusion under $B$; a finite empirical assay can establish only non-detection plus a sampling or power bound. The latter should not be written as absolute impossibility.

## 9. Causal type-equivalence

Causal-model abstraction offers exact and approximate notions under which low- and high-level interventions commute. Such formalisms can test whether two descriptions preserve specified intervention–response relations; they do not choose the biological variables or intervention family. [Rubenstein et al. 2017](https://is.mpg.de/publications/rubensteinetal17), [Beckers, Eberhardt & Halpern 2020](https://proceedings.mlr.press/v115/beckers20a.html)

For Q015, systems belong to the same causal organizational type only relative to a declared $K$. Candidate relations include:

- what counts as a reproducer and which event maps parent to offspring;
- what is transmitted or developmentally reconstructed;
- which components and environmental resources reconstruct which stages;
- which interventions preserve or destroy the life cycle;
- which entity bears heritable fitness differences.

An equivalence $\sim_K$ should preserve the intervention–response structure over these relations, allowing differences in irrelevant material realization and continuous parameter values. A type boundary is supported when no mapping in the tested equivalence family preserves $K$ across ancestor and descendant.

There is no established universal $\sim_K$ for all organizational novelty. ChIMs supply domain-specific identity profiles for anatomical characters; life-cycle and individuality theories constrain collective reproduction; organizational closure identifies mutually maintained constraints at stated timescales. Closure could mark a new organizational regime if a new closure relation is demonstrated under a fixed constraint ontology, but closure alone does not establish novelty, heredity, reproduction, or a unique boundary. [Montévil & Mossio 2015](https://doi.org/10.1016/j.jtbi.2015.02.029)

Causal emergence is also insufficient. A macrovariable can have higher effective information than a microdescription relative to a coarse-graining and intervention distribution without being evolutionarily new, heritable, or a reproducer. [Hoel, Albantakis & Tononi 2013](https://doi.org/10.1073/pnas.1314922110)

## 10. Ancestral reconstruction and intervention

Different experiments answer different counterfactuals.

| Test | Strongest supported inference | Main limit |
|---|---|---|
| Resurrect ancestor; expose it to descendant environment | Direct ancestral reaction norm over tested environments | Environmental range is finite; reconstructed ancestor may be uncertain |
| Assay many ancestral clones, alleles, and crosses | Standing and recombinational capacity in the sampled population | Rare unsampled variants and other populations remain unresolved |
| Introduce descendant mutations singly and jointly into ancestor | Causal sufficiency, epistasis, and order-dependence in the ancestral background | Does not exclude alternative routes or show a type change |
| Revert derived mutations in descendant | Dependence and possible reversibility in the descendant background | Compensatory changes can make reversion fail; failure is not proof of historical necessity |
| Reciprocal common garden or transplant | Genetic versus environmental contribution to reaction-norm divergence | Maternal, ecological, and developmental carry-over require controls |
| Synthetic reconstruction of a relation | The engineered relation is sufficient for a specified output in that background | It can unmask ancestral architecture and need not reproduce the historical route |
| Replay from frozen or resurrected ancestors | Frequency and contingency of routes under the replay protocol | Does not enumerate all routes, environments, or longer histories |

The LTEE citrate case shows the strength and limit of this logic. Replay from frozen clones localized historical potentiation; genomic and genetic reconstruction identified promoter capture that activated an ancestral citrate transporter, subsequent refinement, and background-dependent access. This establishes actualization, potentiation, and refinement along a documented history. It does not entail that aerobic citrate use was either wholly present or wholly absent in an unbounded ancestral possibility set. [Blount, Borland & Lenski 2008](https://doi.org/10.1073/pnas.0803151105), [Blount et al. 2012](https://doi.org/10.1038/nature11514)

Ancestral protein resurrection and derived reversion likewise reveal causal substitutions and epistatic constraints. In the glucocorticoid receptor, later substitutions made direct reversal of earlier function-switching changes nonfunctional. That result demonstrates background-dependent irreversibility, not a universal boundary between parameter and type. [Bridgham, Ortlund & Thornton 2009](https://doi.org/10.1038/nature08249)

Thus, observing both

\[
A\overset{\Delta}{\longrightarrow}D
\quad\text{and}\quad
D\overset{\neg\Delta}{\longrightarrow}A\text{-like}
\]

supports sufficiency and descendant-background dependence of $\Delta$. Historical necessity additionally requires replay or path evidence; ancestral incapacity requires a bounded ancestral assay; causal type change requires an independently declared $\sim_K$.

## 11. Type versus parameter change

The notation $f_{\theta_1}\rightarrow f_{\theta_2}$ versus $f\rightarrow g$ does not create a scientific distinction. Any finite family of functions can be embedded in a larger parameterized family, while a threshold can split continuous variation into types.

Type change becomes non-arbitrary only relative to conserved explanatory commitments. For example, if $K$ requires preservation of collective parentage, inherited reconstruction, and intervention responses, then increased cluster size that preserves the same growth-and-fracture life cycle is a within-type change, whereas the first establishment of a closed collective parent–offspring relation may cross the equivalence.

A defensible type claim should satisfy four safeguards:

1. **Predeclared consequence:** $K$ is chosen because the scientific claim concerns reproduction, inheritance, development, or individuality—not because it separates the observed cases.
2. **Intervention validity:** the proposed mapping predicts responses to interventions not used to fit it.
3. **Representation robustness:** the distinction survives alternative recodings and coarse-grainings that preserve the same $K$-relations.
4. **Boundary controls:** the same rule classifies known continuous variants as same-type and recognized relation changes as different-type.

Even then the result is conditional causal objectivity, not an observer-free ontology. Developmental-system drift proves that extensive mechanistic change can remain within a character type; threshold shifts prove that a small parameter change can alter observed categories; and ETIs can be graded rather than instantaneous.

## 12. Organizational novelty and individuality

Organizational novelty is not coextensive with evolutionary individuality.

- A new developmental or regulatory relation can arise within an existing individual without creating a new reproducer.
- A collective can acquire Darwinian individuality primarily by reorganizing ancestral adhesion, division, and inheritance mechanisms.
- A new collective trait can be causal and heritable without completing an ETI.

If the claimed new organization is a new evolutionary individual, established ETI concepts—collective life cycle, parentage, heritable fitness variation, individuation, conflict mediation, and endogenization—are the right framework. “Organizational-type creation” is redundant in that scope.

If the claim instead concerns a new reproduction or inheritance relation within an existing level, it is broader than ETI but must name that relation. There is no evidence that all such changes form one additional natural category. Character identity, developmental organization, and causal abstraction are complementary tools, not pieces of a universal organizational-novelty predicate.

Snowflake yeast illustrates the separation. Disrupting `ACE2` prevents mother–daughter separation and generates clonal clusters with a growth-and-fracture life cycle and high heritability of collective traits; a single genetic change can therefore have a large organizational consequence. Later evolution of roughly $10^4$-fold toughness and macroscopic size retained the clonal snowflake life cycle while changing cell shape, packing, and branch entanglement. Those later results are major collective innovations but are not automatically additional organizational types. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102), [Bozdag et al. 2023](https://doi.org/10.1038/s41586-023-06052-1)

## 13. Counterexamples

### A — Accepted novelty can begin as ancestral plasticity

Plasticity-first and genetic-assimilation cases intentionally begin with a phenotype inducible in ancestors or ancestral proxies. Later evolution changes its reaction norm or refinement. This defeats the rule “ancestrally inducible means never evolutionarily novel.” It instead dates phenotypic appearance, genetic accommodation, and any later organizational reconstruction separately. [Levis & Pfennig 2016](https://doi.org/10.1016/j.tree.2016.03.012)

### B — Old parts can form accepted novelties

Co-option and facilitated variation explain new traits through regulatory redeployment of conserved components. Therefore component novelty is not necessary for character or relational novelty. [True & Carroll 2002](https://doi.org/10.1146/annurev.cellbio.18.020402.140619), [Gerhart & Kirschner 2007](https://doi.org/10.1073/pnas.0701035104)

### C — New character identities can involve recombination and redeployment

ChIM-based work treats co-option as a candidate explanation for new character origins only after identifying identity mechanisms and testing their altered organization. Reuse does not settle identity either way. [DiFrisco, Love & Wagner 2023](https://doi.org/10.1016/j.semcdb.2022.03.030)

### D — Large genetic or mechanistic change need not change type

Developmental-system drift preserves a homologous character while its developmental genetic machinery diverges. Mutation count, network edit distance, and molecular turnover are therefore insufficient type criteria. [True & Haag 2001](https://doi.org/10.1046/j.1525-142x.2001.003002109.x)

### E — Tiny genetic change can create a major causal organization

A single `ACE2` disruption can transform cell separation into persistent clonal attachment, geometrically structured development, fracture reproduction, and a unicellular genetic bottleneck. Genetic distance is therefore not necessary for a large organizational change. [Ratcliff et al. 2015](https://doi.org/10.1038/ncomms7102)

### F — A derived organization can draw on ancestral plastic capacity

Wild-type *Chlamydomonas* can form transient palmelloids under several environmental triggers, while predation experiments evolved stable, heritable clonal multicellular forms. This weakens any claim of de novo multicellular morphology, but it does not decide whether the evolved life cycle, obligacy, or developmental reconstruction relation was new. [Herron et al. 2019](https://doi.org/10.1038/s41598-019-39558-8)

### G — Classification can disappear under a different causal description

The same transition can be “a threshold change in cell separation” under a cellular regulatory model and “origin of collective reproduction” under a life-cycle model. Both descriptions can be causally adequate for different interventions. Causal-abstraction theory cannot choose between them without a declared variable and intervention set. This defeats a universal type/parameter boundary but not a claim-relative one. [Beckers & Halpern 2019](https://arxiv.org/abs/1812.03789)

### H — Historical novelties need not admit direct ancestral-capacity assays

Morphological novelties are routinely studied through fossils, phylogeny, homology, and comparative development when the actual ancestor cannot be resurrected or its full reaction norm assayed. Novelty theory itself notes that ancestral landscapes and constraints may have to be inferred. A bounded capacity assay is therefore not necessary for every defensible historical novelty claim; it is required for the stronger experimental claim that a descendant capacity was absent from, rather than continuous with, a specified ancestral capacity. [Müller & Wagner 1991](https://doi.org/10.1146/annurev.es.22.110191.001305), [Hallgrímsson et al. 2012](https://doi.org/10.1002/jez.b.22448)

## 14. Central decision

**B — CONDITIONAL ANCESTRAL-CAPACITY TEST**

Construction and latency are scientifically distinguishable only relative to an explicit ancestral ensemble, allowed perturbation/transformation family, resource bound, and causal type-equivalence. This is stronger than outcome comparison and weaker than a universal proof of ancestral incapacity.

Qualifications:

- **C is a common historical pattern:** many documented novelties combine inherited potential with new regulation, coupling, or reconstruction. There is often a continuum of contribution, even when a categorical relation-level claim can be tested.
- **A is too strong:** character-identity and developmental theory solve important morphological cases but do not supply a universal equivalence for reproduction and inheritance.
- **D is partly true but not selected:** reproduction/inheritance organization requires criteria beyond anatomical character identity, yet ETI, life-cycle, intervention, and causal-abstraction theories already supply the pieces. No new theory named “organizational causality” is justified.
- **E is false at the conditional level:** observer dependence prevents a universal boundary, but declared causal consequences and robustness tests make restricted comparisons empirically meaningful.

The unbounded statement “$O$ was reachable from $A$” should be classified as historical evolvability, not latent capacity. A one-mutation result is local accessibility. Neither by itself decides whether a causal organizational type was already instantiated.

## 15. Remaining explanatory gap

The broad latency/construction question is narrowed to a validation problem:

> Can one preregister an intervention-preserving equivalence over reproduction, inheritance, and developmental reconstruction that classifies a known transition and a known within-type refinement correctly under the same bounded ancestral assay?

At the broad level, “evolution changes the causal organization that generates heritable variation” is already covered by evolution of evolvability, developmental-system evolution, and changes to genotype–phenotype maps. Adding a reproduction/inheritance equivalence makes a more specific transition or relation-level claim; it does not create a new OEE principle. One validated type change would still not demonstrate continued or open-ended production of further types.

What remains missing is not another general definition of novelty. It is a worked discriminant showing that the same causal rule can separate:

- ancestral environmental and standing-variation expression;
- local mutational access;
- establishment of a new parent–offspring or inheritance relation; and
- quantitative refinement after that relation already exists.

If no defensible equivalence survives this positive/negative-control test, “organizational type” should be retired in favor of separate character, life-cycle, heredity, and individuality claims. If it survives, the next mechanistic question would concern which evolutionary changes cross that specific boundary. That mechanism is not investigated here.

## 16. Problem classification

| Problem type | Q015 result |
|---|---|
| **Definition** | “Latent” must be indexed to environmental, standing-variation, recombinational, or mutational operators. “Organizational type” must be indexed to causal relations $K$. The unrestricted terms are not well-defined. |
| **Measurement** | Reaction norms, standing-variation assays, common gardens, resurrection, reconstruction, reversion, and replay provide bounded evidence. Their coverage and ancestral fidelity remain finite. |
| **Formalization** | **Primary remaining gap.** No universal $B$ or $\sim_K$ exists; a domain-specific intervention-preserving equivalence over reproduction/inheritance needs a worked validation with controls. |
| **Mechanism** | Not yet reached. Explaining which mutations or ecological/developmental changes reliably cross a validated causal-type boundary is downstream of this pass. |

The absence of a universal equivalence is a formalization limit, not evidence for a missing OEE mechanism.

## 17. Known / Underexplored / Potentially Novel / Unknown

### KNOWN / ESTABLISHED

- Environmental plasticity, cryptic genetic variation, standing variation, local mutational accessibility, and long-run evolvability are distinct.
- Plasticity-first evolution separates ancestral induction from later genetic accommodation; accommodation can change thresholds, robustness, regulation, and form.
- Co-option and exaptation show that old components can support new characters or functions.
- Character identity can persist through developmental-system drift; mechanistic difference alone does not establish type difference.
- Ancestral resurrection, mutation reconstruction, reversion, and replay establish different bounded causal and historical claims.
- Exact or approximate causal equivalence is relative to variables, mappings, and allowed interventions.
- A single genetic change can have a major organizational consequence, while extensive genetic change can preserve character identity.

### UNDEREXPLORED

- A validated causal equivalence for collective reproduction and inheritance that is applied to ancestor, descendant, and within-type controls under one protocol.
- Integration of ancestral reaction norms, standing variation, mutation reconstruction, and life-cycle interventions in claims about experimentally evolved individuality.
- Sensitivity analysis showing which organizational conclusions persist across plausible causal coarse-grainings.

### POTENTIALLY NOVEL

None. The bounded notation composes established reaction-norm, accessibility, character-identity, and causal-abstraction ideas; it is not a new theory or empirical discovery.

### UNKNOWN

- Whether a reproduction/inheritance equivalence can distinguish type origin from later quantitative refinement without being tailored to the desired classification.
- Whether the closest level-blind artificial model lies outside ancestral environmental and standing-variation capacity under such an equivalence.
- Which dynamical changes, if any, recurrently create new causal organizational types rather than locally altering existing ones.

## 18. Hypothesis decision

**NO HYPOTHESIS JUSTIFIED**

Q015 supplies a conditional evidential and formalization boundary, not a new dynamical relation. Co-option, plasticity-first evolution, developmental-system drift, evolved evolvability, and intervention-preserving abstraction are established prior art. The next unknown is whether a proposed equivalence survives a discriminating case analysis; a missing formal criterion is not a scientific hypothesis. [HYPOTHESES.md](HYPOTHESES.md) remains unchanged.

## 19. Highest-information next question

Can one intervention-preserving equivalence over collective parentage, developmental reconstruction, and inheritance classify the `ACE2` snowflake transition as a causal organizational-type change while classifying later snowflake-yeast size and toughness evolution as within-type refinement, under the same bounded ancestral environmental and standing-variation assay?
