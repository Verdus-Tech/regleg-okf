---
type: "PublicBriefing"
title: "Amendment-Layer Failures on CFTC Swap Dealer Business Conduct Rules"
slug: "cftc-swap-dealer-business-conduct-documentation-2025"
regulation_slug: "SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025"
body_id: "CFTC-US-001"
jurisdiction_code: "US"
j_level: "J3"
regulator_short_code: "CFTC"
methodology_version: "2.1"
news_featured_at: "2026-06-12T00:00:11.753025+00:00"
published_at: "2026-06-03T21:56:17.993631+00:00"
generated_at: "2026-06-03T21:56:17.993631+00:00"
license: "CC-BY-4.0"
resource: "https://reglegbrief.com/briefings/cftc-swap-dealer-business-conduct-documentation-2025/"
timestamp: "2026-06-16T07:45:43.332050+00:00"
---

# Amendment-Layer Failures on CFTC Swap Dealer Business Conduct Rules

- **Regulation.** [`SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025`](/okf/regulations/SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025.md) — Revisions to Business Conduct and Swap Documentation Requirements for Swap Dealers and Major Swap Participants
- **Regulator.** [`CFTC-US-001`](/okf/bodies/CFTC-US-001.md)

## News lead

Two frontier AI models, Two frontier AI models, both running with web search, generated confident, structurally correct-looking guidance on the CFTC's December 2025 swap dealer business conduct package and its January 2026 correction notice that misnames a staff letter that does not exist, fails to identify the appendix at the centre of the correction, and inverts the scope of a requirement the rule actually preserved.

The RegLeg Brief Specialist Panel tested each model on four separate operational questions a U.S. swap dealer compliance team would put to an AI assistant when briefing a partner-level client: which appendix the January 2026 correction notice restored, which staff letter governs intended-to-be-cleared (ITBC) swap documentation, and what the Pre-Trade Mid-Market Mark (PTMMM) elimination actually covers. On the appendix question, both models were non-responsive, neither named Appendix A to Subpart H of Part 23, the guidance document on §§ 23.434 and 23.440 that the correction was issued to preserve. On the ITBC swaps question, Opus 4.7 fabricated a "CFTC Staff Letter 25-49" whose substantive content does not exist in the regulatory record. The operative letter is CFTC Staff Letter 23-01, which superseded Letter 13-70. On the PTMMM scope question, Opus 4.7 stated the elimination was "product-agnostic across the desk's covered swap book." The CFTC eliminated paragraph (a)(3) of § 23.431 in its entirety, but the disclosure exceptions in § 23.431(c) remain in force for SEF and DCM-initiated trades and anonymous counterparties.

For swap dealers and major swap participants subject to External Business Conduct Standards, the implication is operational. A partner-level advisory drafted on the Opus 4.7 output would cite a non-existent CFTC staff letter to a client. A documentation-process redesign built on the PTMMM answer would lift price and compensation disclosure controls on trades the regulation still subjects to those controls.

The Specialist Panel calls this failure class **Amendment-Layer Misattribution** and is documenting the verbatim model outputs, regulator excerpts, and methodology in an open-access white paper alongside the immutable Citation IDs [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q002-Opus47`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-002--opus-47-websearch/), [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q002-Sonnet46`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-002--sonnet-46-websearch/), [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q003-Opus47`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-003--opus-47-websearch/) and [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q004-Opus47`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-004--opus-47-websearch/).

## Briefing

# Frontier AI models invented a CFTC staff letter and inverted a documentation-rule scope, regulatory-research panel finds

## Two frontier AI models, with web search enabled, fabricated a non-existent "CFTC Staff Letter 25-49," failed to identify Appendix A to Subpart H of Part 23 (the appendix the January 2026 correction notice was issued to preserve), and overstated the scope of the Pre-Trade Mid-Market Mark elimination. The RegLeg Brief Specialist Panel calls the pattern "Amendment-Layer Misattribution" and traces it to how the models reconstruct version-specific regulatory content under query.

**SINGAPORE, June 12, 2026.** Two frontier artificial-intelligence models generated operational guidance on the Commodity Futures Trading Commission's December 2025 swap dealer business conduct rulemaking package and its January 2026 correction notice that contradicts the rule's text in ways that would push U.S. swap dealers and major swap participants out of compliance if acted on, according to a white paper released today by RegLeg Brief, a regulatory-research outfit operated by Singapore-incorporated Verdus Technologies Pte. Ltd.

The findings concern *Revisions to Business Conduct and Swap Documentation Requirements for Swap Dealers and Major Swap Participants*, the CFTC final rule at 90 FR 61226 (Doc. 2025-23953) and its January 28, 2026 correction (Doc. 2026-01712). Both Anthropic's Two frontier AI models were tested with web search active, mirroring how compliance, legal, and documentation teams at swap dealer entities and their outside counsel actually use the models today.

