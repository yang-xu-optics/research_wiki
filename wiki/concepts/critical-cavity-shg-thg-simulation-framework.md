---
type: concept
name: "Critical cavity SHG/THG simulation framework"
aliases: ["cavity-enhanced critical SHG", "cavity-enhanced critical THG", "ferroelectric cavity nonlinear optics simulation"]
sources: [[critical-correlations-perturbative-nonlinear-optics, second-harmonic-generation, quasi-phase-matching, lithium-niobate]]
related: [[critical-correlations-perturbative-nonlinear-optics, critical-correlations-hhg-entanglement, second-harmonic-generation, lithium-niobate]]
tags: [nonlinear-optics, quantum-optics, simulation, squeezing, ferroelectrics]
---

# Critical cavity SHG/THG simulation framework

> A concrete simulation/theory plan for cavity-enhanced SHG or THG near a ferroelectric or more general critical transition, where order-parameter fluctuations modulate the nonlinear coupling and can imprint squeezing or entanglement on generated light.

## Core claim

The paper should distinguish two effects:

1. **Mean critical enhancement:** the average nonlinear coefficient increases near a transition, raising SHG/THG efficiency.
2. **Critical quantum-noise transfer:** fluctuations and correlations of the order parameter modulate the nonlinear coupling, creating excess noise, squeezing, or entanglement in the generated optical modes.

Only the second effect is the new quantum-optical claim.

## Why use a cavity?

A cavity is not required. It is a simplifying and amplifying platform for a first theory paper.

The cavity does four useful things: it enhances the nonlinear interaction time, reduces the continuum of traveling optical modes to a few measurable modes, makes homodyne/correlation observables cleaner through input-output theory, and introduces tunable linewidths that can be compared directly to the soft-mode frequency and correlation time.

Without a cavity, the same physics can be studied in a traveling-wave crystal or waveguide. The theory then becomes a propagation problem with spatially and temporally fluctuating nonlinear susceptibility, for example:

`H_int = int dz [g(Q(z,t)) b^dag(z,t) a(z,t)^2 + h.c.]`.

That version is more general and closer to many experiments, but it adds phase matching, group-velocity mismatch, pulse propagation, collection modes, and multimode detection. The cavity-first model is therefore a minimal testbed, not a claim that cavities are essential.

## Minimal cavity model

Use two cavity modes for SHG: a fundamental mode `a` near frequency `omega`, and a second-harmonic mode `b` near `2 omega`.

`H_cav = Delta_a a^dag a + Delta_b b^dag b + i(E a^dag - E* a)`.

The ordinary SHG interaction is:

`H_SHG = g(Q) b^dag a a + g*(Q) b a^dag a^dag`.

For THG, replace `b` by a third-harmonic mode `c` and use:

`H_THG = h(Q) c^dag a a a + h*(Q) c a^dag a^dag a^dag`.

The critical material enters through an order parameter `Q` that modulates the nonlinear coupling:

`g(Q) = g0 + g1 Q + g2 Q^2 + ...`.

Near a ferroelectric transition, `Q` can represent the soft polar mode, domain-averaged polarization, or a cavity-weighted collective coordinate of the order parameter.

## Ferroelectric / critical sector

Start with one collective soft mode:

`H_Q = Omega_Q(lambda) d^dag d + beta (d + d^dag)^4`.

Use `Q = q_zpf (d + d^dag)`. The tuning parameter `lambda` controls distance to the transition. Critical softening is modeled by decreasing `Omega_Q(lambda)` and increasing the variance/correlation time of `Q`.

For the first paper, use the harmonic approximation plus damping:

`H_Q = Omega_Q d^dag d`.

Collapse operators:

`sqrt(gamma_Q (n_th + 1)) d`, `sqrt(gamma_Q n_th) d^dag`.

Then add anharmonicity or many-mode order-parameter fluctuations only after the minimal mechanism is clear.

## Open-system master equation

Simulate the density matrix with a Lindblad master equation:

`d rho / dt = -i[H, rho] + kappa_a D[a]rho + kappa_b D[b]rho + gamma_Q (n_th+1) D[d]rho + gamma_Q n_th D[d^dag]rho`.

For SHG:

