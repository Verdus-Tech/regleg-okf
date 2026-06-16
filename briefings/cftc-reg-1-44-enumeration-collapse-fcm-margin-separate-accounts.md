---
type: "PublicBriefing"
title: "Enumeration Collapse in CFTC Regulation 1.44: How Models Reconstruct Regulatory Lists from Operational Priors"
slug: "cftc-reg-1-44-enumeration-collapse-fcm-margin-separate-accounts"
regulation_slug: "FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "v2.3"
news_featured_at: "2026-06-12T04:00:24.227002+00:00"
published_at: "2026-06-07T01:25:43.528347+00:00"
generated_at: "2026-06-11T01:32:19.300654+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cftc-reg-1-44-enumeration-collapse-fcm-margin-separate-accounts/"
timestamp: "2026-06-16T07:45:38.120254+00:00"
---

# Enumeration Collapse in CFTC Regulation 1.44: How Models Reconstruct Regulatory Lists from Operational Priors

- **Regulation.** [`FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44`](/okf/regulations/FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44.md) — Regulations to Address Margin Adequacy and to Account for the Treatment of Separate Accounts by Futures Commission Merchants (17 CFR § 1.44)
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)

## News lead

Two frontier AI models, Two frontier AI models, each running with web search, produced structurally correct-looking operational guidance on CFTC Regulation 1.44 that contradicts the regulation’s text. The Specialist Panel tested each model on the same operational question: map the currency deadline tiers for an FCM margin operations team. Both failed on the regulatory detail that determines how early or late an FCM must collect margin.

Claude Opus 4.7 collapsed the regulation’s three-tier structure into two tiers. Regulation 1.44(f) distinguishes: USD and Canadian dollars (same-day); Appendix A currencies, AUD, CNY, HKD, HUF, ILS, JPY, NZD, SGD, TRY, ZAR, (end of the second business day, T+2); and all other fiat currencies (end of the next business day, T+1). The model assigned Appendix A currencies a T+1 deadline and all other non-USD currencies same-day, compressing an intermediate tier out of existence. An FCM margin team following this guidance would call Appendix A margin one full business day earlier than required, and apply same-day urgency to currencies the regulation permits T+1 collection on.

Claude Sonnet 4.6 introduced a deadline that does not exist in the regulation: “12:00 p.m. ET on the FIRST U.S. business day.” Regulation 1.44(f)(3) sets only “end of the business day after the day on which the margin call is issued”, no intraday time. A system parameter or operations procedure built on this output would implement a self-imposed noon cutoff with no regulatory basis, and the documentation trail would cite a specific time the regulation does not contain.

Both outputs were formatted, internally consistent, and produced without any caveat that source verification was needed. That is the failure mode these findings document.

## Briefing

# Frontier AI models rewrote a CFTC margin rule, regulatory-research panel finds

## Two frontier AI models, with web search enabled, "compressed" a three-tier currency deadline structure into two and invented an intraday cutoff that does not exist in 17 CFR § 1.44(f), confidently, and without caveat. The RegLeg Brief Specialist Panel calls it "Enumeration Collapse" and says the pattern points to a calibration problem in how primary regulatory text is weighted against third-party summaries.

**SINGAPORE, June 12, 2026.** Two frontier artificial-intelligence models generated operational guidance on a recently finalised Commodity Futures Trading Commission rule that contradicts the rule's text in ways that would push U.S. Futures Commission Merchants out of compliance if acted on, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The findings, published with the immutable RLB Citation IDs `RLB-H-US-CFTC-FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44-Q001-Opus47` and `…-Q001-Sonnet46`, concern CFTC Regulation 1.44 (17 CFR § 1.44), the rule that governs how FCMs margin and segregate customer assets in separate accounts. Both Anthropic's Two frontier AI models were tested with web search active, mirroring how compliance and operations staff at FCMs and their technology vendors actually use the models today.

## The Verbatim Rule: Three Tiers, Defined by Appendix Membership

Section 1.44(f) sets out a three-tier currency deadline structure:

- **Tier 1, Same-day Fedwire close.** U.S. and Canadian dollars must be received by close of the Fedwire Funds Service on the same business day the margin call is issued.
- **Tier 2, Appendix A currencies (T+2).** Ten currencies listed in Appendix A, the Australian dollar (AUD), Chinese yuan (CNY), Hong Kong dollar (HKD), Hungarian forint (HUF), Israeli shekel (ILS), Japanese yen (JPY), New Zealand dollar (NZD), Singapore dollar (SGD), South African rand (ZAR) and Turkish lira (TRY), receive a deadline of "the end of the second business day after the day on which the margin call is issued."
- **Tier 3, All other fiat currencies (T+1).** "Payment of margin in fiat currencies other than U.S. Dollars, Canadian Dollars, or currencies listed in Appendix A to this part shall be considered in compliance with the requirements of this paragraph (f) if received by the applicable futures commission merchant no later than the end of the business day after the day on which the margin call is issued."