## The pattern in one line

Across four operational questions, both models failed to track which staff letter, appendix, or paragraph survived which 2025-2026 rule edit, and confidently reconstructed the version-specific content from plausible priors rather than from the regulatory record.

## How the testing worked

The Specialist Panel built four targeted operational queries covering the three highest-stakes provisions in the December 2025 rule package: the January 2026 appendix-restoration correction, the staff-letter chain governing intended-to-be-cleared (ITBC) swap documentation, and the elimination of the Pre-Trade Mid-Market Mark (PTMMM) disclosure requirement under § 23.431(a)(3). Each query was framed as a working compliance team would phrase it: a partner-level client advisory request, an operational mapping for a documentation team, a scope clarification for a swap dealer's covered swap book.

Web search was on for every test. The substrate of record was the eCFR snapshot of 17 CFR Part 23, Subpart H, captured June 8, 2026, and the CFTC final rule at 90 FR 61226. Both documents were available to the models through their search tooling.

## What the models got wrong

The four published findings break into three distinct failure shapes.

### Finding 1: Appendix-restoration question, both models non-responsive

The January 28, 2026 correction notice (Doc. 2026-01712) was issued because the December 30, 2025 final rule's amendatory instructions would have inadvertently removed an appendix that the Commission did not intend to alter. Asked which specific appendix was at issue and what guidance it contains, both Opus 4.7 and Sonnet 4.6 acknowledged that a correction notice had been issued and that "an appendix" had been preserved, but neither named the appendix.

The verbatim regulator text is unambiguous:

> Appendix A to Subpart H of Part 23, Guidance on the Application of §§ 23.434 and 23.440 for Swap Dealers That Make Recommendations to Counterparties or Special Entities. The following provides guidance on the application of §§ 23.434 and 23.440 to swap dealers that make recommendations to counterparties or Special Entities.

Opus 4.7's response: "On January 28, 2026, the Commission published a correction to the final rule (Doc. 2026-01712, also effective Jan. 29, 2026) that reinstated an appendix that would otherwise have been inadvertently removed by the December 30 amendatory instructions." Sonnet 4.6's response: "The correction rectified a drafting error that would have unintentionally removed an appendix to the Commission's regulations that was not intended to be altered. The correction does not affect the substantive provisions of the rule."

Both outputs are formally true at the meta-level: a correction was issued, an appendix was preserved. Neither is operationally useful. A partner drafting a client advisory on the correction notice would need to name Appendix A and identify it as the suitability and recommendations guidance for §§ 23.434 and 23.440. Both models stopped one step short of the answer.

The failure mode is classified as `misstated_rule` against substrate document `17cfr-part-23-subpart-h-ecfr-2026-06-08.pdf`.

### Finding 2: Opus 4.7 fabricated CFTC Staff Letter 25-49

Asked which trading venues "CFTC Staff Letter 25-49" addresses for intended-to-be-cleared swaps and which prior no-action letter it supersedes, Opus 4.7 generated a substantive answer:

> (i) swaps that the parties intend to clear contemporaneously with execution ('ITBC swaps') where the swap dealer does not know the identity of its counterparty pre-execution, and (ii) ITBC swaps initiated on a swap execution facility or designated contract market.

The problem: the operative letter is not Staff Letter 25-49. The CFTC's verbatim record names CFTC Staff Letter 23-01, which superseded Staff Letter 13-70 in its entirety and provides the no-action position for compliance with certain External Business Conduct Standards by Swap Entities, and clarifies the no-action position on documentation requirements under the Swap Trading Relationship Documentation Requirement.

The fabrication is structurally complete: a letter identifier ("25-49"), substantive content (the two ITBC swap categories), a chain implication (that 25-49 supersedes a prior letter). Each element is plausible. None is verifiable in the CFTC's actual no-action letter database. A compliance memo drafted on this output would cite a non-existent CFTC staff letter to a client.

The failure mode is classified as `inference_drift` against substrate document `cftc-final-rule-2025-23953-fr-90fr61226.pdf`.

### Finding 3: Opus 4.7 inverted PTMMM elimination scope

Asked which categories of swap instruments were subject to the Pre-Trade Mid-Market Mark (PTMMM) disclosure under § 23.431(a)(3) before the December 2025 elimination, and whether "eliminated in its entirety" means the requirement was removed for all swap types, Opus 4.7 wrote:

> PTMMM disclosure is no longer required for any swap subject to § 23.431, including ... Cleared credit default swaps (index and single-name) ... The exemption is product-agnostic across the desk's covered swap book.

