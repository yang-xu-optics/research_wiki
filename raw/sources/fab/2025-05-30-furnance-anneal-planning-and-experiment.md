---
type: craft-export
title: "2025-05-30 furnance anneal planning and experiment"
craft_document_id: E4A73334-2077-4950-97FF-CEC97FC3F260
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-05-30 furnance anneal planning and experiment
We have now succeeded in reducing loss using ASML.  This is because we were effectively able to reduce edgewall roughness.  Now, we want to focus more on thermal treatments of the wafer.  While this is not confirmed, I have the suspision that the performance of a film after furnace annealing is somewhat dependent on the starting index of the film.  The idea is we want the index of the film, after annealing, to be as close to stoichiometric as possible.  This means, for higher tempurature anneals, we want the starting index to be quite low.  There are two things that would be interesting to test here:

1. Whether furnace anneals are better than RTA
2. Whether higher tempuratures do have the possiblity of helping reduce loss further

The first is easy to test.  We just put some pieces into furnace tube and anneal at 800 C.  I am not sure what the best proceedure here is.  We could either do an Oscar style anneal where we load at tempurature, slowly let the lid close, and anneal at 800 for an hour.  The plus there is that is cheaper.  The minus is that we run the risk of stress cracking from coefficent of thermal expansion mismatch (as the heating is still rather rapid) and 1 hr of annealing might not be enough.  The alternative is we load at 300 C, heat to 800 C over an hour, and anneal for 3 hours (and cool over night).  We currently have the following in storage:

1. SRN 2.7 Cr mask and MLA
2. SRN 3 oxide mask and ASML
3. SRN 3.5 Cr mask and MLA
4. SRN 4 oxide mask and ASML
5. Takachi Cr mask and MLA

We can also make another SVM wafer, which will use Cr mask and ASML.  We don’t have perfect baselines of absolute loss values, but we will be able to see how the relative loss values of all these processes change.  This is because we took 800 C RTA measurements on all of these processes.  I definately think this should give us a fair comparison, as we will see which processes see by what percentage loss goes down.  We are not concerned with the raw loss values.  Only the relative percentage change.  

From Gui and Oscar, it seems that we ought to do the longer version of 800 C annealing just to be safe.  So lets do a 1.5 hr ramp from 300 C to 800 C.  Lets then do 3 hrs at 800 C.  This should give us a good idea of what we are dealing with.

After that, using whatever pieces we have left, we should do roughly the same thing, but go to 1100C.  We should just use N2 anneals or Ar anneals.  No O2 should be added, as that will just oxidize stuff.  We should at least spin clean all the pieces before we do any high tempurature anneals.  The general intuition is this should be better than RTA.  If 1100 C works, then we can make some new waveguides for 1150 C.  Before we do the anneal, we may want to make some new SVM waveguides.  We can just mass print the previously successful spirals using the same recipe we used on the hard mask pieces.  

### Lithography

ARC coating

![Photo from Library.jpeg](../../assets/fab/2025-05-30-furnance-anneal-planning-and-experiment-001.jpg)

DUV coating

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/3624A944-0D06-4934-8891-4F60427BD0D6_2/tzPsZQTqA2KquusxyxrFPDyIGlzubIuXcJGUyx1awWwz/Photo%20from%20Library.jpeg)

ASML

We read the mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/FAE9FBAC-30C5-4AFC-B7E5-762D939F0454_2/hzsyTDLGf7PjQISNRWx3xMaSCgKc0d5BUM4ODeJs2Fwz/Photo%20from%20Library.jpeg)

Input output in batch data

Before clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/E6419775-399D-40F4-9E57-D88B26945F81_2/lvodJdUBWzUhkLSlGJGxgV6D6Bfx6qshzF8WexFIZvEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/D6DE9861-559D-44A4-A31F-8ADE2314C154_2/DB0cQgnkvRLuG0ZPPVeNtzac8roRyDLep0xCFLAHJCQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/D501E68A-8594-4A34-A8FE-46DCE2806732_2/sisPigNYsnoxBJRvCyBv9Gc4s0mZf50DoqYukjyMEPYz/Photo%20from%20Library.jpeg)

