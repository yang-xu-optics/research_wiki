---
type: craft-export
title: "2025-03-01 1100c sinx annealing literature search"
craft_document_id: 652B85D3-083C-4666-8C02-7196EA8285DB
craft_collections: [etching-sin-waveguides, fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-03-01 1100c sinx annealing literature search
While Ryo and I previously showed 1100C to reduce loss at 1520, recently annealed SiNx devices with full packaging still showed loss.  There are a couple of differences between the devices, listed below:


1. The origonal device that showed minimal loss was ~1cm long, while the deviec that showed loss was 2cm long
2. The origonal device entered the furnace tube as a piece, NOT a wafer.  The device that showed loss entered the tube as a wafer
3. The origonal device that showed minimal was was air top clad, while the current device that showed loss had a PECVD TEOS top cladding. 
4. The device with more loss had a photoconductor.

Personally, my suspicision is that the TEOS layer is what increased our loss.  That is a PECVD layer which probably has plenty of Si-H and N-H bonds remaining.  We also should have pushed for the furance tube to go higher than 1100 C.  The last part is this is a diffusive process, so it is possible that 3 hrs was not long enough given how thick our waveguides are.  I personally don’t think the fact that we annealed on a full wafer matters too much, but that is just me.

[Optica Publishing Group](https://opg.optica.org/oe/fulltext.cfm?uri=oe-26-8-9645&id=385310)

This is the first paper Ryo sent me.  For reference, I am not really that interested in what they used the waveguides for, mostly the fabrication and film characterization.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/6B79275F-4C7D-4A94-8C54-FD1652A93C22_2/WyzoAq4GdYzwyrASutsW7YHTvrnsWRCeVcxnXbTOpV4z/Image.png)

They use our same trick of etch first, anneal second.  It seems they use fairly thick waveguides and observe nonlinear phenomina, meaning annealing should not totally screw up our ability to see E-Fish.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/4FEE7BDD-D27B-4B86-9461-24ED5C165CE9_2/kWGGxEYyR6xEboirfl7iA2x5vWxG67rMhZQhXAtUahYz/Image.png)

They mention using a thicker BOX, which is nice but we can’t do for electrical reasons.  They also use a smaller bend radius than us at the moment, meaning I am not yet worried about our spiral waveguides (and theirs are impressively long).  Other dimensions are actually more aggressive and I am surprised this worked with only contact lithography

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/42A5183C-A137-42BA-B324-A06322570C23_2/SX4YN32qizie1ZIu8TfQedRN0PHcqcQedoeU1cyyOAIz/Image.png)

They now show my first hypothesis.  They do cladding BEFORE annealing.  They also use the PECVD for their top cladding

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/2015608A-6C5C-4981-A3A4-94BA505083F0_2/SlXefF25M2HKoyzQe2epO2PyuUXC2geeUPT4WBBqGjUz/Image.png)

Another important idea is somewhat confirmed here.  They anneal at 1150 C, not 1100 C.  I believe this would make a difference.  Their atmosphere is also a bit different, with the first part being O2 and the end being N2.  We do a mixture of the two.  I don’t think this matters a tonne, but I am not sure.  Their ramp is similar to ours.  Their anneal time is similar to ours.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/D4A2F42D-AE02-4A5F-AEBE-43876DD3EB42_2/emmBkxRWORlQvgWQllTRxzgPcFI4FbdLiywxGSoX6Bgz/Image.png)

Random: They use a very interesting spiral shape, but it would probably be easier to align to something like this because input and output overlap

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/B82FE3B4-C316-4BB8-8C3D-A596879974DB_2/sL5RuT4BTsVwFO8WN9ZMmII0yyGhkppkFNxGNYwVDhUz/Image.png)

Tough to analyze what is being shown here.  They still have photoresist ontop, which makes me believe their waveguides were a bit thinner than ours.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/DCE41471-8E2C-41FF-938D-0268EDE88FB0_2/DesOmRMOyJKp0PPLH8sWFJln4Xh9CwEEgkjjO31z6IMz/Image.png)

