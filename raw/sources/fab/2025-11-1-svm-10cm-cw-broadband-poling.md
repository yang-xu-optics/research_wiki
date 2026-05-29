---
type: craft-export
title: "2025-11-1 svm 10cm cw broadband poling"
craft_document_id: A47F76C5-1651-43FE-8F1E-955DBA0FDC6B
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2025-11-1 svm 10cm cw broadband poling
While the SRN3 waveguides showed nice broadband poling, there is some hope that SVM will show higher baseline conversion efficiency at the cost of higher loss.  So even though some of the shorter wavelengths may work worse, my hope is that we can demonstrate that higher Si-content can get higher raw numbers at certain wavelengths.  I already fabricated a SVM device with 12um of SRN8, so if any device can do it, it is this one.  It should also have a higher breakdown voltage.  So I think we can take it up to 12 Vpp at least.  We are going to follow the exact same alignment proceedure as before, and we will still try a broadband section.  Who knows, perhaps the higher slope efficiency will compensate for higher loss and make this overall better.

## Alignment

We start by coupling 10X filtered EMLO light into square spiral.  We use peak illumination power.  This is not a perfect apples to apples comparison, but so be it.  We see 2.5 mW out with asphere, which is roughly 2x less then before.

Initial vertical sweep

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E7EFFD9B-252B-4708-8226-61D55ACB5D89_2/y1gAVCyBkhyLwe6Fbrh7bihzSIVHVbhfyDzftSFhfGoz/Image.png)

After first certical alignment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/0AB3F75F-F839-45D0-83A2-C3AEFB0BD6D6_2/NtyGsxMRg8au6bAmGxyp1KD510NxVG9LqFOq2Fp7eKoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/B3470B4F-2E35-40FF-8F02-75F2770F8D4C_2/1cWiUHNLZMDRMZKHnSOUTy5UbaxrcLqjF9YntyMJddkz/Image.png)

These are a bit high.  I am going to reduce the voltage to 0.4 Vpp.  There has always been a bit of an asymettry between hertizal and horizontal.  Perhaps it is hgiher now because of loss

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/EDF3C8D8-21FB-40B3-A0A8-197A28CA3729_2/J0fzOl9CsgsmcPsysbCaoxuZv3Mtfsx9UtazbB1t2gQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D4685A59-DEE3-4CE5-83B6-42174C548C2E_2/3f8sUhkp9ernsKNlM01zNaSzNYYLBCyNZkaLz4fVlCMz/Image.png)

There is still this funny focal aberation too.  I don’t know why the peaks are so wide, but perhaps there is soemthing to be said that, having more background SHG and low voltage, it causes this to be wider.

Now lets move to the main spiral (5um).  We see 1mW out with 10x filter and asphere.  Closer to (but still less then), before.  A lot of this comes down to how nice the facets are too.

We see a lot of background SHG, so I am going to use 5V bias. This makes our background the same as before (and prevents too much saturation).  Now we want to align with the ciruclar spiral.  We should probably run a quick poling scan just to get an idea of what the best poling period is so we can align the illumination.  I suspect, because of loss, this one will be a bit more biased to the top.  I feel like a hand-alignment might also be fine.

After first pulse alignment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/57062465-C54C-4E76-B2EC-C568A9A19D1C_2/FqWb9dzoPrnlk5HPSjYG7WRU87dGoxYoMZqxWI0fatIz/Image.png)

Focus aberations are probably more of a camera thing.  We run the same range as before, so we can compare how much aberation there is.  Results of first scan are below.  We are seeing impressively higher conversion efficiencies right now, so I am hopefully (cautious, but hopeful). Top and bottom seem a bit off

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/31EFCDA5-F42D-45C4-B28F-D1195A29B851_2/PUxxyaCyRHCYxdoxNaJPnwPLAkaxAwGwBEEB4cdXeSMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/CFB5B424-7C9B-402F-A6A2-5E6F5F7CE675_2/mDsAPgB3xukTsg6mPzw8WDyEZ3DqduxNxBkCONTKZWgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/F9852224-DF99-4F6B-82DC-5010BCF63BD8_2/gdVC2hOr7Zc4rbJnf5yM0lpU7mUuEaAIDPmnv3QTrhkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/DC6CD964-A907-4A66-A7F0-E116D2FDDC5F_2/yACnkugA5QVdbGKF1wvwRNTb0RLMxgm3txPeoHKlXGwz/Image.png)

