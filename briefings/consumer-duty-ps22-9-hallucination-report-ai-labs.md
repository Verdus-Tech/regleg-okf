---
type: "PublicBriefing"
title: "Consumer Duty Hallucination Report: frontier AI models"
slug: "consumer-duty-ps22-9-hallucination-report-ai-labs"
regulation_slug: "CONSUMER-DUTY-PS22-9"
body_id: "FCA-GB-001"
jurisdiction_code: "GB"
j_level: "J3"
regulator_short_code: "FCA"
methodology_version: "2.3"
news_featured_at: "2026-06-12T12:00:21.164700+00:00"
published_at: "2026-06-07T08:31:34.320675+00:00"
generated_at: "2026-06-11T01:42:44.211287+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/consumer-duty-ps22-9-hallucination-report-ai-labs/"
timestamp: "2026-06-16T07:45:48.382721+00:00"
---

# Consumer Duty Hallucination Report: frontier AI models

- **Regulation.** [`CONSUMER-DUTY-PS22-9`](/okf/regulations/CONSUMER-DUTY-PS22-9.md) — Consumer Duty (PS22/9 + PRIN 2A)
- **Regulator.** [`FCA-GB-001`](/okf/bodies/FCA-GB-001.md)

## News lead

Two frontier AI models running with web search enabled, both tested by the RLB Specialist Panel, produced confidently wrong reconstructions of the UK Financial Conduct Authority's Consumer Duty (PS22/9 and PRIN 2A), the conduct framework governing how authorised firms must act to deliver good outcomes for retail customers. The RegLeg Brief Specialist Panel tested both models across the Duty's foreseeable-harm provision, fair-value assessment expectations, and scope exclusions, and documents eleven findings in which the models added requirements the FCA's text does not contain, or restated settled rules with new conditions attached.

Claude Opus 4.7, asked whether the Consumer Duty applies to group insurance distribution, asserted that "the FCA addressed this in further consultation (CP23/something on group insurance practices) and confirmed that firms manufacturing/distributing policies where individual retail beneficiaries are protected fall within scope." PRIN 2A says the opposite: the Consumer Duty "does not apply to ... activities connected to the distribution of group insurance policies or the extension of these policies to new members." The cited consultation paper number is itself a placeholder, "CP23/something", that the regulator never issued.

Claude Sonnet 4.6, asked about fair-value methodology, wrote that the FCA "does expect firms to go beyond qualitative description and provide substantiated comparisons" for non-monetary costs and benefits. FG22/5 says the precise opposite: "The FCA does not expect firms to quantify non-monetary costs and benefits as part of its fair value assessment process, but firms should undertake some form of qualitative assessment." The model inverted the regulator's stated position on what kind of analysis the Duty requires.

A compliance officer at a UK bank, insurer, or investment platform relying on either output would build a Consumer Duty programme around requirements the FCA never imposed, and would route those requirements through internal governance papers, board minutes, and supervisor-facing disclosures. That is the failure mode these findings document.


## Briefing

# Frontier AI models rewrote FCA Consumer Duty rules with fabricated conditions and inverted fair-value methodology, regulatory-research panel finds

## *Two frontier AI models with web search enabled, added conditions to the foreseeable-harm provision the FCA never wrote, cited a non-existent consultation paper to bring group insurance distribution into scope, and inverted FG22/5 guidance on non-monetary fair-value assessment. The RegLeg Brief Specialist Panel calls the class "Confident Elaboration" and says it points to a generation pathway in which retrieval-augmented models complete regulator-sounding text from training priors rather than from the FCA's actual rulebook.*

**SINGAPORE, June 12, 2026.** Two frontier artificial-intelligence models generated structurally confident but textually wrong reconstructions of the UK Financial Conduct Authority's (FCA) Consumer Duty, the conduct regime set out in Policy Statement PS22/9 and codified in the PRIN 2A chapter of the FCA Handbook, with supplementary finalised guidance in FG22/5, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The eleven findings, published with immutable RLB Citation IDs including `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q018-Opus47`, `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q008-Sonnet46`, `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q003-Opus47`, and `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q002-Sonnet46`, span the Consumer Duty's foreseeable-harm provision, fair-value assessment expectations, the scope exclusions in PRIN 2A.1, the legal-basis question on FSMA, and recent FCA feedback statements. Both Anthropic's Claude Opus 4.7 and Claude Sonnet 4.6 were tested with web search active, mirroring the configuration in which compliance, legal, and product staff at UK-authorised firms and their advisers actually use the models.

