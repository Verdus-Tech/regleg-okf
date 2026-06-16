---
type: "AILabsWhitepaper"
title: "AI Model Hallucination Patterns on CPMI-IOSCO PFMI: A RegLeg Research Report"
slug: "cpmi-iosco-pfmi-2012-ai-labs"
audience: "ai_labs"
regulation_slug: "CPMI-IOSCO-PFMI-2012"
regulation_id: "320317"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-11T01:35:19.027168+00:00"
published_at: "2026-06-07T01:33:31.767655+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/bis-cpmi/CPMI-IOSCO-PFMI-2012/ai-labs/"
timestamp: "2026-06-16T07:45:40.361391+00:00"
---

# AI Model Hallucination Patterns on CPMI-IOSCO PFMI: A RegLeg Research Report

- **Regulation.** [`CPMI-IOSCO-PFMI-2012`](/okf/regulations/CPMI-IOSCO-PFMI-2012.md) — Principles for Financial Market Infrastructures (PFMI)
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-11T01:35:19.027168+00:00

## Executive summary

RegLeg tested two frontier AI models against the Principles for Financial Market Infrastructures (PFMI), the global standard for payment systems, central counterparties, and securities settlement systems published jointly by the Bank for International Settlements Committee on Payments and Market Infrastructures (CPMI) and IOSCO in April 2012. The models tested were Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search, evaluated against the PFMI's Principle 2 governance text and Annex F oversight provisions on critical service providers. Three findings remain active after substrate verification and audit cleanup. All three are inference-drift failures: outputs in which the model substituted a training-data prior for the regulator's actual KC-level or annex text, producing structurally confident citations that do not survive a check against the PFMI document. The pattern is operationally significant for any AI lab whose model is used in regulatory-research tasks because the PFMI is the operative governance standard for systemically critical financial market infrastructure across major jurisdictions.

## Full whitepaper

# AI Model Hallucination Patterns on CPMI-IOSCO PFMI: A RegLeg Research Report


RegLeg tested two frontier AI models against the Principles for Financial Market Infrastructures (PFMI), the global standard for payment systems, central counterparties, and securities settlement systems published jointly by the Bank for International Settlements Committee on Payments and Market Infrastructures (CPMI) and IOSCO in April 2012. The models tested were Claude Opus 4.7 with web search and Claude Sonnet 4.6 with web search, evaluated against the PFMI's Principle 2 governance text and Annex F oversight provisions on critical service providers. Three findings remain active after substrate verification and audit cleanup. All three are inference-drift failures: outputs in which the model substituted a training-data prior for the regulator's actual KC-level or annex text, producing structurally confident citations that do not survive a check against the PFMI document. The pattern is operationally significant for any AI lab whose model is used in regulatory-research tasks because the PFMI is the operative governance standard for systemically critical financial market infrastructure across major jurisdictions.

## When This Affects an AI Lab

The PFMI is the operational backbone of global financial markets. It governs every clearing house, central securities depository, and systemically important payment system across the major jurisdictions where banks, asset managers, and infrastructure operators are supervised. Users in compliance, legal, risk management, board secretariat, and regulatory affairs at FMIs, FMI participants, supervisors, and external advisers routinely use AI assistants for first-pass orientation on the framework's 28 Principles, the underlying Key Considerations, and the annex provisions that scope third-party oversight obligations. When a model produces a structurally confident but wrong answer about, for example, the composition requirements of a board risk committee under Principle 2, or the direction of supervisory oversight under Annex F, a user acting on that output drafts a document (a committee charter, a self-assessment response, a board paper, a transaction opinion) that misstates the regulatory position. The misstatement then circulates through internal review, supervisor liaison, or counterparty due diligence.

