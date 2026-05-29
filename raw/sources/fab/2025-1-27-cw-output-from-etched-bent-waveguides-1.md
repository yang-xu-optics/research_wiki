---
type: craft-export
title: "2025-1-27 cw output from etched bent waveguides 1"
craft_document_id: 5844CC30-0BBE-43C1-AAF0-D0171B98429A
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-1-27 cw output from etched bent waveguides 1
Using the etched bent waveguides, we hope to learn a bit about adjusting the phase of different parts of the poling structure to show quadratic phase increase.  

So I am having a lot of difficulty seeing signal. Below is what I have for power of CW laser with everything running

![Photo from Library.jpeg](../../assets/fab/2025-1-27-cw-output-from-etched-bent-waveguides-1-001.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-1-27-cw-output-from-etched-bent-waveguides-1-002.jpg)

I don’t see any signal though. Now, when I plug the 

With the pulsed laser in

![Photo from Library.jpeg](../../assets/fab/2025-1-27-cw-output-from-etched-bent-waveguides-1-003.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-1-27-cw-output-from-etched-bent-waveguides-1-004.jpg)

I checked both signals with the card and we are good

Now we see signal

![Photo from Library.jpeg](../../assets/fab/2025-1-27-cw-output-from-etched-bent-waveguides-1-005.jpg)

I am poling the length of one waveguide

![Photo from Library.jpeg](../../assets/fab/2025-1-27-cw-output-from-etched-bent-waveguides-1-006.jpg)

My intuition here is that the setup is aligned, but something else is amiss. I am going to do a quick poling period scan, but I believe the crux issue here has to do with phase matching

I am also coupling 1600

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/BCE2E3A0-D9C7-4F72-B138-D43860EB04E8_2/Fzi8bexAx3lwWn8JdBNijAao8hhpCUy5qWZc97KBHLsz/Photo%20from%20Library.jpeg)

No signal, with zoomed in picked

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/F63969D0-2310-476B-A96C-A91B3D4025EC_2/C1ibyWyDDxdn707gYPnLfpTeJHcoIr2cwJI23w0TLxYz/Photo%20from%20Library.jpeg)

Notice y scale is a bit different 

Before, we found the ideal poling period to be 14.6. We are now going to scan around that

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/D9E9A1D2-1B96-4170-9E33-BF6E8B7F380F_2/bh8djeeYBfKx9MTPcEPiRcXQ5x5cXUXsDGvychlEKZkz/Photo%20from%20Library.jpeg)

Pitifully weak signal, could not see anything that did not look like noise. Let’s try to slowly vary poling distance 

What we see

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/02EC4FE0-003A-40E2-B6E6-B56696D14D86_2/xI7rMoT3YoKIyPMAfoqCRhBfeOeA7xh8hJOUX3uEkEkz/Photo%20from%20Library.jpeg)

Nothing useful yet.  I think the next best thing to do is pole a small length of waveguide and scan the poling period there

Still no dice

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/6AE3FC72-80F2-4938-AD0A-C7F8D631C185_2/aYnDMeNnyhOYQdaHqMB2lCnM86Px9E909Gf4rEPkdXkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/247B08E0-9970-4769-950E-2BB3CE53FCAA_2/ZVTovtyN3liFxrKiLIvN5QJmiIE95X4Xd3R8h5Dbelcz/Image.png)

This is a bit surprising to me, as we are literally poling a bent waveguide.  One possibility is that the material loss is higher than we think, and doing 3cm is the issue here.

No dice on other waveguide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/55D6EB8D-F172-4A01-AC1C-F86494EEA512_2/q4f6rKgqUZJoxJ9l8l8HEzmE0AyWxJ5loKJtu7rThigz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/63EFEAE2-D117-4959-AE1E-A1472BA8CDC0_2/0gCC3lbDtXiOflzxinxUtSbyQyJk1MQpc8fseziUfikz/Image.png)

Lets try a scan over a wider array of values.  While I know Ryo says we should increase the integration time, I can’t see anything with my eyes, which is the more concerning part.  I just don’t get why we have so little signal.  I don’t even think loss is a good explaination, as we saw nearly linear increase of SHG using pulsed light.  So I admit to being a bit dumb founded

