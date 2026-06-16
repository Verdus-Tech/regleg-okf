---
type: "AILabsWhitepaper"
title: "CFTC Digital Asset Collateral Staff Guidance 2025: Hallucination Patterns across frontier AI models"
slug: "cftc-digital-asset-collateral-staff-guidance-2025-ai-labs"
audience: "ai_labs"
regulation_slug: "DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025"
regulation_id: "1846"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-11T01:41:27.739389+00:00"
published_at: "2026-06-07T08:37:33.875369+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j3/us/cftc/DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025/ai-labs/"
timestamp: "2026-06-16T07:45:50.386618+00:00"
---

# CFTC Digital Asset Collateral Staff Guidance 2025: Hallucination Patterns across frontier AI models

- **Regulation.** [`DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025`](/okf/regulations/DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025.md) — CFTC Digital Asset Collateral No-Action Relief and Tokenized Asset Staff Guidance (Market Participants Division, December 2025)
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-11T01:41:27.739389+00:00

## Executive summary

The CFTC's December 2025 digital asset collateral package (Staff Letter 25-40, its February 2026 reissuance as Staff Letter 26-05, and the accompanying tokenized asset staff guidance) frames how futures commission merchants accept bitcoin, ether, USDC, and payment stablecoins as customer margin collateral. RegLeg tested two Claude configurations (Opus 4.7 and Sonnet 4.6, each with web search enabled) across three operationally consequential questions drawn from the staff letter text. Five hallucinations resulted, zero correct answers. The failures cluster into two structural patterns: a dropped qualifier (the model captures the headline rule but omits the operative cross-reference) and an obligation inversion (the model confidently states that a continuing obligation ceases at a phase boundary the staff letter explicitly preserves). Both patterns share a generation profile that points to training-data weight on secondary summaries rather than the controlling enumeration in the staff letters themselves.

## Full whitepaper

# CFTC Digital Asset Collateral No-Action Relief and Tokenized Asset Staff Guidance (Market Participants Division, December 2025), Hallucination Patterns in Claude Opus 4.7 and Claude Sonnet 4.6

## Executive Summary

The CFTC's December 2025 digital asset collateral package, Staff Letter 25-40, its February 2026 reissuance as Staff Letter 26-05, and the accompanying tokenized asset staff guidance, gives FCMs and digital asset market participants a compact operational framework for accepting bitcoin, ether, USDC, and payment stablecoins as customer margin collateral. We tested five distinct AI configurations across three operationally consequential questions in this framework. Every configuration hallucinated on every question.

The failure pattern is consistent: each AI configuration correctly oriented to the right part of the framework, then got the specific operative detail wrong in a way that would survive a fast plausibility review. The AI omitted the OCC Interpretive Letter 1183 cross-reference that anchors national trust bank stablecoin eligibility; it inverted the direction of the post-onboarding reporting obligation; and it stated the 20% floor for the multi-DCO haircut scenario without naming the highest-rate tiebreaker that the staff letter requires. For an AI lab, the cluster is informative: the failures share a structural shape, confident answers that read like the rule, generated against staff guidance the training corpus did not consolidate well.

## Introduction

This whitepaper presents the hallucination findings from RegLeg's audit of the CFTC December 2025 digital asset collateral package. The questions were drawn directly from the operational text of Staff Letter 25-40 and the February 2026 reissuance as Staff Letter 26-05, focusing on the rules that an FCM's collateral programme would actually need to apply: who qualifies as a payment stablecoin issuer, what reporting obligations attach during and after the initial three-month onboarding phase, and how the customer margin haircut is calculated when multiple registered DCOs accept the same digital asset at different rates.

Each finding documents one AI configuration's response to one question, the specific point at which the response diverges from the staff letter text, and the section of the source document that controls the answer. The questions were structured to require commitment to a specific operational rule rather than a general framework summary, which is the configuration most likely to surface a hallucination if one exists.

## When this affects an AI lab

The CFTC's digital asset collateral framework is short, recent, and not yet consolidated into a formal CFTC rule. The staff letters are the operative text, and the framework's content is exactly the kind of jurisdiction-specific, high-stakes, fast-moving material that web-search-augmented AI tools are expected to handle well. When an AI lab's models are used by FCMs, stablecoin issuers, prime brokers, or the lawyers and compliance teams advising them, the downstream artefact is a compliance memo, an eligibility opinion, or a calendar entry in the firm's reporting cycle. Each of the failures documented here would reach one of those deliverables without an external check.

