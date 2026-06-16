---
type: "AILabsWhitepaper"
title: "AI Hallucination Evaluation: CFTC Regulation 4.7 (Qualified Eligible Person Portfolio Requirements - 2024 Amendments)"
slug: "cpo-cta-regulation-4-7-qep-thresholds-2024-ai-labs"
audience: "ai_labs"
regulation_slug: "CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024"
regulation_id: "1838"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "2.3"
substrate_version: 1
generated_at: "2026-06-11T07:51:36.493587+00:00"
published_at: "2026-06-11T07:51:36.493587+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j3/us/cftc/CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024/ai-labs/"
timestamp: "2026-06-16T07:45:45.527055+00:00"
---

# AI Hallucination Evaluation: CFTC Regulation 4.7 (Qualified Eligible Person Portfolio Requirements - 2024 Amendments)

- **Regulation.** [`CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024`](/okf/regulations/CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024.md) — Amendments to CFTC Regulation 4.7, Qualified Eligible Person Portfolio Requirements for CPOs and CTAs
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)
- **Audience.** ai_labs
- **Methodology.** 2.3
- **Generated.** 2026-06-11T07:51:36.493587+00:00

## Executive summary

This audit presents findings from RegLeg's evaluation of frontier AI models against the September 2024 amendments to CFTC Regulation 4.7, which raised the qualified eligible person Portfolio Requirement thresholds from $2,000,000 to $4,000,000 for the Securities Portfolio Test and from $200,000 to $400,000 for the Initial Margin and Premiums Test. The amendment package was approved by the Commission on 11 September 2024, published at 89 FR 78814 on 27 September 2024, and is the first inflation adjustment to the QEP Portfolio Requirement since 1992. Two frontier AI subjects tested by the RLB Specialist Panel produced confident, specific answers across seventeen distinct questions in this audit that the CFTC's own primary text directly contradicts. The failures cluster into four thematic groups: NPRM-stage and final-rule CPI-U buying-power figures invented or substituted; statutory thresholds and Source Credits misstated against the U.S. Code; Commission voting records misattributed (including a commissioner who had departed two years earlier); and Federal Register correction-record fields misreported by CFR Part, effective date, and title-line. Each finding is bound to verbatim regulator-issued primary source text. For AI lab teams fielding frontier models into U.S. derivatives and asset-management deployments, the pattern signals systematic gaps in how the models handle statutory-figure quotation, regulatory-history reproduction, and rulemaking-record reproduction on technical regulatory documents.

## Full whitepaper

# AI Hallucination Evaluation: CFTC Regulation 4.7 (Qualified Eligible Person Portfolio Requirements - 2024 Amendments)

## Executive Summary

This audit presents findings from RegLeg's evaluation of frontier AI models against the September 2024 amendments to CFTC Regulation 4.7, which raised the qualified eligible person Portfolio Requirement thresholds from $2,000,000 to $4,000,000 for the Securities Portfolio Test and from $200,000 to $400,000 for the Initial Margin and Premiums Test. The amendment package was approved by the Commission on 11 September 2024, published at 89 FR 78814 on 27 September 2024, and is the first inflation adjustment to the QEP Portfolio Requirement since 1992. Two frontier AI subjects tested by the RLB Specialist Panel produced confident, specific answers across seventeen distinct questions in this audit that the CFTC's own primary text directly contradicts. The failures cluster into four thematic groups: NPRM-stage and final-rule CPI-U buying-power figures invented or substituted; statutory thresholds and Source Credits misstated against the U.S. Code; Commission voting records misattributed (including a commissioner who had departed two years earlier); and Federal Register correction-record fields misreported by CFR Part, effective date, and title-line. Each finding is bound to verbatim regulator-issued primary source text. For AI lab teams fielding frontier models into U.S. derivatives and asset-management deployments, the pattern signals systematic gaps in how the models handle statutory-figure quotation, regulatory-history reproduction, and rulemaking-record reproduction on technical regulatory documents.

## Background: the September 2024 amendments

On 11 September 2024 the Commodity Futures Trading Commission voted to approve a final rule amending 17 CFR 4.7, the qualified eligible person regime applicable to commodity pool operators and commodity trading advisors. The rule was published at 89 FR 78814 on 27 September 2024. The rule's two principal moving parts are (a) inflation adjustment of the Portfolio Requirement thresholds from the levels set in 1992 ($2,000,000 Securities Portfolio Test, $200,000 Initial Margin and Premiums Test) to the amended levels of $4,000,000 and $400,000 respectively; and (b) a series of operational amendments to the recordkeeping, disclosure, and reporting framework for 4.7-exempt CPOs and CTAs.

