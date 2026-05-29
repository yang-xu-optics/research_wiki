---
type: craft-export
title: "2024-6-2 nonlinear dc device 1 design simulation"
craft_document_id: A7BE03A4-F64F-4DB3-A45E-9D85803E930C
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-6-2 nonlinear dc device 1 design simulation
I did some DC device simulation, and came to the final device design.  The file below details the simulation results

[Nonlinear Waveguide DC Design.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/9090F64D-6B3D-47BC-9041-70CC4182B33D_2/08RoFiAWDoNAkwQXuZBYEBxeQIZo9KcsxZfZoyKkbd8z/Nonlinear%20Waveguide%20DC%20Design.pdf)

The important thing is that I use SiH4 = 4 and DON B12.  I can’t use SiH4 = 3.5 as the index is far too close to B12.  I might be able to adjust the decimal a bit.  Either way, the important parameters are the following:

Oxide thickness = 3um

Core thickness = 1.6um

Operating voltage = 950 Volts

I then plug the final fields into a conductivity calculator and get

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-001.png)

Layers 0 and 2 are DON.  Layer 1 is SRN.  I then plug these conductivity values into Ansys with the design below

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-002.png)

I use different oxide blocks in the bright and dark state, as their steady state values are slightly different.  The main point of interest here is what the steady state fringing is, as these devices will be mostly operated in DC steady state.

I am primarily interested in doing a scan to see when our large-device approximation starts to break.  This will give me a sense of the resolution and an approximate minimum resolution from fringing.  I am going to start with a period of 20, and scan the duty cycle (or how large the bright state SRN in the middle is).  I am going to do 10, 5, 3, 1

Period of 20, duty cycle of 10 (20.10)

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-003.png)

20.5

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-004.png)

20.3

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-005.png)

20.1

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-006.png)

Now do 100 nm (test limit of this good resolution)

20.01

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-007.png)

So I can’t make perturbations arbitrarily small and maintain good resolution, but on the scales I need, I can make stuff pretty small.  Next, lets do large period.  The hope here is to see when we loose upper resolution in the dark state (As it seems that most of the smearing happens there).  We will do 15, 17, 19

20.15

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-008.png)

Notice how the edges are getting more slurred.  This means that our max contrast is a bit cecpetive, as there seems to be about 2.5 um of slurring on each side.

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-009.png)

20.17

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-010.png)

We can see the max field has gone down in SRN_Dark, but otherwise our analytical soltuions are holding in the bright areas.

20.19

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-011.png)

Now lets plot the results:

Bottom:

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-012.png)

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-013.png)

Middle:

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-014.png)

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-015.png)

Top:

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-016.png)

![Image.png](../../assets/fab/2024-6-2-nonlinear-dc-device-1-design-simulation-017.png)

We observe a few interesting effects.  The first is that we get better contrast with a smaller bright region than dark region.  If effects from poling dury cycles are symettric, this is desirable.  It seems Duty cycles (so width of light region) of 3 um → 12ish um can maintain 100 V/um of contrast.  This is obviously specific to this device and whatever period we use, but simulations show our Analytic poling for a device like this is around 18um, so this is useful knowledge.  Secondly, the middle of the waveguide has a bit less contrast than the edges.  Lastly, fringing effects happen in the dark parts of the waveguide.