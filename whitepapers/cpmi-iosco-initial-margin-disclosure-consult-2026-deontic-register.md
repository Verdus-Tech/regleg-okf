---
type: "AILabsWhitepaper"
title: "Deontic Register Failure on the CPMI-IOSCO Initial Margin Consultation 2026"
slug: "cpmi-iosco-initial-margin-disclosure-consult-2026-deontic-register"
audience: "ai_labs"
regulation_slug: "CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026"
regulation_id: "320328"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
substrate_version: 1
generated_at: "2026-06-07T08:31:57.765670+00:00"
published_at: "2026-06-07T08:31:57.765670+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/regulators/j1/int/bis-cpmi/CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026/ai-labs/"
timestamp: "2026-06-16T07:45:45.474682+00:00"
---

# Deontic Register Failure on the CPMI-IOSCO Initial Margin Consultation 2026

- **Regulation.** [`CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026`](/okf/regulations/CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026.md) — CPMI-IOSCO Consultation on Updated Guidance and Public Disclosures to Implement Initial Margin Proposals
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)
- **Audience.** ai_labs
- **Methodology.** v2.3
- **Generated.** 2026-06-07T08:31:57.765670+00:00

## Executive summary

The dominant failure observed in Claude Sonnet 4.6 on the CPMI-IOSCO Consultation on Updated Guidance and Public Disclosures to Implement Initial Margin Proposals is deontic register substitution, the model hardened a recommendation into a requirement, replacing 'should' with 'must' when characterising CCP override-framework disclosure obligations. The model identified the correct regulatory subject matter but resolved the consultation's conditional language in the wrong direction, citing a third-party law-firm summary that had editorially strengthened the modal register relative to the primary text. On consultation documents where the normative weight of each modal verb is operationally significant, this failure class carries direct downstream consequences for compliance planning. The failure points to a gap in how the model's retrieval configuration handles deontic precision when secondary-source paraphrase diverges from the regulator's primary text.

## Full whitepaper

# Deontic Register Failure on the CPMI-IOSCO Initial Margin Consultation 2026


The dominant failure observed in Claude Sonnet 4.6 on the CPMI-IOSCO Consultation on Updated Guidance and Public Disclosures to Implement Initial Margin Proposals is deontic register substitution, the model hardened a recommendation into a requirement, replacing "should" with "must" when characterising what CCPs are expected to publicly disclose about their margin model override framework. The source text uses deliberate conditional language; the model's output committed to an obligatory framing that the consultation document does not support. This is not a factual gap on the underlying regulatory substance, the model identified the correct disclosure category and the correct framework, but the modal error is the kind of failure that causes material downstream harm: a compliance officer acting on "must" when the regulator said "should" faces a different planning posture, a different board conversation, and potentially different regulatory exposure. On a consultation document where the normative weight of every verb is load-bearing, register precision is not incidental, it is the substance.

## When This Affects an AI Lab

The CPMI-IOSCO initial margin framework sits at the intersection of global derivatives clearing, CCP risk governance, and cross-border regulatory alignment, precisely the domain where financial institutions, law firms, consultancies, and regulatory-technology vendors are most likely to use frontier models as first-pass research tools. When a compliance professional at a clearing member or CCP asks a model whether a particular disclosure obligation is required or merely recommended, they are making a decision with direct operational and regulatory consequence. A model that consistently upgrading "should" to "must" in this corpus shifts the user's obligation calculus before they have read the source text, compressing a discretionary guidance posture into a mandatory compliance event.

For an AI lab, the exposure is layered. Users acting on confidently-stated "must" language derived from a consultation document that uses "should" may over-provision disclosure infrastructure, misstate their compliance posture to auditors, or escalate to counsel unnecessarily, all traceable downstream to the model's output. Beyond individual users, the failure surface is a red-team gap: evals that test for factual accuracy on regulatory content rarely probe for deontic register fidelity. A model can reproduce the correct substantive content while systematically miscalibrating the normative weight of every obligation it reports, and standard benchmarks will miss this entirely.