Before pattern

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/2C53F0EF-FC58-413F-BCBE-8F523A01DC47_2/XpqQohzqlJL0tzjco3LJOrBixOAU7U9gyBMzVFGUVqAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/79916DF5-6D73-4906-A512-72003A962640_2/y3Qzh8Kf4XGJYyQ0J9bbzvOoy6kqNWbY4LJkaUcRcxcz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/85021932-33D9-4BE8-88DB-FC782B02B3B8_2/jlBx52eal5uEl1G4IJB9H0su9xeSU2UQVaLyPCrFNSAz/Photo%20from%20Library.jpeg)

Development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/461AF7CD-3137-4344-8607-47ED91E95A12_2/ZhMFyXEiNLvleyhaUoejoTlYtRxrp29b2gPOST0gLUMz/Photo%20from%20Library.jpeg)

I think we undex expose, did not seem to remove everything

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/9EEB32EB-D000-48B9-B67B-AC457487DB00_2/e4R9bp52tsxYe9WZNo0byyBQfWcL5xraxCoJxOoJqmAz/Photo%20from%20Library.jpeg)

In future, we should use dose of 20

### Etching

7 min pre clean of 100

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/39CDC7C5-A988-469B-B8B6-733D82703593_2/xyqiqcOKrtGkaCqFq8dhOls7EqyZiDkEYXhpS68yTUkz/Photo%20from%20Library.jpeg)

5 min pre clean of 82

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/82BB15A8-BEE4-453D-8BCB-4AEAB62D18D5_2/8nfKAr562o7ykAfEVM7txxTCvpwl4OB6qjejweMV2jUz/Photo%20from%20Library.jpeg)

Let’s descum for 2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/92638BC8-F805-4C3E-B96C-D7AD11097C19_2/iaHzmYetXKs2w1hkL4rQOvPwUQz7n6GY77IeOIwSECwz/Photo%20from%20Library.jpeg)

100 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/1AE90558-9DF0-47CD-ACE6-59FD385AF2B6_2/hxDxotvpdbjUADHrNMtk53tZMR04NU95uxlRHryyuRIz/Photo%20from%20Library.jpeg)

Descum makes all well

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/9E8AC337-197E-4860-AF09-E90D00D07C97_2/s1yc7YgED1YuxGywybtyCx5MUDKcwEgVfZLSHl4bFbQz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/3467EB90-6D84-4650-8AA3-2B052C57FB60_2/7QU10vHI7ipGYsflLX8qop1FjoNgxuIVOyLxbHbzye4z/Photo%20from%20Library.jpeg)

2 mins Cr etch

Under microscope 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/C8DC3805-182A-4F98-B6C7-E4929BAE9D3E_2/YR0ipngH0f74gOST0sxVz5I5gveby2KXNmKBSkjwOBIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/5A0F2EA0-2236-4432-8C4A-8C6D5577F67D_2/6bdo66x2Q1KUJs2uoChyYcMbjPZgcGs8xh101hsrN7Iz/Photo%20from%20Library.jpeg)

Generally looks good. Few areas under dark field that don’t reflect

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/D1E05B3A-AF3F-4B73-ADA4-29EF1488D7C8_2/vqSqWpgy3CwAMRUKicC4KzuiS2ohQJERD9x8IXrqsxQz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/37F94320-3D63-46EA-A7C4-CF389709B6C2_2/S1jRX3MEyVEo6VkxD68kAxn2dDYXknbReyp6oOeILAMz/Photo%20from%20Library.jpeg)

After etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/A3F8A8E4-C6AF-486E-8BB2-5A19F3DEBBCF_2/zHuOyX4griLBoJ9ckLSlWXoMrjpzgkTV4rCKdHd6Wkwz/Photo%20from%20Library.jpeg)

100 nm shorter than usual, but it’s ok

We now Cr etch for 20 mins and BOE dip for 30 seconds (just to make stuff more clean).  Aaron said in the future we could use the TFT RCA clean to clean stuff that had Cr.  For now, lets keep things consistent.  I will then do 10 mins of smooth oxide to cap the structure.  

