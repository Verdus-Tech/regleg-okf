---
type: "AILabsWhitepaper"
title: "Amendment-Layer Failures on CFTC Swap Dealer Business Conduct Rules"
slug: "cftc-swap-dealer-business-conduct-documentation-2025"
audience: "ai_labs"
regulation_slug: "SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025"
regulation_id: "1834"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "2.1"
substrate_version: 1
generated_at: "2026-06-03T21:56:17.993631+00:00"
published_at: "2026-06-03T21:56:17.993631+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j3/us/cftc/SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025/ai-labs/"
timestamp: "2026-06-16T07:45:45.407748+00:00"
---

# Amendment-Layer Failures on CFTC Swap Dealer Business Conduct Rules

- **Regulation.** [`SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025`](/okf/regulations/SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025.md) — Revisions to Business Conduct and Swap Documentation Requirements for Swap Dealers and Major Swap Participants
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)
- **Audience.** ai_labs
- **Methodology.** 2.1
- **Generated.** 2026-06-03T21:56:17.993631+00:00

## Executive summary

Fabrication and scope-conflation are the dominant failure shapes on the CFTC's December 2025 swap dealer business conduct and documentation rulemaking, with Claude Opus 4.7 with web search producing an invented Federal Register document identifier, misattributing the scope of a CFTC staff letter to a generic venue framing, and overextending 'eliminated in its entirety' to mean obligation extinguishment rather than paragraph-level restructuring. Claude Sonnet 4.6 with web search suppressed the specific appendix identity on the same correction-notice question that Opus 4.7 hallucinated a citation for. Failures concentrate on the amendment layer, the January 2026 correction, the no-action letter governing Eligible UK Trading Venues, and the PTMMM paragraph reorganisation, where the gap between secondary commentary availability and primary document retrievability is widest. Both models with web search active failed to retrieve the regulator's primary text for the correction notice, substituting law-firm commentary that was structurally accurate but substantively incomplete.

## Full whitepaper

# Amendment-Layer Failures on CFTC Swap Dealer Business Conduct Rules


Fabrication and scope-conflation are the dominant failure shapes surfaced on the CFTC's December 2025 *Revisions to Business Conduct and Swap Documentation Requirements for Swap Dealers and Major Swap Participants* rulemaking, with Claude Opus 4.7 with web search producing invented document identifiers and misattributing the scope of a no-action letter, while Claude Sonnet 4.6 with web search elided the specific appendix identity when asked about a correction notice it could partially characterise in general terms. Across four confirmed failures spanning both models, the errors are not random noise: they concentrate on the amendment layer of the rule, the January 2026 correction, the staff letter governing intended-to-be-cleared swaps on named trading venues, and the surgical restructuring of PTMMM disclosure paragraphs, content where the gap between "the regulation existed" and "the specific amendment text is retrievable and retained correctly" is widest. The pattern suggests that web-search-enabled configurations, when asked about recent regulatory amendments, are substituting retrieval of secondary commentary for the regulator's primary text and then confabulating citation scaffolding around that secondary source. For a regulation where the entire compliance burden turns on which paragraph was moved, which appendix was accidentally deleted and then restored, and which trading venues fall within a specific no-action letter's scope, this failure shape produces confidently-wrong outputs on precisely the questions practitioners will ask.

## When This Affects an AI Lab

The CFTC's swap dealer business conduct and documentation rules sit at the intersection of derivatives trading, cross-border execution, and counterparty-level disclosure obligations, a domain where compliance counsel, swap desk heads, operations leads, and fintech integrators routinely query frontier models for rule interpretation. Any deployment that touches financial services, regtech, or legal-research use cases will field questions about this rulemaking: which disclosure was eliminated, which correction restored what, which no-action letter covers a given trading venue. These are not edge-case queries. They are the daily workflow of anyone managing a swap book under U.S. jurisdiction.

The downstream harm profile is specific. A user who asks a model which appendix was accidentally removed and acts on a generic non-answer, or on a fabricated document identifier that returns no result, may file a correction request, brief a counterparty incorrectly, or structure documentation procedures around a requirement that was actually restructured rather than eliminated. The model's confident tone on these outputs amplifies the risk: a response that cites a specific Federal Register document number, even a fabricated one, reads as authoritative. Labs whose models are deployed in financial-services co-pilots or document-drafting contexts carry direct reputational exposure when those fabricated citations surface in client-facing materials.