Membership in each tier is defined by the regulation, not by the currencies' intuitive groupings. CAD's assignment to the USD Fedwire tier and the precise ten-currency Appendix A list are explicit regulatory decisions with no derivable basis in the currencies' properties.

## Claude Opus 4.7: Compressed Three Tiers Into Two

Asked to map the currency deadline tiers for an FCM margin operations team, Claude Opus 4.7 (with web search on) wrote, verbatim:

> "For margin called in a fiat currency other than USD, the deadline may be extended by up to one additional business day… T+1 should be the default presumption… For all other non-USD currencies, default to same-day (T)."

**The structural error.** The model assigned Appendix A currencies a T+1 deadline (the regulation requires T+2) and pushed every remaining non-USD currency to same-day collection (the regulation grants them T+1). An FCM treasury team configuring system parameters from this output would:

- Call Appendix A margin a full business day **earlier** than the regulation permits, across AUD, CNY, HKD, JPY, SGD and the other six Appendix A currencies.
- Apply same-day urgency to currencies the regulation explicitly grants T+1 collection on, for example, EUR, GBP, CHF.

**Why it failed.** The RegLeg Brief Specialist Panel writes that "the two-tier reconstruction matches the format of third-party law-firm summary content that pre-dates or simplifies the rule's actual T+2 Appendix A tier… The retrieval-augmented generation layer either did not surface §1.44(f)(2) verbatim, or did surface it but failed to override the model's prior toward the simpler two-tier schema."

The failure mode is classified as `outdated` against substrate document `R2-REGULATION-17CFR_1_44_eCFR_asof_2026-06-04.pdf`.

## Claude Sonnet 4.6: Invented a Deadline That Does Not Exist

Given the same operational brief, Sonnet 4.6 (with web search on) generated:

> "TIER 1 EXTENSION, OTHER NON-USD/CAD FIAT CURRENCIES (T+1, 12:00 p.m. ET) • Deadline: 12:00 p.m. ET on the FIRST U.S. business day after the business day on which the margin call was issued."

**The fabrication.** Section 1.44(f)(3) sets no intraday cutoff. The regulator's verbatim text reads: "no later than the end of the business day after the day on which the margin call is issued." The "12:00 p.m. ET" figure does not appear in the rule or in Appendix A. A compliance procedure or system parameter configured against this output would impose a self-restricting noon deadline with no regulatory basis, and the documentation trail would cite a specific time that the rule does not contain.

**A fabricated citation, too.** On a parallel question, Sonnet 4.6 supported its two-tier currency reading with a URL on the website of international law firm Sidley Austin. The Specialist Panel verified the cited page does not exist; the citation is flagged as **Fabricated**.

**The diagnostic.** When the panel re-probed Sonnet 4.6 with a neutral prompt, the model self-retracted and produced the correct three-tier structure. The panel writes: "The self-retraction on re-probe confirms the correct three-tier structure was accessible, the generation pathway selected the wrong output despite having the right information available. This is a calibration failure in the RAG-to-generation handoff."

The failure mode is classified as `inference_drift` against the same substrate document.

## The Pattern: Enumeration Collapse

The Regulation 1.44 findings sit inside a broader failure class the RegLeg Brief Specialist Panel has been documenting across CFTC and adjacent regulatory work, which it calls **Enumeration Collapse**, frontier models reconstructing recently enacted regulatory lists from intuitive priors about how such rules typically look, rather than from the regulation's actual enumeration.

The white paper documents a second Regulation 1.44 question, on the rule's cessation triggers, the events that legally force an FCM to stop treating customer accounts as separate:

- **Regulation 1.44 specifies six customer-specific cessation triggers** plus three FCM-level events (distress notification, internal distress determination, insolvency).
- **Claude Sonnet 4.6** disaggregated margin failure into three checkbox items (initial, maintenance, variation margin) while dropping four of the six customer-level triggers, reducing regulatory coverage to two of the required six.
- **Claude Opus 4.7** dropped all three FCM-level events entirely, substituting a seven-item customer-centric margin-call checklist that contained no entry for any of the FCM-level triggers.

