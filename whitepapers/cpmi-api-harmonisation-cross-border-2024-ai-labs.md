---
type: "AILabsWhitepaper"
title: "API Harmonisation for Cross-Border Payments: Model Failure Patterns on CPMI's October 2024 Framework"
slug: "cpmi-api-harmonisation-cross-border-2024-ai-labs"
audience: "ai_labs"
regulation_slug: "CPMI-API-HARMONISATION-CROSS-BORDER-2024"
regulation_id: "320322"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-11T01:44:06.973210+00:00"
published_at: "2026-06-07T08:31:39.252227+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/bis-cpmi/CPMI-API-HARMONISATION-CROSS-BORDER-2024/ai-labs/"
timestamp: "2026-06-16T07:45:40.313543+00:00"
---

# API Harmonisation for Cross-Border Payments: Model Failure Patterns on CPMI's October 2024 Framework

- **Regulation.** [`CPMI-API-HARMONISATION-CROSS-BORDER-2024`](/okf/regulations/CPMI-API-HARMONISATION-CROSS-BORDER-2024.md) — Promoting the Harmonisation of Application Programming Interfaces to Enhance Cross-Border Payments: Recommendations and Toolkit
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-11T01:44:06.973210+00:00

## Executive summary

Across six question-level AI runs on this regulation, Claude Opus 4.7 and Claude Sonnet 4.6, both with web search enabled, failed in structurally similar ways. The October 2024 CPMI recommendations document and the technical annex of the ISO 20022 update sit behind a content boundary that web retrieval does not reliably cross. When the models reach into that boundary, they do not refuse: they fabricate. Opus produced a per-recommendation stakeholder taxonomy keyed to ISO, BIAN, and SWIFT, with no support in the regulator's own recommendation text. Sonnet asserted a specific November 2026 cutover commitment for ISO 20022 structured addresses that the regulator's document does not contain. Both models hedged or denied a SARB-CPMI pre-validation collaboration that CPMI Brief No. 9 (November 2025) names explicitly. Both substituted a 2025 monitoring-survey sample of 57 fast payment systems for the regulator's stated universe of 70+. The failure shape is not model-specific: it is a property of how this regulation's content is exposed publicly, and it reveals retrieval-coverage, source-attribution, and confidence-calibration gaps that an AI lab can address with targeted evaluation.

## Full whitepaper

# API Harmonisation for Cross-Border Payments: Model Failure Patterns on CPMI's October 2024 Framework


Across six question-level AI runs on this regulation, Claude Opus 4.7 and Claude Sonnet 4.6, both with web search enabled, failed in structurally similar ways. The October 2024 CPMI recommendations document and the technical annex of the ISO 20022 update sit behind a content boundary that web retrieval does not reliably cross. When the models reach into that boundary, they do not refuse: they fabricate. Opus produced a per-recommendation stakeholder taxonomy keyed to ISO, BIAN, and SWIFT, with no support in the regulator's own recommendation text. Sonnet asserted a specific November 2026 cutover commitment for ISO 20022 structured addresses that the regulator's document does not contain. Both models hedged or denied a SARB-CPMI pre-validation collaboration that CPMI Brief No. 9 (November 2025) names explicitly. Both substituted a 2025 monitoring-survey sample of 57 fast payment systems for the regulator's stated universe of 70+. The failure shape is not model-specific: it is a property of how this regulation's content is exposed publicly, and it reveals retrieval-coverage, source-attribution, and confidence-calibration gaps that an AI lab can address with targeted evaluation.

## When This Affects an AI Lab

