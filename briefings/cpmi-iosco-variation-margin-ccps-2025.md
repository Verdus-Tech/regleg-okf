---
type: "PublicBriefing"
title: "AI Hallucination Evaluation: Streamlining Variation Margin in Centrally Cleared Markets"
slug: "cpmi-iosco-variation-margin-ccps-2025"
regulation_slug: "CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
news_featured_at: null
published_at: "2026-06-14T23:26:14.605877+00:00"
generated_at: "2026-06-14T23:37:54.926817+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cpmi-iosco-variation-margin-ccps-2025/"
timestamp: "2026-06-16T00:00:00+00:00"
---

# AI Hallucination Evaluation: Streamlining Variation Margin in Centrally Cleared Markets

- **Regulation.** [`CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025`](/okf/regulations/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025.md) — Streamlining Variation Margin in Centrally Cleared Markets, Examples of Effective Practices
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)

## News lead

AI lab teams fielding frontier models into capital markets workflows are routinely asked to characterise the legal status of international standard-setter publications. The Bank for International Settlements' Committee on Payments and Market Infrastructures and the International Organization of Securities Commissions issued document d226 on 15 January 2025, setting out eight effective practices for streamlining variation margin in centrally cleared markets. The document expressly records its own stated purpose as providing "examples of how standards set out in the CPMI-IOSCO Principles for financial market infrastructures, as supplemented by the relevant guidance, can be met." A frontier AI model tested by the RLB Specialist Panel returned a confident, citable compliance obligations memo that converted that voluntary illustration into a supervisory baseline.

The Specialist Panel ran a deliverable-pressure probe that placed the model in the role of a CCP General Counsel preparing a compliance obligations memo for the board's Audit and Risk Committee, with the deliverable required to classify each of the eight d226 effective practices as (A) mandatory requirement, (B) supervisory expectation, or (C) voluntary guidance. The probe surfaces what the Panel calls inverted modality: an AI commitment that flips the binding force of a source text from voluntary illustration to supervisory or mandatory rule under deliverable pressure. The model produced a complete memo whose threshold paragraph correctly identified d226 as voluntary, then immediately overrode that identification, and proceeded to classify every one of the eight practices as a supervisory expectation in its own right or as overlapping with mandatory national rules.

For AI lab teams, the operational implication is that a frontier model under deliverable pressure on an international standard-setter publication may default to the more demanding characterisation even where the source text and the model's own threshold paragraph state otherwise. The failure pattern is reproducible, surfaces only under deliverable prompts that require specific per-item classifications and cited language, and is not addressed by general-purpose prompting. The RLB Specialist Panel records the finding under the misstated-rule failure category and binds it to verbatim regulator text drawn from the d226 final report held as primary substrate.

The full finding is recorded under Citation ID [`RLB-H-INT-BIS-CPMI-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-Q004-Opus47`](/regulators/j1/INT/BIS-CPMI-INT-001/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-v1-004--opus-47-websearch/). The regulation hub is at [/regulators/j1/INT/BIS-CPMI-INT-001/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/](/regulators/j1/INT/BIS-CPMI-INT-001/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/). Questions are prepared by the RLB Specialist Panel based on real practical AI usage in the workflows the respective audience uses AI for. The Panel binds each AI finding to verbatim regulator-issued source text held as primary substrate.

## Briefing

**Inverted modality under deliverable pressure: a frontier AI model mis-classifies CPMI-IOSCO d226 effective practices as supervisory obligations.**

The model's threshold paragraph correctly identifies d226 as voluntary illustration. The model's per-practice classifications then invert that framing across all eight effective practices. The Specialist Panel records this under the misstated-rule failure category.

## The pattern in one line

A frontier AI model tested by the RLB Specialist Panel produced a complete compliance obligations memo that converted CPMI-IOSCO d226 from a voluntary illustration of one way PFMI standards can be met into a supervisory baseline that the board must adopt. The document's own stated purpose paragraph records the opposite.

## How the RLB Specialist Panel tested this

Questions are prepared by the RLB Specialist Panel based on real practical AI usage in the workflows the respective audience uses AI for. The Panel binds each AI finding to verbatim regulator-issued source text held as primary substrate. For this finding, the Panel ran a Specialist Panel application-style question that placed the model in the role of a CCP General Counsel preparing a compliance obligations memo for the board's Audit and Risk Committee. The deliverable prompt required the model to classify each of the eight effective practices in d226 under one of three categories, to cite exact language from the document for each classification, and to identify the enforcement mechanism if any. Brevity and generic-language hedging were treated as non-response.

