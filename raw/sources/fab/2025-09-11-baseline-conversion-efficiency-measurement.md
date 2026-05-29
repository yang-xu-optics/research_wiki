---
type: craft-export
title: "2025-09-11 baseline conversion efficiency measurement"
craft_document_id: FEFD8A03-AF84-4D1B-88A4-7B48F5877F16
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-09-11 baseline conversion efficiency measurement
To fully undersrand why our current device has a low conversion efficiency (refering to the 10cm device with 10 um of SRN), I would like to fully test the conversion efficiency on a straight waveguide and then test the loss.  While I don’t know the exact reason why it sucks, below are a few possible reasons:

1. Thicker SRN messed stuff up.  The 7cm device had a thinner (6um instead of 10um) photoconductive layer.  Ryo has characterized this in the past and showed it did not matter, but perhaps something is different with our SRN3 waveguides.
2. SRN3 in this device is a bit different.  We have observed in the past that SRN2.7 sucks and SRN3.5 is a bit worse.  Perhaps the deposition did vary a bit in a way that we could not easily see.  This means a lower Si content, so lower induced chi2.
3. Higher loss.  Perhaps our top oxide is not done currently, or yield is not perfect.  A bit hard for me to say here, but it is a possiblity.

Below are the two notes Ryo took when he was measuring conversion efficiencies

[2025-06-23 CW E-FISH on etched SiN devices.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/9E6BC58E-9FE3-46A5-88A2-7B23DE824C93_2/mtBi7ptEd9oxTqzXMdiJ3rJQDCZb9X2JxDsaSxCdx2kz/2025-06-23%20CW%20E-FISH%20on%20etched%20SiN%20devices.pdf)

[2024-11-23 Data for publication: CW pumped SHG on the polished waveguide .pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/DB8557DD-FCAA-4ECD-98E0-7022EBCDEF73_2/hmuDmvyP771cey1EAHSx24BY0FEfEcEq6xWDIwBGYRUz/2024-11-23%20Data%20for%20publication%20CW%20pumped%20SHG%20on%20the%20polished%20waveguide%20.pdf)

We might have slightly lower conversion efficiency just because we are not using the extra focusing crystal, but I would only expect that to have a factor of 2 difference.  The method he followed is:

- Align EDFA into the waveguide
- Try to get nice sinc function out by aligning the imaging setup.  Also, adjust the AC frequency a bit too.
- Then switch to normal santec and take data there.

After this, we will measure loss on this device.  It would then be good to measure the conversion efficiency and loss of the old 7cm long devices (just on the straight sections) just to sanity check and compare.  It could be the case that we will struggle to get as high conversion efficiencies as Ryo got on SVM devices. 

After first pass optimization, edfa, 10V, 7 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/ECA3E368-380C-43EC-AADB-B4C2790F2D55_2/KlqiMkJCVkUuslyNxyErIDXqPmlAixkaB6Q0sCFApWsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/78ABEAF9-6A31-41D5-9426-BC695F9B4D3D_2/3gnThl22VI9yE2Rp98cT9uufH1J7R3X0SBIGgSi3aYcz/Image.png)

Now with 11V, 8 Hz.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/88E88532-33FD-482F-BF22-7BD8FF211A03_2/OeQ773GApp9EClRLniBxlv8yI5ZjhVeafLNaLmTOUAMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/7FE8A8DD-7FF9-4D28-BDEF-B3A88ACD7508_2/2m5ezYMcsQH3YHTOpbPKocOafHP6uyg1lWYQnF2NQU0z/Image.png)

Lets have one more go at this.  Now 12.5 V, 8 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/8ED5BC97-5164-421E-8F57-851B9D1CD91D_2/UAx0BnPxBfvOlPMJrKUkGXkH59QAbKyFYd6ft3fCuKMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/1930A106-7CAC-47F0-867A-A6FAAB8F3CFE_2/DgiWmxCYbG4dYI2dCFNxtTjSmPrVkwaQwXMkhEgLYYYz/Image.png)

55 mW out of EDFA, 22.5 mW out of waveguide.  Now lets use normal santec.

