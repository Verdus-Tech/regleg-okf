---
type: "Index"
title: "RegLegBrief OKF Bundle"
description: "Google Open Knowledge Format (v0.1) machine-readable bundle of RegLegBrief content. Each concept is one Markdown file with YAML frontmatter."
okf_spec_version: "0.1"
publisher: "Verdus Technologies Pte. Ltd."
publication: "RegLegBrief"
publication_url: "https://reglegbrief.com"
license: "CC-BY-4.0"
primary_language: "en"
timestamp: "2026-06-16T00:00:00+00:00"
---
# RegLegBrief — Open Knowledge Format bundle

This is the machine-readable bundle of every concept RegLegBrief publishes,
conformed to the Google **Open Knowledge Format (OKF) v0.1** spec. The bundle
is database-driven and rebuilds automatically as new content lands.

Spec: https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf

## Top-level concepts

- [Publisher](/okf/about.md) — who publishes this bundle, legal entity, jurisdiction
- [Methodology](/okf/methodology.md) — how RegLegBrief tests AI subjects and binds findings to verbatim regulator text
- [Editorial Standards](/okf/editorial-standards.md) — what makes a finding ready to publish
- [Taxonomy](/okf/taxonomy/index.md)
    - [Failure modes](/okf/taxonomy/failure-modes.md) — the 4 response-failure modes used to classify hallucinations
    - [Citation issues](/okf/taxonomy/citation-issues.md) — the 3 citation-issue types attached to each finding's cited sources
- [Regulatory bodies](/okf/bodies/index.md) — bodies whose regulations are tested
- [Regulations](/okf/regulations/index.md) — regulations with research_complete status
- [AI hallucination findings](/okf/findings/index.md) — the core: every confirmed delta between AI output and the regulator's verbatim text
- [AI Labs whitepapers](/okf/whitepapers/index.md) — synthesized whitepapers per regulation
- [Public briefings](/okf/briefings/index.md) — news-format briefings published from the same finding set

## Change log

- [log.md](/okf/log.md) — chronological list of publish events

## Bundle layout

```
/okf/
├── index.md            (this file)
├── log.md
├── about.md            (Publisher)
├── methodology.md      (Methodology)
├── editorial-standards.md  (EditorialPolicy)
├── taxonomy/
│   ├── index.md
│   ├── failure-modes.md
│   └── citation-issues.md
├── bodies/
│   ├── index.md
│   └── <body_id>.md     (RegulatoryBody)
├── regulations/
│   ├── index.md
│   └── <regulation_slug>.md  (Regulation)
├── findings/
│   ├── index.md
│   └── <finding_uid>.md  (AIHallucinationFinding)
├── whitepapers/
│   ├── index.md
│   └── <wp_slug>.md      (AILabsWhitepaper)
└── briefings/
    ├── index.md
    └── <briefing_slug>.md  (PublicBriefing)
```

## Conformance

- OKF spec version: 0.1
- Required field present on every concept file: `type`
- Producer-defined types are namespaced by content domain (e.g. `AIHallucinationFinding`,
  `RegulatoryBody`, `AILabsWhitepaper`); the spec permits arbitrary types since
  only `type` is required.
- Every concept file is served as `Content-Type: text/markdown; charset=utf-8`.
- Cross-links use root-relative Markdown links (`/okf/...`).

## Licensing

All concept files are released under CC-BY-4.0. AI labs and ingestion
pipelines may consume, embed, and cite without prior permission. Commercial
redistribution of the finding set as a derived dataset requires a licence —
contact partnership@reglegbrief.com.

## Last updated

2026-06-16T00:00:00+00:00