The amendment package is structurally important to the AI-lab audit lens for three reasons. First, the rulemaking record spans an NPRM stage (88 FR 70852, October 2023), a pre-print version, the final-rule pre-print, the published final rule, and a December 2024 Federal Register correction; this layered record creates several discrete reproduction tasks where the AI is asked to quote a specific figure or field. Second, the rule explicitly anchors its inflation analysis to specific CPI-U reference months (February 2023 at NPRM stage; July 2024 at final-rule stage); each reference month yields a different buying-power figure, and any model that conflates them produces a wrong but plausible answer. Third, the rule sits inside a statutory framework (the Commodity Exchange Act, codified at 7 USC 6n and 1a(18)) whose Source Credits, recordkeeping provisions, and ECP-eligibility thresholds are themselves the subject of verbatim-quotation tasks in legal, compliance, and consulting deliverables.

The RLB Specialist Panel designed the questions in this audit to mirror how lawyers, compliance officers, fund administrators, financial advisers, and management consultants actually use AI on this practice area: drafting memos, populating registers, preparing testimony exhibits, drafting client deliverables, and verifying statutory and Federal Register citations. Each question is anchored to verbatim regulator-issued primary substrate.

## When This Affects an AI Lab

MAS Notice 637 sits in Singapore's prudential framework; this audit by contrast targets the September 2024 amendments to CFTC Regulation 4.7, which sit at the operational core of the U.S. CFTC's QEP regime for commodity pool operators and commodity trading advisors, and at the intersection of legal, compliance, fund-administration, and consulting work for the U.S. private-fund industry. Users asking AI models about this rulemaking include: commodity-pool and commodity-derivatives lawyers at outside firms and in-house counsel; compliance officers at CPO, CTA, and FCM firms; fund administrators producing annual rule-change trackers; in-house and external auditors preparing audit working papers; financial advisers at wealth-management firms with commodity-pool exposure; and regulatory consultants supporting stakeholder-engagement appendices and client briefings.

Any frontier model deployed in an assistant, copilot, or document-query capacity in these contexts will routinely receive the question types tested in this audit: which statutory threshold applies to a CIV under 7 USC 1a(18)(B)(ii)(I), what the NPRM-stage and final-rule CPI-U buying-power figures are, how the Commission voted on the final rule, which trade associations submitted comment letters, what the statutory Source Credit for 7 USC 6n records, what the statutory retention period and registration-expiration date are under 7 USC 6n, and how the December 2024 Federal Register correction is indexed.

The downstream harms are concrete. A lawyer who paste-copies an AI-stated ECP threshold of $5,000,000 or $25,000,000 into a partner-level memo introduces a two-hundred-fold or forty-fold misstatement of the actual $1,000,000,000 statutory threshold, with direct consequences for the client's counterparty-eligibility analysis. A fund administrator who logs the AI's stated CFR Parts and effective date on the 89 FR 96897 correction populates the annual tracker with incorrect operational data. A consulting deliverable that recites approximately 40 comment letters where the final rule documents 8, and that names commenters not in the regulator's footnote, leaves the client deliverable directly testable against the published record. For the lab, confident wrong outputs on authoritative regulatory text are the misuse-claim exposure that arises when enterprise customers act on model outputs in high-stakes contexts.

## Aggregate impact

The 17 findings in this audit cluster into five thematic groups, each of which has direct AI-lab eval implications. The clusters point to a generation pattern where the model commits, with no hedging, to a verbatim-looking answer on a quotation, threshold, citation, or named-individual question, and where the model's answer diverges from the regulator's source text on a specific, testable fact. The substrate for every finding in this audit is regulator-issued primary text held by the RLB Specialist Panel; the model had access to that substrate at query time via search and retrieval.

### NPRM-vs-final CPI-U figure errors (Findings 3, 4, 5, 7)

- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q011-Sonnet46** (Sonnet 4.6): AI invented February-2023 buying-power figures that the NPRM does not record. Reported $4,070,000 and $407,000 NPRM-era figures, where the NPRM's verbatim text records $4,270,000 and $427,000.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q016-Opus47** (Opus 4.7): AI reported a July-2024 buying-power figure that the final-rule pre-print does not record. Reported $4,464,200 and $446,420 (apparent extrapolation), where the final-rule pre-print records $4,464,726 and $446,472.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q016-Sonnet46** (Sonnet 4.6): AI reported the NPRM-era February-2023 figures in answer to a July-2024 final-rule question. Reported $4,270,000 and $427,000 (the NPRM-stage February-2023 figures) in response to a July 2024 question.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q020-Sonnet46** (Sonnet 4.6): AI invented February-2023 figures in a CCO briefing memo where the NPRM records different figures. Reported $4,070,000 and $407,000 as the NPRM verbatim figures, where the NPRM records $4,270,000 and $427,000.

### Statutory threshold and recordkeeping rule misstatements (Findings 1, 10, 11, 12, 15)

- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q005-Opus47** (Opus 4.7): AI misstated the regulator's stated rule on existing-investor grandfathering. Asserted a subscription-agreement / re-investment carve-out theory where the final-rule preamble provides a direct grandfathering rule for existing QEPs.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q024-Opus47** (Opus 4.7): AI misstated the statutory total-assets threshold for the ECP-eligible collective investment vehicle test. Reported total-assets threshold as $5,000,000 where the statute records $1,000,000,000 (in the aggregate for grouped vehicles).
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q024-Sonnet46** (Sonnet 4.6): AI misstated the statutory total-assets threshold and omitted the December 21, 2000 definitional anchor date. Reported total-assets threshold as $25,000,000 and did not name the statute's December 21, 2000 definitional anchor.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q027-Sonnet46** (Sonnet 4.6): AI misstated the statute's books-and-records retention period. Reported the statutory retention period as five years, where 7 USC 6n(3)(A) records three years.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q029-Sonnet46** (Sonnet 4.6): AI misstated the statutory registration-expiration date. Reported expiration date as the 31st day of October, where the statute records the 30th day of June.

### Source Credit and rulemaking-history fabrication (Findings 8, 9, 13, 14)

- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q021-Opus47** (Opus 4.7): AI reported a wrong Commission-approval footer date on the NPRM pre-print PDF. Reported the footer as 'Commission approved on 10/2/2023', where the actual footer records 9/29/2023.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q021-Sonnet46** (Sonnet 4.6): AI reported a wrong Commission-approval footer date on the NPRM pre-print PDF. Reported the footer as 'Commission approved on 10/2/2023', where the actual footer records 9/29/2023.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q028-Opus47** (Opus 4.7): AI misstated the statutory Source Credit, naming Pub. L. citations the statute does not list. Reported four post-1978 amendment Pub. L. citations (1992, 2000, 2010 specifically) where the Source Credit records only Pub. L. 97-444 (1983).
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q028-Sonnet46** (Sonnet 4.6): AI misstated the statutory Source Credit, naming Pub. L. citations the statute does not list. Listed four post-1978 amendments (1983, 1992, 2000, 2010 plus Stat. citations that diverge from the Source Credit) where the Source Credit records only Pub. L. 97-444 (1983) and Pub. L. 95-405 (1978).

### Commission vote and commenter-set misattribution (Findings 2, 6)

- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q008-Sonnet46** (Sonnet 4.6): AI misattributed the Commission's vote and named a commissioner who had departed two years earlier. Named Commissioner Brian Quintenz as a possible affirmative voter despite his 2022 departure, with the actual fifth voter Goldsmith Romero missing from the model's list.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q017-Opus47** (Opus 4.7): AI reported approximately 40 comment letters where the final-rule documents receipt of eight. Reported approximately 40 comment letters and named additional trade associations (SIFMA AMG-only listed as 'SIFMA', plus ICI, IAA, and ABA Business Law Section) that the final-rule footnote does not include.

### Federal Register correction-record errors (Findings 16, 17)

- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q031-Opus47** (Opus 4.7): AI misstated the CFR Parts affected by the 89 FR 96897 correction and the effective date. Reported affected parts as 17 CFR Parts 37, 38, and 40 with a 12/6/2024 effective date; the index entry records 17 CFR Part 40 only with a 12/9/2024 effective date.
- **RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q031-Sonnet46** (Sonnet 4.6): AI misstated the CFR Part and the correction title-line on the 89 FR 96897 record. Reported affected part as 17 CFR Part 4 with a title invented to match the QEP rulemaking; the index records 17 CFR Part 40 and the title 'Provisions Common to Registered Entities; Correction'.

