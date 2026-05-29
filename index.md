# Index

Content catalog for the vault. Updated on every ingest.
See [[CLAUDE]] for conventions, [[log]] for chronological history.

## Overviews

- [[programmable-photonic-computing]] — McMahon-group research program for 2D-programmable photonic substrates (linear + nonlinear arms)
- [[knowledge-base-architectures]] — how raw-document RAG, NotebookLM-style retrieval, and the LLM Wiki pattern compare

## Concepts

- [[programmable-photonic-waveguide]] — slab waveguide whose Δn or χ⁽²⁾ is reprogrammable across ~10⁴ regions via patterned light
- [[photoconductive-gain-programming]] — patterned light + photoconductor switches a single high-voltage bias into thousands of virtual electrodes
- [[lithium-niobate]] — ferroelectric crystal with strong Pockels effect and χ⁽²⁾; substrate of the McMahon linear waveguide
- [[quasi-phase-matching]] — periodically modulating χ⁽²⁾ to compensate phase mismatch and recover efficient nonlinear conversion
- [[second-harmonic-generation]] — χ⁽²⁾ process converting two ω photons into one 2ω photon; benchmark NLO process
- [[optical-neural-network]] — neural networks whose linear layers run on photonic hardware to cut per-MAC energy
- [[llm-wiki-pattern]] — incrementally LLM-maintained markdown KB sitting between user and raw sources
- [[rag]] — retrieval-augmented generation; re-derives knowledge from chunks per query
- [[ingest-operation]] — workflow for absorbing a new source into the wiki
- [[query-operation]] — workflow for asking the wiki and filing answers back
- [[lint-operation]] — periodic health-check of the wiki for contradictions, orphans, gaps
- [[memex]] — Vannevar Bush's 1945 personal-knowledge-store concept; spiritual ancestor of the pattern

## Entities

- [[peter-mcmahon]] — PI of the McMahon Lab; corresponding author on both 2025/26 programmable-waveguide papers
- [[mcmahon-lab-cornell]] — Cornell research group working on physics-based computing and programmable photonics
- [[ntt-research-pin-labs]] — NTT Research Physics & Informatics Laboratories (Sunnyvale); long-running collaborator with McMahon Lab (vault owner's org)
- [[ryotatsu-yanagimoto]] — lead author of the programmable nonlinear-waveguide paper; joint Cornell + NTT Research
- [[tatsuhiro-onodera]] — co-first author of the programmable linear-waveguide paper; joint Cornell + NTT Research
- [[andrej-karpathy]] — author of the LLM Wiki gist; ex-OpenAI / Tesla AI researcher
- [[obsidian]] — local-first markdown editor used as the wiki frontend
- [[claude-code]] — Anthropic's CLI agent; reads `CLAUDE.md` as its schema file
- [[notebooklm]] — Google's document-grounded LLM tool; contrast example for retrieval-only KBs
- [[qmd]] — local hybrid BM25/vector search engine for markdown files
- [[obsidian-web-clipper]] — browser extension that saves web pages as markdown into the vault
- [[marp]] — markdown-to-slides format with an Obsidian plugin
- [[dataview]] — Obsidian plugin that queries page frontmatter

## Sources

- [[2d-programmable-nonlinear-waveguide-mcmahon]] — Yanagimoto et al., Nature, Jan 2026; programmable χ⁽²⁾ on SiN (2026-05-28 ingest)
- [[2d-programmable-linear-waveguide-mcmahon]] — Onodera, Stein et al., Nature Physics, Dec 2025; programmable Δn on LiNbO₃ (2026-05-28 ingest)
- [[llm-wiki-pattern-karpathy]] — Andrej Karpathy's gist proposing the LLM Wiki pattern (2026-05-28 ingest)
