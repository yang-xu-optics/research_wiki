---
type: craft-export
title: "2025-12-24 photonic crystal design"
craft_document_id: ADDA8B52-137E-4835-AB51-DD363952CADC
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-12-24 photonic crystal design
As a final demonstration for the etched device, we would like to show poling on a photonic crystal structure.  Technically, we want to do two demonstrations, one of which will be flat poling on a DBR waveguide and show a very weird shape of the poling period with the wavelength.  The other is we want to do a waveguide with rather long perturbations (ie, much longer than the poling period we use), and show that the poling structure can adapt to the underlying geometry.  This note will describe the simulation efforts to understand the design implications for the photonic crystal waveguides.  

Below is the derivation of the photonic crystal reflection coefficient (which is the square of the A(L) term).  

[Photonic Crystal Derivation.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/6E3F4871-8E9F-484E-93B9-55D2D8B49FF8_2/UVxEy4Cy979ywT3LL6cU8AnYlOSYx8rTPUij2OpJxuQz/Photonic%20Crystal%20Derivation.pdf)

It does not cover an important note: the scaling of the coupling coefficient with the shape that you fabricate.  For example, if we use a higher order diffraction grating, then we are obviously not using the central fourier component.  So, if we use a sine-wave, then we only have fourier components at that frequeny, but not any of the higher-order fourier componentents.  In some sense, the idea is we get high fourier components from sharp edges, so something like a square or a triangle is better.  For now, we are going to use a square grating, which gives a sinc function for the fourier components, so kappa(q) scales as 1/q, where q is the diffraction order we use. 

We know that we need 2 beta of backward momentum to make our mode go from forward to backward.  We use a dispersion model for a SVM waveguide that is 6um wide and 2um tall.  We use effective index approxiation to calculate the modes, so this is not perfect.  It is simply supposed to give an idea of what we should expect and provide order of magnitude estimates for grating periods.

Below are the dispersion and first-order grating periods we need to use.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/6F4328C3-DEE4-4E3A-9D61-BCE87B7F8582_2/2Nt1mqFtuecfYfyOFtt8dJ8u3TlFfVtTuL08TdTKJw8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/4473D9C9-A8CD-4658-81B5-B4421B4B01D8_2/A6DBoXboUs1HQCSzjfqMMysANf8QBt9hk7PJyOZukCoz/Image.png)

Grating periods = lamb / (2*neff), so small effors in neff give linear scaling to the grating period. We expect about 30 nm of bandwidth for the first-order grating period.  Each higher-order grating period has grating_order * 30nm of bandwidth.  So we must use the 13th grating period to get some overlap between the (i+1) period and i period.  Below are the period for higher grating orders (which just scale linearly with the grating order)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/8749EC19-F722-443B-93C4-227CA3713E8E_2/LLsYyIxmr041zx2bemxlRymvr1AsDkHGR8eGP793Uf8z/Image.png)

The decimal should not be there on grating order, as it should just be integrer grating orders. Next, for 1565, I am going to plot the expected transmission spectrum for different diffraction orders.  I want to see how sensitive the output transmission spectrum is as we use higher-diffraction orders.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/5F3ED062-0290-41E0-AC89-22C6C8767D06_2/rYPKnlt1qQkAxl4etIP4PmBkjgN9PJQvJOr92BDr5hAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/EC111EFD-6D56-4D68-B3CF-15C0E08CB70D_2/IEQIeUaOuC4hilrF4lEiNdH4EKfQt8ktEhdGEMsPktMz/Image.png)

We used a delta_n of 1e-2 and length of 1cm.  There work as scaling factors.  Basically, we will always have a reflection at 1565, but the width of the stopband does decrease with order (as the kappa decreases with higher order).  I would say using a diffraction order of 10 is reasonable.  Just to make the point clear, below is how the expected grating period for 1565 for different diffraction orders

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/4F8A2A21-1893-496E-950D-30B57CA465AD_2/U5kro4499Mt4YgS0CxhL4ZTeeUKAPsMyw2oSQRrDBvoz/Image.png)

Given that we expect a poling period arond 14-16um, we basically know that the linear diffraction grating period is going to be less than the poling period.  So this is why we are bifurcating and doing seperate experiemtns with much longer periods to show how poling period can adapt to the underlying structure.  Something that is challenging is that we don’t know the exact dispersion model.  An advantge of the higher-order diffraction orders is that the bandwidth is larger, but the variance is amplified

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADDA8B52-137E-4835-AB51-DD363952CADC/075E74C5-F549-4DA8-8558-7DE2175E3639_2/mf5Fny1irL2Et8LkTxhDk1XmXuclqpxeQeJd1GsN7dMz/Image.png)

And of course, this variance gets amplitifed for higher orders.  So I think these simulations are going to be surprisingly useful, given that this varience is still in the 30nm of bandwidth given by the first-order diffraction from 1500nm to 1630nm