Their transmission without annealing, which looks like ours

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/344DD1DB-F488-402C-9B0C-6E65F3F7C613_2/3yAwyYZF1AVGqTdzSCFP5LhRPM87pZixqMAynrEz8bwz/Image.png)

This also kinda says our tempurature might have been too low

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/F2F21210-7498-49A0-A4BD-EDB622E1E7B5_2/Lyr353WJAQhWyZRfaapxaaqNYw2q5XzHjdWfsNC5Ezkz/Image.png)

After annealing, they see flat loss

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/36643563-207C-4A3B-B880-11BFFC6CA5DA_2/ftFxUkixAVMYgZyE56OTcy9btyt72udh3syuXloyVHQz/Image.png)

Just the effects of scattering loss, but they finally confirm their waveguide thickness of 580 nm

[Researchgate](https://www.researchgate.net/profile/Alfred-Driessen/publication/241875246_Characterization_of_thermally_treated_PECVD_SiON_layers/links/0f31752ebeffabc15e000000/Characterization-of-thermally-treated-PECVD-SiON-layers.pdf)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/ED1CDC28-51AC-4ACC-91A8-AB3AB7825739_2/PiRn1lbGF9vPmm9xywTk2AJiayuCcGBezxRRFAZeVF0z/Image.png)

They use an N2 environment.  I truly doubt it matters much, but maybe I am wrong.  They also use a higher final annealing tempurature.  They seem to confirm the 3 hour annealing time as well, and they have some fairly thick films, so I think it transfers to us.  So I don’t think longer annealing is needed

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/0E2013CF-0EB1-477F-A2D0-80E58D652A5B_2/kyvL4T5ZF4ZtywKCtikLAIMxtrN3eIKmeOxLKiFNyxMz/Image.png)

It is interesting to see that annealing at 1000 C really does not help much.  They mention crakcing, but given our etching trick, this is not relevant.  This reinforces the notion that 1150 C annealing is best.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/0CB43CF2-1FC7-4A97-A102-0DC7F3B00127_2/UAjII3khrbgdVYKqBmzpt8hLf6C20bNLtTDAMIDiKAIz/Image.png)

Kinda as we expected.  The N-H bond is really the killer

[Laser annealing of SiO2 film deposited by ICPECVD for fabrication of silicon based low loss waveguide](https://link.springer.com/article/10.1007/s12200-016-0616-1)

These people seem to help confirm my intuition that PECVD SiO2 is lossy, though I can’t say they give the level of detail that I would like.  They test their waveguides with SiO2 claddings and Al2O3 cores.  They also use a laser annealing procedure instead of furnance annealing, so this is not a perfect apples to apples comparison.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/934593F4-5FA7-444D-B324-3A59C640BBB3_2/p2slUmJRKCoy4Wyhv7iPGyJQvGYZktyVfHDQB3ySQooz/Image.png)

This more confirms my idea that PECVD oxide != thermal oxide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/081DF700-E9CA-4149-90B6-A6F37321C909_2/bA9WjfnqFv5JKBoZccXisq6aQ0lKqmiGwxaQl5jNAuYz/Image.png)

[Optica Publishing Group](https://opg.optica.org/oe/fulltext.cfm?uri=oe-19-24-24090&id=224301)

This paper again confirms the oxide intuition

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/0BD03BED-9658-46D1-A6F0-B251BC543EDF_2/SJDGERZBSXdqozhxgW6Kwio42jcxR5qdsI8ywH6ysDsz/Image.png)

They also seem to do annealing of the oxides

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/8B1F2E16-E550-4E2D-A80E-533F2D362D04_2/PGROYS1yxTJ6uGxO4Si262oHyGzcOvxd7CmLPQyvUZMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/E8DCC204-3611-46BC-AC22-5CFE48B9E98B_2/qt8H04YbxjJMbgb9UCcfV3EXUVMaL2fMnEyH2HUICKgz/Image.png)