### PECVD Capping

we run 10 minute clean

Before 1 min season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/3DAB2B96-9FC3-4C8F-BFE9-FE441CAC9EB3_2/irtGniUiTtQP9ozcVCrYKKBFmJHxxCyO4iIqMc37wB4z/Photo%20from%20Library.jpeg)

We will do 10 min cap deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/66384B43-8791-4E7F-96B6-01E06A16316B_2/eBsywiznVjIMFObRTh9FcqaCayO42dzYODaruEYOvMQz/Photo%20from%20Library.jpeg)

### Annealing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/ADC63EB7-A7D3-4446-9787-E6C0F5F38A16_2/82zFZNdThY4WyDsZCkSJtbKQDeosxp1zh8uEzsMTTDkz/Photo%20from%20Library.jpeg)

The pieces I labelled are those I spin cleaned

Set points

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/827DB2CD-6B32-4DB9-B16D-95AF1643EF2B_2/rr871gbQRtx95KRvchgWI4G0RLrmXLbJ6xnbwsSoobMz/Photo%20from%20Library.jpeg)

The recipe we want to run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/26C30774-CE0C-4405-BD9A-32984639D885_2/fnfYuxPOdVjXpXjcAjaELyTBkBDjGnwQrdWnhfHoyR4z/Photo%20from%20Library.jpeg)

Before run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/463A1225-45BB-4F3D-B1A9-BED48CAB12AC_2/QBymVPS2ehj9TEM86oOmtOkg5saqEorySIeaejrhU4wz/Photo%20from%20Library.jpeg)

Loading

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/15B08382-DDC0-4E06-BCA4-A355B705BAD5_2/xCBJDxJaZ66wnbG9BqstBYp0t2WJuVw0mnmODuB5EVIz/Photo%20from%20Library.jpeg)

SVM back, 4 middle, 3 front

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/5A2F7716-9534-41CB-B30F-9F8755B8C2C6_2/bcJ7cIGAMii3MuXUlyfKPDxH4abw82x3AbbQ6VnnPocz/Photo%20from%20Library.jpeg)

Takachi front, 2.7 middle, 3.5 back

We load fast at 15. I don’t suspect any stress issues with loading this fast 

During load

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/07E3986F-F83D-48FC-A219-E7E3503ABAA6_2/BUcZl1cBHjqYB3hI9v6VVAXTgbKeNHWlxZVxL49J6xcz/Photo%20from%20Library.jpeg)

Ramp has started

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/9536A553-A079-45D0-89CC-B72519B6376A_2/yoBUsOREs5Nm964qUdpNbFRjrymAxTHxVLhu4f13vy4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/10213B36-15FB-47D8-AB9B-0D148E0F16AE_2/mpbgtQaSOuoc6pOIoaIWrBZp7TQX7p7EHno5rfqO8awz/Photo%20from%20Library.jpeg)

Further along during ramp

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/053BBB11-B70B-46EA-9D9A-1C48711A3EE8_2/Fyf0VK2vzn23CdNkBga4ZjGSXSJCH18YpMociUMtgTsz/Photo%20from%20Library.jpeg)

During anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/04FC1822-D895-4A2E-8DCF-12F48F993116_2/VOGNNHQUXA8FCiWDU7mlbsBWtnibzFp2wsMSDn5vZmoz/Photo%20from%20Library.jpeg)

A day later 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/6EFD2C82-7B05-4A45-8429-F5FA5F99E7E3_2/46UyuuM4eIJLCfQJCvH1fZvCINmkbPt1PhM3to38wDsz/Photo%20from%20Library.jpeg)

### Loss measurement

We used second setup 1570 EDFA. There was no visable cracking after annealing. 10 x objective 

56 mW in, though this is a pretty wide beam. Efficiency in may not be great

SRN 3.5

Straight 1

600 uW 

Straight 2

600 uW

Straight 3

500 uW

Spiral 1

120 uW

Spiral 2

140 uW

Spiral 3

230 uW. I think I did the earlier ones wrong

