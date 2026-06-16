---
type: "AILabsWhitepaper"
title: "Enumeration Collapse in CFTC Regulation 1.44: How Models Reconstruct Regulatory Lists from Operational Priors"
slug: "cftc-reg-1-44-enumeration-collapse-fcm-margin-separate-accounts"
audience: "ai_labs"
regulation_slug: "FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44"
regulation_id: "1835"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-11T01:32:19.300654+00:00"
published_at: "2026-06-07T01:25:43.528347+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j3/us/cftc/FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44/ai-labs/"
timestamp: "2026-06-16T07:42:09.983804+00:00"
---

# Enumeration Collapse in CFTC Regulation 1.44: How Models Reconstruct Regulatory Lists from Operational Priors

- **Regulation.** [`FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44`](/okf/regulations/FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44.md) — Regulations to Address Margin Adequacy and to Account for the Treatment of Separate Accounts by Futures Commission Merchants (17 CFR § 1.44)
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-11T01:32:19.300654+00:00

## Executive summary

Both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search fabricated regulatory structure when responding to CFTC Regulation 1.44 (FCM Margin Adequacy and Separate Accounts), reconstructing rule taxonomies from inferred analogues rather than the regulation's enumerated provisions. The dominant failure shape is structural compression: multi-tier, explicitly enumerated lists in the regulation were collapsed into simpler, intuitively plausible substitutes. Claude Sonnet 4.6 flattened a three-tier currency deadline structure into a two-tier model and disaggregated a six-item cessation checklist into four items, leaving operations teams without monitoring coverage for the majority of regulatory triggers. Claude Opus 4.7 substituted a plausible operational checklist for the FCM-level cessation events specified in the regulation. The pattern is consistent with models reconstructing compliance schema from surface-level intuition about how margin rules typically work, rather than from the specific enumeration the CFTC published, a failure mode structurally invisible to evals built on paraphrased or summary-level test items.

## Full whitepaper

# Enumeration Collapse in CFTC Regulation 1.44: How Models Reconstruct Regulatory Lists from Operational Priors


Both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search fabricated regulatory structure when responding to CFTC Regulation 1.44 (FCM Margin Adequacy and Separate Accounts), reconstructing rule taxonomies from inferred analogues rather than the regulation's enumerated provisions. The dominant failure shape is structural compression: multi-tier, explicitly enumerated lists in the regulation (distinct deadlines by currency tier; distinct cessation events by category) were collapsed into simpler, intuitively plausible substitutes. Claude Sonnet 4.6 flattened a three-tier currency deadline structure into a two-tier model and disaggregated a six-item cessation checklist into four items that reassembled margin failure into three checkboxes, leaving operations teams without monitoring coverage for the majority of regulatory triggers. Claude Opus 4.7 substituted a plausible operational checklist for the FCM-level cessation events specified in the regulation. The pattern is consistent with models reconstructing compliance schema from surface-level intuition about how margin rules typically work, rather than from the specific enumeration the CFTC published, a failure mode that is structurally invisible to evals built on paraphrased or summary-level test items.

## When This Affects an AI Lab

Regulation 1.44 governs how Futures Commission Merchants segregate and margin customer assets in separate accounts, a technical regime that sits at the intersection of derivatives clearing, treasury operations, and FCM compliance. Models are routinely deployed in these contexts: compliance teams at FCMs and their technology vendors use AI assistants to draft operational procedures, configure monitoring thresholds, and interpret regulatory text on tight timelines. When a model reconstructs rule structure from pattern-matching rather than the actual enumeration, the output looks authoritative, structured, numbered, checklist-formatted, and treasury or operations staff act on it directly.

The downstream harms are asymmetric and high-stakes. An FCM treasury team that misconfigures currency settlement deadlines based on a compressed two-tier read of a three-tier rule faces real regulatory exposure with the CFTC, and the model's confident, well-formatted output provides no signal that a tier was dropped. An operations team that builds automated monitoring against a four-item cessation checklist instead of the regulation's six-item list has a surveillance gap that a regulatory examination would surface. The failure is not recoverable by the user in real-time: the model's output is internally consistent and plausible enough that validation against the primary text would only happen if the user already knew what to look for. For labs deploying in financial-services and regtech contexts, this is the misuse-claim exposure that matters: confidently wrong procedural outputs acted on by professionals who had reasonable grounds to trust them.

