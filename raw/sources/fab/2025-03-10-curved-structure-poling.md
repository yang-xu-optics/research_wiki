---
type: craft-export
title: "2025-03-10 curved structure poling"
craft_document_id: A8182761-9AE4-403E-AAD6-C53E2456D67B
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-03-10 curved structure poling
I currently have the snake etched RTA waveguides nicely aligned and producing quite a bit of SHG (the only thing I need to scan is the AC frequency to check that 5 Hz is right).  I have the EMLO pulsed laser installed right now because it will give me more signal.  My concern now is trying to pole the bent region, as the imaging setup is nicely aligned over it.  Below is a rough sketch of the poling I have for a curved structure (using sine, though I also have a sign function version)

![Screenshot 2025-03-10 at 6.50.05 PM.png](../../assets/fab/2025-03-10-curved-structure-poling-001.jpg)

The only downside is I don’t have a tilt of some variet in case that should be needed (basically, if our x and y axis are not aligned with the real x and y axis).  I generally feel like this is more solved by picking a differnet starting and ending angle, but that is just me.

![Image.png](../../assets/fab/2025-03-10-curved-structure-poling-002.jpg)

![Image.png](../../assets/fab/2025-03-10-curved-structure-poling-003.jpg)

First scan predicutably does not work.  Something that makes this a bit hard is we might not even share the same origon for both structures.  This could mean the poling period on the waveguide is effectively getting chirped.

![Image.png](../../assets/fab/2025-03-10-curved-structure-poling-004.jpg)

![Image.png](../../assets/fab/2025-03-10-curved-structure-poling-005.jpg)

Still no dice.  I can’t tell if we have the radii quite right

![Image.png](../../assets/fab/2025-03-10-curved-structure-poling-006.jpg)

Reducing the width shows that we are pretty well aligned, so I am not sure what the problem is.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/35E775A1-B282-4067-91C7-7DAE3B45C490_2/aM4rq6Xzmijy2vRLdCH4tvfKo1xaOXxraGPqtKUGv88z/Image.png)

Poling a similarly small straihgt region is above.  We sorta get a curve, but it is hard to say.  

We now do a straight section with a comparable length using sign

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/3D8563FE-5CC3-44AD-887F-432FED3465F8_2/YYuFG4TGi4hZJrSf0KXhJkwl4Rvq6TOqCkozeWCO3KIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/C5376FAC-9167-489D-90B8-8F199944B7DB_2/1yymFumA3pdHMxgONiYv4f1EodSXV1ib5P0kGBJwWsoz/Image.png)

So now the signal is easy.  Either way, we really do expect something from the curved sectino, which we don’t see

Below is the same scan but using a sine (instead of sign) function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/CCF4D278-7AF0-499D-AEC2-FCBEBF804FA5_2/xVfiAoGEIdQgPax7VTqFo39CVCDgy2lNhEorbMe5pzoz/Image.png)

So we might just need to use the sign function.  FWIW, because the waveguide is bent, it could just be the case that the effective indexes are a bit lower.  I suppose we should bias our poling periods to be a bit longer.  If these continue to not work, I say we do a poling period scan on the two straight waveguides near the bend.

Below is with sign

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/C5A73042-AFC3-416D-9720-46526C1157A3_2/wGiZiRoaSocz0Hv4daF1yzrx0T9gizZ2REI9OsKQ1ecz/Image.png)

That did not seem to work, which is a shame.  Though I will say that the signal is just annoyingly weak.  Anyway, I think the next best course of action is to slightly pole the beginning and exit straight sections into the bend.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/D88B9256-BE3A-4B4E-89FC-B20BA6A2BCDE_2/Se1d0rp8T6wYUR6PtrBSIqJzujB6CoIHVQZ4Dfw4J3kz/Image.png)

The transmision lokos nice, so I think the period is consistent

Now lets do a quick poling scan of these two straight sections to figure out where their best poling periods are.  We will then probably remove some of the NA filters so we can take a look at the poling of the bend better.  As Ryo said, we just need a starting signal, and then we can align

