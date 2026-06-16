---
type: "AILabsWhitepaper"
title: "Structural Fabrication and Qualifier Erasure: AI Failure Modes on the 2025 OECD Merger Review Recommendation"
slug: "oecd-merger-review-recommendation-2025-ai-labs"
audience: "ai_labs"
regulation_slug: "OECD-MERGER-REVIEW-RECOMMENDATION-2025"
regulation_id: "328106"
body_id: "OECD-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "OECD"
methodology_version: "2.1"
substrate_version: 1
generated_at: "2026-06-07T23:25:58.509970+00:00"
published_at: "2026-06-07T23:25:58.509970+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/oecd/OECD-MERGER-REVIEW-RECOMMENDATION-2025/ai-labs/"
timestamp: "2026-06-16T07:45:50.612854+00:00"
---

# Structural Fabrication and Qualifier Erasure: AI Failure Modes on the 2025 OECD Merger Review Recommendation

- **Regulation.** [`OECD-MERGER-REVIEW-RECOMMENDATION-2025`](/okf/regulations/OECD-MERGER-REVIEW-RECOMMENDATION-2025.md) — Recommendation of the Council on Merger Review (2025 Revision)
- **Regulator.** [`OECD-INT-001`](/okf/bodies/OECD-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** 2.1
- **Generated.** 2026-06-07T23:25:58.509970+00:00

## Executive summary

Both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search independently fabricated a sixth operative section for the 2025 OECD Merger Review Recommendation (OECD/LEGAL/0333), which has five. On the same question about the failing firm defence, both models dropped the regulation's explicit 'inter alia' qualifier and presented an open-ended evidentiary standard as a closed exhaustive test. Claude Sonnet 4.6 with web search additionally elaborated a three-tier internal remedy ranking drawn from EU and US practice that does not appear in the OECD text, and collapsed a two-stage reporting cadence into a uniform interval while projecting specific future years. The cross-model convergence on two distinct failure shapes, structural schema fabrication and precision-qualifier erasure, points to a shared training-data gap on the 2025 revision rather than model-specific artefacts, and web search active on both configurations did not correct either failure.

## Full whitepaper

# Structural Fabrication and Qualifier Erasure: AI Failure Modes on the 2025 OECD Merger Review Recommendation


Both Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search independently fabricated a structural section of the 2025 OECD Merger Review Recommendation (OECD/LEGAL/0333) that does not exist in the instrument, each constructing a sixth operative section when the Recommendation has five. The convergence is exact: both models inserted "Monitoring and Review" or "Cross-Jurisdictional Co-operation" as a standalone section, drawing on merger-review convention and prior OECD instruments rather than the 2025 revision's actual architecture.

Beyond the structural fabrication, both models erased the Recommendation's explicit epistemic qualifier on the failing firm defence, converting an "inter alia" open-ended evidentiary standard into a closed, exhaustive three-condition test. Claude Sonnet 4.6 with web search produced two further failure patterns: elaborating a multi-tier internal remedy-ranking framework that appears nowhere in the instrument's text, and collapsing a two-interval reporting cadence (initial report within five years, then at least every ten years thereafter) into a uniform five-year cycle, projecting specific future years with no basis in the text.

The cross-model convergence on both the structural fabrication and the failing-firm-defence qualifier erasure is the signal of consequence: these are not stochastic errors but shared gaps in how the 2025 revision's text is represented across training. On an instrument that governs jurisdictional alignment across merger review globally, referenced by competition lawyers, M&A advisers, and regulatory economists advising on multi-jurisdiction transactions, confident fabrications about section structure, evidentiary standard exhaustiveness, and remedy hierarchy propagate directly into professional work product.

## When This Affects an AI Lab

Competition lawyers, M&A advisers, regulatory economists, and in-house counsel at multinational companies routinely ask models about the OECD Merger Review Recommendation when advising on multi-jurisdiction transaction clearance strategy. The 2025 revision is the operative version; practitioners distinguishing it from the 2005 predecessor are exactly the users whose queries surface the structural fabrication documented here. When a model confidently generates a six-section architecture for an instrument that has five, or presents a closed exhaustive standard where the text explicitly says "inter alia," the output functions as authoritative guidance, it has the format and register of a correct answer. Users with partial familiarity with the Recommendation are unlikely to detect the error before acting on it.

The downstream harms a lab should map are concrete: merger filings that mischaracterise the Recommendation's operative scope, advisory memoranda that cite a non-existent "Monitoring and Review" section as support, transaction counsel that presents the failing firm defence as a closed three-condition gate when the regulator's text leaves the evidentiary list open. Any of these constitutes a professional liability exposure for the user, and positions the lab's model as the source of a consequential error in a regulated, adversarial proceeding context. The remedy-hierarchy fabrication (an elaborated multi-tier ranking drawn from EU and US practice that is not in the OECD text) is particularly high-risk: remedy structuring is a late-stage, high-stakes moment in merger review, and divergence from the applicable instrument's actual hierarchy shapes negotiating positions with competition authorities.

The structural properties of this regulation make it a likely failure surface across models generally. The 2025 revision is recent: it superseded the 2005 version and the instrument's updated architecture is not extensively represented in pre-cutoff training data. The Recommendation's five operative sections do not map onto the section numbering conventions of the EU Merger Regulation, the US HSR framework, or prior OECD merger guidance, all of which models have seen extensively and from which they appear to reconstruct a plausible-but-wrong schema. The "inter alia" qualifier on the failing firm defence is a brief, easily-overlooked phrase whose erasure converts a flexible standard into a rigid one, precisely the kind of low-salience precision that standard evals miss and that regulatory practitioners depend on.

## Aggregate Impact

| Model | Configuration | Failure count | Dominant error pattern |
|---|---|---|---|
| Claude Opus 4.7 | Web search | 3 | Structural section fabrication; open standard converted to closed exhaustive test |
| Claude Sonnet 4.6 | Web search | 4 | Structural fabrication; cross-framework schema elaboration; numeric-interval collapse; qualifier erasure |

Claude Opus 4.7 with web search produced three failures, all sharing the same underlying shape: the model reconstructed plausible-sounding content from adjacent training signal rather than from the 2025 Recommendation's primary text. Two of the three findings concern the instrument's section structure, on separate questions, the model independently generated a six-section architecture (the Recommendation has five), each time inserting a "Monitoring and Review" or "Transnational Co-operation" section and attributing the missing content to a specific OECD legal instrument identifier that does not appear in the 2025 text. The third failure converts the failing firm defence's "inter alia" evidentiary list into a closed three-condition test, with the third condition subtly reframed from a competitive-harm counterfactual into an asset-exit inevitability gate, a meaningful legal distinction that the model erased. Web search did not correct any of these reconstructions; the model appears to have retrieved third-party commentary or prior-instrument descriptions rather than the 2025 primary text.

Claude Sonnet 4.6 with web search produced four failures across four distinct failure shapes. The structural fabrication matches Opus 4.7 exactly on the same question, a near-identical six-section reconstruction, independently reached. Beyond that, the model elaborated a three-tier internal ranking for structural remedies (upfront divestiture, buyer pool with trustee backstop, crown jewel packages) that maps onto EU and US merger remedy practice but does not appear in the OECD Recommendation's text, which specifies only a two-level preference. On the Competition Committee's reporting cadence, the model collapsed a two-stage interval (initial report within five years, then at minimum every ten years thereafter) into a uniform five-year cycle and arithmetically projected specific report years. And on the failing firm defence, it dropped the "inter alia" qualifier and presented the evidentiary list as closed and exhaustive, converging with Opus 4.7 on the same erasure.

The joint failure pattern across both configurations signals something specific about the 2025 revision's coverage in training. Failures cluster on two axes: the instrument's structural schema (where both models reconstruct from convention rather than text) and the precision qualifiers that distinguish the 2025 standard from prior-generation merger doctrine (where both models default to the harder, more familiar version of the rule). The cross-model convergence on the same structural fabrication and the same qualifier erasure, across configurations that differ in model size, post-training tuning, and retrieval behaviour, points to a shared training-data gap on the 2025 text rather than a model-specific artefact. Web search on both configurations failed to correct either failure, suggesting the retrieval layer is not surfacing the 2025 Recommendation's primary text at sufficient weight to override reconstruction.

## Findings


### Finding 1. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** How is the 2025 OECD Merger Review Recommendation (OECD/LEGAL/0333) structured, and which subject-matter areas were added in the 2025 revision relative to the superseded 2005 version?
- **AI's response:** "OPERATIVE CONTENT: (a) MERGER REVIEW FRAMEWORK ... (e) INTERNATIONAL CO-OPERATION, focused specifically on transnational mergers and remedy alignment, deliberately narrower than 2005 ... (f) MONITORING and review by the Competition Committee"
- **Regulator's text:** The Recommendation comprises five operative sections: Section I (maintain an effective merger review framework); Section II (apply effective merger notification and review procedures); Section III (apply sound merger analysis); Section IV (develop and apply a clear framework for remedies); Section V (conduct ex-post assessment).
- **Why the AI went wrong:** The model generated a six-section architecture for an instrument that has five, inserting "International Co-operation" and "Monitoring" as standalone operative sections. The 2025 Recommendation does not structure those topics as separate sections; the model appears to have reconstructed the document's architecture from merger-review convention and prior OECD instruments, both of which commonly present monitoring and cooperation as dedicated sections, rather than from the 2025 revision's actual text.
- **Cited source(s):**
  - _Regulator portal: https://www.oecd.org_

### Finding 5. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** What conditions must a merging party satisfy to invoke the failing firm defence under the 2025 OECD Merger Review Recommendation, and how demanding is the overall standard compared to established doctrine?
- **AI's response:** "THREE cumulative conditions ... (3) ABSENT-THE-MERGER COUNTERFACTUAL: ASSETS WOULD EXIT, without the merger, the target's productive assets would inevitably leave the market (i.e. the competitive constraint disappears regardless of the merger)."
- **Regulator's text:** Section III.11.b requires "inter alia, evidence that the business was likely to have exited and the existence of less anti-competitive alternative buyers or other options for reorganisation are not viable, and that the exit of the firm's assets would cause more harm to competition than the merger."
- **Why the AI went wrong:** Two compounding errors. First, the Recommendation's evidentiary standard is explicitly open-ended ("inter alia"), the model converted it into a closed, exhaustive three-condition test, stripping the qualifier that preserves regulatory flexibility. Second, the model reframed the third evidentiary element: the Recommendation requires a showing that asset exit would cause more competitive harm than the merger, a counterfactual competitive-harm assessment, whereas the model characterised it as a gate requiring proof that assets would "inevitably leave the market," shifting the legal burden in a way the text does not support.
- **Cited source(s):**
  - https://one.oecd.org/document/DAF/COMP(2009)38/en/pdf, Pretextual
  - https://www.oecd.org/en/publications/failing-firm-defence_1712635f-en.html, Pretextual
  - _Regulator portal: https://www.oecd.org_

### Finding 6. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** What do the primary operative sections of the 2025 OECD Merger Review Recommendation (OECD/LEGAL/0333) address, and what topics were deliberately separated into other OECD instruments rather than included in this Recommendation?
- **AI's response:** "(v) TRANSNATIONAL CO-OPERATION specifically on merger reviews and remedy design, deliberately narrower than 2005 because broader cooperation is now governed by OECD/LEGAL/0408 (2014) ... (vi) MONITORING by the OECD Competition Committee with periodic reporting to Council."
- **Regulator's text:** The Recommendation's five operative sections are: Section I (maintain an effective merger review framework); Section II (apply effective merger notification and review procedures); Section III (apply sound merger analysis); Section IV (develop and apply a clear remedies framework); Section V (conduct ex-post assessment of merger decisions and/or remedies).
- **Why the AI went wrong:** On a second, differently-framed question about the same instrument, the model again generated a six-section structure and this time fabricated a specific cross-reference, attributing broader cooperation governance to OECD/LEGAL/0408 (2014), a legal instrument identifier that does not appear in the 2025 Recommendation's text. The response constructed a coherent-sounding inter-instrument division of scope that is consistent with how OECD governance generally works but is not what the 2025 Recommendation states. The repeated structural fabrication across independently posed questions, with web search active, confirms the reconstruction is drawn from training rather than corrected by retrieval.
- **Cited source(s):**
  - _Regulator portal: https://www.oecd.org_

### Finding 1. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** How is the 2025 OECD Merger Review Recommendation (OECD/LEGAL/0333) structured, what does each operative section address, and which subject-matter areas did the 2025 revision add that were absent from the 2005 version?
- **AI's response:** "structured around six broad operative areas: 1. Merger Review Framework... 2. Notification and Review Procedures... 3. Substantive Merger Analysis... 4. Merger Remedies... 5. Cross-Jurisdictional Co-operation... 6. Monitoring and Review."
- **Regulator's text:** The Recommendation has five operative sections: Section I (maintain an effective merger review framework); Section II (apply effective merger notification and review procedures); Section III (apply sound merger analysis); Section IV (develop and apply a clear framework for remedies); Section V (conduct ex-post assessment of merger decisions and/or remedies).
- **Why the AI went wrong:** The model generated an identical structural error to Claude Opus 4.7 with web search on the same question, a six-section architecture with "Cross-Jurisdictional Co-operation" and "Monitoring and Review" inserted as standalone operative areas. The near-exact convergence across two configurations that differ substantially in size and post-training tuning, both with web search active, points to a shared training-data gap on the 2025 revision's structure rather than a configuration-specific artefact. The retrieval layer did not surface or weight the primary text sufficiently to correct the reconstruction.
- **Cited source(s):**
  - _Regulator portal: https://www.oecd.org_

### Finding 2. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** What does Section IV.3 of the 2025 OECD Merger Review Recommendation establish as the hierarchy for acceptable remedies in merger proceedings, and what is the priority ordering within the structural remedies tier?
- **AI's response:** "Within structural remedies, there is a further internal preference ordering:, Upfront / 'fix-it-first' divestitures...rank highest...,  Divestiture commitments with an approved buyer pool and a trustee mandate as backstop rank second., 'Crown jewel' or ring-fenced asset packages...rank third."
- **Regulator's text:** Section IV.3 states: "Prioritise structural remedies over behavioural ones and, for structural remedies, prioritise the divestiture of standalone businesses."
- **Why the AI went wrong:** Section IV.3 establishes a two-level preference: structural over behavioural, and standalone-business divestiture as the preferred structural form. The model elaborated this into a three-tier internal ranking, upfront/fix-it-first divestiture, buyer pool with trustee backstop, crown jewel packages, that maps onto common EU and US merger remedy practice but does not appear in the 2025 OECD Recommendation's text. The model substituted a practitioner-familiar remedy taxonomy drawn from other jurisdictions' frameworks for the Recommendation's simpler, less-prescriptive hierarchy, and presented the elaborated ranking as the OECD standard.
- **Cited source(s):**
  - _Regulator portal: https://www.oecd.org_

### Finding 4. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** What does Section VIII.c of the 2025 OECD Merger Review Recommendation require of the Competition Committee regarding Council reporting, including the specific timeline and whether the reporting structure involves a single uniform interval or multiple distinct intervals?
- **AI's response:** "Fixed interval: 5 years (next report: 2030; following report: 2035)"
- **Regulator's text:** Section VIII.c requires the Competition Committee to "report to Council on the implementation, dissemination and continued relevance of this Recommendation no later than five years following its revision and at least every ten years thereafter."
- **Why the AI went wrong:** Section VIII.c establishes a two-stage interval structure: an initial report within five years of the 2025 revision, then reports at minimum every ten years thereafter. The model collapsed this into a uniform five-year cycle, applying the initial, tighter interval as the recurring interval, and then arithmetically projected specific report years (2030, 2035) that appear nowhere in the text. The error erases a meaningful structural distinction: the first interval is an expedited post-revision check; the recurring interval is a longer-cadence review. The model produced a response with the format of a precise, text-grounded answer while substituting a simpler reconstruction for the actual two-interval structure.
- **Cited source(s):**
  - _Regulator portal: https://www.oecd.org_

### Finding 5. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** Under Section III.11.b of the 2025 OECD Merger Review Recommendation, what conditions must a merging party satisfy to successfully invoke the failing firm defence before OECD member jurisdiction competition authorities, and is the enumerated evidence list exhaustive?
- **AI's response:** "Under the OECD standard, a failing firm defence requires the merging parties to demonstrate all three of the following conditions... All three conditions must be satisfied simultaneously. Failure on any one condition is fatal to the defence."
- **Regulator's text:** Section III.11.b requires "inter alia, evidence that the business was likely to have exited and the existence of less anti-competitive alternative buyers or other options for reorganisation are not viable, and that the exit of the firm's assets would cause more harm to competition than the merger."
- **Why the AI went wrong:** The Recommendation's failing firm defence standard is explicitly non-exhaustive, "inter alia" preserves regulatory flexibility for competition authorities to require additional evidence. The model dropped the qualifier and presented the evidentiary list as a closed, exhaustive three-condition test with an expressly fatal consequence for failure on any single condition. This convergence with Claude Opus 4.7 with web search on the same erasure, across two different configurations, both with web search active, indicates that the 2025 Recommendation's exact phrasing of this standard is not adequately represented in training for either model, and that retrieval did not surface the primary text to correct it.
- **Cited source(s):**
  - https://www.oecd.org/en/publications/failing-firm-defence_1712635f-en.html, Pretextual
  - _Regulator portal: https://www.oecd.org_

## What Your Team Should Do

### Implications for your training data

The structural fabrication, both models independently generating a six-section architecture for a five-section instrument, points to a gap specific to the 2025 revision. The 2025 Recommendation updated the 2005 predecessor; models appear to hold a representation of the prior instrument's structure (or of merger-review convention generally) that is not overridden by the 2025 text. The training corpus for this regulator's primary outputs likely lacks sufficient coverage of the 2025 revision at the verbatim-text level, leaving the models to reconstruct from adjacent signal. For this regulator and for OECD soft-law instruments generally, corpus ingestion should prioritise the primary legal text in its current revision, not commentary, secondary summaries, or prior-instrument versions which may be more heavily represented.

The "inter alia" erasure on the failing firm defence is a precision-qualifier failure that training data alone may not fix, but corpus composition shapes it. Where the 2025 revision's verbatim text is sparse in training, models default to a harder, more rule-like version of the standard, which is the more commonly articulated form in practitioner commentary and comparative-law literature. Pairing the regulator's verbatim text with explicitly flagged contrast cases (open-ended standard vs. closed exhaustive standard) as a structured training signal would provide the model with a stable representation of where this Recommendation diverges from more prescriptive frameworks. The remedy-hierarchy over-specification (elaborating a three-tier ranking from a two-level text preference) follows the same pattern: the elaborated framework is drawn from EU and US remedy doctrine, which is heavily represented in training; the OECD's simpler formulation needs to be weighted as the authoritative source for OECD-context queries.

### Implications for your post-training logic

Two calibration targets are directly implicated. First, when the model commits to an instrument's section count or structural schema, it should register uncertainty where its representation of the primary text is thin, particularly for instruments revised within the last 24 months. A self-check pass that surfaces "my training coverage of this specific revision may be limited" before committing to a structural description would catch the class of fabrication documented here. The web search retrieval layer is not currently providing this correction: both configurations with web search active produced the structural fabrication, suggesting retrieved content consisted of commentary or prior-instrument material rather than the 2025 primary text, and the model did not flag the retrieval gap.

Second, where a legal standard's text contains an explicit exhaustiveness qualifier ("inter alia", "including but not limited to", "among other things"), the model's response should preserve that qualifier rather than convert the standard into a closed rule. Post-training calibration on precision-qualifier preservation, specifically in regulatory and legal text contexts, would address both the failing firm defence erasure and the reporting-interval collapse (where "no later than five years... and at least every ten years thereafter" was converted into a single uniform interval). These are not retrieval failures; they are characterisation failures that occur when the model has a partial representation of the text and fills in a simpler, more familiar version.

### Specific eval / red-team probes RegLeg suggests

- Section-count verification probes for recently-revised OECD and other international soft-law instruments: ask for the number and titles of operative sections, then compare against the primary text.
- Exhaustiveness-qualifier preservation probes: present a regulatory standard that uses "inter alia" or equivalent, ask whether the evidentiary list is exhaustive, and check whether the model preserves or erases the qualifier.
- Cross-framework contamination probes on remedy doctrine: ask for the remedy preference hierarchy under a specific instrument, then check whether the model's answer reflects that instrument or a more familiar jurisdiction's framework.
- Multi-interval reporting cadence probes: ask for the specific reporting intervals where a regulation uses a two-stage cadence (initial + recurring), and check whether the model distinguishes the two intervals or collapses them.
- Fabricated cross-reference probes: ask what topics are "delegated to other OECD instruments" under a given Recommendation, then verify whether any instrument identifiers cited appear in the primary text.

## How RLB Can Partner With Your Lab

We document nuanced, regulation-specific failure modes across model versions and configurations, the kind that surface only when testing against primary regulatory text rather than widely-reproduced commentary. The failure shapes documented in this paper represent categories we track systematically across an expanding regulatory portfolio: structural schema reconstruction from prior-instrument conventions on recently-revised soft-law instruments; precision-qualifier erasure converting open-ended legal standards into closed rules; cross-framework schema elaboration where a model substitutes a more familiar jurisdiction's doctrine for the applicable instrument's simpler standard; multi-interval numeric collapse where a two-stage cadence is flattened to a single recurring interval; and fabricated cross-reference generation where instrument identifiers are produced without basis in the primary text. Each of these is a failure shape the lab's standard internal evals are unlikely to surface at the granularity needed to act on.

Where your team wants to close gaps, we can provide: correction-pair generation derived directly from the regulator's authoritative text, wrong response paired with the ground-truth excerpt and the precise point of divergence, formatted for ingestion into your training pipeline. We can run embedded comparative evaluations against a defined regulatory portfolio on a quarterly cadence, tracking regression on previously documented failure modes across model versions and flagging where a capability release degrades precision-qualifier preservation or structural schema fidelity. For capability launches that touch regulated domains, financial services, cross-border transaction review, payments infrastructure, competition law, we can run pre-release evaluation cycles scoped to the regulator portfolio relevant to your deployment surface and deliver a failure-mode report before the release reaches customers. And for specific regulators your team is prioritising, we can run targeted red-team consultations focused on the failure surfaces most likely to generate consequential errors for your users.

To scope a partnership focused on refining your models against these failure modes, reach out at reglegbrief.com.


## Related concepts

- Regulation: [OECD-MERGER-REVIEW-RECOMMENDATION-2025](/okf/regulations/OECD-MERGER-REVIEW-RECOMMENDATION-2025.md)
- Regulator: [OECD-INT-001](/okf/bodies/OECD-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)