Nothing for shorter region

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/86B20CA4-1BD7-43D2-B9A2-B8B50BA17E04_2/KhbkPzyy9yGrqHHeL30vMidx0yuIGhsyqpRjP8dIDxwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/163D9E98-E892-419D-BB17-D21B1CAD4F99_2/3T8xAEFAZtuz0HDVxRPtOZA8hGKjpOSv009sQl9yvesz/Image.png)

Ok, so this is still strange.  Next, lets do poling over wider range of poling periods.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/B3F122B0-4359-4833-83E9-545C59C56567_2/z9xSfq7FmoH6dBPWnEvXGCuVxJpdB0vRgk4rTlqnSZQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/D81D63D7-630B-4A14-9900-ACC6F44143AF_2/ntkyBL5KHu0ffVoz9l2ZJQeO7XgVmyOn9aRhtbmDuREz/Image.png)

Still nothing.  Honestly, very surprising.  Next, lets try to do some longer poling periods.  Maybe we just moved way off the beaten track

For the upper limit

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/FECA4046-856A-4876-9663-2C914ECA8548_2/boxNXepGOXTmZyMqdcwlf85IEpW3YozmDbpUTk7OAUAz/Image.png)

Below are Ryo’s old results

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/805AE22E-C22B-48C4-89AA-7B6E85C80134_2/0AKdy3W7IxBzPYtRN1BpVOn0JxvUja5AYO8Q02uE7O8z/Image.png)

From this, I would tend to believe that we should look much more closely at the 1600 range with 12.5 as the poling period.  That being said, we did just scan that area and see nothing.  Keep in mind, he did this on a straight waveguide.  But something else that should be noted is that Ryo did not see a crazy shift in poling period.  Here is a link to his note for future reference: [https://tdwg.craft.me/etOAf7NIpUAmHx](https://tdwg.craft.me/etOAf7NIpUAmHx).

Below is the Loss plot for bent waveguide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/D6023976-A2C0-441A-9D74-3D5F6264DE47_2/anBsyiwT5pER0x0XNJG3cQ8YrLnQoQvxxjjAAypROccz/Image.png)

I measured on the order of 0.8 mW coming out with fan turned off.  So it seems like we are close.  Plus, we are definately working near an optimal wavelength (of 1600), so I am now quite confused

Below is the plot as well for long poling of different straight waveguide.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/31EF8487-CBF5-4E8E-B79A-C2447515A774_2/MLi8rudeoCIAD3Ab0ilF47mzlqQCfktRH5QBCmrPMS8z/Image.png)

The point here is to say that I don’t have a good hypothesis for why this is happening.  I checked electrical contact (and most importantly, I already saw SHG with the pulsed laser anyway).  I think a key point here is that we are always below the noise threshold.

1600 power

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/A46708AE-4A8B-4A5E-A53B-02C4B929467E_2/MWAD2PgfUPs9WGauzVpDXvIcH3vUxyRxTNeZsw3rCcwz/Photo%20from%20Library.jpeg)

We loose some power going down to 1570, but this may still work

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/1EA72E8C-854E-4B75-9195-0C8FFEEA1B86_2/eokjAWsSLQAj4V2UDGRyzY71AEEQFOpd8YFpyYou7ywz/Photo%20from%20Library.jpeg)

Nope on 1570

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/5FB3F701-6222-4A62-8F91-E26434E6231E_2/khjZGz5MPFRzuvYsoCE62fx4J4KHXgBlBhnrIa6kBbYz/Photo%20from%20Library.jpeg)

We saw maximum SHG before at 790, so maybe try 1580

Still no dice

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/535D41A4-02E8-4A44-B8F6-9654D29B2F6C_2/8Wt7kShdC4FCqTJpedgRAZT40XAyeLMfbPZhSmLN6zEz/Photo%20from%20Library.jpeg)

Set the phase correctly, to make sure things are really overlapping correctly.  Add more samlpes in code.  Do extra integration.  More dark shielding, and increase the gain.  Power meter screen is pretty bad.  Easier to scan poling period than wavelength