For an AI lab, the downstream exposure has two shapes. First, users who rely on confident model outputs to navigate PFMI compliance and act on fabricated or inverted claims face direct regulatory risk, potential supervisor findings in a PFMI assessment cycle, embedded misstatements in disclosure-framework responses, or board governance arrangements documented against citations that do not check out. Second, when the errors are traceable to the model, they create reputational and litigation exposure for the lab in a domain where the regulatory record is precisely documented and auditable. The PFMI assessment cycle generates published Level 2 and Level 3 monitoring reviews by national authorities and the FSB; that evidentiary chain establishes exactly what the operative regulatory position was at any given date.

What makes the PFMI a particularly acute failure surface is its structural profile. The framework deliberately leaves implementation detail to the FMI while binding it to framework-level obligations whose actual text matters: KC 6's documented risk-management framework requirement, Annex F's scope-direction language, the assessment methodology's rating scale terminology. A model that fills in implementation specifics from generic corporate-governance or supervisory-architecture priors will produce outputs that look authoritative, specific KC numbers, named annex provisions, quoted phrasing, while the underlying citations either invert the regulator's stated scope or assert requirements that do not appear in the published text. That gap, between the form of the answer and the substance of the regulatory source, is the failure surface this finding set documents.

## Aggregate Impact

**Claude Opus 4.7 with web search**, 1 active finding. On PFMI Principle 2 KC 6, Opus 4.7 fabricated a non-executive risk-committee chair mandate that does not appear in the PFMI text. KC 6 speaks only to the documented risk-management framework and the independence of control functions; the committee-composition language is a training-data prior from adjacent corporate-governance literature substituted for the regulator's actual KC text. The accompanying inversion of KC ordering and misattribution of KC 5's management-roles content to internal-control requirements indicates the model reconstructed the Principle 2 governance architecture from training-weighted best-practice frameworks rather than from the document's actual structure.

**Claude Sonnet 4.6 with web search**, 2 active findings. On Principle 2, Sonnet 4.6 attached a soft risk-committee recommendation to KC 5 with quoted committee-mandate language, when KC 5's actual subject is the roles and responsibilities of management. The compound error, wrong KC number, fabricated quoted text, citation to a third-party FMI disclosure document rather than the PFMI primary source, makes the failure especially hard to detect on review. On Annex F, Sonnet 4.6 inverted the regulator's stated supervisory scope, asserting that authorities do not directly supervise or oversee CSPs and that the annex's expectations "flow from the FMI to its CSPs." Annex F's opening text contradicts that framing.

The joint pattern is consistent across both models: structured fabrications and inversions where the PFMI's actual KC-level or annex text is at the framework level ("the board should establish a documented risk-management framework," "the expectations outlined below are specifically targeted at critical service providers") and the model fills in implementation detail or scope-direction framing from training-data priors. The retrieval step is not catching or correcting the substitution. For an alignment team, the diagnostic value of this finding set is that it isolates a specific category of failure, generic-prior interference on regulator-specific framework text, that is high-confidence at generation, high-impact at use, and invisible to surface-level review by the user.

## Findings


### Finding 22. Claude Opus 4.7 with web search