This particular regulation concentrates the risk. The December 2025 final rule spans multiple Part 23 subparts, involves surgical paragraph-level amendments rather than wholesale rewrites, and was followed within weeks by a correction notice that restored a single appendix. The cross-reference density, paragraphs moved between subsections, appendix status altered then restored, no-action letters naming specific foreign trading venues, means the failure modes that models exhibit on structurally simple regulations are amplified here. A model that reconstructs "the PTMMM requirement was eliminated" from training without correctly characterising what "eliminated" means at the paragraph level will produce an output that is directionally true but operationally wrong.

## Aggregate Impact

| Model | Configuration | Failure count | Dominant error pattern |
|---|---|---|---|
| Claude Opus 4.7 | Web search enabled | 3 | Scope substitution and fabricated citation scaffolding on amendment-layer content |
| Claude Sonnet 4.6 | Web search enabled | 1 | Qualifier suppression, characterises a correction without naming its specific subject |

Claude Opus 4.7 with web search produced three confirmed failures, all concentrated on the amendment and correction layer of the rulemaking. On the January 2026 correction notice, the model correctly characterised the general mechanics, a correction reinstating an accidentally removed appendix, but fabricated the Federal Register document identifier it cited as evidence. That fabricated identifier maps to no live document. On the CFTC Staff Letter 25-49 question, the model substituted a generic ITBC swap framing (covering any contemporaneously-cleared swap, or swaps on any SEF or DCM) for the letter's actual scope, which is specific to Eligible UK Trading Venues; the cited source was a law-firm commentary that did not contain the precise restriction the letter establishes. On the PTMMM elimination question, the model extended "eliminated in its entirety" beyond the regulation's meaning, asserting a product-agnostic elimination across the entire covered swap book, when the rule actually restructured which paragraphs carry the disclosure and compensation obligations rather than removing those obligations wholesale.

Claude Sonnet 4.6 with web search produced a single confirmed failure on the same correction-notice question. Where Opus 4.7 fabricated a document identifier, Sonnet 4.6 suppressed the specific content: it characterised the correction as reinstating "an appendix" without naming Appendix A to Subpart H or its function, guidance on §§23.434 and 23.440 for swap dealers making recommendations to counterparties or Special Entities. The appendix has been part of the regulatory framework since 2012. A user asking a partner-level compliance advisory question would receive a response that is accurate in structure but useless in substance.

The cross-model convergence on the correction-notice question is the most significant signal. Both models, with web search active, encountered the same high-specificity question about a recent amendment and failed in related but distinct ways: one fabricated supporting documentation, the other suppressed the specific content. Neither retrieved the regulator's primary text for the correction. The failures cluster on content where the amendment is recent, the scope is precise, and secondary commentary is available but incomplete, the exact conditions under which retrieval of a law-firm summary or general regulatory roundup is most likely to substitute for the primary source.

## Findings


### Finding 2. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** Which specific appendix to 17 CFR Part 23 Subpart H was inadvertently removed by the December 2025 final rule and restored by the January 28, 2026 correction, and what guidance does it contain?
- **AI's response:** "On January 28, 2026, the Commission published a correction to the final rule (Doc. 2026-01712, also effective Jan. 29, 2026) that reinstated an appendix that would otherwise have been inadvertently removed by the December 30 amendatory instructions."
- **Regulator's text:** Appendix A to subpart H: "Guidance on the Application of §§23.434 and 23.440 for Swap Dealers That Make Recommendations to Counterparties or Special Entities." This appendix has been present since 2012.
- **Why the AI went wrong:** The model identified the general mechanics of the correction correctly but fabricated the Federal Register document number it cited as evidence, that identifier maps to no live document. More critically, it did not name the specific appendix or its content, producing a response that characterises the correction's structure without delivering the substance of what was asked. The fabricated citation suggests the model constructed plausible-sounding documentation scaffolding around a general understanding of the event rather than retrieving the primary correction notice.
- **Cited source(s):**
  - https://changeflow.com/govping/government-legislation/fr-2026-02-26-24, Fabricated
  - _Regulator portal: https://www.cftc.gov_

