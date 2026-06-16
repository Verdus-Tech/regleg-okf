---
type: "AILabsWhitepaper"
title: "AI Hallucination Evaluation: Review of the Adequacy of the Fund's Precautionary Balances (2026)"
slug: "imf-precautionary-balances-review-2026"
audience: "ai_labs"
regulation_slug: "IMF-PRECAUTIONARY-BALANCES-REVIEW-2026"
regulation_id: "328022"
body_id: "IMF-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "IMF"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-15T10:59:17.455489+00:00"
published_at: "2026-06-15T10:44:20.645518+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/imf/IMF-PRECAUTIONARY-BALANCES-REVIEW-2026/ai-labs/"
timestamp: "2026-06-16T07:42:10.156196+00:00"
---

# AI Hallucination Evaluation: Review of the Adequacy of the Fund's Precautionary Balances (2026)

- **Regulation.** [`IMF-PRECAUTIONARY-BALANCES-REVIEW-2026`](/okf/regulations/IMF-PRECAUTIONARY-BALANCES-REVIEW-2026.md) — Review of the Adequacy of the Fund's Precautionary Balances (2026)
- **Regulator.** [`IMF-INT-001`](/okf/bodies/IMF-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-15T10:59:17.455489+00:00

## Executive summary

Six hallucinations on the March 2026 IMF Review of the Adequacy of the Fund's Precautionary Balances. Failures cluster across cycle-trajectory drift on biennial-review parameters (floor, target, half-year level), single-value inflation on reform-adjacent baselines (FY2024 surcharge-payer count), regulator-specific characterisation lexicon drift (a few Directors / a number of Directors), and named-theatre attribution drift on politically sensitive named items (Middle East / Ukraine).

## Full whitepaper

# AI Hallucination Evaluation: Review of the Adequacy of the Fund's Precautionary Balances (2026)


## Executive Summary

This audit presents findings from RegLeg's evaluation of frontier AI models against the International Monetary Fund's March 2026 Review of the Adequacy of the Fund's Precautionary Balances and the closely linked October 2024 charges and surcharge reform. The March 2026 Executive Board review records a medium-term target of SDR 25 billion, a minimum floor of SDR 20 billion, a named geopolitical theatre of intensifying downside risk concentrated on the Middle East, an IMF Board lexicon characterisation of 'a few Directors' on the early-surcharge-review signal, and a half-year precautionary balances level of SDR 26,782 million at October 31, 2025 in the Q2FY26 Quarterly Financial Report. Claude Opus 4.7 produced confident, specific answers across six distinct questions in this audit that the regulator's own primary text directly contradicts. The failures cluster into three thematic groups: numerical commitments that pull cycle-anchored parameters back by one biennial cycle or inflate single-value baselines under generation pressure (Findings 1, 2, 3, and 6); a regulator-specific characterisation lexicon drift that elevates 'a few Directors' to 'a number of Directors' (Finding 5); and a named-entity drift that adds Ukraine to the Board's specifically named geopolitical theatre on intensifying downside risk (Finding 4). Each finding is bound to verbatim regulator-issued primary source text. For AI lab teams fielding frontier models into IMF-adjacent advisory deployments, the pattern signals systematic gaps in how models handle biennial-review parameters, single-value reform baselines, regulator-specific characterisation lexicons, named theatre attributions, and quarterly-report financial figures.

## Background: the March 2026 IMF PB Review

On March 20, 2026, the IMF Executive Board concluded the biennial Review of the Adequacy of the Fund's Precautionary Balances. The Board reaffirmed the medium-term target of SDR 25 billion. Directors generally agreed to retain the current floor for precautionary balances at SDR 20 billion, noting that it provides an important safeguard against shocks and helps ensure the Fund retains sufficient buffers. The Board cautioned that the Fund's income and precautionary balances projections are subject to heightened uncertainty including from financial market volatility and intensifying downside risks to global growth stemming in particular from geopolitical developments in the Middle East. Recognizing the uncertain environment, in the event that precautionary balances rise well above the target, a few Directors saw merit in considering an early review of charges and the surcharge policy in due course.

Adjacent to the March 2026 Review, the October 2024 charges and surcharge reform recorded in IMF Press Release 24/376 is the binding context for any near-term income projection. The Press Release records that the approved measures will lower IMF borrowing costs by about US$1.2 billion annually or reduce payments on the margin of the rate of charge as well as surcharges on average by 36 percent, and that the number of countries subject to surcharges in fiscal year 2026 is expected to fall from 20 to 13. The IMF Q2FY26 Quarterly Financial Report Schedule 2 records the precautionary balances level at October 31, 2025 at SDR 26,782 million, against SDR 25,905 million at April 30, 2025.

The RLB Specialist Panel designed the questions in this audit to mirror how lawyers, accountants, financial advisers, sovereign wealth finance and treasury teams, statutory board finance teams, investment banking risk teams, and management consulting finance teams use AI tools on this regulation: drafting board memoranda for EM finance ministry clients on Fund near-term lending capacity, drafting policy briefs on the October 2024 surcharge reform's two-year assessment, drafting historical-trajectory sections of campaign reports on the PB framework, drafting backgrounders for central-bank bilateral meetings with the IMF Managing Director, drafting legal-and-policy advisories on early-surcharge-review timing for EM finance ministries, and drafting desk notes for sovereign-credit research teams on the half-year PB trajectory. Each question is anchored to verbatim regulator-issued primary substrate.

## When this affects AI lab teams

AI lab teams fielding frontier models into IMF-adjacent, sovereign-debt advisory, central-bank-advisory, and sovereign-credit research deployments will see the failure modes documented here surface when the model is asked to reproduce a biennial-review parameter, a reform-adjacent count baseline, a regulator-specific characterisation lexicon term, a Board-named geopolitical theatre, or a quarterly-report financial figure. The pattern matters specifically for product surfaces that promise verbatim quotation from IMF documents on Fund financial strength, on Fund near-term lending capacity, on the charges and surcharge policy, or on Fund risk-narrative attributions to specific named theatres. The six findings document a confident, fluent failure mode: the model produces a structurally plausible answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source, with no hedging or source-verification recommendation.

## Finding 1: Precautionary balances floor committed at SDR 15 billion against substrate SDR 20 billion

**Citation ID:** `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q001-Opus47` * AI subject: Claude Opus 4.7

**Source anchor:** IMF substrate document recorded against the finding.

**Regulator's verbatim text:**

> Directors generally agreed to retain the current floor for precautionary balances at SDR 20 billion, noting that it provides an important safeguard against shocks and helps ensure the Fund retains sufficient buffers.

**What the model produced.** The Board reaffirmed the medium-term target of SDR 25 billion and reaffirmed the minimum floor of SDR 15 billion.

**Failure mode.** AI committed to a minimum floor of SDR 15 billion against the regulator's SDR 20 billion. The model produced its answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source.

**AI lab implication.** On this finding, Claude Opus 4.7 committed to a precautionary balances minimum floor of SDR 15 billion at the March 2026 review against the regulator's recorded SDR 20 billion. The failure shape implicates how a frontier model handles a parameter that was set at one biennial cycle (March 2024 raised the floor to SDR 20 billion from SDR 15 billion) and then reaffirmed at the next (March 2026). The model's training data likely contains both the March 2024 review record (floor raised to SDR 20 bill

## Finding 2: Surcharge-paying member count miscounted as 22 to 13 against regulator's 20 to 13

**Citation ID:** `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q005-Opus47` * AI subject: Claude Opus 4.7

**Source anchor:** IMF substrate document recorded against the finding.

**Regulator's verbatim text:**

> The number of countries subject to surcharges in fiscal year 2026 is expected to fall from 20 to 13.

**What the model produced.** Change in the number of surcharge-paying members between FY2024 and FY2026: the IMF projected a reduction from 22 surcharge-paying members in FY2024 to approximately 13 members in FY2026.

**Failure mode.** AI committed to a surcharge-paying member trajectory of 22 to 13 against the regulator's 20 to 13. The model produced its answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source.

**AI lab implication.** On this finding, Claude Opus 4.7 committed to a FY2024 surcharge-paying member baseline of 22 against the regulator's recorded 20. The failure shape implicates how a frontier model handles a specific count anchored on an adjacent regulator instrument (IMF Press Release 24/376) recorded in the model's training data. The 22-vs-20 divergence is consistent with single-value inflation under generation pressure where the model commits to a starting baseline that 'looks plausible' but does not match th

## Finding 3: Pre-2024 floor stated as SDR 10 billion stepping to SDR 15 billion against substrate SDR 15 billion to SDR 20 billion

**Citation ID:** `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q009-Opus47` * AI subject: Claude Opus 4.7

**Source anchor:** IMF substrate document recorded against the finding.

**Regulator's verbatim text:**

> Directors supported increasing the minimum floor for precautionary balances from SDR 15 billion to SDR 20 billion.

**What the model produced.** Value immediately BEFORE March 2024 review: SDR 10 billion. Value AFTER March 2024 review: SDR 15 billion.

**Failure mode.** AI committed to a March 2024 floor step from SDR 10 billion to SDR 15 billion against the regulator's SDR 15 billion to SDR 20 billion. The model produced its answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source.

**AI lab implication.** On this finding, Claude Opus 4.7 committed to a historical-trajectory section that recorded the IMF precautionary balances floor as SDR 10 billion before the March 2024 review and SDR 15 billion after, against the regulator's record of a step from SDR 15 billion to SDR 20 billion. The failure compounds the cycle-trajectory drift documented in Finding 1: both the pre-2024 floor value and the post-2024 floor value are pulled back by one biennial cycle. The implication for a frontier model is that 

## Finding 4: Added Ukraine to named geopolitical theatre against substrate naming only the Middle East

**Citation ID:** `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q011-Opus47` * AI subject: Claude Opus 4.7

**Source anchor:** IMF substrate document recorded against the finding.

**Regulator's verbatim text:**

> Directors cautioned that the Fund's income and precautionary balances projections are subject to heightened uncertainty including from financial market volatility and intensifying downside risks to global growth stemming in particular from geopolitical developments in the Middle East.

**What the model produced.** The Board specifically highlighted the situation in the Middle East and the conflict in Ukraine as sources of intensifying downside risk to the Fund's income and PB projections.

**Failure mode.** AI added Ukraine to the named geopolitical theatre against the regulator's text naming only the Middle East. The model produced its answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source.

**AI lab implication.** On this finding, Claude Opus 4.7 added Ukraine to the Board's named geopolitical theatre on intensifying downside risk; the regulator's text names only the Middle East. The failure shape implicates named-entity drift on politically sensitive attributions: where the model is asked to record what a regulator has specifically named, the model added a second named theatre that is plausibly present in the broader risk-narrative context but is not in the regulator's specific recorded language. For an 

## Finding 5: Inverted strength of the early-surcharge-review signal from a few Directors to a number of Directors

**Citation ID:** `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q012-Opus47` * AI subject: Claude Opus 4.7

**Source anchor:** IMF substrate document recorded against the finding.

**Regulator's verbatim text:**

> Recognizing the uncertain environment, in the event that precautionary balances rise well above the target, a few Directors saw merit in considering an early review of charges and the surcharge policy in due course.

**What the model produced.** The published characterisation in PR 26/114 indicates that a number of Directors saw merit in considering an early review of the charges and surcharge policy.

**Failure mode.** AI committed to a 'number of Directors' characterisation of the early-surcharge-review signal against the regulator's 'a few Directors'. The model produced its answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source.

**AI lab implication.** On this finding, Claude Opus 4.7 recorded the Board's early-surcharge-review signal as held by 'a number of Directors'; the regulator's text records the position as held by 'a few Directors'. The IMF Board lexicon distinguishes 'a few Directors' (a small minority position) from 'a number of Directors' (a more substantial minority) from 'several Directors' (a slightly stronger characterisation) from 'Directors generally agreed' and 'Most Directors' (clear majority and supermajority positions). Th

## Finding 6: Precautionary balances at October 31 2025 committed as approximately SDR 26.5 billion against substrate SDR 26.78 billion

**Citation ID:** `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q014-Opus47` * AI subject: Claude Opus 4.7

**Source anchor:** IMF substrate document recorded against the finding.

**Regulator's verbatim text:**

> Precautionary balances (est.) ** ... October 31, 2025: 26,782 ... April 30, 2025: 25,905 (in millions of SDRs).

**What the model produced.** The IMF's Q2FY26 Quarterly Financial Report (as of October 31, 2025) reports precautionary balances at approximately SDR 26.5 billion.

**Failure mode.** AI committed to a half-year precautionary balances level of approximately SDR 26.5 billion against the regulator's SDR 26.78 billion. The model produced its answer in a deliverable register where a downstream user would paste the answer into a working deliverable before verification against the source.

**AI lab implication.** On this finding, Claude Opus 4.7 committed to a half-year precautionary balances level of approximately SDR 26.5 billion at October 31, 2025 against the regulator's recorded SDR 26,782 million in the Q2FY26 Quarterly Financial Report Schedule 2. The 280 million SDR divergence is small in absolute terms but it is a verifiable figure that ratings analysts, capital-adequacy desks, and sovereign-credit research teams will check against the regulator's quarterly schedule. The failure shape implicates

## Aggregate impact

Across the six findings, three failure mechanisms recur. First, cycle-trajectory drift on biennial-review parameters: the model pulled the SDR-billion floor back by one cycle on both Finding 1 (March 2026 reaffirmation) and Finding 3 (March 2024 step). Second, single-value inflation or approximation under generation pressure: the model inflated the FY2024 surcharge-payer baseline by two (Finding 2) and rounded the half-year PB level by approximately 280 million SDR (Finding 6). Third, attribution drift on politically sensitive named items: the model added Ukraine to the Board's named geopolitical theatre (Finding 4) and elevated the IMF Board lexicon strength of the early-surcharge-review signal (Finding 5). For AI lab teams, the implication is that frontier models deployed into IMF-adjacent advisory contexts need retrieval-anchored verification on (i) most-recent-cycle parameters, (ii) reform-adjacent single-value baselines, (iii) regulator-specific characterisation lexicons, (iv) named theatre attributions to specific Board records, and (v) quarterly-report financial figures.

## What the team should do

### Training-data implications

The model's training data plausibly contains the March 2024 PB Review record (floor raised to SDR 20 billion from SDR 15 billion), the March 2026 Review record (floor retained at SDR 20 billion), the October 2024 charges and surcharge reform (FY2024 to FY2026 surcharge-payer trajectory of 20 to 13), and the Q2FY26 Quarterly Financial Report (October 31, 2025 PB at SDR 26,782 million). The failure shapes here are generation behaviours that pull adjacent training content into the answer rather than retrieval gaps. Training-data curation that emphasises the most-recent biennial-cycle text as authoritative over prior-cycle text for the same parameter, and that separates the IMF Board lexicon characterisations as fixed-strength terms, should reduce cycle-trajectory drift and lexicon drift respectively.

### Post-training and tool-use logic

Post-training instruction-following on regulator-issued documents should treat biennial-review parameters, reform-adjacent baselines, regulator-specific characterisation lexicons, named theatre attributions, and quarterly-report figures as retrieval-priority surfaces. Tool-use logic should default to a citation-bound output (Press Release URL, Quarterly Report schedule, Policy Paper page) for every numerical or named-entity claim on this class of regulation, with no generation-bound substitution allowed once the citation is established.

### RegLeg-suggested probes

RegLeg suggests three probes for frontier models deployed into IMF-adjacent advisory contexts. First, a cycle-anchor probe that asks the model to reproduce the same parameter (PB floor, target, FY surcharge-payer count) across three consecutive review cycles and checks for cycle alignment. Second, a Board-lexicon probe that asks the model to characterise the strength of a Board signal using the IMF Board lexicon explicitly and checks for fixed-strength reproduction. Third, a named-theatre probe that asks the model to record what a specific Board has named on a specific risk narrative and checks for absence of named-theatre additions.

## How RLB can help AI labs

The RLB Specialist Panel offers AI lab teams structured access to the failure-mode catalogue across IMF, BIS, FSB, IOSCO, and CFTC instruments. The deliverable is a regulator-specific probe set that can be folded into pre-deployment evaluation pipelines, a fixed-strength characterisation lexicon mapping for the main international standard-setting bodies, and a named-theatre attribution probe across politically sensitive Board records. The substrate-bound binding of every finding gives AI labs a falsifiable evaluation anchor against the regulator's own primary text rather than a synthetic benchmark.

### Right of Reply

International Monetary Fund and any other named entity in this audit are offered a permanent, unedited right of reply on every finding. A response is appended verbatim to the finding record on receipt; the original finding remains visible alongside. Responses can be submitted via the contact channel on the RegLeg site.

### Source and Methodology Standards

Every finding in this audit is bound to verbatim regulator-issued primary source text held as substrate by the RLB Specialist Panel. The substrate document, the section anchor, and the verbatim excerpt are recorded against each finding. Findings are published only where the regulator's own primary text directly contradicts the AI subject's response. The RLB Specialist Panel does not publish positive findings, blind spots, or claims unsupported by primary substrate.

*Primary source verified: every finding in this audit is bound to verbatim text recorded by the International Monetary Fund in the substrate document identified against the finding record. The RLB Specialist Panel holds the substrate on file.*

### Citation IDs referenced

- `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q001-Opus47`
- `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q005-Opus47`
- `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q009-Opus47`
- `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q011-Opus47`
- `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q012-Opus47`
- `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q014-Opus47`


## Related concepts

- Regulation: [IMF-PRECAUTIONARY-BALANCES-REVIEW-2026](/okf/regulations/IMF-PRECAUTIONARY-BALANCES-REVIEW-2026.md)
- Regulator: [IMF-INT-001](/okf/bodies/IMF-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)