`H = H_cav + H_Q + H_SHG`.

For THG:

`H = H_cav + H_Q + H_THG`.

Input-output fields are:

`a_out = a_in + sqrt(kappa_a) a`,

`b_out = b_in + sqrt(kappa_b) b`.

This makes the simulation directly comparable to homodyne, heterodyne, and photon-correlation measurements.

## Simulation ladder

1. **Ordinary cavity SHG baseline.** Set `g(Q) = g0`. Sweep pump strength, detuning, and cavity loss. Reproduce conversion, harmonic squeezing, and pump-harmonic correlations in the standard model.
2. **Static critical enhancement.** Let `g_eff(lambda)` increase as the transition is approached, but keep `Q` classical and noiseless. This isolates simple efficiency enhancement.
3. **Quantum fluctuating nonlinearity.** Use `g(Q) = g0 + g1 Q` with `Q` as a damped soft quantum mode. Sweep `Omega_Q`, `gamma_Q`, and `n_th`.
4. **Critical-noise comparison.** Compare quantum `Q` to classical stochastic `g(t)` with the same spectrum. Any squeezing/entanglement that survives beyond the classical model is the nonclassical part.
5. **Many-mode critical bath.** Replace the single `Q` oscillator by a colored noise or bath spectral density with critical form, e.g. longer correlation time near the transition.
6. **THG variant.** Repeat with `c^dag a^3`. THG may be better for centrosymmetric phases where chi(2) vanishes but chi(3) remains.

## Observables

- Mean conversion: `<b^dag b>` for SHG or `<c^dag c>` for THG.
- Harmonic quadrature squeezing: `min_theta Var[X_b(theta)]` or `Var[X_c(theta)]`.
- Pump-harmonic entanglement: covariance matrix of `(a,b)` or `(a,c)`, with logarithmic negativity or Duan-Simon criterion.
- Photon statistics: `g2_b(0)`, `g2_c(0)`, and cross-correlations `g2_ab(0)`.
- Output noise spectra: homodyne spectrum of the harmonic mode near soft-mode sidebands.
- Critical scaling: squeezing or entanglement versus `Omega_Q`, susceptibility, correlation time, temperature, and distance from transition.

## Expected signatures

- If only `g_eff` increases, harmonic intensity rises but nonclassicality does not necessarily improve.
- If quantum `Q` fluctuations dominate, harmonic squeezing and pump-harmonic entanglement can peak near the transition.
- If thermal/classical critical noise dominates, conversion may rise while squeezing is degraded and photon statistics become noisy or bunched.
- The optimum likely occurs near the transition, not exactly at it, because susceptibility enhancement competes with thermal noise and dephasing.
- Soft-mode sidebands in the harmonic output noise would be a clean signature that order-parameter dynamics, not just static chi enhancement, is being transferred into the light.

## First numerical implementation

Use QuTiP with Hilbert cutoffs such as `N_a = 20-40`, `N_b = 10-20`, and `N_Q = 8-20`, adjusted by pump strength. Run steady-state calculations when stable, and time-domain master-equation evolution when approaching instabilities or bistability.

Parameter sweep:

- `Omega_Q / kappa_b`: soft-mode frequency relative to harmonic cavity linewidth.
- `gamma_Q / kappa_b`: slow versus fast order-parameter dynamics.
- `g1 / g0`: strength of critical modulation of the nonlinear coefficient.
- `n_th`: thermal critical noise.
- `Delta_a`, `Delta_b`: cavity detunings.
- pump amplitude `E`.

The first result should be a map of harmonic squeezing/log-negativity versus `Omega_Q` and `n_th`, showing the boundary between useful quantum critical enhancement and destructive classical critical noise.

## Paper framing

The safest paper title concept is:

> Critical fluctuations as a quantum-noise resource in cavity nonlinear optics.

The SHG version is closest to ferroelectrics and lithium-niobate-style platforms. The THG version is more symmetry-general and may be useful when the high-symmetry phase is centrosymmetric and chi(2) disappears.

## Related

- [[critical-correlations-perturbative-nonlinear-optics]]
- [[second-harmonic-generation]]
- [[quasi-phase-matching]]
- [[lithium-niobate]]
