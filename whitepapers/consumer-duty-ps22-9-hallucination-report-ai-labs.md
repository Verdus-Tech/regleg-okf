---
type: "AILabsWhitepaper"
title: "Consumer Duty Hallucination Report: frontier AI models"
slug: "consumer-duty-ps22-9-hallucination-report-ai-labs"
audience: "ai_labs"
regulation_slug: "CONSUMER-DUTY-PS22-9"
regulation_id: "320339"
body_id: "FCA-GB-001"
jurisdiction_code: "GB"
j_level: "J3"
regulator_short_code: "FCA"
methodology_version: "2.3"
substrate_version: 1
generated_at: "2026-06-11T01:42:44.211287+00:00"
published_at: "2026-06-07T08:31:34.320675+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j3/gb/fca/CONSUMER-DUTY-PS22-9/ai-labs/"
timestamp: "2026-06-16T07:45:45.421535+00:00"
---

# Consumer Duty Hallucination Report: frontier AI models

- **Regulation.** [`CONSUMER-DUTY-PS22-9`](/okf/regulations/CONSUMER-DUTY-PS22-9.md) — Consumer Duty (PS22/9 + PRIN 2A)
- **Regulator.** [`FCA-GB-001`](/okf/bodies/FCA-GB-001.md)
- **Audience.** ai_labs
- **Methodology.** 2.3
- **Generated.** 2026-06-11T01:42:44.211287+00:00

## Executive summary

This paper presents findings from a structured evaluation of two frontier AI models, Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search, against the Financial Conduct Authority's Consumer Duty rules, as set out in PS22/9 and PRIN 2A. Across fifteen findings, both models produced responses containing factual errors, omissions, and unsupported additions relative to the FCA's published regulatory text. The dominant error pattern is confident elaboration beyond what the regulator's text permits: models added conditions, caveats, and procedural requirements that are not present in the FCA's rules, while in other cases declining to provide information that the regulator has published clearly. Every cited source across both models was independently assessed and found to be either non-authoritative or presented in a context that did not support the claim it was used to justify. These results are a signal that current models, even with live web retrieval, show systematic weaknesses on regulatory content characterised by precise defined terms, recent amendments, and technical cross-references.

## Full whitepaper

# Consumer Duty Hallucination Report: Claude Opus 4.7 and Claude Sonnet 4.6


This paper presents findings from a structured evaluation of two frontier AI models, Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search, against the Financial Conduct Authority's Consumer Duty rules, as set out in PS22/9 and PRIN 2A. Across fifteen findings, both models produced responses containing factual errors, omissions, and unsupported additions relative to the FCA's published regulatory text. The dominant error pattern is confident elaboration beyond what the regulator's text permits: models added conditions, caveats, and procedural requirements that are not present in the FCA's rules, while in other cases declining to provide information that the regulator has published clearly. Every cited source across both models was independently assessed and found to be either non-authoritative or presented in a context that did not support the claim it was used to justify. These results are a signal that current models, even with live web retrieval, show systematic weaknesses on regulatory content characterised by precise defined terms, recent amendments, and technical cross-references.

## When This Affects an AI Lab

The FCA's Consumer Duty framework is one of the most operationally significant pieces of UK financial regulation for firms serving retail customers. Legal, compliance, and financial-services teams at banks, insurers, investment platforms, fintechs, and regtechs routinely use frontier AI models to research their obligations under Consumer Duty, asking questions about scope, defined terms, the four outcomes framework, fair value requirements, and the boundary between binding rules and non-binding guidance. Any model deployed in those contexts, whether through a direct API integration, a co-pilot product, or an enterprise assistant, will be asked exactly the kinds of questions tested in this evaluation.

The downstream harms from errors in this domain are concrete. A compliance officer who acts on a model's incorrect description of the "retail customer" threshold for charities, or who takes a model's fabricated procedural requirement as authoritative, may build a compliance programme around a rule that does not exist in the FCA's text. Firms that rely on AI-assisted regulatory summaries for Consumer Duty implementation face regulatory risk if those summaries import errors silently; the FCA has stated explicitly that firms cannot outsource their regulatory obligations. For a lab, the exposure extends further: if customers act on confidently-presented incorrect outputs and then face regulatory action or financial loss, the lab's documentation of model limitations becomes material. Errors that embed plausibly-presented fabrications, rather than obvious failures, are the ones that reach this downstream harm threshold.

