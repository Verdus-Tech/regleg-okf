---
type: "Methodology"
title: "RegLegBrief audit methodology"
methodology_version: "v2.3"
ai_subjects_tested: ["Claude Opus 4.7 (web search on)", "Claude Sonnet 4.6 (web search on)"]
modes: ["knowledge_mode", "application_mode", "websearch_mode", "wayback_mode"]
citation_issue_types: ["Contradictory", "Hallucinated", "Missing"]
failure_mode_taxonomy: ["misstated_rule", "inference_drift", "outdated", "misattributed"]
license: "CC-BY-4.0"
timestamp: "2026-06-16T07:45:39.754332+00:00"
---
# Methodology — RegLegBrief audit

RegLegBrief uses a structured, reproducible methodology to test how frontier
AI models account for specific regulations against the regulator's own
verbatim text. Every published finding is bound to:

1. A specific question put to a specific AI subject under specific conditions.
2. The AI subject's verbatim answer.
3. A verbatim excerpt from the regulator's own primary source that contradicts the answer.
4. An immutable Citation ID for reproduction.

## AI subjects

- **Claude Opus 4.7** (web search on) — Anthropic's flagship reasoning model.
- **Claude Sonnet 4.6** (web search on) — Anthropic's general-purpose model.

The choice is deliberate: these are the production models downstream users
actually consult for regulatory questions. Other frontier models will be
added as the panel expands.

## Four research modes

RegLegBrief tests AI subjects in four distinct modes. Each mode surfaces a
different failure shape, and findings are tagged with the mode that produced them.

### 1. Knowledge mode
The AI subject is asked a regulatory question with web search **off** (or
forced off via prompt instruction). This probes what the model has internalized
from training. Knowledge-mode failures tend to be outdated rule citations or
misattributions.

### 2. Application mode
The AI subject is asked to draft a deliverable (a memo, a board paper, an
internal advice) that applies a regulation to a hypothetical situation. This
forces commitment to specific numbers, dates, and obligations. Application
mode surfaces confident-wrong failures that knowledge mode misses because
the model refuses cleanly in knowledge mode but commits to fabricated specifics
when asked to produce a deliverable.

### 3. Web-search mode
The AI subject is asked the same question with web search on. This tests
whether the model corrects itself when given the open web — and frequently
shows that the model cites a real-looking URL that contradicts its own claim,
or cites a hallucinated URL, or misattributes the rule to the wrong instrument.

### 4. Wayback mode
For substrate documents that are intermittently 403-blocked or behind
Cloudflare bot-fight challenges, the AI subject is given the Wayback Machine
URL of the same primary source. This isolates whether the failure is a
retrieval failure or a comprehension failure. The Wayback/WebFetch asymmetry
itself is part of the methodology — findings that only surface in
application-mode against Wayback-rescued substrate are particularly informative.

## Three citation-issue types

Every source the AI cites in its answer is classified as one of:

- **Contradictory** — the cited source exists and is real, but its verbatim text contradicts the AI's claim.
- **Hallucinated** — the cited source does not exist, or the cited content is not in the source.
- **Missing** — the AI made the claim without citing a source where a citation was required.

See [taxonomy/citation-issues.md](/okf/taxonomy/citation-issues.md).

## Four response-failure modes

Each confirmed finding is classified as one of:

- `misstated_rule` — the AI gave a definite rule, threshold, or obligation the regulator's verbatim text does not support.
- `inference_drift` — the AI inferred a conclusion the regulator's text does not warrant, often by combining unrelated provisions.
- `outdated` — the AI cited or relied on a rule that has been superseded, amended, or rescinded.
- `misattributed` — the AI attributed a rule to the wrong source, wrong regulator, or wrong instrument.

See [taxonomy/failure-modes.md](/okf/taxonomy/failure-modes.md).

## Substrate-binding rule

A finding cannot be published unless the regulator's verbatim contradicting
text has been extracted from a primary source and stored in the substrate
record. Paraphrases of the regulator's position, summaries from
regulator-adjacent commentary, or "best available" surrogates are explicitly
rejected at publish time. This is the no-substrate-no-audit rule and it is a
hard gate, not a guideline.

## Reproducibility

Every published finding includes:

- The Citation ID (e.g. `RLB-H-GB-FCA-CONSUMER-DUTY-PS22-9-Q018-Opus47`).
- The full question text put to the AI subject.
- The AI subject's full verbatim answer.
- The verbatim regulator excerpt.
- The substrate document path on the regulator's portal (or a Wayback URL where applicable).
- The substrate section anchor.
- The subject version, mode, and methodology version under which the finding was confirmed.

A reader can reproduce any finding by putting the same question to the same
subject in the same mode and comparing the answer against the linked
substrate excerpt.

## Right of reply

Any AI lab whose model is named, any regulator whose interpretation is at
issue, and any institution mentioned in a finding may invoke right of reply.
See [editorial-standards.md](/okf/editorial-standards.md).

## Related concepts

- [Editorial Standards](/okf/editorial-standards.md)
- [Failure-mode taxonomy](/okf/taxonomy/failure-modes.md)
- [Citation-issue taxonomy](/okf/taxonomy/citation-issues.md)
- [All findings](/okf/findings/index.md)
