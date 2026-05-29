---
type: concept
name: "Lint (operation)"
aliases: ["lint", "wiki lint"]
sources: [[llm-wiki-pattern-karpathy]]
related: [[llm-wiki-pattern, ingest-operation, query-operation]]
tags: [workflow, maintenance]
---

# Lint (operation)

> A periodic health-check of the [[llm-wiki-pattern|wiki]]: look for contradictions, stale claims, orphan pages, missing pages, broken links, and coverage gaps — and propose fixes rather than auto-applying them — [[llm-wiki-pattern-karpathy]].

## Origin

The third of Karpathy's three operations, alongside [[ingest-operation|ingest]] and [[query-operation|query]] — [[llm-wiki-pattern-karpathy]]. Framed as the mechanism that keeps the wiki healthy as it grows.

## How it works

In this vault (see [[CLAUDE]]):

- **Contradictions** — scan for opposing claims; flag with `> [!warning]` callouts on both pages.
- **Stale claims** — statements superseded by a newer source (check `date_published` in source frontmatter).
- **Orphans** — wiki pages with no inbound `[[wikilinks]]`.
- **Missing pages** — terms cited in 3+ pages without a dedicated page.
- **Broken links** — `[[wikilinks]]` pointing at non-existent slugs.
- **Coverage gaps** — concepts mentioned offhand that deserve their own page; suggest sources to find.

Output: a `## [YYYY-MM-DD] lint | <scope>` log entry with findings as a checklist. Destructive changes are proposed, not auto-applied.

## Trade-offs / Contrasts with

- vs **ingest-time cleanup** — small fixes happen during [[ingest-operation|ingest]]; structural sweeps wait for lint.
- vs **no lint** — without lint, the wiki silently drifts: contradictions accumulate, dead links pile up, orphans multiply.

## Open questions

- Right cadence: per-N-ingests, weekly, or on-demand only? Karpathy doesn't prescribe.
- How autonomous should lint be? Proposing-only is safer; auto-apply is faster but risks silent edits.

## Related

- [[llm-wiki-pattern]]
- [[ingest-operation]]
- [[query-operation]]
