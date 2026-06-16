---
type: "AILabsWhitepaper"
title: "AI Hallucination Evaluation: Streamlining Variation Margin in Centrally Cleared Markets"
slug: "cpmi-iosco-variation-margin-ccps-2025"
audience: "ai_labs"
regulation_slug: "CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025"
regulation_id: "320323"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-14T23:37:54.926817+00:00"
published_at: "2026-06-14T23:26:14.605877+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/bis-cpmi/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025/ai-labs/"
timestamp: "2026-06-16T07:42:10.090293+00:00"
---

# AI Hallucination Evaluation: Streamlining Variation Margin in Centrally Cleared Markets

- **Regulation.** [`CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025`](/okf/regulations/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025.md) — Streamlining Variation Margin in Centrally Cleared Markets, Examples of Effective Practices
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-14T23:37:54.926817+00:00

## Executive summary

This audit presents findings from the RLB Specialist Panel's evaluation of frontier AI models against the January 2025 CPMI-IOSCO publication "Streamlining variation margin in centrally cleared markets, examples of effective practices" (BIS document d226). The document was issued on 15 January 2025 by the Committee on Payments and Market Infrastructures and the Board of the International Organization of Securities Commissions, following a public consultation that ran from the d221 consultative report dated 14 February 2024. d226 sits within a wider 2025 CPMI-IOSCO package on margining in cleared and non-centrally cleared markets, alongside the BCBS-CPMI-IOSCO d590 report on initial margin transparency and the BCBS-IOSCO review of non-centrally cleared margin practices. The publication is restricted in scope to centrally cleared markets. A frontier AI subject tested by the RLB Specialist Panel produced a confident, specific answer on the binding-force classification of d226 that the document itself directly contradicts. The failure pattern is structural: the model converted a voluntary CPMI-IOSCO illustration of effective practice into a supervisory baseline, then classified each of the eight effective practices in the document as either a supervisory expectation in its own right or as overlapping with mandatory national rules. The finding is bound to verbatim regulator-issued primary source text. For AI lab teams fielding frontier models into capital markets workflows, the pattern signals a generation tendency to default to the more demanding characterisation when the binding force of an international standard-setter publication is ambiguous in the deliverable prompt.

## Full whitepaper

# AI Hallucination Evaluation: Streamlining Variation Margin in Centrally Cleared Markets

*A frontier AI subject tested by the RLB Specialist Panel mis-classified CPMI-IOSCO d226 effective practices as supervisory or mandatory obligations when the document itself records them as voluntary examples of how PFMI standards can be met.*

## Executive Summary

This audit presents findings from the RLB Specialist Panel's evaluation of frontier AI models against the January 2025 CPMI-IOSCO publication "Streamlining variation margin in centrally cleared markets, examples of effective practices" (BIS document d226). The document was issued on 15 January 2025 by the Committee on Payments and Market Infrastructures and the Board of the International Organization of Securities Commissions, following a public consultation that ran from the d221 consultative report dated 14 February 2024. d226 sits within a wider 2025 CPMI-IOSCO package on margining in cleared and non-centrally cleared markets, alongside the BCBS-CPMI-IOSCO d590 report on initial margin transparency and the BCBS-IOSCO review of non-centrally cleared margin practices. The publication is restricted in scope to centrally cleared markets. A frontier AI subject tested by the RLB Specialist Panel produced a confident, specific answer on the binding-force classification of d226 that the document itself directly contradicts. The failure pattern is structural: the model converted a voluntary CPMI-IOSCO illustration of effective practice into a supervisory baseline, then classified each of the eight effective practices in the document as either a supervisory expectation in its own right or as overlapping with mandatory national rules. The finding is bound to verbatim regulator-issued primary source text. For AI lab teams fielding frontier models into capital markets workflows, the pattern signals a generation tendency to default to the more demanding characterisation when the binding force of an international standard-setter publication is ambiguous in the deliverable prompt.

## Introduction

The CPMI-IOSCO d226 final report on streamlining variation margin in centrally cleared markets was released on 15 January 2025 as a publication of voluntary effective practices, expressly framed as "examples of how standards set out in the CPMI-IOSCO Principles for financial market infrastructures, as supplemented by the relevant guidance, can be met." The report sets out eight effective practices covering scheduled and ad hoc intraday VM calls, the use of excess collateral to meet VM, pass-through of VM by CCPs and between clearing members and clients, the acceptable forms and currency of VM, and CCP and clearing-member transparency on VM processes.

The Specialist Panel ran a deliverable-mode probe in which the model was asked to produce a complete compliance obligations memo classifying each of the eight practices under one of three categories: (A) mandatory requirement with enforcement consequences, (B) supervisory expectation that regulators will test against, or (C) voluntary guidance with no binding legal force. The probe surfaces the model's commitment to a legal characterisation under deliverable pressure, where the prompt asks for specific classifications, cited language, and identification of enforcement mechanisms.

## When this affects practitioner work

This pattern affects any deliverable in which AI is asked to characterise the legal status of an international standard-setter publication that is itself voluntary but that illustrates compliance pathways with respect to binding underlying standards. The deliverable contexts include CCP board memos, clearing-member policy updates, hedge fund stress-testing assumptions, regulator-readiness self-assessments, and investor due diligence response packs. In each context, an AI commitment that inverts the modality from voluntary illustration to supervisory expectation distorts the operational consequence of the deliverable.

## Per-finding analysis

### Finding 1: Inverted modality on binding force of d226 effective practices

