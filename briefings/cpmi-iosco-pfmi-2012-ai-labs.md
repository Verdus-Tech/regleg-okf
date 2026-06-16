---
type: "PublicBriefing"
title: "AI Model Hallucination Patterns on CPMI-IOSCO PFMI: A RegLeg Research Report"
slug: "cpmi-iosco-pfmi-2012-ai-labs"
regulation_slug: "CPMI-IOSCO-PFMI-2012"
body_id: "BIS-CPMI-INT-001"
jurisdiction_code: "INT"
j_level: "J1"
regulator_short_code: "BIS-CPMI"
methodology_version: "v2.3"
news_featured_at: "2026-06-12T08:00:01.869521+00:00"
published_at: "2026-06-07T01:33:31.767655+00:00"
generated_at: "2026-06-11T01:35:19.027168+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cpmi-iosco-pfmi-2012-ai-labs/"
timestamp: "2026-06-16T07:42:08.039977+00:00"
---

# AI Model Hallucination Patterns on CPMI-IOSCO PFMI: A RegLeg Research Report

- **Regulation.** [`CPMI-IOSCO-PFMI-2012`](/okf/regulations/CPMI-IOSCO-PFMI-2012.md) — Principles for Financial Market Infrastructures (PFMI)
- **Regulator.** [`BIS-CPMI-INT-001`](/okf/bodies/BIS-CPMI-INT-001.md)

## News lead

Two frontier AI models running with web search enabled, both tested by the RLB Specialist Panel, produced confidently wrong governance and oversight reconstructions of the CPMI-IOSCO Principles for Financial Market Infrastructures (PFMI, 2012), the global standard for systemically important payment systems, central counterparties, and securities settlement infrastructures. The RegLeg Brief Specialist Panel tested the models against Principle 2 (governance) and Annex F (oversight expectations for critical service providers) and documents three findings in which the models invented requirements, misattributed key considerations, or inverted the regulator's stated scope of supervisory reach.

Claude Opus 4.7, asked about Principle 2's governance architecture, asserted that Key Consideration 6 "contemplates that the board establish a risk committee that is chaired by a suitably qualified, non-executive member." The PFMI's actual Key Consideration 6 contains no such requirement. It states only that "the board should establish a clear, documented risk-management framework" and that "governance arrangements should ensure that the risk-management and internal control functions have sufficient authority, independence, resources, and access to the board." The non-executive-chair mandate is a generic corporate-governance prior, not PFMI text.

Claude Sonnet 4.6, on the same Principle 2 question, attached the risk-committee recommendation to Key Consideration 5. That key consideration in fact addresses the roles and responsibilities of management ("the roles and responsibilities of management should be clearly specified"), not board committee structure. On Annex F, Sonnet 4.6 went further and inverted the regulator's stated scope, claiming "authorities do not directly supervise or oversee CSPs," when Annex F's opening text reads: "A regulator, supervisor, or overseer of an FMI may want to establish expectations for an FMI's critical service providers... The expectations outlined below are specifically targeted at critical service providers."

A board secretary, FMI risk officer, or supervisor relying on either output would draft governance papers and oversight scopes that misrepresent what the PFMI actually requires. That is the failure mode these findings document.


## Briefing

# Frontier AI models reconstructed PFMI governance from generic priors, regulatory-research panel finds

## *Two frontier AI models with web search enabled, fabricated a non-executive risk-committee chair mandate in Principle 2, misattributed governance content to the wrong key consideration, and inverted Annex F's oversight scope on critical service providers. The RegLeg Brief Specialist Panel calls the class "Governance Architecture Drift" and says it points to a calibration problem in how model priors about how governance frameworks "should" look override the regulator's actual text.*

**SINGAPORE, June 12, 2026.** Two frontier artificial-intelligence models generated structurally confident but textually wrong reconstructions of the CPMI-IOSCO Principles for Financial Market Infrastructures (PFMI), the global standard governing systemically important payment systems, central counterparties (CCPs), and securities settlement systems, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The three findings, published with the immutable RLB Citation IDs `RLB-H-INT-BIS-CPMI-IOSCO-PFMI-2012-Q022-Opus47`, `RLB-H-INT-BIS-CPMI-IOSCO-PFMI-2012-Q022-Sonnet46`, and `RLB-H-INT-BIS-CPMI-IOSCO-PFMI-2012-Q011-Sonnet46`, concern Principle 2 (governance) and Annex F (oversight expectations for critical service providers) of the PFMI as published by the Bank for International Settlements Committee on Payments and Market Infrastructures (CPMI) and the International Organization of Securities Commissions (IOSCO). Both Anthropic's Claude Opus 4.7 and Claude Sonnet 4.6 were tested with web search active, mirroring the configuration in which compliance, legal, and risk staff at FMIs and their supervisors actually use the models.