An impressive amount of signall, but we can do better.  I think the horizontal and vertical position of the illumination is a bit off.  There is also just a chance that, unfort, do do have some focal aberation near the bottom.  Lets try to better align the horizontal in code and twist the imaging light a bit.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/BF54D6B1-128E-41A3-9A90-E5B9BB2CADA8_2/mrtV9PbXlIyOcXapBxx7QuScEtLJR0ImqR0Dj1D1hsQz/Image.png)

For some reason, I still feel like we are clipping the bottom.

I think the big mirror was a bit off

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/FDA693FA-EB51-49A3-B252-4A537E4C36A0_2/iAMy3STS8kZR5lUAopeJfU0NHkhtypU1JG4Ze6T7ET8z/Image.png)

After

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D4C19B08-9BCA-4D59-A30E-51603E71341B_2/JVudtwbzukdWb0OSKEKIRBApiSQycuIxPKa2rlpVd6Qz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/1F0A51F1-A5A8-4E56-AE9F-79A86588D8C2_2/loDcVWExkGJT391azv9csyIgu06tLgKxWvwaRN9saOwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/174419DA-F032-4DCA-A2A7-B788A93E7104_2/ZGy9VO3MTMKBobN706pEzQEg65qhRNW5KX6iJuYrvWMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E43E4710-621A-4C41-8367-A4CBCDB38CD0_2/qA5YwizbWPI9WsvMdj9ytW5u49fj8wub1XeQ2DMdD7cz/Image.png)

Bottom region still sucks, but we see less poling dispersion.  I say we go with this, and we can correct later.  As for wavelengths, lets start with the longest and work down.  We will only use just santec for everything.  So 1630 is where we start. 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/6d96196a-4b60-cd55-37ea-8993ba630570/q5sMoxZG0hoBfiMYAEjgbXRye2aD1cfnxlwOOCtnQREz/Image.png)

The above alignment still is not great.  I wanna shift spiral along the x=y axis

## 1630

Course alignment.  We do all optimizaiton at 9 Vpp.  Afterall, if it can’t handle this (with thicker SRN), what is even the point.  It is neat that even in these waveguides, there is a bit of background SHG

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/5C82CA99-A1C0-4D87-BE4E-45A27EE5CD19_2/ZQELqNeYjc4FnSpVeVAEiz5Wep7Fr4hvAVNBKaik8Kwz/Image.png)

We shifted spiral again very slighly, below is our alignment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/38012BE5-087B-44FA-8053-89ECFD7FBDB2_2/2saPulylDeiChbXJ48xSf56rIf1yCxcZ2THqUJvuq14z/Image.png)

We use pp_temp = 15.1, and now we just run long man scan. This 1630 data was taken with 16 averaging for the most part (my bad), so the interference curves might look a bit funny

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/08710500-221C-4F24-AA59-9FDD1CAD609C_2/nB5luQTGyb2Nifa1RMK43reCIOEpIqeYhLsERnfsd88z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/AC0E4319-7783-4373-BA80-2595E6655BDF_2/aDVXobpy98RsdperxruLdAndxg0WSQkTPrl2wAVxQ3sz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E6D9B4EB-A5FA-4952-97C0-EF8E43D27067_2/4EMGVAZbPi7tycd4FPyozBtdQ7kJKeOE3cvTHAgwCFUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/A898709B-9F5D-401E-911B-3D4A4360606C_2/Tx1HVnHFpAlQKnJE3s9ILHPjhNVyFlh7SQxtsWkyycgz/Image.png)

I still need to realign the optics, and because averaging was bad, I suspect that the perturbative will help.  We also need the up the voltage.  So I am optimistic this is higher than before, but how much higher, I am not sure.  The ending points were with higher averaging, so it might be worth it is to do a second pass man scan, as I suspect some of these are not at their needed average

