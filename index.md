# Index

Content catalog for the vault. Updated on every ingest.
See [[CLAUDE]] for conventions, [[log]] for chronological history.

## Overviews

- [[knowledge-base-architectures]] — how raw-document RAG, NotebookLM-style retrieval, and the LLM Wiki pattern compare

## Concepts

- [[llm-wiki-pattern]] — incrementally LLM-maintained markdown KB sitting between user and raw sources
- [[rag]] — retrieval-augmented generation; re-derives knowledge from chunks per query
- [[ingest-operation]] — workflow for absorbing a new source into the wiki
- [[query-operation]] — workflow for asking the wiki and filing answers back
- [[lint-operation]] — periodic health-check of the wiki for contradictions, orphans, gaps
- [[memex]] — Vannevar Bush's 1945 personal-knowledge-store concept; spiritual ancestor of the pattern

## Entities

- [[andrej-karpathy]] — author of the LLM Wiki gist; ex-OpenAI / Tesla AI researcher
- [[obsidian]] — local-first markdown editor used as the wiki frontend
- [[claude-code]] — Anthropic's CLI agent; reads `CLAUDE.md` as its schema file
- [[notebooklm]] — Google's document-grounded LLM tool; contrast example for retrieval-only KBs
- [[qmd]] — local hybrid BM25/vector search engine for markdown files
- [[obsidian-web-clipper]] — browser extension that saves web pages as markdown into the vault
- [[marp]] — markdown-to-slides format with an Obsidian plugin
- [[dataview]] — Obsidian plugin that queries page frontmatter

## Sources

- [[llm-wiki-pattern-karpathy]] — Andrej Karpathy's gist proposing the LLM Wiki pattern (2026-05-28 ingest)
