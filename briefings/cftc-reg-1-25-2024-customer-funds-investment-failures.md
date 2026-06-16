---
type: "PublicBriefing"
title: "Regulation 1.25 Amendment Failures: Schema Substitution and Procedural Confabulation on CFTC Customer Fund Investment Rules"
slug: "cftc-reg-1-25-2024-customer-funds-investment-failures"
regulation_slug: "FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "v2.3"
news_featured_at: "2026-06-14T00:00:04.861717+00:00"
published_at: "2026-06-07T08:39:33.721893+00:00"
generated_at: "2026-06-11T01:39:05.145683+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cftc-reg-1-25-2024-customer-funds-investment-failures/"
timestamp: "2026-06-16T07:45:43.309650+00:00"
---

# Regulation 1.25 Amendment Failures: Schema Substitution and Procedural Confabulation on CFTC Customer Fund Investment Rules

- **Regulation.** [`FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024`](/okf/regulations/FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024.md) — Amendments to Regulation 1.25, Permissible Investments of Customer Funds by Futures Commission Merchants and Derivatives Clearing Organizations
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)

## News lead

Two frontier AI models running with web search enabled, both tested by the RLB Specialist Panel, produced confidently wrong reconstructions of the CFTC's 2024 amendments to Regulation 1.25, the rule governing permissible investments of customer segregated funds by futures commission merchants and derivatives clearing organizations. The RegLeg Brief Specialist Panel tested both models on the size-triggered 50 per cent concentration limit for government money market funds and qualified Treasury ETFs, the dollar-weighted average maturity (DWAM) limit and its carve-out set, and the separate March 31, 2025 compliance date for the Segregation Investment Detail Report and customer risk disclosure statement, and documents findings in which the models dropped the asset-size and management-company-size triggers that activate the 50 per cent ceiling, inverted the DWAM exclusion set by swapping the carved-out asset classes for unrelated ones, and drifted on the SIDR compliance anchor into a generic "roughly six months to a year after the effective date" formulation that does not match the regulator's published deadline.

Claude Opus 4.7, asked which concentration limits apply to government money market funds and Treasury ETFs under the 2024 amendments and whether any tiered or size-based thresholds exist, wrote that "the final rule did not adopt tiered or FCM-size-based thresholds, the percentage limits apply uniformly regardless of FCM size." The regulator's text in 17 CFR 1.25(b)(3)(ii) is unambiguous that a size-based trigger does exist, keyed to the fund's own assets and to its management company's assets: investments in government money market funds or qualified ETFs whose fund assets are at least $1 billion and whose management company manages at least $25 billion may not exceed 50 per cent of total segregated assets. The model surfaced the FCM-side question correctly while dropping the fund-side and management-company-side triggers that actually govern the 50 per cent ceiling. On the DWAM question, Opus 4.7 wrote that "U.S. Treasuries held under repurchase agreements" are excluded from the portfolio-level 24-month dollar-weighted average maturity calculation. The regulator's carve-out set in 17 CFR 1.25(b)(3)(iv) is government money market funds, Treasury ETFs, and foreign sovereign debt; U.S. Treasury repos are not part of the carve-out. The model inverted the exclusion set. Asked separately for the SIDR and customer risk disclosure compliance date, Opus 4.7 anchored the deadline at "a separate, later date (commonly described as roughly six months to a year after the effective date)" where the regulator's published anchor is March 31, 2025.

Claude Sonnet 4.6 reproduced the size-trigger elision and added a fabricated tier structure. On the concentration-limit question, Sonnet 4.6 wrote that "there is no size-based tier that changes the percentages based on the FCM's total assets" and then described a Tier 1 "no more than 10 per cent of total assets held in customer segregation may be invested in any single government money market fund" rule. The regulator's text does not key the 50 per cent ceiling to FCM size; it keys it to fund asset size and management company asset size, the exact triggers the model dropped while presenting an FCM-size-negation answer that misdirects the reader away from the actual governing thresholds. On the DWAM question, Sonnet 4.6 wrote that the 2024 amendments "do not impose a new dollar-weighted average maturity (DWAM) standard or a maximum remaining-maturity cap specifically on direct U.S. Treasury obligations" and concluded that "no DWAM standard or individual-maturity cap found in the 2024 amendments applies to that category." The regulator's text imposes a 24-month portfolio-level DWAM that applies to direct U.S. Treasury obligations by default; the carve-out covers government money market funds, Treasury ETFs, and foreign sovereign debt, not direct Treasuries. The model returned a no-standard answer to a question the regulator answers with a standard.