After perturbations

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/69ED349D-FB29-43F8-B4B7-0646DC110D4F_2/BJdplyaywvSGsQGK6OuEygoqK16tgTDOmdu2wyjM4Wwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/F2CA7FF2-AB8C-4A18-92ED-7A82963C83CE_2/btQWncFOsmiP5yfQOPdboVHRmyuFVCxslJ9SO5VYWK8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/501DD729-5A2F-43EA-9C8B-F3B73C164E0A_2/DEImy4ySWRuapv7dvbEqQODuWtuPMsYBYcZ9XxBCerkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/26C3F34D-E5AE-49FF-B295-76CAC4AA5DDC_2/UIyCUF1qKfUqDD5yyqnAumEJzN41qT1PoCi9wBiRut4z/Image.png)

For some reason, I still think the origonal man scan is bad.  I realigned the optics, so I feel like we should be close to the ideal point there.  Lets try one more man scan and see if it gets better.  For reference, we saw about 0.2 in the past.  So I still think higher voltage can get us there, but we are not showing demoninatingly better performance right now (as I really expected a factor of 2-3 better than this).

I think in the future, a problem I notice is the course scan sometimes leads more astray.  I think it would be better to just add a bit more resolution and range to the phase-pp scans.  At least, in our current system, if the ideal point is near the edge, one would figure that the perturbation scans would correct for that more easily than being far away (Where the loss landscape is more challenging to traverse)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/20014198-1951-4A26-8D52-6F806B953FA9_2/HZVYWDVM2BSwRqfgnFOymvAv0z3xCxMkR1l8F9s55SUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/1069D954-B986-4F35-8A58-8CF720CB1DCE_2/ryjjlAQFlyblse9YFn5feinlvW1QgkCY005ZL8nv5mQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D3132E98-73F8-4395-BD4F-CD98CA854817_2/aEqKB7cBprbyT8kvrTbdlKnpi4BgTld4qtntNykyWl8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/54997993-283F-42FE-A08A-02A51A8BA7FB_2/OU06MOaRZ3AmaVTth7pUZQYDUsL9pghsWEbg3cSvlzIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/89D5235A-2270-428D-A8F2-48C9176D4537_2/YF1qM0bx6xj2y1bNl5mXcb7uJoUbTx8xXxYhTdEFFxwz/Image.png)

The above image basically says, during optimization, it seems a few opints were found to be slightly off.  Perturbative is not really working, so we are going to use above chat to sorta predict where we could squeeze a bit more out of.

We now increase voltage to 12 V and get ready for final data.  Surprisingly, as we played around with things, we found 10V and 6Hz to be best.  Applying higher voltage actually hurt the system, and higher frequency could not account for it.  I suspect something interesting happens in the photoconductor. I was at least able to do a bit of realignment.  I see 17 mW out of laser and 1 mW out of waveguide

Forward Pass

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/CDD3447E-EAA1-4CC5-9986-C8603CD448C7_2/SHQOd6l3qzVlPBr86wx9PKBA9XTK9p26y2cdsF4esKwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/C469C4B6-8334-4045-A44B-6A28B4841AE2_2/DC9cFgWzx6iNu6XIfE5qqfwQ1z467uFEux7qaOzg6Tkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/7160A1E7-2960-4425-9688-392871A7B6F2_2/1NXY1uu04ek8dWyurOXxCEyBWyKOQGvaCYE5fIEpdh0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/571D9608-DC32-4CB5-AF42-A901127A4364_2/8iKu2nAxQIW54xyKKHVVDBaxLvGrNeeHJZZv93Tu2Q8z/Image.png)

Backward Pass:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/A304A9F6-84A7-4A08-A576-1F1007EF519B_2/q3hMlEKRWnqYWexkvegnilwcqgwYe8u5WW6pFRFjfuEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/04BEC593-F90C-4225-9B7C-6F7BEEECB437_2/jrPF3pQhUIQNGKmzI7iKKe3o4GGNSyiyM1q42nYbYIwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/142AA15C-A725-4681-9CC7-137D73A69216_2/3iyZqM2RENiKncEsttwuG4qQSTlD9WYkyJZGRvckAUYz/Image.png)

