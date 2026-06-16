---
type: "AILabsWhitepaper"
title: "Numeric Reconstruction Failures on OECD Digital Technologies and the Environment (2025)"
slug: "oecd-digital-technologies-environment-2025-numeric-reconstruction"
audience: "ai_labs"
regulation_slug: "OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025"
regulation_id: "328105"
body_id: "OECD-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "OECD"
methodology_version: "2.1"
substrate_version: 1
generated_at: "2026-06-08T09:51:11.316086+00:00"
published_at: "2026-06-08T09:51:11.316086+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/oecd/OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025/ai-labs/"
timestamp: "2026-06-16T00:00:00+00:00"
---

# Numeric Reconstruction Failures on OECD Digital Technologies and the Environment (2025)

- **Regulation.** [`OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025`](/okf/regulations/OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025.md) — Recommendation of the Council on Digital Technologies and the Environment (2025 Revision)
- **Regulator.** [`OECD-INT-001`](/okf/bodies/OECD-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** 2.1
- **Generated.** 2026-06-08T09:51:11.316086+00:00

## Executive summary

Numeric substitution on a specific statistical figure, an 11% share inflated to 14%, is the central failure observed in Claude Sonnet 4.6 with web search on the OECD's Recommendation of the Council on Digital Technologies and the Environment (2025 Revision). The model retrieved and cited the correct source combination but produced a figure that does not appear in the regulator's text, while appending a forward-extended series that reflects trend reconstruction rather than retrieval. The failure pattern is not a retrieval failure, the model located the right document lineage, but a numeric reconstruction where confident output diverges from the verbatim figure at the point of reporting. On regulatory content where specific percentages carry policy weight and are frequently paraphrased across secondary sources, this class of error presents a systematic exposure: the model's output is plausible, internally coherent, and wrong.

## Full whitepaper

# Numeric Reconstruction Failures on OECD Digital Technologies and the Environment (2025)


Numeric substitution on a specific statistical figure, an 11% share inflated to 14%, is the central failure observed in Claude Sonnet 4.6 with web search on the OECD's Recommendation of the Council on Digital Technologies and the Environment (2025 Revision). The model retrieved and cited the correct source combination (Ireland's Central Statistics Office 2023 data as reported in the OECD Digital Economy Outlook 2024) but produced a figure that does not appear in the regulator's text, while also appending a forward-extended series (18% in 2022, 21% in 2023) that reconstructs plausible trend logic rather than quoting the authoritative record. The failure pattern is not a retrieval failure, the model located the right document lineage, but a numeric reconstruction where the model's confident output diverges from the verbatim figure at the point of reporting. On regulatory content where specific percentages carry policy weight and are frequently paraphrased across secondary sources, this class of error presents a systematic exposure: the model's output is plausible, internally coherent, and wrong.

## When This Affects an AI Lab

The OECD's Digital Technologies and the Environment recommendation sits at the intersection of technology governance, climate disclosure, and infrastructure policy, exactly the territory where enterprise compliance teams, sustainability officers, and public-sector advisors are currently relying on frontier models to interpret and summarise official guidance. Users querying a model about data-centre energy obligations, national reporting benchmarks, or OECD member-state implementation commitments expect the model to surface the regulator's figures accurately. When it produces a plausible but wrong statistic, drawn from the right source lineage but with a quietly substituted value, that output travels: into briefing notes, regulatory filings, policy submissions, and procurement decisions. The downstream actor has no reason to distrust a model that cited the correct regulator and the correct source year.

For an AI lab, the exposure is asymmetric. Users who act on a confidently stated 14% figure instead of the regulator's 11% are not flagging a model failure, they are writing the wrong number into documents where it matters. The lab's liability surface for confidently-wrong numeric outputs on regulatory content is not theoretical; it accumulates quietly in every customer interaction where the model's output is the only source consulted. Gaps in red-team and eval coverage for this class of near-miss numeric error, right source, wrong figure, mean the failure is not being caught pre-deployment.

