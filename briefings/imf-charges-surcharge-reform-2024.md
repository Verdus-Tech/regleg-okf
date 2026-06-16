---
type: "PublicBriefing"
title: "IMF Surcharge Reform 2024: Numeric Baseline Failures Across Frontier AI Model Configurations"
slug: "imf-charges-surcharge-reform-2024"
regulation_slug: "IMF-CHARGES-SURCHARGE-REFORM-2024"
body_id: "IMF-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "IMF"
methodology_version: "v2.3"
news_featured_at: "2026-06-13T08:00:00.533364+00:00"
published_at: "2026-06-07T08:36:30.759469+00:00"
generated_at: "2026-06-07T08:36:30.759469+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/imf-charges-surcharge-reform-2024/"
timestamp: "2026-06-16T07:45:43.444641+00:00"
---

# IMF Surcharge Reform 2024: Numeric Baseline Failures Across Frontier AI Model Configurations

- **Regulation.** [`IMF-CHARGES-SURCHARGE-REFORM-2024`](/okf/regulations/IMF-CHARGES-SURCHARGE-REFORM-2024.md) — Review of Charges and the Surcharge Policy, Reform Proposals (October 2024)
- **Regulator.** [`IMF-INT-001`](/okf/bodies/IMF-INT-001.md)

## News lead

**SINGAPORE, June 10, 2026.** Two frontier AI models running with web search enabled, both tested by the RLB Specialist Panel, produced confidently wrong reconstructions of the headline baseline figure in the International Monetary Fund's October 2024 surcharge reform, in findings released today by the RegLeg Brief Specialist Panel. Asked how many IMF member countries were paying surcharges immediately before the reform took effect on 1 November 2024, both models committed to a specific integer that diverges from the Fund's own published count, and arrived at the same wrong number through different failure paths.

Claude Opus 4.7, queried on the immediate impact of the reform and the projected count through fiscal year 2026, answered that "before reform: 19 IMF member countries were paying surcharges" and that "after 1 November 2024: 11 countries continue to pay surcharges," with a net of eight countries released. The IMF Executive Board's published record, in press release PR/24/385 dated 11 October 2024, states that the number of surcharge payers is expected to decline from 20 to 13 countries in FY2026. The model dropped one country from the pre-reform baseline and reconstructed the post-reform count from a net-release figure rather than from the regulator's published projection.

Claude Sonnet 4.6, on the same question, answered that "before the reform: 19 countries were paying surcharges" and that "after the reform took effect: 11 countries remain subject to surcharges." Sonnet 4.6 attributed the figures to Green Central Banking reporting on IMF Board data, then offered a separate "pre-reform baseline was 20 surcharge-paying countries" line in the same response, surfacing both the regulator figure and the wrong figure without resolving the conflict in favour of the regulator.

A sovereign debt economist, IMF country team, finance ministry desk officer, or research analyst drafting a surcharge impact note against either output would publish a pre-reform baseline one country short of the Fund's own count and a post-reform projection short of the FY2026 figure the Board approved.


## Briefing

**SINGAPORE, June 13, 2026.** The RegLeg Brief Specialist Panel released today findings showing that Two frontier AI models, each running with web search enabled, produced the same wrong pre-reform baseline when asked about the International Monetary Fund's October 2024 surcharge reform. Both models reported that 19 IMF member countries were paying surcharges before the reform took effect on 1 November 2024. The IMF's Executive Board, in press release PR/24/385 dated 11 October 2024, states the figure as 20. Both models also projected 11 surcharge-paying countries after the reform, where the Board's own projection through fiscal year 2026 is 13.

The regulation under review is the Review of Charges and the Surcharge Policy, the package of reform proposals approved by the IMF Executive Board on 11 October 2024 and effective from 1 November 2024. The reform raises the threshold above which surcharges apply, lowers the level-based surcharge rate, lengthens the time-based surcharge clock, and changes the underlying reference rate. The headline numerical outcome, repeated in the Board's communique, the Managing Director's accompanying statement, and the press release, is a decline in surcharge-paying members from 20 to 13 by FY2026. That projection is the figure sovereign debt economists, IMF country teams, and finance ministry debt offices cite when sizing the immediate fiscal relief to borrower countries and the corresponding revenue impact on the Fund's burden-sharing capacity.