Perhaps I overcompensated a bit with a loss guess of 0.55 dB/cm.  As this predicted more power in my waveguides than before.  While that is possible (as coupling efficiencies can change), I am personally a bit doubtful.  Better loss numbers would help tremendously.  This higher voltage effect is also kinda of annoying, as it really is make it more challenging for us to push numbers higher.  I will have to measure 1D waveguides on this chip to confirm things a bit.  I will also be curious to see how much background PGE we have.

Transfer Function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/C65C59F1-1DE7-4F2B-AA59-6AA8546851A0_2/H4kZWy3gUQWETtzCv9bhxob7yz377WIOyaxXAWRwyf8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/0F94673F-6F0C-44B0-A7EC-B9C6EDB82FE9_2/37IAHg9sZuBDrY9K1lhD7ss7uiWegLcZm6A9b0HzKkwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/83F57F12-0B9D-4796-8F7F-0F11C2976354_2/tj05KSwYOqkcZdSw5I4FyMQ2CFYwbGOK84UTGKWjPYUz/Image.png)

After releasing power, we saw 1.4 mW out with 17 mW in. Perhaps loss is just lower.  Below is updated version assuming loss = 0.4 (same as before), with 1.4 mW in.  In the above, I used loss = 0.55 with 1 mW in.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/515CA9E2-A37E-4B66-9FE1-65956F24C7C0_2/oeVAXfmsvMO8CNl98yyVrjcMO4is0jz4hcQS6ZYJ1Ngz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E55580E9-32EC-4E76-87A1-389EA758EEE1_2/wLYffTDu6lB5OKeyIDUCyqxw3RuGLqnnQJzDbKnkN9Yz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/8E320953-0D1A-4D34-98CB-4AC0A0E9F82A_2/BynXxuCwy87nX1K7bhpNzxDXFo4sOHM0sIlZqGPMn2Uz/Image.png)

Suprisingly little difference. Lets move on.

## 1610

We will be doing all measurements, from now on, at 10 Vpp with 6 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/7834F899-7B94-4FC8-9C21-79847F59C433_2/DG3BhLuOvaKtyDoaX9IhETuTSG86HDHkwJS2yYtF6UQz/Image.png)

After manscan

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/9ED5A229-0BAD-44D6-9FF1-5D62238E3FE8_2/H4yhFJSgwXzV96NUziPdFLU3xxFEUtmTxfNgM4tz1Ngz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/89CFFAFC-48B2-49F9-9B4F-69A60FE9CC4F_2/NtwMpwj0FULTaF3FhBVBmXYklmuTv5NuanL8KaJ7UnMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D94281B8-DCC0-4CB4-A7F9-73E4917C9B29_2/0pLt41xDQ2MwX6WkGmUMqVdXvMkDDixCns63urPVPGUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/4218C4AB-E653-4198-9DE9-6A2039EA2B96_2/yuV3ogEebGsgRNM0VGMmgV2HLany6b7CrTllFxkt1fwz/Image.png)

Interesting how the end part looks.  I can almost feel some multimodeness in the middle.  I did an error correct that only made things a bit worse (unfort), but we will do a manual realignment and then proceed with final data.  Pert did not help

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/67BE422A-A886-460A-B008-501153D5608C_2/8hxyEpSDXNambcG5WyZf0MUaMtTYbed1G4yMYCynhgAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D0597084-0EDF-4FC1-9B19-C1A58C433342_2/RMi2Lnya6dSfNduFaSOYC2ADbiVlTKYztzbWpsvi8xkz/Image.png)

Slight lower, but whatever.  No manual optimization and final data.  Funny enough, I found that 11.5 Vpp and 6.5 Hz to be best.  I found 1.9 mW out of the waveguide.  These differences in output power compared to the SRN3 waveguide are a bit annoying, as I can’t do an easy apples to apples comparison.  In theory, if everything is normalized, we are only slightly better right now, or we over-estimated the previous waveguides or underestimated the current ones.  A lot of this can simply be how nice the facets are.

