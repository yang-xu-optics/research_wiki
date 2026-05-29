---
type: craft-export
title: "2025-12-02 dispersion calculation for resonators"
craft_document_id: 5F862063-AD1B-415D-AE69-DB8967292A6F
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-12-02 dispersion calculation for resonators
We want to simulate the dispersion parameters for SiNx waves for ring resonators for AIM photonics.  In lumerical, we are using teh palik disperiosn model for SiO and the Luke dispersion model for SiNx.  Mode 1 is fundamental TE, Mode 2 is fundamental TM (we can tell by looking at the effective indicies.  TM should be slightly lower, which is the case that we confirm).

We now want to run a sweep over wavelength and waveguide width.  We should run a pretty big simulation, and collect the ng and neff.  We will do so for mode1 and mode2 (as there might be some utility for doing this as a TE/TM mode coupling).  For wavelength range, lets do 1500 nm to 1630 for FH (as that is what our tunable laser can do), and 750 to 815 nm for SH.

We must set the waveguide thickness to 800 nm.  No sidewalls either (complete etch is assumed).  We will do widths from 1 um to 2.5 um.  I say we have 260 wavelength points and 25 waveguide width iterations.

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-001.png)

Above is a picture of a 2.5 um by 800 nm waveguide, with the appropriate buffer regions

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-002.png)

E-field of fundamental, which looks right, as TM should have a bit of field above and below waveguide in the tight-confinement direction

183.922 THz is 1630 nm.  199.862 THz is 1500 nm.  So lets simulate from 183.922 to 199.862.  Recall that a THz is 1e12 Hz.  The simulation is going now, so we just wait.

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-003.png)

Above are the effective indicies of my modes.  I had to cut one width that had some computational issues, but the trend is very obvious.  Below are the ng and GVD calculiations

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-004.png)

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-005.png)

There are just there very weird points of discontinuity at specific wavelengths.  I generally prefer when things are a bit more continuous.  These are at specific wavelengths, so lets maybe look under the hood a bit.

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-006.png)

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-007.png)

We just get these annoying discontinuities.  I would almost prefer to go from GVD back to ng, as we at least know what we should get.  The problem is we don’t know the offset.  ng has these annoying discontinies that I can’t explain. I suppose we can just pick a group index that we trust

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-008.png)

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-009.png)

Funny, no matter what, there will always have these annoying discontinuities.  I don’t think it matters a lot, but I don’t like the visual.

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-010.png)

Above is the dispersion data.  If possible, I would like to stick with 1.5um as the width of our waveguides.  I got the frequency scan feature to work in ansys, so I will proceed with that.  Well, the freuqnecy scan actually does not work.  So Below are the figures I am happy to send along

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-010.png)

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-008.png)

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-009.png)

We can just explain the discontinuities from discretization errors.  

![Image.png](../../assets/fab/2025-12-02-dispersion-calculation-for-resonators-011.png)

We will use 1.5 um as the waveguide width