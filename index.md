# Index

Content catalog for the vault. Updated on every ingest.
See [[CLAUDE]] for conventions, [[log]] for chronological history.

## Overviews

- [[optics-photonics-research-map]] — cross-field map for optics/photonics mechanisms, platforms, and research-idea prompts
- [[programmable-photonic-computing]] — McMahon-group research program for 2D-programmable photonic substrates (linear + nonlinear arms)
- [[knowledge-base-architectures]] — how raw-document RAG, NotebookLM-style retrieval, and the LLM Wiki pattern compare

## Concepts

- [[iii-v-integrated-photonics]] — compound-semiconductor photonics linking active, EO, nonlinear, and quantum functions
- [[algaas-on-insulator]] — high-confinement III-V platform for combs, supercontinuum, and quantum light
- [[semiconductor-phase-matching]] — BRW, QPM, inversion, and geometry tricks for chi(2) processes in III-V waveguides
- [[bragg-reflection-waveguide]] — phase-matching waveguide using Bragg confinement for one interacting optical mode
- [[electro-optic-modulation]] — phase/amplitude control bridge between communications, programmable optics, and III-V platforms
- [[electro-optic-effect]] — field-induced refractive-index change linking LiNbO3, III-V modulators, and programmable media
- [[integrated-quantum-photonics]] — chip-scale quantum light sources, circuits, filters, modulators, and detectors
- [[optical-frequency-comb]] — integrated comb and supercontinuum sources for metrology, communications, and quantum scaling
- [[high-harmonic-generation]] — nonperturbative extreme upconversion producing XUV/attosecond harmonics
- [[hhg-entanglement-mechanism]] — why quantized HHG can entangle driver and harmonic field modes
- [[critical-correlations-hhg-entanglement]] — research idea: use critical/long-range matter correlations to enhance HHG squeezing
- [[critical-hhg-simulation-framework]] — simulation/theory blueprint for HHG entanglement from critical correlations
- [[critical-correlations-perturbative-nonlinear-optics]] — SHG/THG/SPDC/FWM version of matter-correlation-induced quantum light
- [[critical-cavity-shg-thg-simulation-framework]] — cavity SHG/THG model where critical order-parameter noise modulates nonlinear coupling
- [[strong-field-quantum-optics]] — quantized-field view of intense light-matter interactions and HHG correlations
- [[bright-squeezed-vacuum]] — macroscopic squeezed-light state now used as an HHG/strong-field driver
- [[quantum-light-driven-hhg]] — HHG controlled by nonclassical driver statistics and fluctuations
- [[stochastic-field-theory-for-hhg-thz]] — when stochastic HHG/THz models are useful and where classical noise fails
- [[solid-state-high-harmonic-generation]] — HHG in crystals/materials as ultrafast spectroscopy and quantum-light source
- [[attosecond-pulse-generation]] — synthesis of attosecond bursts from phase-locked high harmonics
- [[silicon-nitride-on-sapphire]] — low-stress Si3N4/sapphire platform for crack-free thick LPCVD films
- [[silicon-nitride]] — low-loss dielectric photonics material used across visible, near-IR, telecom, and mid-IR
- [[wide-band-photonics]] — integrated photonics designed to operate across visible, near-IR, telecom, and mid-IR bands
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

- [[zhaohui-ma]] — first author of the 2026 Si3N4-on-sapphire wide-band photonics paper
- [[kartik-srinivasan]] — NIST/JQI photonics researcher and corresponding author on the Si3N4-on-sapphire paper
- [[xiyuan-lu]] — NIST/JQI photonics researcher and corresponding author on the Si3N4-on-sapphire paper
- [[nist]] — U.S. federal research institute; affiliation/fabrication context for the Si3N4-on-sapphire paper
- [[joint-quantum-institute]] — NIST/University of Maryland institute affiliated with the Si3N4-on-sapphire authors
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