So far, fine scan of poling period has not yielded any useful results.  This is really quite surprising.  For reference, our scan is from 14.5um to 14.75um with 4000 points.  This means a fineness of scan of 0.0000625 um.  For reference, Ryo’s previous scans had a fineness of 0.04 um.  So we are definately doing fine.  While we can expand the range of poling periods, I am really not sure that will help.  I just don’t understand why I see nothing.  Maybe just try a different waveguide? There is nothing that should make a bent waveguide so fundamentally different than a straight waveguide.  Shoot, we should just try to couple into a straight waveguide and see if we can reproduce the earlier results.  It might also be possible that are coupling into weird modes.  

For reference, our expected dispersion is below

![Labelled Preliminary Dispersion Plot.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/cf68371e-41ab-f4cc-f241-5a357712b5c9/fVguErbyLf7y79NiQofWRxdKjysV1gjAlNCxaPgbmxAz/Labelled%20Preliminary%20Dispersion%20Plot.jpeg)

It is definately possible that we are coupling into really fat waveguides.  Our waveguides go from 4 to 7 um wide.  It is possible that we are just coulping into an annoyingly fat waveguide or something else is amiss.  I say we try to couple into a new bent waveguide if these continue to not work

Looking at Ryo’s earlier results, it is important to look closely at them

![Image.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/061B9960-B73B-4A2A-BA58-C18D4E2FBAE0_2/fquYNwVoXOxHXerQ94pYwhAgEqw0Xw87iztbdQjuQDsz/Image.tiff)

![Image.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/577D621E-2BED-409A-AEA3-73066DD6B1EE_2/fYVz4Ov08n8f2RD9oFIO0oT1yOV23bFjptzecDdP0vQz/Image.tiff)

Notice, that his large poling scan went from 12.3 to 12.7 for pulsed light.   My current scan goes from 14.5 to 14.75.  The second measurement is more consistent with Ryo’s CW experiment.  Now, I have done very large scans, but the idea is still there.  I still say we go to the narrower waveguide just to get closer to what we know already works.  It might also give me some needed practice aligning the system.  Because it is easy, I am going to setup a Santec programmable sweep for a poling period of 14.62

No Dice on longer poling scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/131430AE-E725-4D9B-B8AF-FDA3FBA0D70F_2/f81KqPqB6Ip1oYxwP2jviuGPvR3Td3xBOCmp7vedMRkz/Image.png)

While it is course, the wavelength sweep did not do me much good either.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/A6E06308-E8D1-4E2F-8D7B-E156CA409090_2/hGijm6xhxE781czXe2mRkzZ6Ui8dIMrE9K6nT4Id9x0z/Image.png)

So we have a few options.  Firstly, we can try to up the applied voltage a bit and refine alignment.  While I don’t love the hypothesis, it might just be possible that we are not efficently getting power out of the waveguide.  For this, we would have to still use CW light.  I would still assume that poling of 14.62 is roughly right.  I would also use 1580.  This distinction comes from the fact that pulsed light has much higher peak power.  

So as it turns out, the above measurements suck.  Someone turned the PMT off, so I was not collecting anything anyway

Still no more luck here.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/74442CB7-CD77-44BA-980A-13F11C8E014C_2/nNrKQxzbBDfBgX1515mcrXB6YhctpkGAsizc73uZnEYz/Image.png)

Lets really try to get the alignment to be optimal, and then if we get nothing, we can then try to do a different waveguide

An extra scan where I confirmed everything was working

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/FB0D4FFF-504C-4D1B-878C-8B843FD3B21D_2/m9uDNgerKbcUhxMFzEJJgZs0zIrfUnLaci2xAfHEpjgz/Image.png)

At this point, we focus on alignment

Starting power before any alignment (no back objective focusing)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/A79670A7-371C-4450-940F-2CB43E75EBD0_2/UqdrvpP7rYnTNKpZbOLO0soCdpdadMCBw7I00G3E74wz/Photo%20from%20Library.jpeg)

Input power

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/5844CC30-0BBE-43C1-AAF0-D0171B98429A/594173DC-27F1-4A4C-8780-F2826EEB33CC_2/o3ctfXEyIeowo40i84h2LPtpPzaFhtXoxds7UbFXh1Iz/Photo%20from%20Library.jpeg)

After visual inspection, I know I am coupling into the 5.5 um waveguide.  I also know the top of the pylon camera view is the beginning of the waveguide, and the part I have been poling thus far.  