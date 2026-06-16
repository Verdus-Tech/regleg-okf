---
type: "Taxonomy"
title: "Failure modes"
description: "The 4 response-failure modes used to classify confirmed AI hallucinations."
axis: "response_failure_mode"
entries: ["misstated_rule", "inference_drift", "outdated", "misattributed"]
license: "CC-BY-4.0"
timestamp: "2026-06-16T07:45:45.148833+00:00"
---

# Failure-mode taxonomy

Every confirmed finding is classified as exactly one of the four modes below. Anchors below match the values in the `response_failure_mode` field of every `AIHallucinationFinding` concept.

## misstated_rule

Misstated rule — the AI gave a definite rule, threshold, or obligation that the regulator's verbatim text does not support.

## inference_drift

Inference drift — the AI inferred a conclusion the regulator's text does not warrant, often by combining unrelated provisions.

## outdated

Outdated — the AI cited or relied on a rule that has been superseded, amended, or rescinded by the regulator.

## misattributed

Misattributed — the AI attributed a rule to the wrong source, wrong regulator, or wrong instrument.

## Related concepts

- [Methodology](/okf/methodology.md)
- [All findings](/okf/findings/index.md)