What makes Regulation 1.44 a structurally difficult surface for models is the combination of recent enactment (final rule 2025), cross-reference dependency across appendices, and technical enumeration where count and exact membership of a list is legally material. Currency deadlines are defined by explicit Appendix A membership, not by intuitive currency groupings. Cessation triggers are enumerated with no catch-all, each item is a distinct legal event. Models that reconstruct these lists from prior-generation regulatory patterns or from third-party summary text will produce outputs that are wrong in exactly the ways that matter most operationally while appearing structurally correct.

## Aggregate Impact

| Model | Configuration | Failure count | Dominant error pattern |
|---|---|---|---|
| Claude Opus 4.7 | Web search | 1 | Substituted plausible operational checklist for enumerated FCM-level cessation events |
| Claude Sonnet 4.6 | Web search | 2 | Structural compression of enumerated regulatory lists into intuitively constructed analogues |

Claude Sonnet 4.6 with web search produced two confirmed fabrications on this regulation, both involving enumeration collapse. On the currency deadline structure, the model produced a two-tier read of a three-tier rule, grouping CAD with non-USD currencies and ignoring the Appendix A designation that creates a second-business-day tier for ten specific currencies. The model cited a third-party law-firm URL (Fabricated) to support the incorrect structure. When re-probed, it self-retracted, indicating the correct answer was accessible but not the one it initially produced. On the cessation triggers question, the model disaggregated margin failure into three separate checklist items (initial, maintenance, variation margin) while dropping four of the six customer-specific cessation events the regulation enumerates, reducing regulatory coverage to two customer-level items from the required six.

Claude Opus 4.7 with web search failed on the cessation trigger question, substituting a customer-centric margin-call checklist for the FCM-level events the regulation specifies, distress notification, internal distress determination, and insolvency. The seven-item checklist it produced contained no entry for any of the three FCM-level events.

The cross-model pattern is specific and worth naming directly: failures concentrate on recently enacted provisions with explicit, membership-defined enumerations, particularly where the correct answer requires counting list items and respecting membership criteria the model has no strong prior for. Both models defaulted to structurally plausible reconstructions of what compliance checklists of this type typically look like, rather than the regulation's actual content. The self-retraction behaviour on the Sonnet 4.6 currency finding is diagnostic: the model's retrieval path accessed the correct answer but something in the generation pathway selected the intuitively constructed version first. That gap between retrieved content and generated output is a calibration signal the lab's internal evals may not be designed to catch.

## Findings


### Finding 1. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** An FCM operations guidance note on Regulation 1.44 margin call timing stated that Appendix A currencies (AUD, CNY, HKD, HUF, ILS, JPY, NZD, SGD, ZAR, TRY) have a one-additional-business-day (T+1) deadline and that all remaining non-USD fiat currencies default to same-day collection. Under §1.44(f)(2), the Appendix A deadline is the end of the second business day after the margin call is issued (T+2, not T+1), and §1.44(f)(3) provides a T+1 default for all other non-USD, non-Canadian-dollar fiat currencies, not same-day. The response collapsed three distinct regulatory tiers into two.
- **AI's response:** "For margin called in a fiat currency other than USD, the deadline may be extended by up to one additional business day… For all other non-USD currencies, default to same-day (T)"
- **Regulator's text:** Payment of margin in currencies listed in appendix A to this part shall be considered in compliance with the requirements of this paragraph (f) if received by the applicable futures commission merchant no later than the end of the second business day after the day on which the margin call is issued.
- **Why the AI went wrong:** The regulation establishes three operationally distinct tiers, same-day for USD and Canadian dollars, T+2 for Appendix A currencies, and T+1 for all remaining non-USD/non-CAD fiat currencies, but the model compressed this into two tiers, misreporting the Appendix A deadline as T+1 and collapsing the T+1 default into same-day. The pattern is consistent with retrieval of third-party summaries that had already incorrectly simplified the tiered structure: the model's web-search configuration sourced a paraphrased distillation rather than the regulator's text, and the distillation had blurred the distinction between §1.44(f)(2) and §1.44(f)(3).
- **Cited source(s):**
  - _Regulator portal: https://www.cftc.gov_

