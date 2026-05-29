---
type: craft-export
title: "2024-4-7 ln dc device simulations"
craft_document_id: ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-4-7 ln dc device simulations
The purpose of this document is to see, for a three layer device, the range of tolerance we have for the bottom oxide conductivity.  After chatting with Hiro the other day, he seems very bullish on the prospect of making a DC LN device.  His idea was to put a more conductivity bottom cladding as the bottom layer and then use Ryo’s SRN as the top cladding and photoconductor.  The purpose of this simulation is to use reasonable parameters for the LN and SRN layer and see what conductivity values for the bottom oxide cause our device to steop working.  What I am basically worried about is the bottom oxide acting like a virtual ground, which will cause the field lines to all be orthogonal and we will lose our pattern.  If this does not happen, creating an LN device will be a piece of cake.

Here are the parametesr of our device that are constant:

top cladding: eps = 8, cond_dark = 5e-9, cond_bright = 5e-8, h = 2um

core: eps = 27, cond = 1e-9, h = 1um

bottom cladding: eps = 5, h = 2um



For cond = 1e-10 for bottom cladding, we get the following result

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/041FEBAA-5CB7-4B7F-B3A5-53BB31AF6C24_2/KpZmdveDrux9Cf2lHKsbcDyb9nsLyj6A8qZZdnyVad0z/Image.png)

For 1e-9

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/8D41B707-747D-4D94-A5B1-428000F44FC6_2/t9McfnJ9PQIcqG0GIJmgMiPCn7imeXNq6FxOHPIlrhUz/Image.png)

for 1e-8

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/58149F23-CCB6-4EFE-AB65-5B6640BFF167_2/Jyl4UoPAAaE6WDBxjRV2fv9lv1FR3yu7qeg7fvuUWz0z/Image.png)

For 1e-7

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/493E0562-0DB5-4FEE-AEBE-FB4402DACC07_2/PBSj4GPmzipGuwz5SYGa7xStvrkGOdlx9WwvBrq8g7wz/Image.png)

I don’t quite understand why the bottom oxide is purple, but we do see changes here, so evidently the conductivity changes are working.

For 1e-6

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/4198443F-0780-47F6-9A62-CB80EB2FE8CF_2/5VoDFKLPbDP5O38DAyEpeRyWxp1WR0831KKvVwNxJrUz/Image.png)

For 1e-5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/2987A20F-C53D-4F0D-BBED-0FF7591F480A_2/5wnxYcndHERN7PM0URwrSQYpSV1eN4M4u5TOCpxbRQkz/Image.png)

It seems to be saturating a bit here.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/6D8305D9-6772-4C88-920B-A5146AF6486D_2/OP1j6Qygz2iZURZRUJRMyYhpXNeiO5C1eh40CqSoMz8z/Image.png)

All the fields are pointing down, so the orthogonality condition for the bottom oxide does not hurt our device.

Below are the final results:

Top

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/06270B52-013D-4782-BC3C-6599A41DF31E_2/uOxRJH9y0OgvZRU5ECDTxuYrcUdRCakmyik44uOR1vsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/0401873C-20D1-4BC1-9E5D-6129D8E13ECD_2/8QYwRFroiU0py6BKOC9lgiT7jS5sA8qOXRSPO4dyIiQz/Image.png)

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/1869D046-67BE-4201-A24F-DF5C36E6E174_2/Mvsp7RYFEpTKE7x76QPAzhfIOqWr0nuyyVY8u8yrBdUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/5FEF3B48-E568-4D7A-99B7-3AA939FC8FFE_2/Wjh0ycQkkSaQjzWilRzGb1HEXTs31DeCmb53q4bvUJwz/Image.png)

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/311B8D24-9844-461A-9647-388D6187E263_2/FxFTwzBY42ABxmwtnwyDZy2Ftif44VBOiufvvYns1Vwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/ADC8897D-E1A7-4E4C-BA6F-97CB6B82FCCE/95A34AEC-7933-4CA4-AAD1-EDD6ABEB5209_2/MVWPzzS0BNgRzLmQOFytyrgxceswxxroCVBo1x2jYI0z/Image.png)

Hiro was totally correct, more conductive bottom oxide is what we want.  We don’t need to conductivity match with a 3 layer device with the bottom oxide. It is also nice to see that hte fields seem to saturate, which is good too.  I was expecting a bit more of a switching ratio, but some more simulations might reveal some tricks there.  It could be that the SRN should be thicker or thinner to help us out.  I would also be curious to see whether having a thicker or thinner bottom would help.  Either way, these simulations were done with rather thick claddings, so either way I do see any good reason not to be optimistic. 

Below is a draft email to Mabel at nanoLN to inquire about getting an LN wafer.  I will probably be spending a decent amount of time this coming month working on the bottom oxide.  I want something that is at least a factor of 10 lower for conductivity than the conductivity of LN.  Hiro guesses it is somewhere between 1e-9 and 1e-10.  So anything lower than 1e-8 should be fine.  We should still give some thought at some point to what happens if we fall into the exponentially decreasing conductivity region at low field.  We might not wantt as huge of a conductivity swing for the photoconductor to make sure we don’t fall our of the linearly resistive region.



Draft:

Hello, 



My name is Ben Ash, I am a member of Peter McMahon’s group at Cornell University, and I work on the programmable 2D waveguide project with Dr. Tatsuhiro Onodera (cc’ed here).  We are interested in putting in an order for a custom wafer with thin film lithium niobate.  We would ideally like to send a wafer we have fabricated from Ithaca to you guys and for the lithium niobate to be put on that wafer.  The wafer stack that we would like to send you guys is as follows (from bottom up):

P-type doped NOVA silicon substrate with a sheet resistance of 0.01 ohm cm.

Approximatley 2 microns of PECVD thin film doped oxynitride.  To grow this film, we flow N2O, Ar, SiH4, and B2H6.



We are still working through the exact parameters of our device, but recent results in simulation and experiment have made us very intereted to see if we can get lithium niobate on the previously described wafer.  If it would be possible to do this, we have a few questions, listed below:

1. Is there any processing or cleaning you guys would like us to do to make this easier on your end?
2. We have not quite chosen the thickness we would like.  What is the possible range of lithium niobate thickness we could get?
3. What would be the lead time for a wafer like this?
4. What is the approximate price range for us to move forward with this process?

We will probably need another month or so to perfect our device design and to make sure we have the best possible recipe for the film beneath the lithium niobate, so we expect to send a wafer out in the middle of May.  



Thanks for your help, 

Ben