## What the models said

Claude Opus 4.7 was asked what the immediate impact of the October 2024 IMF surcharge reform was on the number of countries paying surcharges as of 1 November 2024, and what the projected count of surcharge-paying countries was through fiscal year 2026. The model answered that before reform, 19 IMF member countries were paying surcharges; that after 1 November 2024, 11 countries continue to pay surcharges; and that the net effect was that eight countries were immediately released from surcharge obligations. The answer is internally consistent within itself, with the post-reform figure of 11 derived from the pre-reform figure of 19 minus the net-release figure of eight. It is not consistent with the IMF Board record. The Board's published figure for the pre-reform baseline is 20, and the Board's published projection for the FY2026 count is 13. The model produced a specific integer for both anchors, and both anchors are wrong by the same margin in the same direction.

Claude Sonnet 4.6 was asked how many countries were paying IMF surcharges immediately after the 1 November 2024 reform took effect, and what the projected count was for IMF fiscal year 2026. The model answered that before the reform, 19 countries were paying surcharges; that after the reform took effect, 11 countries remain subject to surcharges; and that immediate relief reached eight countries that dropped below the new surcharge threshold. Sonnet 4.6 attributed the figures to Green Central Banking reporting on IMF Board data. The model then produced a follow-on line in the same response, prefaced by a confirmation note citing a Green Central Banking full fetch, which described the surcharge-paying country count under the new regime as dropping from 20 to 11 by FY2025, and which explicitly stated that the pre-reform baseline was 20 surcharge-paying countries. The same response therefore contains both the regulator figure of 20 and the wrong figure of 19, without resolving the conflict in favour of the regulator and without flagging the contradiction to the reader.

The convergence is the finding. Opus 4.7 reached 19 by what reads as a reconstruction from training-era reporting that had already settled on 19 as the working number. Sonnet 4.6 reached 19 by deferring to a third-party source that had reproduced the same wrong number. Two different retrieval and reasoning paths arrive at the same specific integer, and that integer is one short of what the IMF Board published. When two models converge on the same specific wrong number through different mechanisms, the systematic signal is that the correct figure is under-indexed in the content both training pipelines and live retrieval pull from, relative to the widely-circulated wrong figure.

## Why the baseline matters

The pre-reform baseline of 20 surcharge-paying countries and the post-reform projection of 13 are not background numbers. They are the headline metrics cited in the IMF's own communications to anchor the reform's distributional impact. A sovereign debt economist sizing the fiscal relief to borrower countries against the wrong baseline of 19 understates the cohort by one country; against the wrong projection of 11, overstates the cohort reduction by two countries. A finance ministry desk officer drafting a brief for a minister on the reform's bilateral relevance reaches the wrong shortlist if the baseline cohort is off by one. A research analyst building a model of IMF burden-sharing revenue under the reformed surcharge schedule prices the revenue impact off a cohort that is wrong at both anchors.

The reform is also the operative reference for the next round of IMF income policy discussion. The Board's review of net income, precautionary balances, and the burden-sharing framework runs against the surcharge cohort the reform produces. A wrong cohort count carried into that discussion compounds.

## What we tested

The Specialist Panel test on this regulation focused on the numerical baseline questions because those are the questions where the regulator's published record is most directly checkable and where divergence is least defensible. Both models were given the same effective date of 1 November 2024, the same regulator (IMF Executive Board), and the same source document set (the press release, the Managing Director's statement, and the Board communique). Both were run with web search enabled. Both were asked the baseline and projection question in plain numerical terms. Both committed to a specific integer for the pre-reform baseline. Both committed to a specific integer for the post-reform count. The integers do not match the regulator's published figures.