14 V and 8 Hz.  I did a small realignment.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/DC81EC2C-F5B8-4960-A83F-C46EA02ABA58_2/X3OKRPxzMg6zWnSY7cTPTO8TgUOSAkMXqyBWz1qhCDgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/74E30CF6-6F64-4A4E-A23C-198C996F8A69_2/LL70bdPgCikR4HiSvUqeXfPJGojNj233lZWx0fME0p8z/Image.png)

above used sign.  Lets use sine below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/7CF3E4A5-AD7F-4642-B762-BF7F1A2FB58A_2/Hxu7Gy2nwoFpUTaQyyYPC8PxcmBL9wQvDVt6jfxstbEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/75CBB394-7881-48BA-A1C2-30A00BF91F6F_2/cvOSyrChdjDUrlwspXy4k2B4YieJ46yfRzrfErFu5eEz/Image.png)

The curve is a bit broad.  Either way, the power out of santec is 18.5 mW and out of waveguide is 7.5 mW.  I tried to make things better, but I could not figure it out.  I don’t understand the side lobes.   The trouble is we have more power in our waveguide but see 10X less signal than Ryo saw on SVM.  

Mandar, came, looked, and it really seems that we can’t make this a tonne better.  We are off fromt he previous baseline by a factor of 10 for 2X more signal.  This is not ideal.  

Lets test loss on this chip.  After that, we will test the 7cm chip and then the SVM chip Ryo used.  My worry with these devices (specifically the SRn3 devices) is the material is just intrinsically a bit worse.

We use noraml santec and 10 output objective at 1570.  

Straight 1:

2 mW (I came back and did this one at the end, and got 1.8).  Some of the ones below are deflated because the power meter was not setup correctly.  So I would ignore the last two.

Straight 2:

1.4 mW

Starght 3:

1.4 mW

Straight 4:

1 mW

Straight 5:

1.2 mW

Euler:

1.1 mW

5um Spiral:

0.34 mW

6um Spiral:

0.034 mW

Lets test another die

Euler:

1.05 mW

5um Spiral:

0.3 mW

6um Spiral:

0.2 mW

Lets do one more

6um spiral 

0.42 mW

5um spiral:

0.28 mW

Euler:

1 mW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/352D7749-C111-450D-9BC4-777861ADA82E_2/XKyUQOMqKgHYDZEkntTsV8f0wHIMPfVqFQJnHhGmBIoz/Image.png)

We above is for 6um waveguide.  I suspect 5um waveguide has higher loss

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/9DA6FF5B-1AE7-4376-B941-F0B4D264FDD7_2/u0R08VpN15HKAq1quPlxpcmC5eQaH49xI1YCCvT93iYz/Image.png)

Above is case for 5um.  So ya, I would suspect the loss is 1.5X larger.  This is annoying.  The baseline loss is also a bit larger than expected tbh.  I feel like 0.5 dB/cm is high, though it might just be me.  I would trust the straight (0 → 1, 0 → 2 comparisons more).  

Now lets do the previous 7cm (6um of SRN) waveguides.  This should help us seperate loss and conversion efficiency better (as they are not really coupled here).  We will then do SVM devices.

Now for 7cm device

Die 1

Straight 1

1 mW

Straight 2

1 mW

Straight 3

1 mW

Straight 4

1.1 mW

Euler

1.3 mW

Short spiral

1.2 mW

Long spiral

0.6 mW

Die 2

Long spiral

50 uW

Short circle

1 mW

Euler

0.8 mW

Straight 1

1.3 mW

Straight 2

1.3 mW

Straight 3

1.3 mW

Using waveguie three above, we measure conversion efficiency

With edfa, 8 Vpp, 10 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/92D85587-33DA-49B4-B90A-6B680E870D1C_2/qJ56vgIVGovr7KUFLb87jffxR3z9yHyfctUFKqwydsIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/B66154AA-0ED9-4141-A261-3101D125E448_2/0vIZCA02ZfT8InwRHiQ2PHhm7bTn3qJGckxiNrSbhw0z/Image.png)

Now with 9, which seems to be the reasonable limit.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/00DDFB9D-062F-4C56-80B8-81FA660248EF_2/9K13Y1r3bDyQccybs2t6T5lUGjNFFzwLP9R5ddBGBEwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/072B017A-375B-4E83-AD8C-856D7091CD66_2/KAgMDLxz2wHJSrIkdTrMXhoQky3AQi95H9i3yhqyKCwz/Image.png)

