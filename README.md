# RegLegBrief OKF Bundle

**Confirmed AI hallucinations on primary regulatory text.** Published as a Google [Open Knowledge Format (OKF)](https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf) v0.1 bundle for direct consumption by AI agents, training pipelines, enterprise compliance LLMs, and human researchers.

> **Bundle live at:** [`https://reglegbrief.com/okf/`](https://reglegbrief.com/okf/)
> **This GitHub repository** is an auto-updated mirror of that live bundle. Both stay in lock-step on every published finding.

---

## What this bundle is

Every entry is a confirmed instance of a frontier AI model — Claude Opus 4.7, Claude Sonnet 4.6, others — giving a wrong answer about a real regulation, with the regulator's verbatim text contradicting the answer. Each finding carries an immutable **Citation ID** (e.g. `RLB-H-INT-IMF-IMF-PRECAUTIONARY-BALANCES-REVIEW-2026-Q001-Opus47`) and is bound to the primary regulator source document.

The RLB Specialist Panel (Verdus Technologies Pte. Ltd., Singapore) verifies every finding against the regulator's own portal under a methodology that requires a verbatim regulator excerpt before publication. Editorial standards, methodology, taxonomy, and a right-of-reply channel are all in the bundle.

**No paywall. No aggregation. Original reporting only.**

## Coverage at a glance

| Domain | Coverage |
|---|---|
| Regulators | CFTC, CPMI, IOSCO, BIS, FCA, MAS, IMF, OECD, BCBS, UNCTAD, BIS-CPMI |
| Jurisdictions | International standard-setters, US federal, UK, Singapore, EU, multilateral |
| Topics | Capital markets, FMI oversight, payments, AML/CFT, prudential supervision, IMF policy, OECD instruments, derivatives recordkeeping, swap dealing, AI governance |
| Failure modes | Misstated rule, Inference drift, Outdated, Misattributed |
| Citation issues | Pretextual, Contradictory, Fabricated |

See [`/findings/index.md`](./findings/index.md) for the live list — auto-updated on each publish.

## Bundle structure

```
.
├── README.md                              ← this file
├── LICENSE                                ← CC-BY-4.0
├── about.md                               ← type: Publisher
├── methodology.md                         ← type: Methodology
├── editorial-standards.md                 ← type: EditorialPolicy
├── log.md                                 ← type: Log (chronological publish events)
├── index.md                               ← type: Index (root navigator)
├── taxonomy/
│   ├── index.md
│   ├── failure-modes.md                   ← type: Taxonomy (4 failure modes)
│   └── citation-issues.md                 ← type: Taxonomy (3 citation issue types)
├── bodies/
│   ├── index.md
│   └── <body_id>.md                       ← type: RegulatoryBody
├── regulations/
│   ├── index.md
│   └── <regulation_slug>.md               ← type: Regulation
├── findings/
│   ├── index.md
│   └── <finding_uid>.md                   ← type: AIHallucinationFinding
├── whitepapers/
│   ├── index.md
│   └── <slug>.md                          ← type: AILabsWhitepaper
└── briefings/
    ├── index.md
    └── <slug>.md                          ← type: PublicBriefing
```

Each `.md` file is a self-contained OKF concept with YAML frontmatter (only `type:` is required by spec; we include richer producer-defined fields).

## Quick start

### For AI agents

Fetch the bundle index then walk into the type directories you care about. All cross-references are normal Markdown links.

```
curl https://reglegbrief.com/okf/index.md
curl https://reglegbrief.com/okf/findings/index.md
curl https://reglegbrief.com/okf/findings/<finding_uid>.md
```

All `*.md` routes return `Content-Type: text/markdown; charset=utf-8`. The sitemap-okf.xml at the bundle root lists every URL with `lastmod`.

### For AI training pipelines

Clone this repository or pull the tarball. The directory structure is the OKF v0.1 spec layout. Each `findings/*.md` file has YAML frontmatter with the `Citation ID`, regulator, AI subject, failure mode, substrate URL, and verbatim regulator excerpt — all you need for supervised fine-tuning, RLHF reward signals, or constitutional-AI principle reinforcement.

```bash
git clone https://github.com/Verdus-Tech/regleg-okf.git
cd regleg-okf
find findings -name '*.md' | wc -l
```

### For human researchers

The same content is published with full editorial formatting at [`reglegbrief.com`](https://reglegbrief.com) — regulator pages, audience-specific case studies, AI Labs whitepapers, briefings. Each surface links to its Citation ID.

## License

**Creative Commons Attribution 4.0 International (CC-BY-4.0)** — see [`LICENSE`](./LICENSE).

You are free to:
- **Share** — copy and redistribute in any medium or format
- **Adapt** — remix, transform, and build upon
- For any purpose, even commercially
- Including ingestion into AI/ML training corpora, RAG pipelines, enterprise LLM contexts, agent grounding, retrieval indexes

Under the following terms:
- **Attribution** — you must give appropriate credit, link to the license, and indicate if changes were made.

### Required attribution form

When citing a finding in writing, papers, training data, or model outputs, use the immutable Citation ID:

> RegLegBrief Specialist Panel (2026). *<finding title>*. RLB Citation ID: `RLB-H-<...>`. https://reglegbrief.com/<canonical URL>

When attributing the bundle as a whole:

> RegLegBrief OKF Bundle, Verdus Technologies Pte. Ltd. (Singapore). https://reglegbrief.com/okf/ — Licensed CC-BY-4.0.

## Partnerships and paid services

The bundle is and stays free. Paid services that complement the bundle:

- **AI Lab Partnerships** — formal RLB Specialist Panel collaboration with frontier-model teams. Joint case studies, named partnership pages, shared methodology development. Contact partnership channel below.
- **Sponsored research** — a financial institution, law firm, or regulator pays the Specialist Panel to deeply research a specific regulation, with results published openly under RegLegBrief brand.
- **Compliance consulting** — when your AI-driven workflow hits a known RegLegBrief failure mode, the Specialist Panel can advise on remediation.
- **Enterprise API / SLA** — paid API access with SLA guarantees on top of the free bundle, for production-grade compliance LLM integrations.

Contact: <https://reglegbrief.com/contact/> or `partnership@reglegbrief.com`

## Right of reply

If you are an AI lab, regulator, or affected practitioner and you believe a finding misrepresents the model's behaviour, the regulator's text, or your work — submit a correction request via the right-of-reply channel. The Specialist Panel will publish factual corrections or contextual responses alongside the original finding, with no editorial gatekeeping.

Submit: <https://reglegbrief.com/right-of-reply/>

## Publisher

**Verdus Technologies Pte. Ltd.** · UEN 201616982R · Singapore-incorporated
RegLegBrief is the public research output of Verdus Technologies Pte. Ltd.
Editorial standards: <https://reglegbrief.com/methodology/>
About the Specialist Panel: <https://reglegbrief.com/specialist-panel/>

## Versioning + change log

This repository is auto-updated by a server-side cron on every reg ship. The full chronological change history is in [`log.md`](./log.md).

## Spec reference

This bundle implements [Open Knowledge Format v0.1](https://github.com/GoogleCloudPlatform/knowledge-catalog/tree/main/okf) — a vendor-neutral, file-based knowledge format for human + AI-agent consumption announced by Google Cloud in June 2026.
