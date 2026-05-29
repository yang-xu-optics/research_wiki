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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/17ACEFDC-2B6F-4AFD-9666-AF78590D1353_2/EO3EJJQTghUyV6kxSFb6WOzoBwkyX0Z9sdetXBat1KMz/Image.png)

Layers 0 and 2 are DON.  Layer 1 is SRN.  I then plug these conductivity values into Ansys with the design below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/16B042A1-4908-46B8-BA79-7C7A038883B0_2/tjju7AW6rjAhKPpSQ9ao3rFdvHapvPSC5dmFKNe1jNsz/Image.png)

I use different oxide blocks in the bright and dark state, as their steady state values are slightly different.  The main point of interest here is what the steady state fringing is, as these devices will be mostly operated in DC steady state.

I am primarily interested in doing a scan to see when our large-device approximation starts to break.  This will give me a sense of the resolution and an approximate minimum resolution from fringing.  I am going to start with a period of 20, and scan the duty cycle (or how large the bright state SRN in the middle is).  I am going to do 10, 5, 3, 1

Period of 20, duty cycle of 10 (20.10)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/EEC77AFD-23B0-4085-B499-AD881D961F1B_2/nwPWQFQpxOz5SPHhyB2mCJyLzZPFtbXNbK5LqISqhHIz/Image.png)

20.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/04E49B7A-6374-4AC5-8331-A36AD07A0CE9_2/VvoWuMoibwnZD6hgoiYVpTbRBdf4vsnUN9q5uCX7REIz/Image.png)

20.3

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/FEB0C235-9FF2-4F1F-AF28-F373168153C9_2/Zizfi2rR93tlpJwNyT908P7jZhp6zZNtZEAd294dIDAz/Image.png)

20.1

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/CF8B6AD0-FD5E-4CAD-B817-7CA86A1CD432_2/elRBKJoRYfkSZEELfR6n3oaEmt4ys4ABcCah3eTPWToz/Image.png)

Now do 100 nm (test limit of this good resolution)

20.01

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/6807F61C-1117-45C6-B809-808B333BA95C_2/VBWx5SsEVCfOiV71EypQ4FGTyl9DtMQlyoScJ4uzyGAz/Image.png)

So I can’t make perturbations arbitrarily small and maintain good resolution, but on the scales I need, I can make stuff pretty small.  Next, lets do large period.  The hope here is to see when we loose upper resolution in the dark state (As it seems that most of the smearing happens there).  We will do 15, 17, 19

20.15

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/3AEB7BBE-D417-46A4-9753-7BF2197DC10E_2/6kwhmp3xQoF5zAAlYriC2W3KfxzKKFv9gN1wlJ1we1kz/Image.png)

Notice how the edges are getting more slurred.  This means that our max contrast is a bit cecpetive, as there seems to be about 2.5 um of slurring on each side.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/CDBB0568-408E-47AC-A943-3AD0A1BE335D_2/2YvAR4wZ7YbwF1WylYBhPznq2u3Bw9EyAXNdqZiXtj8z/Image.png)

20.17

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/64C5C5F4-CA55-4868-9938-49C6B927D406_2/NYAovoSlTTToxEp9wndQYZyd89hZAPdGGsFIMnNKz18z/Image.png)

We can see the max field has gone down in SRN_Dark, but otherwise our analytical soltuions are holding in the bright areas.

20.19

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/63C53C2D-83DA-4F16-9117-E5B46C01F873_2/y05H8cn5GE1ZbuUWNqTbkygfhy6BWIBTFjPFaTrslQYz/Image.png)

Now lets plot the results:

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/12A26ACC-522B-41BA-B847-9C179CB83757_2/ului4HA6NmT8ukrDcfewWSLxx0ExgbaDyEp0rW4SaIwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/447D4F2B-995B-4E22-9C47-838FC41A3B55_2/5ml57cjMHjupbociHLGqkBQkDwfSDkanoZIN1kWsYgwz/Image.png)

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/C5960D40-B2D1-4B17-8A6D-DE5081BA68E3_2/q2gRxszGBl9ORyP15Z9eXe20Ex7FdMOLWWPjBXgL4h4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/83119E39-7ACA-46CB-8A02-F5A58683BB84_2/V6wqOPxp3yxgiskQI0ve59hEF1tOkSmnerdV2wXqoVwz/Image.png)

Top:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/0FFE8031-7722-4153-81DE-B7A42456F3D1_2/1FStTvvIw9SVWzRe36mYmUyO5GVSZrrB9xOtrYWo3soz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A7BE03A4-F64F-4DB3-A45E-9D85803E930C/43D82A47-344C-4103-92AB-A7B3DA98ED8C_2/04NB0WnkFRBmH3jPKI2J9MxoG6g3jx9uRymSkYsK3EQz/Image.png)

We observe a few interesting effects.  The first is that we get better contrast with a smaller bright region than dark region.  If effects from poling dury cycles are symettric, this is desirable.  It seems Duty cycles (so width of light region) of 3 um → 12ish um can maintain 100 V/um of contrast.  This is obviously specific to this device and whatever period we use, but simulations show our Analytic poling for a device like this is around 18um, so this is useful knowledge.  Secondly, the middle of the waveguide has a bit less contrast than the edges.  Lastly, fringing effects happen in the dark parts of the waveguide.