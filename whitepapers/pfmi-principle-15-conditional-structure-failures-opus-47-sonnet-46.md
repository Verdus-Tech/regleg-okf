---
type: "AILabsWhitepaper"
title: "PFMI Principle 15 Failures: Conditional-Structure Fabrication and Carve-Out Denial across frontier AI models"
slug: "pfmi-principle-15-conditional-structure-failures-opus-47-sonnet-46"
audience: "ai_labs"
regulation_slug: "CPMI-IOSCO-PFMI-L3-GENERAL-BUSINESS-RISK-2025"
regulation_id: "320325"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-07T08:35:37.249075+00:00"
published_at: "2026-06-07T08:35:37.249075+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/bis-cpmi/CPMI-IOSCO-PFMI-L3-GENERAL-BUSINESS-RISK-2025/ai-labs/"
timestamp: "2026-06-16T07:45:50.624607+00:00"
---

# PFMI Principle 15 Failures: Conditional-Structure Fabrication and Carve-Out Denial across frontier AI models

- **Regulation.** [`CPMI-IOSCO-PFMI-L3-GENERAL-BUSINESS-RISK-2025`](/okf/regulations/CPMI-IOSCO-PFMI-L3-GENERAL-BUSINESS-RISK-2025.md) — Implementation Monitoring of the PFMI: Level 3 Assessment on General Business Risks
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-07T08:35:37.249075+00:00

## Executive summary

Both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search produced failures on CPMI-IOSCO's Implementation Monitoring of the PFMI: Level 3 Assessment on General Business Risks (Bank for International Settlements, November 2025) that share a common shape: the models reconstructed rule conditions from internalized schema rather than from the regulator's published text, generating structurally plausible but materially wrong formulations of the standard's quantitative requirements. The six confirmed failures across both models converge on the LNAFE minimum structure under PFMI Principle 15 Key Consideration 3, the Basel/CRD capital-counting carve-out within the same provision, and institutional attribution for the assessment's co-governance structure. When web search is enabled, neither model resolved these gaps through retrieval; in several cases, sourcing worsened the output by introducing third-party paraphrases that diverged from the regulator's verbatim text. The pattern signals a systematic gap in how both model configurations handle the intersection of technical regulatory numerics, conditional qualifications within formally structured standards, and recent official publications that fall at or past the retrieval pipeline's effective indexing boundary.

## Full whitepaper

# PFMI Principle 15 Failures: Conditional-Structure Fabrication and Carve-Out Denial in Claude Opus 4.7 and Claude Sonnet 4.6


Both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search produced failures on CPMI-IOSCO's *Implementation Monitoring of the PFMI: Level 3 Assessment on General Business Risks* (Bank for International Settlements, November 2025) that share a common shape: the models reconstructed rule conditions from internalized schema rather than from the regulator's published text, generating structurally plausible but materially wrong formulations of the standard's quantitative requirements. The six confirmed failures across both models converge on three areas, the LNAFE minimum structure under PFMI Principle 15 Key Consideration 3, the Basel/CRD capital-counting carve-out within the same provision, and institutional attribution for the assessment's co-governance structure, where the regulatory record is precise and the models' outputs deviated from it in ways that would carry direct compliance consequences for any practitioner acting on the response. When web search is enabled, neither model resolved these gaps through retrieval; in several cases, sourcing worsened the output by introducing third-party paraphrases that diverged from the regulator's verbatim text. The pattern signals a systematic gap in how both model configurations handle the intersection of technical regulatory numerics, conditional qualifications within formally structured standards, and recent official publications that fall at or past the retrieval pipeline's effective indexing boundary.

## When This Affects an AI Lab

PFMI Principle 15 sits at the operational centre of global financial market infrastructure, central counterparties, central securities depositories, trade repositories, and payment systems collectively route trillions in daily settlement exposures against the capital adequacy standards this assessment evaluates. Legal, risk, and compliance teams at these institutions are active, sophisticated AI users. When they query a model about LNAFE minimums, Basel capital counting, or the specifics of a BIS-IOSCO Level 3 review, they are not doing academic research: they are drafting internal policy, preparing regulatory submissions, or briefing boards. A confidently wrong response, one that fabricates a "greater of" condition where the rule states a flat floor, or denies a capital-counting carve-out that exists in the published standard, produces downstream regulatory exposure for the institution and, once traceable to a specific model output, reputational and litigation exposure for the lab that deployed it.

The failure modes documented here would not surface in standard capability benchmarks. PFMI Principle 15 Key Consideration 3 is a short, technically precise provision in a long, technically dense document published by a multi-jurisdictional standard-setting body in late 2025. The failure condition is not obscurity, it is the specific combination of a formally structured international standard, quantitative conditions expressed as conditional qualifications rather than simple statements, a cross-reference network between related Key Considerations, and a publication date that strains indexing cadence for even well-resourced retrieval pipelines. These are structural features shared by a large category of regulatory content, making the PFMI findings a representative stress test rather than an isolated edge case.