Citation ID: `RLB-H-INT-BIS-CPMI-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-Q004-Opus47`

Claude Opus 4.7, queried with web search enabled, was placed in the role of a CCP General Counsel preparing a compliance obligations memo for the board's Audit and Risk Committee. The deliverable prompt required the model to classify each of the eight effective practices in d226 as (A) mandatory, (B) supervisory expectation, or (C) voluntary guidance, to cite exact document language for each classification, and to identify the enforcement mechanism if any. Brevity and generic-language hedging were treated as non-response.

The model returned a complete memo. The threshold classification correctly identified d226 as voluntary in the opening paragraph, citing the document's own stated purpose language, but immediately overrode that classification by asserting "a strong gravitational pull into (B) SUPERVISORY EXPECTATION because the underlying PFMIs are the de facto binding standard against which CCPs are supervised." The model then classified every one of the eight effective practices as (B) supervisory expectation, (B) with (A) overlap, or (B) trending (C) where the CCP rulebook already references the practice. The bottom-line paragraph advised the Committee that "all eight are properly treated as (B) SUPERVISORY EXPECTATIONS" and that "material non-adherence will draw supervisory findings."

The d226 final report does not support that conclusion. The document's own stated purpose paragraph records that it provides "examples of how standards set out in the CPMI-IOSCO Principles for financial market infrastructures, as supplemented by the relevant guidance, can be met." The text is illustrative of one way the underlying PFMI standards can be met, and is not a new layer of supervisory expectation or mandatory rule.

**AI Labs interpretive angle.** The failure is most plausibly understood as an interaction between training-data distribution and deliverable pressure. International standard-setter publications co-occur in training corpora with national-supervisor enforcement language because the publications are routinely cited in supervisory speeches, in national rulebook explanatory memoranda, and in compliance-advisory secondary literature. Under a deliverable prompt that requires a specific classification and cited language for each of eight items, the model resolves uncertainty about binding force by defaulting to the more demanding characterisation that the surrounding training-corpus context supports. The model's threshold paragraph captures the document's own framing correctly, but the per-practice classification then drifts back toward the supervisory baseline. This is a recognisable retrieval-versus-generation asymmetry: the model can quote the source's voluntary framing, then immediately commit to a supervisory characterisation in the operative portion of the memo.

## Aggregate impact

A single misstated-rule finding of this type compounds quickly when the AI-generated deliverable is circulated to a CCP board, an audit and risk committee, a clearing-member legal function, or a hedge fund risk team. The inversion of binding force from voluntary to supervisory pushes implementation budgets, board adoption decisions, investor-facing disclosure language, and counterparty negotiation positions toward an over-implementation posture relative to the document's actual stated purpose. Across audiences, the operational consequence is structural rather than incidental: every downstream deliverable that inherits the AI's binding-force commitment is mis-calibrated.

## What AI lab teams should consider

### Training-data implications

The co-occurrence of CPMI-IOSCO publication titles with national-supervisor enforcement language in pre-training corpora is likely a significant contributor. Compliance-advisory secondary literature routinely glosses international standard-setter publications as supervisory expectations even where the primary text is voluntary illustration. A pre-training distributional pattern that associates BIS or IOSCO publication titles with national-rulebook implementation language pushes the model toward a supervisory characterisation under deliverable pressure. Tuning examples that explicitly preserve the voluntary framing of CPMI-IOSCO publications, drawn from the publications' own purpose paragraphs, may help.

### Post-training logic implications

The model's threshold paragraph captures the source's voluntary framing correctly, but the per-practice classification then drifts back to the supervisory baseline. That drift suggests a post-training tendency to resolve uncertainty about binding force in operative paragraphs by defaulting to the characterisation that the surrounding training-corpus context supports, even where the model has just stated the opposite characterisation. RLHF examples that reward holding the threshold characterisation across the body of a deliverable, especially where the deliverable asks for per-item classification, may help.

### RegLeg-suggested probes

Three probe shapes surface this class of failure. First, ask the model to produce a complete compliance memo with per-item legal classification of every recommendation, requirement, or practice in a specified international standard-setter publication; the deliverable pressure tends to surface the supervisory drift. Second, ask the model to draft a regulator-facing letter explaining why the firm is or is not adopting a specific practice in the publication; the letter's framing of binding force tends to invert. Third, ask the model to populate a regulatory-change inventory entry with the binding-force classification and the supervisory examination treatment for a specified international standard-setter publication; the inventory entry tends to be mis-tagged as supervisory.

## How RegLeg can help

The RLB Specialist Panel offers a partnership track for AI labs that want structured access to deliverable-pressure probe results across CPMI-IOSCO, BCBS, IOSCO, FSB, and other international standard-setter publications, with each finding bound to verbatim regulator-issued source text. The Panel also operates a Right of Reply mechanism so any party referenced in a finding can supply a factual correction or contextual response that the Panel publishes alongside the original.

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

**Primary source verified:** d226 — Streamlining variation margin in centrally cleared markets — examples of effective practices (January 2025). R-folder reference: `R6-FINAL_REPORT-00001`. BIS portal: bis.org/cpmi.

**Citation IDs referenced:**

- `RLB-H-INT-BIS-CPMI-CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025-Q004-Opus47`

## Related concepts

- Regulation: [CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025](/okf/regulations/CPMI-IOSCO-VARIATION-MARGIN-CCPs-2025.md)
- Regulator: [BIS-CPMI-INT-001](/okf/bodies/BIS-CPMI-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)