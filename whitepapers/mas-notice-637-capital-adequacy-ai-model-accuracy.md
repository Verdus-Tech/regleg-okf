---
type: "AILabsWhitepaper"
title: "MAS Notice 637 Capital Adequacy: AI Model Accuracy Evaluation"
slug: "mas-notice-637-capital-adequacy-ai-model-accuracy"
audience: "ai_labs"
regulation_slug: "NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025"
regulation_id: "2055"
body_id: "MAS-SG-001"
jurisdiction_code: "SG"
j_level: "J3"
regulator_short_code: "MAS"
methodology_version: "2.3"
substrate_version: 1
generated_at: "2026-06-10T23:35:14.568926+00:00"
published_at: "2026-05-28T10:23:18.799941+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j3/sg/mas/NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025/ai-labs/"
timestamp: "2026-06-16T00:00:00+00:00"
---

# MAS Notice 637 Capital Adequacy: AI Model Accuracy Evaluation

- **Regulation.** [`NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025`](/okf/regulations/NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025.md) — MAS Notice 637 (Amendment) 2025, Risk Based Capital Adequacy Requirements for Banks Incorporated in Singapore
- **Regulator.** [`MAS-SG-001`](/okf/bodies/MAS-SG-001.md)
- **Audience.** ai_labs
- **Methodology.** 2.3
- **Generated.** 2026-06-10T23:35:14.568926+00:00

## Executive summary

This audit presents findings from RegLeg's evaluation of AI model responses to questions about MAS Notice 637, the Monetary Authority of Singapore's risk-based capital adequacy framework for banks, covering both the consolidated notice and its 2025 amendment. Claude Opus 4.7 in a web-search-enabled configuration was tested across the question set. Across two confirmed findings, the model produced confident, specific answers that MAS's own published text directly contradicts: a fabricated parallel notice ('Notice FHC-N637') for financial holding companies, and a wrong characterisation of MAS's yellow-highlight editorial convention in the 2025 amendment PDF. Both failures are inference drift: the model committed to a specific answer in cases where the correct posture was to surface the actual passage of Notice 637 or to flag that the text resolves the question differently. For labs fielding these models in Singapore enterprise and regulatory contexts, this pattern represents a material gap in how the models handle instrument-identification queries and editorial-convention interpretation under partial information retrieval.

## Full whitepaper

# MAS Notice 637 Capital Adequacy: AI Model Accuracy Evaluation

## Executive Summary

This audit presents findings from RegLeg's evaluation of AI model responses to questions about MAS Notice 637, the Monetary Authority of Singapore's risk-based capital adequacy framework for banks, covering both the consolidated notice and its 2025 amendment. Claude Opus 4.7 in a web-search-enabled configuration was tested across the question set. Across two confirmed findings, the model produced confident, specific answers that MAS's own published text directly contradicts: a fabricated parallel notice ('Notice FHC-N637') for financial holding companies, and a wrong characterisation of MAS's yellow-highlight editorial convention in the 2025 amendment PDF. Both failures are inference drift: the model committed to a specific answer in cases where the correct posture was to surface the actual passage of Notice 637 or to flag that the text resolves the question differently. For labs fielding these models in Singapore enterprise and regulatory contexts, this pattern represents a material gap in how the models handle instrument-identification queries and editorial-convention interpretation under partial information retrieval.

## When This Affects an AI Lab

MAS Notice 637 sits at the operational core of bank capital management in Singapore, one of the world's principal financial centres. Users asking AI models about this notice include compliance officers at Singapore-licensed banks, in-house and external lawyers advising on capital instrument eligibility, fintech and regtech builders embedding regulatory logic into product flows, treasury teams structuring capital issuance, accountants preparing capital adequacy disclosures, public auditors performing statutory verification of capital ratios, risk functions running capital adequacy stress testing, and company secretarial teams preparing board reporting on prudential compliance. Any model deployed in an assistant, copilot, or document-query capacity in these contexts will routinely receive the question types tested in this audit: which MAS instrument applies to a particular entity in a banking group, what does a paragraph of the consolidated notice mean, and how does an amendment change the consolidated text.

