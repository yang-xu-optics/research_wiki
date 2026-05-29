---
type: craft-export
title: "2024-9-6 review of e-beam systems with sinx"
craft_document_id: E2DF52FC-47BE-47F5-958E-6D15AA9DA37A
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-9-6 review of e-beam systems with sinx
The purpose of this document is to figure out an ideal fabrication flow (specifically for lithography) for patterned SiNx waveguides.  There is a bit of an assumption here that I am going to use e-beam, so I am going to be biased towards those sources.  The hope is to see whether people use masks, how deep they etch, and what are the general tricks they play on their resists to make them have the desired shape.

This paper ([https://www.nature.com/articles/nphoton.2009.259#Sec2](https://www.nature.com/articles/nphoton.2009.259#Sec2)) made SiNx waveguides in the CNF for nonlinear optics (a product of Lipson's group before she left Cornell).  Below is their fabircation processs

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/75EF125A-8A6D-4654-855D-0A3BB7A87D56_2/rq587WuLMTTTbldXbnt7uiBkYNRltfbkVB45r8mDD70z/Image.png)

I am not sure what resist they used off the top of my head, but I would venture to guess that it is negative (as the N in the name).  It seems that they did NOT use a Cr hard mask.  Then again, they only etched 500 nm down, so maybe it was not nessesary.  I would be curious to know how they removed the resist when they were done, as that can be quite tricky.  I would also want to check that we use the same etching chemistry (That being said, their current guy who comes to CNF uses the 100, so it should work)

This paper ([https://iopscience.iop.org/article/10.35848/1347-4065/abc78d](https://iopscience.iop.org/article/10.35848/1347-4065/abc78d)) seems to specifically test e-beam exposures on similar tools to ours with SiNx waveguides

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/2DD21D68-5989-4539-B000-57973A955926_2/jvP5yVxGPzntQKGAVqIkVimeEhAVCqtXm65t57AuJxsz/Image.png)

They seem to think 700 nm is thick.  In theory, this is not impossible for us to etch with.  We would probably remove the resist using the oxford 81/82, as it will be fairly burnt.  My general worry is that, if the selectivity truly is 1:1, then we have some issues.  But if it is better, (even 2:1), we should be fine.  I feel like it should be at least 2:1 on the oxford 100, so I don’t think that will be a big issue.  Still, we should probably cleave up our wafer before we start etching.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/66CB188A-7D63-49CF-8E52-5717EC64372A_2/rmd3pnFzw2QMRkFEOhaP4O9tiPyq38OcOQ9z8yguJ0cz/Image.png)

These people also seemed to cleave the edge to include the waveuide, which sorta makes sense as it allows us to access the edge more easily.

I am not sure how useful these people are ([https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=887192](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=887192)) as they use some very exotic processes that I don't really think it is worth it for us to develop

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/AC9ACA19-C70C-4444-B1B3-5A2FE721D8F1_2/50Mya1A2W9cbXcLSMgxKo5vk5EbRal0kKi2AvDeaX4Mz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/82A12BFA-9772-42FD-9E52-6676DBAB1814_2/aCg4G3HVXy5ue7XL5YmxMgJCTPDEXDfKdFDDDQ5xYywz/Image.png)

The annoying takeaway here is that these people generally use thin masks.  This is annoying, as 150 nm is most definately too thin for us.  They also use some exotic developing and etching process, but it would really suprise me if the resists we use don’t have some standard developing processes.

It is a bit suprising that they bake for 45 mins.  This feels super long.  The pre-bake only gets rid of solvent, so it does not make sense why they do it for so long.

Something that is reassuring here is that no one bakes after developing.  My fear was that those bakes help the resist get rid of sidewall roughness.  Then again, we were going to photo-lith all of these features earlier, so it is doubtful to me that we care that much about roughness. Either way, we don’t need to worrry about a post bake unless Oscar tells us otherwise.