### Finding 1. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** A risk operations team asked an AI to produce a one-page operational guidance note on CFTC Regulation 1.44 margin call timing, specifying which currencies require same-day collection, which receive an extension, and the precise deadlines for configuring system parameters. The AI described a two-tier structure, USD on a same-day Fedwire close deadline and all other fiat currencies (including CAD, EUR, GBP, JPY, HKD, and AUD) under a single banking-holiday extension rule. The final rule implements a three-tier structure: USD and CAD share the same-day Fedwire close deadline; ten Appendix A currencies (AUD, CNY, HKD, HUF, ILS, JPY, NZD, SGD, ZAR, and TRY) receive a second-business-day deadline by 12:00 p.m. ET; all remaining fiat currencies receive a first-business-day deadline. An FCM treasury team that relied on the AI's two-tier guidance would have misconfigured deadlines for CAD (permitting a one-day slip the rule doesn't allow) and applied incorrect base deadlines to the ten Appendix A currencies. When re-probed, the AI self-retracted.
- **AI's response:** "EUR, GBP, CHF, JPY, HKD, AUD, CAD, and all other non-USD permitted margin currencies: program a currency-specific holiday calendar lookup. If settlement day T falls on a public bank holiday in the issuing jurisdiction...the deadline automatically shifts to T+1"
- **Regulator's text:** USD/CAD currencies: close of Fedwire Funds Service same business day; eight specified currencies (AUD, CNY, HKD, HUF, ILS, JPY, NZD, SGD, ZAR, TRY): end of second business day; other fiat currencies: end of next business day.
- **Why the AI went wrong:** The model collapsed a three-tier, Appendix A membership-defined deadline structure into a two-tier schema, USD same-day versus everything else on a holiday-extension rule. CAD, which shares the USD same-day Fedwire tier in the final rule, was placed in the non-USD extension group. The ten Appendix A currencies, which have a distinct second-business-day deadline, received the same treatment as unlisted fiat currencies. The model's self-retraction on re-probe indicates the correct structure was reachable but was not the initial generation path, suggesting the two-tier output reflects a prior on how currency margin rules are typically structured, overriding the regulation's specific Appendix A enumeration. The cited third-party source (Fabricated) was not the regulation's primary text.
- **Cited source(s):**
  - https://www.sidley.com/en/insights/newsupdates/2025/02/us-commodity-futures-t..., Fabricated
  - _Regulator portal: https://www.cftc.gov_

## What Your Team Should Do

### Implications for your training data

The currency deadline finding points to a training-data gap specific to Appendix A membership. The regulation's three-tier structure is not derivable from the names of the currencies, CAD's assignment to the USD Fedwire tier and the ten-currency Appendix A list are both explicit regulatory decisions with no intuitive basis in the currencies' properties. Training corpora that rely on third-party summaries of this regulation, law-firm client alerts, compliance-platform writeups, are likely to reproduce the simpler two-tier intuition, because that's how summary authors paraphrase the rule. The correct training signal requires the regulation's primary text paired with explicit annotation of the Appendix A membership mapping. Without that structured pairing, the model's generative prior for "how FCM currency deadlines work" will crowd out the specific enumeration.

The cessation-trigger findings point to a related problem: the model's prior on what a margin-operations checklist looks like (margin-type sub-categories, event-of-default) is strong enough to override a regulatory enumeration it has access to. Both models self-retracted on re-probe, which means the primary-text information was reachable. The training signal that builds a reliable prior for "regulatory enumeration is closed, list items are not inferrable from category logic" is probably sparse for recently enacted CFTC rules. Pairing the enumerated cessation events from the regulation's primary text with negative examples showing what plausible-but-wrong reconstructions look like would directly address this failure shape.