Below they report on losses

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/515C2B1E-5FDD-4475-9D8C-D800231A2369_2/IZcDgFZEuHqUQ4Y531xlrxy6FU8IWHAtJFqr1gp7Dhsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/31DEA0DE-C868-4B8C-9261-62EF436206B4_2/kXUAzZNz5DOpua9mcBXE6ETvf35SsNZM20eTUkC3YxIz/Image.png)

An interesting feature here is this is still with waveguide annealing, though the losses are still very small.  I guess this goes to show that the photoconductor is probably causing some amount of loss, as there is obviously a bit of overlap

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/BFC3961C-79AE-48B8-AAD4-4742215FD63E_2/h0hZVcCgNa25qDFsAyNYhR2No4FXaSRnX9hntYDlHjsz/Image.png)

Above is with no PECVD oxide, which is obviously better.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0925346703003513)

This seems to be a sorta “seminal” paper on the composition of PECVD films.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/A3D8BFBD-0A98-413A-AD35-B2821A599AB2_2/gmI9W6sPRGIbNkK1QOeTgnOOJ2tATaub9BQ6dYEWhH4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/A3DA2E9F-F8BC-4E2C-8E8B-62A3EE58327A_2/9f5R1yBXmUJ5DfvDJu4yS3RDRHLlEHcpPA0ggc7UpqAz/Image.png)

Above is for oxides

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/D631243C-30BC-4182-8DC4-9788F3483B20_2/ip7Ay1fofs3AgWYgHJlW915fOHhecyCHaAXynptFUKAz/Image.png)

Above is for oxynitride and nitride.  So obviously the effect of the N-H bond is weaker for a normal oxides, but it is definitely noticable.  SiON is easier to see.  So it is not clear how much it matters, but we see a lot in nitride.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/7EF19D4E-0249-4268-930A-031C9A28B29A_2/tCML1Kw1AB3nZGIyQNMmB4Z6VcDV11WW5xbTIsmnKbwz/Image.png)

An interesting observation is O-H bonds begin to dominate with more N2O flow than N-H bonds.  Our PECVD SiO2 is deposited with a huge abundance of N2O.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/980BC5F6-AF57-49F7-AABA-4CD385286B9D_2/EZjiSnldKhmACyqkXeysMqA4OB8BsxWX5yK8k4QjClIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/C4795028-23E5-4E4B-87C5-1B45BEC97B4D_2/ApiMiOxswbpqyMpaxSDzrwuK2Hz2uegz949BlAHTncMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/302F5D32-1EDC-4828-8D08-6E69553A7B96_2/aX1wrIGVTGonqNAIIzv99xvnT33jmf1eSHkvCBPSiD8z/Image.png)

It is just tough looking at this to be convinced we are really seeing N-H bond issues with our oxides, as they at least have an order of magntiude less N-H bonds.  Then again, we did see less loss otday then normal.  This more convinces me of the need for higher tempurature

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/14F3E5BD-B361-4934-8127-DCACCE0362F1_2/WqbyxViVC7U2kFcBpFzBWGiQQuTK5A5el2OIGxHQiGEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/656E0BE9-9260-47AC-A536-F80A13CBEBDF_2/0ewzBMkLpMcUk3MP4ukhusF211xGERTrMly9O9CT7yUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/0D28BC24-7A0A-4A6C-B933-FCFD3A1BF713_2/UE7uH7gGzva5LpWGcFsbW6DixfK4bTDunoGuSmbGpHQz/Image.png)

They anneal the lowest index SiON (n = 1.5 at 1550) in an N2 environment.  This seems to get rid of most of the N-H.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/3610322D-2964-4C63-B860-FE955AA1F410_2/7uVBmlafrq5qXVp9SIo5JudcG8oevxVLLk8UsGuOnVcz/Image.png)

It seems that O-H bonds are weaker, as they are gone by 800.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/DEDFE0E2-768D-4A19-AB9C-F0743A2817A3_2/e2Xxii3pliTAnS0BOQDzM3DUpEhm1ucQ2LCMw6nPuu4z/Image.png)