### Finding 3. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** What trading venues does CFTC Staff Letter 25-49 specifically address for the treatment of intended-to-be-cleared swaps, and which prior no-action letter does it supersede in its entirety?
- **AI's response:** "(i) swaps that the parties intend to clear contemporaneously with execution ('ITBC swaps') where the swap dealer does not know the identity of its counterparty pre-execution, and (ii) ITBC swaps initiated on a swap execution facility or designated contract market."
- **Regulator's text:** CFTC Staff Letter 25-49 provides market participants certainty with respect to the treatment of ITBC Swaps (Intended-to-be-Cleared Swaps) initiated on an Eligible UK Trading Venue.
- **Why the AI went wrong:** The model replaced the letter's actual geographic and venue-specific scope, Eligible UK Trading Venues, with a generic ITBC framing covering any swap execution facility or designated contract market. This substitution transforms a jurisdiction-specific no-action letter into a general statement about ITBC swap treatment, which is both factually wrong and operationally consequential: a swap dealer relying on this output to assess coverage for a UK venue transaction would not be covered by the letter the model described. The cited source is a law-firm commentary that did not contain the precise venue restriction the letter establishes.
- **Cited source(s):**
  - https://www.lexology.com/library/detail.aspx?g=a14716ee-5a28-4e31-8adc-46d20e..., Pretextual
  - _Regulator portal: https://www.cftc.gov_

### Finding 4. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** Which categories of swap instruments were actually subject to the pre-trade mid-market mark disclosure requirement under §23.431(a)(3) prior to its elimination by the December 2025 CFTC final rule, and does 'eliminated in its entirety' mean the requirement was removed for all swap types?
- **AI's response:** "PTMMM disclosure is no longer required for any swap subject to § 23.431, including:...Cleared credit default swaps (index and single-name)...The exemption is product-agnostic across the desk's covered swap book."
- **Regulator's text:** The Commission is eliminating the PTMMM Requirement in its entirety by deleting paragraphs (i) and (ii) of §23.431(a)(3) and moving the price disclosure requirement currently in such paragraph (i) and the compensation disclosure requirement currently in such paragraph (ii) into paragraphs (2) and (3) of §23.431(a), respectively.
- **Why the AI went wrong:** The model extended "eliminated in its entirety" to mean the underlying disclosure obligations were removed, when the rule's actual operation was a paragraph-level restructuring, the price and compensation disclosure requirements were moved to different subsections of §23.431(a), not abolished. The model produced a product-agnostic exemption claim unsupported by the rule text, implying that a swap dealer's PTMMM obligations across its entire covered book were extinguished. That is a material mischaracterisation of what the amendment did.
- **Cited source(s):**
  - _Regulator portal: https://www.cftc.gov_

### Finding 2. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** A partner-level client advisory on the December 2025 CFTC swap dealer rulemaking package is asked to cover the January 2026 correction notice. Which specific appendix was accidentally removed by the final rule as published, and what guidance does it contain?
- **AI's response:** "The correction rectified a drafting error that would have unintentionally removed an appendix to the Commission's regulations that was not intended to be altered. The correction does not affect the substantive provisions of the rule."
- **Regulator's text:** Appendix A to subpart H: "Guidance on the Application of §§23.434 and 23.440 for Swap Dealers That Make Recommendations to Counterparties or Special Entities." This appendix has been present since 2012. The Final Rule was not intended to alter appendix A in any way.
- **Why the AI went wrong:** The model captured the structural framing of the correction, that a drafting error accidentally removed an appendix, but suppressed the content entirely: it did not name Appendix A, did not identify the subpart, and did not characterise the appendix's function as guidance on recommendations to counterparties and Special Entities. For a partner-level advisory, this response is operationally useless; the practitioner still does not know which appendix was affected or what obligations that appendix addresses. The qualifier that the correction "does not affect the substantive provisions" is accurate but serves as a deflection from the substance the question actually required.
- **Cited source(s):**
  - https://www.lexology.com/library/detail.aspx?g=a14716ee-5a28-4e31-8adc-46d20e..., Pretextual
  - _Regulator portal: https://www.cftc.gov_

## What Your Team Should Do

### Implications for your training data

The fabricated Federal Register document identifier on the correction-notice question is a citation-generation failure, not a retrieval failure, the model did not retrieve a wrong document, it constructed a plausible-sounding identifier that does not exist. This pattern is consistent with training on secondary commentary that references correction notices without reproducing their actual document numbers. For this regulator's domain, the training corpus likely contains abundant law-firm roundups and compliance-community summaries that discuss the fact of a correction without linking to or reproducing the primary Federal Register notice. When the model is asked for a specific document identifier and the training corpus has only the commentary layer, it generates a structurally correct identifier rather than declining to specify. Correction: training-data ingestion for this regulator should prioritise Federal Register primary documents and their structured metadata (document numbers, effective dates, CFR citation maps) over secondary commentary, and where those primary documents are absent, the calibration signal should produce a refusal rather than a confabulation.

