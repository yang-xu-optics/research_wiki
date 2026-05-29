---
type: craft-export
title: "2025-2-9 quadratic scaling of shg for etched bent waveguides"
craft_document_id: 6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-2-9 quadratic scaling of shg for etched bent waveguides
Now comes the fun part.  We are going to try to show quadratic scaling as we increasing the poling amplitude.  To do this, we are going to have to optimize the phase and poling period for each additional poling amplitude increase.  This may be hard, as short poling amplitude may not give us much signal.  

We are trying two methods at doing this, the quick and the thorough.  For the quick method, we are doing to do a three branch phase scan and find the optmial phases for the two lower waveguide.  We are then doing to increase the poling distance using the correct phases.  It should also be noted that we will increase the poling distance along the path of light flow, so each waveguide’s poling amplitude increase will occur in opposite directions as we go down the waveguide.

The longer option is to subdivide each waveguide into 3-4 pieces.  We then scan the poling period and phase of each waveguide as we add each successive bit.  Once we find the optimal poling period and phase, we move onto the next part.  This is definately a full parameter sweep, but I am worried that some of the early signals will be so weak that the first few points will kinda be BS.  It will also take a lot longer, as I am introducing poling period as a fully new degree of freedom.

Below is the first scan for the quick method, showing both the optimized phase and the output signal for increased poling amplitude.

pp = 14.825

![Image.png](../../assets/fab/2025-2-9-quadratic-scaling-of-shg-for-etched-bent-waveguides-001.jpg)

![Image.png](../../assets/fab/2025-2-9-quadratic-scaling-of-shg-for-etched-bent-waveguides-002.jpg)

The factor of 3 less signal is merely a coding mistake.  I can see some quadratic curve from the second two waveguides, but nothing from the first.  It is also a bit werid that I seem to see some destructive interference at the end, which I would not expect.  Lets try the other poling period

pp = 14.015

![Image.png](../../assets/fab/2025-2-9-quadratic-scaling-of-shg-for-etched-bent-waveguides-003.jpg)

![Image.png](../../assets/fab/2025-2-9-quadratic-scaling-of-shg-for-etched-bent-waveguides-004.jpg)

This is a bit more like it.  I am going to do a more thorough scan of the poling amplitude and do a curve fitting to see what our current exponent is.  For the curve below, n_itr = 5 and n_samples = 7, so it is pretty accurate

![Image.png](../../assets/fab/2025-2-9-quadratic-scaling-of-shg-for-etched-bent-waveguides-005.jpg)

![Image.png](../../assets/fab/2025-2-9-quadratic-scaling-of-shg-for-etched-bent-waveguides-006.jpg)

For reference, below is the form of our polynomial function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/A7F9E694-81B3-464D-972C-A9F2C52FABE8_2/FJykmPdcdFAKr4jBspyGeqcxwNYi45TxqyCxI4rXssgz/Image.png)

I am going to do one last really long scan and then move to the longer version

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/65F19272-F85A-4ED8-92C3-BADCE19C748E_2/NnSACpXR2Gk1Lv2RfhBw9IeGI7tPDvv9PDMwMk14OJQz/Image.png)

Another annyoing dip.  I almost suspect that wehn I go off the computer (or it sleeps), that causes the issue

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/3F638083-AE11-44C1-BDA9-7A92B2E53498_2/YU13LsiCW9n6AeGKFWmgxyE29rCBCzGhXf2EFy00fYAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/3702A9A0-EAF7-4487-8F4E-F4AFE04EDAAC_2/09sbrEkhv1PZc4lbTehaeF1MGpVyh4TCP86UAIQkJu8z/Image.png)

I am going to do a quick extra few phase optimization scans followed by a more detailed poling scan.  I think I will generally find that this will get me an exponent of 1.6-1.7.  This looks fairly similar to what I had earlier as well.  Below is a zoom-in scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/7C243BB1-D5EA-4A20-AFE6-2F14F2200AF4_2/9a2L2ijGzIhK53iSJLgtV6UryTKO45kBGObxyAiwjeAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/A6078664-4E59-4CFB-9287-52258C0D06A9_2/y3tsgmlh41AxDZLLvfJsB8oWR90qVhzDAJpAGWfJDPEz/Image.png)

Below is what we got before

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/A346B55E-96F2-49AE-AA18-BE1EA5177FDE_2/tsWgkilWACqvylcTfRaWGVNkTGdYN0D8kfrLAz4kXiUz/Image.png)

At some level, this makes a bit more sense, so we are going to do another larger scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/03FAF92B-CDAB-48BD-92D3-8680E260ABD0_2/5k3l9uXc72tvJClBGRxxQxlhYre44F6igp93I8KyY3wz/Image.png)

The exponent is 1.6

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/C9900017-2BC7-40A5-9132-0DF39A93DD18_2/eRoR5chLsIw0uIpCzPRnypuaDpdUuFCdyr8URYI7xRkz/Image.png)

Trying again, (as the previous one had weak signal).  Now 1.44.  The main issue is the end seems ot saturate a bit, and there seem to be some regions with a lot less efficency.  So that is an issue.  Anyway, I feel like the poling period scan will help.  Below is the result after doing the very long scan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/6A6CEDE5-A7F3-42F3-B05A-E4A2DB512997_2/eIX5IJUGsxAQsiMy1HM7Zkf6SyO3gndnExicxZ2jJewz/Image.png)

It is just surprising to me that these poling period scans don’t converge as much.  The phase scans give very strong data, but poling period not so much.  It is weird that you can almost see destructuve interference.  Ryo had a good idea that we should try to quadratically and linearly chirp the poling periods for each waveguide to optimize, so that is what I am going to do.

I got more power from the laser using a fiber amplifier, with new average power using power meter as

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6D7AAA17-7B86-4E8A-AEFE-3369EAECD6BE/9D2456E6-AB86-4782-9685-252751E29774_2/W8fLpReJxuuW8h4nbL4EoaXJXNdUPvw1xJQQaTEUx0wz/Photo%20from%20Library.jpeg)

Almost a factor of 3 better. I eventually got it up to 3.1.  There is probably still more room for improvement, but I feel as though I am in the sensitive regime where too much fiddling can destroy things

I also increased applied voltage to 12.5 and LED current to 4.325