Consultation documents from standard-setting bodies like CPMI-IOSCO are structurally high-risk for this failure class. They are long, technically dense, structured around conditional language ("should", "are expected to", "may consider"), and sit in a distinctive normative register between final rule and informal guidance. The consultation format means the authoritative text is often less thoroughly indexed than final rules, and the deontic markers that distinguish a proposal from a requirement are exactly the kind of fine-grained linguistic signal that post-training reward on fluency and accuracy can inadvertently suppress, a model that sounds confident and complete may be doing so by resolving the modal ambiguity in the wrong direction.

## Aggregate Impact

| Model | Configuration | Failure count | Dominant error pattern |
|---|---|---|---|
| Claude Sonnet 4.6 | With web search | 1 | Deontic register hardening, recommendation rendered as requirement |

Claude Sonnet 4.6 with web search produced a response that was substantively oriented toward the correct disclosure category and the correct regulatory framework but committed a deontic register error: the model characterised the CCP override-framework disclosure as a requirement ("must publicly disclose") where the CPMI-IOSCO consultation text specifies a recommendation ("should publicly disclose"). The cited source was a third-party law-firm summary, a Pretextual citation, rather than the consultation document itself, consistent with the retrieval ranker treating secondary summary as authoritative for this query class. The failure is not a gap in knowledge of the subject matter; it is a resolution of normative ambiguity in the wrong direction, likely reinforced by the secondary source's own editorial paraphrase of the original obligation.

The failure here points to a specific gap in how this model's web-search configuration handles modal weight in regulatory consultation language. Consultation documents are structurally distinct from final rules: their obligations are deliberately tentative, and the "should/must" distinction carries legal and operational significance. A retrieval path that routes through third-party summary content amplifies this risk, because secondary sources routinely collapse the consultation's conditional framing into a more decisive register for readability. The model did not correct for this, it reproduced the secondary source's stronger framing without flagging the normative downgrade from the primary text.

## Findings


### Finding 5. Claude Sonnet 4.6 with web search

- **Question (paraphrased to protect IP):** What information are CCPs expected to publicly disclose about their margin model override framework under the CPMI-IOSCO 2026 consultation, and does the guidance frame this as a requirement or a recommendation?
- **AI's response:** "CCPs must publicly disclose relevant information on their margin model override framework."
- **Regulator's text:** CCPs should publicly disclose relevant information on their override framework.
- **Why the AI went wrong:** The model reproduced the correct subject matter, CCP override-framework disclosure, but upgraded the normative weight from the regulator's "should" to "must", converting a recommendation into an obligation. The cited source is a third-party law-firm summary that likely paraphrased the consultation in more decisive language; the model carried that paraphrase through without correcting for the deontic downgrade relative to the primary text. The error is not in the content domain, it is in the model's failure to preserve the modal register of a consultation document, where "should" and "must" are not interchangeable.
- **Cited source(s):**
  - https://www.regulationtomorrow.com/2026/05/cpmi-iosco-consult-on-updated-guid..., Pretextual
  - _Regulator portal: https://www.bis.org_

## What Your Team Should Do

### Implications for your training data

The core failure here, treating a consultation's "should" as equivalent to a final rule's "must", points to a training-data shaping issue specific to regulatory document types. Consultation papers, discussion papers, and guidance consultations from standard-setting bodies like CPMI-IOSCO occupy a distinct normative register that sits between informal commentary and binding rule. If the training corpus does not separate these document types with explicit deontic-register signal, the model learns a blurred obligation landscape: final rules, consultations, and guidance merge into a single regulatory-content bucket where "should" and "must" are treated as near-synonyms rather than load-bearing modal distinctions. A targeted fix: the training corpus for regulatory content should include explicit annotation of document type (final rule / consultation / guidance / speech), and the deontic markers within each document type should carry type-conditional weight in the training signal. Pairs of consultation-text passages alongside their final-rule counterparts, where the obligation language strengthened between stages, would directly surface this distinction to the model.

The secondary-source routing failure compounds the training issue: the model's retrieval path treated a third-party law-firm summary as an authoritative source for a normative question about a consultation document. Law-firm summaries routinely resolve conditional language into more definitive framing for readability. The training corpus for this domain should pair primary regulator text with its common secondary-source paraphrases, with explicit divergence scoring on deontic modal terms, so the model learns that "the law firm said must; the regulator said should" is a meaningful divergence, not a stylistic variant.