The CPMI API harmonisation framework is directly operational for compliance lawyers, payments-infrastructure architects, central-bank regulatory counsel, fintech product teams building cross-border payment rails, and correspondent-bank operations managers. All of these audiences routinely use frontier models to accelerate regulatory interpretation. The questions that produced failures here are not adversarial probes: 'which stakeholders does each recommendation target?', 'what does the self-assessment toolkit contain?', 'which central bank is CPMI's named partner on pre-validation APIs?', 'what does the February 2026 ISO 20022 update commit to?'. These are live professional queries that drive regulatory submissions, vendor scoping, corridor strategy work, and supervisory engagement. When a model answers confidently with fabricated structure or denies regulator-published facts as unavailable, the downstream professional harm is concrete: advice given on invented authority, implementation plans built on fabricated taxonomies, market briefings compressing a 70+ universe to a 57-sample figure that the regulator did not state.

For the lab, the exposure compounds. A model that presents fabricated per-recommendation stakeholder assignments with the same surface confidence as retrieved fact creates liability ambiguity for customers who cannot distinguish inference from retrieval. A compliance team that submits a CPMI-facing position paper misattributing a recommendation's target stakeholder group, because the model invented the breakdown, has a reputational and regtech-liability path that leads back to the model's output. Separately, evals that test the model on this regulation by querying its accessible surface (the publication abstract, the four recommendation-category names) will return false confidence scores: the model answers shallow questions correctly while hallucinating everything behind the PDF barrier.

The structural feature of this regulation that makes it a high-yield failure surface is the combination of a machine-readable landing page with an inaccessible full-text PDF containing all substantive technical content, plus a set of adjacent CPMI publications (briefs, speeches) that the model retrieves intermittently. The abstract signals enough structure, four categories, ten recommendations, a self-assessment toolkit, a named collaboration partner, that the model can construct a plausible-seeming answer to granular questions using that skeleton. The answers sound specific. They are not retrieved. Partial-signal hallucination behind an inaccessible primary source is the pattern AI labs need to red-team for before deploying retrieval-augmented models into regulated professional workflows.

## Aggregate Impact

Six findings, two models, one regulation: the failures cluster around three identifiable defect patterns. First, false-negative retrieval (findings 007-Sonnet and 010-Sonnet): the model reported regulator-published facts as unavailable when the underlying source, CPMI Brief No. 9 in one case, the November 2023 Tara Rice speech in the other, explicitly contains them. The model's web-retrieval coverage is intermittent across CPMI publications, and absence in the retrieved set is reported to the user as absence from the regulator's record. Second, inference-presented-as-retrieval (findings 008-Opus and 009-Sonnet): the model fabricated structured taxonomic content, a stakeholder breakdown for ten recommendations, a specific ISO 20022 cutover commitment, that has no support in the regulator's primary text. The structured presentation format gives the inference the visual register of retrieved fact. Third, statistical-substrate confusion (finding 010-Opus): the model substituted a survey-sample figure (57 FPS systems) for the regulator-stated universe figure (70+), without distinguishing between the two related-but-different numbers.

These three defect patterns are not idiosyncratic to a single question or a single model. False-negative retrieval appears in both Sonnet outputs; inference-as-retrieval appears across Opus and Sonnet; statistical-substrate confusion is an extension of the same retrieval-coverage gap. For an AI lab, this means the failures here are diagnosable as pipeline-level rather than as content-specific. The retrieval-grounding gate is not catching that retrieval was incomplete before allowing inference to fill; the source-attribution layer is not distinguishing between regulator publication and adjacent industry-community material; the user-facing response layer is not signalling confidence asymmetries between retrieved facts and inferred structure.

The cross-finding signal is that this regulation's content surface is a natural high-yield evaluation environment. The landing page is retrievable; the recommendations PDF is not; the adjacent briefs and speeches are intermittently retrievable; the technical annex of the ISO 20022 update is structurally inaccessible. Any eval suite that covers regulatory question-answering should include questions across that boundary to surface the inference-presented-as-retrieval pattern that this set of findings consistently produces.

## Findings