Spiral 4 (longest one)

115 uW

For the calculation, I only used the spiral 3 number.  We generally can guess the loss is around 1 dB/cm

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/7502D8AE-32D8-4884-99B1-CAD4CA9092B9_2/HjtvjThepsivgqXxrLPx8TnBLn7VMyZRSy9QKXhwyf4z/Image.png)



SRN 2.7

Straight 1

11 uW

Straight 2

12 uW

Straight 3

9 uW

Spiral 1

Too lossy to find

Still just very high, which is what we got earlier



Takachi

Straight 1

2 uW

Straight 2

1 uW.

Generally, this one is still impossible 

Still very high, which is what we got earlier



SRN 3

Straight one

830 uW

Straight two

830 uW

Medium circle

330 uW

Medium square 

270 uW

Middle straight 1

679 uW

Middle straight 2

770 uW

Long square

160 uW

Long circle

230 uW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/92DB935F-6D1D-47ED-ABD7-A59EE8B71265_2/8oDHeMPVSqoJyJaGdJwz94GGOeju2yuOHaDT9PiBjhsz/Image.png)

We compare square and circle spirals as the same (adjusting for lenght, but no distinctino for curvature).  Overall, this is good



SRN 4

Straight 1

235 uW

Straight 2

190 uW

Straight 3

200 uW

Medium circle

8 uW

Medium square

3.5 uW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/32AEE030-0936-45D3-9639-FB96667F5F38_2/yA8v76LQRrvSJaKogyvwr62fBcCwRrIxSNu5FyLWUDYz/Image.png)



SVM

Straight 1

600 uW

Straight 2

382 uW

Straight 3

500 uW

Straight 4

600 uW

Straight 5

180 uW

Medium circle

25 uW

Large square

6.6 uW

Large circle

39 uW

Middle straight 1

710 uW

Middle straight 2

535 uW

Middle straight 3

750 uW

Middle straight 4

540 uW

Long square 2

3.4 uW

Long circle 2

Can’t find

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/B8F8B4B5-0FA9-4391-AF16-FEFC5231F957_2/ZIWKntP8TuiWUzWCkesYelQgmDP6mxZXPjgClWykqIEz/Image.png)

Despite all the points we took, I just decided to compare long circle to straight.  I would agree SVM felt lossy.  This is not a perfect apples to apples with SRN3, as SRN 3 probably suffers more from scattering losses.  The main point is SVM only works with RTA, not furnace anneals.  I could not possibly start to explain why.  Below is a pdf of the calculations

[2025-06-02 Cutback Loss Measurement 800 C Furnace Anneal.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/E7EF9359-D5E3-49D2-96AE-0089C21E2273_2/SZXztmG1ZeRy9piUhgtc7OJFZDZ9qjRpBPex2r0m6DAz/2025-06-02%20Cutback%20Loss%20Measurement%20800%20C%20Furnace%20Anneal.pdf)

Below are results for RTA and Furnace annealing

| Film Recipe | SRN2.7 (Cr + MLA) | SRN3 (oxide + ASML) | SRN3.5 (Cr + MLA) | SRN4 (oxide + ASML) | Takachi (Cr + MLA) | SVM (Cr + ASML) |
| ----------- | ----------------- | ------------------- | ----------------- | ------------------- | ------------------ | --------------- |
| Room Temp   | high              | 1.87                | 2.4               | 1.1                 | 2.3                | 1.95            |
| 800 RTA     | high              | 0.86                | 1.14              | 2.5                 | high               | 0.94            |
| 800 Furnace | high              | 0.82                | 1.22              | 3.2                 | high               | 1.984           |

As for next steps, we could just use this time to go straight to 1100 C anneal.  I would all (maybe not Takachi only because I literally know the films are already broke) into the tube.  I have the most hope for SRN2.7 or SRN3.  Even though SRN2.7 is broke now, I have hope that annealing further might revive it.  SRN 3 is not broke at the moemnt, but it might break during anneal.  This would give us a very small window where we could finesse working films out of the PECVD and into the furnace tubes.  I suspect SRN4, SRN3.5, and SVM will all get worse, but given they are mostly broken anyway, no point in not going higher.  If something works at 1100C, then I have confidence we could go all the way up to 1150 C.  Another reason I want to put SVM in is to see if 2um can survive the anneal (even if loss is low, I wanna see if cracks form on a fully etched wafer).  