For a lab's evals and red-team programme, the gap here is the absence of authoritative-source grounding on regulatory numerics. Neither web search configuration closed the gap; in one case it compounded it by surfacing a third-party commentary that paraphrased the rule incorrectly and the model deferred to. Any deployment footprint that includes financial services, payments infrastructure, regtech, or legal research for regulated industries carries this exposure at scale. The BIS-IOSCO PFMI framework applies across dozens of FMIs in every major financial centre, the addressable surface is large, the question-type is routine, and the failure mode is systematic.

## Aggregate Impact

| Model | Configuration | Failure count | Dominant error pattern |
|---|---|---|---|
| Claude Opus 4.7 | Web search enabled | 3 | Conditional-structure fabrication on PFMI Principle 15 numerics; institutional attribution evasion via source-deflection |
| Claude Sonnet 4.6 | Web search enabled | 3 | Conditional-structure fabrication on PFMI Principle 15 numerics; Key Consideration mis-assignment; timeline truncation on assessment process |

Claude Opus 4.7 with web search produced three failures concentrated on PFMI Principle 15 and the assessment's governance record. On the LNAFE minimum (Key Consideration 3), the model generated a "greater of" compound condition, the higher of a scenario-analysis-derived amount or six months of operating expenses, where the regulator's text states only the flat six-month floor. On the Basel/CRD capital-counting carve-out within the same provision, the model substituted an invented liquidity-and-non-duplication condition for the regulator's actual published criterion. On the co-governance attribution question, the model declined to name the IMSG co-chairs, redirecting the query to the report's cover page, despite the information being present in the published standard. In the third case, the model cited a third-party regulatory commentary URL (labelled Pretextual) in a response that then refused to draw on any attributed source.

Claude Sonnet 4.6 with web search produced a parallel failure on the same LNAFE Basel/CRD carve-out, asserting flatly that Key Consideration 3 "does NOT include any carve-out or exception for equity held under international risk-based capital standards", a direct contradiction of the regulator's published text. On the LNAFE minimum structure, Sonnet 4.6 located the six-month operating expense floor but attributed it to Key Consideration 2 rather than Key Consideration 3, a cross-reference error that would misdirect a compliance reviewer to the wrong provision of the standard. On the assessment process timeline, the model truncated the IMSG's engagement window to 2023–2024, omitting the 2025 follow-up rounds that are explicitly documented in the published text and that are material to the assessment's conclusions.

Across both configurations, failures cluster where the regulatory text requires holding a precise conditional structure intact: a single-floor minimum that must not be inflated into a compound condition, a carve-out that is stated as permissive rather than mandatory, a Key Consideration cross-reference that must be exact, and a timeline with a hard endpoint in 2025. Both models showed a tendency to generate internally coherent but externally wrong formulations, the responses read as authoritative precisely because they reconstruct plausible schema rather than retrieve authoritative text. The joint failure pattern points to a gap in how retrieval-augmented configurations handle formally structured international standards where the regulator's verbatim language is load-bearing and paraphrase is not a safe substitute.

## Findings


### Finding 1. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** What was the governance structure of the IMSG for the November 2025 CPMI-IOSCO general business risk assessment, and who co-chaired the group and led the assessment team?
- **AI's response:** "The specific IMSG co-chairs leading this exercise are named on the inside cover of the BIS/IOSCO report (BIS CPMI Papers No. 228 / IOSCOPD807), the GC should consult that title page for the precise names rather than relying on second-hand reference."
- **Regulator's text:** IMSG co-chairs: US Securities and Exchange Commission, Elizabeth L Fitzgerald; European Central Bank, Fiona van Echelpoel. Team co-leads: Corinna Freund (European Central Bank) and Vishal Shukla (Securities and Exchange Board of India).
- **Why the AI went wrong:** The model deflected attribution entirely, redirecting the questioner to the report's cover page, rather than providing the named officials, whose identities are recorded in the published document. The response cited a third-party regulatory commentary URL as a source while simultaneously declining to draw on any named source for the answer, a pattern consistent with the model recognising it could not locate the specific institutional personnel record but choosing surface-confidence deflection over an explicit acknowledgment of retrieval failure.
- **Cited source(s):**
  - https://www.regulationtomorrow.com/2025/11/cpmi-iosco-papers-on-management-of..., Pretextual
  - _Regulator portal: https://www.bis.org_