## The Verbatim Rule: PRIN 2A and FG22/5

The Consumer Duty is a layered framework. Principle 12 ("A firm must act to deliver good outcomes for retail customers") sits at the top of the FCA's Principles for Businesses. PRIN 2A is the rulebook chapter that operationalises it, with provisions marked "R" (binding rules), "G" (guidance), and "E" (evidential provisions). FG22/5 is the finalised guidance document published alongside PS22/9.

Three of the verbatim passages tested here read:

- **Foreseeable harm (PRIN 2A.2)**: "Where a firm reasonably believes a retail customer understands and accepts such risks, it will not breach the rule if it fails to prevent them."
- **Scope exclusion (PRIN 2A.1.8R)**: the Consumer Duty "does not apply to reinsurance, contracts of large risk sold to commercial customers where risk is located outside the UK, nor to activities connected to the distribution of group insurance policies or the extension of these policies to new members."
- **Fair value methodology (FG22/5)**: "The FCA does not expect firms to quantify non-monetary costs and benefits as part of its fair value assessment process, but firms should undertake some form of qualitative assessment."

Each of these provisions states a single, unhedged position. None contains the conditions, additional procedural requirements, or methodological expectations that the models grafted on.

## Claude Opus 4.7: Fabricated a Consultation Paper to Pull Group Insurance Into Scope

Asked whether the Consumer Duty applies to reinsurance, group insurance distribution, and large-risk commercial contracts, Claude Opus 4.7 (with web search on) wrote, verbatim:

> "Group insurance: the Duty can apply via the distribution chain when group policy beneficiaries are retail customers; the FCA addressed this in further consultation (CP23/something on group insurance practices) and confirmed that firms manufacturing/distributing policies where individual retail beneficiaries are protected fall within scope."

**The structural error.** PRIN 2A.1.8R expressly excludes the distribution of group insurance policies from the Consumer Duty. There is no FCA consultation paper that brings group insurance distribution into scope; the citation "CP23/something" is itself a structural tell, a placeholder the model produced where a real paper number would sit. A UK insurer or broker treating the model's output as authoritative would:

- Apply Consumer Duty conduct obligations to group insurance distribution activities the FCA has deliberately excluded.
- Build Consumer Duty product-governance, fair-value, and consumer-understanding workstreams over group insurance schemes that sit outside PRIN 2A's scope.
- Cite a non-existent consultation paper in internal compliance papers and supervisor-facing self-assessments.

**Why it failed.** The Specialist Panel writes that the model "completes a Consumer-Duty-applies frame from priors about how broad consumer-protection regimes typically extend through distribution chains, rather than retrieving the express exclusion at PRIN 2A.1.8R. The placeholder consultation reference is the signature of a fabricated citation: the model knows the answer requires a citation, but cannot supply one because none exists."

The failure mode is classified as `misstated_rule` against substrate document `R3-GUIDELINE-Q17_consumer_duty_focus_areas.pdf`.

On a separate question on the foreseeable-harm provision, Opus 4.7 added conditions the FCA's text does not contain, writing that the Duty is satisfied "where a retail customer understands the risk and the firm has acted in good faith, supported understanding, avoided foreseeable harm caused by its own conduct, and otherwise complied with the Duty." PRIN 2A's actual safe-harbour is narrower and turns on one test: whether the firm reasonably believes the customer understands and accepts the risk. The model layered three additional conditions onto a provision that contains none of them.

## Claude Sonnet 4.6: Inverted FG22/5 on Fair-Value Methodology and Misstated the Legal Basis

On fair-value assessment methodology, Claude Sonnet 4.6 (with web search on) wrote:

> "the FCA does not mandate a single financial methodology for non-monetary items, but it does expect firms to go beyond qualitative description and provide substantiated comparisons."