Obviously, I am not crazy about doing this annealing and long deposition proceedure for each wafer.  That being said, we really only need to do it for the last ones.  We can still characterize new GDS files on SVM and get things close to perfect there, which allows us to save a lot of time.

### 1100 C anneal



---

[`Mon, Jun 2`](day://2025.06.02)

Furnace anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/B6FA191B-B12F-4ECC-ACFB-548D71FB8CE2_2/CNDvBIm7dSHE77TFYxk1V4bxMaWMtfzH3y1ys44nUeoz/Photo%20from%20Library.jpeg)

We use this

Select the right file

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/D51F6732-8C37-44E1-B873-E75AE150690E_2/JqQ6o8OKYmZKcgqi19fAZRGOCgRKU3N6jtSv3Lm6m1Iz/Photo%20from%20Library.jpeg)

We use N2 anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/CE6B5B74-4D67-4328-85A5-23AC5375B2AE_2/7Ii8NkJV7EUZdWvlW6eeUDRcxfxgve69OzVFyJ3YA5Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/72C63BF5-DF90-4049-B429-CBD1CE853293_2/xui1qhgssKXY25uv9wAcyYiujfNGP8vpwxxGILh181cz/Photo%20from%20Library.jpeg)

Zone 4 matters

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/FEEE9CF9-559B-4B8C-B841-F7D7224257C6_2/yTNhVxSpJxkj2lVVzki66858nvM1YClTfrzqKeczcaEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/62D14E78-50E4-44CF-8183-13DB3ACD091E_2/Cv5b6KHZCFhaqx1K4DxG7GrcZAKRQ5ZH9mYZNsd6EXYz/Photo%20from%20Library.jpeg)

Download to tymcon

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/ABEAE11A-BDB6-4183-9815-51CC71A61CD3_2/22axK4CwyEiHU0t4iYCrH0JPw0KkSWxu7MPD0AWgISgz/Photo%20from%20Library.jpeg)

Select N2 annealng

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/01588831-5406-4962-9E0F-0B43BD50882E_2/Q2lAoFT9dCYEBepgiTMyFdp6at1VVXV0LhLvFC9ss84z/Photo%20from%20Library.jpeg)

Now we log onto the tool

Run the recipe 

2 is pause. Stop auto

Pause then menu

3 for manual

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/81AAA1B7-AA45-411B-8737-15A243D80EDB_2/0hObSZQwbfvwwKygMe1iSb0ecmRyKUKL41GiPzOJMxEz/Photo%20from%20Library.jpeg)

Speed 

Make the load speed fast

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/120B56B8-19B2-4495-BDDE-15F9B41ABF13_2/29FpeNp3zc1WVingwQu4iq4szJW0vyVE6y66ratq9twz/Photo%20from%20Library.jpeg)

Unloading now 

Full wafer load

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/173FEE96-CA6E-4F70-B83F-469225276BD3_2/Zq5xyrnY1l2Y6KJwAOQaEPlTf8p1popuznbU3vVLx6kz/Photo%20from%20Library.jpeg)

We have, from front to back, 3, 4, SVM

Front

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/B79F5F3B-F284-4922-94B9-F3111AB7E649_2/HxpyZud554qhP8r7Qr92mhVpLl7NwRo6yxaye0fM61oz/Photo%20from%20Library.jpeg)

3.5 front, 2.7 back

Load and unload at 21 ipm

We are now ramping

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/7836635D-3206-4D4C-B187-5DB50EDEE2B0_2/ieyn6gMinAgfCpJCk1EL2XAf0L9kIgnthuGencD5xosz/Photo%20from%20Library.jpeg)

If the step does not move forward, do hold step run