- [[photon-antibunching-hhg-stammer]] — Stammer, Rivera-Dean, Lewenstein, 2026; antibunching in HHG photons
- [[nonclassical-cutoff-fluctuations-hhg-khurelbaatar]] — Khurelbaatar et al., 2026; cutoff variance as nonclassical HHG witness
- [[edge-states-quantum-optical-hhg-lange]] — Lange and Madsen, 2026; edge states in quantum-optical HHG
- [[band-topology-quantum-optical-signatures-hhg-ilin]] — Ilin et al., 2026; topology signatures in solid-state high harmonics
- [[symmetry-breaking-quantum-light-solid-state-hhg-stammer]] — Stammer et al., 2026; quantum-light symmetry breaking in solid HHG
- [[fluctuation-induced-symmetry-breaking-bicircular-hhg-stammer]] — Stammer et al., 2026; bicircular quantum-light HHG symmetry breaking
- [[quantum-dial-hhg-wang]] — Wang et al., 2025; weak quantum light as a tunable HHG control dial
- [[solid-state-high-order-harmonic-generation-frontiers-ciappina]] — Ciappina, 2025; solid-state HHG frontiers review
- [[structured-squeezed-light-forbidden-hhg-rivera-dean]] — Rivera-Dean et al., 2025; squeezed light enables classically forbidden HHG
- [[quantum-optics-optical-coherence-hhg-stammer]] — Stammer, Rivera-Dean, Lewenstein, 2025; optical coherence theory for HHG
- [[excitonic-enhancement-squeezed-light-mott-hhg-lange]] — Lange et al., 2025; excitonic squeezing enhancement in Mott HHG
- [[crystal-hhg-driven-by-quantum-light-gothelf]] — Gothelf et al., 2025; crystal HHG driven by quantum light
- [[squeezed-states-after-hhg-excited-atoms-rivera-dean]] — Rivera-Dean et al., 2025; squeezed states after HHG in excited atoms
- [[observation-displaced-squeezed-state-hhg-theidel]] — Theidel et al., 2025; observed displaced squeezed state in HHG
- [[attosecond-pulse-synthesis-squeezed-light-hhg-wang]] — Wang, Lai, Liu, 2024; attosecond synthesis from squeezed-light HHG
- [[evidence-quantum-optical-nature-hhg-theidel]] — Theidel et al., PRX Quantum 2024; experimental quantum-optical evidence in HHG
- [[high-harmonic-generation-bright-squeezed-vacuum-rasputnyi]] — Rasputnyi et al., 2024; HHG driven by bright squeezed vacuum
- [[photon-bunching-high-harmonic-emission-lemieux]] — Lemieux et al., 2024; photon bunching in quantum-light-controlled HHG
- [[entanglement-squeezing-optical-field-modes-hhg-stammer]] — Stammer et al., PRL 2024; HHG field-mode squeezing/entanglement
- [[high-harmonic-generation-driven-by-quantum-light-gorlach]] — Gorlach et al., Nature Physics 2023; quantum-light-driven HHG
- [[entanglement-measurement-theory-hhg-stammer]] — Stammer, 2022; measurement theory for HHG entanglement
- [[quantum-optical-nature-hhg-gorlach]] — Gorlach et al., 2020; quantum-optical nature of HHG
- [[generation-squeezed-high-order-harmonics-tzur]] — Even Tzur et al.; quantum-state transfer into squeezed high-order harmonics
- [[gaas-algaas-travelling-wave-eo-modulator-spickermann]] — Spickermann et al., 2024; GaAs/AlGaAs travelling-wave EO modulator >40 GHz
- [[nonlinear-integrated-quantum-photonics-algaas-baboux]] — Baboux, Moody, Ducci, Optica 2023; AlGaAs quantum photonics review
- [[algaas-nonlinear-integrated-photonics-mobini]] — Mobini et al., 2022; broad AlGaAs nonlinear integrated photonics review
- [[algaas-oi-entangled-photon-pair-microring-steiner]] — Steiner et al., PRX Quantum 2021; ultrabright entangled pairs in AlGaAsOI
- [[octave-supercontinuum-algaas-oi-kuyken]] — Kuyken et al., Optics Letters 2020; octave supercontinuum in AlGaAsOI
- [[low-voltage-high-power-algaas-mzi-bhasker]] — Bhasker/Dagli et al.; low-voltage high-power AlGaAs MZI modulator manuscript
- [[chip-frequency-comb-parallel-data-hu]] — Hu, Da Ros, Pu et al., Nature Photonics 2018; AlGaAsOI comb for 661 Tbit/s transmission
- [[directionally-induced-qpm-algaas-morais]] — Morais et al., Optics Letters 2017; QPM from curved AlGaAs waveguide geometry
- [[frequency-comb-algaas-oi-pu]] — Pu et al., Optica 2016; efficient Kerr comb generation in AlGaAs-on-insulator
- [[algaas-guided-wave-shg-qcl-ozanam]] — Ozanam et al., Applied Optics 2014; QCL frequency doubling in GaAs/AlOx waveguides
- [[iii-v-chip-correlated-photon-pair-source-sarrafi]] — Sarrafi et al., APL 2013; CW QPM photon-pair source on a III-V chip
- [[dfg-algaas-brw-han]] — Han et al., Optics Letters 2010; DFG in AlGaAs Bragg reflection waveguides
- [[femtosecond-shg-algaas-brw-han]] — Han et al., JOSA B 2010; ultrafast SHG theory/experiment in AlGaAs BRWs
- [[type-ii-qpm-superlattice-waveguides-hutchings]] — Hutchings et al., Optics Letters 2010; type-II QPM in intermixed superlattices
- [[periodically-inverted-algaas-waveguides-ota]] — Ota et al., JJAP 2009; periodically inverted AlGaAs waveguides
- [[ridge-bragg-reflection-waveguide-shg-helmy]] — Bijlani, Abolghasem, Helmy, APL 2008; ridge BRW SHG
- [[nonlinear-propagation-algaas-bragg-grating-millar]] — Millar et al., Optics Letters 1999; nonlinear propagation in AlGaAs gratings
- [[optically-activated-gaas-mzi-cheng-tsai]] — Cheng and Tsai, APL 1991; optically activated GaAs MZI
- [[carrier-induced-index-iii-v-bennett]] — Bennett, Soref, del Alamo, IEEE JQE 1990; carrier-induced index in III-Vs
- [[crack-free-silicon-nitride-on-sapphire-lu]] — Ma et al., 2026; crack-free stoichiometric Si3N4 on sapphire for wide-band photonics
- [[2d-programmable-nonlinear-waveguide-mcmahon]] — Yanagimoto et al., Nature, Jan 2026; programmable χ⁽²⁾ on SiN (2026-05-28 ingest)
- [[2d-programmable-linear-waveguide-mcmahon]] — Onodera, Stein et al., Nature Physics, Dec 2025; programmable Δn on LiNbO₃ (2026-05-28 ingest)
- [[llm-wiki-pattern-karpathy]] — Andrej Karpathy's gist proposing the LLM Wiki pattern (2026-05-28 ingest)
