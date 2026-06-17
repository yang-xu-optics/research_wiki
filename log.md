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

## [2026-06-17] ingest | Direct growth of crack-free stoichiometric silicon nitride on sapphire for wide-band photonics (Ma et al., 2026)

- **Source:** [[crack-free-silicon-nitride-on-sapphire-lu]]
- **Pages touched:** [[crack-free-silicon-nitride-on-sapphire-lu]], [[silicon-nitride]], [[silicon-nitride-on-sapphire]], [[wide-band-photonics]], [[zhaohui-ma]], [[kartik-srinivasan]], [[xiyuan-lu]], [[nist]], [[joint-quantum-institute]], [[2d-programmable-nonlinear-waveguide-mcmahon]], [[photoconductive-gain-programming]], [[programmable-photonic-waveguide]], [[lithium-niobate]], [[programmable-photonic-computing]], [[mcmahon-lab-cornell]]
- **Notes:** Renamed the raw PDF to `raw/sources/articles/2026-06-17-crack-free-silicon-nitride-on-sapphire.pdf`. The paper argues that sapphire relieves residual tensile stress in stoichiometric LPCVD Si3N4, enabling crack-free films up to about 2 micrometers while retaining competitive visible/near-IR/telecom photonic losses.

## [2026-06-17] ingest | III-V / AlGaAs integrated photonics symlink batch

- **Source:** [[carrier-induced-index-iii-v-bennett]], [[optically-activated-gaas-mzi-cheng-tsai]], [[nonlinear-propagation-algaas-bragg-grating-millar]], [[ridge-bragg-reflection-waveguide-shg-helmy]], [[periodically-inverted-algaas-waveguides-ota]], [[type-ii-qpm-superlattice-waveguides-hutchings]], [[femtosecond-shg-algaas-brw-han]], [[dfg-algaas-brw-han]], [[iii-v-chip-correlated-photon-pair-source-sarrafi]], [[algaas-guided-wave-shg-qcl-ozanam]], [[frequency-comb-algaas-oi-pu]], [[directionally-induced-qpm-algaas-morais]], [[chip-frequency-comb-parallel-data-hu]], [[octave-supercontinuum-algaas-oi-kuyken]], [[algaas-oi-entangled-photon-pair-microring-steiner]], [[algaas-nonlinear-integrated-photonics-mobini]], [[nonlinear-integrated-quantum-photonics-algaas-baboux]], [[low-voltage-high-power-algaas-mzi-bhasker]], [[gaas-algaas-travelling-wave-eo-modulator-spickermann]]
- **Pages touched:** [[optics-photonics-research-map]], [[iii-v-integrated-photonics]], [[algaas-on-insulator]], [[semiconductor-phase-matching]], [[bragg-reflection-waveguide]], [[electro-optic-modulation]], [[electro-optic-effect]], [[integrated-quantum-photonics]], [[optical-frequency-comb]], [[second-harmonic-generation]], [[quasi-phase-matching]], plus all source pages listed above, [[index]], and [[AGENTS]]
- **Notes:** Ingested 19 PDFs from the `raw/sources/articles/iii-v_devices` symlink by copying normalized raw-source filenames into `raw/sources/articles/iii-v-devices/`. Updated the project aim to make the vault explicitly serve as a cross-field optics/photonics literature and research-idea database.

## [2026-06-17] ingest | Quantum-optical high-harmonic generation papers