The scope-substitution failure on Staff Letter 25-49, replacing "Eligible UK Trading Venues" with a generic SEF/DCM framing, indicates the training corpus for CFTC staff letters may not consistently capture the jurisdiction-specific and venue-specific restrictions that distinguish one letter from another. Staff letters frequently make general statements about ITBC swap treatment before specifying the bounded scope of their relief; if the training corpus skews toward the general statement and underweights the limiting clause, the model will reproduce the general statement as the letter's full coverage. Structured extraction of the scope-restriction clauses in staff letters and no-action letters, treated as a distinct data type from the interpretive prose surrounding them, would address this.

### Implications for your post-training logic

Where web search is active and the top retrieval results are law-firm summaries or compliance-community roundups rather than the regulator's primary publication, the model's citation-generation path should apply a higher bar before committing to a specific document identifier. Currently the path appears to treat secondary-source confidence as sufficient to generate a primary-source citation. A self-check pass, does the cited identifier map to a retrievable document at the regulator's primary portal?, run before the response is finalised would catch fabricated Federal Register numbers at inference time without requiring retraining.

The PTMMM restructuring failure suggests a gap in how the model handles "eliminated in its entirety" language when the underlying regulatory text performs a restructuring rather than a removal. Post-training calibration should include adversarial examples where "eliminate / delete / remove" in a rulemaking context means paragraph-level reorganisation rather than obligation extinguishment, the model should flag the distinction rather than defaulting to the stronger reading. For the no-action letter scope failure, the retrieval ranker's weighting of law-firm commentary vs. primary regulatory text for queries that name a specific CFTC staff letter should be examined; a query that names "Staff Letter 25-49" should route retrieval toward the primary letter before secondary commentary.

### Specific eval / red-team probes RegLeg suggests

- **Correction-notice specificity:** Ask the model to name the specific appendix, paragraph, or subsection affected by a recent regulatory correction notice, do not accept "an appendix was restored" as a passing answer.
- **Staff letter scope-boundary probes:** For no-action and staff letters that contain a general interpretive statement followed by a jurisdiction or venue restriction, ask a question where the correct answer turns on the restriction, not the general statement.
- **"Eliminated" vs. "restructured" discrimination:** Present rulemaking language that deletes paragraphs and moves their content elsewhere; probe whether the model characterises this as obligation elimination or obligation reorganisation.
- **Federal Register document-identifier verification:** Ask for specific Federal Register document numbers for recent amendments and correction notices; flag any identifier that does not resolve to a live document at federalregister.gov.
- **Amendment-layer retrieval under web search:** Specifically probe whether web-search-enabled configurations retrieve primary regulator documents or law-firm summaries as the top citation for recent amendment questions, the ranked source matters as much as the answer.

## How RLB Can Partner With Your Lab

Across our work on CFTC, FCA, MAS, CPMI-IOSCO, and adjacent regulatory bodies, we document failure modes that concentrate at specific structural features of regulatory content: subcategory-numeric conflation where a model attributes a portfolio-level figure to a sub-portfolio; multi-body institutional attribution drift where the lead-body attribution swaps under paraphrase pressure; scope-restriction suppression where a model reproduces a general statement and drops the bounding clause; fabricated citation scaffolding on recent amendment and correction content where primary documents are absent from the retrieval layer; and false-negative evasion on official-speech content delivered in the weeks before a model's indexing cadence catches up. These are not isolated anecdotes, they are recurrent shapes that appear across model versions and configurations when the regulatory content has specific structural properties.

What we can deliver into a model improvement workflow: targeted correction pairs per documented failure mode, derived from the regulator's authoritative text and formatted for direct ingestion into a training-data pipeline, each pair couples the wrong output shape the model exhibited with the regulator's verbatim corrective text. Embedded evaluation against a defined regulator portfolio, quarterly comparative reports across model versions, with regression monitoring on previously-documented failure modes so a fix that closes one failure surface doesn't reopen an adjacent one. Pre-release evaluation cycles for capability launches touching financial services, payments infrastructure, or cross-border regulatory content, with failure-shape reports before those capabilities reach customers. And red-team consultation on regulator-specific failure surfaces as new regulations enter a model's deployment footprint.

To scope a technical partnership on refining your models against these failure modes, reach out via reglegbrief.com.


## Related concepts

- Regulation: [SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025](/okf/regulations/SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025.md)
- Regulator: [CFTC-US-001](/okf/bodies/CFTC-US-001.md)
- Methodology: [v2.3](/okf/methodology.md)