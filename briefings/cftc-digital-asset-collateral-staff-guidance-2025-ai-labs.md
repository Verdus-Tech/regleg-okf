---
type: "PublicBriefing"
title: "CFTC Digital Asset Collateral Staff Guidance 2025: Hallucination Patterns across frontier AI models"
slug: "cftc-digital-asset-collateral-staff-guidance-2025-ai-labs"
regulation_slug: "DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "v2.3"
news_featured_at: "2026-06-13T16:00:02.423607+00:00"
published_at: "2026-06-07T08:37:33.875369+00:00"
generated_at: "2026-06-11T01:41:27.739389+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cftc-digital-asset-collateral-staff-guidance-2025-ai-labs/"
timestamp: "2026-06-16T07:45:48.336540+00:00"
---

# CFTC Digital Asset Collateral Staff Guidance 2025: Hallucination Patterns across frontier AI models

- **Regulation.** [`DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025`](/okf/regulations/DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025.md) — CFTC Digital Asset Collateral No-Action Relief and Tokenized Asset Staff Guidance (Market Participants Division, December 2025)
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)

## News lead

Two frontier AI models running with web search enabled, both tested by the RLB Specialist Panel, produced confidently wrong reconstructions of the CFTC's Digital Asset Collateral No-Action Relief and Tokenized Asset Staff Guidance, the Market Participants Division's December 2025 framework that lets futures commission merchants accept bitcoin, ether and qualifying payment stablecoins as customer margin collateral under a phased pilot. The RegLeg Brief Specialist Panel tested both models on the operative staff letter and its February 2026 amendment, on which onboarding conditions persist past the initial three-month phase, and on the multi-DCO haircut rule for digital assets, and documents findings in which the models over-generalised partial sunset language to a continuing reporting obligation, fabricated an amendment reissuance date and a non-existent staff FAQ to support the wrong answer, dropped the OCC Interpretive Letter 1183 eligibility hook for national trust bank issuers, and defaulted to the base haircut threshold instead of the regulator's worst-case selection rule.

Claude Opus 4.7, asked which CFTC staff letter is operative for FCM acceptance of payment stablecoins backed by national-trust-bank reserves and what the amendment changed, wrote that "Staff Letter 25-40 was reissued as Staff Letter 26-05 on February 6, 2026" and described the revision as adding national trust banks as permitted issuers. The regulator's record confirms the reissuance and the definitional expansion but provides no basis for the specific February 6, 2026 date; the model fabricated the date while simultaneously eliding the OCC Interpretive Letter 1183 cross-reference that anchors national-trust-bank eligibility. Asked separately which conditions terminate at the end of the initial three-month onboarding phase, Opus 4.7 classified the weekly digital-asset holdings reporting obligation as one of the conditions that lapses. The staff letter's text places asset-type restrictions and incident-reporting conditions in the sunsetting set but explicitly continues the weekly reporting obligation for total crypto assets held in futures, foreign futures and cleared swaps customer accounts.

Claude Sonnet 4.6 reproduced the same condition-sunset error and added two further failures. On the amendment question, Sonnet 4.6 described the definitional change to add national trust banks without surfacing OCC Interpretive Letter 1183 as the eligibility hook. On the sunset question, the model went further than Opus 4.7: it cited "March 2026 CFTC Staff FAQs" as the authority for the weekly reporting requirement ceasing, a fabricated source document, and presented the termination as a precise procedural rule keyed to the third calendar month following notice filing. On the haircut-rate question, Sonnet 4.6 described the 20 per cent haircut floor as applying to digital assets not accepted by any registered DCO as initial margin, omitting the regulator's multi-DCO rule that the FCM must apply the highest haircut among all registered DCOs that accept the asset.

A futures commission merchant compliance officer, payment-stablecoin issuer counsel, DCO risk team, or regtech tool advising on the December 2025 framework and relying on either output would file under a sunset schedule for an obligation the regulator continues, cite a fabricated FAQ as procedural authority, structure a payment-stablecoin eligibility memo without the OCC Interpretive Letter 1183 hook, and apply the base haircut where the worst-case selection rule governs. That is the failure mode these findings document.


## Briefing

# Frontier AI models over-generalised a phased-pilot sunset and fabricated a staff FAQ on the CFTC's digital asset margin framework, regulatory-research panel finds

## Two frontier AI models, with web search enabled, classified the CFTC's weekly digital-asset reporting obligation as sunsetting at the end of the initial three-month pilot phase when the regulator's text explicitly continues it, fabricated a February 6, 2026 reissuance date and a "March 2026 CFTC Staff FAQs" source document, dropped the OCC Interpretive Letter 1183 cross-reference that anchors national-trust-bank eligibility for payment stablecoin issuers, and defaulted to the base 20 per cent haircut where the regulator's multi-DCO worst-case selection rule governs. The RegLeg Brief Specialist Panel calls the pattern "Phased Sunset Over-Generalisation and Amendment-Cycle Confabulation" and says it points to a systematic gap in how frontier models handle phased regulatory frameworks where partial sunset language is paired with continuing obligations, and recent amendment cycles where the corpus has not yet caught up to the regulator's published record.