The OECD recommendation's structure amplifies this risk. It is a policy-level text that aggregates statistical evidence from third-party reports, national statistical offices, and prior OECD publications, a citation web that large models are likely to have encountered in multiple paraphrased forms across training. Where secondary sources have reported figures from earlier-edition data or selectively rounded or truncated the original, the model is navigating a landscape where several plausible numbers exist for the same underlying fact. That is precisely the condition under which confident numeric reconstruction, rather than verbatim retrieval, becomes the failure mode.

## Aggregate Impact

| Model | Configuration | Failure count | Dominant error pattern |
|---|---|---|---|
| Claude Sonnet 4.6 | with web search | 1 | Numeric substitution on a specific statistical figure drawn from a correctly-identified source |

Claude Sonnet 4.6 with web search produced a confirmed numeric hallucination on Ireland's data-centre share of metered electricity in 2021, citing 14% against the regulator's 11%, while attributing the figure to the correct source pairing. The failure extends beyond a single substituted number: the model appended a forward-projected series (18% in 2022, 21% in 2023) that does not appear in the regulator's text and reflects trend extrapolation rather than retrieval. This is a reconstruction pattern, the model identified the right document lineage, then generated a figure that is internally consistent with the trend direction but diverges from the verbatim authoritative value.

The failure surface here is concentrated at the intersection of correctly-attributed sources and incorrectly-reproduced statistics. The model's citation behaviour is functionally accurate, right regulator, right source, right year, but the numeric content at the point of reporting has drifted. This is distinct from a hallucinated citation or a wrong-source attribution; the model's retrieval orientation is intact, but its numeric reproduction is not. On regulatory content where secondary sources have circulated multiple paraphrased or approximate versions of the same underlying figure, the model appears to draw on reconstructed plausibility rather than the verbatim record.

## Findings


### Finding 6. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** What share of Ireland's 2021 metered electricity did data centres account for, per the figure cited in the OECD Digital Economy Outlook 2024 chapter (sourced from Ireland's CSO 2023)?
- **AI's response:** "Data centres consumed **14%** of Ireland's total metered electricity in 2021, a figure drawn from Ireland's Central Statistics Office (CSO, 2023) and cited in the OECD Digital Economy Outlook 2024."
- **Regulator's text:** "data centre energy consumption increased by 144% between 2015 and 2020, accounting for 11% of metered electricity consumed in the country in 2021 (Central Statistics Office, 2023)"
- **Why the AI went wrong:** The model correctly identified the source chain, CSO 2023 as cited in the OECD Digital Economy Outlook 2024, but substituted 14% for the regulator's 11%. It then extended the response with a forward-projected series (18% in 2022, 21% in 2023) that is not present in the regulator's text, suggesting the model reconstructed a plausible growth trajectory rather than quoting the authoritative figure. The error is not a misidentified source but a numeric value that has drifted at the point of reproduction.
- **Cited source(s):**
  - _Regulator portal: https://www.oecd.org_

## What Your Team Should Do

### Implications for your training data

The observed failure, correct source attribution, wrong numeric value, points to a training corpus where the OECD's statistical evidence appears in multiple paraphrased forms across secondary aggregators, law-firm briefings, think-tank summaries, and news coverage. Where those secondary sources have cited earlier-edition data, rounded figures, or selectively quoted from evolving statistical series, the model has encountered several plausible-but-divergent values for the same underlying fact. The 11% figure from Ireland's CSO 2023 as cited in the OECD Digital Economy Outlook 2024 is a specific, verbatim claim; the 14% the model produced is consistent with figures that may appear in adjacent commentary on the same statistical series. A training-side fix requires pairing the regulator's verbatim numeric statements with explicit negative examples from secondary sources that have paraphrased or approximated the same data, scored so the model learns to privilege the primary text over secondary reconstruction when source attribution is explicit.