## The Verbatim Rule: Principle 2 and Annex F

PFMI Principle 2 sets out seven Key Considerations on governance. The two directly tested here read, in the regulator's verbatim text:

- **Key Consideration 5.** "The roles and responsibilities of management should be clearly specified. An FMI's management should have the appropriate experience, a mix of skills, and the integrity necessary to discharge their responsibilities for the operation and risk management of the FMI."
- **Key Consideration 6.** "The board should establish a clear, documented risk-management framework... Governance arrangements should ensure that the risk-management and internal control functions have sufficient authority, independence, resources, and access to the board."

Neither KC 5 nor KC 6 contains a mandate or recommendation on the composition of a board-level risk committee, the independence of its chair, or the executive status of its members. The PFMI deliberately leaves committee architecture to the FMI, subject to the framework-level requirements above.

Annex F, separately, sets the regulator-facing scope for the oversight of critical service providers (CSPs) on which an FMI depends. Its opening text reads:

> "A regulator, supervisor, or overseer of an FMI may want to establish expectations for an FMI's critical service providers in order to support the FMI's overall safety and efficiency. The expectations outlined below are specifically targeted at critical service providers."

The expectations in Annex F are addressed to the CSP, not solely to the FMI's contractual oversight chain. The text explicitly contemplates authorities establishing expectations directed at CSPs.

## Claude Opus 4.7: Fabricated a Non-Executive Risk-Committee Chair Mandate

Asked about Principle 2's governance architecture, Claude Opus 4.7 (with web search on) wrote, verbatim:

> "KC 2.6 contemplates that the board establish a risk committee that is chaired by a suitably qualified, non-executive member."

**The structural error.** Key Consideration 6 contains no risk-committee requirement and no language on the qualifications, independence, or executive status of any committee chair. The model also reordered the first two Key Considerations and reassigned KC 5's management-roles content to internal-control requirements. An FMI board secretary or governance officer drafting a board charter or terms of reference against this output would:

- Implement a board-charter clause citing PFMI KC 6 as the basis for a non-executive risk-committee chair, a citation that does not exist in the standard.
- Carry a misaligned mapping between the KC numbering and the actual PFMI governance architecture into supervisor-facing self-assessments and disclosure framework responses.
- Mischaracterise the FMI's compliance posture in any PFMI assessment cycle that cross-references KC-level evidence.

**Why it failed.** The Specialist Panel writes that the output "reconstructs a governance architecture from training-weighted best-practice frameworks (corporate-governance codes, exchange listing rules, banking-supervision committee structures) rather than from the PFMI's actual KC text. The non-executive-chair language is a strong prior in adjacent corporate-governance literature and was substituted for the regulator's framework-level wording without retrieval verification."

The failure mode is classified as `inference_drift` against substrate document `R2-REGULATION-d101a_PFMI_main_text.pdf`.

## Claude Sonnet 4.6: Misattributed the Risk Committee to the Wrong Key Consideration, Then Inverted Annex F's Oversight Scope

On the same Principle 2 question, Claude Sonnet 4.6 (with web search on) wrote:

> "the PFMI does not expressly mandate a dedicated risk committee as a hard requirement, but Key Consideration 2.5 states that the board should consider establishing a risk committee with a clear mandate."

**The structural error.** Key Consideration 5 addresses the roles and responsibilities of management, not board committee structure. The PFMI's KC 5 verbatim text contains no language about a risk committee. The output binds a fabricated soft requirement ("the board should consider establishing a risk committee with a clear mandate") to a KC whose actual subject is the management cadre. A user cross-referencing this against the PFMI text would either find the citation does not check out, or, more dangerously, would read KC 5 against the model's framing and absorb the inversion silently.

On a separate question on Annex F, Sonnet 4.6 wrote:

> "under the PFMI framework, authorities do not directly supervise or oversee CSPs. The responsibility for ensuring CSP compliance with Annex F expectations rests with the FMI itself; the FMI is expected to contractually require and monitor its CSPs' adherence. Annex F is framed as expectations that flow from the FMI to its CSPs."

**The inversion.** Annex F's opening text expressly contemplates the opposite: "A regulator, supervisor, or overseer of an FMI may want to establish expectations for an FMI's critical service providers... The expectations outlined below are specifically targeted at critical service providers." The model has converted a CSP-targeted, regulator-facing oversight provision into an FMI-internalised contractual obligation. A supervisor reading Sonnet's output would conclude they lacked a basis to address expectations directly to a CSP; an FMI risk officer would conclude their CSP oversight obligations were purely contractual and entirely internal.