Final data. 17.6 mW out of santec. 1.9 out of waveguide

Forward pass

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/22417E21-FE98-4F1D-BCFF-0C0489B39BD5_2/qnwx7CIlSyJuikgIJ5sF1fIfPfw9Q2ppvxsIxkLIwIUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/8CA31121-E274-4B47-A32B-AAC470081841_2/7aYB3ltdYj0pCrxqBD3F9gUoJqUKfvZf9anzaiE1xLIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D263D961-CC17-4DD8-8E7F-22BFF8E4844A_2/rnlPwT5KZZRcby3HjRxbyLgpzHYUeTz42yLQITW8Elgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E421282A-E4BC-44F2-B1D9-D05BAF1F9FEF_2/IgH8oetUjxZGymkkEkMgOxTFKpsw1NGY2x3xVYi4NGoz/Image.png)

Backward

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/75ADC145-3994-488E-89FF-01AA15410E58_2/dd7qabkHkrfZmyyXW3vr2MEysvQRsVH2yQAZqzxuaUIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/737460CB-456D-4DBF-B3C4-54BF775E4294_2/liz4HTVTJ9lNBnuyAvc0Ub0AEwUManKLOBM9rj5HeOYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/0AEA3087-2BDF-4ACB-8DF9-A94B6FDEB35B_2/7uSlAIat3q9Hpl2eyEjhWJRAPjcjnkMIeVBsMUy0xiMz/Image.png)

From the scalings above, it is quite clear that fundamental loss is still a much bigger issue then SH loss

Transfer function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/071451C7-4BCC-4897-B640-730634701A6E_2/xUzQSTEogzKi1FVUTsWVk8EDsccVi7YACORPCfbYxqYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/37E789C3-8595-4457-8FF9-178133ABD14C_2/1d6A6conxTuNG7zkyS4N4Zy78O0xxmE9wlwl6LCuP7Ez/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/A09DA40F-1840-49A9-80B1-8A653C150989_2/KmNRFe3A5iimxtIC2xhJjWBnmxyaheSNNgIn6zIRkC0z/Image.png)

## 1590

We do optimization scans with 10 V adn 6.5 Hz.  We will up the voltage later when we do the final realignment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/63C0D603-6206-42ED-8D09-DC25BEBF45C0_2/odVkyfOqxdUnGTM6kj56Gu6bysmRgxPKzdrhYFcPmG4z/Image.png)

After man scan (we have not seen, up to this point, the perturbative optimizations help, but who knows, they might come through at some point, so we always let them go for a little bit).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/37ED33C0-8F40-4BAD-A72F-B4C4F96FC10B_2/Lc3OyHxhuSV2yjSB2ragA5fZiuvGxS8ryazdVqMSgAQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/ED40DA81-69F1-4931-AF26-F251DD1EA865_2/gNmQS9mfNuWZtyING9laLyfLumvDvznW1R5IDq5laB0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/AE9560F5-C53E-4F59-849A-5C41184C4CDB_2/AqIhoLiTMEvExuWObBQFZy0xRBY5ywjpzd7TYy3zDBUz/Image.png)

Pert scan did not improve anything.  We do slight realignment.  We also notice that interference fringes get a lot weaker as you go through the waveguide, so it is possible the loss is still fairly high.  There is a fair (though unfortunate), argument that we should try some shorter waveguides with thicker SRN8.

We see 1.6 mW out of waveguide.  We see 11.8 V and 6.5 Hz is ideal.  I think this small variance in voltage compared to before is reasonable.  I am still surprised that 1630 required so much less votlage, and it might be worth it to go back there at some point and double check.  It might also be the case that the photoconductor needs to be activated somehow, as we did observe those kind of effects in the past. 

Forward pass:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/DC397612-4B02-4936-8382-23C61E14EAF0_2/IeHjPYpTp3WLJEhit5GLrXnxNU2Klys6I5INCrRQlJEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/4FBE0922-18ED-406A-A179-F4CC29F29EA4_2/yyPxulVMiAR502oxxjXyBAtBsq21NyFyli93yUJTyrsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/7141FF11-3EBF-4D10-A466-DF0D72E6B462_2/Ocyn03oxtyccshOCC3qEcyjyWEap7aNgUVWDq1pMB7gz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/43279079-B11F-4F22-BA40-089A19639C9A_2/dCUnBSGlgTNyQd82I6xBS5Ug5pJrwIRrlV2xjbj78aYz/Image.png)