The model's forward-projected series (18% in 2022, 21% in 2023) signals a second training-side gap: the corpus likely contains extrapolative commentary on Ireland's data-centre growth trajectory, and the model has learned to append trend continuations in contexts where a figure is cited with a year anchor. Structured ingestion of the regulator's primary statistical tables, where the values are fixed and the series boundaries are explicit, would constrain this behaviour. Extrapolation from a cited base figure should be a high-uncertainty signal, not a confident addendum.

### Implications for your post-training logic

When web search is active and the model has retrieved a document that explicitly names a numeric figure, a verification pass before output finalisation would catch this class of error. Concretely: where the model's planned response contains a specific percentage attributed to a named source and year, a secondary check against the retrieved content for that exact value would surface the discrepancy before it reaches the user. This does not require retraining, it is a tool-use or chain-of-thought step that compares the intended output figure against the retrieved text.

The model's generation of a forward-projected series (22, 23 data) where the retrieved source does not contain those years is a separate signal: the retrieval pipeline did not surface the forward-series data, but the model produced it anyway. Post-training calibration should treat "I am appending data beyond what I retrieved" as a high-uncertainty state warranting either explicit hedging or omission. The current calibration appears to treat trend continuation as a low-risk addition rather than an unverified claim.

### Specific eval / red-team probes RegLeg suggests

- **Verbatim-figure retention under secondary-source pressure:** Probe whether models reproduce the regulator's exact numeric value when the correct source is cited but secondary-source paraphrases of a different value are available in the retrieval pool.
- **Forward-series confabulation:** Probe whether models append years or data points beyond what is present in the retrieved document, particularly where the cited source contains a single anchor year.
- **Source-chain vs. value accuracy decoupling:** Probe whether models correctly attribute source lineage (primary → aggregator → regulator text) while simultaneously drifting on the numeric payload within that lineage.
- **Multi-vintage statistical conflict resolution:** Probe how models resolve conflicts between an older paraphrased figure and a newer authoritative revision when both appear in the retrieval results for the same query.
- **Trend-extrapolation calibration on policy-relevant statistics:** Probe whether models correctly signal uncertainty when asked to extend a statistical series beyond the regulator's published data, versus silently constructing a plausible continuation.

## How RLB Can Partner With Your Lab

We identify nuanced failure modes across model versions and configurations on regulatory content, failure classes that internal evals tuned to the lab's own model family are structurally unlikely to surface. Across our documented work to date, these include: subcategory-numeric conflation where the model reproduces a plausible aggregate instead of the regulator's disaggregated figure; multi-body institutional attribution drift where the named lead is the lower-frequency institution; schema over-specification on technical formats where the model imposes a structure the regulator's text does not require; false-negative evasion on retrievable official-speech content that falls within the retrieval window but outside the indexing cadence; and, as documented in this paper, source-chain-accurate but value-inaccurate numeric reproduction paired with forward-series confabulation on policy-relevant statistics.

We can accelerate the lab's model improvement on these failure surfaces in several concrete ways. Correction-pair generation: for each documented failure mode, we produce paired (wrong output, authoritative regulator text) examples formatted for direct ingestion into the training pipeline, derived from the regulator's verbatim text rather than secondary commentary. Comparative eval partnership: quarterly reports across model versions against a defined regulator portfolio, with regression monitoring on previously-documented failure modes so new releases don't reintroduce closed gaps. Pre-release evaluation cycles: for capability launches touching regulated domains, financial services, payments infrastructure, environmental compliance, cross-border regulatory content, we flag failure shapes before they reach customers. Red-team consultation: for specific regulators entering the lab's deployment footprint, we provide targeted failure-surface analysis scoped to the content structure, amendment cadence, and secondary-source paraphrase landscape that makes that regulator a likely failure surface.

To scope a technical partnership focused on refining the lab's models against these failure modes, reach out at reglegbrief.com.


## Related concepts

- Regulation: [OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025](/okf/regulations/OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025.md)
- Regulator: [OECD-INT-001](/okf/bodies/OECD-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)