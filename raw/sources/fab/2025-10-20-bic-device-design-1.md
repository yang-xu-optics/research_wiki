---
type: craft-export
title: "2025-10-20 bic device design 1"
craft_document_id: DAE04443-D39B-4382-8D40-4AA7B8BEE7FC
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2025-10-20 bic device design 1
Currently, we are using the DC device designed here to show bic: [https://tdwg.craft.me/fpch0H0frO3xIx](https://tdwg.craft.me/fpch0H0frO3xIx).  This device, if you trust our past notes, showed roughly the highest delta_n.  But, it seems in experiment we are barely reaching 1e-4 as the delta_n, so it would be nice if we could increase this a bit.  My guess, FWIW, is we can probably juice another 2-4X out of better device design.  We will see.  Below are some of my guesses, just for the record, of some experimental choices that could be hampering device performance.

1. We might need more illumination power.  If this is an illumination-induced chi3, then I would presume more power helps (unless there is some saturation effect)
2. We might want to use a different wavelength.  Again, given that illumination is what helps, using a different wavelength might excite more or less charges in a way that benifits us.

But, for now, we are going to focus on device geometry.  Below are the things we know about how devices work in DC

- It seems that we are using DC kerr.  So getting more field in the waveguide core is key to getting better performance.  This means, in both bright and dark state, we want the core photoconductor to be far more insulating.
- It seems that our devices rely on illumination to induce an index change.  This means we want to get as much illumination power into the core as possible.
- It seems that loss is less important (we can always just blast the waveguide with EDFA if needed).  So lets focus less on loss (which we cared about more in the past).

From these bullet points, below are some ideas (before any real simulations are done for geometry)

- SRN3 seemed to be the lowest silane flow recipe at room temp (which all of these will have to be, as I am fairly convinced annealing will cause some wild results and likely crack things).  SRN2.7 technically allowed some light through, but I don’t want to go too low for now.  I am going to assume SRN3 is probably the most insulating (and has the highest breakdown).  I am also going to assume it has the lowest chi3 (and probably induced chi3).  So using this film will really be a test of whether higher field is the best approach.
- Alternatively, we can try something where we see if more silane (meaning higher native and possibly induced chi3) is the approach.  This means using a more SiH4-rich deposition proceedure.  Of course, to preserve the above resistance relation, it would need to increase the conductivity of the claddings.
- I would generically say we should aim for thinner claddings.  The bottom one needs to be a bit thicker to prevent loss into the substrate, but the top cladding can be a bit thinner (I don’t want too much loss into the ITO, but I am more concerned about getting our illumination into the core).
- I think a thicker core is generally adventaegous.  We want our modulation efficiency to be as high as possible, and this will help us get more conductive and thinner claddings that push the limit of the possible cladding index (as we know conductivity and index are very much coupled for these).

So I guess the general question for DC devices is: whether it is better for have more Si (and higher nature chi3 and possibly greater induced chi3) or whether it is better to hvae less Si and greater breakdown voltage.  Personally, I will always be biased towards the latter just because of the scaling.  Still, I should give this full thought.  My take is, if we fabricate SRN3, SRN4, and SRN5, this sweep of optimized devices should give us some idea of which direction to go.  My general take is higher silane, at some point, will start to get lossy and annoying with the required claddings.  So I think it is just easier if we scan this range, and if SRN5 works the best, we can explore future devices (possibly AC with a-Si) in that direction.  

Assuming we stick with the induced-chi3 approach, I am very condident that the DC method is better, as you really don’t want to be limited in anyway by the breakdown of your claddings. 

For AC, you are using theh conventional voltage-divider technique, and the delta_n ideas are reversed.  For that, you probably want a large difference between bright and dark conductivity whlie maintaining a decent breakdown field.  Martin had trouble with this approach, so I am not confident it will be super prosperous for us (as breakdown will quickly become annoying).  I say we stick to DC devices in this test.

Again, to emphasize, we want to use claddings that ensure the core always dominates the resistance.  That means we have to adjust core thickness to prevent too much leakage.  I don’t think it is worth it to run any electrostatic simulations, as we really don’t know what any of these conductivies are.  We at least know what works for SRN3.5, so we can use that as a baseline.  I will have to use some of my old notes to calibrate these recipes.  It would also be nice if everything happened with 350 C as the dep temp, just to make things easy and consistent.

## SRN3 Device

core_coeffs = [1.861, 0.02278, -0.00235], so n_1550 ~= 1.87.

In the past, we used B8, which had the following deposition parameters:

B8:

Temp: 300 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 475 sccms

Power: 10W

N2O flow: 160 sccms

It deposited a film with [1.828, 0.04337, -0.00658] and n_1550 = 1.85 before annealing.  After 350 RTA, we had [1.852, 0.04457, -0.00590] and n_1550 = 1.87 after annealing.  Keep in mind, there was  a bit of a native oxide here, so I don’t fully trust this number (I think it is a bit low). 

Lets try cladding n_1550 = 1.85

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/1EDAD6D0-66CA-4205-9AC6-342CEBC189C6_2/yD4yWnLWl2fyELt1DxIt43m5kI2eT6AMXfTst5vjyywz/Image.png)