The downstream harms are concrete. A compliance officer who acts on a fabricated parallel notice when structuring a group-perimeter assessment produces a record that misstates the regulatory architecture. A lawyer who reads the AI's wrong characterisation of yellow highlighting as a reader-attention signal on live text treats editorial annotations as operative regulatory obligations, with direct effect on legal opinions and on advice transmitted to compliance and reporting functions. For the lab, confident wrong outputs on authoritative regulatory text are the misuse-claim exposure that arises when enterprise customers act on model outputs in high-stakes contexts. Regulatory and financial-services use cases are among the fastest-growing deployment verticals for frontier models; the failure surface here is large and growing.

## Aggregate impact

The two findings in this audit identify a specific generation pattern that practitioners and labs should both treat as material on MAS Notice 637 questions. The model commits, with no hedging, to a fabricated regulatory instrument on a scope-perimeter question where the source notice itself resolves the issue through a scope carve-out (paragraph 11.2.2 of Notice 637), and the model imposes a general drafting convention onto a regulator-specific editorial annotation device that the regulator's own text explains (paragraph 3(c) of the 2025 amendment). In both cases the model had access to the actual MAS published text via web search; in both cases the model produced a confident answer that the published text directly contradicts.

Two structural risk drivers compound. First, the model is willing to construct parallel-instrument answers when the regulator has instead used scope rules within an existing notice. This points to a generation behaviour on instrument-existence queries where the model synthesises a plausible-looking instrument by analogy with the known notice rather than producing a calibrated 'not found' or 'scope-defined' response. Second, the model is willing to characterise regulator-specific editorial conventions by mapping them onto general drafting practice rather than reading the regulator's own statement of the convention. Both behaviours are silent in the deliverable; neither output signals to the user that the underlying claim has no basis in MAS's published text.

For Singapore enterprise deployments, these failure modes will recur on every banking-prudential notice that (a) defines its scope by reference to other instruments rather than through stand-alone separate notices, and (b) uses regulator-specific editorial conventions in tracked-change amendment PDFs. Both characteristics are common in MAS publications and in comparable banking regulators.

## Per-finding analysis

### Finding 1 . Fabricated 'Notice FHC-N637' for financial holding companies

**Citation:** RLB-H-SG-MAS-NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025-Q010-Opus47

This finding identifies an inference drift failure in instrument-existence handling: when asked which MAS notice applies to financial holding companies incorporated in Singapore, the model fabricated a specific instrument designation, 'Notice FHC-N637 (Risk Based Capital Adequacy Requirements for Financial Holding Companies)', framed as a parallel notice issued under the Financial Holding Companies Act. MAS Notice 637 itself addresses the FHC scope question in paragraph 11.2.2 through a scope carve-out: a Reporting Bank that is the subsidiary of a financial holding company subject to requirements similar to Part VII need not duplicate Part VII compliance. The model had access to the source notice via web search, and the source text resolves the question. The gap implicates the generation layer's handling of instrument-existence queries in cases where the correct answer is a scope rule rather than a parallel instrument: the model synthesised a plausible-looking instrument by analogy with the known parent notice. Targeted eval coverage for regulatory-instrument-existence queries on entities defined through scope carve-outs would surface this failure mode systematically. Recommended probes: instrument-existence queries on FHC-equivalent perimeter entities across multiple regulator portfolios; reading-rule queries that explicitly cite a scope paragraph as the answer anchor; retrieval-grounded queries that require pulling the scope paragraph before answering an instrument-naming question.

### Finding 2 . Misrepresented yellow-highlight meaning in MAS amendment PDFs

**Citation:** RLB-H-SG-MAS-NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025-Q012-Opus47

