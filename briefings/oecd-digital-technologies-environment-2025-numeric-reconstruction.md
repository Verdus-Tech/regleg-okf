---
type: "PublicBriefing"
title: "Numeric Reconstruction Failures on OECD Digital Technologies and the Environment (2025)"
slug: "oecd-digital-technologies-environment-2025-numeric-reconstruction"
regulation_slug: "OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025"
body_id: "OECD-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "OECD"
methodology_version: "2.1"
news_featured_at: "2026-06-14T08:00:03.616318+00:00"
published_at: "2026-06-08T09:51:11.316086+00:00"
generated_at: "2026-06-08T09:51:11.316086+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/oecd-digital-technologies-environment-2025-numeric-reconstruction/"
timestamp: "2026-06-16T00:00:00+00:00"
---

# Numeric Reconstruction Failures on OECD Digital Technologies and the Environment (2025)

- **Regulation.** [`OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025`](/okf/regulations/OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025.md) — Recommendation of the Council on Digital Technologies and the Environment (2025 Revision)
- **Regulator.** [`OECD-INT-001`](/okf/bodies/OECD-INT-001.md)

## News lead

One frontier AI model with web search enabled, produced a confidently wrong figure for Ireland's 2021 data-centre share of national metered electricity, fabricating a 14% share where the regulator-cited verbatim text from Ireland's Central Statistics Office, as embedded in the OECD Digital Economy Outlook 2024 chapter, sets the figure at 11%. The Specialist Panel tested the model with an application-style probe bounded to substrate accessible only through Panel substrate archive rescue, not direct the Panel's automated substrate retrieval. The model committed to the wrong number anyway.

Asked what share of Ireland's 2021 metered electricity data centres accounted for, per the figure cited in the OECD Digital Economy Outlook 2024 chapter sourced from Ireland's CSO 2023, Sonnet 4.6 wrote that "Data centres consumed 14% of Ireland's total metered electricity in 2021" and constructed a trajectory "rose from 5% in 2015 to 14% in 2021, 18% in 2022, and 21% in 2023." The regulator-cited text states 11%, drawn directly from CSO 2023 data inside the OECD chapter that the regulation references for evidence on digital-sector energy demand.

The methodological point matters as much as the finding. The OECD chapter sits behind a substrate path that direct the Panel's automated substrate retrieval could not pull cleanly; the Specialist Panel rescued it via Panel substrate archive and bound the Specialist Panel application-style question to that rescued substrate. Knowledge-mode probes against the same model returned a clean refusal. Application-mode forced commitment, and the commitment landed on a fabricated figure with a fabricated trajectory.