A futures commission merchant chief risk officer, derivatives clearing organization treasury team, customer-funds compliance officer, or regtech tool drafting an investment policy statement, scoping segregated-fund concentration testing, or scheduling SIDR and customer risk disclosure updates against either output would set the wrong concentration ceiling triggers, exclude the wrong asset classes from DWAM testing, and miss the regulator's March 31, 2025 compliance anchor. That is the failure mode these findings document.


## Briefing

# Frontier AI models dropped the size-based concentration triggers, inverted the DWAM exclusion set, and drifted on the SIDR compliance anchor in the CFTC's 2024 Regulation 1.25 amendments, regulatory-research panel finds

## Two frontier AI models, with web search enabled, told a Chief Risk Officer drafting an FCM investment policy that no size-based tier governs the 50 per cent ceiling on government money market funds and Treasury ETFs when 17 CFR 1.25(b)(3)(ii) keys the ceiling to a one-billion-dollar fund-asset trigger and a twenty-five-billion-dollar management-company trigger, classified U.S. Treasury repos as excluded from the 24-month dollar-weighted average maturity calculation when the carve-out set is government money market funds, Treasury ETFs, and foreign sovereign debt, returned a no-standard answer for direct U.S. Treasury obligations under the DWAM rule when the regulator's 24-month portfolio limit governs them by default, and anchored the Segregation Investment Detail Report compliance date at "roughly six months to a year after the effective date" when the regulator's published deadline is March 31, 2025. The RegLeg Brief Specialist Panel calls the pattern "Threshold-Trigger Elision and Carve-Out Inversion" and says it points to a systematic gap in how frontier models handle conditional concentration rules whose ceilings activate only when named asset-size and management-company-size triggers are crossed, and exclusion lists where the regulator's carved-out classes look superficially similar to other adjacent classes that are not carved out.

**SINGAPORE, June 14, 2026.** Two frontier artificial-intelligence models generated reconstructions of the CFTC's 2024 amendments to Regulation 1.25 that drop the asset-size and management-company-size triggers governing the 50 per cent concentration ceiling, invert the carve-out set under the 24-month dollar-weighted average maturity rule, and drift on the Segregation Investment Detail Report compliance anchor, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The findings concern the **CFTC's 2024 amendments to 17 CFR 1.25**, the rule governing permissible investments of customer segregated funds by registered futures commission merchants and derivatives clearing organizations, including the revised concentration limits, the portfolio-level dollar-weighted average maturity (DWAM) standard, and the separate compliance date for the Segregation Investment Detail Report (SIDR) and customer risk disclosure statement. Both Anthropic's Claude Opus 4.7 and Claude Sonnet 4.6 were tested with web search active, mirroring how FCM chief risk officers, DCO treasury teams, customer-funds compliance officers, and regtech tools actually use the models when drafting investment policy statements, scoping segregated-fund concentration testing, or scheduling the post-amendment SIDR update cycle.

## The Verbatim Rule: Size Triggers Govern the Ceiling, and the Carve-Out Set Is Narrow

The regulator's record on the 50 per cent concentration ceiling under 17 CFR 1.25(b)(3)(ii) is unambiguous. The ceiling is not a uniform percentage applied regardless of counterparty size; it is a conditional limit that activates only when two named size triggers are simultaneously crossed. The verbatim structure reads:

> "Investments in government money market funds or qualified ETFs whose assets are at least one billion dollars and whose management company manages at least twenty-five billion dollars: may not exceed 50% of total segregated assets."

The structural register matters. The regulator characterises the 50 per cent ceiling as **conditional**: it engages only against funds and ETFs that clear both the one-billion-dollar fund-asset threshold and the twenty-five-billion-dollar management-company threshold. An FCM that reads the rule as a uniform percentage limit will misclassify smaller funds and incumbent name-brand managers under the wrong concentration regime.

The regulator's record on the DWAM rule is similarly explicit:

- **Portfolio standard**: the dollar-weighted average of the time-to-maturity of the portfolio may not exceed 24 months.
- **Carve-out set**: government money market funds, Treasury ETFs, and foreign sovereign debt are excluded from the DWAM calculation.
- **What is not carved out**: direct U.S. Treasury obligations and U.S. Treasury repurchase agreements are not on the exclusion list and are subject to the 24-month portfolio standard.
- **SIDR anchor**: SIDR Report and customer Risk Disclosure Statement updates carry a compliance date of March 31, 2025.