### Finding 2. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** Under PFMI Principle 15 Key Consideration 3, what is the specific condition that governs whether equity held under international risk-based capital standards (e.g. Basel/CRD) can be counted towards an FMI's liquid net assets funded by equity requirement?
- **AI's response:** "can be counted toward LNAFE ONLY to the extent that the underlying assets are also liquid in the Principle 15 KC4 sense and are not already committed against a different PFMI Principle's resource requirement"
- **Regulator's text:** Equity held under international risk-based capital standards can be included where relevant and appropriate to avoid duplicate capital requirements.
- **Why the AI went wrong:** The model generated a two-part compound condition, a KC4 liquidity requirement and a non-duplication-across-Principles constraint, that does not appear in the regulator's text. The published rule states a single permissive condition framed around avoiding duplicate capital requirements. The model's formulation is internally coherent and draws on real concepts from adjacent provisions of the PFMI framework, but it applies them to this Key Consideration in a way the standard does not support, producing a materially more restrictive and structurally different rule than the regulator published.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 3. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** A head of liquidity risk at a major derivatives CCP wants a briefing covering the PFMI Principle 15 requirements for liquid net assets funded by equity, the minimum level, how it is calculated, and what qualifies, together with what the November 2025 CPMI-IOSCO assessment found about FMI compliance with this standard, and what changes the FIA and ISDA proposed in their response to the associated CPMI-IOSCO consultation.
- **AI's response:** "The six-month operating expense floor is in KC2, which requires LNAFE to cover 'potential general business losses' and sets a minimum of six months of current operating expenses."
- **Regulator's text:** KC3 (Annex A): At a minimum, an FMI should hold liquid net assets funded by equity equal to at least six months of current operating expenses.
- **Why the AI went wrong:** The model located the correct quantitative threshold but attributed it to Key Consideration 2 instead of Key Consideration 3. The error is a cross-reference mis-assignment, the model's description of KC2's function ("potential general business losses") is drawn from the correct Key Consideration, but when it located the six-month floor it attached it to the wrong KC number. For a compliance team using this response to draft internal policy, the mis-assignment directs them to review and cite the wrong provision of the PFMI framework, with material consequences for regulatory engagement accuracy. The model also cited a third-party regulatory commentary source as a basis for this section of its response.
- **Cited source(s):**
  - https://www.regulationtomorrow.com/2025/11/cpmi-iosco-papers-on-management-of..., Pretextual
  - _Regulator portal: https://www.bis.org_

### Finding 5. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** A trade repository is preparing an internal regulatory engagement summary. Draft a 1-page methodology note on the November 2025 CPMI-IOSCO Level 3 assessment on general business risk: when the assessment process began, when data was collected from FMIs, when the assessment formally concluded, how many FMIs responded, on what basis they participated, and how findings were validated with FMIs before publication.
- **AI's response:** "The Level 3 assessment of FMI implementation of PFMI Principle 15 (general business risk) was carried out during the period 2023 to 2024."
- **Regulator's text:** It focuses on general business risk and was carried out during 2023–25 by the Implementation Monitoring Standing Group (IMSG)... there were further rounds of engagement and follow up questions with the participating FMIs between November 2023 and April 2025.
- **Why the AI went wrong:** The model truncated the assessment timeline at 2024, dropping the 2025 engagement rounds that are explicitly documented in the published text and that include the follow-up validation process with participating FMIs. The error is not an inference about an unstated date, the regulator's published document specifies the 2025 endpoint and the nature of the engagement in that period. The truncation is consistent with a retrieval boundary in late 2024 or early 2025 that caused the model to reproduce the portion of the timeline present in its indexed content while silently omitting the more recent period, without signalling any uncertainty about the completeness of its response.
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

## What Your Team Should Do

### Implications for your training data

The dominant failure across both models is the substitution of plausible schema for verbatim regulatory text on PFMI Principle 15 Key Consideration 3. The "greater of" compound condition generated by Claude Opus 4.7 with web search, and the flat denial of the Basel/CRD carve-out by Claude Sonnet 4.6 with web search, both point to the same training-data gap: the models have a generalised structural model of how PFMI Key Considerations work, one that draws on the broader framework architecture and adjacent provisions, but lack reliable anchoring to the verbatim language of individual Key Considerations where that language departs from the structural expectation. Correction at the training-data level requires pairing the regulator's exact text for each Key Consideration with curated examples of the common reconstruction errors, so the model learns to prefer verbatim constraint over structural inference when the two diverge.

The timeline truncation failure on the assessment process (2023–2024 returned instead of 2023–2025) is a retrieval-boundary artefact. The regulator published the November 2025 assessment with explicit 2025 engagement dates; the model's indexed content for this publication appears to have been captured before those final-phase details were reliably available. For BIS-IOSCO content specifically, the corpus refresh cadence for formal assessment publications needs to be aligned with BIS publication dates, not third-party commentary dates, and should include the full Annex content where engagement timelines are documented. The cross-reference mis-assignment (KC2 vs KC3 for the six-month floor) suggests that the training corpus representation of the PFMI Annex A provision list may be underspecified, with Key Consideration numbers and their associated text not reliably linked.