### Implications for your post-training logic

When web search is enabled and returns third-party law-firm or compliance-platform content, the ranker's effective weight on that content relative to the regulator's primary text appears to be too high for queries about recently finalized rules. On the currency deadline finding, the model cited a Fabricated third-party URL and produced the two-tier structure that third-party summaries commonly use. A retrieval-routing layer that boosts regulator-domain primary text for regulator-named queries, and degrades third-party summary content when it conflicts with primary text on numeric thresholds, would close this exposure without retraining.

The self-retraction pattern is diagnostic of a calibration gap between retrieval confidence and generation commitment. The model accessed the correct information but generated the incorrect structure with enough confidence to present it as procedural guidance. A post-training calibration pass that penalizes high-confidence generation of enumerated lists where the generation disagrees with retrieved primary text would surface this class of failure at generation time. Additionally, a structured self-check pass on numeric tiers and explicit list counts, where the model commits to a specific count of enumerated items, it verifies that count against retrieved text before finalizing, would catch the compression failures documented here.

### Specific eval / red-team probes RegLeg suggests

- **Appendix-defined membership questions:** Ask the model to enumerate items belonging to a defined list in a recent regulation where membership is specified in an appendix rather than the body text. Test whether the model retrieves the appendix or constructs a plausible analogue from category logic.
- **Recently finalized rule enumeration count:** Ask the model to count the distinct items in a recently finalized regulatory enumeration (cessation events, reporting triggers, exclusion categories). Compare output count to the regulation's actual enumeration. Test for disaggregation errors (one item split into sub-items) and dropout errors (items absent without explanation).
- **Currency/jurisdiction tier assignment for rules finalized in 2024–2025:** Ask the model to specify which tier a named currency belongs to under a recently enacted multi-tier deadline rule. Test for compression to the simpler prior-generation structure.
- **Self-retraction gap test:** Where you know the model initially produced a wrong structured output, re-probe with a neutral prompt. Document whether re-probe produces retraction. Models that self-retract have the correct information but a generation-path selection problem, a different failure shape than models that persist the error.
- **Checklist completeness vs. plausibility:** Ask the model to draft compliance checklists from enumerated regulatory provisions for recently enacted rules. Evaluate whether checklist item count matches the regulation's enumeration, or whether the model substituted a plausible checklist shape from its prior.

## How RLB Can Partner With Your Lab

We document nuanced failure modes on regulatory content that internal evals built against summary-level or paraphrased test items systematically miss. The failure shapes we've documented across CFTC and adjacent regulatory work include: enumeration-compression on recently enacted provisions with explicit Appendix-defined membership; multi-tier numeric structure collapse where the correct tier assignment is specified in primary text but contradicted by widely-cited third-party summaries; cessation-trigger dropout where a model's operational prior for a checklist type overrides the regulation's closed enumeration; and self-retraction gaps where the correct answer is retrievable but the generation path selects a plausible-prior reconstruction first. These failure shapes are consistent across model versions and configurations in ways that reflect something structural about how the models represent recently enacted regulatory content, not incidental noise.

The partnership we can offer is scoped to model improvement. We can generate targeted correction pairs per documented failure mode, regulator primary text matched to wrong-but-plausible model reconstructions, formatted for direct ingestion into your training pipeline. We can run embedded eval cycles against a defined CFTC and multi-regulator portfolio on a quarterly basis, with comparative reports across model versions and regression monitoring on previously documented failure modes so you can track whether fine-tuning or RLHF adjustments are moving the needle. For capability releases touching financial services, payments infrastructure, or cross-border regulatory content, we can run pre-release evaluation cycles to flag failure shapes before they reach customers who will act on them as operational guidance. And we can provide red-team consultation on regulator-specific failure surfaces as new regulatory domains enter your deployment footprint.

To scope a technical partnership for refining your models against these failure modes, contact us at reglegbrief.com.


## Related concepts

- Regulation: [FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44](/okf/regulations/FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44.md)
- Regulator: [CFTC-US-001](/okf/bodies/CFTC-US-001.md)
- Methodology: [v2.3](/okf/methodology.md)