## Claude Opus 4.7: Dropped the Size Triggers, Inverted the DWAM Exclusion, Drifted on the SIDR Anchor

Asked which concentration limits apply to government money market funds and Treasury ETFs under the 2024 amendments, including any tiered or size-based thresholds based on fund and management company asset sizes, Claude Opus 4.7 (with web search on) wrote, verbatim:

> "the final rule did not adopt tiered or FCM-size-based thresholds, the percentage limits apply uniformly regardless of FCM size"

**The dropped triggers.** The regulator's text in 17 CFR 1.25(b)(3)(ii) keys the 50 per cent ceiling to two thresholds: the fund's own assets must be at least one billion dollars, and the management company's assets must be at least twenty-five billion dollars. Opus 4.7 surfaced the FCM-side question correctly (the rule is not keyed to FCM size) while dropping the fund-side and management-company-side triggers that actually govern when the 50 per cent ceiling engages. A Chief Risk Officer reading the output as a uniform percentage rule would size the firm's segregated-fund book against the wrong governing structure.

**The inverted DWAM carve-out.** Asked what dollar-weighted average maturity limit applies to an FCM's overall portfolio of customer segregated fund investments and which asset classes are excluded from the portfolio-level calculation, Opus 4.7 wrote:

> "with U.S. Treasuries held under repurchase agreements excluded from the calculation"

The regulator's carve-out set under 17 CFR 1.25(b)(3)(iv) is government money market funds, Treasury ETFs, and foreign sovereign debt. U.S. Treasury repos are not on the exclusion list. The model swapped one adjacent asset class (Treasury repos) into the carve-out while dropping the actual carved-out classes; a treasury team running DWAM concentration testing on the model's output would exclude the wrong book and over-include the right ones.

**The SIDR drift.** Asked for the separate compliance deadline for updating Segregation Investment Detail Reports and customer risk disclosure statements, Opus 4.7 anchored the deadline at "a separate, later date (commonly described as roughly six months to a year after the effective date)". The regulator's published anchor is March 31, 2025. The model retrieved the structural distinction (SIDR has its own date separate from the general effective date) and then drifted on the specific anchor, returning a generic range where the regulator documents a date certain.

**Why it failed.** The RegLeg Brief Specialist Panel writes that the failure shape is characteristic of conditional-ceiling retrieval: the model surfaces one axis of the conditional structure (the FCM-size axis) correctly and then flattens the other axes (fund size, management-company size) out of the answer. The DWAM inversion has the same shape on the exclusion side, the model has enough corpus coverage to know that some asset class is carved out from the 24-month standard but not enough to retrieve the specific carved-out set, producing a plausible substitution from the adjacent asset universe.

The failure modes are classified as inference_drift against substrate documents covering 17 CFR 1.25(b)(3)(ii), 17 CFR 1.25(b)(3)(iv), and the operative section of the Commodity Exchange Act at 7 USC 6d.

## Claude Sonnet 4.6: Reproduced the Trigger Elision With a Fabricated Tier Structure, Returned a No-Standard Answer on DWAM

Given the parallel concentration-limit brief, Sonnet 4.6 (with web search on) wrote:

> "there is no size-based tier that changes the percentages based on the FCM's total assets, the limits apply uniformly: Tier 1, Per Instrument: No more than 10% of total assets held in customer segregation may be invested in any single government money market fund"

**The misdirected negation.** Sonnet 4.6 produced a negation of the FCM-side trigger ("no size-based tier... based on the FCM's total assets") that is technically correct on the FCM axis but is operationally misleading: it presents the question as resolved while dropping the two triggers the regulator actually applies (fund asset size and management-company asset size). A risk officer reading the answer would walk away believing the size question has been adjudicated, when the only two size triggers that matter have been omitted.

**The no-standard DWAM answer.** Asked whether a portfolio maturity constraint applies to direct U.S. Treasury securities held in an FCM's customer segregated account under Regulation 1.25, Sonnet 4.6 wrote:

> "The 2024 amendments do not impose a new dollar-weighted average maturity (DWAM) standard or a maximum remaining-maturity cap specifically on direct U.S. Treasury obligations... No DWAM standard or individual-maturity cap found in the 2024 amendments applies to that category."