**The inversion.** FG22/5's actual position is that the FCA does not expect firms to quantify non-monetary costs and benefits at all, and that a form of qualitative assessment is sufficient. The model has reversed the expectation: where the regulator says "qualitative is enough", the model tells the user "qualitative is not enough, you must go further." A product-governance lead at a UK retail bank or investment platform reading this output would build a fair-value assessment template that demands a level of non-monetary quantification the FCA has expressly said is not required, raising both the cost and the documentation burden of the Duty's product-governance workstream with no regulatory basis.

On a separate question on the Consumer Duty's legal basis, Sonnet 4.6 stated that "the legal basis is the FCA's statutory rule-making power under the Financial Services and Markets Act 2000 (FSMA 2000)", with framing that implied FSMA 2023 had no relevance at all. The regulator-text position is narrower: FSMA 2023 did not create the Consumer Duty, but the model's framing collapses a precise temporal fact into a generic FSMA 2000 attribution, omitting that the post-Brexit FSMA 2023 conduct architecture sits alongside the Duty.

The failure mode for the Sonnet findings is classified as `inference_drift` or `misstated_rule` against substrate documents `p_05_REGULATION_FG22_5___Fair_value_assessment__no_quant_2.html` and `R2-REGULATION-PS22_9_full_policy_statement.pdf`.

## The Pattern: **Confident Elaboration**

The Consumer Duty findings sit inside a failure class the RegLeg Brief Specialist Panel labels **Confident Elaboration**: frontier models generating regulator-sounding completions that add conditions, methodological expectations, or scope extensions the regulator's text does not contain, while routing the output through the surface forms (citations, defined terms, rule numbering) that ordinarily mark authoritative regulatory writing.

Across the eleven findings, the elaboration takes four shapes:

- **Fabricated procedural conditions** (Opus 4.7 on PRIN 2A.2): generic "good faith / supported understanding / otherwise complied" language is layered onto a single-test safe-harbour the regulator wrote tightly.
- **Scope expansion via non-existent citation** (Opus 4.7 on PRIN 2A.1.8R): the express group-insurance exclusion is overridden by a fabricated consultation paper that brings the excluded activity back into scope.
- **Methodological inversion** (Sonnet 4.6 on FG22/5): the regulator's "qualitative is sufficient" position is recast as a "qualitative is not sufficient" expectation, doubling the assessment burden the Duty imposes.
- **Citation pretextuality** (both models, across the FS25/2 and Dear CEO findings): web-retrieved sources are appended to responses that were already generated from training inference, without the retrieval step actually anchoring the content.

The common substrate is a generation pathway in which the model's prior about what a "comprehensive" answer on a UK conduct rule looks like overrides the FCA's actual structural decisions about what the rule requires.

## Why the Failure Is Invisible at Runtime

All eleven outputs shared the same surface characteristics: confident rule-level citations, internally coherent conduct logic, defined-term usage that tracks the Handbook vocabulary, and no hedging or caveats. The failure is not recoverable by the user in real time because the output reads like a Consumer Duty self-assessment response, the kind of paragraph a compliance lead would expect to receive from a senior consultant. Validation against the regulator's primary text would only happen if the reader already knew which PRIN 2A provision contained which subject matter, which is the question they asked the model in the first place.

The population most exposed includes compliance and conduct-risk officers at UK banks, insurers, investment platforms, and consumer-credit firms; product-governance leads completing fair-value assessment templates; legal counsel drafting Consumer Duty board reports and the annual board assessment required by PRIN 2A.8.3R; supervisory and complaint-handling staff at UK firms scoping the foreseeable-harm provision into customer journey maps; and external consultants advising on Consumer Duty implementation. All of these workflows route through AI-assisted research on tight timelines, and almost all of them generate written deliverables that downstream readers treat as authoritative without re-checking the underlying citation.

## What AI Labs Can Do: Suggested Probes (Open-Access)

