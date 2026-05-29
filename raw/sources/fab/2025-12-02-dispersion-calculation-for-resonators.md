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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/02FFB2E1-E91B-4E78-A31E-4703DA418E07_2/4Tn8RxgdMqNHRtItPx6GvSyCI6OqgYQKEN1sYjmheicz/Image.png)

Above is a picture of a 2.5 um by 800 nm waveguide, with the appropriate buffer regions

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/514ED01F-17D8-45F8-BD27-9D507A9D5F8E_2/wltU6g7nESHZz21j6E74mlKWBXrI8DRzRqrYd6y9YZoz/Image.png)

E-field of fundamental, which looks right, as TM should have a bit of field above and below waveguide in the tight-confinement direction

183.922 THz is 1630 nm.  199.862 THz is 1500 nm.  So lets simulate from 183.922 to 199.862.  Recall that a THz is 1e12 Hz.  The simulation is going now, so we just wait.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/BF400033-3CEA-4A32-A832-90B27A48F768_2/KifiHv9Upu9aNQ0vcOZxakpdxif9Fdz6HqLFQDocZlkz/Image.png)

Above are the effective indicies of my modes.  I had to cut one width that had some computational issues, but the trend is very obvious.  Below are the ng and GVD calculiations

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/983D899F-D0D7-4914-9E13-8C8CABAC8572_2/L6UZgi1V4ja8GqX2VKfIqVuxhvZBeawqLLxtxJZNqhYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/0C3EDA9A-11C9-4097-9C08-2B842582518D_2/TcXV5bLvnhin3SJjM1oXhI1aX9Yy2caR1HDgE4deLrMz/Image.png)

There are just there very weird points of discontinuity at specific wavelengths.  I generally prefer when things are a bit more continuous.  These are at specific wavelengths, so lets maybe look under the hood a bit.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/CEBC5B56-D994-47EF-A835-13620EAD7BD4_2/gTsDoYIqkuxJ8rMI0iXgT0bKyZMNpUuuHbxfMeHip8sz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/E27AD3A0-47AC-4E98-BA23-3D1ED83AED3F_2/pND7QmYye8KjyBvggP8EHNmcDOR6OMDrGZzL3X9ExX0z/Image.png)

We just get these annoying discontinuities.  I would almost prefer to go from GVD back to ng, as we at least know what we should get.  The problem is we don’t know the offset.  ng has these annoying discontinies that I can’t explain. I suppose we can just pick a group index that we trust

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/8B076EC6-8D4D-4979-AE74-B26C21C07EF5_2/Z5eyCkiyfji1XpZq6Ifl2Xz3U0zx2clZpJQxDyt0YmYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/CFB1BB72-3553-43CA-A985-3FCCB13C10C3_2/xxtYwX9hrcHHSq45UiefJMIGY1gEOWHQrrJGOi16xqgz/Image.png)

Funny, no matter what, there will always have these annoying discontinuities.  I don’t think it matters a lot, but I don’t like the visual.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/E51DBDE2-621E-4440-AF24-6D5772DAA2EE_2/Kvp76ltrCjydvTD64RW26ZCxtrNWiZDhsgcxX3lOMDEz/Image.png)

Above is the dispersion data.  If possible, I would like to stick with 1.5um as the width of our waveguides.  I got the frequency scan feature to work in ansys, so I will proceed with that.  Well, the freuqnecy scan actually does not work.  So Below are the figures I am happy to send along

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/E51DBDE2-621E-4440-AF24-6D5772DAA2EE_2/Kvp76ltrCjydvTD64RW26ZCxtrNWiZDhsgcxX3lOMDEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/8B076EC6-8D4D-4979-AE74-B26C21C07EF5_2/Z5eyCkiyfji1XpZq6Ifl2Xz3U0zx2clZpJQxDyt0YmYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/CFB1BB72-3553-43CA-A985-3FCCB13C10C3_2/xxtYwX9hrcHHSq45UiefJMIGY1gEOWHQrrJGOi16xqgz/Image.png)

We can just explain the discontinuities from discretization errors.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5F862063-AD1B-415D-AE69-DB8967292A6F/E8384D06-34DA-42E5-84A9-8BD363772022_2/l4V5qSZQquKwCvmBdL5zLvq4EBPdPhbnFBDqQxqlAzoz/Image.png)

We will use 1.5 um as the waveguide width