I really just have to wonder, even on the bad peak, why we are always still out of phase.

Backward pass

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/21A9E76F-0203-4EC4-AEDA-802B6E9170A7_2/vu3aMV2XkWzRTeSyIGTo7jzEjkv7OG0I8KpBvCUgxEEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/F22FF474-134F-434E-91DD-475D3944663F_2/BO41hggWAjMUHpoyHtUJ7yHoqtdPpCJJ1JNBaLNzUa8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/CCD8569C-CC28-472B-A216-0B19806EB24E_2/hW12zJjdTCcQcIW0GZSF5bNvS5BAFLCgHIHwDklk8lwz/Image.png)

Fwiw, when comparing to the results on the straight waveguides, we get ~10x improvements on these devices.  In that sense, they are basically what we expected.  I guess the scaling on SRN3 is just a bit nicer (so added loss and higher conversion efficiency kinda cancel out)

Transfer Function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/A472091E-FE5B-4AC6-9712-4FECEECDF451_2/h1e5E2IyfJN5TlwxB0E9V98mncCN2qdswVvIG988ytEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/DBDDB007-7096-475D-B751-C3D01E401B75_2/z20yYxQHXO1EHmYXxvaDYUAUZklBObNjb7XSwLgz5H8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/BA555836-E316-4352-BB89-4D407FE38E78_2/pcHYXQlwwYcj409INsOXIT2NO6yfpEgByCyO2Yuf6soz/Image.png)

eh, about the same as before.  We can start to see the effect of loss though.  Lets start 1570

## 1570

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D3F3F6EE-6D26-4EEA-B491-BEFC01DA02A3_2/81ayGIRWqRycPyq6TGzy242Ywu97anbulssHYGym6cAz/Image.png)

Now we get man scan going from 14.6 to 15.05

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/612F39E2-4295-445F-ABF7-FF53307CEBB4_2/PJ7t3fjHzgNpWONIbrqZ7ZYrDyvaogE31y8gV1r7lBgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/B409685B-42AB-4A0C-8C64-1D66F2277F07_2/0SZ8mtk0IMlzMjttWxMzZYh4qC2y0xPAysXRxL5iKWgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/834A2158-BC15-45EE-B31B-20A56AB8BF19_2/PLSJ6UKlgn70K6qalusySshvCd0ySQYwgCSrBGYNgV8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/07E9002A-F3FF-483C-BF35-9A3C23143ABD_2/RJ4UTQoeymF4tzWePVWf1ZXrPnuxgTis27UUcOdMlw8z/Image.png)

After Pert 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/F52C71E0-55ED-4AC3-9CDA-8F12A6D5AAC4_2/XJchSuvBUjkVsOQfqW3YcRSyGliupmcxg1UWSHRcgbgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/2D24BA0B-4A3D-462A-ACB8-781C106CA875_2/WZRMMpV7LD9WrujEyYmR65zvEx244MyebF29vleh7uwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E7B776F7-2D7D-4C36-A9B9-99DD4387B13F_2/VyHKiOFyE4cvnldTMe2Oum0VAQl7IVKjsHwyXd2WELEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/ADC22950-962C-4261-B3BA-21F32297D4F8_2/2f0D2UU9lxjXBK8OtvYior72IG9YkAQ9RPKfunW9Logz/Image.png)

Now we do some small realignments and take final data.  I feel like we are starting to see the effect of loss.  As a reminder, all this optimization scan data is taken with 10 Vpp and 6.5 Hz.

For final data, I saw 1.4 mW out.  I used 11.8 Vpp and 6.5 Hz