This finding identifies an inference drift failure in regulator-specific editorial-convention handling: when asked what yellow-highlighted passages signify in MAS Notice 637 (Amendment) 2025, the model characterised the highlighting as a general drafting or visual aid drawing reader attention to defined terms, cross-references, or items requiring particular attention in review. Paragraph 3(c) of the amendment is explicit on the convention: yellow-highlighted text marks annotations describing changes, and will not appear in the published untracked version of the Notice. The model's characterisation reflects generation from training knowledge about general drafting conventions rather than retrieval of the amendment's own reading-convention statement. The gap implicates the retrieval and generation layers' handling of regulator-specific editorial conventions: the model should either retrieve the convention paragraph of the source amendment or decline to characterise. Recommended eval probes: regulator-specific formatting and convention queries on tracked-change amendment PDFs across multiple regulator portfolios; reading-rule queries on instruments that include their own statement of convention; retrieval-grounded queries that require pulling the reading-convention paragraph before responding to a formatting question. This is a high-value eval surface because regulator-specific conventions appear across the prudential, securities, and financial-conduct regulatory portfolios; any model with broad enterprise-regulatory exposure will encounter these queries at volume.

## What Your Team Should Do

The targeted evaluation work for these failure modes should focus on three areas.

First, expand evaluation coverage of regulatory-instrument-existence queries where the correct answer is a scope rule within an existing instrument rather than a stand-alone parallel notice. The model in this audit fabricated 'Notice FHC-N637' as the parallel instrument for financial holding companies, where Notice 637 paragraph 11.2.2 itself resolves the FHC scope question. Eval probes should include (a) instrument-existence queries on entities defined by scope carve-outs in existing notices, (b) instrument-naming queries where the correct response is 'no separate instrument; the scope rule sits in [paragraph] of [notice]', and (c) instrument-architecture queries on regulatory frameworks that handle entity perimeter through scope rules rather than parallel instruments.

Second, expand evaluation coverage of regulator-specific editorial conventions on tracked-change amendment PDFs. The model in this audit characterised MAS's yellow-highlight convention as a general-purpose reader-attention signal on live text, where the amendment's paragraph 3(c) explicitly states it marks annotations that will not appear in the published untracked version. Eval probes should include (a) regulator-specific formatting and convention queries where general drafting practice diverges from the regulator's own statement, (b) reading-rule queries on amendment instruments that include their own statement of convention, and (c) retrieval-grounded queries that require pulling the reading-convention paragraph before answering a formatting question.

Third, the deployment-time mitigation is to treat instrument-identification answers and amendment-convention answers as high-risk outputs that should either (a) cite a verifiable paragraph of the regulator's own text, or (b) decline to commit. Both failure modes in this audit would have been prevented by a retrieval-grounded answer that cited the relevant paragraph of MAS Notice 637 or the 2025 amendment; both failure modes flowed from a generation behaviour that produced a confident answer by analogy with general knowledge rather than from the source text.

## How RLB Can Help

RegLeg is positioned to support labs working on the failure modes surfaced in this audit. Our research operates on the boundary where labs' enterprise customers are most exposed: technical regulatory documents where the model is asked to identify instruments, interpret editorial conventions, and characterise specific regulator text. For labs, our findings supply ready-made eval scaffolding (the question types, the regulator-text anchors, the expected failure modes) that can be adapted into internal benchmark sets.

Where labs are interested, we are open to engagement on (a) targeted evaluation set development for specific regulator portfolios (MAS, SEC, CFTC, FCA, EU prudential authorities), (b) failure-mode taxonomy work on regulatory-instrument identification and editorial-convention reading, and (c) eval-design consultation on retrieval-grounded answer behaviour for authoritative technical documents. We can also support post-audit communication with affected enterprise customers, where the lab has decided to surface a known limitation rather than allow customer-side discovery.

Practitioners and enterprise teams using AI tools on Singapore banking work can consult our published Hallucination Research for a free pre-flight check on AI-assisted regulatory research, identifying the question types and instrument areas where current models have demonstrably mis-stated the rules.


## Related concepts

- Regulation: [NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025](/okf/regulations/NOTICE-637-CAPITAL-ADEQUACY-BANKS-2025.md)
- Regulator: [MAS-SG-001](/okf/bodies/MAS-SG-001.md)
- Methodology: [v2.3](/okf/methodology.md)