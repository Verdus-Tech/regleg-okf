---
type: "EditorialPolicy"
title: "RegLegBrief editorial standards"
governing_panel: "RLB Specialist Panel"
right_of_reply_window_days: 14
correction_policy: "All corrections logged with original published_at preserved; corrected text appended."
license: "CC-BY-4.0"
timestamp: "2026-06-16T00:00:00+00:00"
---
# Editorial Standards — RegLegBrief

## The four gates a finding must pass before publish

1. **Substrate-bound.** The regulator's verbatim contradicting text is extracted from a primary source and stored in the substrate record. No paraphrases. No regulator-adjacent commentary as substitute. No "best available" surrogates.

2. **Subject-bound.** The AI subject, subject version, mode, and methodology version are all recorded. A finding is reproducible against that exact configuration.

3. **Question-bound.** The exact question put to the AI subject is preserved verbatim. Paraphrasing the question after the fact invalidates the finding.

4. **Failure-mode-classified.** The finding is classified as exactly one of the four response-failure modes (misstated_rule, inference_drift, outdated, misattributed). Findings that don't fit are not published.

## What is NOT published

- Positive findings (where the AI is correct against the regulator's text). RegLegBrief publishes only the delta.
- "Probably wrong" or "appears to misstate" — only findings with verbatim regulator text contradicting the AI's claim.
- Findings where the substrate is paraphrased rather than verbatim.
- Findings classified as cosmetic (synonym substitutions, title formatting) rather than material substantive errors.

## Right of reply

Any AI lab whose model is named, any regulator whose interpretation is at issue, and any institution mentioned in a finding may submit a right-of-reply statement. The window is 14 days from publication. RoR statements are appended to the finding page without altering the original published text, with the date of the RoR.

Submit to: avichal987@gmail.com

## Corrections

Errors are corrected via append, not overwrite. The original `published_at` is preserved; a correction note with timestamp is added. The finding_uid never changes.

## Independence

RegLegBrief receives no funding, sponsorship, or other consideration from AI labs, regulators, or regulated institutions named in its findings.

## Source-of-truth precedence

Where a regulator publishes the same instrument in multiple places (e.g. a press release plus the full text PDF), the full instrument text governs. Press release summaries are not substrate.

## Related concepts

- [Methodology](/okf/methodology.md)
- [Publisher](/okf/about.md)