### Finding 7. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** An advisor to a South African financial institution needs to know which central banks are actively involved in piloting or implementing specific API harmonisation recommendations, and whether any central bank is specifically named as partnering with CPMI on the payment pre-validation API recommendation.
- **AI's response:** "it is plausible that SARB is engaged with the d224 implementation track, but I cannot point to a public CPMI statement naming SARB as the specific partner on the pre-validation API recommendation."
- **Regulator's text:** CPMI Brief No. 9 (Nov 2025): 'The CPMI, in collaboration with the South African Reserve Bank (SARB), has been advancing the API recommendation on payment pre-validation by conducting interviews with market stakeholders.'
- **Why the AI went wrong:** The model retrieved enough surface signal to identify SARB and the payment pre-validation recommendation but treated retrieval-uncertainty as truth-uncertainty, producing a hedge where CPMI Brief No. 9 had already removed the uncertainty by naming the partnership explicitly. The model's calibration here is biased toward hedge when it cannot directly verify a retrieved fact, even when the regulator has published the verifying source.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 7. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** Which central bank is explicitly named as a collaborating partner with CPMI on the payment pre-validation API recommendation from the October 2024 API harmonisation report, and what does that collaboration involve?
- **AI's response:** "available sources do not identify SARB as a named pilot partner for any specific d224 recommendation, including the pre-validation API recommendation"
- **Regulator's text:** CPMI Brief No. 9 (Nov 2025): 'The CPMI, in collaboration with the South African Reserve Bank (SARB), has been advancing the API recommendation on payment pre-validation by conducting interviews with market stakeholders.'
- **Why the AI went wrong:** Sonnet 4.6's web-search loop did not surface CPMI Brief No. 9 (or did surface it without extracting the SARB identification) and the model reported the absence-of-retrieval as an absence-of-fact. The negative answer is presented with the same surface confidence the model uses for verified positive retrieval; nothing in the response signals that the underlying retrieval coverage was incomplete.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 8. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** A compliance analyst asks which of the 10 CPMI API harmonisation recommendations specifically target commercial banks or correspondent banking institutions, which target payment system operators, which target central banks or regulators, and which target standards bodies, seeking a recommendation-by-recommendation stakeholder breakdown.
- **AI's response:** "(i) FACILITATIVE / GLOBAL HARMONISATION PROCESSES, primarily targeted at API standards-setting bodies (ISO, BIAN, Swift, regional/sectoral bodies), CPMI itself, and public authorities coordinating global governance; secondarily at payment-system operators that adopt those standards. Not specifically at correspondent banks."
- **Regulator's text:** Recommendation 1: Open API standards. All stakeholders in API standardisation, but especially jurisdictional authorities and standards organisations, should actively support the development of cross-border payment API standards that are voluntary, open and consensus-based. [...] Recommendation 2: Existing harmonisation initiatives. Jurisdictional authorities (eg central banks, relevant government agencies, and regulatory bodies) and standards organisations should leverage the experience of existing API harmonisation initiatives [...]
- **Why the AI went wrong:** With no retrievable per-recommendation content, the model inferred stakeholder assignments from the recommendation category names and its knowledge of how standards-body governance typically works. BIAN, ISO, and SWIFT appear as plausible assignments to a harmonisation-processes category without any retrieved basis. The model presented this inference as a stakeholder breakdown rather than as reasoned extrapolation from category names, and the structured taxonomic format gave the inference the surface register of a retrieved factual breakdown.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 9. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** What specific changes did the February 2026 updated CPMI harmonised ISO 20022 data requirements make compared to the October 2023 original, including regulatory developments incorporated, clarifications provided, and how the separate technical annex relates to the main document?
- **AI's response:** "From November 2026 onwards, only structured and hybrid addresses will be permitted in ISO 20022 cross-border payment messages, the fully unstructured address format is being phased out. This is being driven by the SWIFT/CBPR+ community and is reflected in d230's updated requirements."
- **Regulator's text:** The updated version of the report takes into account standardisation and regulatory developments since 2023, provides clarification where market participants had sought further guidance, and sets out the updated and expanded data model in a separate technical annex.
- **Why the AI went wrong:** The model fabricated a specific commitment, November 2026 cutover, structured-and-hybrid-addresses-only, and attributed it to the CPMI document. The actual CPMI text describes only generalised standardisation and regulatory developments since 2023, with a separate technical annex containing the data model. The structured-address content appears drawn from SWIFT/CBPR+ community material that the model has cross-attributed to CPMI without distinguishing the source corpus.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 10. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** A market briefing on the global fast payment system landscape needs CPMI data on how many domestic fast payment systems are currently operational globally, how many have already enabled cross-border payment exchanges, how many are planning cross-border linkages, and what proportion are operated by central banks versus private entities.
- **AI's response:** "the 2025 monitoring survey covers 57 fast payment systems (56 for one of the graph cuts), up from prior surveys; this is the most recent CPMI count"
- **Regulator's text:** Speech sp231115 (Nov 2023, Tara Rice): '70+ domestic fast payment systems currently operational globally'; '14 fast payment systems already enabling cross-border exchanges'; '24 systems planning linkages within five years'; '40% operated by central banks; 35% by private entities'
- **Why the AI went wrong:** The model retrieved a 2025 monitoring-survey figure (57 systems) and presented it as the answer to a question about the global FPS universe. The November 2023 Tara Rice speech documents the 70+ universe figure, but the model defaulted to the more recently retrieved sample figure without distinguishing between universe and sample. The user-facing response gives no signal that a sample-versus-universe substitution has occurred.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 10. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** A market briefing on the global fast payment system landscape was asked to include the proportion of fast payment systems operated by central banks versus private entities. The response correctly cited the 70+ global systems, 14 already cross-border, and 24 planning links, but falsely stated the ownership breakdown was not available in public CPMI sources, when the November 2023 CPMI speech by Tara Rice explicitly gives 40% central bank-operated and 35% privately operated.
- **AI's response:** "A precise percentage breakdown of central bank vs. privately operated FPS is not enumerated in the public Brief 10 summaries available."
- **Regulator's text:** Speech sp231115 (Nov 2023, Tara Rice): '70+ domestic fast payment systems currently operational globally'; '14 fast payment systems already enabling cross-border exchanges'; '24 systems planning linkages within five years'; '40% operated by central banks; 35% by private entities'
- **Why the AI went wrong:** The model could not surface the operator-mix percentages (40% central-bank-operated, 35% privately-operated) from its retrieval set and reported the absence as a property of the regulator's public record rather than as a property of its retrieval coverage. The November 2023 Tara Rice speech documents the figures explicitly; the model's retrieval of that speech is intermittent, the same source supplies the 70+ universe figure in other answer paths, and the inconsistency is not flagged in the user-facing response.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