This is for the same SiON as before.  I still believe some loss is caused in the oxide, but it is clearly not a tonne

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/43D986DF-673D-4014-BB7F-AA255EA0FA54_2/FuuhtoGdiJJCaew5GSm4aBwBwz9omeO1PmCSnNqK8xgz/Image.png)

They probably use recipe 3 or 2.  Interesting that this is definately on the order of the oxides, so maybe I think this loss is the issue

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/A4A99AFF-C247-4B4F-AD29-A30471441F42_2/SrzIBxCPItCTpx6HGzuzVcNYbyjUzM91R5Z0KGuOXpAz/Image.png)

This seems to confirm that even this small amount of N-H can still cause some loss.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/897964E7-82A6-4F28-AA49-72256DCC7CAA_2/1hEMwwmdLhbH27zOfkimyLPVmEy58US5dj5WGL2oaxsz/Image.png)

They seem to also use 1150 C as the tempurature.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/4D17F983-648D-461A-AD2A-D0255FE95D7D_2/5FQj0ed7SfACoeAYPX2ddyEUN6hqFGnCZo4MRAKpy7Az/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/5E819037-CDFD-4775-B709-EF671B77A4C8_2/7g5HSaSrcFFsUSK71qOHfZZKNBGqT9931Wq1rlRDWpwz/Image.png)

Despite the whole conversation, it seems that they don’t anneal the device as one, but rather use a normal PECVD cladding at the top.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/C9564BCE-00AD-40FF-AD79-5043A8B83B7F_2/DdoHB0JeC5tbM07ErXxUGw7hoPCoUeZnhilRyVUnpj0z/Image.png)

They at least acknowledge this fact, so it might still be possible.  I think the most important thing is annealing at 1150 C

[Optica Publishing Group](https://opg.optica.org/ao/fulltext.cfm?uri=ao-30-31-4560&id=39335)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/B5413843-A862-406C-9964-3916F841F4B2_2/JJcC7ThWoLYnP3FfxxcyZHBQKWHBFP4nXyWfc7IDvZIz/Image.png)

This says it all.  It is also interesting that they use think 5um waveguides and only do annealing at 1100 C (instead of higher).  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/B38ACD7B-A15F-4086-9435-AC306D4FEFE3_2/0xcqHiTS77fVNjRtWg4sDLOJ4uGpl29bmpx5RkQX5SMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/75355E34-2262-440A-9ACD-51B6E219FE3A_2/iypFxIAZVQ7SjKdJ6AgPfESBqQBG0YlczcVQ7lXVFLoz/Image.png)

It seems that 1100 C does not remove the peak around 1.51 um, which would also confirm our recentl annealing results

[Optica Publishing Group](https://opg.optica.org/ol/fulltext.cfm?uri=ol-40-21-4823&id=331311)

A Lipson paper, so we know its good

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/7F1E1728-91B6-4502-AF72-16C02931B9EF_2/9vcIFAZvqDhwLprXGqlqv0U3XUZRZtYGqOj7xDTm3OQz/Image.png)

Interesting that they comment that H has a hard time diffusing out of SiNx

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/A8E757B9-1B44-4128-A5F1-9BBA4C67E880_2/XGsgjCm2f4IJgyFLQg4yEGYMFUyi28CcfUUanUAk1DMz/Image.png)

They also annealing their PECVD oxides, which is a bit interesting

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/5CF14B0D-4FB2-4008-AFFE-38C39C06351E_2/SLCT5ewx96Ml7VFEQS4QxpXQ50jCiSNtyaM3bnToKdsz/Image.png)

They are serious about getting resiudal hydrogen out of their films.  I don’t think we will do that extreme

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/7D48C69C-C5DA-4846-B875-DE0682358E33_2/d36whQY4k2ZGvy0jQ3tCQRRMlr9MSUCwPknhZfFi614z/Image.png)

This paper really makes the point that you want to anneal thinner films to allow the hydrogen to leave the film.  The above graph is without annealing cycling, which is evidently worse