This regulation is a structurally demanding surface for models. Consumer Duty spans a primary Principle (Principle 12), a detailed PRIN 2A rulebook chapter with multiple sub-chapters containing binding rules ("R"), guidance ("G"), and evidential provisions ("E"), and a body of finalised guidance (FG22/5) that supplements but does not override the rules. Defined terms such as "retail customer", "foreseeable harm", and "consumer understanding" have specific regulatory meanings that differ from ordinary language usage. The framework was finalised in July 2022 with implementation staggered across 2023–2024, meaning models trained before those dates, or with patchy post-2022 coverage, will fill gaps with plausible-sounding inference. The combination of technical defined terms, recent layered amendments, and a distinction between binding rules and guidance that is marked typographically in the Handbook but invisible in plain prose makes this regulation a high-probability hallucination surface across model generations.

## Aggregate Impact

**Per-model summary:**

| Model | Configuration | Findings | Dominant failure pattern |
|---|---|---|---|
| Claude Opus 4.7 | With web search | 8 | Confident elaboration beyond the regulator's text, adding conditions, procedural steps, and qualifications that appear reasonable but are not present in the FCA's published rules. Five of eight findings involve fabricated factual content. |
| Claude Sonnet 4.6 | With web search | 7 | A mix of over-elaboration and under-disclosure: in some cases the model added unsupported requirements; in others it declined to provide information that the regulator has published clearly, citing an inability to find a verified source. Two findings involve evasion responses where the published answer was accessible. |

Claude Opus 4.7 with web search produced a consistent pattern of response augmentation: when the FCA's text provides a clean, unqualified rule, the model tended to reconstruct a more elaborate or hedged version, adding conditions and caveats that would seem plausible to a general reader but that the regulator's text does not support. This is most visible in findings relating to the foreseeable harm provision, the scope of the fair value assessment methodology, and the group insurance exclusion. The model appears to be generating regulatory-sounding completions from inference rather than grounding its responses in retrieved text, even when web retrieval was active. Citation behaviour reinforces this: sources cited were consistently non-authoritative or used out of context, suggesting the model is selecting plausible-seeming URLs independently of whether those sources contain the claimed content.

Claude Sonnet 4.6 with web search shows a different surface: it is more likely to produce evasion responses on recent regulatory developments, particularly FCA feedback statements and withdrawal notices from 2025, while also generating unsupported augmentations on definitional questions. The contrast between the two models is instructive for an alignment team: Opus 4.7 with web search is more willing to commit to a specific (often wrong) answer; Sonnet 4.6 with web search is more likely to hedge or decline when recent content is involved, but still produces augmented responses on older settled provisions. Both models shared a structural weakness in citation generation, neither model's web retrieval step produced sources that independently supported the response content. This suggests that the web-search-augmented configuration does not reliably anchor content generation to retrieved documents: the retrieval and content generation steps appear to be operating with some independence, with fabricated or pretextual citations appended to responses that were already constructed from training inference.

## Findings


### Finding 3. Claude Opus 4.7 with web search

**Question (paraphrased to protect IP):**
Does the Consumer Duty require firms to prevent all foreseeable harm to retail customers? What is the position where a customer understands and accepts a risk?

**AI's response:**
> "Where a retail customer understands the risk and the firm has acted in good faith, supported understanding, avoided foreseeable harm caused by its own conduct, and otherwise complied with the Duty, the customer accepting a risk does not breach the Duty."

**Regulator's text:**
Where a firm reasonably believes a retail customer understands and accepts such risks, it will not breach the rule if it fails to prevent them.

**Why the AI went wrong:**
The FCA's rule sets a single condition, the firm's reasonable belief that the customer understands and accepts the risk. The model reconstructed a multi-part compliance test (good faith, supported understanding, avoided firm-caused harm, plus general Duty compliance) that does not appear in the regulator's text. This expansion substitutes an inference-derived elaboration for the published rule, removing the qualifier "reasonably believes" and replacing it with a more demanding composite standard.

**Cited source(s):**
- https://handbook.fca.org.uk/handbook/PRIN/2A/2.html, Pretextual
- https://www.fca.org.uk/publication/finalised-guidance/fg22-5.pdf, Pretextual
- _Regulator portal (if any cited link is dud): https://www.fca.org.uk_

### Finding 5. Claude Opus 4.7 with web search

**Question (paraphrased to protect IP):**
Does the Consumer Duty apply to micro-enterprises or small charities? Are they 'retail customers' under PRIN 2A?

**AI's response:**
> "charities with annual income under £1 million"

**Regulator's text:**
Retail customer includes consumers (individual persons), micro-enterprises, and charities with annual turnover less than £1 million. Definition varies by sourcebook.

**Why the AI went wrong:**
The FCA's definition uses "annual turnover" as the threshold measure for charities. The model substituted "annual income", a different financial metric that would produce different results in practice for charities that have income sources distinct from trading turnover. This is a precise definitional substitution: the word swap is small but changes which charities fall within scope, and reflects the model applying a common synonym rather than retrieving the regulator's exact defined term.