## What Your Team Should Do

### Implications for your training data

The cross-model commonality on this regulation suggests training-data coverage of CPMI's API harmonisation material is uneven: the landing-page abstract and the four recommendation-category names are well-represented, but the per-recommendation stakeholder assignments, the self-assessment toolkit's structure, and the technical annex content of the ISO 20022 update are not. Adjacent material, SWIFT/CBPR+ community discussions, payment-industry commentary, monitoring-survey summaries, is well-represented and is being substituted as a proxy for the missing regulator-primary content. Training data review for regulatory document corpora should explicitly check coverage at the boundary between abstract/landing-page material and deep-PDF technical content, because the model's behaviour on this regulation suggests it treats one as evidence for the other when no signal flags the substitution.

A second training-data implication concerns regulator publications that postdate the model's training cutoff. CPMI Brief No. 9 (November 2025) names the SARB pre-validation partnership; the model is not retrieving or extracting that source consistently in its web-search loop. If training data coverage of CPMI material extends only through a particular cutoff, retrieval is the only path to post-cutoff facts, and the retrieval gap therefore manifests as a confidence-calibration gap (the model hedges or denies the post-cutoff fact). This pattern is observable here on a single regulator but is structurally a general feature of regulator-facing model deployment.

### Implications for your post-training logic