Two structural risk drivers compound across the five themes. First, the model is willing to construct numeric, structurally plausible answers (a CPI-U buying-power figure, a statutory threshold figure, an effective date) by analogy with known reference points rather than by retrieval of the regulator's actual text. Second, the model is willing to reconstruct historical or institutional records (Source Credit chains, Commission voting rosters, commenter lists) from general topical knowledge rather than from the source document. Both behaviours are silent in the deliverable; neither output signals to the user that the underlying claim has no basis in the regulator's published text.

For U.S. derivatives and asset-management enterprise deployments, these failure modes will recur on every CFTC rulemaking that (a) anchors quantitative analysis to specific reference months, (b) carries a multi-stage rulemaking record (NPRM pre-print, final-rule pre-print, published rule, Federal Register correction), and (c) sits inside a statutory framework whose Source Credits and codified thresholds are the subject of verbatim quotation tasks. All three characteristics are common across the CFTC, SEC, and other prudential and securities portfolios.

## Per-finding analysis

### Finding 1 . Misstated grandfather rule for existing QEP investors under prior thresholds

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q005-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a misstated-rule failure on the existing-investor grandfathering provision of the September 2024 final-rule preamble. When asked to draft an advisory memo on what the amended Portfolio Requirement does to three existing QEPs who no longer meet the updated threshold, the subject model produced an answer turning on a 'pre-existing subscription agreement' carve-out theory and 'mechanical features of the existing subscription' analysis. Neither construct appears in the regulator's text. The preamble states directly that a CPO or CTA is not required to redeem pool participations of, or terminate the advisory relationship with, a person who qualified as a QEP under the prior Portfolio Requirement but who does not meet the updated Portfolio Requirement. The gap implicates the generation layer's handling of grandfathering-rule queries where the correct answer is a direct rule recorded in the preamble; the model synthesised a plausible-looking carve-out by analogy with general transactional-law conventions. Recommended eval probes: grandfathering-rule queries on rulemakings that document the rule directly in the preamble; advisory-memo drafting queries where the regulator's own text resolves the question.

### Finding 2 . Misattributed Commission vote and named non-sitting commissioner

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q008-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a misattribution failure on the Commission's voting record. When asked to draft a briefing memo on the September 2024 final rule including how each commissioner voted, the subject model produced an answer naming Chairman Behnam, Commissioners Johnson, Pham, and Mersinger affirmative, and naming Commissioner Brian Quintenz (with a self-flagged note about Quintenz's possible departure) as the fifth voter, omitting Commissioner Christy Goldsmith Romero entirely. Quintenz departed the Commission in 2022. The final-rule Appendix 1 Voting Summary at 89 FR 78814 records Goldsmith Romero as the fifth affirmative voter. The gap implicates the generation layer's handling of agency-composition queries at a specific historical date: the model has reconstructed the roster from training-era data rather than from the source record. Recommended eval probes: named-individual queries on agency voting records at specific dates; agency-roster queries on Commissioner sets at the date of a specific rulemaking action; voting-Summary reproduction queries that require pulling the Appendix at the cited page of the Federal Register.

### Finding 3 . NPRM-stage CPI-U buying-power figures invented

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q011-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on NPRM-stage CPI-U buying-power figure reproduction. When asked to draft a technical note quantifying the inflation gap that the September 2024 amendments sought to address, with specific CPI-U-based buying-power calculations from the NPRM, the subject model produced figures of $4,070,000 and $407,000 for the $2 million and $200,000 thresholds at February 2023. The NPRM's verbatim text records $4,270,000 and $427,000 at the same reference month. The 5 percent gap between the model's figures and the regulator's stated figures cannot be reconciled to any CPI-U release. The gap implicates the generation layer's handling of regulator-issued quantitative figure queries: the model produced a coherent paragraph anchored on invented figures rather than retrieve the regulator's source figures. Recommended eval probes: regulator-issued figure-quotation queries on rules that document specific dollar buying-power calculations; CPI-U-based threshold-quotation queries at specific reference months; retrieval-grounded queries that require pulling the verbatim figure from the source document.

### Finding 4 . July 2024 CPI-U buying-power figures invented (Opus 4.7)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q016-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on final-rule CPI-U buying-power figure reproduction. When asked to draft a CCO briefing memo opening with the July 2024 CPI-U buying-power figures from the final-rule pre-print's Section II.A, with both updated figures quoted verbatim, the subject model produced $4,464,200 and $446,420 for the $2 million and $200,000 thresholds. The final-rule pre-print records $4,464,726 and $446,472 at the same reference month. The model has produced figures that are close to the source but not identical; the difference indicates near-extrapolation behaviour rather than retrieval. The gap is interesting precisely because the model's answer is close enough to the regulator's text to suggest the model partially retrieved the figure and then rounded or substituted. Recommended eval probes: precise-figure verbatim-quotation queries where the regulator's text records a specific multi-digit figure; rounded-versus-verbatim figure-quotation queries; retrieval-grounded queries that require pulling the verbatim figure with full precision.

