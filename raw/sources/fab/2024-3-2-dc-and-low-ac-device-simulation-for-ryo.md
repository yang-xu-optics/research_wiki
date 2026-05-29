---
type: craft-export
title: "2024-3-2 dc and low ac device simulation for ryo"
craft_document_id: 1828F793-9300-41B2-BAB7-5583A2C10A8B
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-3-2 dc and low ac device simulation for ryo
The purpose of this note/simulation is to documnet my work on Ansys simulations investigating the ideal DC device (bascially, does our field contrast reduce as we have better conductivity, and to investigate Ryo’s device and to see the index contrast he achieves..  This will hopefully help us get a better intution for how our devices work.

The inital values I am using for a flat SRN device for Ryo are:

SRN_bright: eps = 8, cond = 1e-7

SRN_dark: eps = 8, cond = 1e-10

oxide: eps = 4, cond = 1e-12

Ta2O5: eps = 27, cond = 1e-12

Cr as high voltage and Si as ground, but choice really does not matter anyway.

Note Si substrate was cond = 0, but should not matter because it is ground.  Below is what I see

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/9D963A47-A0BA-47E4-8072-9FB0A3807C19_2/RtTKdNZJnhUwuZ2JYMPjSxVS1pJyndP0PYPOyuFH6bwz/Image.png)

Above is full device, but this is clearly useless as we can’t see into the core.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/87FF1322-2F97-4D88-8DB7-3F26691A55D5_2/wzUkGd7z7NURggrAcxLL9RQxaqfYP7xuKiacsyqOCcUz/Image.png)

Above is freq = 0 (DC)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/98637995-228E-49F5-B5DF-FC46798BC36C_2/3yFllSFkyATxR80xRW4bNI4KDD2XQk76fLyn44pB6xMz/Image.png)

Above is freq = 2.  So we get better magnitude of contrast here, though the high contrast regions have shrunck a bit.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/AC4CE952-7B2F-4808-84D2-280049BC848F_2/xrT8oxyz4ZWlxfHaQkaOwl0PQVC8YU3cDqNHGHClilsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/D9B5C0E4-BEF7-4707-B524-D28D953D24D4_2/NNyvIEQHSKzUVcc7C1SEy63Bw40eA0WWXxpW1DJP54Mz/Image.png)

The files are saved as Pos1_Ryo, where pos is top, bottom, or middle.  Bascially, we have not observed any saturating effect yet. My best guess is that the conducitvty of dark state SRN is too high.  Lets make it closer to 5e-12.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/5E3B7B13-AAB2-4588-8929-EED61702D45D_2/ePxkABx36xRDQyd2vtFc99l2xxeOXfHrFZJuRTzKSl8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/5C0081A2-59F5-44DF-B55F-93BF894AE034_2/qczoMG90h1aZhPsTRS3un0m59iJ3KyhXTeAbEQCnTVcz/Image.png)

So, evidently, that was too low (it bascially behaves like DC).  On the bright side, this already shows DC devices are useful even without etching.  We don’t see any cut-off effect.  We should restrict ourselves to 0-4 hertz with 0.2 intervals.  Lets try 1e-11 next for dark.  Above data is 2

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/03D3B667-3F13-42C3-BBCC-33EB4BD688A4_2/L3lea71hk9KDy6zu0Ak36Mv7ulbxMyixrfEoE65zSnAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/5EB523B5-AEA2-47F2-89CF-DD795955D654_2/BSsxMoEDWNSTTdZo2EZITCi7HXG2oaZWqEp5u8umeksz/Image.png)

We are very close.  If we zoom in a bit on the frequecny graph (Exclude the first few points) we get

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/681C4C5F-2413-4CF5-82E2-4AD2398192AF_2/gpwcu3k0L8gGBzdTCKNprmTulTBccQSO5MbxVNQnQwsz/Image.png)

So zooming in, we can see that there is a prefered freuqency.  This data is 3

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/BBCEE072-CCAA-42DB-81ED-2E3E14CE3D53_2/um5UrGbaaF8UOiXNUf9NkJqwvBWVmSmqzmuS14trSuwz/Image.png)

Above is what Ryo observed.  So we are not quite in the right range, as he used miliihertz.  So we really want something closer to DC to make this all work.  I think dark state and core/clad conductivity matter the most.  I am going to redo data 2 with cond = 5e-12 and see if that gives us a small hump.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/E43A27C5-B97D-4EA3-9D31-E44FD94D9EF1_2/8wmWJ8gG2mcDVYKe3bWfB5RGbayd6VTwKXcsvAxWp5cz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/36C99AA2-B3B4-4E9C-9E53-BB562C1C3431_2/Qr0U5VywEVhsQWjyo71bTH36iIuQBfC8apQCfnJm9VMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/1DA38E8C-8378-424D-BE14-9FDED765B5CD_2/5d4P1OXG6xyg2ASwWLgNyyFSrUmQQ29dyp4clzxqrS0z/Image.png)

