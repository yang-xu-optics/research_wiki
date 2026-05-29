---
type: craft-export
title: "2024-10-06 final ln dc device design"
craft_document_id: 24FE4A07-302A-4DCA-8604-20E03C8F8EC0
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-10-06 final ln dc device design
This document is merely going to be a concise summary of our design parameters.  Below are the plots for ideal SRN (5e-16 to 5e-11) scanning over DON parameters

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-001.png)

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-002.png)

From this, we suspect that, as long as the DON is around 2 to 2.5, we are probably safe with the thickness.  Cond0 is not super sensitive.  Next, we do SRN sweep, roughnly with the conductivity data that matches the annealed films.

B28

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-003.png)

Below are the delta_n simulations for cond0 SRN = 1e-15

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-004.png)

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-005.png)

From this, we suspect that a thicker SRN is better (as long as we apply higher voltage).  I say a thickness of 2 um should be fine.  From the plots below on Bright and dark state conductivity, we can find the optimal SRN

![Screenshot 2024-07-28 at 3.19.05 PM.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-006.png)

![Screenshot 2024-07-28 at 3.18.55 PM.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-007.png)

Looking at the dark state, anything between 4 and 5 sccms is good.  More silane is good because we can use lower voltage and have less substrate loss.  Less silane is good because we get better modulation efficency.  Below are the indexes I think I will use

DON

![Photo from Library.jpeg](../../assets/fab/2024-10-06-final-ln-dc-device-design-008.jpeg)

SRN

![Photo from Library.jpeg](../../assets/fab/2024-10-06-final-ln-dc-device-design-009.jpeg)

Below are the index related results

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-010.png)

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-011.png)

This is probably fairly optimal.  I say we still try to shoot for 2um for each film.  

Our final stack should be 2um DON B28, 0.7 um of X-cut LN, and 2um of SRN 4.5.  For the transient solution, we get

![Image.png](../../assets/fab/2024-10-06-final-ln-dc-device-design-012.png)

Bottom is dark state, top is bright state.  We get ~1 Hz operation speed.  Again, if we used more conductivity SRN or cladding, this would probably be faster.  The voltage here is 460.  A little slow, but oh well.  