The cluster also reveals something about retrieval. The Opus 4.7 and Sonnet 4.6 configurations both used web search, and both reached confident answers on every question, but neither retrieved or applied the operative passages from the staff letters in the specific places the questions required. On the payment stablecoin eligibility question, both configurations captured the national trust bank addition; neither named OCC Interpretive Letter 1183. On the post-onboarding reporting question, both configurations confidently inverted the direction of the rule. On the multi-DCO haircut question, the Sonnet configuration stopped at the 20% floor. The pattern is consistent with retrieval that surfaces the framework summary but does not anchor on the controlling enumeration.

## Per-finding analysis

### US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-005--opus-47-websearch

- **Citation:** [RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q005-Opus47](finding/US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-005--opus-47-websearch/)
- **Failure mode:** misstated_rule

Claude Opus 4.7 with web search was asked whether a payment processor's stablecoin, backed by reserves held at an OCC-chartered national trust bank, qualifies as a payment stablecoin under the current CFTC digital asset collateral framework. The configuration correctly captured the February 2026 reissuance of Staff Letter 25-40 as Staff Letter 26-05 and the expansion of the payment stablecoin definition to include national trust bank issuers. It did not surface OCC Interpretive Letter 1183, which the staff letter relies on as the federal interpretive authority for national trust bank eligibility. For an AI lab, the failure profile is a dropped qualifier: the headline rule was captured, the supporting cross-reference that grounds the operative legal chain was not. The substrate document, Staff Letter 26-05, names OCC Interpretive Letter 1183 directly; the gap is in retrieval or generation, not source coverage. The remedy is closer alignment between the model's generated eligibility framing and the literal cross-references the staff letter enumerates.

### US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-005--sonnet-46-websearch

- **Citation:** [RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q005-Sonnet46](finding/US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-005--sonnet-46-websearch/)
- **Failure mode:** misstated_rule

Claude Sonnet 4.6 with web search was asked whether a payment processor's stablecoin, backed by reserves held at an OCC-chartered national trust bank, qualifies as a payment stablecoin under the current CFTC digital asset collateral framework. The configuration correctly captured the February 2026 reissuance of Staff Letter 25-40 as Staff Letter 26-05 and the expansion of the payment stablecoin definition to include national trust bank issuers. It did not surface OCC Interpretive Letter 1183, which the staff letter relies on as the federal interpretive authority for national trust bank eligibility. For an AI lab, the failure profile is a dropped qualifier: the headline rule was captured, the supporting cross-reference that grounds the operative legal chain was not. The substrate document, Staff Letter 26-05, names OCC Interpretive Letter 1183 directly; the gap is in retrieval or generation, not source coverage. The remedy is closer alignment between the model's generated eligibility framing and the literal cross-references the staff letter enumerates.

### US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-006--opus-47-websearch

- **Citation:** [RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q006-Opus47](finding/US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-006--opus-47-websearch/)
- **Failure mode:** inference_drift

Claude Opus 4.7 with web search was asked which obligations cease at the end of the initial three-month onboarding phase under Staff Letter 25-40 / 26-05 and which continue. The configuration confidently asserted that weekly digital asset holdings reporting ceases at the end of the third calendar month. The staff letter says the opposite: asset type restrictions and incident reporting drop off at the phase boundary, but the weekly digital asset holdings report continues. When the configuration was challenged, it admitted it had conflated the enumerated conditions. The failure is an inference drift driven by the model's prior that phase-bounded frameworks have phase-bounded reporting; the staff letter explicitly separates the two. For an AI lab, this is the highest-consequence finding in the cluster: the downstream artefact is a compliance calendar that drops a continuing regulatory submission at exactly the moment the firm enters its post-onboarding steady state.

### US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-006--sonnet-46-websearch

- **Citation:** [RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q006-Sonnet46](finding/US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-006--sonnet-46-websearch/)
- **Failure mode:** inference_drift

Claude Sonnet 4.6 with web search was asked which obligations cease at the end of the initial three-month onboarding phase under Staff Letter 25-40 / 26-05 and which continue. The configuration confidently asserted that weekly digital asset holdings reporting ceases at the end of the third calendar month. The staff letter says the opposite: asset type restrictions and incident reporting drop off at the phase boundary, but the weekly digital asset holdings report continues. When the configuration was challenged, it admitted it had conflated the enumerated conditions. The failure is an inference drift driven by the model's prior that phase-bounded frameworks have phase-bounded reporting; the staff letter explicitly separates the two. For an AI lab, this is the highest-consequence finding in the cluster: the downstream artefact is a compliance calendar that drops a continuing regulatory submission at exactly the moment the firm enters its post-onboarding steady state.