So we still see this rounding effect, though obvously at a lower frequecny.  What we do not see, however, is the decaying off as much.  The plot is not going down a lot.  This does not feel a lot like our first 5e-12 simulation, so lets try with a greater frequecny range and check stuff.  What is super interesting is DC just does not have a continuous behavior.  So smaller frequecny does not really converge to DC solution is this is to be trusted.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/FF09A489-F1F5-40A8-9210-CF133133696F_2/jIa6aOmDbMUlkrNdUcKaASOywGFZgRPpGOJSGmYtoMMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/4903738C-D3F1-4288-90A7-7748F4562257_2/StuWivqh2xaM1yyigZVhQlNI8asBOfUTLCj0S0y13Zoz/Image.png)

Zoomed in



![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/4164E9C1-9FAB-47DA-8706-677EC5864E13_2/g1cixiPYzCtG1IbQYIEruwinBKCGFMOi9mkStkmXm3Yz/Image.png)

The hump is in the same spot and we qualitiatively agree with before (both the first time will did the simulation and hump placement).  So this fifth simulation confirms the results from 2 and 4.  I am still really nervous about the DC solution, just because it looks so discontinuous.  While I could try to get something higher resolution there, I am not sure it is worth it yet. To confirm Ryo’s results of a peak of about 1/10 of what we have in frequnecy (about 15 mHz), we probably just decrease all of our conductivities by a factor of 10.  Lets give that a quick try.

I reduced SRN_bright, oxide, Ta, and SRN_Dark all by 1/10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/EA1FD3A2-5270-4AB4-9418-C5F14715C942_2/RbtdPjd1gigfKjnhzRNK2o2GNCGx0yx5WfPEd2NQSx0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/F845CA47-97DA-40AC-8611-F9E6CCB40BCB_2/emPjSXp4S4wZaLcGUuqDep4d78w4bruSMpEtS5bCcVsz/Image.png)

Zoomed

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/05A7A7D7-5F4E-4C34-95C1-20DE76726EE3_2/3siyAxPy1cTyW0iLvkyICBx1Vs60aVXFtNeRfAJaEKwz/Image.png)

So ya, under 0.1, which is in the range we are looking for.  We should have run higher resolution here.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/4BAD595A-CD82-43B7-81B7-64D9E8BA719F_2/3vBZJyjEwSQ710PJvSoAHQ0WpM3IwKzJ2oG0uTPs9tEz/Image.png)

Also, the blue line aboe is 60hz.  Evidently, not much contrast.  We will do one more simultion with much better resolution to try to find this frequency.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/281E8ED4-DAFC-4CF6-897B-36FBC2FCBEEA_2/0ve8GlnZNEMGnM4m96da8YX6YpaDXwbabe2qwwAhWQQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/151073F6-0E6F-4451-8CB3-67823EAFA87D_2/dynyKxLktcjd5c3jXnKZvxqSYdHyBZy3gzHyN2gs7eIz/Image.png)

Above is zoomed in.  So the peak is between 50 and 100 mHz.  So maybe hack another factor of 10 off conductivity, but we bascially get the ideal.  Ta is super insulating if it is dominating the resistivity of the waveguide (which it should be because LN does not observe this effect).

I reduced SRN_bright, oxide, Ta, and SRN_Dark all by 1/10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/96D37183-90ED-40F4-A6F5-5D546502FC33_2/WxJSwj3GZzEjvS0xVcKwRVxeZHqHKe999qfm6c7fvBgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/9EE1C578-D6E0-4895-A913-5EA6987FF809_2/xXPEMGyk5eDQxeLk1e3AKto2Ayq6pIbMWZ58Xn8M2RQz/Image.png)

Ok, so we definatley have found a way to get the ideal frequency into the correct range.  It is a tad small, but we can adust our conductivities up a bit to deal with this.  Now lets see if we can use the values Ryo found for conductivity.  Above is 8.  Below, for 9, I am going to use:

Ta: 5e-14 (8 uses 1e-14)

oxide: 5e-14 (8 uses 1e-14)

SRN_bright: 1e-7