**SINGAPORE, June 13, 2026.** Two frontier artificial-intelligence models generated reconstructions of the CFTC's Digital Asset Collateral No-Action Relief and Tokenized Asset Staff Guidance that over-generalise a phased pilot's sunset language, fabricate amendment provenance, and drop the cross-document eligibility hook for national-trust-bank stablecoin issuers, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The findings concern the **CFTC Market Participants Division's December 2025 Digital Asset Collateral No-Action Relief and Tokenized Asset Staff Guidance**, the framework that lets registered futures commission merchants accept bitcoin, ether, and qualifying payment stablecoins as customer margin collateral under a three-month phased onboarding pilot, subsequently amended by Staff Letter 26-05 to expand the payment-stablecoin issuer category. Both Anthropic's Claude Opus 4.7 and Claude Sonnet 4.6 were tested with web search active, mirroring how FCM compliance teams, payment-stablecoin issuer counsel, DCO risk officers, and regtech tools actually use the models when scoping the pilot's onboarding obligations, drafting eligibility memos, or briefing senior management on the post-phase reporting cadence.

## The Verbatim Rule: Sunset Language Is Partial, Not Total

The regulator's record on which onboarding conditions persist past the initial three-month phase is unambiguous. Staff Letter 25-40 enumerates the conditions that terminate at phase-end and separately lists the conditions that continue. The verbatim structure reads:

> "After the initial 3-month phase, asset-type restrictions and incident-reporting conditions will no longer apply. Weekly reports of total crypto assets held in each of the futures, foreign futures, and cleared swaps customer accounts continue."

The structural register matters. The regulator characterises the sunset as **partial**: a defined subset of conditions lapses, while specifically-enumerated reporting obligations persist. An FCM compliance officer reading the model output as a total sunset would file the firm under a reporting schedule the regulator does not authorise.

The regulator's record on the multi-DCO haircut rule is similarly explicit:

- **Base case**: a 20 per cent haircut floor applies to digital assets not accepted by any registered DCO as initial margin.
- **Multi-DCO case**: where multiple DCOs accept the same asset at different haircuts, the FCM must apply the **highest** such haircut.
- **Amendment hook**: Staff Letter 26-05 expanded the payment-stablecoin definition to include national trust banks; OCC Interpretive Letter 1183 provides the eligibility hook for that charter type.

## Claude Opus 4.7: Fabricated the Amendment Date, Over-Generalised the Sunset, Dropped the OCC Cross-Reference

Asked which CFTC staff letter is operative for FCM acceptance of payment stablecoins backed by reserves at an OCC-chartered national trust bank, and what the substantive change was, Claude Opus 4.7 (with web search on) wrote, verbatim:

> "Staff Letter 25-40 was reissued as Staff Letter 26-05 on February 6, 2026. The substantive change was a revision to the definition of 'payment stablecoin' to add national trust banks as permitted issuers."

**The fabricated date.** The regulator's record confirms the reissuance and the definitional expansion to national trust banks; it does not anchor February 6, 2026 as the reissuance date. The model committed to a specific date that reads as authoritative procedural citation but is the model's own reconstruction.

