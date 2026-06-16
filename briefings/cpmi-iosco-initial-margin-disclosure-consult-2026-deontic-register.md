---
type: "PublicBriefing"
title: "Deontic Register Failure on the CPMI-IOSCO Initial Margin Consultation 2026"
slug: "cpmi-iosco-initial-margin-disclosure-consult-2026-deontic-register"
regulation_slug: "CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
news_featured_at: "2026-06-12T16:00:24.233802+00:00"
published_at: "2026-06-07T08:31:57.765670+00:00"
generated_at: "2026-06-07T08:31:57.765670+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cpmi-iosco-initial-margin-disclosure-consult-2026-deontic-register/"
timestamp: "2026-06-16T07:42:08.028430+00:00"
---

# Deontic Register Failure on the CPMI-IOSCO Initial Margin Consultation 2026

- **Regulation.** [`CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026`](/okf/regulations/CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026.md) — CPMI-IOSCO Consultation on Updated Guidance and Public Disclosures to Implement Initial Margin Proposals
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)

## News lead

Two frontier AI models running with web search enabled, both tested by the RLB Specialist Panel, produced confidently wrong reconstructions of the CPMI-IOSCO Consultative Report on Updated Guidance and Public Disclosures to Implement Initial Margin Proposals, the May 2026 consultative document (d232) that codifies how central counterparties must disclose initial margin responsiveness, override frameworks, and simulation tools. The RegLeg Brief Specialist Panel tested both models on the consultation's text and on the January 2025 BCBS-CPMI-IOSCO report it implements, and documents findings in which the models softened mandatory CCP obligations into discretionary "should consider" language, invented a three-category taxonomy the source report does not contain, and fabricated a three-element public disclosure structure for override frameworks the guidance does not enumerate.

Claude Opus 4.7, asked what obligation the final CPMI-IOSCO guidance places on CCPs to provide margin simulation tools, wrote that CCPs "should consider" making the tools available to clearing members and, where feasible, their clients. The 2024 consultative text from which the obligation derives reads: "Margin simulation tools with certain minimum functionality should be made available by CCPs to clearing members and their clients." The model converted a positive obligation into a discretionary consideration, the difference between a CCP being expected to provide a tool and a CCP being expected to think about providing one. Asked about the structure of the January 2025 BCBS-CPMI-IOSCO report, Opus 4.7 also asserted the report's ten policy proposals fall into "three broad categories" of CCP transparency, governance and clearing-member transparency. The report's published text describes ten proposals aimed at resilience of the centrally cleared market ecosystem; no three-category taxonomy is stated in the source.

Claude Sonnet 4.6 reproduced the same obligation-softening on margin simulation tools and added a fabricated disclosure structure for the override framework. Asked what CCPs must publicly disclose about their override framework, Sonnet 4.6 enumerated three elements: instances or circumstances where overrides may be warranted, the key decision-makers authorised to exercise override discretion, and the permissible types of adjustments. The consultative text says only: "CCPs should publicly disclose relevant information on their override framework." The three-element list is the model's construction, not the regulator's.

A CCP risk officer, clearing-member compliance lead, or supervisor drafting a comment letter, board paper, or implementation plan against either output would understate CCP obligations on simulation tools, structure their override-framework disclosure against a taxonomy that does not exist in the source, and cite a category framework for the underlying policy proposals that the BIS press release does not endorse. That is the failure mode these findings document.


## Briefing

# Frontier AI models softened CCP margin obligations and invented disclosure taxonomies, regulatory-research panel finds

## Two frontier AI models, with web search enabled, converted a CPMI-IOSCO "should be made available" CCP obligation into a discretionary "should consider", manufactured a three-category taxonomy for the January 2025 BCBS-CPMI-IOSCO policy proposals that the source report does not state, and fabricated a three-element public disclosure structure for the override framework the consultation does not enumerate. The RegLeg Brief Specialist Panel calls the pattern "Obligation Softening" and says it points to a systematic drift in how frontier models weight mandatory regulatory language against discretionary phrasing in adjacent governance literature.

**SINGAPORE, June 12, 2026.** Two frontier artificial-intelligence models generated reconstructions of the CPMI-IOSCO May 2026 consultative report on initial margin transparency that soften mandatory central-counterparty obligations into discretionary language and invent structural taxonomies the regulator's text does not contain, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The findings concern the **CPMI-IOSCO Consultative Report on Updated Guidance and Public Disclosures to Implement Initial Margin Proposals** (BIS document d232, May 2026), which operationalises the ten policy proposals from the January 2025 BCBS-CPMI-IOSCO report on transparency and responsiveness of centrally cleared initial margin. Both Anthropic's Claude Opus 4.7 and Claude Sonnet 4.6 were tested with web search active, mirroring how central-counterparty risk teams, clearing-member compliance leads, and supervisors actually use the models when drafting comment letters, board papers, or implementation roadmaps.

## The Verbatim Rule: Mandatory Provision, Not Discretionary Consideration

The 2024 consultative text from which the margin simulation tool obligation derives states, verbatim:

> "Margin simulation tools with certain minimum functionality should be made available by CCPs to clearing members and their clients."