cladding n_1550 = 1.825

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/092A7812-E2E2-4DF6-B88C-2491CE227780_2/jqaC6QaV3jwVJgVbftDER6vkjWn8l4IHEMxe9XXWuE0z/Image.png)

cladding n_1550 = 1.8

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/2EF29DD1-FC9F-445C-8AED-247F9D8C747D_2/4fXPcCNPOT2R7boFhsB6LWcUDavS0N43kDNPJKWU9cUz/Image.png)

Well, it seems from that that we want at least 2um of SRN3.  It seems that an index of 1.825 → 1.8 is also ideal.  Now lets do substrate loss assuming d_core = 2um

n_1550 = 1.85

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/7CFE1517-5C09-4F97-8C75-71D53307F551_2/5Pgrqbc4XmjiRIgFuPFfq9C842tKVogzfkZQSUlwAtAz/Image.png)

n_1550 = 1.825

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/2754155D-93B7-4AF5-9A59-9DC82F08908B_2/eDaQqSLeGXR3SCR6izK1ExNOPjU8dsOkYjaxIoKfAqYz/Image.png)

n_1550 = 1.8

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/6B775C0A-9E58-4C81-ADE3-C3CF70355B1B_2/ED7ir1noR5JvK6RxjNxQvEnoVlSxhCKagmOMfKAx7QYz/Image.png)

Just for some context, below were some of my old designs:

Below used B8, but it was annealed at 375, which caused the index to go up a bit

SRN3.5 device:

Cladding index: 1.892

Core index: 1.916

Bottom cladding thickness: 3um

Core thickness: 2.5 um

Top cladding thickness: 3um



I used B12 for the below devices (not B8)

SRN6 device: 

Cladding index: 1.846

Core index: 2.174

Bottom cladding thickness: 3um

Core thickness: 0.9 um

Top cladding thickness: 1.5um



SRN8 device:

Cladding index: 1.846

Core index: 2.298

Bottom cladding thickness: 3um

Core thickness: 0.9um

Top cladding thickness: 1.5um



Below is on B8 (I don’t know the index for sure, as annealing would effect things during SRN dep)

SRN4 device:

Cladding index: 1.86

Core index: 1.962

Bottom cladding thickness: 3um

Core thickness: 1um

Top cladding thickness: 1.5um



SRN4.5 device:

Cladding index: 1.86

Core index: 2.03

Bottom cladding thickness: 3um

Core thickness: 1um

Top cladding thickness: 1.5um



SRN5 device: 

Cladding index: 1.86

Core index: 2.095

Bottom cladding thickness: 3um

Core thickness: 1um

Top cladding thickness: 1.5um



We observed in the past that SRN4 worked pretty well.  So while we would like a large conductivity contrast, perhaps that contrast needs to only be like 0.1 to make things work.  SRN5 was the cross over point, so I would suspect 0.2 difference is not good.  Again, I am making a somewhat hazy assumption that everything scales (in both DON and SRN) the same way with index, which is probably not true but a fine approximation to build a rough bound for now.  So given our core index of 1.87 for SRN3, I think we can safely go with a cladding that has ~1.825 (leaning on the lower side). Below is our mode for these indexes

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/E8166AC9-9F7B-453E-9FB1-B8177B35BB39_2/UwSnWcsA91E9rbjJNxpEBXyWZn5JxtChxynohDInjocz/Image.png)

Above is what we expect.  Ignore the x-axis (I had to make it larger to get around the boundary condition at the edges being zero).  Either way, I am generally of the opinion that 3 on the bottom is probably fine, and 1.5 on the top is probably fine, though I think going for an index of 1.8 or a bit less is probably safer.  I think we should stick to the 0.7ish less rule.  Again, I don’t think ITO is going to kill the device, but I would prefer to be a bit safer given how long these depositions are going to take.

**So we want 2um of SRN3 as the core, 3um of DON bottom, and 1.5 um of DON top.  We want this index to be ~1.8-1.825.**

## SRN4 Device

core_coeffs = [1.945, 0.04418, -0.01089], so n_1550 = 1.962

Now we are going to scan over a few cladding indexes

n_1550 = 1.9

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/7340667C-8812-428B-A631-6E26BAEE212D_2/rcf0QVa4EWgVQ02TM0P9Yd63XssQr0bd4zCSN9AXebUz/Image.png)

n_1550 = 1.88

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/8676AE4E-6358-44DB-80AB-4D18091F5888_2/WxZeUimnG3IJaBHcMc1OZLk3O73cQ09NI7Oi6512aBkz/Image.png)

n_1550 = 1.92

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/278FEFC3-2C94-4112-8B75-E47DB284DAEB_2/OE42kFAuWKwopmcs6JNniFBApcxal4qn81qZbZRR5VUz/Image.png)

So we want 1.9 or less

Now for substrate loss.

n_1550 = 1.9

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/CABB9C4E-6015-45A6-B38D-2A200F04EEB1_2/A5b0mX9aL9evhIYLfeADhVkcQnTU1hO9dOHrmlNJZcQz/Image.png)