**The dropped cross-reference.** OCC Interpretive Letter 1183 is the regulatory instrument that provides the eligibility hook for national-trust-bank issuers under the expanded definition. The model answered the structural question (what changed) while dropping the operationally critical cross-reference (what anchors the new category's qualification), a payment-stablecoin issuer counsel drafting a charter-type eligibility memo against the output would miss the governing secondary instrument.

**The sunset over-generalisation.** Asked separately whether the weekly digital-asset reporting obligation continues after the three-month phase, Opus 4.7 wrote that this cadence "terminates at the end of the initial three-month phase per the letter". The letter does not terminate this obligation; it continues it. The model retrieved the partial-sunset structure and over-generalised it to a continuing obligation.

**Why it failed.** The RegLeg Brief Specialist Panel writes that the failure shape is characteristic of phased-framework retrieval: the model surfaces the headline sunset language correctly and then flattens the enumerated carve-outs in the regulator's text, defaulting to the simpler total-sunset interpretation. The fabricated reissuance date has the same shape on the amendment side, the model has enough corpus coverage to describe the amendment's structural effect but not enough to retrieve the specific date, producing a plausible confabulation instead of a retrieval failure.

The failure modes are classified as `misstated_rule` and `inference_drift` against substrate documents covering Staff Letter 25-40, Staff Letter 26-05, and OCC Interpretive Letter 1183.

## Claude Sonnet 4.6: Fabricated a Staff FAQ, Reproduced the Sunset Error, Dropped the Multi-DCO Worst-Case Rule

Given the parallel sunset brief, Sonnet 4.6 (with web search on) wrote:

> "Weekly Digital Asset Reporting (CEASES at end of third calendar month following notice filing). Based on the March 2026 CFTC Staff FAQs, this reporting terminates at the end of the third calendar month following the firm's notice filing."

**The fabricated source.** The "March 2026 CFTC Staff FAQs" is not a document the CFTC has published; the model committed to a named source title and date with no apparent retrieval basis. This is the most severe finding in the paper: a confidently-wrong answer supported by a fabricated authority document, presented as a precisely-worded procedural rule.

**The dropped multi-DCO rule.** Asked how the 20 per cent haircut applies in a multi-DCO context, Sonnet 4.6 wrote that the 20 per cent floor "applies to digital assets not accepted by any registered DCO as initial margin." The base threshold is correct, but the answer omitted the governing rule for the multi-DCO case, which is the only rule that matters when multiple DCOs accept the same asset at different haircuts. The regulator requires the FCM to apply the **highest** such haircut; Sonnet 4.6 returned a worst-case-less answer.

**The amendment elision.** On the payment-stablecoin amendment question, Sonnet 4.6 described the definitional expansion to national trust banks but omitted OCC Interpretive Letter 1183 as the eligibility hook. The structural question was answered while the operationally critical secondary instrument was dropped.

The failure modes are classified as `inference_drift` and `misstated_rule` against the same substrate.

## The Pattern: Phased Sunset Over-Generalisation and Amendment-Cycle Confabulation

The CFTC Digital Asset Collateral findings sit inside a broader failure class the RegLeg Brief Specialist Panel has been documenting across recent regulatory instruments published close to or after frontier models' training horizons, which it calls **Phased Sunset Over-Generalisation and Amendment-Cycle Confabulation**, frontier models systematically flattening partial-sunset enumerations into total sunsets, fabricating amendment-cycle metadata such as reissuance dates and FAQ titles, and dropping cross-document eligibility hooks where the operative rule turns on a named secondary instrument.

The white paper documents the pattern across the audited question set:

- **Phased-pilot sunset over-generalisation**: Both models classified the continuing weekly digital-asset reporting obligation as terminating at the end of the three-month phase, with Sonnet 4.6 anchoring the termination to a fabricated procedural rule.
- **Fabricated amendment-cycle metadata**: Opus 4.7 anchored the Staff Letter 26-05 reissuance to a specific February 6, 2026 date with no regulator basis; Sonnet 4.6 cited a "March 2026 CFTC Staff FAQs" document that does not exist.
- **Cross-document eligibility hook elision**: Both models described the payment-stablecoin definitional expansion to national trust banks without surfacing OCC Interpretive Letter 1183 as the eligibility hook.
- **Multi-entity worst-case selection failure**: Sonnet 4.6 stated the base 20 per cent haircut for the no-DCO case while dropping the governing rule that the highest haircut among multiple registered DCOs applies in the multi-DCO case.
- **Web search did not correct the errors**: Both models ran with web search active and neither configuration surfaced the regulator's primary text on the persisting reporting obligation, the amendment date, the OCC cross-reference, or the multi-DCO worst-case rule.

An FCM compliance officer, payment-stablecoin issuer counsel, DCO risk team, or regtech tool automating onboarding-readiness scoping or pilot-condition tracking on either model would carry the over-generalised sunset, the fabricated reissuance date, the missing OCC cross-reference, the fabricated FAQ citation, and the dropped worst-case haircut rule into the artefacts the firm produces.

## Why the Failure Is Invisible at Runtime

Both Claude outputs shared the same surface characteristics, structured enumerations of pilot conditions, dated procedural citations, regulator-attributed phrasing, and in Sonnet 4.6's case, an apparently precise named-source attribution that reads as a calibration signal. The white paper states the operational risk plainly:

> "The failure is not recoverable by the user in real-time: the model's output reads as a faithful summary of the regulator's phased-pilot structure, and validation would only happen if the reader already knew that the weekly reporting obligation is specifically carved out from the sunset, that no 'March 2026 CFTC Staff FAQs' document exists, that the February 6, 2026 reissuance date has no regulator basis, and that the multi-DCO case is governed by a worst-case selection rule rather than the base 20 per cent threshold."

FCM compliance teams, payment-stablecoin issuer counsel, DCO risk officers, and regtech tools advising on the December 2025 framework are the population most exposed. They use AI assistants to summarise CFTC staff letters, draft eligibility memos, and structure board-paper briefings against the pilot's tight onboarding timeline, the exact workflow in which the failure surfaces.

## What AI Labs Can Do: Suggested Probes (Open-Access)

The RegLeg Brief Specialist Panel documents five red-team probe designs in the white paper that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **Phased-pilot sunset enumeration probes.** Where a regulatory instrument lists a defined subset of conditions that terminate at a phase boundary and separately enumerates continuing obligations, test whether the model preserves the partial-sunset structure or over-generalises to a total sunset. Cadence-based obligations (weekly, monthly) are the highest-risk class for the over-generalisation failure mode.
2. **Cross-document eligibility hook probes.** Where an amendment expands a definitional category and the eligibility hook for the new category sits in a named secondary instrument (an interpretive letter, a grandfather provision, a cross-referenced charter type), test whether the model surfaces the specific secondary instrument or describes only the structural effect of the expansion.
3. **Multi-entity worst-case selection probes.** Where a numeric threshold is paired with a tie-breaking rule in multi-party contexts (highest haircut among multiple DCOs, most restrictive capital charge among multiple regulators), test whether the model applies the tie-breaking rule or defaults to the base threshold.
4. **Recent-amendment provenance probes.** For instruments amended within 6 to 12 months of the model's training horizon, test whether the model can accurately identify the amendment date, the superseded letter, and the specific definitional change without fabricating reissuance dates or FAQ titles to fill corpus gaps.
5. **Named-source citation verification probes.** Where the model commits to a document by title and date in support of a procedural rule, verify that the cited document exists and that the regulator documents it under the cited title; treat any unverifiable named-source citation as a candidate fabrication.

## Open-Access Risk Mitigation: A Public Good for AI Labs, Regulators, and the Compliance Community

RegLeg Brief operates as a completely ungated, open-access public resource. The white papers, per-finding cards, regulator verbatim excerpts, RLB Citation IDs, methodology notes and supporting data logs are all published without paywalls, registration walls, or data-licensing fees. By documenting original regulatory research without financial or distribution barriers, the platform ensures that:

- **AI engineering and alignment teams** can immediately ingest the verbatim model outputs and matched regulator-text excerpts to identify, reproduce, and address the structural failure modes the Specialist Panel documents.
- **Regulatory agencies and supervisors** can use the standardised RLB Citation IDs to benchmark AI-driven compliance risks surfacing in their own jurisdictions, with full traceability back to the original model output and the regulator's primary source.
- **The global compliance, derivatives-markets, and digital-asset community** can freely adapt the Specialist Panel's screening methodologies to safeguard internal data pipelines and AI-assisted regulatory workflows.

Because RegLeg Brief conducts its own original research and adversarial analysis against frontier AI models, the detail in each published finding is precise enough to enable AI labs to take targeted hallucination-mitigation measures. Directions an AI lab might consider, drawing on the published findings, include:

- **Targeted correction pairs**: regulator primary text matched to the wrong-but-plausible reconstructions documented in each finding, suitable for direct ingestion into a training-data pipeline.
- **Quarterly embedded eval cycles**: continuous evaluation against a defined CFTC and digital-asset regulator portfolio, with regression monitoring on previously documented failure modes to track whether fine-tuning or RLHF adjustments are moving the needle on Phased Sunset Over-Generalisation and Amendment-Cycle Confabulation.
- **Pre-release evaluation cycles**: sandboxed probes against catalogued failure shapes for capability releases touching derivatives, payments infrastructure, and digital-asset regulatory content, before the release reaches customers.
- **Post-release model enhancements**: regulator-specific failure-surface monitoring as new CFTC staff letters, FAQ updates, and amendment cycles enter a model's live deployment footprint.

AI labs and model developers named in any published finding have an unconditional [right of reply](https://reglegbrief.com/right-of-reply/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** CFTC Staff Advisory on Digital Asset Collateral and Tokenized Assets (2025) · Substrate documents: `p_02_GUIDELINE_CFTC_Staff_Letter_25_40___26_05___two_di_download.pdf`, `p_02_GUIDELINE_CFTC_Staff_Letters_25_40___26_05___post_download.pdf`, `p_03_NOTICE_CFTC_Staff_Letter_26_05__February_6__202_download.pdf` · CFTC: cftc.gov

**Citation IDs referenced:**

- `RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q005-Opus47`
- `RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q005-Sonnet46`
- `RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q006-Opus47`
- `RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q006-Sonnet46`
- `RLB-H-US-CFTC-DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025-Q007-Sonnet46`


## Related concepts

- Whitepaper: [cftc-digital-asset-collateral-staff-guidance-2025-ai-labs](/okf/whitepapers/cftc-digital-asset-collateral-staff-guidance-2025-ai-labs.md)
- Regulation: [DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025](/okf/regulations/DIGITAL-ASSET-COLLATERAL-TOKENIZED-ASSETS-STAFF-GUIDANCE-2025.md)
- Methodology: [v2.3](/okf/methodology.md)