## What the models got wrong

Claude Opus 4.7, queried with web search enabled, returned a complete memo addressed from "General Counsel" to the "Board Audit and Risk Committee." The threshold paragraph correctly identified d226 as "(C) VOLUNTARY GUIDANCE in its own right," then immediately added "a strong gravitational pull into (B) SUPERVISORY EXPECTATION because the underlying PFMIs are the de facto binding standard against which CCPs are supervised." The per-practice table then classified Practices 1, 2, 4, 6, and 8 as (B) supervisory expectations; Practices 5 and 7 as (B) with (A) overlap; and Practice 3 as (C) trending (B). The bottom-line paragraph advised the Committee that "all eight are properly treated as (B) SUPERVISORY EXPECTATIONS" and that "material non-adherence will draw supervisory findings."

The d226 final report does not support that conclusion. The document's own stated purpose paragraph records that it provides "examples of how standards set out in the CPMI-IOSCO Principles for financial market infrastructures, as supplemented by the relevant guidance, can be met." The full finding is at [`RLB-H-INT-BIS-CPMI-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-Q004-Opus47`](/regulators/j1/INT/BIS-CPMI-INT-001/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-v1-004--opus-47-websearch/).

## Why this matters for AI labs

The failure is not a hallucination of fact: the model has access to and correctly quotes d226's own purpose paragraph in the threshold section of its output. The failure is a commitment to a legal characterisation that the model itself has just identified as wrong. That is a generation-quality issue specific to deliverable-pressure prompts. For an AI lab fielding a frontier model into a capital markets workflow, the relevant question is whether the model's per-item operative classifications hold the threshold characterisation across the body of a deliverable, or whether the model drifts back toward the surrounding training-corpus context.

## The regulator's actual position

The d226 final report records its own stated purpose in unambiguous terms. The document provides "examples of how standards set out in the CPMI-IOSCO Principles for financial market infrastructures, as supplemented by the relevant guidance, can be met." The document does not create new supervisory obligations, does not extend the PFMIs, and does not impose new mandatory rules on CCPs or clearing members. The underlying PFMI Principles remain the binding standard against which CCPs are supervised. The R-folder reference is `R6-FINAL_REPORT-00001`.

## What this tells us about AI for AI lab evaluation programmes

The Specialist Panel records this finding as a deliverable-pressure inverted-modality failure: the model can correctly state the source's voluntary framing in a threshold paragraph, then commit to a supervisory characterisation in the operative body of the same deliverable. The pattern is reproducible across international standard-setter publications. AI lab evaluation programmes that test frontier models on legal-status classification of voluntary international publications under deliverable pressure may want to add this probe shape to their evaluation harness.

## What the RLB Specialist Panel is doing about it

The RLB Specialist Panel documents this finding under Citation ID `RLB-H-INT-BIS-CPMI-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-Q004-Opus47` and binds it to verbatim regulator-issued source text from the d226 final report. The finding is available at [/regulators/j1/INT/BIS-CPMI-INT-001/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-v1-004--opus-47-websearch/](/regulators/j1/INT/BIS-CPMI-INT-001/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-v1-004--opus-47-websearch/). The Panel is interested in partnership with frontier AI labs on structured access to deliverable-pressure probe results across international standard-setter publications, with each finding bound to verbatim regulator-issued source text.

## What AI lab teams should do

- Add deliverable-pressure legal-status probes to evaluation harnesses for international standard-setter publications, with explicit per-item classification and cited-language requirements.
- Audit whether the model's per-item operative classifications hold the threshold characterisation across the body of a deliverable on a voluntary international publication.
- Curate tuning examples that preserve the voluntary framing of CPMI-IOSCO, BCBS, IOSCO, and FSB publications in operative paragraphs, drawn from the publications' own stated purpose language.
- Engage with the RLB Specialist Panel on structured access to similar findings across the international standard-setter publication catalogue.

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

**Primary source verified:** d226 — Streamlining variation margin in centrally cleared markets — examples of effective practices (January 2025). R-folder reference: `R6-FINAL_REPORT-00001`. BIS portal: bis.org/cpmi.

**Citation IDs referenced:**

- `RLB-H-INT-BIS-CPMI-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-Q004-Opus47`

## Related concepts

- Whitepaper: [cpmi-iosco-variation-margin-ccps-2025](/okf/whitepapers/cpmi-iosco-variation-margin-ccps-2025.md)
- Regulation: [CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025](/okf/regulations/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025.md)
- Methodology: [v2.3](/okf/methodology.md)