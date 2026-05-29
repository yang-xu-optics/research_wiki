---
type: craft-export
title: "2024-12-06 final dc ln device for 800 nm with annealing b38"
craft_document_id: 2B9DDD52-174D-4392-AB41-FCA949D90DDB
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-12-06 final dc ln device for 800 nm with annealing b38
Given our new measurements with B38 annealed, I am going to update our simulations for this type of device just to make sure everything looks ok.

A general pdf of the code is below, but I will also include some highlights

[2024-12-6 B38 DC LN Device.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/2B9DDD52-174D-4392-AB41-FCA949D90DDB/5542649E-CA0A-4547-82E2-FDFF5268C9B7_2/nUKDqT5no47yIJ9g4wLGQD1gGzOM5FHJtPCMr57ObQAz/2024-12-6%20B38%20DC%20LN%20Device.pdf)

Modulation efficency: 

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-001.png)

Substrate loss

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-002.png)

Delta_n perfomance:

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-003.png)

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-004.png)

Steady state field

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-005.png)

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-006.png)

A generally interesting thing to note is that the max field in DON occurs in bright state, not dark state.  So that is what I am plotting above.  Because it is more conductive than SRN, it seems to ahve roughly constant field

Transient solution (SRN constrast = 300, volt = 545)

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-007.png)

Below is the relevant plot for DON breakdown (just trust that SRN is fine)

![Image.png](../../assets/fab/2024-12-06-final-dc-ln-device-for-800-nm-with-annealing-b38-008.png)

I don’t love how close some of the capactive regions of DON are getting to breakdown, but oh well.  My feeling is that the permitivity could be higher than I am guessing.  We also don’t perfectly know the LN conductivity, which could mean we are lower.  I am a bit scared the SRN won’t have as much contrast as I would like, but that can be solved with a more intense top imaging setup.