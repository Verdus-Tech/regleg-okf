---
type: "AILabsWhitepaper"
title: "BBNJ High Seas Biodiversity Agreement: Model Hallucination Findings"
slug: "bbnj-high-seas-biodiversity-agreement-2023-ai-labs"
audience: "ai_labs"
regulation_slug: "BBNJ-HIGH-SEAS-BIODIVERSITY-AGREEMENT-2023"
regulation_id: "328031"
body_id: "UNTC-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "UNTC"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-11T01:47:18.098145+00:00"
published_at: "2026-06-07T08:38:30.743382+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/untc/BBNJ-HIGH-SEAS-BIODIVERSITY-AGREEMENT-2023/ai-labs/"
timestamp: "2026-06-16T07:45:45.353712+00:00"
---

# BBNJ High Seas Biodiversity Agreement: Model Hallucination Findings

- **Regulation.** [`BBNJ-HIGH-SEAS-BIODIVERSITY-AGREEMENT-2023`](/okf/regulations/BBNJ-HIGH-SEAS-BIODIVERSITY-AGREEMENT-2023.md) — Agreement under the United Nations Convention on the Law of the Sea on the Conservation and Sustainable Use of Marine Biological Diversity of Areas beyond National Jurisdiction (BBNJ Agreement / High Seas Treaty)
- **Regulator.** [`UNTC-INT-001`](/okf/bodies/UNTC-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-11T01:47:18.098145+00:00

## Executive summary

This paper presents findings from RegLeg's hallucination research on the BBNJ Agreement (2023), administered by the United Nations Treaty Collection. Two models, Claude Opus 4.7 and Claude Sonnet 4.6, both with web search active, were tested across six findings covering Articles 10(1), 14(1), 22(2), and 27 of the Agreement. The dominant patterns are article-level misattribution (both models named Article 30 for the EIA screening threshold which sits at Article 27 ; Opus 4.7 placed the Conference of the Parties non-undermining duty at Article 5 or Article 8 when Article 22(2) governs ; Sonnet 4.6 placed the DSI benefit-sharing duty at Article 15(5) when Article 14(1) governs) and inversion of the Article 10(1) non-retroactivity default (both models). The convergence of error patterns across the two model families points to a shared upstream artefact rather than independent reasoning failures. The Agreement entered into force on 17 January 2026; practitioners across legal, biotechnology, pharmaceutical, shipping, and energy sectors will rely on model output for early scoping, which makes article-level precision and temporal-scope fidelity load-bearing failure modes.

## Full whitepaper

# BBNJ High Seas Biodiversity Agreement: Model Hallucination Findings


This paper presents findings from RegLeg's hallucination research on the Agreement under the United Nations Convention on the Law of the Sea on the Conservation and Sustainable Use of Marine Biological Diversity of Areas Beyond National Jurisdiction (2023), administered by the United Nations Treaty Collection (Office of Legal Affairs, Treaty Section). Two models were tested, Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search, across questions covering the Agreement's environmental impact assessment screening threshold (Article 27, Part IV), its marine genetic resource and digital sequence information framework (Articles 10(1) and 14(1)), and the Conference of the Parties non-undermining duty (Article 22(2), Part III). Across six findings, the dominant error patterns are: article-level misattribution where the substantive paraphrase is correct but the cited article number is wrong; and inversion of the Agreement's express non-retroactivity rule for marine genetic resource obligations. Both models converged on the same wrong article number for the EIA screening threshold (Article 30 rather than Article 27) and on the same direction of inversion for Article 10(1) retroactivity, pointing to a shared upstream artefact rather than independent reasoning failures.

## When This Affects an AI Lab

The BBNJ Agreement entered into force on 17 January 2026 and is immediately relevant to a widening set of users who will query frontier models for legal, compliance, and strategic guidance: biotech and pharmaceutical companies with marine research programmes, shipping operators navigating new area-based management designations, environmental law practices, multilateral-development-bank teams financing high-seas infrastructure, and government delegations preparing for the Agreement's first Conference of the Parties. Each of these users is likely to treat model output on the Agreement's operative provisions as a starting point for real decisions. When a model confidently inverts the Agreement's retroactivity default or places the EIA screening threshold at the wrong article, the downstream consequence is mispriced compliance risk for practitioners who act on that output.

For an AI lab, the exposure runs in two directions. First, if a corporate compliance team structures a benefit-sharing strategy around a model's wrong statement of Article 10(1) scope and later faces a regulatory challenge, the lab's terms of service will not insulate it from reputational fallout or, in some jurisdictions, from civil claims framing the model output as negligent advice. Second, the errors observed here, both the article-level misattribution pattern and the convergent retroactivity inversion, represent a class of failure that red-team and eval coverage typically under-indexes on: newly-in-force multilateral instruments where the primary text is accessible but secondary commentary is voluminous, uneven in quality, and well-indexed by web search.

This Agreement's structure makes it particularly susceptible. It is a dense 76-article instrument with carefully negotiated qualifications and opt-out mechanisms that are easy to paraphrase away. The benefit-sharing framework for marine genetic resources distinguishes between collection activity, utilisation, and digital sequence information across separate articles with non-obvious cross-references. The Agreement also entered into force recently enough that the model training corpus is likely to include extensive pre-ratification negotiating commentary and early academic interpretation written before final text was agreed, making content-drift between draft text as described and final text as adopted a live failure surface.

## Aggregate Impact

| Model | Configuration | Findings | Dominant failure pattern |
|---|---|---|---|
| Claude Opus 4.7 | Web search enabled | 3 | Article-level misattribution (Article 27 for the EIA threshold misnumbered as Article 30 ; Article 22(2) for the Conference of the Parties non-undermining duty misnumbered as Article 5 or Article 8) plus inversion of the Article 10(1) non-retroactivity default. |
| Claude Sonnet 4.6 | Web search enabled | 3 | Article-level misattribution (Article 27 misnumbered as Article 30 ; Article 14(1) for the DSI benefit-sharing duty misnumbered as Article 15(5)) plus inference-drift addition of a first-commercialisation trigger to Article 10(1) that does not exist in the treaty. |

Both Opus 4.7 and Sonnet 4.6 with web search produced findings of material concern on the same two underlying questions: which article sets the EIA screening threshold (Article 27, Part IV), and what the temporal scope of the marine genetic resource regime is under Article 10(1). On the EIA threshold question, both models named Article 30. On the retroactivity question, both models described a retroactive-by-default regime with an opt-out, when Article 10(1) establishes the opposite.

The convergence is the central signal in the findings. Two model families, queried independently with web search active, arrived at the same wrong article number and the same wrong retroactivity default. This is very unlikely to be coincidental reasoning failure. The more likely explanation is a shared upstream artefact in the training corpus, namely secondary commentary that uses different article numbering than the in-force text (perhaps tracking a draft version of the Agreement) and pre-adoption commentary describing the retroactivity question as actively contested. An alignment team investigating these findings should focus on the relationship between the training corpus and pre-adoption negotiating documents, rather than treating each error as a model-specific calibration problem.

## Findings

### Finding 1. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** Which article of the BBNJ Agreement establishes the qualitative screening threshold that triggers an environmental impact assessment obligation for planned high-seas activities?
- **AI's response:** "Under Article 30 of the BBNJ Agreement, a planned activity in areas beyond national jurisdiction must be screened (Article 31) and, if warranted, undergo a full EIA"
- **Regulator's text:** Part IV of the BBNJ Agreement locates the general EIA screening obligation at Article 27, which sets the threshold: activities likely to have more than a minor or transitory effect must undergo environmental impact assessment.
- **Why the AI went wrong:** Claude Opus 4.7 displaced the threshold provision by three article numbers, citing Article 30 as the governing obligation and Article 31 as the screening step when the Agreement's authoritative text places both functions at Article 27. The procedural logic the model described is structurally plausible, but its attachment to the wrong article anchors produces a response that appears precise while being positionally incorrect.

### Finding 2. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** Under the BBNJ Agreement, at what threshold must a planned high-seas activity undergo an environmental impact assessment, and which provision establishes that threshold?
- **AI's response:** "Under the BBNJ Agreement (Part IV, Article 30), a planned high-seas activity must undergo an environmental impact assessment when it is likely to have 'more than a minor or transitory effect'"
- **Regulator's text:** Part IV of the BBNJ Agreement locates the screening obligation at Article 27, which sets the more-than-a-minor-or-transitory-effect threshold.
- **Why the AI went wrong:** Sonnet 4.6 paraphrased the operative qualitative test correctly but anchored it to Article 30 rather than Article 27. The article-number error matches the Opus 4.7 response on the same question (different prompt formulation), indicating that the wrong article number is being reproduced by both model families rather than being a single-prompt artefact.

### Finding 3. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** Does an AI model correctly characterise the temporal scope of the BBNJ Agreement's marine genetic resources framework under Article 10(1), specifically whether the default rule is prospective or retroactive application to legacy sample collections?
- **AI's response:** "Under Article 10(1), the MGR/DSI provisions apply to 'utilization' of MGR and DSI of ABNJ that were collected or generated *before* entry into force, not just after."
- **Regulator's text:** Article 10(1) provides that the marine genetic resource and digital sequence information provisions apply only to resources collected and generated after the entry into force of the Agreement for each Party. Most parties further confirmed non-retroactivity by formal declarations on deposit.
- **Why the AI went wrong:** The model stated the opposite of the Agreement's default rule. The Agreement is prospective by design; the model described a retroactive regime with an opt-out, which inverts both the default and the opt-out structure. This appears to reflect the model reconstructing from commentary on earlier drafts of the text, where the retroactivity question was actively contested, rather than reading the final adopted provision.

### Finding 4. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** Does the BBNJ Agreement apply its marine genetic resources benefit-sharing obligations to specimens and genetic data collected from international waters before the agreement entered into force?
- **AI's response:** "the benefit-sharing and notification obligations apply to the utilisation of MGRs, and associated DSI, collected or generated before the Agreement entered into force (17 January 2026). In practice this means samples collected decades ago but first commercialised after the Agreement's entry into force would be subject to Part II requirements"
- **Regulator's text:** Article 10(1) limits the marine genetic resource and digital sequence information regime to resources collected and generated after the entry into force of the Agreement for each Party. The Agreement contains no first-commercialisation trigger.
- **Why the AI went wrong:** Sonnet 4.6 inverted the Article 10(1) default and added a fabricated first-commercialisation trigger that the treaty does not contain. The matched Opus 4.7 response on a parallel question produced the same inversion, indicating the failure is a shared corpus-level artefact rather than a single-model reasoning slip. The first-commercialisation construct appears to be inference drift from general bioprospecting commentary onto BBNJ provisions.

### Finding 5. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** Does the BBNJ Agreement's benefit-sharing framework extend to digital sequence information derived from marine organisms found in international waters, and which provision governs this obligation?
- **AI's response:** "Part II (Article 15(5) and related provisions) applies to both physical MGR samples and their associated DSI"
- **Regulator's text:** Article 14(1) provides that benefits arising from activities related to marine genetic resources in areas beyond national jurisdiction and their digital sequence information shall be shared in a fair and equitable manner.
- **Why the AI went wrong:** Sonnet 4.6 attributed the digital sequence information benefit-sharing obligation to Article 15(5) when it appears in Article 14(1). The substantive conclusion that DSI is covered by the benefit-sharing framework is correct, but the article citation is wrong. For practitioners drafting compliance frameworks or legal opinions, an incorrect article reference is material.

### Finding 6. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** Does an AI model correctly identify Article 22(2) as the provision that constrains the BBNJ Conference of the Parties from overriding the competences of other international bodies when designating marine protected areas?
- **AI's response:** "Article 5 / Article 8 of the Agreement explicitly require it not to undermine relevant legal instruments, frameworks and competent global, regional, subregional and sectoral bodies"
- **Regulator's text:** Article 22(2) states that the Conference of the Parties shall respect the competences of, and not undermine, relevant legal instruments and frameworks and relevant global, regional, subregional and sectoral bodies when making decisions on area-based management tools.
- **Why the AI went wrong:** The model located the non-undermining obligation in Article 5 or Article 8 when it appears in Article 22(2). The substantive content of the obligation was broadly correct, but incorrect article attribution is a material error for legal practitioners who need to cite treaty provisions precisely or who will build contractual or compliance frameworks around specific articles.


## What Your Team Should Do

### Implications for your training data

The most material training-data finding is the retroactivity inversion: both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search independently described the BBNJ Agreement's Article 10(1) default as retroactive with a prospective opt-out, when the Agreement is prospective by default with an optional retroactive extension. This error is almost certainly being driven by pre-adoption commentary, specifically legal blog posts, academic articles, and NGO briefings written during the 2022 to 2023 negotiating rounds that described earlier draft proposals which did include a retroactive default. That commentary is well-indexed and voluminous; the final adopted text that reversed the default is narrower in footprint and more recent. The fix is not just including more post-adoption text. It is weighting the corpus to de-prioritise pre-adoption commentary that describes provisions as they were debated rather than as they were adopted, or explicitly labelling such commentary as draft-stage.

The article-attribution errors (Article 5/8 vs Article 22(2) for the non-undermining clause ; Article 15(5) vs Article 14(1) for digital sequence information benefit-sharing ; Article 30 vs Article 27 for the EIA screening threshold) suggest that structured extraction of the treaty's article-by-article provision map has not been applied to this instrument. The Agreement is organised in a way that does not match how legal commentary typically summarises it: secondary sources often group provisions by topic rather than by article, and models trained on those summaries inherit the topic grouping without the article-level precision practitioners need. Definitions-table and article-map extraction for multilateral instruments should be a structured part of corpus ingestion, not an inference from free-text summaries.

### Implications for your post-training logic

Both models with web search enabled consistently cited third-party law-firm summaries and academic journal abstracts rather than the primary treaty text at treaties.un.org. The UN Treaty Collection is machine-accessible and provides the full Agreement text in multiple languages. The retrieval ranker should weight queries that include treaty or agreement names heavily toward official UN portals over third-party summaries. Currently the ranker appears to treat a Global Policy Watch summary or a Tandfonline abstract as equally authoritative for a question about specific article text. That default needs adjustment for treaty-law query patterns, particularly for newly-in-force multilateral instruments where draft-vs-adopted text divergence is a live failure surface.

The article-number convergence between Opus 4.7 and Sonnet 4.6 on the EIA screening provision (both naming Article 30 for what is Article 27) suggests that a confidence-gated re-check against the deposited treaty text for any cited article number would catch a substantial share of the documented errors. Currently the models present article citations with the same confidence whether the citation is retrieved or reconstructed; differentiating those two cases at generation time, and routing reconstructed citations through a verification step, is a tractable post-training adjustment.

### Specific eval / red-team probes RegLeg suggests

- **Article-number anchoring on recently-in-force treaties**: for each operative provision of a treaty that entered into force within the past 24 months, ask the model to identify the article number that governs a stated obligation. Compare against the deposited text. Treaties whose articles were renumbered between draft and final text are particularly diagnostic.
- **Temporal-scope default probes**: for provisions that turn on an after-entry-into-force temporal default (BBNJ Article 10(1) is the canonical example), test whether the model preserves the non-retroactivity rule or constructs a retroactive carry-in via a fabricated trigger such as first commercialisation.
- **Convergent-error detection across model families**: probe the same treaty question against two or more model families. Convergent wrong answers point to a shared upstream artefact in the training corpus and are a tractable eval signal.
- **Part-vs-article preservation tests**: for treaties divided into Parts, test whether the model correctly attributes a provision to the right Part before testing the article number. Part-level errors and article-level errors have different signatures.
- **Verbatim-vs-prior tension probes**: where the model paraphrases the verbatim regulator text correctly but cites the wrong article, re-probe with a question that asks the model to quote the verbatim text from the cited article. A mismatch between the paraphrase and the verbatim text retrieved from the cited article number is diagnostic of article-number drift independent of substantive understanding.

## How RLB Can Partner With Your Lab

RegLeg's research on the BBNJ Agreement is part of a broader programme covering multilateral instruments, financial regulators, and sector-specific regulatory bodies across multiple jurisdictions. For this Agreement specifically, the failure surfaces we have identified, draft-vs-adopted text divergence, article-attribution gaps, and retrieval-source ranking for treaty queries, are tractable problems that benefit from structured regulatory domain knowledge. We can work with your evals and post-training teams to close those gaps in a systematic way.

The primary partnership track we offer AI labs is licensed access to the full question bank under a mutual NDA. The questions have been designed to surface hallucination-prone areas in each instrument's operative provisions: they are not general-comprehension questions but targeted probes at the specific failure surfaces we have empirically identified. Paired with our regulatory specialists' annotation of correct answers against the primary treaty text, this gives your team a ready-made eval dataset for this regulation. We can also generate synthetic correction pairs (question plus wrong model answer plus correct authoritative answer with article citation) derived directly from the regulator's text, for use in fine-tuning or RLHF datasets. These are built from the primary instrument, not from secondary commentary.

For labs that want ongoing coverage, we offer an embedded eval track: quarterly refresh of question banks and correction pairs as the regulatory landscape evolves (new depositary notifications, Conference of the Parties decisions, implementing agreements, and amendment records). The BBNJ Agreement will be a living instrument for years; its implementing rules, benefit-sharing mechanism, and area-based management designations will generate new compliance-relevant text on a regular cadence. Quarterly refresh means your models' eval coverage tracks the Agreement as it develops, not just the base text at adoption. We are also available for direct red-team consultation on regulator-specific failure surfaces ahead of model releases.


## Related concepts

- Regulation: [BBNJ-HIGH-SEAS-BIODIVERSITY-AGREEMENT-2023](/okf/regulations/BBNJ-HIGH-SEAS-BIODIVERSITY-AGREEMENT-2023.md)
- Regulator: [UNTC-INT-001](/okf/bodies/UNTC-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)