An automated risk-monitoring system built on either output would carry a surveillance gap a CFTC examination would surface.

## Why the Failure Is Invisible at Runtime

Both Claude outputs shared the same surface characteristics, checklist formatting, jurisdictional groupings, internal cross-references, no hedging language. The white paper states the operational risk plainly:

> "The failure is not recoverable by the user in real-time: the model's output is internally consistent and plausible enough that validation against the primary text would only happen if the user already knew what to look for."

Compliance and operations teams at FCMs and their technology vendors are the population most exposed. They use AI assistants to draft operational procedures, configure monitoring thresholds, and interpret regulatory text on tight timelines, the exact workflow in which the failure surfaces.

## What AI Labs Can Do: Suggested Probes (Open-Access)

The RegLeg Brief Specialist Panel documents five red-team probe designs in the white paper that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **Appendix-defined membership questions.** Test whether the model retrieves a regulation's appendix or constructs a plausible analogue from category logic.
2. **Recently-finalised rule enumeration count.** Compare the model's listed count to the regulation's actual enumeration. Test for disaggregation errors (one item split into sub-items) and dropout errors (items absent without explanation).
3. **Currency / jurisdiction tier assignment for rules finalised 2024–2025.** Test for compression to a simpler prior-generation structure.
4. **Self-retraction gap test.** Where the model initially produced a wrong structured output, re-probe with a neutral prompt. Retraction is diagnostic of a generation-path selection problem rather than a retrieval gap.
5. **Checklist completeness vs. plausibility.** Evaluate whether checklist item count matches the regulation's enumeration, or whether the model substituted a plausible checklist shape from its prior.

## Open-Access Risk Mitigation: A Public Good for AI Labs, Regulators, and the Compliance Community

RegLeg Brief operates as a completely ungated, open-access public resource. The white papers, per-finding cards, regulator verbatim excerpts, RLB Citation IDs, methodology notes and supporting data logs are all published without paywalls, registration walls, or data-licensing fees. By documenting original regulatory research without financial or distribution barriers, the platform ensures that:

- **AI engineering and alignment teams** can immediately ingest the verbatim model outputs and matched regulator-text excerpts to identify, reproduce, and address the structural failure modes the Specialist Panel documents.
- **Regulatory agencies and supervisors** can use the standardised RLB Citation IDs to benchmark AI-driven compliance risks surfacing in their own jurisdictions, with full traceability back to the original model output and the regulator's primary source.
- **The global compliance, treasury, and legal community** can freely adapt the Specialist Panel's screening methodologies to safeguard internal data pipelines and AI-assisted regulatory workflows.

Because RegLeg Brief conducts its own original research and adversarial analysis against frontier AI models, the detail in each published finding is precise enough to enable AI labs to take targeted hallucination-mitigation measures. Directions an AI lab might consider, drawing on the published findings, include:

- **Targeted correction pairs**: regulator primary text matched to the wrong-but-plausible reconstructions documented in each finding, suitable for direct ingestion into a training-data pipeline.
- **Quarterly embedded eval cycles**: continuous evaluation against a defined CFTC and multi-regulator portfolio, with regression monitoring on previously documented failure modes to track whether fine-tuning or RLHF adjustments are moving the needle on Enumeration Collapse.
- **Pre-release evaluation cycles**: sandboxed probes against catalogued failure shapes for capability releases touching financial services, payments infrastructure, or cross-border regulatory content, before the release reaches customers.
- **Post-release model enhancements**: regulator-specific failure-surface monitoring as new regulatory domains enter a model's live deployment footprint.

AI labs and model developers named in any published finding have an unconditional [right of reply](https://reglegbrief.com/right-of-reply/), the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** 17 CFR § 1.44, Risk-based Capital Requirements and Margin Adequacy for Separate Accounts · Substrate documents: `R2-REGULATION-17CFR_1_44_eCFR_asof_2026-06-04.pdf` · eCFR: ecfr.gov · CFTC: cftc.gov

**Citation IDs referenced:**

- `RLB-H-US-CFTC-FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44-Q001-Opus47`
- `RLB-H-US-CFTC-FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44-Q001-Sonnet46`


## Related concepts

- Whitepaper: [cftc-reg-1-44-enumeration-collapse-fcm-margin-separate-accounts](/okf/whitepapers/cftc-reg-1-44-enumeration-collapse-fcm-margin-separate-accounts.md)
- Regulation: [FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44](/okf/regulations/FCM-MARGIN-ADEQUACY-SEPARATE-ACCOUNTS-REG-1-44.md)
- Methodology: [v2.3](/okf/methodology.md)