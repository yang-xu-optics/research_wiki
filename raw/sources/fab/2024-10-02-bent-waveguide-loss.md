---
type: craft-export
title: "2024-10-02 bent waveguide loss"
craft_document_id: F1331F5B-C29C-4310-BE5D-821DBD390276
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-10-02 bent waveguide loss
This has been a long time coming (I think I am three weeks late on doing this)?  The purpose of this document is to describe how I calculated the loss of my bent waveguide modes.  The videos below are what I used:

[Bend Analysis with Lumerical Mode — Lesson 3](https://www.youtube.com/watch?v=U-v1ySEDZ08)

For mode overlap loss (as bent modes will have slightly differnet propagation constants).  

With 100 um bend radius

![Image.png](../../assets/fab/2024-10-02-bent-waveguide-loss-001.jpg)

With no bend

![Image.png](../../assets/fab/2024-10-02-bent-waveguide-loss-002.jpg)

So the bend of 100 um caused loss to go up by 10X.  Now we have all we need for a sweep.  

![Image.png](../../assets/fab/2024-10-02-bent-waveguide-loss-003.jpg)

Now lets do a quick scan of different etch depths.  Generally, I would expect some incomplete etching to increase the loss, as the confinement is worse.  Below is the full plots for a lossless core of bend waveguide losses

![Loss plot for wall height0.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/F1331F5B-C29C-4310-BE5D-821DBD390276/99EDC558-D47B-48E1-9292-3724EEAC77C2_2/A6Oo1kkXzpQzoZCeyRR8wZdVl0YIiLIlnAChRVhjcH0z/Loss%20plot%20for%20wall%20height0.0.png)

![Loss plot for wall height0.375.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/F1331F5B-C29C-4310-BE5D-821DBD390276/FB1F8399-0A63-4BBC-B814-A95DB6F94C74_2/C0PUfSSy40UAinF48U8bwZyRgdG06DcXX5coybmesucz/Loss%20plot%20for%20wall%20height0.375.png)

![Loss plot for wall height0.75.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/F1331F5B-C29C-4310-BE5D-821DBD390276/AAE4C609-242D-4744-A5C1-5C1D12CB04F2_2/NEFzW0exQw6ipboxXOy05bOx7HwdCeLYYkTfyAAY2oYz/Loss%20plot%20for%20wall%20height0.75.png)

![Loss plot for wall height1.125.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/F1331F5B-C29C-4310-BE5D-821DBD390276/33B239D9-6EC9-43D2-829B-4B29087FA9D5_2/N9CuWfyyxcf098YfGy1bp5TdYPRMlhWE0LVrr3oIF3sz/Loss%20plot%20for%20wall%20height1.125.png)

![Loss plot for wall height1.5.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/F1331F5B-C29C-4310-BE5D-821DBD390276/79898FC9-6907-4425-A03F-A2D56AE40916_2/rS4r9eH9vELzJtYojeGX3yCivKoy6c8njeVYyBxO2p8z/Loss%20plot%20for%20wall%20height1.5.png)

We are probably going to use a sidewall height of ~1um, so anything above a 100 um bending radius is good.  Because our features are huge anyway, I say we use a 400 um bend radius just to be safe.