### Implications for your post-training logic

The retrieval ranker, when web search is active, should apply a primary-source preference signal for regulator-name + obligation-type queries. Queries that ask whether a specific obligation is "required" or "recommended" are precisely the queries where third-party summary divergence from the primary text is most consequential, and currently the ranker appears to treat a third-party summary as equally authoritative to the regulator's own published text for this query class. A targeted calibration: for queries containing a regulator name + a normative question token ("required", "must", "should", "recommended", "mandatory"), the ranker should down-weight secondary summary sources and privilege the regulator's own domain.

Additionally, the model's confidence calibration on normative assertions needs tightening for consultation-class documents. When the best available retrieved source is a secondary paraphrase of a consultation (rather than the consultation itself), the model should express lower confidence on the obligation-level characterisation and flag the distinction between "the guidance proposes" and "the rule requires." A self-check pass on modal terms, specifically, flagging cases where the model's drafted response uses stronger obligation language ("must", "shall", "required") than the retrieved source text supports, would catch this class of error before output is finalised.

### Specific eval / red-team probes RegLeg suggests

- **Consultation-vs-final-rule modal fidelity:** Probe the model with parallel questions about the same regulatory topic drawn from the consultation version and the final rule, verify that the model preserves the modal distinction rather than converging on the stronger obligation language.
- **Third-party paraphrase correction:** Feed the model a secondary-source summary that strengthens modal language relative to the primary, then ask a normative question, verify that the model flags the discrepancy rather than amplifying the secondary source's register.
- **Standard-setting body consultation corpus:** CPMI-IOSCO, FSB, BCBS, IOSCO, and IAIS all publish consultation documents in this register; probe systematically across these bodies for modal-hardening errors.
- **Override and discretionary-framework disclosure probes:** Across CCP and CSD regulatory frameworks, probe for disclosure obligations that are framed as recommended rather than required, this is a recurring pattern in post-crisis infrastructure guidance where the normative weight is intentionally graduated.
- **Regulator portal primary vs. aggregator secondary:** For any normative query about a recent consultation, compare the model's response when the retrieval path returns the regulator's own domain vs. a third-party aggregator, map the modal drift between source types.

## How RLB Can Partner With Your Lab

Across our documented work on regulatory content, spanning CCPs, prudential banking rules, consumer protection frameworks, and cross-border market infrastructure standards, we have catalogued specific, recurring failure shapes: deontic register hardening on consultation-class documents; subcategory-numeric conflation on disaggregated statistical thresholds; multi-body institutional attribution drift where the named lead is the lower-frequency institution; schema over-specification on technical message formats; and false-negative evasion on retrievable official-speech content from early-adoption periods. These are not isolated incidents. They are structural failure surfaces that appear predictably across model configurations and regulatory domains, and they are the kind of gap that internal eval coverage, focused on the lab's own model in isolation, is poorly positioned to surface.

We can deliver targeted correction-pair generation per failure mode, derived from the regulator's authoritative text and formatted for direct ingestion into your training-data pipeline, covering deontic register pairs, primary-vs-secondary-source modal divergence examples, and structured obligation-taxonomy annotations across the consultation → final-rule → guidance spectrum. We can run embedded eval partnerships against a defined regulator portfolio, producing quarterly comparative reports across model versions with regression monitoring on previously-documented failure modes, so your team knows whether a model update improved or degraded performance on this failure class. For capability launches that touch regulated domains, financial services, payments infrastructure, cross-border regulatory content, we can run pre-release evaluation cycles and flag failure shapes before they reach customers. And for new regulations entering your deployment footprint, we offer red-team consultation on regulator-specific failure surfaces tailored to the document type and normative register.

To scope a partnership for refining your models against these failure modes, reach out at reglegbrief.com.


## Related concepts

- Regulation: [CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026](/okf/regulations/CPMI-IOSCO-INITIAL-MARGIN-DISCLOSURE-CONSULT-2026.md)
- Regulator: [BIS-CPMI-INT-001](/okf/bodies/BIS-CPMI-INT-001.md)
- Methodology: [v2.3](/okf/methodology.md)