Upper straight waveguide (in the middle of the 3 branch bend)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E938BAEA-ED05-4097-B77C-D02D15619976_2/DtyiurODxZDrBxeocncLTdTbAYy22vL23UBhXg2YD6cz/Image.png)

Not very strong, but the waveguide is only a mm long.  Lets make it longer.  Below is for a waveguide that is 1.5 mm long.  We expect the bottom branch to have a different poling period based on previous phi scans

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/2A25CD7E-AABC-41D1-83BB-248D5F57F7C7_2/Tsn9pXBylXw5sw7UlpAshVmQZGxBnvUpWip2OVsaLLYz/Image.png)

An otherwise very similar shape, just a stronger signal.  Below is for the bottom waveguide (still using a straight poling length of ~1.5 mm)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E33E90CE-20A3-4E3E-9E72-0817A8B2922F_2/mFwGhRllq6JOTbOJvehVGyrRgUocdXcO80iRAVekyhoz/Image.png)

Nothing, which is a bit strange.  I am going to make the waveguide longer (3.5 mm) and increase the poling range.  Also, wave propagtes in from top left of the image on the pylon camera

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/CB796E82-8D71-47A7-A96F-84C64EB0D3E2_2/gEXziWPdiOYvUuxeqDDnXvwPHNw2xESxrG2pEPCKEtkz/Image.png)

zooming back in

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/6FDE4AB2-92CC-4808-8741-C61290311AF2_2/66gcrRvXzxTSXsLNhJuSTf7PX2h1Z7DWe4JTVOwPKvAz/Image.png)

Something is happening, but it is hard to say what.  Lets make the poling distance longer (now 5 mm).  I want to make sure I have enough signal that I can then align the setup to it.  I think the image tilt it just a bit off.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/3C7B33C5-30B6-43BE-9296-BECBA38780E8_2/zsSsIxbUdGFNop66NPWlW0o0VNYqQTCQV8LgYpYOOF8z/Image.png)

Still not great, but I will try an alignment anyway

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/01A542CD-059D-4421-ACE4-4053ECAE949F_2/iWLEaSx4fYydUHXNEObCMMqdZpyP75bDvxfNO0fIfHUz/Image.png)

With a bit of relaignment (ignore first point).  Lets recheck the middle waveguide.  Objectively speaking, the waveguide is a bit long (at 5mm), but we get a rough sense of things this way.  It is also nice how broad the peak is, so hopefully there will be something to align to when the time comes.  We may also need to remove NA filter, but we will cross that bridge when we get there.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/A747F189-2169-4B9B-9017-49E135213D31_2/stSraSdQBuPSHEf62r8ey7nyzJkofipgJHaxG1wwqFoz/Image.png)

Interesting that this waveguide is more nonlinear.  In the future, this is definitely something we want to note.  This probably helps with the idea that a smaller device footprint is better as you get less imaging aberration.

Now lets try the bent section scan again

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/ACBA68A6-028A-4168-80E7-0C2CD0D3A427_2/zz5EVQcgmdjBr1ZfumXevzdu4QBO1v56SCSwxVuDYikz/Image.png)

Seems to be roughly centered, and again, hopefully the peak is somewhat broad (though this boads a bit worse for CW, as that alignment will need to be really good).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/2C534FF7-F60D-4628-9914-DC9D066D00CC_2/vE1tx3xQGxrntyfcVkS6R2uU7Ppqvsv8Exc4qc9qhxEz/Image.png)

Above is during scan.  Again, it would not surprise me if I need a bit more alignement here

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/0D64121E-11A1-4667-9D2A-97DB70B31448_2/uMQEUWBdDlS5ryVsUEQPPKJLcfNMynmcyzGkgypP2zgz/Image.png)

If this is to be trusted, we want shorter.  Lets try again there

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/D898C0B6-3ACB-4887-BD5B-B53606DC135E_2/cOyo7qK1fnrEWpiBZY0FtCWiJ6jgFBOrnDGX9xLxNSkz/Image.png)