n_1550 = 1.88

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/8ED12E80-E505-4577-95CE-105E721FF450_2/2pNECm8RLFgj60UwFFQyrLUPlJ4e0vDKKiYf03ZrvWIz/Image.png)

n_1550 = 1.92

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/B81BBF5F-BD4B-4F4B-BFAF-5B0BC08A4EF1_2/GumxpUgH59HMcs4Ay7KXp4nO13O2mTbwxJ0aYBY2OkQz/Image.png)

I think slighlty under 1.9 makes sense, so we will do 1.89 as the index.  I am genreally biased towards the 0.7-0.8 index seperation if previous devices are to be any guide

Below is a rough plot of the mode shape.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/3664C3A6-085E-487E-B53D-F4A6AC19A82D_2/GGEcQ60q1M1ivELxabWbQDKZf5BnuNJcMRJjeFCdNWYz/Image.png)

So it does just seem that higher index, off piste, helps.  I think we go for the same geometry of 3um below, 2um core, and 1.5 um top cladding.

## SRN5 Device

core_coeffs = [2.077, 0.04981, -0.00853], so n_1550_core = 2.096

now lets sweep the cladding indicies

n_1550 = 1.95

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/C2D3880D-5F2D-45C0-B8C3-91B068D9721E_2/ke2gtSJx84M7zC14MOWyHKlq7h1BMmXnRyGeK7HjiV0z/Image.png)

n_1550 = 1.93

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/E5B004D8-335C-4CEB-8B8A-6DA95EC7C548_2/ueCGVKEpkOpO9nsvYkkNfbcQy4gX8ePqwffSpkzYLtAz/Image.png)

n_1550 = 1.97

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/03C6287D-0FFC-45A6-AB66-1E5F4F67BAD9_2/QaHBZWTKh4VmSuy0JozLLIUrfrgBFbbWEFT3DYj3zNIz/Image.png)

n_1550 = 1.99

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/E9F39125-6E07-4F83-A33C-42EAE7EB3677_2/FyXc3VVcS6A4oydzydrbz18fJ7KiPsIMYL70Ru7ODroz/Image.png)

Now substrate loss

n_1550 = 1.97

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/95FBD19D-6EA3-437B-A780-A992F5AFC397_2/UrjwAcG2GCvqOwO93fwIvyiizeLOfzTWgfVy435xn5wz/Image.png)

n_1550 = 1.99

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/EE40D655-2F6A-43D1-8B1D-EBAC0B2EF3F6_2/cXfLQxg3EtcNy0zi1Cmxg7BFGkHO91ZYaSx1YRznys0z/Image.png)

n_1550 = 1.95

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/8CCA2DD3-72D6-46F3-A02D-2AC964BCE7CF_2/ezKZSiAoibdWUIx2vpA2SuDkRrWQFaHWl4u29yNusT0z/Image.png)

Suprisingly high cladding indexes can be tolerated.  I would say 1.98 is fine, and we could probably even go higher.  I will try that on for size below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DAE04443-D39B-4382-8D40-4AA7B8BEE7FC/4B0532E1-6A6A-4E80-8153-18599BD66CD9_2/EyNHKPsIkLSmHy8qZkTM7LAxwm5LSoWGSnfEr3ScyA8z/Image.png)

I say we do 2um bottom cladding, 2um core, and 1um top cladding.  Cladding target index of 1.98.  Say what you will, but because the cladding contrast narrows with higher core index, I am more bullish about getting these working in DC than before.  Now we just have to see the chi3 vs breakdown tradeoff.

At some level, I don’t know how easy it is to call all of his a perfeclty fair comparison, as cladding absorptions are going to be differnet.  But modulation efficienies are within 10% fo each other, and losses should again all be around 1 dB/cm (unless ITO really screws us).  Nothing is a perfect comparison, but if one of these devices should 2x greater delta_n, it is probably more of a winner and shows a more promising path.

After talking with Fan, I also checked the number of allowed modes.  SRN5 has two modes, and I imagine the rest are 1 or barely 2 (With a decent amount of loss).  So I don’t think multi-modeness is going to be an issue.

From previous experiments, we know we get a 0.05 index increase with higher temp.  90 sccms more of N2O causes index to go down by as much.  So, if 300 C and 160 sccms means an index of 1.85. 

So, for SRN3, if we want a film with 1.8, we should do 250 sccms of N2O at 350.  We can use this as a testing baseline and start here.

## AC Devices

Now lets give some thought to AC devices.  These work on the voltage divider principal.  We are still going to use three-layer devices, as they should be more efficient (and unlike the nonlinear project, we don’t care too much about SH loss).  FWIW, we don’t care too much about loss in general.  For this, there is still a bit of a tradeoff between breakdown and chi3, but there is also the added tradeoff with how photoconductive the layer is.  This makes me bias towards more Si-rich photoconductors.  

There is also the difficulty of the respective layer thicknesses.  It is not quite as trivial as it might seem on first pass, as a thickner oxide means we get a larger percentage change over the photoconductor, but at the cost of less field on the photoconductor and breakdown being dominated by the oxide.  At some level, we can just manufacture AC devices much faster.