### Finding 5 . July 2024 CPI-U buying-power figures stated as outdated NPRM-era figures (Sonnet 4.6)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q016-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an outdated-fact failure on final-rule CPI-U buying-power figure reproduction. When asked to draft a briefing memo opening with the July 2024 CPI-U buying-power figures from the final-rule pre-print, the subject model produced $4,270,000 and $427,000 for the $2 million and $200,000 thresholds. Those are the NPRM-stage February 2023 figures, not the final-rule July 2024 figures (which are $4,464,726 and $446,472). The model has substituted the earlier-stage figures for the requested later-stage figures, presenting them as the July 2024 buying-power equivalents. The gap implicates the generation layer's handling of multi-stage rulemaking records where the same conceptual question takes a different numeric answer at different stages: the model has selected the wrong stage's answer. Recommended eval probes: NPRM-versus-final-rule figure-quotation queries on rules that update the figure between stages; stage-specific buying-power queries where the model must distinguish the NPRM reference month from the final-rule reference month.

### Finding 6 . Inflated comment-letter count and invented commenter names

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q017-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a fabricated-fact failure on rulemaking-record commenter-set reproduction. When asked to draft a stakeholder-engagement appendix opening with the exact number of comment letters received on the NPRM and naming the trade-association commenters cited in the relevant footnote, the subject model reported approximately 40 comment letters and named SIFMA AMG, IAA, AIMA, MFA, ICI, NFA, and the American Bar Association Business Law Section's Committee on Derivatives and Futures Law. The final-rule pre-print documents receipt of eight comment letters, with the relevant footnote naming SIFMA AMG, IAA, AIMA, MFA, ICI, and NFA. The model has inflated the count by roughly five-fold and added an extended commenter that does not appear in the footnote. The gap implicates the generation layer's handling of rulemaking-record-quotation queries where the correct answer is a specific count and a specific named-commenter list. Recommended eval probes: comment-letter-count queries on rulemakings where the count is recorded in the Background discussion; trade-association named-commenter queries on rulemaking footnotes; retrieval-grounded queries that require pulling the count and the named list from the source.

### Finding 7 . NPRM-stage CPI-U buying-power figures invented (verbatim-quote request)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q020-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on NPRM-stage CPI-U buying-power figure reproduction in a CCO briefing memo. When asked to quote verbatim the NPRM-era $2 million and $200,000 buying-power equivalents at February 2023, the subject model produced $4,070,000 and $407,000. The NPRM records $4,270,000 and $427,000 at the same reference month. The model has produced the same fabrication pattern as Finding 11 in a different deliverable. The repetition suggests a generation-layer pattern rather than a single retrieval miss: when asked for the NPRM-stage figures, the model produces $4,070,000 and $407,000, which appear to be a stable hallucination across the question set. Recommended eval probes: regulator-issued figure-quotation queries where the model has previously produced a specific wrong figure; cross-prompt consistency queries on figure-quotation tasks; retrieval-grounded queries that require pulling the verbatim figure from the source.

### Finding 8 . Wrong NPRM-pre-print footer date for Commission approval

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q021-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on NPRM-pre-print footer text reproduction. When asked to quote the recurring footer of the NPRM pre-print PDF that records the Commission approval date, the subject model reported 'Pre-Print Version - Commission approved on 10/2/2023'. The actual footer reads 'Pre-Print Version - Commission approved on 9/29/2023 (subject to technical corrections required for Federal Register publication)'. The model has conflated the 9/29/2023 (Friday) Commission approval date with the 10/2/2023 (Monday) open Commission meeting date at which the proposal was discussed. The gap implicates the generation layer's handling of multi-date rulemaking records where the model must distinguish the formal approval date from related-event dates. Recommended eval probes: footer-text quotation queries on pre-print PDFs where the recorded date diverges from the publication or meeting date; date-distinguishing queries on rulemaking records that carry multiple related dates; retrieval-grounded queries that require pulling the verbatim footer text from the source PDF.