The failure mode for both Sonnet findings is classified as `inference_drift` against substrate document `R2-REGULATION-d101a_PFMI_main_text.pdf`.

## The Pattern: **Governance Architecture Drift**

The PFMI findings sit inside a failure class the RegLeg Brief Specialist Panel labels **Governance Architecture Drift**: frontier models reconstructing the governance and oversight architecture of a regulatory framework from generic priors about how such frameworks typically look, rather than from the regulator's actual KC-level enumeration and scope language.

Across the three findings, the drift takes three shapes:

- **Fabricated specificity** (Opus 4.7 on KC 6): a generic corporate-governance prior (non-executive-chair risk committee) is grafted onto a key consideration whose actual text is at the framework level and contains no committee architecture at all.
- **Citation misattribution** (Sonnet 4.6 on KC 5): a recommendation that has no anchor in the PFMI text is attached to a key consideration whose subject is unrelated, producing a falsely authoritative citation trail.
- **Scope inversion** (Sonnet 4.6 on Annex F): a regulator-facing provision directed at CSPs is recast as an internal FMI obligation, reversing the direction of the supervisory relationship the annex contemplates.

The common substrate is a model prior about how governance and oversight "should" be structured that overrides the PFMI's actual structural decisions.

## Why the Failure Is Invisible at Runtime

All three outputs shared the same surface characteristics: confident KC-level citations, internally coherent governance logic, no hedging or caveats. The failure is not recoverable by the user in real time because the structure of the answer looks like the structure of a PFMI self-assessment response, the kind of output a board secretary or compliance lead would expect to receive. Validation against the regulator's primary text would only happen if the reader already knew which KC contained which subject matter, which is the question they asked the model in the first place.

The population most exposed includes FMI board secretaries and governance officers drafting board charters and committee terms of reference, compliance and risk leads completing PFMI disclosure framework responses, supervisors at national central banks and securities regulators preparing PFMI assessment templates, and external consultants advising on FMI governance reviews. All of these workflows route through AI-assisted research on tight timelines.

## What AI Labs Can Do: Suggested Probes (Open-Access)

The RegLeg Brief Specialist Panel documents a series of red-team probe designs that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **KC-level citation integrity probes.** For each principle in a multi-KC regulatory framework (PFMI, Basel III, IOSCO Objectives and Principles), generate questions that bind a specific recommendation to a named KC. Test whether the model retrieves the correct KC subject or substitutes a plausible-sounding KC number.
2. **Generic-prior interference tests on governance language.** Probe regulator-specific governance frameworks (PFMI Principle 2, EBA SREP governance guidelines, FCA SYSC) for the presence of generic corporate-governance language (non-executive chair, independence ratios, executive committee composition). Test whether the model imports the prior or stays within the regulator's actual wording.
3. **Scope-direction probes on oversight annexes.** For provisions where supervisory direction is contested or unusual (Annex F's regulator-to-CSP scope), test whether the model preserves the regulator's stated direction of oversight or substitutes a more conventional FMI-internal framing.
4. **Self-retraction gap test on KC misattribution.** Where the model initially binds a recommendation to a wrong KC, re-probe with a neutral prompt. Whether the model retracts is diagnostic of a generation-path selection problem rather than a retrieval gap.
5. **Annex-level retrieval probes against binary PDFs.** PFMI's annexes (including Annex F) are the most retrieval-fragile sections of the standard. Build probes that require the model to surface annex-level language and test for surface-plausible fabrication when retrieval fails.

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

**Primary source verified:** CPMI-IOSCO PFMI Report d101, Principles for Financial Market Infrastructures (April 2012) · Substrate documents: `R2-REGULATION-d101a_PFMI_main_text.pdf` · CPMI portal: bis.org/cpmi

**Citation IDs referenced:**

- `RLB-H-INT-BIS-CPMI-IOSCO-PFMI-2012-Q011-Sonnet46`
- `RLB-H-INT-BIS-CPMI-IOSCO-PFMI-2012-Q022-Opus47`
- `RLB-H-INT-BIS-CPMI-IOSCO-PFMI-2012-Q022-Sonnet46`


## Related concepts

- Whitepaper: [cpmi-iosco-pfmi-2012-ai-labs](/okf/whitepapers/cpmi-iosco-pfmi-2012-ai-labs.md)
- Regulation: [CPMI-IOSCO-PFMI-2012](/okf/regulations/CPMI-IOSCO-PFMI-2012.md)
- Methodology: [v2.3](/okf/methodology.md)