The regulator's 24-month portfolio DWAM standard applies to direct U.S. Treasury obligations by default. The carve-out set covers government money market funds, Treasury ETFs, and foreign sovereign debt, not direct Treasuries. Sonnet 4.6 returned a no-standard answer to a question the regulator answers with a standard, the most operationally consequential failure mode in the audit because it tells the user that no compliance work is required where the regulator requires it.

The failure modes are classified as inference_drift against the same substrate.

## The Pattern: Threshold-Trigger Elision and Carve-Out Inversion

The Regulation 1.25 findings sit inside a broader failure class the RegLeg Brief Specialist Panel has been documenting across recent regulatory instruments whose operative ceilings turn on multi-axis conditional triggers, which it calls **Threshold-Trigger Elision and Carve-Out Inversion**, frontier models systematically dropping one or more axes of multi-condition trigger structures, inverting narrow carve-out sets by substituting superficially-similar adjacent asset classes, and drifting from date-certain compliance anchors into generic "roughly N months after" formulations that read as procedural caveats but materially misstate the deadline.

The white paper documents the pattern across the audited question set:

- **Multi-axis trigger elision**: Both models surfaced one axis of the size-trigger structure (the FCM-size axis the regulator does not key on) correctly while dropping the two axes the regulator does key on (fund asset size at one billion dollars, management-company asset size at twenty-five billion dollars).
- **Carve-out inversion**: Opus 4.7 inserted U.S. Treasury repurchase agreements into the DWAM exclusion set in place of the regulator's actual carve-out set of government money market funds, Treasury ETFs, and foreign sovereign debt.
- **No-standard substitution**: Sonnet 4.6 returned a no-DWAM-standard answer for direct U.S. Treasury obligations where the 24-month portfolio standard governs by default.
- **Date-certain drift**: Opus 4.7 anchored the SIDR and customer risk disclosure compliance deadline at "roughly six months to a year after the effective date" where the regulator documents a date certain of March 31, 2025.
- **Web search did not correct the errors**: Both models ran with web search active and neither configuration surfaced the fund-asset and management-company-asset triggers, the actual DWAM carve-out set, or the March 31, 2025 SIDR anchor.

A futures commission merchant Chief Risk Officer, derivatives clearing organization treasury team, customer-funds compliance officer, or regtech tool automating investment policy drafting, segregated-fund concentration testing, or post-amendment SIDR scheduling on either model would carry the dropped size triggers, the inverted DWAM carve-out, the no-standard direct-Treasury answer, and the drifted SIDR anchor into the artefacts the firm produces.

## Why the Failure Is Invisible at Runtime

Both Claude outputs shared the same surface characteristics, structured enumerations of concentration limits and tier labels, regulator-attributed phrasing on exclusion sets, and in both models' cases, confident negations on the size-trigger axis that read as adjudicative resolutions of the question. The white paper states the operational risk plainly:

> "The failure is not recoverable by the user in real-time: the model's output reads as a faithful summary of the 2024 amendments, and validation would only happen if the reader already knew that the 50 per cent ceiling is keyed to the fund's own assets and to its management company's assets rather than to FCM size, that the DWAM carve-out set is government money market funds, Treasury ETFs, and foreign sovereign debt rather than U.S. Treasury repos, that the 24-month portfolio standard applies to direct U.S. Treasury obligations by default, and that the SIDR compliance anchor is the specific date of March 31, 2025."

FCM chief risk officers, DCO treasury teams, customer-funds compliance officers, and regtech tools advising on the 2024 amendments are the population most exposed. They use AI assistants to summarise the amended rule, draft investment policy statements, and structure concentration-testing playbooks against the post-amendment compliance calendar, the exact workflow in which the failure surfaces.

## What AI Labs Can Do: Suggested Probes (Open-Access)