Forward pass:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/64F32091-4AC1-4ABC-9B6E-E58A0771B25F_2/s9lRFE7ExHvbhrSJKjeBRA0DXeIKelQeKcvttqSLZCQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/15D7CFD4-F156-4705-8873-8DFBC02DC155_2/2QYhOjbMAmBsFtTx2F2mRi1m99psWNBrvp0DejIOt9sz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/05C3CF27-5212-4A05-AC0C-909FED17F4BB_2/TxJLJCedumZakoqu2nP1GMg8HgNEcQneyZO4GB4SsCUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/C2EE4E39-5A61-4167-BB40-998D14FAED5F_2/fpzHqkfQ2NmIuo0PPnZ1PbeY02BOGnhJKyaPWQhioZ8z/Image.png)

Backward pass (same dramatic backward scalling.  I fear this is only going to get worse as we go to shorter wavelengths)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/6AE9D23E-2331-427F-901A-E463C5D28039_2/dJf7jOmEPG5bkrxrRypFqaMYOn1gYVKlvyhMT4AQnioz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/B8F44928-4D11-49AA-B1C8-A71DA4B436DE_2/m4WTQsFnbhBMwcToxDx8JyHfIEM9VGhooFFiwWTLaO4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/5E7BCB6C-3A8E-4239-B6DD-4D32DCE4F8FF_2/5yBYexbZr4d2mQt1yweZQew74Id8WEuXHylmnaZdmbsz/Image.png)

Transfer function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/B3B91BC3-C4F4-46F5-829A-D094A3A06118_2/Gw6GkpwIdR7ZoBfaxhsZx8bDbmun88QlMufjnKkwxtgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/BE20F3C4-DDFB-4126-86E1-A2780AEDA87E_2/S5Bf3EAUAOvzKYN8Jidf0PeyGo0JtT96StMLD2kUWAoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/62CF12D6-78C9-4C7F-B470-BC6AEB91BD76_2/Ba9yoKxE4x0GpN4SnLy1Q2cLsUcRRpr0WHa2Hva64K8z/Image.png)

We kinda get bs too far away.  This is because of loss.  I can see we are heading in lossy territory though, and I think 1570 was right at the edge

## 1550

We only see 260 uW out, so we def notice the loss right now.  Once more, we optimize with 10 Vpp and 6.5 Hz.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/9CCB1688-D06C-4CD4-B393-F415204B8F1F_2/Qhc7lrntKhd08KQZAPpx5XHRm944NLxhPYMG9aRvPAkz/Image.png)

We now do man scan

![Screenshot 2025-11-07 at 12.50.37 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/A4381453-7F33-41C5-96A0-4F4076E063B5_2/O3H1exzwCWZZHOix83gF6iwEb1gWgPQ2xigbnJmM8KIz/Screenshot%202025-11-07%20at%2012.50.37PM.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/EB198065-4228-4710-BCA0-0AA98DDF2AAE_2/3A4P4UjocLFoLX21NVGwXU35kcDcfMK4Zn6nuh2DOpcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/8172544C-9D7B-4D0F-B8AA-B1AC8EBB06C5_2/lNHAp8PdctOfezeODMcH1lRgurcxqgSRvq6osnszjhQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/AA0A0BDB-04D9-4098-9533-15D436D952EF_2/RL9y7OeUIlrqFd2AWhULbz7ppOcq8iyJqjyWtrRYe5gz/Image.png)

This is like insanely bad.  Given that we expect the input signal to be comparable to before, this is some really bad conversion efficiency.  I am going to run more more man-scan, as some of the early points are uniquely bad.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/3AF1097E-5064-41D5-B87D-49AE8D5CE49C_2/cZTnWhw1Eg1nMtgzTkek4yBUURxMOiYkBJfSUmqTGw8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/0B5F228C-7B62-4D5D-BA9C-2CC94DFC2D44_2/PDqkTdeqRn1BXjN7CSyA91TrX5g8yEgUYXNiSy6duN0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/134AF5C5-BE1B-4280-9D57-8C4C9407A7CB_2/TOsljZBrgkChys6Vvp7yz6Syok308dOL0hHMmlBpBGIz/Image.png)

Above is after reoptimization with perturbation.  An interesting note is that we see decent scaling for forward pass.  This almost inciducates we are at a SH resonance.

