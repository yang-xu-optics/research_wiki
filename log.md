# Log

Append-only chronological record. Newest entries at the bottom.
Entry prefix is fixed: `## [YYYY-MM-DD] <op> | <title>`.

Quick recent view: `grep "^## \[" log.md | tail -10`.

---

## [2026-05-28] note | vault initialized

- **Notes:** Instantiated Karpathy's [[llm-wiki-pattern]] in this vault. Created `CLAUDE.md`, `index.md`, `log.md`, `templates/`, and the `raw/` + `wiki/` layer directories. See [[CLAUDE]] for the schema.

## [2026-05-28] ingest | LLM Wiki (Andrej Karpathy gist)

- **Source:** [[llm-wiki-pattern-karpathy]]
- **Pages touched:** [[llm-wiki-pattern-karpathy]], [[llm-wiki-pattern]], [[rag]], [[ingest-operation]], [[query-operation]], [[lint-operation]], [[memex]], [[andrej-karpathy]], [[obsidian]], [[claude-code]], [[notebooklm]], [[qmd]], [[obsidian-web-clipper]], [[marp]], [[dataview]], [[knowledge-base-architectures]]
- **Notes:** Seed ingest. The gist becomes both a source and the conceptual backbone of the schema (`CLAUDE.md`). Created one overview to anchor future comparisons of KB architectures.

## [2026-05-28] ingest | Arbitrary control over multimode wave propagation for machine learning (Onodera, Stein et al., Nature Physics 2025)

- **Source:** [[2d-programmable-linear-waveguide-mcmahon]]
- **Pages touched:** [[2d-programmable-linear-waveguide-mcmahon]], [[programmable-photonic-waveguide]], [[photoconductive-gain-programming]], [[lithium-niobate]], [[optical-neural-network]], [[peter-mcmahon]], [[mcmahon-lab-cornell]], [[ntt-research-pin-labs]], [[tatsuhiro-onodera]], [[programmable-photonic-computing]]
- **Notes:** Linear arm of the McMahon-group programmable-photonics program. Programs refractive index Δn(x, z) on a lithium niobate slab via photoconductive gain; demonstrates ONN inference at N=49 with claimed N^1.5 area scaling. Used to seed [[programmable-photonic-waveguide]], [[photoconductive-gain-programming]], and the [[programmable-photonic-computing]] overview.

## [2026-05-28] ingest | Programmable on-chip nonlinear photonics (Yanagimoto et al., Nature 2026)

- **Source:** [[2d-programmable-nonlinear-waveguide-mcmahon]]
- **Pages touched:** [[2d-programmable-nonlinear-waveguide-mcmahon]], [[programmable-photonic-waveguide]], [[photoconductive-gain-programming]], [[quasi-phase-matching]], [[second-harmonic-generation]], [[ryotatsu-yanagimoto]], [[peter-mcmahon]], [[mcmahon-lab-cornell]], [[ntt-research-pin-labs]], [[programmable-photonic-computing]]
- **Notes:** Nonlinear arm of the same program. Same photoconductive-gain programming trick applied to electric-field-induced χ⁽²⁾ on SiN. Demonstrates programmable QPM gratings for broadband SHG with spectral/spatial/spatio-spectral control, in-situ inverse design, and real-time drift compensation. Companion to the linear paper — see [[programmable-photonic-computing]] for the synthesis.