**Cited source(s):**
- https://handbook.fca.org.uk/handbook/PRIN/2A/1.html, Pretextual
- https://www.fca.org.uk/publication/finalised-guidance/fg22-5.pdf, Pretextual
- _Regulator portal (if any cited link is dud): https://www.fca.org.uk_

### Finding 13. Claude Opus 4.7 with web search

**Question (paraphrased to protect IP):**
Has the FCA withdrawn any pre-Consumer Duty Dear CEO letters following implementation, and if so how many?

**AI's response:**
> "Around 90+ Dear CEO/portfolio letters were retired in April 2025, with a further tranche of multi-firm and thematic reports retired in August 2025."

**Regulator's text:**
FS25/2 (March 2025): FCA removed more than 90 pre-Consumer Duty Dear CEO letters and cleared over 100 old multi-firm reports.

**Why the AI went wrong:**
The FCA's feedback statement FS25/2 was published in March 2025 and announced the withdrawal of both categories simultaneously. The model re-dated the Dear CEO letter withdrawal to April 2025 and fabricated a separate August 2025 tranche for multi-firm reports that does not exist in the regulator's record. The model appears to have split a single announced action into two sequential events, adding invented dates for each.

**Cited source(s):**
- https://www.fca.org.uk/news/news-stories/fca-simplifies-supervisory-letters, Pretextual
- _Regulator portal (if any cited link is dud): https://www.fca.org.uk_

### Finding 17. Claude Opus 4.7 with web search

**Question (paraphrased to protect IP):**
Were there significant differences between the Consumer Duty as proposed in CP21/36 and the final rules in PS22/9? What specific provisions were changed?

**AI's response:**
> "PS22/9 made several changes from the CP21/36 draft... Key changes/clarifications included: (i) split implementation timeline... (ii) clarifications on scope/distribution chains... (iii) refinement of the foreseeable harm cross-cutting rule wording... (vi) confirmation that a Private Right of Action would NOT be introduced."

**Regulator's text:**
The specific differences between CP21/36 and PS22/9 were not independently verifiable from retrieved sources for this evaluation.

**Why the AI went wrong:**
The model produced a numbered list of specific changes between the consultation paper and the final policy statement without access to a verified source that documents those changes. Some items may reflect general knowledge of the Consumer Duty policy development process, but the model presented them as a reliable enumerated account without acknowledging that this information was not retrieved from a source. The gap between confident presentation and actual source availability is the substantive failure.

**Cited source(s):**
- https://www.fca.org.uk/publication/consultation/cp21-36.pdf, Pretextual
- _Regulator portal (if any cited link is dud): https://www.fca.org.uk_

### Finding 5. Claude Sonnet 4.6 with web search

**Question (paraphrased to protect IP):**
Does the Consumer Duty apply to micro-enterprises and small charities? At what annual turnover threshold do charities qualify as 'retail customers' under PRIN 2A?

**AI's response:**
> "micro-enterprises and small charities are explicitly captured within the definition of 'retail customer'... Larger small businesses that are neither micro-enterprises nor small charities in those categories would generally not be 'retail customers'"

**Regulator's text:**
Retail customer includes consumers (individual persons), micro-enterprises, and charities with annual turnover less than £1 million. Definition varies by sourcebook.

**Why the AI went wrong:**
The model confirmed that micro-enterprises and small charities are within scope, which is correct, but it omitted the specific £1 million annual turnover threshold for charities that the FCA's definition requires. The threshold is the operative detail for any compliance team assessing whether a particular charity counterparty falls within scope. Confirming category membership without providing the defined numeric criterion leaves the reader unable to apply the rule.

**Cited source(s):**
- https://handbook.fca.org.uk/handbook/PRIN/2A/5.html, Pretextual
- https://handbook.fca.org.uk/handbook/prin2a, Pretextual
- _Regulator portal (if any cited link is dud): https://www.fca.org.uk_

### Finding 7. Claude Sonnet 4.6 with web search

**Question (paraphrased to protect IP):**
Is consumer testing of communications a mandatory requirement under the Consumer Duty? What does PRIN 2A.5 require versus what FG22/5 recommends on this point?

**AI's response:**
> "Consumer testing is not an absolute mandatory rule, but PRIN 2A.5.10R (a binding rule, marked 'R' in the Handbook) requires firms to test the effectiveness of their communications 'where appropriate'."

**Regulator's text:**
FG22/5 contains guidance (not rules) recommending firms 'should' consider consumer testing of communications. PRIN 2A.5 (rule) requires firms to act to deliver good consumer understanding outcome, no specific methodology prescribed.

**Why the AI went wrong:**
The model cited a specific rule reference, PRIN 2A.5.10R, as imposing a testing requirement "where appropriate." The FCA's actual rules in PRIN 2A.5 set an outcome obligation (delivering good consumer understanding) without prescribing consumer testing as a specific method. The recommendation to consider consumer testing appears in FG22/5, which is guidance rather than a binding rule. The model cross-referenced the wrong instrument type and attributed a specific rule citation that does not map to the FCA's text in the way described.

