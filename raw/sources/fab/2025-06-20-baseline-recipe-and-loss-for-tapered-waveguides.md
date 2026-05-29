---
type: craft-export
title: "2025-06-20 baseline recipe and loss for tapered waveguides"
craft_document_id: 7CA1AE59-4B37-4AA8-A260-87A62519919D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-20 baseline recipe and loss for tapered waveguides
We have so far struggled to make low-loss waveguides for our tapered structures.   This is turning into a real pain.  We have so far only tried oxide hard mask recipes, and I am getting the suspiscion that something is off there.  The only difference between our previously owrking hard mask recipea dn the one we are doing now is the thickness of the resist mask.  While this might not sound like much, my hunch is that the CH2F2 etch reacts weirdly with ARC.  I don’t have a better explaination than that, as it is just a hunch.  It is sorta like how CH2F2 reacts weirdly with Cr.

Anyway, we are going to do two things to settle this loss issue once and for all:

1. Make an SVM wafer with 800 nm of resist on oxide hard mask.  Literally copy the extra recipe from before
2. Make an SVM wafer with 600 nm of resist on Cr hard mask (just copy the Cr recipe).  

At the very minimum, 2 is a process we have ues so often that I really feel like it will work.  If neither works, we know the issue is just the etcher.  We are going to use the tapered waveguide pattern.  We can us the power out of the straight waveguides as our baseline to compare the performance.  We expect roughly 5 mW out of the straight waveguides using the main setup, EDFA, and 10X at 1570.

As a future thing, I would also like to calculate the viability of using CHF3/O2 to etch the oxide instead of CH2F2/He.  I can’t explain why, but I feel like the latter recipe is a bit cursed.

We have found that 750 nm of oxide allows us to etch through 2000 nm of SiNx.  This means the selectivity is 2.66:1 for CHF3/O2/N2 for nitride to oxide.  This is good.  Another important note is we will probably do this etch for a minute shorter in the future, as we want to strip the top oxide anyway.  We ideally want 100 nm of SiNx left to protect the bottom oxide from BOE stripping.  We did a 6 minute etch, so we know oxide etched at roughly 125 nm/min (again, a bit of an estimate).  This means nitride etched at 325 nm/min, which is consistent with earlier findings for nitride.  We then know we etch oxide at 180 nm/min with CHF3/O2 and resist at 120 nm/min.  So we still want around 1000 nm of oxide, so we need 660 nm of resist.  This means we must use the thick resist recipe and not descum for too long.  It might be possible.  We would then leave the wafer in BOE for 5-10 mins to strip off any remaining hard mask.

In previous studies ([https://tdwg.craft.me/9TKpCasWHuS8oN](https://tdwg.craft.me/9TKpCasWHuS8oN)), we definitely hit the ARC using the CHF3/O2 etch, so this is not unprecedented there.  It seems, using our preovously working hard mask thicker resist, after 1:20 of descum, we get 700 nm of resist, which should give us 1000 nm of oxide.  At this point, we just hope to get lucky on selectivities.  It is defintiely a bit tight.

### Photolithography

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/43861E11-FAF0-4BE8-9E9E-8031B0567E46_2/zj3kyb6geJV6vTbysES7TGabDr37nxR3jvZloIqxHGwz/Photo%20from%20Library.jpeg)

Oxide top, Cr bottom 

Arc

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/0B22039F-0370-456F-AF70-DF84190AA11D_2/0xHCEnLbIE2uSqX4ClQ076RXSaLNxXWS65drceHKwzAz/Photo%20from%20Library.jpeg)

We first run the thinner coating on the Cr wafer, so 600 nm

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/731DBEAB-1482-4C1C-B737-563AFC268F38_2/DAIYVRXSoy4Dk1h265ACy6seY7MnET26XMjAYvxN9gkz/Photo%20from%20Library.jpeg)

We then run recipe 1206 for thicker resist on oxide.  I don’t see any issues with ARC coating at the moment.  Resist coating was a little bit nonuniform, but this could have been from the markings left from the sputter.  I don’t think this is out of the ordinary from what I remember

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/3DB18923-DD7A-4FA7-9969-0160D4819D27_2/29nRutlwis1C5UCHiu6HZBxf3po5rAxK9l48ZGjU0SYz/Photo%20from%20Library.jpeg)

Before thick resist

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/880271B5-2E21-4500-8F70-F51E3F4AC6CB_2/lf6Gft0Ity0iaFxOzzUlSoQLtEVcYVh8gU5yGhFYyc4z/Photo%20from%20Library.jpeg)

Before edge clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/E8124557-51E3-4739-950E-76F36EE36CC2_2/r9b5pclEMnEG2s3EyHEfUmxaZ0WzDWjP22V3LF8pS4cz/Photo%20from%20Library.jpeg)

During edge clear 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/106EEF62-3973-4D18-A5C1-A3D8042AFFD0_2/WESWHgahCxHEixszxsg6Y1rraiiJ7NNLplPnVXmXDz4z/Photo%20from%20Library.jpeg)