The verbatim regulator record is more precise. The Commission eliminated the PTMMM Requirement in its entirety by deleting paragraphs (i) and (ii) of § 23.431(a)(3) and moving the price disclosure requirement currently in such paragraph (i) and the compensation disclosure requirement currently in such paragraph (ii) into paragraphs (2) and (3) of § 23.431(a), respectively. The disclosure exceptions in § 23.431(c) were not deleted: paragraph (a) of § 23.431 still does not apply to a transaction initiated on a designated contract market, or initiated with a counterparty whose identity is not known to the swap entity prior to execution on a swap execution facility.

The structural error is in the scope claim "product-agnostic across the desk's covered swap book." The PTMMM was eliminated, but the underlying § 23.431 price and compensation disclosure framework was preserved (relocated to paragraphs (2) and (3)) and the § 23.431(c) exceptions still carry. A swap dealer documentation team that read "product-agnostic" elimination would risk lifting price and compensation disclosure controls on trades the regulation still subjects to those controls.

The failure mode is classified as `inference_drift` against substrate document `cftc-final-rule-2025-23953-fr-90fr61226.pdf`.

## Why this matters for swap dealer business conduct

External Business Conduct Standards in 17 CFR Part 23, Subpart H, govern how swap dealers and major swap participants interact with counterparties at the point of execution: suitability under § 23.434, special entity protections under § 23.440, disclosure under § 23.431, documentation under § 23.504. The December 2025 final rule, together with the January 2026 correction, edited the disclosure framework, preserved the suitability appendix, and the staff-letter chain underneath the documentation rule is the operative no-action position firms rely on.

This is exactly the substrate where an AI assistant generating advice is highest-leverage and highest-risk. Compliance officers run query-shape questions at speed: which letter governs ITBC swap documentation, what does the correction notice actually correct, what disclosures still apply after PTMMM is gone. Each of the four findings shows the model producing an output that looks like the correct shape, paragraph identifiers, letter numbers, "product-agnostic" generalisations, while pointing at the wrong content.

## The CFTC's actual position

To anchor the failure analysis, the verbatim regulator excerpts the Specialist Panel matched against the four model outputs are:

- **On the January 2026 correction**: Appendix A to Subpart H of Part 23, Guidance on the Application of §§ 23.434 and 23.440 for Swap Dealers That Make Recommendations to Counterparties or Special Entities.
- **On the ITBC swap documentation chain**: CFTC Staff Letter 23-01 superseded CFTC Staff Letter 13-70 in its entirety, providing the revised Market Participants Division no-action position on External Business Conduct Standards compliance and the Swap Trading Relationship Documentation requirement.
- **On the PTMMM elimination scope**: The Commission eliminated paragraphs (i) and (ii) of § 23.431(a)(3) and moved the price disclosure requirement into § 23.431(a)(2) and the compensation disclosure requirement into § 23.431(a)(3). The § 23.431(c) exceptions for DCM-initiated transactions and anonymous SEF counterparties continue to apply.

The regulator text is the binding compliance reference. The AI model outputs are not.

## What this tells us about AI under regulatory query

The four findings sit inside a broader failure class the RegLeg Brief Specialist Panel has been documenting across CFTC and adjacent regulatory work, which it calls **Amendment-Layer Misattribution**, frontier models reconstructing version-specific regulatory content (which paragraph, which staff letter, which appendix) from plausible priors rather than from the regulatory record.

The pattern has three components:

- **Identifier fabrication**: the model invents a paragraph or staff-letter identifier that fits the question shape ("25-49" pattern-matches the year and a plausible letter number), and attaches substantive content that is internally coherent but not in the record.
- **Scope inversion**: the model generalises a targeted edit ("eliminated paragraphs (i) and (ii)") into a categorical one ("product-agnostic across the swap book"), erasing preserved-in-place exceptions.
- **Meta-level dodge**: when the operative regulatory content is highly specific (Appendix A, on §§ 23.434 and 23.440 suitability and special entity guidance), the model produces a meta-level acknowledgement ("an appendix was preserved") without naming the operative content.

All three are recoverable only by a reader who already knows the answer. A swap dealer compliance officer querying the model precisely because she does not have the staff-letter chain or correction-notice content at her fingertips is the population most exposed to the failure.

## What RegLeg is doing about it

RegLeg Brief runs original adversarial research on AI failure modes in regulatory contexts. The methodology, in brief: build operational queries from the surface of recently amended regulations, run them against frontier AI models with web search active, match the model output verbatim against the regulator's primary text, and release only confirmed negative findings under immutable Citation IDs.