It works!!  But the amplitude is not insanely high.  I think the next thing to do is slighlty very some of the x and y offset terms such that we can get a more uniform poling.  Once we have optimized those parameters, we can go into lab and focus the entire setup.  Above was for y_offset_percent = 0.06 and x_center_percent = 0.2235

Below is y_offset_percent = 0.06 and x_center_percent = 0.2238.  The challenge with doing a scan of one geometry parameter is that the poling period is a function of geomerty, so we could just force ourselves into some weird local minimum

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/0AF521FC-5C69-4EEF-A10B-EA79DC41F859_2/hLHFzi50andzrU7ZVovSSiaSP5mjkgIlZVO8ieohrusz/Image.png)

Tough to say if this is better.  The peak is mostly narrower but not higher.  Lets take X in the other direction (now 0.223

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/263E9040-D07B-4FAA-B0DA-87A63CE20D76_2/orJ6iCcIHHYB2y0vOGOu3YMg3Tzb7YOTQ2NmGTayDxcz/Image.png)

Really is quite hard to say that I am seeing much difference.  Lets return the x value to 0.2235 and scan y

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/6E99460D-D86B-4747-9EE5-C2E685E57E24_2/yl2zg9xkJl7gbgYQhyD2edqg8KtwHxxvCfJoBoRSZEYz/Image.png)

above is 0.07.  This is comically bad.  Good to know you can go too far.  Lets try something more reasonable.  Below is 0.062

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/D14D03A1-DD51-48C4-B745-9551DCBF7B61_2/mAJmvsP5sgXyGUGzpFWqDDjw0bjiy1mxzL0jnjvSiygz/Image.png)

Worse, but we are moving.  Below is 0.0595

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/6C7335DE-52A4-4E21-807D-F7458C6F52FA_2/c2xDxXiheI56XmXLenGPXNn4v9Z4yXjxE4MIsYwqMqsz/Image.png)

These are all worse.  I say we go back to baselien and just try to optimize focus more

Refocusing worked fairly well.  It is nice that you get such smooth control in x and y.  I focused optimally with the straight sections.  We do see decent signal from the bent section if you zoom in on oscilliscope, so it might be even better just to leave the straight sections out (in case there is some advantage in one direction).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/5584D8F3-5A3B-4FE2-BF56-634929917F5C_2/BOXx17SSBxpiJo4IjRcFCrWXAvc6gJVPs1YbSK6YQ6Uz/Image.png)

Above is after realignment.  This is not a tonne more signal, but it is still a very well defined peak.  Lets do one of the straight waveguides (the bottom one) of the same poling length just to compare.  We can also do one huge poling scan to finish off the day just in case something is a bit wrong.

Bottom

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/111D4BC1-A74E-4F5A-947C-1BFC33ED2BA7_2/9dpSyebpvk8MYaJl6bIxNrd5UxADj1yTtPPcWAo7es0z/Image.png)

Middle

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/B7474614-A4B0-4D3F-80AB-B6F06AD38ECE_2/y9rAjOSQZI2wWZg9TBYkeJMVHNOAqptHqii5FC3q1c8z/Image.png)

good to see that they look similar.  We still get a lot more power out of the straight regions, which is tough to explain.  Let do a broader poling scan, and then change to the CW EDFA.  While I would noramlly blame focus for our issues, if we see such similar results for the two wavweguides that are vertically seperated, I would imagine we are fairly close to ideal here.  May we could adjust the hoizontal focus, but again, the waveguides would all notice that.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/5DCCA2FB-7B38-4EF2-8F7F-39B8C072C075_2/MGC0dVr1sVgKZKteCYIM1Hbx8D4vRGyuBskdT9pMxQEz/Image.png)

This scan makes me a believer.  It seems like there might be something at even loer areas or even higher areas.  I will scan from 10->13 and 17→ 20 for good measure

10 → 13

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/B5F03143-8041-4FCD-86A6-6EFCB30DC698_2/Z7RJAUn9KATkhASM3IBluUbuKISxxsShPb4SQRASesoz/Image.png)

mostly seems like small peak around 13 um