During edge clear 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/75E97901-13AA-467B-A15A-DFF721B56257_2/zdKiIib7QZrsQ9QOstWzbhY8PXhPXd9tmgFUOeAEQksz/Photo%20from%20Library.jpeg)

We read mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/C3291E17-43B7-4104-B161-78BD7625FCE0_2/Oym6PeFuCxEd7owboO30h3sx5iipG8X02gSbQY88XXoz/Photo%20from%20Library.jpeg)

Before exposing Cr

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/8A69A3F1-9662-4F70-B5F1-5B80DF588F86_2/sfJ0xlwJC51asQykfmKZMLWySc2a0KQ7s8VFvCMwXE0z/Photo%20from%20Library.jpeg)

During Cr

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/0FCBB8DD-2CE6-4550-9D5A-30E1F543E03E_2/dwL7h3tGA34oqm1J55xPQDZJi3EQ9wdHznyEDaJFtEsz/Photo%20from%20Library.jpeg)

Before exposing oxide (use dose of 20) and changed all images

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/2D18C142-9E6B-4813-870B-8F2D0647D6F4_2/VQXNjoWIyUAMS96R491Rjux1AgysmtdGV3plbzLMcUIz/Photo%20from%20Library.jpeg)

During oxide

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/63AD41D6-2622-4850-80CC-92DD11DC57A0_2/kyROsPPvorTItIZ1xcfKNROqiX2yaZZUa0J2xN13zqIz/Photo%20from%20Library.jpeg)

Before developing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/3A461B69-AACE-47EE-B084-B562707844DF_2/VEL80fW5R29KhqnqpBzFyMa48fqQ7F7VHd6d5Ejg6Bsz/Photo%20from%20Library.jpeg)

Once more, Cr does. Not fully expose

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/6479A5BB-CCF9-412E-BBA4-C679FFB340F0_2/uwhkkH0kKrvFXvsEyM0PpAxxTMSwp7pilmFraZlmUjUz/Photo%20from%20Library.jpeg)

Let’s do 1:20 descum on both and see what we get

### Etching

We clean 82 for 5. We now do 1:20 descum on both wafers

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/6B28815B-6116-4B6D-BE00-DF05FCF8267E_2/ty9LAxtdqE6xcbo0J5BlRirQ8whecqJJYj2VqCOmtlEz/Photo%20from%20Library.jpeg)

Plasma during process

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/71A3195C-8677-4B73-B0E4-3AE2DE3CD792_2/nIlp3D8yHvIEUlJukOmLlVF5I31GVTq00dLxuUlidhIz/Video%20from%20Library.mov)

45 seconds to a minute is needed to change color

Let’s measure resist thickness after on thick wafer

After 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/11F563D2-76EF-4372-919F-049F1C54B934_2/4a5SkU45yQf35W1xJhyETeYNJfdQT7sGWG7Pmq8p3r8z/Photo%20from%20Library.jpeg)

Profilometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/C809646C-1BD3-4DC4-97E8-25B6C425D063_2/i51Fw4a2USWX5HyfQIIHZ0oPoSbcm3KOl8py979Oepsz/Photo%20from%20Library.jpeg)

Very consistent

5 days later, resist broadly seems fine

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/C5D50E95-0C18-4FC4-9F7A-A1062CB8789C_2/RZh5yKtgabAiF7QSRkJE04Mva88FNA6IApo7SNAItgAz/Photo%20from%20Library.jpeg)

We will just do Cr wafer as truest baseline

100 during 5 min clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/213A600D-56F7-46F0-9781-667675947E6A_2/NBDrWalxzXM1fZ91a9ovZzhwDcCMPHOPVy12bnBQlVMz/Photo%20from%20Library.jpeg)

Good cooling

We did a 4 minute season, then a 7 minute etch

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/DBF140BE-ED07-4090-BB61-D4A144A31B51_2/QYrg7xmy5ml0I2J6SrRrBlfIzUZhZOjsLU8d4VsLTKYz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/9CB36DE8-3582-4366-AA21-3F3CEC4DB995_2/PyrJpRHrkWycdh3QjKN1aTHbOXrVsTkKNJAWth97ABYz/Photo%20from%20Library.jpeg)

After etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/760DFF0D-C7A6-49A0-897B-EAF3B151DDD8_2/8NoeMOxpw3i5klR3oqqYVGUWkjsj4beJEmQmyxpTbFwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/B664A857-8A8D-41FD-898D-FA46AC74C3D2_2/ZKcC3fFdg4F7KLBYxPZPmIPx0Gx0Qw6f6296BXYwsIAz/Photo%20from%20Library.jpeg)

This is ~100 nm shorter than last time.  Frustrating, but I don’t think this is critical.  Last time, I also looked around a waveguide, not a larger step.  We will just have to see.