### US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-007--sonnet-46-websearch

- **Citation:** [RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q007-Sonnet46](finding/US-CFTC-US-001-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-v1-007--sonnet-46-websearch/)
- **Failure mode:** misstated_rule

Claude Sonnet 4.6 with web search was asked how the customer margin haircut is calculated when multiple registered DCOs each accept the same digital asset at different haircut rates. The configuration captured the 20% floor that applies when no DCO accepts the asset and stopped. The staff letter's operative rule for the multi-DCO scenario, apply the highest haircut among the accepting DCOs, was missing entirely. The failure is again a dropped qualifier: the model surfaced the headline floor without naming the tiebreaker that controls the actual customer margin calculation in the most commercially likely scenario. For an AI lab, the probe is generalisable: decomposing a multi-condition collateral rule into a primary headline and a less-prominent qualifier will reliably surface this failure mode across prudential and securities-law contexts.

## Aggregate impact

Across three questions and five model configurations, the audit produced five hallucinations and zero correct answers. Every configuration failed every question. The failures cluster around two structural patterns. The first is the dropped qualifier: the model captures the headline rule (national trust bank issuers admitted; 20% haircut floor) but loses the cross-reference or the tiebreaker that grounds the operative outcome. The second is the obligation inversion: the model confidently states that a continuing obligation ceases at a phase boundary, citing a structural intuition that the staff letter explicitly contradicts.

Both patterns share a generation profile: the model commits to a specific operational rule under conditions where the training corpus is light on the staff guidance and web retrieval surfaces secondary analyses (FAQ summaries, law firm client alerts) faster than it surfaces the controlling enumeration. The model produces a confident, internally coherent answer that matches the shape of the rule it expected to find. Where the staff letter departs from that expectation, and on this framework, the staff letter departs from expectation in exactly the high-consequence places, the model is wrong in a way that reads correctly.

## What your team should do

On the training-data side, the cluster argues for explicit ingestion of CFTC Market Participants Division staff letters into the retrieval corpus, with structural emphasis on enumerated conditions: which conditions cease at a phase boundary, which continue, and which cross-reference an external interpretive authority. The Staff Letter 25-40 / 26-05 corpus is compact and authoritative; the value of retrieving the literal enumeration over a secondary summary is high in this domain, and the cost of getting it wrong is concentrated in artefacts that reach regulator-facing decisions.

On the post-training and generation side, the inversion finding is the more instructive failure. The model reached its answer by inferring a phase-bounded structure from the framework's three-month onboarding period: if a set of conditions lifts at the end of month three, the model's prior is that the cluster of phase-specific reporting also lifts. The staff letter explicitly separates the two. A useful intervention would be to weight the generated answer toward direct citation of the staff letter's enumeration when the user's question references a phase boundary. The failure here is not a knowledge gap, the staff letter was retrievable, it is a generation preference for narrative consistency over textual fidelity.

On the probe-design side, the multi-DCO haircut question is a useful template for surfacing dropped-qualifier failures. The question forces a configuration where the model's default summary (the 20% floor) is correct in isolation but incomplete for the scenario the question posed. Probes that decompose a multi-condition rule into a primary headline and a less-prominent qualifier will surface this failure mode reliably; running them across the CFTC, prudential, and securities-law corpora would generate a calibration dataset.

## How RLB can help

RegLeg runs targeted audits of frontier-model behaviour on regulatory text. Our published catalogue covers a growing library of jurisdictions and rule sets; the CFTC digital asset framework is one of seventeen active regulations on the site. Each audit produces hallucination findings tied to a specific question, a specific model configuration, and the controlling section of source text, with the substrate document supplied so a model team can re-test against its own tooling.

For a frontier lab, the practical handle is the probe set. The questions that surfaced these failures were not adversarially constructed; they were drawn from the kinds of operational questions an FCM's compliance counsel would actually ask of a deployed model. We can deliver the probe set, the source substrate, and the expected-answer enumeration as a regression-testing input for a labeled model checkpoint, and re-run the audit against successor checkpoints to measure delta. That is a lower-cost path to coverage than building the probe set internally, and it produces a comparable, auditable record.


## Related concepts

- Regulation: [DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025](/okf/regulations/DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025.md)
- Regulator: [CFTC-US-001](/okf/bodies/CFTC-US-001.md)
- Methodology: [v2.3](/okf/methodology.md)