- **Source:** [[photon-antibunching-hhg-stammer]], [[quantum-optical-nature-hhg-gorlach]], [[entanglement-measurement-theory-hhg-stammer]], [[high-harmonic-generation-driven-by-quantum-light-gorlach]], [[entanglement-squeezing-optical-field-modes-hhg-stammer]], [[photon-bunching-high-harmonic-emission-lemieux]], [[high-harmonic-generation-bright-squeezed-vacuum-rasputnyi]], [[attosecond-pulse-synthesis-squeezed-light-hhg-wang]], [[evidence-quantum-optical-nature-hhg-theidel]], [[squeezed-states-after-hhg-excited-atoms-rivera-dean]], [[excitonic-enhancement-squeezed-light-mott-hhg-lange]], [[structured-squeezed-light-forbidden-hhg-rivera-dean]], [[solid-state-high-order-harmonic-generation-frontiers-ciappina]], [[quantum-dial-hhg-wang]], [[crystal-hhg-driven-by-quantum-light-gothelf]], [[generation-squeezed-high-order-harmonics-tzur]], [[observation-displaced-squeezed-state-hhg-theidel]], [[quantum-optics-optical-coherence-hhg-stammer]], [[band-topology-quantum-optical-signatures-hhg-ilin]], [[edge-states-quantum-optical-hhg-lange]], [[nonclassical-cutoff-fluctuations-hhg-khurelbaatar]], [[fluctuation-induced-symmetry-breaking-bicircular-hhg-stammer]], [[symmetry-breaking-quantum-light-solid-state-hhg-stammer]]
- **Pages touched:** [[high-harmonic-generation]], [[strong-field-quantum-optics]], [[bright-squeezed-vacuum]], [[quantum-light-driven-hhg]], [[solid-state-high-harmonic-generation]], [[attosecond-pulse-generation]], [[optics-photonics-research-map]], all source pages listed above, [[index]], and [[log]]
- **Notes:** Ingested 23 deduplicated HHG/high-order-harmonic papers from new top-level PDFs and the `raw/sources/articles/stochastic_em_theory` symlink. Normalized copies live in `raw/sources/articles/high-harmonic-generation/`; excluded `PhysRevA.96.033847.pdf` because it is microring photon-pair theory rather than HHG, and deduplicated the PRL HHG squeezing paper.

## [2026-06-17] query | Why entanglement can appear in HHG

- **Pages touched:** [[hhg-entanglement-mechanism]], [[index]], [[log]]
- **Notes:** Filed a reusable explanation of HHG entanglement: quantized field modes couple through the same quantum matter response, so dipole/current correlations prevent the harmonic output from factorizing into independent coherent states.

## [2026-06-17] query | Why ground-state depletion creates dipole correlations

- **Pages touched:** [[hhg-entanglement-mechanism]], [[log]]
- **Notes:** Added the mechanism: in the weak-depletion limit two-time dipole averages approximately factorize, while depletion makes the emitter state at later times depend on earlier emission/ionization, creating connected dipole correlations that couple harmonic modes.

## [2026-06-17] query | Whether stochastic field theory remains worthwhile after HHG antibunching

- **Pages touched:** [[stochastic-field-theory-for-hhg-thz]], [[index]], [[log]]
- **Notes:** Filed the strategic conclusion: the antibunching paper rules out a purely classical stochastic explanation for all HHG observables, but strengthens the case for a stochastic/phase-space framework that maps the boundary between classical noise, quantum field statistics, HHG, and THz observables.

## [2026-06-17] query | Critical correlations as an HHG entanglement resource

- **Pages touched:** [[critical-correlations-hhg-entanglement]], [[optics-photonics-research-map]], [[index]], [[log]]
- **Notes:** Filed the research idea that ferroelectric phase transitions and more general long-range matter correlations could enhance HHG squeezing/entanglement through connected polarization/current correlators, while requiring nonclassical witnesses to separate quantum correlations from classical critical noise.

## [2026-06-17] query | Simulation framework for critical HHG entanglement paper

- **Pages touched:** [[critical-hhg-simulation-framework]], [[critical-correlations-hhg-entanglement]], [[index]], [[log]]
- **Notes:** Filed a concrete theory/simulation plan: use input-output relations from connected matter current correlators to harmonic covariance matrices, then simulate correlated-emitter, ferroelectric soft-mode, and HHG-active solid models with squeezing and entanglement witnesses.

## [2026-06-17] query | Perturbative nonlinear optics version of critical-correlation entanglement

- **Pages touched:** [[critical-correlations-perturbative-nonlinear-optics]], [[critical-correlations-hhg-entanglement]], [[critical-hhg-simulation-framework]], [[index]], [[log]]
- **Notes:** Clarified that HHG is not required: SHG, THG, SPDC, and four-wave mixing can test the same source-correlation mechanism in a cleaner few-mode perturbative regime, though classical susceptibility fluctuations must be separated from genuine squeezing/entanglement.

## [2026-06-17] query | Cavity SHG/THG simulation framework near a critical transition

- **Pages touched:** [[critical-cavity-shg-thg-simulation-framework]], [[critical-correlations-perturbative-nonlinear-optics]], [[index]], [[log]]
- **Notes:** Filed a concrete open-system simulation plan: a driven lossy cavity SHG/THG model with nonlinear coupling `g(Q)` modulated by a ferroelectric soft mode or critical order parameter, evaluated through output squeezing, photon statistics, and pump-harmonic entanglement.