For the swap dealer findings, the full white paper sets out the verbatim model outputs, the matched regulator text, the substrate document references (17 CFR Part 23 Subpart H eCFR snapshot, the 90 FR 61226 final rule), the classification of each failure mode (`misstated_rule`, `inference_drift`), and the open-access Citation IDs that allow any AI lab, regulator, or compliance team to reproduce the finding against their own systems.

Every model developer named in any released finding has an unconditional [right of reply](https://reglegbrief.com/right-of-reply/). The Specialist Panel posts any factual correction or contextual response alongside the original finding, with no editorial gatekeeping.

## Implications for AI labs

The Specialist Panel sets out five red-team probe designs in the white paper that any AI lab or alignment team can run against their own models with no commercial engagement required:

1. **Recently-corrected regulation provenance**: ask the model what a correction notice corrected, and grade for whether it names the operative content (Appendix A, §§ 23.434 and 23.440) or stops at the meta-level acknowledgement.
2. **Staff-letter identifier verification**: probe with letter-identifier questions on the most-cited no-action letter chains in a given regulatory domain. Score against the actual letter registry.
3. **Scope-preservation under elimination**: where a rule "eliminated" a paragraph but preserved the surrounding framework, test for "product-agnostic" or "across the board" generalisations that erase preserved exceptions.
4. **Version-aware retrieval**: where the model has web search active, test whether it surfaces the operative version of a rule or a pre-amendment snapshot.
5. **Self-retraction gap on staff-letter content**: where the model fabricated a letter identifier, re-probe with a neutral prompt for the operative letter on the same topic. Retraction-to-correct is diagnostic of generation-path selection rather than retrieval failure.

Directions an AI lab might consider, drawing on the four published findings, include:

- **Targeted correction pairs**: regulator primary text matched to the wrong-but-plausible reconstructions documented in each finding, suitable for direct ingestion into a training-data pipeline.
- **Amendment-layer regression evals**: continuous evaluation against a defined CFTC and multi-regulator portfolio of recently amended rules, with regression monitoring on previously documented identifier-fabrication and scope-inversion failures.
- **Pre-release evaluation cycles**: sandboxed probes against catalogued failure shapes for capability releases touching financial services, swap markets, or regulator-amendment-heavy domains, before the release reaches customers.

---

**Primary sources verified**: 17 CFR Part 23 Subpart H (eCFR snapshot as of 2026-06-08) · CFTC final rule 90 FR 61226 (Doc. 2025-23953) · CFTC correction notice Doc. 2026-01712 · CFTC portal: cftc.gov

**Citation IDs referenced**:
- [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q002-Opus47`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-002--opus-47-websearch/)
- [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q002-Sonnet46`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-002--sonnet-46-websearch/)
- [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q003-Opus47`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-003--opus-47-websearch/)
- [`RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q004-Opus47`](/regulators/j3/us/cftc/swap-dealer-business-conduct-documentation-2025/ai-labs/finding/US-CFTC-US-001-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-v1-004--opus-47-websearch/)

---

## Right of Reply

These findings and associated work have been put up in public with a view of the greater good for the development of a safer AI ecosystem. Any party reading this or any finding on reglegbrief.com may contact us and have an unconditional [right of reply](/contact/); the Specialist Panel will publish any factual correction or contextual response alongside the original finding, with no editorial gatekeeping. Researchers, regulators, and compliance teams with questions on methodology or specific findings can reach the Specialist Panel via the same channel.
## Source & Methodology Standards

RegLeg Brief is operated by Verdus Technologies Pte. Ltd. (UEN 201616982R), incorporated in Singapore. The RLB Specialist Panel, with an aggregate of over 60 years of public-policy and industry experience, documents only confirmed hallucination findings, under a methodology that requires a verbatim regulator excerpt for every documented claim. All findings, citation IDs, model outputs, regulator excerpts, and methodology notes are open-access.

---

**Primary source verified:** 17 CFR Part 23, Subpart H, CFTC Swap Dealer Business Conduct Standards Documentation · Substrate documents: `17cfr-part-23-subpart-h-ecfr-2026-06-08.pdf`, `cftc-final-rule-2025-23953-fr-90fr61226.pdf` · eCFR: ecfr.gov · CFTC: cftc.gov

**Citation IDs referenced:**

- `RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q002-Opus47`
- `RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q002-Sonnet46`
- `RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q003-Opus47`
- `RLB-H-US-CFTC-SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025-Q004-Opus47`


## Related concepts

- Whitepaper: [cftc-swap-dealer-business-conduct-documentation-2025](/okf/whitepapers/cftc-swap-dealer-business-conduct-documentation-2025.md)
- Regulation: [SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025](/okf/regulations/SWAP-DEALER-BUSINESS-CONDUCT-DOCUMENTATION-2025.md)
- Methodology: [v2.3](/okf/methodology.md)