### Finding 9 . Wrong NPRM-pre-print footer date for Commission approval (Sonnet 4.6)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q021-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on NPRM-pre-print footer text reproduction, paralleling Finding 8 on Opus 4.7. When asked to quote the recurring footer of the NPRM pre-print PDF that records the Commission approval date, the subject model reported 'Pre-Print Version - Commission approved on 10/2/2023'. The actual footer records 9/29/2023. The model has produced the same conflation pattern as Opus 4.7 on the same question, suggesting a generation-layer pattern where both subject models map the multi-date rulemaking record onto the salient open-meeting date rather than the formal approval date recorded in the footer. Recommended eval probes: cross-model consistency queries on date-quotation tasks; multi-date rulemaking-record queries that require distinguishing the formal approval date from the open-meeting date; retrieval-grounded queries that require pulling the verbatim footer text.

### Finding 10 . Wrong total-assets threshold in 7 USC 1a(18)(B)(ii)(I) for collective investment vehicles

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q024-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a misstated-rule failure on the statutory total-assets threshold in 7 USC 1a(18)(B)(ii)(I) for ECP-qualifying collective investment vehicles. When asked to quote verbatim the in-the-aggregate total-assets threshold, the subject model reported $5,000,000. The statute records $1,000,000,000 (in the aggregate for grouped vehicles), anchored to the QEP, accredited investor, and qualified purchaser definitions in effect on December 21, 2000. The misstatement is by a factor of two hundred. The gap implicates the generation layer's handling of high-magnitude statutory thresholds in counterparty-eligibility provisions: the model has substituted a different threshold (likely confused with the $5,000,000 ECP-individual threshold elsewhere in 1a(18)) for the specific CIV threshold. Recommended eval probes: high-magnitude statutory-threshold queries where the model must distinguish multiple thresholds within the same statutory section; ECP-eligibility queries on collective investment vehicles; retrieval-grounded queries that require pulling the verbatim threshold figure from the U.S. Code.

### Finding 11 . Wrong total-assets threshold and definition reference date in 7 USC 1a(18)(B)(ii)(I)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q024-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on the statutory total-assets threshold in 7 USC 1a(18)(B)(ii)(I) and the statutory definitional anchor date. When asked to quote verbatim the threshold and the anchor date, the subject model reported $25,000,000 and omitted the December 21, 2000 anchor. The statute records $1,000,000,000 (in the aggregate for grouped vehicles), anchored to definitions in effect on December 21, 2000. The misstatement is by a factor of forty on the threshold, and the missing anchor date allows the AI's reader to substitute current-day QEP, accredited investor, or qualified purchaser definitions for the statute's intended fixed-date definitions. The gap implicates the generation layer's handling of statutory provisions with fixed-date definitional anchors. Recommended eval probes: fixed-date definitional-anchor queries on statutory provisions; ECP-eligibility threshold queries; retrieval-grounded queries that require pulling both the threshold and the anchor date.

### Finding 12 . Wrong statutory recordkeeping period under 7 USC 6n(3)(A)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q027-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a misstated-rule failure on the statutory books-and-records retention period in 7 USC 6n(3)(A). When asked to quote verbatim the statutory retention period and inspection rights, the subject model reported five years (deriving the period from CFTC Regulation 1.31 rather than the statute). 7 USC 6n(3)(A) records a three-year minimum, or longer if the Commission so directs. The model has conflated the statutory minimum with the regulation-implemented period. The gap implicates the generation layer's handling of statute-versus-regulation distinctions on technical compliance provisions: the model is willing to quote a regulation-derived figure as if it were the statutory figure. Recommended eval probes: statute-versus-regulation distinguishing queries on recordkeeping provisions; minimum-versus-implemented retention period queries; retrieval-grounded queries that require pulling the verbatim statutory text.

### Finding 13 . Wrong Source Credit history for 7 USC 6n

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q028-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on the Source Credit reproduction for 7 USC 6n. When asked to reproduce verbatim the statute's Source Credit, the subject model produced a chain including Pub. L. 102-546 (1992), Pub. L. 106-554 (2000), and Pub. L. 111-203 (2010), and omitted Pub. L. 97-444 (1983). The actual Source Credit reads: '(Sept. 21, 1922, ch. 369, paragraph 4n, as added Pub. L. 93-463, title II, paragraph 205(a), Oct. 23, 1974, 88 Stat. 1398; amended Pub. L. 95-405, paragraph 9, Sept. 30, 1978, 92 Stat. 870; Pub. L. 97-444, title II, paragraph 213, Jan. 11, 1983, 96 Stat. 2305.)' The model has reconstructed the chain from topical CPO/CTA regulatory-history knowledge rather than retrieved the codified Source Credit. The gap implicates the generation layer's handling of treatise-grade statutory-history reproduction tasks. Recommended eval probes: Source Credit verbatim-reproduction queries on U.S. Code provisions; statutory-history chain queries where general topical knowledge diverges from the codified chain; retrieval-grounded queries that require pulling the Source Credit from the U.S. Code itself.