**Cited source(s):**
- https://handbook.fca.org.uk/handbook/PRIN/2A/5.html, Pretextual
- https://www.fca.org.uk/publication/finalised-guidance/fg22-5.pdf, Pretextual
- _Regulator portal (if any cited link is dud): https://www.fca.org.uk_

## What Your Team Should Do

The most immediate eval surface this evaluation surfaces is the boundary between binding rules and non-binding guidance in the FCA Handbook. Consumer Duty spans both a rulebook (PRIN 2A, with provisions marked "R", "G", and "E" in the Handbook) and a separate finalised guidance document (FG22/5). Models consistently failed to maintain this distinction, attributing guidance-level recommendations as rule requirements, or vice versa. A targeted eval set should include paired questions that probe whether the model can correctly identify whether a Consumer Duty provision is a binding rule or guidance, and whether it can distinguish between what the FCA requires and what it recommends. This is a replicable pattern across both models tested.

The findings on numerical thresholds and defined terms point to a second eval category: questions where precision matters and where the regulatory text uses a specific term that has a close synonym in ordinary language. The £1 million "annual turnover" threshold for charities (versus "annual income") and the specific conditions in the foreseeable harm provision are examples where both models substituted plausible alternatives for the exact regulatory language. Synthetic training correction pairs built from the FCA Handbook's defined terms, particularly for "retail customer", "foreseeable harm", and the four outcomes, would directly address this failure mode. These terms appear throughout the Handbook and FG22/5 in contexts that could generate large correction-pair sets without requiring novel regulatory interpretation.

The retrieval findings warrant attention from teams working on RAG architectures and web-tool integrations. Both models with web search produced cited sources that were either non-authoritative (law firm commentary, practitioner guides) or used out of context relative to the claim being cited. Neither model's retrieval step appeared to anchor content generation to retrieved documents: the responses read as training-inference completions with citations appended, rather than as summaries of retrieved content. Red-team probes targeting recent FCA publications, particularly feedback statements, Dear CEO letter withdrawals, and post-implementation supervisory communications from 2023–2025, would expose how far the web-search augmentation actually shifts the model's grounding on recently-published regulatory content. The two evasion findings from Claude Sonnet 4.6 with web search on FS25/2 content, combined with the fabricated timeline from Claude Opus 4.7 with web search on the same material, suggest this is a shared weak point in the retrieval layer rather than a model-specific content gap.

## How RLB Can Partner With Your Lab

RegLeg's core capability is maintaining a verified, current, machine-readable corpus of regulatory text across a defined portfolio of regulators and instruments. For the Consumer Duty specifically, this covers PS22/9, PRIN 2A (all sub-chapters), FG22/5, and the ongoing FCA feedback statement and supervisory communication record, updated as the FCA documents. We can provide your evals or post-training team with licensed access to the full question bank under NDA, including the verbatim question set used in this evaluation, the verified regulator-text answers, and the model response records. This gives your team a ready-to-use benchmark on a real-world regulatory surface without any of the IP or sourcing overhead of building it from scratch.

Beyond the question bank, RegLeg can support your teams in two complementary ways. First, we can generate synthetic correction-pair datasets derived directly from the regulator's authoritative text, designed specifically to address the failure modes your models are showing on defined terms, rule/guidance distinctions, and numeric thresholds. These pairs are built by our regulatory specialists from primary source material, not reconstructed from third-party commentary, so they carry the evidentiary weight needed for post-training use. Second, we offer per-regulation deep-dive panels where our specialists walk your alignment or red-team staff through the structural features of a regulation that make it a high-probability hallucination surface: the typographic distinctions between binding rules and guidance, the cross-reference architecture, the defined terms, and the amendment history.

For labs building towards embedded eval coverage on financial regulation, RegLeg offers a quarterly refresh service across a defined regulator portfolio, covering the FCA, PRA, and selected EU and US regulators, that keeps your benchmark current as regulations evolve. Regulatory content is not static: new feedback statements, Dear CEO letters, and supervisory expectations are published continuously, and the gap between a model's training coverage and the live regulatory record is the primary driver of the failure patterns in this evaluation. A partnership with RegLeg means that gap is actively managed rather than accumulating silently between training runs. We are structured as a domain partner, not a data vendor, our preference is to embed within your evals workflow and adapt as your model development priorities shift.


## Related concepts

- Regulation: [CONSUMER-DUTY-PS22-9](/okf/regulations/CONSUMER-DUTY-PS22-9.md)
- Regulator: [FCA-GB-001](/okf/bodies/FCA-GB-001.md)
- Methodology: [v2.3](/okf/methodology.md)