17 → 21

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/4D504CE5-9C0A-4694-9F09-5FE26412264C_2/nIsPeoiyeoFhUbQipiWFldkLv9y2wjLNrOx5LqP3JxIz/Image.png)

So we do see another real peak.  Lets do scan from 13 → 19 where we can see both peaks.  From Ryo, it sounds like the next best idea is to do some chirping of the poling period, as the peaks are rather wide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/6406236E-D2F5-49A5-9539-02EC17231585_2/4xSkTkdhbEHmxqdrmLCqQS8ktC3AuMXsF50VeckUM3Mz/Image.png)

This is quite interesting.  I am going to do a broad seach (say from 11 um to 21 um) of the straight poling period to see how many peaks we have.  I would like to know if the bend causes the period to go up or down.  It is interesting how wide these are, and rather not sharp or smooth at the top.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/98EDDE8E-A8C4-4E4A-BCD7-792BFDCEEDBD_2/UrpXOqxuiOpxz941H0xqxIHNUEoeTTZmVJk1FhoLPpkz/Image.png)

So it seems that the poling period goes down slightly

In the mean time, we should think about what we should do for the chirped poling period.  My general take is we should write some function should we can input into the circular sine pattern generator that is able to define the period for a specific angle.  We can have a linear and quadratic term.  It might also be a good idea to calculate the integral of the curves above, as this area should be conserved.  It is a nice sanity check

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/DBCC311A-FF3D-4FCF-9E51-35DE629242AE_2/exMg1q6RZDgTMOt24EOvqQXgymgBisUFORDvRP9UxUYz/Image.png)

This is what we saw for linear chirp.  So there does seem to be a peak, but it is kinda isolated, so it could just be some noise bs.  There does seem to be some dependance on the linear chirp and poling period.  Small, but I feel like you could plot a linear line and see something.  We are now running a very large scan where the constant, linear, and quadratic chirp are all adjusted.  It is 23 by 24 by 25 respectiviely.  At this point, lets see what happens

![Screenshot 2025-03-12 at 6.22.39 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/3734916F-90E0-4CD8-8D3A-E6AECF3CE6C5_2/TLSkyMDgwVvC8V63X3Krt974d4hajDD678qYpHxlg8wz/Screenshot%202025-03-12%20at%206.22.39PM.png)

The plot above is for varying the constant, linear, and quadratic chirp.  There is a peak, but hoenstly, I am so sure how much I believe in it.  The max value is around 0.02, and we got it with the following parameters:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/048708EB-DFD5-4F6B-8DA2-7B48C4FF90C4_2/WQ03zKsgn3EgseysxMDMdA9J6NFpuCyG4LXQdrXNU0oz/Image.png)

Ok, now lets try Ryo’s idea of poling subsections of the waveguide.  The hope is that each section of the waveguide might have a better poling period so we can sort out this two peak business.  The advantage of pulsed light is the phase does not matter

Below is pi/2 → pi

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/74408FBD-3235-499B-BC58-CECCC2481491_2/GDZRNwesIMcqRJ58nkx85JztzeMLAxyhD5hSbhq0QEAz/Image.png)

![Screenshot 2025-03-12 at 8.08.05 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E1C9AD41-1BEC-4551-8967-D85D39B0BC4D_2/6xcVYZRxOZAaODJaqR3oOHcXp2eOPpZvufFx2aqNgt8z/Screenshot%202025-03-12%20at%208.08.05PM.png)

Interesting that we have a rather broad conversion region, but we really only get a lot of conversoin at 14.75 (which is what we expect).  The other peak goes away

pi→ 3pi/2

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/9BC8375D-7EF0-485F-839A-CEE4E84D775C_2/Xxx7daeC9bXIy0gcqZQdcxdkXC7FEuHClXZxp8eyCXwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/47A0C7A7-E1BE-41D4-9558-8D847C77CEC8_2/yPnAZMKfJ970MTNqqgfoU3L7aCBMJDFx7RPb241ybXYz/Image.png)

Ok, so this is where the longer period comes.  Lets try narrowing search