### Finding 14 . Wrong Source Credit history for 7 USC 6n (Sonnet 4.6)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q028-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on the Source Credit reproduction for 7 USC 6n, paralleling Finding 13 on Opus 4.7. When asked to reproduce verbatim the statute's Source Credit, the subject model produced an extended amendment list including the 1983 Futures Trading Act, the 1992 Futures Trading Practices Act, the 2000 Commodity Futures Modernization Act, and the 2010 Dodd-Frank Act. The actual Source Credit lists only Pub. L. 95-405 (1978) and Pub. L. 97-444 (1983) as the amendment chain through to the codified text. The other public laws named did amend other provisions of the Commodity Exchange Act but not 7 USC 6n. The model has substituted topical regulatory-history knowledge for the actual Source Credit. The same generation pattern as Opus 4.7 on the same task. Recommended eval probes: cross-model consistency queries on Source Credit reproduction; statutory-history-versus-topical-history distinguishing queries; retrieval-grounded queries that require pulling the codified Source Credit.

### Finding 15 . Wrong statutory registration-expiration date in 7 USC 6n(2)

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q029-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies an inference drift failure on the statutory registration-expiration date in 7 USC 6n(2). When asked to quote verbatim the statutory expiration rule, the subject model reported the 31st day of October. 7 USC 6n(2) records the 30th day of June. The model has misstated the statutory date by four months. The gap implicates the generation layer's handling of statutory-date provisions where the date is specific and operational: a registration-renewal calendar memo built on the AI's stated October 31 date would misalign the firm's renewal cycle by four months, with direct registration-lapse exposure. Recommended eval probes: statutory-date verbatim-quotation queries on registration and renewal provisions; statutory-versus-administrative-date distinguishing queries; retrieval-grounded queries that require pulling the statutory date from the U.S. Code.

### Finding 16 . Wrong CFR Parts on the 89 FR 96897 correction index record

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q031-Opus47

**Subject:** Claude Opus 4.7 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a misstated-rule failure on the December 2024 Federal Register correction index record. When asked to reproduce verbatim the CFTC Final Rules 2024 index-page record of the 89 FR 96897 correction, the subject model reported affected CFR Parts as 17 CFR Parts 37, 38, and 40 and the effective date as 12/6/2024. The index records 17 CFR Part 40 only and an effective date of 12/9/2024 (Monday). The model has overstated the CFR-Part scope by two parts and misaligned the effective date by three days (treating the publication date as the effective date). The gap implicates the generation layer's handling of Federal Register index-record reproduction tasks where multiple fields must be quoted in concert. Recommended eval probes: Federal Register correction-record verbatim-reproduction queries; multi-field index-entry queries where the model must quote publication date, effective date, CFR Parts, and title-line in concert; retrieval-grounded queries that require pulling the index entry from the Federal Register.

### Finding 17 . Wrong CFR Part and title on the 89 FR 96897 correction index record

**Citation:** RLB-H-US-CFTC-CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024-Q031-Sonnet46

**Subject:** Claude Sonnet 4.6 (web search on)

**Substrate:** verbatim source bound by RLB Specialist Panel

This finding identifies a misstated-rule failure on the 89 FR 96897 correction record where the model has misattributed the correction across two distinct CFTC rulemakings. When asked to reproduce verbatim the index-page record, the subject model reported affected CFR Part as 17 CFR Part 4 and the title-line as a correction to the QEP-definition rulemaking. The index records 17 CFR Part 40 and the title 'Provisions Common to Registered Entities; Correction'. The model has read the index entry as a correction to the Reg 4.7 QEP rulemaking on substantive grounds (because the audit topic is Reg 4.7), when the index records the correction as applying to a different (Provisions Common to Registered Entities) rulemaking. The gap implicates the generation layer's handling of topical-context bias on Federal Register index-record reproduction. Recommended eval probes: topical-bias-resistance queries on Federal Register index reproduction; rulemaking-attribution queries where the model must distinguish substantively related but procedurally distinct rulemakings; retrieval-grounded queries that require pulling the index entry without topical inference.