The RegLeg Brief Specialist Panel documents a series of red-team probe designs that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **Rule-versus-guidance attribution probes.** For each Consumer Duty provision, generate paired questions that ask the model to identify whether the source is a binding rule (PRIN 2A "R"), guidance (PRIN 2A "G"), evidential provision (PRIN 2A "E"), or finalised guidance (FG22/5). Test whether the model preserves the binding-versus-non-binding distinction or collapses it.
2. **Safe-harbour minimality tests on the foreseeable-harm provision.** Probe PRIN 2A.2 with questions that test whether the model adds conditions ("good faith", "supported understanding", "complied with the Duty otherwise") to a safe-harbour that turns on a single test. Compare against the regulator's verbatim wording.
3. **Scope-exclusion preservation probes.** For each express exclusion in PRIN 2A.1.8R (reinsurance, large-risk commercial contracts, group insurance distribution), test whether the model preserves the exclusion or pulls the excluded activity back into scope via a fabricated or misattributed authority.
4. **Citation-integrity probes on placeholder consultation references.** Where the model produces a citation pattern such as "CP23/something" or "the further FCA consultation", verify the citation independently. Placeholder citations are a strong tell for confident-elaboration drift and a tractable eval signal.
5. **Methodological-expectation inversion tests on FG22/5.** Probe the fair-value, consumer-understanding, and consumer-support guidance for inversions of "the FCA does not expect" / "firms should" framings. Test whether the model preserves the regulator's expectation level or upgrades it into a stronger requirement.

## Open-Access Risk Mitigation: A Public Good for AI Labs, Regulators, and the Compliance Community

RegLeg Brief operates as a completely ungated, open-access public resource. The white papers, per-finding cards, regulator verbatim excerpts, RLB Citation IDs, methodology notes and supporting data logs are all published without paywalls, registration walls, or data-licensing fees. By documenting original regulatory research without financial or distribution barriers, the platform ensures that:

- **AI engineering and alignment teams** can immediately ingest the verbatim model outputs and matched regulator-text excerpts to identify, reproduce, and address the structural failure modes the Specialist Panel documents.
- **Regulatory agencies and supervisors** can use the standardised RLB Citation IDs to benchmark AI-driven compliance risks surfacing in their own jurisdictions, with full traceability back to the original model output and the regulator's primary source.
- **The global compliance, treasury, and legal community** can freely adapt the Specialist Panel's screening methodologies to safeguard internal data pipelines and AI-assisted regulatory workflows.

Because RegLeg Brief conducts its own original research and adversarial analysis against frontier AI models, the detail in each published finding is precise enough to enable AI labs to take targeted hallucination-mitigation measures. Directions an AI lab might consider, drawing on the published findings, include:

- **Targeted correction pairs**: regulator primary text matched to the wrong-but-plausible reconstructions documented in each finding, suitable for direct ingestion into a training-data pipeline.
- **Quarterly embedded eval cycles**: continuous evaluation against a defined regulator portfolio, with regression monitoring on previously documented failure modes.
- **Pre-release evaluation cycles**: sandboxed probes against catalogued failure shapes for capability releases touching the relevant regulatory domain, before the release reaches customers.
- **Post-release model enhancements**: regulator-specific failure-surface monitoring as new regulatory domains enter a model's live deployment footprint.

AI labs and model developers named in any published finding have an unconditional [right of reply](https://reglegbrief.com/right-of-reply/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** FCA PS22/9 + PRIN 2A + FG22/5 · Substrate documents: `R2-REGULATION-PS22_9_full_policy_statement.pdf`, `R3-GUIDELINE-Q17_consumer_duty_focus_areas.pdf`, `p_05_REGULATION_FG22_5___Fair_value_assessment__no_quant_2.html`, `p_05_REGULATION_FG22_5_vs_PRIN_2A___guidance_obligation_2.html`, `p_15_OTHER_PART_CIRCULAR___Dear_CEO_letters_withdra_page.html`, `p_21_ACT_FS25_2__March_2025____Rules_and_Dear_CEO_137A.html` · FCA portal: fca.org.uk

**Citation IDs referenced:**

- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q002-Sonnet46`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q003-Opus47`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q007-Sonnet46`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q008-Opus47`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q008-Sonnet46`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q013-Opus47`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q013-Sonnet46`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q018-Opus47`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q020-Opus47`
- `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q020-Sonnet46`


## Related concepts

- Whitepaper: [consumer-duty-ps22-9-hallucination-report-ai-labs](/okf/whitepapers/consumer-duty-ps22-9-hallucination-report-ai-labs.md)
- Regulation: [CONSUMER-DUTY-PS22-9](/okf/regulations/CONSUMER-DUTY-PS22-9.md)
- Methodology: [v2.3](/okf/methodology.md)