SRN_dark: 1e-10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/D7F3CB5D-0F1E-4E7C-A6EE-81675954455B_2/76ZdBxoxxrxy4ZVuCbywY4dPiTXpYKQ9JEs9IWyCrYcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/A46A941B-76C7-40DF-9BBD-8B186CEB653B_2/zQffx2yhxTdZpvRfmKvr8dLxBtzWlMWUdbiGEdU9Iswz/Image.png)

So, evidently, we have not hit the right frequency yet.  It seems like something is off in Ryo’s measurements.  Let me quickly try to get the oxide and Ta much closer to SRN.  Here is what I plan on using

Ta: 8e-11

oxide: 8e-11

SRN_bright: 1e-7

SRN_dark: 1e-10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/925D973F-CB87-42AE-AB26-F13B5887E7D5_2/eT9PsKPuf80CF9N6wOiOOQuUnYuQlyEhVkkqhx670Qcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/8FCE155D-5BB7-4F6B-93ED-00448EE8865B_2/kSrnHynzNTGuKmVUD8zh2S2uH9DwYeqbMLWHZO5p6tgz/Image.png)

This is really cool!  So it really seems that, if we get near DC, the conductivty does not matter much.  The above curve is not even zoomed in.  So we are really close!  Lets quickly make the oxide conductivity a factor of 10 lower (to 8e-12) and see if that effects this frequency.  The above device is 10.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/BCE2DC92-D026-446A-8143-A32BEA44972B_2/xHFjkkrqEBD3hSICAtacfqw54fH6sqX1Cg41ovNr5DUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/608CD103-0732-4BC0-B2D6-5AF8AB1952A8_2/UILBRWCy0bhAeRa09T1KqOTX4MKf14nyycJwlZ37AzYz/Image.png)

So it bascially seems like lower oxide conductivity causes the corner frequency to move.  So we don’t want lower oxide conductivity.  So it really seems like the device is 10 is the best!

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/CCE6A331-C3A5-42DE-87FD-3C3AD971084E_2/xWVacnnzPCVw3vYA2J59KpwcbtFndoyvNkPlDNLYVzgz/Image.png)

The above graph shows device 10 with square field.  So it might be possible that there is a bit more contrast then I am showing.  The next device will be:

Ta: 2e-11

oxide: 2e-11

SRN_bright: 1e-7

SRN_dark: 1e-10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/25CDCCCA-36A5-4443-BE94-D4EB8514029C_2/yxvYEOgU6L0JUOvalGtiA0YlNrmHVa1x2m28li24Lz0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/D83493B1-6A81-41C1-9DFF-31A35C046137_2/SJQvtuTYTj2XqpLKVVMHPO0wI6MUjDlnKxjISN8xhsMz/Image.png)

So this still did not quite move the corner frequncy.  Maybe I need some asymmetry between oxide and (based on result 11).  For now, I am going to leave this here and design an etched device.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/E7DB1BBB-7B79-40B8-A3BA-EEF846BC614B_2/B8JWMjEkEUqXFriSrQyYc00pprBW4DSBRkmKYAd6WOAz/Image.png)

Above is the chi2 (not chi3) graph for device 12.  One of the key trends we notice is that DC devices have a higher mangitude of field in the guiding layer, even if that field might have slightly less absolute value of contrast.

Below’s images are for etched structures, like the image shows

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/9E58262E-11E2-4FDB-9796-52EE5998FE6E_2/5AZpEfOwMJHes19YbfqgIT2llUAztwSrkczV8kFPYygz/Image.png)

The width of the towers is p_etch (presently 4) and the period of each structure (which the above showing 2 period) is 6.  Below is what I see using the same values as I did in 12.

![Screenshot 2024-03-03 at 2.41.09 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/13E92C31-847A-4513-8AF8-1AD68DBC538E_2/kFepQW2dGDBhmFS71rEmDvMvXretkpC3yhPbJHz14Q0z/Screenshot%202024-03-03%20at%202.41.09PM.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/1828F793-9300-41B2-BAB7-5583A2C10A8B/2398CBE9-62EC-45C1-8726-8D7B16804C34_2/vzAV2gRfoL3zQENbYgsNOf3IDpycrZLnKlEY7HRdkZ4z/Image.png)

This file is save as 1_Etched.  What is suprising here is that etching does not give us any better contrast than the normal flat SRN structure.  And this is with smaller features than Ryo is working with.  So this makes me pretty convinces that they will not be helpful for Ryo.  This, on its own, is a pretty cool find.  It also makes me susepct our field contrast was already saturated with the period of 6 with the flat electrod (and a bright width of 2um).  