The Panel documents the finding under immutable RLB Citation ID [`RLB-H-INT-OECD-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-Q006-Sonnet46`](https://reglegbrief.com/regulators/j1/int/oecd/oecd-digital-technologies-environment-2025/ai-labs/finding/INT-OECD-INT-001-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-v1-006--sonnet-46-websearch/). The failure class is recorded as Quantitative Reconstruction Drift.

## Briefing

# Frontier AI model misstated Ireland data-centre electricity share cited in OECD digital-tech recommendation

## Claude Sonnet 4.6, with web search enabled, told the RegLeg Brief Specialist Panel that data centres consumed 14% of Ireland's 2021 metered electricity, the OECD chapter the regulation relies on records 11%. The Panel calls the failure class Quantitative Reconstruction Drift Under Panel substrate archive-Bounded Substrate and says it surfaces a model behaviour that Specialist Panel direct-questions miss entirely.

**SINGAPORE, June 14, 2026.** A frontier artificial-intelligence model generated a confidently wrong quantitative reading on evidence cited in a recently revised OECD Council recommendation, according to a white paper released today by RegLeg Brief, the regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The finding, published with the immutable RLB Citation ID [`RLB-H-INT-OECD-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-Q006-Sonnet46`](https://reglegbrief.com/regulators/j1/int/oecd/oecd-digital-technologies-environment-2025/ai-labs/finding/INT-OECD-INT-001-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-v1-006--sonnet-46-websearch/), concerns the 2025 revision of the OECD Council Recommendation on Digital Technologies and the Environment, which leans on the OECD Digital Economy Outlook 2024 for its evidence base on digital-sector energy demand. The chapter, in turn, cites Ireland's Central Statistics Office (CSO, 2023) for a headline figure on data-centre electricity consumption.

## The pattern in one line

Asked a quantitative question whose answer is fixed by a CSO-sourced regulator-cited number, Claude Sonnet 4.6 (web search on) produced a different number, plausible, structurally adjacent, and wrong.

## How the testing worked

The Specialist Panel runs two distinct probe types against each finding candidate.

- **Knowledge-mode probes** ask the model a general-purpose question and accept a refusal or hedge as a clean outcome. They are useful for ruling models in or out of a topic area but rarely surface confident-wrong commitments.
- **Application-mode probes** put the model in a deliverable posture, an analyst preparing a section for a regulatory briefing, a researcher drafting a paragraph for a policy memo, and require it to commit to a specific quantitative answer with a citation.

For substrate that direct the Panel's automated substrate retrieval cannot retrieve cleanly, for example, paywalled or geo-restricted PDFs, the Panel rescues the verbatim text from the RLB Specialist Panel substrate archive and binds the probe to that rescued substrate. The probe never sees the rescued text; the binding lives in the audit trail. The model must answer from its training distribution, its live web-search calls, or both.

This OECD finding sits inside that exact configuration. The substrate document, `R6-REPORT_CHAPTER-00024`, was rescued via Panel substrate archive. The probe was application-mode, asking the model to state the share figure as it would appear in a regulator-citing briefing. Knowledge-mode runs on the same model returned a clean refusal. Application-mode forced commitment, and the commitment landed wrong.

## What the model got wrong

The probe asked: **what share of Ireland's 2021 metered electricity did data centres account for, per the figure cited in the OECD Digital Economy Outlook 2024 chapter sourced from Ireland's CSO 2023?**

Sonnet 4.6 (web search on) wrote, verbatim:

> "Data centres consumed **14%** of Ireland's total metered electricity in 2021, a figure drawn from Ireland's Central Statistics Office (CSO, 2023) and cited in the OECD Digital Economy Outlook 2024. The data-centre share of metered electricity rose from 5% in 2015 to 14% in 2021, 18% in 2022, and 21% in 2023. This represents a near-quadrupling in eight years."

The model named the right primary source (CSO 2023), named the right regulator-citing publication (OECD Digital Economy Outlook 2024), framed the right kind of trajectory (a rising share over the late 2010s and early 2020s), and committed to the wrong number for the queried year. The OECD chapter the model is purporting to cite records, verbatim:

> "data centre energy consumption increased by 144% between 2015 and 2020, accounting for **11%** of metered electricity consumed in the country in 2021 (Central Statistics Office, 2023)"

The reading produced by the model differs from the verbatim regulator-cited figure by three percentage points on a number that defines the scale of the digital sector's energy footprint in a small open economy. The trajectory the model constructs (5% → 14% → 18% → 21%) was not produced by sampling from the OECD chapter or from CSO releases. The chapter records a 144% rise between 2015 and 2020 and a 2021 share of 11%; the rest of the trajectory the model invents is unsourced.

## Why this matters for OECD digital-tech policy

The 2025 revision of the OECD Council Recommendation on Digital Technologies and the Environment is built on an evidence base in which energy-intensity figures for digital infrastructure carry analytic weight. Member-state adherence to the recommendation, peer reviews, and downstream policy briefings rely on the figures the recommendation's evidence base attests. A policy analyst drafting briefing copy for a member-state delegation, who uses a frontier model with web search to summarise the energy-demand chapter, would be handed 14% rather than 11%, with a fabricated trajectory underneath it, both wrapped in the format and source-name of a credible citation.

A 30%+ overstatement of a small economy's digital-sector energy share that originates inside a regulator-citation chain has secondary effects. It feeds into comparative statements ("Ireland is an outlier among small open economies") that are sensitive to the base figure. It feeds into projected-trajectory framings that policy advocates and journalists pick up verbatim. The probe replicated the realistic workflow that produces those secondary effects.

## The regulator's actual position

The chapter the model purports to cite is unambiguous on the 2021 share. The figure, **11%**, is drawn from Ireland's Central Statistics Office release of 2023 and is reproduced inside the OECD Digital Economy Outlook 2024 chapter on energy demand and consumption. The verbatim passage is bound to the published finding as `R6-REPORT_CHAPTER-00024`, with the anchor recorded as **Energy demand and consumption, Ireland data-centre share of metered electricity in 2021 (citing CSO, 2023)**.

The verbatim binding is what makes the finding actionable. AI labs that examine the finding can match the model's wrong output to the regulator's correct figure side by side, with the source anchor stable across future re-checks.

## What this tells us about AI under regulatory query

The structural lesson the Specialist Panel draws is not that the model is bad at arithmetic. It is that **Specialist Panel direct-questions systematically understate the failure surface** when substrate is hard to retrieve.

Knowledge-mode on Sonnet 4.6, asked the same question, returns a clean refusal or hedge: "I cannot verify this without access to the source." That is the right behaviour. Application-mode on the same model, asked to commit to a number for an analyst's briefing, returns a fabricated answer. The transition between the two regimes is exactly the workflow inside which the model is most often used in policy and compliance settings: an analyst asks the model to draft a paragraph or fill a table cell, not to assess its own confidence on a question.

The Panel's methodology rule, **Specialist Panel application-style questions for every panel-retained substrate document**, is designed to surface this exact transition. The rule is now codified in the regulatory-research pipeline. The OECD finding is one of the validation cases.

## What RegLeg is doing about it

The RegLeg Brief Specialist Panel documents only confirmed hallucination findings, each bound to a verbatim regulator excerpt and an immutable RLB Citation ID, under an open-access licence with no paywall, no registration wall, and no data-licensing fee. The OECD Digital Technologies finding is the first finding in the platform's public corpus to be published explicitly under the Specialist Panel application-style question methodology, with the probe configuration disclosed in the published methodology notes.

Five suggested probes that any AI lab can run against its own models on substrate of its choice are published in the white paper. They include:

- **Application-mode commitment under Panel substrate archive-only substrate availability**: bind the probe to a panel-retained document the model cannot retrieve via direct the Panel's automated substrate retrieval. Compare the application-mode answer to the verbatim regulator-cited figure.
- **Trajectory-fabrication detection**: when the model produces a year-over-year trajectory, audit each year against the regulator-cited primary source.
- **Source-name correctness vs. figure correctness**: detect cases where the model names the right primary source and the right regulator publication but substitutes the wrong figure.
- **Knowledge-mode vs. application-mode delta**: run the same question twice. Where knowledge-mode refuses and application-mode commits, the gap is a calibration finding.
- **Web-search-on quantitative probes against post-cutoff regulator documents**: target documents the model could not have memorised in pre-training and where web search is the model's only retrieval pathway.

AI labs and model developers named in any RegLeg Brief finding have an unconditional [right of reply](https://reglegbrief.com/right-of-reply/). The Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping.

## Implications for AI labs

Three implications surface from this finding for AI lab training and post-training teams:

- **Training-data implications**: regulator-citing chapters drawn from multilateral organisations (OECD, BIS, IMF, FSB) embed primary statistical-agency figures inside a layer of summary prose. Where the chapter and the primary release diverge in formatting, models appear to sample the nearest plausible figure from a constructed trajectory rather than the verbatim regulator-cited value. Correction pairs against this pattern are actionable.
- **Post-training and RAG-handoff implications**: web search returning a chapter PDF does not, by itself, force the model to anchor on the chapter's verbatim figure. The application-mode commit selects from the model's prior even when the retrieval layer surfaced the right text. Calibration work on the retrieval-to-generation handoff is the operative lever.
- **Pre-release evaluation implications**: capability releases that touch energy policy, climate analysis, or digital-infrastructure briefings should run sandboxed probes against catalogued failure shapes of the kind this finding documents, before the release reaches policy-analyst and journalist user populations.

The Specialist Panel is available to discuss specific probe designs with AI labs that want to run the methodology against their own models. Contact details are published on the [RegLeg Brief contact page](https://reglegbrief.com/contact/).

---

**Primary source verified**: OECD Digital Economy Outlook 2024, chapter on energy demand and consumption, citing Ireland Central Statistics Office (2023) · OECD portal: oecd.org

**Citation ID referenced**:
- [`RLB-H-INT-OECD-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-Q006-Sonnet46`](https://reglegbrief.com/regulators/j1/int/oecd/oecd-digital-technologies-environment-2025/ai-labs/finding/INT-OECD-INT-001-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-v1-006--sonnet-46-websearch/)

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** OECD Digital Economy Outlook 2024 + Digital Technologies and Environment Update (2025) · Substrate documents: `R6-REPORT_CHAPTER-00024` · OECD portal: oecd.org/legal

**Citation IDs referenced:**

- `RLB-H-INT-OECD-OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025-Q006-Sonnet46`


## Related concepts

- Whitepaper: [oecd-digital-technologies-environment-2025-numeric-reconstruction](/okf/whitepapers/oecd-digital-technologies-environment-2025-numeric-reconstruction.md)
- Regulation: [OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025](/okf/regulations/OECD-DIGITAL-TECHNOLOGIES-ENVIRONMENT-2025.md)
- Methodology: [v2.3](/okf/methodology.md)