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

![Image.png](../../assets/fab/2024-10-02-bent-waveguide-loss-001.png)

With no bend

![Image.png](../../assets/fab/2024-10-02-bent-waveguide-loss-002.png)

So the bend of 100 um caused loss to go up by 10X.  Now we have all we need for a sweep.  

![Image.png](../../assets/fab/2024-10-02-bent-waveguide-loss-003.png)

Now lets do a quick scan of different etch depths.  Generally, I would expect some incomplete etching to increase the loss, as the confinement is worse.  Below is the full plots for a lossless core of bend waveguide losses

![Loss plot for wall height0.0.png](../../assets/fab/2024-10-02-bent-waveguide-loss-004.png)

![Loss plot for wall height0.375.png](../../assets/fab/2024-10-02-bent-waveguide-loss-005.png)

![Loss plot for wall height0.75.png](../../assets/fab/2024-10-02-bent-waveguide-loss-006.png)

![Loss plot for wall height1.125.png](../../assets/fab/2024-10-02-bent-waveguide-loss-007.png)

![Loss plot for wall height1.5.png](../../assets/fab/2024-10-02-bent-waveguide-loss-008.png)

We are probably going to use a sidewall height of ~1um, so anything above a 100 um bending radius is good.  Because our features are huge anyway, I say we use a 400 um bend radius just to be safe.