This paper is the one Martin found a while ago ([https://arxiv.org/pdf/2301.03053](https://arxiv.org/pdf/2301.03053)) 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/47C8C75E-49BE-47BA-B35D-A2DED5A23801_2/WCIyDwsnfleVJR2zetzVeHFccxKnNgnw0FRjRlQev6Az/Image.png)

Firstly, these people are impressive at polishing.  I almost wish they would detail how they did it.  Something very impressive about this process is that they used an oxide hard mask on nitride, which is kinda brilliant.  I do wonder a bit on how well you can tune the selectivity (as I onlny observe ~20 nm/min differences with my recipe) but this is a very cool approuch.  We probably need to be more deliberate about how we pick the etching recipe in this case and stay away from the high rate recipe (Which itself might heavily polymerize the edges). Even if we can’t get the cladding the way they do, this is still a really cool approuch with equal selectivity on oxide and nitride

The key takeaway here is that they use ma-N 2403 several eyars apart, so if they use this, so will we.

The file below is the PhD thesis done by the first author above

[Ji_cornellgrad_0058F_11164.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/3026428D-9BF5-4CA3-8B87-3CF142CE2CFD_2/8yUXNZ6TEsQK2lHPqPGtlzun0ONwKp6hhHtDrrPnPqAz/Ji_cornellgrad_0058F_11164.pdf)

It honestly has super impressive detail, and it was completed in 2018, so it should still be useful.  Below are some useful passages

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/8D15FF90-80DB-4EDD-9771-C544541FC7E9_2/jlWwNWgfJmBUxfK6G2PaFNyKcZNNBoWrzGWsaJXJsRsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/230B0410-B0D4-48E6-A54A-9B114CBD8906_2/cIl7RC6Am7RLX28LCgzEzddXGRGLrcCrkrhxCMqZouMz/Image.png)

At some level, the Piranha preclean might be a bit much.  Keep in mind, this guy is making ring resonators where every dB less of loss is a gift from God.  He has designed two processes, one is standard and the other is his special one.  At some level, while I think his special process is very sexy, I feel like it would be best if we avoid something too complicated.  Again, our loss requirements are not as advanced as his.  The only way I would do his approuch is if he wrote down the gas flows for everything.

For resist, we are definately going to copy their standard approuch.  This means the follwoing steps:

1. spin coat surpass 300 on the wafer (adhesion layer)
2. MaN-2403 at 1000 rpm for 30 seconds to get 700 nm of resist (assume we use high ramp and same recipe for both coatings)
3. Bake at 95 C for 1 minute
4. Spin a chemical e-spacer at 2000 rpm for 30 sceonds
5. Use a dose between 900 and 1000 uC.  
6. Use Hamatech psin developed with MiF-726 for 90 seconds
7. Hard back at 135 C for 5 mins.  This is the reflow process which increases selectivity but can cause weird trapazoidal features.  Maybe a bit shorter than this would be better (say 3 mins)

Something interesting (but very much makes sense) is that he uses greater dosage and develops for differing times for differnet resist thicknesses.  We only do the former for photoresist (which is a bit strange)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/88894051-C0D3-47D2-B240-B26BB0BF2E2A_2/NL3pkbFouVm35bbnNW7S6BPRo0QLCTmM6OLzXtObTloz/Image.png)

As a side note (while he does not elaborate on which pads and slurries to use) he does seem to confirm our previous observation.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E2DF52FC-47BE-47F5-958E-6D15AA9DA37A/A9CB001B-244B-457B-A617-8711ADF791C8_2/x3CxISn93yywYvSZzbSVo7bJU50MyjQnsWqkIMwu8eAz/Image.png)

Another cool trick this guy plays is multi-pass roughness reduction.  Again, unless Alan thinks this is easy, I say we avoid it.  we are not as obsesive about these losses as the Lipson people are

Honestly, I don’t think we need to do any more looking.  This guys has got it figured out