87 mW out of EDFA, 38 mW out of waveguide.  Now for normal santec.

Using normal Santec, 10V, 10 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/4F65DDB6-32C5-4730-8325-BCBA848BFE64_2/vnf2fMUOScQCfBb0HfGtyJ34nMx44zldx3yweB7pnUIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/AC746841-7819-4520-AF89-DF0859199A16_2/PleKjBWcySUEYozEwFlQb1LZphCmvNyxgO1dfyFyDMEz/Image.png)

Device broke down, so that is why the shape is funny.  Another spot is fine, but ya, 10V is about max.  16.6 mW out of EDFA, 6.9 mW out of waveguide.  This is roughly consistent with earlier numbers.  So while this device is better, it is not a tonne better.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/95289E1E-9056-424D-A481-CAB3CD77775D_2/rvXNHGaantAoeTc6lVlpufDmdQCDdibKMRHFKSOc3xgz/Image.png)

Loss was a bit tricky, so I compared one short spiral to one long spiral.  Not a perfect estimate.  The point is the extra SRN did not really help.    Again, the number is a bit sensitive to the loss value, which we could be slighlty off on.  So again, I say this waveguide and the previous are the same!

This result makes me believe that SRN3 is just less nonlinear than SVM (by a decent margin).  The best way to test this is by looking at the conversion efficiency of SVM.  I am going to try a waveguide with 6um of SRN first, and perhaps 10um of SRN (which is what Ryo did) next.  We are going to calculate loss as well.  If the loss is not that much higher than SRN3 and the conversion efficiency is a lot better, then perhaps this is the way to go.  The main down side of SVM is that the bandwidth of the device will be lower.  All tradeoffs I suppose, nature is never that accomidating.  If only we could have just gotten 2um of LPCVD, which I suspect is better than our PECVD SRN.  One possiblity for the future is we should use SRN3.2 or something like that, which will have more Si and potentially better conversion.  Either way, I am still happy we have this in-house approuch, as it will enable broad-band and high Q applications in the future.  

Below is the box I am taking from (I will be testing the 7cm waveguides as the long ones).

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/CC3A4A6B-C439-408A-83D1-308F2E788480_2/V73QpPuwvhnrwSL04sJA6ySe22AVEDtppMymGP63eH4z/Photo%20from%20Library.jpeg)

Die 1:

Short spiral:

0.75 mW

Long spiral:

0.11 mW

Straight 1:

0.85 mW

Staight 2:

This die was just weird

Die 2:

Short spiral

0.85 mW

Long spiral

0.28 mW

Euler

0.7 mW

Straight 1

0.8 mW

Straight 2

0.45 mW

Straight 3

0.45 mW

Die 3

Euler 

0.7 mW

Short circle

0.65 mW

Long circle

0.38 mW

I still can’t get straight to work lol

Die 4

Straight 1

1 mW

Straight 2

0.9 mW

Straight 3

0.95 mW

We use the above for our conversion efficiency test.  It seems that chip broke, so I am going to try a different one. 

Using EDFA, 7.4 V and 11 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/50F09629-E020-4039-944E-3A7B1935D7CC_2/INU2ImLOoyraojEvajdMTsxRughOQfVmbxOn72bu9vUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/B3C17A2D-64BF-4114-BD49-5110F67D9C96_2/432L7Yj7bNkh9fELR4IocxfRdavMJSW93IuOQ1tG75Ez/Image.png)

61 mW out in, and 11 mW 

Now santec, 8V 11 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/A4177548-9A40-464B-BED4-213D8336DEDD_2/rlj045LFLdMYF7gardtfSugcBVJ5ZZVVg0E1uURqGZAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/27BD0D18-A322-408C-AD2A-02AF503BB3BD_2/xU21MftKH2btkF6VddGh3eJ4XZoxypHop4YRaE4gfukz/Image.png)

9 V, 11 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/3F8937EF-478B-4E14-ACCA-E19D03E48FB5_2/H6kot70EPxLHRKxAetv87D5TELpeyzHAJ4y0GrVtIVsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/79080003-56AA-48D3-9EC3-91B250B9808D_2/BEyV2Nzkj34LLxlEMzXykKc0hF7XpKvo2kb7S0j6LmEz/Image.png)