I stopped the anneal 20 mins early, stepped, and let it cool overnight

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/7DFB1A97-D529-4B91-B3B5-FDDA0AC631E3_2/3LNFb6ZxeexTiyZQi3lSuBkR29c3nSNkwkGAXJIpUbEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/B632F18A-F008-4A6E-B13F-1E346B11DAD1_2/nPO1xDalL8bfZENt51THXJVA0bMrHsD6eVlhA5FYzo4z/Photo%20from%20Library.jpeg)

After cooling over night

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/E6B6FC09-FC76-49EF-94E1-D87316DDB7C1_2/wPdf9NtmxB6avjyj8zqc0zg6tRtx9LVbYrwyy5Q0JE8z/Photo%20from%20Library.jpeg)

We now unload

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/F4EF5830-51D0-455C-84D5-1BD1A53CD0E9_2/NoFioyixMAQmFxMV8s4mIZyrYjxGSR8xqmvAQXz87w4z/Photo%20from%20Library.jpeg)

No obvious and visable signs of cracking, which is good

### 1100 C preliminary lost test

We use 1550 laser (not santec) no edfa and 10 x objective. So we will not have a tonne of power. 7.5 mW in

SRN 3

Straight 1

66 uW

Straight 2

95 uW

Straight 3

91 uW

Straight 4

72.4 uW

Long square 

55 uW 

Long circle

50 uW

Medium circle

53.5 uW

Medium square

33 uW

Let’s try one more die, as the data above is a bit strange

If we compare straight to long square

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/2BC6C47D-49A9-417F-87C2-FA98BE6DE6CD_2/cTSl5zkL3pmdNKC5VoylKmOZ5453KYKUwpXs46Bddcsz/Image.png)

If we compare straight to long circle

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/942D3534-8323-46C2-993B-67BC32C71B2C_2/hyUSSshGvAFQ4rKbQTVrP8ETxDYiX8AEx1xiK7dXcs0z/Image.png)

Straight to medium circle

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/1F41A6E7-6D16-4FE0-B2F8-5F7B281CED5B_2/kBNUraGpmwgCEhvRNVRxl1yuGRkx30vRUzt4lVvxoMwz/Image.png)

Straight to medium square

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/BEA176C3-0002-405F-AAC7-AE59AC4331C9_2/EsDbGZ3EtZFYdcDd5ywoBmgi2exSMGx3dQhl7VtRjCsz/Image.png)

I would say a loss probably below 0.5 dB/cm from the average above.  



Die 2

Medium square

38 uW

Medium circle

42 uW

Straight 1

82 uW

Straight 2

100 uW

Straight 3

85 uW

Straight 4

94 uW

Long square

36 uW

Long circle

55 uW

Not fully consistent, but maybe a bit better 



Comparing straight to small circle to long square.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/CE839272-D17D-453D-9A24-00167DF64636_2/Wo6o2hyGmYKDrftX48oGOxDSPFJWiLp42HQcFjiBTKMz/Image.png)

0.5 feels like a good estimate still



Die 3

Long circle

26 uW 

Long square

22 uW

Straight 1

40.5 uW

Straight 2

105 uW

Straight 3

75 uW 

Straight 4

100 uW ignore the upper lower values. The power meter was mounted in correctly 

Medium circle

105 uW

Medium square

45 uW

These numbers are very much all over the place, but generally indicate very low loss



SVM

Straight 1

8 uW

Straight 2

6.5 uW

Straight 3

8 uW

I can’t find any more, but we know that it is possible to get light through



SRN 3.5 

Straight 1

44 uW

Straight 2

63 uW

Straight 3

65 uW

Straight 4

60 uW

Spiral 1

12 uW

Spiral 2

12 uW

Spiral 3

11 uW

Spiral 4

0.7 uW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/E4A73334-2077-4950-97FF-CEC97FC3F260/06722966-BB73-40D1-A065-309EA82DA451_2/A27jj57OZ8zmv9PKYFjyxCXnb3MjwoQjXcKy2Sw0gL0z/Image.png)

It effectively seems that SRN3.5 has its loss go slightly up from annealing.  Either way, SRN3 is the best 

SRN 2.7

Can’t find anything



SRN 4

Can’t find anything