We see 250 uW out of the waveguide.  I am going to assume a loss of 0.65 dB/cm, but it might be higher. We used 11.5 V

Forward pass

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/C821C7AC-9B3E-4611-94D7-28BDEB51C246_2/m2CJW67SzqyNrXFTfNOxztWVx9rselW4CRF5X0ftoBQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/D9988194-43FA-4930-89B4-936CFD10195B_2/aKxQAsW7lot1JkqagigZKYtgs1PkIwQ9HWyoPQfKSm8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/B502DD20-8585-4AD5-985A-909D51E4EF8E_2/7q2csT0fCDYCyLxDfeWtyFk5DhRlr0WTmK1vH5K19qIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/B578E8A1-AF90-41A3-8D9A-B0F0AE823046_2/qN3mBpxFmP0dIwp2vSbWzG8Rv9KoUV1YCPt9CpRhLBAz/Image.png)

Backward:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/86AD675A-CBE7-4665-97F2-14CD514B0D98_2/Lv4LL2DhOGc0bgnQlukfEyarcy9IsNATRVgoC6v6Hv8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/E92AA081-AF7C-4F47-9383-56CA88893647_2/TSHKUptFnSwxrfGOMHlG3iA2G0AXRuoRZ0lcFWKxxO0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/F81E3D10-24DD-41E9-AB63-642D6CF7FE53_2/2ryy75pxvDzIqjIdaKCW0Qtq0x7vUO8cgUWzeh1DRq8z/Image.png)

Scaling will never stop being weird to me.  I may have underestimated loss, so we really do need a better loss measurement.

Transfer Function

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/502D0F9F-A6D0-4B4B-8442-F665CED5E836_2/Ozgp973VhacycWKuHGsws5RAnUXXYV3pCfT3GYQBPDwz/Image.png)

Waveguide got misaligned as I took power data.  I will need to come back, but it is very clear that taking data at 1530 would be impossible.

I think we should just collect some transmission data (get the loss curves), and call it there.  We can retake the transmission for above later.

## Final Results 1

Scaling

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/69259BDF-6F00-4706-AAEE-69AF720D7C00_2/cXHTxlsa7o7R0tVO8kyfqNu4hwleHfcyg2O6CMjBTC0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/91DB6572-9834-4672-B932-D6F2DA759467_2/7UNhyjwpgnqU6dHDkjbPUy1eFN2W58xEVMPT4cU3fE4z/Image.png)

Really notice the different scaling

Transmission

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/309C05F6-2EA4-465D-A65E-7D6ECAD8A33A_2/4zRJDyj2wCyPMSQB1ZkFvtOkJxulXycxwTLGWgNH2Hwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/2EBD68DE-D4E2-4260-A009-DABE3576A558_2/o8Kf9vTHKXGiESYH6iL82oc8FZSuq8x6KFivNQHgVK8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/A60D0625-21A8-4F3C-BC70-BE55ADB2DD11_2/H9mpTWXMX38I5Q6rLax7zOJNGwxlBSsIRIwKmTxjDBAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/EE234DAF-6EB5-4728-B2C4-269B32B8CB5B_2/GvJbgX8BgG0WlMjb6dA9zPCxQttxOmLDcyZ45yJpgsoz/Image.png)

My loss prediction at 1550 is bs.  We do show more light at the start

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/46535699-27C2-4830-B0ED-CC05F6617F8F_2/gIpr5HSboEkJejSoN8BiG8vHTv9InXcPnHCKGKgbuZsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/3E90070D-2973-4BB3-94A9-11B597D34339_2/iqtdJLjdCwgtz0zO5yG69srfqYFGhqGSmkkZotKxbCMz/Image.png)

Below is full spiral transmission:

![27A93155-226A-4C1D-8C92-EB7F9D463C4A.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/A47F76C5-1651-43FE-8F1E-955DBA0FDC6B/1E1169B8-4982-433E-B491-5DA5B1038398_2/qBCrjo4qDYoONwgRErhwrsWmFqYUND93AKXQ8TXU5m4z/27A93155-226A-4C1D-8C92-EB7F9D463C4A.png)