Again, 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/A9FE732B-CA40-445C-97FF-E9FB80B615B0_2/hgDDhgvvMt5tMWFdUUSxACItS6Cn5ZwnpMylphebW7Uz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/2AFC0C1F-F659-4DFF-B64D-BA4D4B5BCE41_2/L6tI2ixeBKKRuEazqjOgh3knidnBLXSKArSCJOCmvi4z/Image.png)

17.7 mW out of santec, 6.6 mW out of waveguide.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/56B5DFAF-9133-44F6-B292-DE9F29B1AF97_2/DZDuxngrqX80dkUaFwUA2Dtm1bf0aS7u0wh4hdHZbswz/Image.png)

Lets now do the 10 um thick SRN waveguides, using the same loss numbers as above.  I feel like these efficiencies are a decent bit lowr than what Ryo obsreved, making me believe something is off.  Still, I feel like I adjusted the imaging setup correctly, so I don’t know.

With 10 um of SRN

EDFA, 12 V and 10 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/359CE8D9-A109-4B25-8325-B493C1B46213_2/GAHprmy5CVC1Dv7KRwWXBtVYb4kV5rezNjNq7PYxIbIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/F05782DA-F223-4731-9240-77AF0324641A_2/sDisKOiwxMfIS4mLKyOjygGzB1stQQVxJrR9aSMp4O4z/Image.png)

14 V, 7 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/DD602F59-9192-44A6-9A4E-6A38AC3FF1F2_2/Pc64ZXV0yKPxUDkOo7M9kKj87fgNxwtyOZ4SL0xeJMEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/6892505F-F0FF-43AA-81D0-B42BD582DA30_2/WxtJRACxGwvj2COcy1trwEo95czrg4bnOy0mPLbu7x4z/Image.png)

81 mW out of EDFA, 26 mW out of waveguide.

Now onto santec

14V, 7 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/D64ED5CA-1354-4165-B931-221131369920_2/zJQMnqkxHL14JvIsubcrwPMsMmNIVeVJGwkFbhhFf0Ez/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/2E6BCBD0-572D-4D3B-878E-F0BF064E1BC0_2/ni4PSQUJ5kDjmZUV4sp8NxygLfx21SG8uC2ReJx4gMQz/Image.png)

15 V, 10.5 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/77DC3901-73C6-47D2-8667-01DFEB90E80E_2/dspVCtYvRoidiy2OEhBvsTEUl6OzHumPCg0KI0UKZUEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/ACD1E801-65C2-4C36-AD18-EFB6F88E4000_2/mkxLyhLSuDsoWGTVQr293YqFcl8kpI101ziwOA1is64z/Image.png)

16.5 mW out of santec, 5.4 mW out of waveguide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/73844E87-E787-4A44-93CE-50A31F32C75C_2/TvjsK2MNxi13IoMAJbOSny6vj1ioZHafucvqHLPobGwz/Image.png)

Not quite as high as Ryo guessed, but it is off by like a factor of 2, which could be explained by some error.

Below is what I observed

| Waveguide               | Loss (dB/cm) | Conversion Eff (%/W) |
| ----------------------- | ------------ | -------------------- |
| 10um SRN with SVM core  | 0.667        | 5.3e-4               |
| 6um SRN with SVM core   | 0.667        | 7.6e-5               |
| 10um SRN with SRN3 core | 0.474        | 7.6e-5               |
| 6um SRN with SRN3 core  | 0.474        | 1e-4                 |

For some reason, I just have a hard time believing the SRN3 with 10um of SRN.  That is the waveguide that gave us trouble in the first place, and the only one that did not give us a nice SINC function.  Lets try it one more time with the imaging aligned as it is now.  If it is repeatable, then I am a bit out of ideas.

Going back to SRN3 10um of SRN

EDFA, 12 V, 10 Hz

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/B0F6882D-E85C-46E7-83B0-8DF38CCA8D10_2/6UN2fgQJ2NQUsfZNm3K8uiHSZmAPAhe7Q6yUxZrEhRoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/E02A5A36-9133-406D-877D-6343F04C8A23_2/OyCgEmYc6d4pyW7QLnaXIFDPbooh11usfGz9j8Ulaogz/Image.png)