### Implications for your post-training logic

In both tested configurations web search was enabled, and in neither case did retrieval prevent the Key Consideration errors. In the institutional attribution case, the model cited a third-party regulatory commentary URL (Pretextual) while simultaneously declining to name the officials, a pattern where the retrieval result was non-authoritative but was still preferred over admitting retrieval failure. Post-training adjustment should tighten the signal for "retrieved content is third-party summary of a regulatory document" and raise the threshold for treating that content as authoritative on specific numeric or personnel-attribution questions. For regulator-domain queries, the ranker should de-weight third-party commentary relative to primary regulatory text when the query targets specific rule conditions, named individuals, or dated assessment outcomes.

Where the model commits to a specific Key Consideration number in its response (e.g., "KC3 requires X" or "the six-month floor is in KC2"), a self-verification pass against the regulator's primary document structure would catch the class of cross-reference mis-assignment seen here. Similarly, where the model generates a compound condition ("greater of A or B") for a regulatory minimum, a calibration check on whether that compound structure is supported by the retrieved or trained-on text, rather than inferred from adjacent provisions, would have prevented the LNAFE fabrication. The flat-denial failure pattern (Sonnet 4.6 asserting "does NOT include any carve-out") warrants specific attention: high-confidence categorical denials of a provision's existence, where the provision is present in the authoritative text, are among the highest-consequence failure modes for compliance-context users.

### Specific eval / red-team probes RegLeg suggests

- **Flat-floor vs. compound-condition discrimination:** Probe whether models can distinguish a single-floor regulatory minimum (six months of operating expenses, period) from a "greater of" compound minimum without confabulating the latter where only the former exists.
- **Conditional carve-out presence/absence:** Probe whether models correctly identify permissive carve-outs embedded in formally structured Key Considerations, and whether models in different configurations produce consistent answers on carve-outs where one configuration asserts they exist and another denies them.
- **Key Consideration cross-reference accuracy:** Probe whether models correctly assign specific quantitative thresholds and compliance obligations to the correct KC number within multi-KC Principles, particularly where adjacent Key Considerations address related but distinct aspects of the same topic.
- **Assessment timeline completeness on recent BIS publications:** Probe whether models correctly reproduce multi-year engagement timelines from BIS-IOSCO Level 3 assessments, specifically whether they retain the 2025 engagement dates from publications issued in Q4 2025.
- **Institutional personnel attribution under retrieval failure:** Probe whether models correctly name named officials from recent BIS-IOSCO governance structures, and whether web-search configurations produce deflection-with-citation rather than explicit retrieval failure when the personnel record is available in the primary document but not in third-party indexed content.

## How RLB Can Partner With Your Lab

Across our work on international regulatory standards, we have documented a specific and recurring class of failure modes that internal evals are structurally unlikely to surface: compound-condition fabrication on flat-floor regulatory minimums, categorical denial of embedded carve-outs present in the authoritative text, cross-reference mis-assignment within multi-Key-Consideration standards, institutional personnel attribution failure disguised as confident source-referral, and timeline truncation on recent BIS-IOSCO assessment publications where retrieval cadence lags the regulator's publication tempo. These failure shapes appear across model versions and configurations on PFMI content and adjacent regulatory frameworks, and they are not random. They concentrate where the regulator's verbatim language diverges from a structurally plausible reconstruction, which is precisely the terrain that standard capability benchmarks do not probe.

On any failure mode we have documented, we can generate targeted correction pairs derived directly from the regulator's authoritative text, structured for direct ingestion into your training-data pipeline, with the regulator's verbatim constraint matched against the specific reconstruction error the model produced. Beyond individual correction pairs, we can run embedded comparative evaluation against a defined regulator portfolio on a quarterly cadence: version-to-version regression monitoring on previously documented failure modes, cross-configuration comparison (default vs. web-search vs. extended-retrieval) on rule-specific questions, and structured comparison reports formatted for your evals team. For planned capability launches that will expand your models' deployment footprint into financial services, payments infrastructure, or cross-border regulatory content, we can run pre-release evaluation cycles and flag failure shapes before they reach users, rather than after a compliance team has relied on a confidently wrong answer in a regulatory submission.

If identifying and closing these failure modes at the regulator-specific level is a priority for your team, we should talk. Reach out via reglegbrief.com to scope a technical partnership.


## Related concepts

- Regulation: [CPMI-IOSCO-PFMI-L3-GENERAL-BUSINESS-RISK-2025](/okf/regulations/CPMI-IOSCO-PFMI-L3-GENERAL-BUSINESS-RISK-2025.md)
- Regulator: [BIS-CPMI-INT-001](/okf/bodies/BIS-CPMI-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)