I will also do a piranha clean of my wafer after the acid etching.  I don’t think it will hurt.  I won’t do eco clean in case the Cr oxidizes.  In theory, the eco clean should be fine, but I don’t want to play with fire.  I will then do 10 mins of smooth oxide deposition.

Before piranha clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/24A34A29-1486-4CC7-B43A-ECD0CE49DBD5_2/7iKHkmomMnJ1sJ3mMPsnaqrxFTEORF2DOyxB6ma5x04z/Photo%20from%20Library.jpeg)

After Piranha

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/DD7CC042-5D3D-4195-B62E-854E9EB5EF9B_2/db2JD2C5RQNz7SB333It5eyfiy4lkL3krZZzZTWciZsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/B38D9928-8488-4947-BE8E-12AA9DE9BC7F_2/4tKPvTRbhvdfiFtFCTCdQ9BRU5zVaprbGZ4Gu6ty6o8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/DC17397D-BFE3-4CCE-B8C5-AFB922263414_2/rQTAfYzTrUs2YXQoxapSLhypZEgXeq1htvr1xkCyVFsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/54BE4BB1-A907-4AC4-BEFC-8DA6436675E0_2/O31NM5QspLNXs6uzEffeNcRNRCMWpoMqNPgCHgDqSx8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/23370333-80EC-4848-8982-9A92CC1A32DD_2/X7G5SQflzkX5Aq86zywpLWlv4QbYbaPWSNydd1Xu6KYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/5510A710-E0BA-4108-B3BA-5335AB078735_2/ltP76e8nwfqnUxrGDjWDMwZpUZr7O99IYk2afBibbycz/Photo%20from%20Library.jpeg)

Still a bit of micro masking

Before Pecvd

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/71E31A8A-DB31-4B69-B793-13AF24C56EAA_2/5b3OPWSBdwxzxxTAGwjludBDOgjH3fByoc9bftY4Mvcz/Photo%20from%20Library.jpeg)

### RTA

During calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/DACD8076-DCEC-4191-9293-DC90EC538146_2/vrNH0OUiPXnqpCfCpOkQhu6xt8DZRJIoo6CDjcWVxBAz/Photo%20from%20Library.jpeg)

During main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/AFEA5993-06CF-445E-B14D-D4FE67117F19_2/yTiVblrWq6yQ1UnxpzvxLfjTnTzhEiLkhA1Cfuqbth8z/Photo%20from%20Library.jpeg)

Half the chips don’t have RTA

### Loss test on Cr

Edfa main setup 10x

3 um RTA die 1

Straight 1

3.9 mW

Straight 2

2.8 mW

Straight 3

2.5 mW

Straight 4

2.7 mW

Straight 5

1.5 mW

Euler 

0.5 mW

Circle short

0.2 mW



RTA 3um die 2

Straight 1

3 mW

Straight 2

3.5 mW

Straight 3

3.4 mW

Straight 4

3.2 mW

Euler

0.33 mW

Short circle

0.5 mW

Long circle

50 uW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/F99EBB50-6A59-4A4A-8BDA-978D191E78FD_2/g06cpt0ZExvfx01KeLFW5zAO6snQQt0nyx36YE8jsfcz/Image.png)

Not a perfect calculation, but ~2.5-3 dB/cm feels right to me



3 um no RTA die 1

Straight 1

1.7 mW

Straight 2

2.1 mW

Straight 3

2.2 mW

Straight 4

2 mW

Euler

0.18 uW

Short circle

100 uW

Long circle

30 uW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7CA1AE59-4B37-4AA8-A260-87A62519919D/481C3E11-07AD-40C3-BB71-258C6F2269EE_2/uWEVy73NlOa8SxB0ms5uyCI8IQXRxHJx4CQeeQob9xUz/Image.png)

We don’t really need to run the 2um waveguides, as I can’t get the idea above.  We roughly get the idea that the waveguides are still pretty lossy.

Unless we see a mW out of these device, we have some issues.  The main challenge is we have seen at least 1 mW out of comparable Euler Spirals in the past.  We have definately had some waveguides with 2dB/cm look like this with euler spirals.  So if you think the loss is dominated by some bending behaviour there, then maybe it is not such a big deal. We did find the in the past that the circular spirals always did have lower loss than the euler spirals.  I guess I wish I had put a cicular spiral in the baseline die at the bottom.  Oh well.  This is roughly consistent with the values found here: [https://tdwg.craft.me/xR4W6jytzF1ND1](https://tdwg.craft.me/xR4W6jytzF1ND1).  We can somehwat glean that the oxide hard mask was not the issue, and ARC was not an issue either.

While I want to believe this is a mask-specific issue, there is a part of me that is starting to doubt the new SVM wafers.  I have a suspision they are inherently higher-loss.  This means we will need SRN3 more and more, which should have a lower loss in the RTA annealed state (at least less than 1 dB/cm).  I am also not quite willing to blame the bad cooling, as things have been rather consistent.