## What Your Team Should Do

The targeted evaluation work for the failure modes surfaced in this audit should focus on four areas.

**First, expand evaluation coverage of multi-stage rulemaking-record reproduction tasks.** The CFTC Regulation 4.7 record spans an NPRM at 88 FR 70852, a pre-print version of the NPRM, a final-rule pre-print, the published final rule at 89 FR 78814, and a December 2024 correction at 89 FR 96897. Each stage carries discrete fields a practitioner might be asked to quote: a CPI-U reference month, a buying-power figure, a comment-letter count, a Commission voting roster, a footer date, an effective date, an affected CFR Part. The findings in this audit show the model is willing to fabricate or substitute on each of these fields where the correct answer is a quotation from the source document. Eval probes should include (a) NPRM-stage versus final-rule figure-quotation queries on rules that update the figure between stages; (b) Federal Register correction-record queries where the correction title diverges from the substantive rulemaking topic; (c) NPRM-pre-print footer-text quotation queries where the footer date diverges from the published Federal Register date.

**Second, expand evaluation coverage of verbatim statutory-text reproduction.** The findings in this audit show the model misstating the 7 USC 1a(18)(B)(ii)(I) total-assets threshold by factors of forty and two hundred, misstating the 7 USC 6n(3)(A) recordkeeping retention period (three years vs five), misstating the 7 USC 6n(2) registration expiration date (June 30 vs October 31), and misstating the 7 USC 6n Source Credit (substituting topical regulatory-history knowledge for the codified amendment chain). Eval probes should include (a) verbatim-quotation queries on statutory thresholds where the correct answer is a specific dollar figure; (b) verbatim-quotation queries on statutory date provisions; (c) verbatim-quotation queries on statutory Source Credits where the correct answer is a specific Pub. L. chain.

**Third, expand evaluation coverage of institutional-record reproduction.** The findings in this audit show the model misattributing the Commission's vote on the final rule (naming a departed commissioner, omitting the actual fifth voter), and inflating the comment-letter count from eight to approximately forty (with an extended commenter list). Eval probes should include (a) named-individual queries on agency voting records where the correct answer is the Appendix 1 Voting Summary; (b) commenter-set queries on rulemaking records where the correct answer is the final-rule's footnote enumeration; (c) institutional-composition queries on agency rosters where the correct answer is the published record at the relevant date.

**Fourth, the deployment-time mitigation is to treat statutory-quotation, figure-quotation, and institutional-record answers as high-risk outputs that should either (a) cite a verifiable paragraph of the regulator's own text or the U.S. Code, or (b) decline to commit.** Every failure mode in this audit would have been prevented by a retrieval-grounded answer that cited the relevant paragraph of the final rule, the NPRM, the U.S. Code, or the Federal Register index; every failure mode flowed from a generation behaviour that produced a confident answer by analogy with general knowledge rather than from the source text.

## How RLB Can Help

RegLeg is positioned to support labs working on the failure modes surfaced in this audit. Our research operates on the boundary where labs' enterprise customers are most exposed: technical regulatory documents where the model is asked to quote statutory text, reproduce regulator-issued figures, and characterise rulemaking-record fields. For labs, our findings supply ready-made eval scaffolding (the question types, the regulator-text anchors, the expected failure modes) that can be adapted into internal benchmark sets.

Where labs are interested, we are open to engagement on (a) targeted evaluation set development for specific regulator portfolios (CFTC, SEC, FCA, MAS, EU prudential authorities); (b) failure-mode taxonomy work on statutory-figure quotation, regulatory-history reproduction, and institutional-record reproduction; and (c) eval-design consultation on retrieval-grounded answer behaviour for authoritative technical documents. We can also support post-audit communication with affected enterprise customers, where the lab has decided to surface a known limitation rather than allow customer-side discovery.

Practitioners and enterprise teams using AI tools on CFTC and U.S. derivatives work can consult our published Hallucination Research for a free pre-flight check on AI-assisted regulatory research, identifying the question types and instrument areas where current models have demonstrably misstated the rules.


## Related concepts

- Regulation: [CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024](/okf/regulations/CPO-CTA-REGULATION-4-7-QEP-THRESHOLDS-2024.md)
- Regulator: [CFTC-US-001](/okf/bodies/CFTC-US-001.md)
- Methodology: [v2.3](/okf/methodology.md)