The RegLeg Brief Specialist Panel documents five red-team probe designs in the white paper that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **Multi-axis trigger preservation probes.** Where a regulatory ceiling is keyed to two or more named size triggers (fund asset size, management-company asset size, counterparty asset size), test whether the model preserves all axes of the trigger structure or surfaces one axis correctly while dropping the others. Negation answers on the dropped axes are the highest-risk class for the elision failure mode.
2. **Carve-out exact-set probes.** Where a numeric standard carries a narrow exclusion list of named asset classes, test whether the model retrieves the specific carved-out set or substitutes superficially-similar adjacent classes (Treasury repos for Treasury ETFs, foreign sovereign debt for foreign agency debt) from the surrounding asset universe.
3. **Default-application probes.** Where a portfolio-level standard applies to an asset class by default and carries a narrow carve-out list that does not include that class, test whether the model applies the standard or returns a no-standard answer suggesting no compliance work is required.
4. **Date-certain anchor probes.** For instruments that publish a specific date certain compliance anchor (March 31, 2025) separate from the general effective date, test whether the model returns the published date or drifts into a generic "roughly N months after" formulation that reads as procedural caveat but materially misstates the deadline.
5. **Conditional-ceiling decomposition probes.** Where a percentage ceiling activates only when multiple conditions are simultaneously satisfied, test whether the model decomposes the conditional structure (when does the ceiling engage, what triggers each axis) or flattens it into an unconditional percentage limit.

## Open-Access Risk Mitigation: A Public Good for AI Labs, Regulators, and the Compliance Community

RegLeg Brief operates as a completely ungated, open-access public resource. The white papers, per-finding cards, regulator verbatim excerpts, RLB Citation IDs, methodology notes and supporting data logs are all published without paywalls, registration walls, or data-licensing fees. By documenting original regulatory research without financial or distribution barriers, the platform ensures that:

- **AI engineering and alignment teams** can immediately ingest the verbatim model outputs and matched regulator-text excerpts to identify, reproduce, and address the structural failure modes the Specialist Panel documents.
- **Regulatory agencies and supervisors** can use the standardised RLB Citation IDs to benchmark AI-driven compliance risks surfacing in their own jurisdictions, with full traceability back to the original model output and the regulator's primary source.
- **The global compliance, derivatives-markets, and futures-clearing community** can freely adapt the Specialist Panel's screening methodologies to safeguard internal data pipelines and AI-assisted regulatory workflows.

Because RegLeg Brief conducts its own original research and adversarial analysis against frontier AI models, the detail in each published finding is precise enough to enable AI labs to take targeted hallucination-mitigation measures. Directions an AI lab might consider, drawing on the published findings, include:

- **Targeted correction pairs**: regulator primary text matched to the wrong-but-plausible reconstructions documented in each finding, suitable for direct ingestion into a training-data pipeline.
- **Quarterly embedded eval cycles**: continuous evaluation against a defined CFTC and customer-funds regulator portfolio, with regression monitoring on previously documented failure modes to track whether fine-tuning or RLHF adjustments are moving the needle on Threshold-Trigger Elision and Carve-Out Inversion.
- **Pre-release evaluation cycles**: sandboxed probes against catalogued failure shapes for capability releases touching derivatives, futures-clearing, and customer-funds regulatory content, before the release reaches customers.
- **Post-release model enhancements**: regulator-specific failure-surface monitoring as new CFTC amendments, staff letters, and concentration-rule updates enter a model's live deployment footprint.

AI labs and model developers named in any published finding have an unconditional [right of reply](https://reglegbrief.com/right-of-reply/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** CFTC Amendments to Regulation 1.25, Permissible Investments of Customer Funds by Futures Commission Merchants and Derivatives Clearing Organizations (2024) · Substrate documents: `R1-ACT-Q4_7_USC_6d_Commodity_Exchange_Act.pdf`, `p_03_REGULATION_17_CFR_1_25_b__3__ii____two_tier_asset_b_download.pdf`, `p_03_REGULATION_17_CFR_1_25_b__3__iv____dollar_weighted_download.pdf` · eCFR: ecfr.gov · CFTC: cftc.gov

**Citation IDs referenced:**

- `RLB-H-US-CFTC-FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024-Q001-Opus47`
- `RLB-H-US-CFTC-FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024-Q001-Sonnet46`
- `RLB-H-US-CFTC-FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024-Q002-Opus47`
- `RLB-H-US-CFTC-FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024-Q002-Sonnet46`
- `RLB-H-US-CFTC-FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024-Q004-Opus47`


## Related concepts

- Whitepaper: [cftc-reg-1-25-2024-customer-funds-investment-failures](/okf/whitepapers/cftc-reg-1-25-2024-customer-funds-investment-failures.md)
- Regulation: [FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024](/okf/regulations/FCM-DCO-CUSTOMER-FUNDS-INVESTMENTS-REG-1-25-2024.md)
- Methodology: [v2.3](/okf/methodology.md)