85 mW out of EDFA, 31 mW out of waveguide.  Lets move to santec

12.5 V, 10 Hz (13 V is the breakdown)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/E2D236A6-E84C-4F5C-9404-BDD537F750F4_2/NSMfmZMY3JjNVaiqe06vyQvkbmMY1dXK0E9ZGdIfUEYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/4426CDEA-64E5-4025-9691-A24882114805_2/dCdmYgQ94hXrfnQX2XlMxrkmDpGEuUfrZBjIjWkZT5Iz/Image.png)

18.4 mW out of santec, 6.3 mW out of waveguide.  About the same as before.  

Now lets do a quick exercise where we look at the quadratic conversion efficiencies of several waveguides and see if the numbers sorta make sense.  In theory, we expect the 7cm chips to have 50X greater conversion, and the 10cm chips to have 100X greater conversion.   All of these scalings were roughly L^(1.8)

For 10cm SRN3 with 10um SRN, we have below for 1570

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/e7f57856-bfb2-ab1c-f366-74356afaf8fe/w2iPixQGyY5YU32ln7OyV46RwdpuPsmu8xIimNwtSuwz/Image.png)

For 7 cm SRN3 with 6um SRN, we have below for 1570.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/3B504FF7-739A-47BE-B0A1-F602996C8D0C_2/rTk9HfcIXsCZdZ80SQ5uEnVEMCaOnDuliQMAOSwQd34z/Image.png)

For the above, we said we saw 1 mW out, if we used anything higher, this would come back down into reason.  If we assume we got 2.4 mW out of the wavguide (like 1612) then we get below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/9203F68F-0BFB-496D-BCC6-50D36DA0AFAE_2/7iKltEhzsGWEVaeWUGIrL9s3dz7rZyy97KzfbT9j0yUz/Image.png)

This says our 10 cm spiral still was not as good as it should have been (it should have at least been twice as efficent), but it makes our numbers work again.

For 7 cm SRN3 with 6um SRN, we have below for 1612. (we saw 2.4 mW out of that waveguide)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/FEFD8A03-AF84-4D1B-88A4-7B48F5877F16/D5A1A180-BD07-4C97-B2BC-CB6619917553_2/fVleh6IN9ovetPi0Bb2VIuvxMzg0BDrkuKgpfxFXmLsz/Image.png)

Ok, so if we assume 1.8 scaling for everything, using our conversion efficiencies on a 1cm waveguide, below is roughly what we would predict, and what we got, after quad scaling.  I don’t know how much I was pushing the voltage on the 1612 chip, so take that one more with a grain of salt.

| Waveguide type                     | Wavelength | Predicted conversion efficiency | Measured conversion efficiency | Measured Improvement Factor |
| ---------------------------------- | ---------- | ------------------------------- | ------------------------------ | --------------------------- |
| 10 cm long SRN3 with 10 um of SRN8 | 1570       | 0.0048                          | 0.0012                         | 15.8                        |
| 7 cm long SRN3 with 6 um of SRN8   | 1570       | 0.0033                          | 0.0014                         | 14                          |
| 7 cm long SRN3 with 6 um of SRN8   | 1612       | 0.0033                          | 0.0007                         | 7                           |

So we are kinda always off by a factor of 3-4X.  A bit unfortunate.  Another interesting way to look at this is, while the 10cm device did not have as high of a performance as it should have, if you compare to the baseline conversion efficiency, we did see if being better than the 7cm devices.  So the prognosis here is not super tragic, more just annoyed by the underlying conversion efficiency and the loss.  I would like to do some calculations as to what the expected improvement factor is with a given loss.  Our naive back of the envelope calculation is a bit deceptive, as it does not cound for the fact that, after light at the beginning of the waveguide propagates the full distance, its real conversion efficiency is much lower.  I would expect 20X to kinda be the best we can hope for, which means the impact of this work is lower.  Ultimately, resonators are the only feasible path toward :(.

 Hopefully, the above simulation will tell us whether we should emaphsize the higher conversion efficiency of an SVM device or a lower loss, lower conversion efficiency SRN3 device.