- **Question (paraphrased to protect IP):** PFMI Principle 2 KC 6, non-executive risk-committee chair mandate fabricated
- **AI's response:** "KC 2.6 contemplates that the board establish a risk committee that is chaired by a suitably qualified, non-executive member"
- **Regulator's text:** KC 6: The board should establish a clear, documented risk-management framework... Governance arrangements should ensure that the risk-management and internal control functions have sufficient authority, independence, resources, and access to the board.
- **Why the AI went wrong:** On PFMI Principle 2's Key Consideration 6, Claude Opus 4.7 with web search asserted that the board should establish "a risk committee that is chaired by a suitably qualified, non-executive member," and accompanied this with an inverted KC ordering and a misattribution of KC 5's management-roles content to internal-control requirements. The fabricated non-executive-chair mandate is the kind of high-confidence structured hallucination that an FMI board secretary or governance lead drafting a committee charter would absorb directly into the document, because the surface form looks like a PFMI self-assessment response. The error reflects a training-weighted prior on corporate-governance committee structure (drawn from listing rules, banking-supervision codes, and conventional governance frameworks) substituted for the PFMI's framework-level KC 6 text, which speaks only to the documented risk-management framework and the independence of control functions. Verbatim paragraph probes across the Principle 2 KCs, with structured comparison against generic corporate-governance language, would directly target this class of error.
- **Citation ID:** [RLB-F-INT-BIS-CPMI-IOSCO-PFMI-2012-Q022](https://reglegbrief.com/regulators/j1/int/bis-cpmi/cpmi-iosco-pfmi-2012/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-PFMI-2012-v1-022--opus-47-websearch/)
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 11. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** Annex F critical service provider oversight, supervisory scope inverted
- **AI's response:** "under the PFMI framework, authorities do not directly supervise or oversee CSPs. The responsibility for ensuring CSP compliance with Annex F expectations rests with the FMI itself; the FMI is expected to contractually require and monitor its CSPs' adherence. Annex F is framed as expectations that flow from the FMI to its CSPs"
- **Regulator's text:** A regulator, supervisor, or overseer of an FMI may want to establish expectations for an FMI's critical service providers in order to support the FMI's overall safety and efficiency. The expectations outlined below are specifically targeted at critical service providers.
- **Why the AI went wrong:** On Annex F, Claude Sonnet 4.6 with web search inverted the regulator's stated scope, asserting that authorities do not directly supervise or oversee critical service providers and that Annex F's expectations "flow from the FMI to its CSPs." Annex F's opening text expressly contemplates the opposite: a regulator, supervisor, or overseer of an FMI may want to establish expectations directed at CSPs, and the outlined expectations are "specifically targeted at critical service providers." The inversion is structural rather than textual, the model converted a regulator-to-CSP oversight channel into an FMI-internalised contractual obligation, and is the kind of failure that would not surface in standard text-completion evaluations because the surface form of the answer is internally coherent. A probe specifically on Annex F's scope-direction language, tested against the model's default framing of FMI-CSP supervisory relationships, would expose whether the inversion is model-specific or a corpus-level pattern.
- **Citation ID:** [RLB-F-INT-BIS-CPMI-IOSCO-PFMI-2012-Q011](https://reglegbrief.com/regulators/j1/int/bis-cpmi/cpmi-iosco-pfmi-2012/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-PFMI-2012-v1-011--sonnet-46-websearch/)
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

### Finding 22. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** PFMI Principle 2, risk-committee recommendation misattributed to KC 5
- **AI's response:** "the PFMI does not expressly mandate a dedicated risk committee as a hard requirement, but Key Consideration 2.5 states that the board should consider establishing a risk committee with a clear mandate"
- **Regulator's text:** 5. The roles and responsibilities of management should be clearly specified. An FMI's management should have the appropriate experience, a mix of skills, and the integrity necessary to discharge their responsibilities for the operation and risk management of the FMI.
- **Why the AI went wrong:** On PFMI Principle 2, Claude Sonnet 4.6 with web search attached a soft risk-committee recommendation to Key Consideration 5: "Key Consideration 2.5 states that the board should consider establishing a risk committee with a clear mandate." KC 5 actually addresses the roles and responsibilities of management, not committee structure. The compound error, wrong KC number, fabricated quoted language, and a citation to a third-party FMI disclosure document rather than the primary PFMI source, makes the failure especially hard to detect: the citation pattern (a specific KC number with quoted text) is structurally indistinguishable from a verified citation. The model's citation generator reached for the most accessible document that mentions PFMI rather than the authoritative source, a pattern that an alignment team could test by probing whether the model preferentially cites primary regulator portals when the verbatim text is requested versus when only a paraphrase is asked for.
- **Citation ID:** [RLB-F-INT-BIS-CPMI-IOSCO-PFMI-2012-Q022](https://reglegbrief.com/regulators/j1/int/bis-cpmi/cpmi-iosco-pfmi-2012/ai-labs/finding/INT-BIS-CPMI-INT-001-CPMI-IOSCO-PFMI-2012-v1-022--sonnet-46-websearch/)
- **Cited source(s):**
  - _Regulator portal: https://www.bis.org_

## What Your Team Should Do

The PFMI findings point to three concrete areas for your evals and alignment teams. First, the failure shape is generic-prior interference on regulator-specific framework text. Where the PFMI's actual KC or annex text is at the framework level, "the board should establish a documented risk-management framework," "the expectations outlined below are specifically targeted at critical service providers", both models tested filled in implementation specifics from training-data priors (committee-chair composition, FMI-internalised oversight framing). Targeted probes across framework-level regulatory text, not just PFMI but Basel III's SREP governance guidelines, IOSCO Objectives and Principles, FCA SYSC, would directly surface this class of error.

Second, the citation pattern is diagnostic. Both models produced specific KC numbers with quoted phrasing in the context of fabricated or misattributed content. On the Sonnet finding, the model cited a third-party FMI disclosure document rather than the BIS primary source. That citation behaviour suggests the citation generator is reaching for the most accessible document that mentions the framework rather than for the authoritative source. A probe that tests whether the model preferentially cites primary regulator portals (bis.org publications, iosco.org publications) when verbatim text is requested versus when only a paraphrase is asked for would isolate whether this is a citation-layer behaviour or an upstream retrieval issue.

Third, the Annex F inversion is the kind of structural error that would not show up in standard text-completion evaluations because the surface form of the answer is internally coherent. The model produced a logically consistent FMI-internalised oversight framing that just happens to invert the regulator's actual scope direction. Scope-direction probes, testing whether the model preserves the regulator's stated direction of oversight on provisions where supervisory direction is contested or unusual, would surface this category of failure. Synthetic training pairs derived from the verbatim text of Annex F's opening provision, paired against the inverted framing the model produced here, would be a directly usable corrective for any model showing the same behaviour.

## How RLB Can Partner With Your Lab

RegLeg has built a structured question bank across PFMI and the broader CPMI-IOSCO publication corpus, designed specifically to probe the failure surfaces that matter in regulatory-research tasks. For the framework-level failure shape documented here, generic-prior interference on regulator-specific KC and annex text, the question bank includes verbatim-paragraph probes across Principle 2's KCs, scope-direction probes on Annex F, and structured comparisons against generic corporate-governance language drawn from listing rules and supervisory codes. We make the question bank available to AI labs under NDA as a licensed eval resource, with full paraphrase-to-original mappings so your team can understand exactly what each probe is testing without the IP being exposed publicly.

Where a deeper engagement makes sense, we offer per-regulation specialist panels, structured sessions with our regulatory domain team on a defined PFMI topic area (Principle 2 governance, Annex F oversight scope, the assessment methodology rating scale, the broader CCP resilience or stablecoin guidance lineage), covering the document family, the current operative standards, the open consultations, and the structural KC and annex relationships in sufficient depth to support targeted fine-tune data construction. These sessions are designed to be actionable for post-training and evals teams.

On the training-data side, RegLeg can generate synthetic correction-pair datasets derived from the regulator's authoritative text, question/wrong-answer/correct-answer triples drawn from real observed failure patterns, with sourcing back to the primary document. For the PFMI failures documented here, the highest-value targets are the Principle 2 KC sub-paragraphs (which drive most of the framework-level recall failures), Annex F's opening scope-direction text, and the assessment methodology rating scale terminology. We also offer embedded eval coverage on a defined regulator portfolio, refreshed quarterly as new consultations and final guidance are published, so your evals stay current with the regulation rather than lagging it.


## Related concepts

- Regulation: [CPMI-IOSCO-PFMI-2012](/okf/regulations/CPMI-IOSCO-PFMI-2012.md)
- Regulator: [BIS-CPMI-INT-001](/okf/bodies/BIS-CPMI-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)