pi → 5pi/4

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/C6C3678E-75E1-4D01-8BC5-02DDD62CC384_2/XDlY2aHfhenBGPf3ytXXkn2LCw5i2C6c0ocXp3GDRLEz/Image.png)

![Screenshot 2025-03-12 at 8.59.06 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/177BE413-6E66-4E50-B31B-275702494DC0_2/OFI5WFqJBFSz5w0WquXvsR9nRHWyHlaxwvssdwg36AMz/Screenshot%202025-03-12%20at%208.59.06PM.png)

5pi/4 → 3pi/2

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/4260993E-488F-4DF5-A3D2-D09C755CF08E_2/U5YB3xbO9EV9sSuy6wjBBR6hITtoGgVVUzRbwHDA2swz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E4F73706-BCCE-4C07-9ADE-49798E5C2EBA_2/pS8VfJHwSC7DC3SvUFuZjrHbJDTVHX4PAvbyBxmCxg0z/Image.png)

pi/2->3pi/4

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/4BD4B66B-4620-4361-A9E5-5A56A0D3FFD3_2/tLR0cyjYRrKviyHPbNg6aXsdOONCmsImv6hI20MMyiUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/88A171BA-83E0-4C28-906A-39A1341DF518_2/BI8qX7x3oWaoKovc3ZeWtzK8ILspWggdzxiFURfy9ygz/Image.png)

3pi/4 → pi

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/0664659B-199F-4F34-BC37-332FB9ABA9DA_2/yna71DaHHBOXSU0x3LbbHgxbPSIVsv31FrsMfGhpbikz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/91B5B8FD-9B9E-4D5A-A02A-661FB15BD290_2/6zRNpKLMGq1jv624fFrqkoF7VFWY1iOBVMToZfBBxxMz/Image.png)

As summary, below is the plot from pi/2 → pi

![Screenshot 2025-03-12 at 8.08.05 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E1C9AD41-1BEC-4551-8967-D85D39B0BC4D_2/6xcVYZRxOZAaODJaqR3oOHcXp2eOPpZvufFx2aqNgt8z/Screenshot%202025-03-12%20at%208.08.05PM.png)

Below are the subplots

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/91B5B8FD-9B9E-4D5A-A02A-661FB15BD290_2/6zRNpKLMGq1jv624fFrqkoF7VFWY1iOBVMToZfBBxxMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/88A171BA-83E0-4C28-906A-39A1341DF518_2/BI8qX7x3oWaoKovc3ZeWtzK8ILspWggdzxiFURfy9ygz/Image.png)

We would expect the sum of these subplots to be the same as the total.  It it possible to see, but the issue is neither plot gives us one peak, which makes this tough

Below is same think for pi → 3pi/2

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/47A0C7A7-E1BE-41D4-9558-8D847C77CEC8_2/yPnAZMKfJ970MTNqqgfoU3L7aCBMJDFx7RPb241ybXYz/Image.png)

Subplots

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E4F73706-BCCE-4C07-9ADE-49798E5C2EBA_2/pS8VfJHwSC7DC3SvUFuZjrHbJDTVHX4PAvbyBxmCxg0z/Image.png)

![Screenshot 2025-03-12 at 8.59.06 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/177BE413-6E66-4E50-B31B-275702494DC0_2/OFI5WFqJBFSz5w0WquXvsR9nRHWyHlaxwvssdwg36AMz/Screenshot%202025-03-12%20at%208.59.06PM.png)

Again, it is possible to see where things are coming from, but I feel like all these subplot scans basically return the same period at 14.76 (maybe with one exception).  It would almost be nicer to do a homodyne detection scheme, only that requires CW light and is phase sensitive.  It is not clear that the sum of these plots is exactly the same.   I feel like a perturbative approuch might be the best, but I am happy to move to CW light soon.  Maybe doing a mode simulation here is best

We are now running CW scan of top waveguide as baseline

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/D7E28089-7CC8-4DC3-9033-FE11269DE671_2/7IbQV4qcm4NCj1ysyY8Bo1yv3GVwkxpJPoJUftMktYAz/Image.png)