The structural register matters. "Should be made available" is the deontic phrasing CPMI-IOSCO uses to express a positive expectation on the regulated entity. It is not the same as "should consider making available", which expresses a procedural duty to deliberate, satisfied by the act of deliberation regardless of the outcome.

The May 2026 consultation preserves that register across the proposals it implements:

- **Margin simulation tools**: CCPs are expected to make tools with minimum functionality available to clearing members and clients.
- **Initial margin responsiveness measure**: CCPs must disclose the measure on a quarterly basis for the most relevant products per clearing service, reflecting the largest single-business-day and largest 20-business-day changes over 3-month and 12-month observation periods.
- **Override framework**: CCPs should publicly disclose relevant information on their override framework. The consultation does not enumerate sub-elements of that disclosure.
- **Implementation timeline**: CPMI and IOSCO encourage CCPs to implement the PQD amendments within 12 months of publication of the final report. That phrasing is genuinely discretionary, and is the one place the regulator chose softer language.

## Claude Opus 4.7: Softened Mandatory Provision, Invented a Three-Category Taxonomy

Asked what obligation the final CPMI-IOSCO guidance places on CCPs for margin simulation tools, Claude Opus 4.7 (with web search on) wrote, verbatim:

> "CCPs 'should consider' making margin simulation tools available to all clearing members, and where feasible their clients, including prospective clearing members and prospective clients, subject to appropriate non-disclosure agreements where necessary."

**The structural error.** The model converted "should be made available" into "should consider making available". A CCP risk-governance team configuring policy from this output would record the simulation-tool requirement as a deliberation duty rather than a provision duty. The compliance artefact, an internal policy, a board paper, a comment-letter response, would commit only to consider, not to provide.

**The taxonomy fabrication.** On a parallel question about the January 2025 BCBS-CPMI-IOSCO report that the May 2026 consultation implements, Opus 4.7 wrote that the report's ten policy proposals fall into three broad categories: CCP transparency, governance and review of CCP initial margin models, and clearing-member transparency to clients and to CCPs. The BIS press release text reads only that the report contains "ten final policy proposals which aim to increase the resilience of the centrally cleared market ecosystem in times of market stress." The three-category taxonomy is the model's structural overlay, not the regulator's.

**Why it failed.** The RegLeg Brief Specialist Panel writes that "the three-category framing matches the explanatory structure third-party legal commentary uses to make the ten proposals digestible, but the source documents themselves do not group the proposals taxonomically. The model promoted a commentary-side organising frame into a regulator-attributed claim."

The failure modes are classified as `inference_drift` against substrate document `R6-REPORT_CHAPTER-d232-cpmi-iosco-may-2026.pdf`.

## Claude Sonnet 4.6: Reproduced the Softening, Fabricated a Three-Element Disclosure Structure

Given the same simulation-tool brief, Sonnet 4.6 (with web search on) wrote:

> "The guidance uses 'should consider making' language: CCPs should consider making margin simulation tools available to all clearing members (CMs) and, where feasible, their clients."

The model went further than Opus 4.7 by explicitly attributing the "should consider" phrasing to the guidance text, despite the guidance using "should be made available".

**The disclosure-structure fabrication.** Asked what specific information CCPs must publicly disclose about their override framework, Sonnet 4.6 enumerated three elements:

> "(1) the instances or circumstances where overrides may be warranted; (2) the key decision-makers authorised to exercise override discretion; and (3) the permissible types of adjustments that can be made."

The consultative text says only that "CCPs should publicly disclose relevant information on their override framework." It does not enumerate sub-elements. A CCP disclosure team building a public-disclosure template against this output would structure the override disclosure around a three-bucket framework the consultation does not require and the final report may not adopt. Comment letters citing the three-element structure as a fixed requirement would commit the writer to a regulator position the regulator has not taken.

**The diagnostic.** When the Specialist Panel cross-checked the three-element list against the cited BIS sources, every URL the model produced was either contradictory to the claim or pretextual. The three elements appear nowhere in the consultation; they are a plausible reconstruction of what a comprehensive override disclosure would contain, projected back onto the regulator's text.

The failure mode is classified as `fabrication` against the same substrate document.

## The Pattern: Obligation Softening

The CPMI-IOSCO Initial Margin findings sit inside a broader failure class the RegLeg Brief Specialist Panel has been documenting across central-counterparty, market-infrastructure, and prudential-supervision work, which it calls **Obligation Softening**, frontier models systematically rephrasing positive regulatory obligations into discretionary deliberation duties, and structuring open-ended disclosure requirements against fabricated sub-element taxonomies.

The white paper documents the pattern across 17 audited questions:

- **Direct softening**: Two of the 17 questions show direct softening of "should be made available" into "should consider making" on the margin simulation tool obligation, reproduced independently by both models.
- **Taxonomy projection**: Two of the 17 questions show an invented three-category taxonomy projected onto the January 2025 ten-proposal report, again across both models.
- **Disclosure fabrication**: One question shows Sonnet 4.6 fabricating a three-element structure for an override-framework disclosure the consultation describes only as "relevant information".
- **Confidence without hedging**: Additional questions show consistent confidence in the model output, formatted enumerations, internal cross-references, no hedging, even where the regulator-attribution does not survive verification.