The Panel did not test paraphrase fidelity, scope characterisation, or qualitative description of the reform mechanism. Those tests were out of scope for this finding set. The finding is narrow and specific: on the numerical anchors that frame the reform's distributional impact, two frontier models with web search enabled produce the same wrong figures.

## Failure classification

The Opus 4.7 finding is classified as inference drift. The model reconstructed the baseline from training-era priors that had settled on 19 as the working number, and then derived the post-reform count internally from that wrong baseline rather than from the regulator's published projection. The internal arithmetic is consistent. The anchor is wrong.

The Sonnet 4.6 finding is classified as outdated retrieval. The model deferred to a third-party source that had reproduced the wrong baseline, and surfaced the regulator's correct figure of 20 alongside the wrong figure of 19 in the same response without resolving the conflict. The failure is not that the model could not find the regulator figure; the failure is that the model presented both figures and let the wrong one stand as the primary answer.

The shared failure mode, across both classifications, is that web search did not correct the baseline. Both models had retrieval enabled. Neither model anchored its answer on the IMF press release. Both produced a specific integer that diverges from the regulator's published count.

## Who is exposed

A sovereign debt economist documenting a note on the IMF surcharge reform's distributional impact, using either model as a drafting aid, would carry the wrong baseline cohort into the published note. An IMF country team drafting an article IV consultation working paper that touches on surcharge incidence would carry the wrong baseline into the working paper. A finance ministry desk officer briefing a minister on the bilateral fiscal relief from the reform would brief on a cohort that does not match the IMF Board record. A research analyst at a sovereign rating agency, a multilateral development bank, or a sell-side macro desk building a surcharge cohort model would price the cohort off the wrong baseline.

The exposure is at the headline number, not at a footnote. The 20 to 13 figure is the figure cited in the reform communications. Replacing it with 19 to 11 is not a paraphrase; it is a substitution of a specific wrong integer for a specific right one, at the anchor of the reform.

## Right of reply

The IMF Communications Department and the office of the Strategy, Policy and Review Department, which led the Board paper underlying the reform, were notified of the Specialist Panel findings on 4 June 2026 with a deadline for comment of 9 June 2026; no response was received by the time of release. Anthropic, which produces Claude Opus 4.7 and Claude Sonnet 4.6, was notified of the model-level findings on 4 June 2026 with the same deadline; no response was received by the time of release. The right of reply remains open and any response received will be appended to the public record.

## Methodology note

The Specialist Panel runs each model under the same prompt configuration, captures the response verbatim, and compares the response against the regulator's published text. Findings are published only where the model commits to a specific factual claim that the regulator's published text contradicts. Paraphrase, qualitative characterisation, and well-calibrated refusals are not published. The substrate for this finding set is the IMF press release PR/24/385 dated 11 October 2024, supplemented by the Board communique and the Managing Director's accompanying statement. The substrate is held in the Panel's audit record and is identifiable by the citation IDs RLB-H-INT-IMF-IMF-CHARGES-SURCHARGE-REFORM-2024-Q004-Opus47 and RLB-H-INT-IMF-IMF-CHARGES-SURCHARGE-REFORM-2024-Q004-Sonnet46.

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** IMF Review of Charges and the Surcharge Policy: Reform Proposals (October 2024) · Substrate documents: `R6-SPEECH-Q4_press_release_pr24385.pdf` · IMF portal: imf.org

**Citation IDs referenced:**

- `RLB-H-INT-IMF-IMF-CHARGES-SURCHARGE-REFORM-2024-Q004-Opus47`
- `RLB-H-INT-IMF-IMF-CHARGES-SURCHARGE-REFORM-2024-Q004-Sonnet46`


## Related concepts

- Whitepaper: [imf-charges-surcharge-reform-2024](/okf/whitepapers/imf-charges-surcharge-reform-2024.md)
- Regulation: [IMF-CHARGES-SURCHARGE-REFORM-2024](/okf/regulations/IMF-CHARGES-SURCHARGE-REFORM-2024.md)
- Methodology: [v2.3](/okf/methodology.md)