A nice and large peak.  Now lets do the bent waveguide.  It is around the same poling period as before 15.77.

I moved the bend slighlty in space to try to center it better.  I will now do a large scan of the bent waveguide over the two poling periods we saw before.  If this does not work, we will need to do some homodyne detection with the large top waveguide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/492CE15E-4E7A-4E8F-A8F2-C805DCA86EC7_2/e1PhTI2gmU6FqBhZqy2Rlmodp7Zlys8I24MTErwlX8oz/Image.png)

This plot is suggestive, but I can’t say I am seeing anything yet.  I will need to do homodyne detection for this, but poling the top waveguide and than varying phase and pp of the curved structure..  We are getting a suggestive peak somewhere between 14 and 15, as well as a suggestive peak between 17 and 18.  Lets do a homodyne detection scheme in those areas were we turn the poling on at the top and while scanning the phase.  I would be curious to see if the ideal phase is a functino of the poling period.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/37FFB695-DE63-447C-98AD-CDB7B781FBFB_2/SIFeqy50OrtTWrizgdb5g06z2WkjXQ5X4j9x3JPsqdMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/278A495D-76D0-4B4A-9231-4A5459535441_2/GSYNyIYr34T4IBVyYvvDKB6UuQ8UzWBIKmyxfyDuHroz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/CCC62034-0CD2-4F96-9203-72F047489943_2/hBEVZw8AIm6bDWNKm1HjMMRfb1p5y4LyAj9vKCoQgVEz/Image.png)

I think the main concern here is the scanning region was way too large

14→15

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/1F787558-3EFE-48AA-8465-4C3BAA6AD599_2/OMhF8MvlD6xyqE2ngav4HoVYwDE1uyLE32dP818i6Ekz/Image.png)

It seems that 14.6 might be it fols.  Lets zoom in.  We are really looking for these sin-like curve.  We should probably add in the middle branch too.  The lower branch might be hard just because the phase offset might be screwed up with the different poling in the bend.  This will give us extra power to homodyne onto.  For now, I will do the zoom-in scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/F53C97CE-3FBB-40D3-9134-976447ED2DA5_2/2GGSIDvMAdRVUXXv55tpxxeZnofXdR8cHWYimdLDMqIz/Image.png)

It seems like some peak exists.  Lets try the other domain from above

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/52B867B3-6703-4A5B-B1FD-1FCF5B29B943_2/0cilcmEygjTxCt5qGRPFEfiutC8ZW4NceWmLelAOPxIz/Image.png)

So I do think the optimal region is around 14.6ish

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/75CDAB3B-A7D4-4231-8CA6-EA54FA50DE59_2/YxP06xaSDLMhroA993sCwREZyzUj01yjyJq097mjxxsz/Image.png)

There seems to be two ideal poling periods.  Good to see that things are a bit reproducible.  The werid part is the poling period around 14.4 was not as bright last time.  Last do a quick scan on the middle waveguide.  We will probably want to do some type of homodyne detection with both the top and middle waveguide poled

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/08C082B8-22C2-4B8B-88F7-27C554C9B403_2/Mtt1pz6lSRBlBCS5h0dSuzPDNRnVW52ogvZ69edJOFEz/Image.png)

Now for phase scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/B01C162D-2F19-4978-9104-DD4EBD17DEFC_2/i24YdNajn7yqTdbvYWNIli22oxqgyhcUQBvIPiuw26oz/Image.png)

Interesting that we really need the full 2pi.  Worth noting for the waveguide scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/76F25E0D-83B8-4DE9-A039-FDD62D0D5290_2/MWGDnWHF6hzFJ7ofZ6Hw2unkFYwbebQwOm6geQMEh98z/Image.png)

Results

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/D36B78AE-873D-48CE-92CE-81F2651CB788_2/Na8aflEtbyhfbIRwweE80y8UV2ywLqZnXSyeViYygIgz/Image.png)

If the result is true, it seems like the ideal phase drifts a bit depending on the poling period