[Arxiv](https://arxiv.org/pdf/2301.03053)

This is the old paper that Martin and I got excited about for using SiNx from the PECVD as a waveguiding layer.  As we are learning now, processing SiNx is not so trivial.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/30970CD1-20F6-4F8C-8006-1E6185B64E06_2/ASJyUS6eHxUsAk7Se06ORIgMErKxDkZO91YTitTmXRwz/Image.png)

They annealed at 1150 for 3 hrs in N2 environment for PECVD SiNx.  They had top cladding on, and things seemed to work.  I am sure the loss would have been better if they used cycled annealing (based on the above paper), but for our means, it looks ok.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/D84FA226-0CA0-48AB-9CCE-215AE2279C85_2/DwyPFtbiTdvkhbZFOle659r5Jm4xIoS2y6AD8ifZQVQz/Image.png)

Above shows how loss goes down

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/C1C6C5AB-1B88-44C6-89AB-13E7E86F1DC0_2/6wZMclatq5yxgGTMzxI92vV2BH1ZECxm4Jz3NkjggBkz/Image.png)

It seems RTA helps reduce loss, so we should be able to observe some imporvement over the RTA devices with furnace annealing (at least that is the hope).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/652B85D3-083C-4666-8C02-7196EA8285DB/09B35E48-8DF8-4171-8E01-2780F338413C_2/g01TVgEJGXjRvRJFzKxc5sUMS6O3doLOZGN7lLh9ymcz/Image.png)

Interesting that reactively sputtering SiNx could also be good.



Email quesitons for the last paper:



(Some greeting), 



(Some introduction).  We are emailing to inqiure about your work reducing loss in PECVD SiNx in [https://arxiv.org/pdf/2301.03053](https://arxiv.org/pdf/2301.03053), which was performed in the CNF like our current work.  We previously demonstrated programmable E-Fish on a slab waveguide (reference to one of your conference talks or attach paper manuscript).  We are interested in expanding this work to etched SiNx waveguides to take advantage of the higher propagation lengths, confinement, and dispersion engineering capabilities.  Additionally, we would like to eliminate loss at 1520 caused by N-H bonds so we can do spectral engineering over a larger range of the C-band.  Because we are using etched waveguides, our structures can survive annealing at high tempuratures without stress-induced cracks.



Recently, we fabricated SiNx waveguides and, after annealing, we did not observe any drop in the loss at 1520.  We measure loss by coupling into our etched waveguides using an aphserical objective lens and use a power meter to see the transmission spectrum from 1500 nm to 1630 nm.  After annealing, we still see a distinctive transmission drop at 1520 nm with greater transmission at 1500 nm and 1550 nm.  Our fabrication procedure follows the following procedure.  Starting with 2um thick SiNx wafers from Silicon Valley Microelectronics (inlcude link to wafers), we deposit 300 nm of PECVD oxide followed by sputtering 150 nm of Cr.  We pattern the Cr and then use the Cr as a hard mask to etch the SiNx so we have waveguides with widths between 3 um and 9 um.  We wet etch the Cr mask away and then anneal at 1100 C for 3 hrs in an N2 and O2 environment.  After annealing, we deposit an additional 1um oxide cladding in the PECVD using TEOS, deposit a 6um silicon-rich ntiride layer in the PECVD (which gives us programmability), and sputter 30 nm of ITO.  



Our questions for you on how to minimize loss are below:
1. We saw in your paper that you anneal at 1150 C.  Do you believe this 50 C tempurature difference is critical to removing more N-H bonds?  Do you believe annealing at 1200 C would be even better?
2. We saw that your waveguides are only 730 nm tall and 1500 nm wide, meaning ours are much larger.  Do you think that larger waveguides require longer annealing times?  

3. If we had to keep the annealing tempurature at 1100 C because of CNF material resistructions, would longer anneals help decrease loss?
4. Is waveguide loss performance effected by annealing with or without the PECVD cladding on the device.
5. Do you expect that PECVD SiNx’s provided by different sources (ie, one from the CNF’s PECVD and the other from SVM) to have different annealing conditions to remove loss?
6. Is sidewall roughness effected by annealing, and if so, how?



(Closing statement and thank you for his time)