The inference-presented-as-retrieval pattern observed here is a post-training calibration issue, not a knowledge-deficit issue. The model has enough domain context to recognise that a stakeholder taxonomy or a structured-address commitment is the right shape of answer; what it lacks is the retrieval-grounding gate that should prevent emission of a structured detail when the underlying primary content was not retrieved. RLHF or constitutional-style fine-tuning that scores against retrieval-grounded output, where the model is penalised for emitting structured taxonomic detail without a corresponding retrieved-content signal, would address this specific failure mode.

The false-negative pattern (findings 007-Sonnet and 010-Sonnet) is a related but distinct post-training defect. The model's confident negatives on entity-level regulatory questions appear to be a generalisation of safety-aligned hedging: when the model cannot directly confirm a positive, it defaults to a confident negative rather than a flagged uncertainty. For regulator-facing deployment, this is exactly the wrong default: a confident negative on a fact the regulator has explicitly published causes more downstream professional harm than a flagged 'retrieval coverage may be incomplete' response. Calibration tuning that surfaces retrieval-coverage uncertainty in the user-facing response would address this.

### Specific eval / red-team probes RegLeg suggests

RegLeg suggests three probe categories for AI lab evaluation work on this regulation and structurally similar ones. First, retrieval-coverage probes: ask the model to identify specific facts published in CPMI briefs and speeches dated November 2025 and later, and score whether the model retrieves the underlying source consistently across multiple question phrasings. Intermittent retrieval, surfacing in some phrasings and not others, is itself the failure mode, and current responses do not signal it.

Second, inference-versus-retrieval probes: ask the model for structured taxonomic detail (per-recommendation stakeholder mapping, toolkit internal architecture, technical annex content) on regulations whose primary text is known to be inaccessible to web retrieval. Score whether the model signals that the structured detail is inference rather than retrieval, and what fraction of the time the inference output is materially correct against the regulator's actual text.

Third, universe-versus-sample probes: where a regulator documents both a universe figure (in a speech or brief) and a sample figure (in a monitoring survey), ask quantitative questions and score whether the model returns the figure that matches the question scope. The 70+ versus 57 substitution observed here is a single instance of a defect pattern that almost certainly appears across other regulator-published statistical material.

## How RLB Can Partner With Your Lab

RegLeg's published research is a documented record of where frontier models, Claude Opus 4.7, Claude Sonnet 4.6, both with and without web search, have produced confident, wrong answers on specific regulator-published material. The research is built to be useful to AI labs: each finding includes the question phrasing, the model's verbatim response, the regulator's primary text, and a diagnosis of where in the retrieval-and-generation pipeline the failure occurs. For an AI lab evaluating retrieval-grounded model behaviour on regulator-facing workloads, the research is a ready-made adversarial test corpus drawn from real professional queries on live regulations.

RegLeg works with AI labs on three specific engagement types. First, eval corpus development: we build evaluation question sets calibrated against the specific defect patterns we have documented, false-negative retrieval, inference-as-retrieval, statistical-substrate confusion, scored against regulator-primary-source ground truth that we have already aggregated. Second, retrieval pipeline audit: we run the lab's deployed model against a curated set of regulator-facing questions whose answers we know, and surface where the retrieval coverage gaps are, where the inference fill is happening, and where the confidence-calibration layer is miscalibrated. Third, red-team partnership: we provide ongoing adversarial probe sets as new regulator publications emerge, so the lab's eval coverage stays current with the regulatory material the model is being asked to handle in production.

Engagements are confidential by default. The published research is the pitch; the methodology, test-corpus assembly, and probe construction sit inside the partnership. For an AI lab preparing to deploy retrieval-augmented models into regulatory and professional-services workflows, this partnership shape is the most direct path from documented failure patterns to shippable model improvements.

## Related concepts

- Regulation: [CPMI-API-HARMONISATION-CROSS-BORDER-2024](/okf/regulations/CPMI-API-HARMONISATION-CROSS-BORDER-2024.md)
- Regulator: [BIS-CPMI-INT-001](/okf/bodies/BIS-CPMI-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)