A CCP, clearing member, or supervisor automating consultation-response drafting or implementation-planning on either model would carry the softened obligation register and the fabricated taxonomies into the artefacts the firm produces.

## Why the Failure Is Invisible at Runtime

Both Claude outputs shared the same surface characteristics, structured enumeration, regulator-attributed phrasing, internal coherence, no hedging language. The white paper states the operational risk plainly:

> "The failure is not recoverable by the user in real-time: the model's output reads as a faithful summary of the regulator's position, and validation against the primary consultative text would only happen if the reader already knew that 'should consider' and 'should be made available' carry different deontic weight in CPMI-IOSCO drafting."

Central-counterparty risk teams, clearing-member compliance leads, and supervisors drafting comment letters by the consultation's 30 June 2026 deadline are the population most exposed. They use AI assistants to summarise the consultation, draft response language, and structure internal implementation plans on tight timelines, the exact workflow in which the failure surfaces.

## What AI Labs Can Do: Suggested Probes (Open-Access)

The RegLeg Brief Specialist Panel documents five red-team probe designs in the white paper that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **Deontic register preservation.** For consultations and guidance using "should be made available", "must disclose", "should consider", test whether the model preserves the exact deontic register or collapses to a single discretionary form. Diff the model output against the regulator's verbatim verb phrase.
2. **Taxonomic overlay detection.** Where a regulator documents an enumerated list without a stated category structure, test whether the model spontaneously generates a category taxonomy and attributes it to the regulator. Compare to the regulator's verbatim framing of the list.
3. **Disclosure-element enumeration.** For open-ended disclosure obligations ("relevant information on X"), test whether the model fabricates a closed sub-element list. Cross-check the sub-elements against the source's verbatim text.
4. **Commentary-vs-primary attribution.** Where third-party commentary structures the regulator's material more digestibly than the regulator does, test whether the model attributes the commentary structure to the regulator. Probe with prompts that force a primary-source citation.
5. **Cross-document consistency on co-author attribution.** Where one international report is co-authored by a specific subset of standard-setters (e.g. BCBS and IOSCO without CPMI), test whether the model preserves the subset or defaults to the larger trilateral grouping it sees more often in adjacent documents.

## Open-Access Risk Mitigation: A Public Good for AI Labs, Regulators, and the Compliance Community

RegLeg Brief operates as a completely ungated, open-access public resource. The white papers, per-finding cards, regulator verbatim excerpts, RLB Citation IDs, methodology notes and supporting data logs are all published without paywalls, registration walls, or data-licensing fees. By documenting original regulatory research without financial or distribution barriers, the platform ensures that:

- **AI engineering and alignment teams** can immediately ingest the verbatim model outputs and matched regulator-text excerpts to identify, reproduce, and address the structural failure modes the Specialist Panel documents.
- **Regulatory agencies and supervisors** can use the standardised RLB Citation IDs to benchmark AI-driven compliance risks surfacing in their own jurisdictions, with full traceability back to the original model output and the regulator's primary source.
- **The global compliance, treasury, and legal community** can freely adapt the Specialist Panel's screening methodologies to safeguard internal data pipelines and AI-assisted regulatory workflows.

Because RegLeg Brief conducts its own original research and adversarial analysis against frontier AI models, the detail in each published finding is precise enough to enable AI labs to take targeted hallucination-mitigation measures. Directions an AI lab might consider, drawing on the published findings, include:

- **Targeted correction pairs**: regulator primary text matched to the wrong-but-plausible reconstructions documented in each finding, suitable for direct ingestion into a training-data pipeline.
- **Quarterly embedded eval cycles**: continuous evaluation against a defined CPMI-IOSCO and multi-regulator portfolio, with regression monitoring on previously documented failure modes to track whether fine-tuning or RLHF adjustments are moving the needle on Obligation Softening.
- **Pre-release evaluation cycles**: sandboxed probes against catalogued failure shapes for capability releases touching financial-market infrastructure, central clearing, or cross-border prudential content, before the release reaches customers.
- **Post-release model enhancements**: regulator-specific failure-surface monitoring as new consultation cycles and final-report publications enter a model's live deployment footprint.

AI labs and model developers named in any published finding have an unconditional [right of reply](https://reglegbrief.com/right-of-reply/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** CPMI-IOSCO Consultative Report d232, Streamlining Variation Margin Disclosure (2026) · Substrate documents: `p_03_ANNEX_Override_framework___public_disclosure_r_d232_covernote.pdf` · CPMI portal: bis.org/cpmi

**Citation IDs referenced:**

- `RLB-H-INT-BIS-CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026-Q005-Sonnet46`


## Related concepts

- Whitepaper: [cpmi-iosco-initial-margin-disclosure-consult-2026-deontic-register](/okf/whitepapers/cpmi-iosco-initial-margin-disclosure-consult-2026-deontic-register.md)
- Regulation: [CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026](/okf/regulations/CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026.md)
- Methodology: [v2.3](/okf/methodology.md)