1d cross sections

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/3584139F-2AAC-4358-96F5-5209F14ABC2A_2/sTabYAxHpp3kY8sqv3FLLvN92Ze2PUk856PuFICB9eEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/845056B1-A07D-4307-B889-F637C02347FB_2/vnO4p2pOLWXaS9aT6ifaNLqWJIe6Fi47wrMFc4LP3BMz/Image.png)

It is just weird so see such asymettry around the peak, but this is very similar to before.  Lets zoom it and scan further.  We can sorta see stuff going on, but I want a bit more confirmation

Another one

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/38F3B474-104A-4BE0-A8E3-2B7C0CE95A6E_2/i7sryYkenhyZmZlxZLjWpKgXk7H4XAApm3yDQNu7IIEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/99F3EFF3-B6FD-45B5-99F1-E0B0EC3F1AAE_2/lxnx50cqLbUx5SUbXb9yEMITB3FHtXm6hBlFzuQQpxQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/8216048C-D604-46AE-8EC2-128013775732_2/mCb6fVOWAWbyaJB7hndsTnpufmyZAHQhSulbOuYZlVkz/Image.png)

I feel like its a moving target.  I am going to zoom around 14.5 +/- 0.05 and take some more points

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/7AB64CDE-D2EF-4199-A909-1A60673077B9_2/AzQdcWRptXr2146KPaKSXTjkwgy43l0jxZvzmBtWtkUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/B96F5E5C-147D-4566-AAD1-AC661FE06054_2/J7aWsqLXczjS26zmXVT1QlRgh62sCZ0XGv2YbxGNZ2gz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/EEC4D86E-F102-4A36-8BF2-660B3AFFC71D_2/8CLKqAF6mZtairACy8NyajVZ2yNNYqq5X7KeSwpXHnwz/Image.png)

Lets continue to do scans here.  I am still not convinced as to what we are seeing

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/F80F4FD1-DF2F-4FCC-8888-535C104B0BD4_2/SP1EuxtFKx5wh0tCkOhCen1yoSy2bIyaxQEPLvy3PM8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/E5C4F602-7DDC-4F39-B902-0DEBC5C1EF2E_2/WtOxxjouIZ0CbvQUKJPvuLY148HyQnmqHdCDLIWY2J4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/CDF27BD4-C5EE-4912-BF09-B27F64F76197_2/MN4V4K9V2GXx3eb31BPTuHN5go1tDdnDAQ0xucQOxAYz/Image.png)

I feel like each time we do this we just get a tonne of drift.  I will go into the lab later and make sure the oscilliscope resolution is good enough.  Below is zoomed in oscilliscope, though wider data

![Screenshot 2025-03-16 at 10.03.23 AM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/B9F08F2B-AC41-48D5-8CEB-3EA3BA6F2CC7_2/0jr02p3nNWMTIfwymkvgWszFbf6w6PtyjpDrn5TxNnQz/Screenshot%202025-03-16%20at%2010.03.23AM.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/57D3119F-2DD8-4B36-9382-16AB4E4119CF_2/ODg1ZfEjMk04chCzGJ6iT64yTeiakIO7Nsi9zEhgRCIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/06C3D20F-0DDC-40AF-9665-C898CD978E33_2/cyDG4q1y9evK3mXjjjoReTtRY1kS8bmQukuAQ0a9ojkz/Image.png)

Ok, so I think we have taken enough scans of this region.  Lets do around 18 just to see if anyhting is up there (as something was there for pulsed light)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/7B7967FE-12CF-4336-A2AF-8FA5CB1BB7CC_2/LMd796aR7jFTtRjRyR6nlLFXvDhcWGe9GiNTygfyW7Ez/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/14B95EA8-61DA-410D-89B5-B754E8EB0BF9_2/z5TNLgyBdRpz4r07EavQaP6QisB2rML48Q4b8jzyy00z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A8182761-9AE4-403E-AAD6-C53E2456D67B/CFF4E281-F2F7-4CB3-A960-6E3B012D7AB9_2/ebdUF7mJjiMCcylTbXKWxBgIXZNL89ZQQB4ceVdlzokz/Image.png)