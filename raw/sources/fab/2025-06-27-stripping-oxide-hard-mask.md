---
type: craft-export
title: "2025-06-27 stripping oxide hard mask"
craft_document_id: 0599FB52-ED07-4AD8-928E-E1CE0A71A964
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-27 stripping oxide hard mask
We seem to have confirmed that we can make low-loss waveguides using oxide hard mask on tapered structures.  The goal now is to see whether we can strip the oxide hard mask off at the end (or at least make the structure look pretty).  The main concern is that our structures seem to have this annoying mushroom shape, and this does not look nice when we are trying to do capping.  We will try to do a BOE dip in this study and see what effect it has.  Below is the fab proeedure:

1. 800 nm of DUV reist and exposure with the tapered structures with 20 mJ of power.  I am not sure exactly what the feature size is here
2. After development, descum for 1:20.
3. We know we etch ~1400 nm of oxide in 9.5 mins.  This means we etch oxide at 148 nm/min.  We want to etch through 900 nm of oxide, so we etch for 6 minutes.  
4. We run Piranha and eco clean
5. We etch the nitride for 5:15 minutes, as we really would prefer to not over etch much.  
6. We dip in BOE for 1 minute (cleave wafer up here too so we can see wht happens after several different dips

We will take SEM images after to see what we get

### Photolithography

Before arc

![Photo from Library.jpeg](../../assets/fab/2025-06-27-stripping-oxide-hard-mask-001.jpg)

Before resist

![Photo from Library.jpeg](../../assets/fab/2025-06-27-stripping-oxide-hard-mask-002.jpg)

Before Edge Clear

![Photo from Library.jpeg](../../assets/fab/2025-06-27-stripping-oxide-hard-mask-003.jpg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/1CEDAC0A-89C3-4C6A-832B-2E1E2F6A04FA_2/F5iAttQKCLfwM5ulqdKQHTKUboHCDDFHVQD23wYVSfkz/Photo%20from%20Library.jpeg)

Before main pattern

Changed all doses to 20

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/7B6C0DD7-84AF-4BE1-BFEC-3DA5AA80852F_2/jxOMer9BSC8UM8VrvTee6yHF5FhgnBRQPBM0XEIeutEz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/4902E6EF-D292-42B8-84D6-049ACD22A65B_2/bEOBy2dljaWu7jkBjzC95DkNZKOEvHDRxChFl6RTAbEz/Photo%20from%20Library.jpeg)

Before developing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/6EFFE93D-4E69-45AF-BCBE-D07DB8066BA1_2/0pn2kOp9xHpy6nxEES7oaszqHpicTxmp9ebJ16SIXNoz/Photo%20from%20Library.jpeg)

### Etching

We preclean 81 and 100 for 5 mins. We then do a 1:20 descum on 81 and a 1 min season on the 100

Before oxide season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/1F9213E4-7DD2-4A1A-B54B-DB1C1A13B279_2/PzNvLwvj6Lb6SMxxmmz71NCRRAbmaGpMDy4vubjB6ZMz/Photo%20from%20Library.jpeg)

Before descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/C20B086F-E8E3-4A38-8B9F-166A37F617C3_2/axJYJRXm0ExPlZr4SObuHBwFr5JDNpgCoSc962XJ58Uz/Photo%20from%20Library.jpeg)

If the SiNx etch gets rid of 700 nm of oxide in 6 mins, it etches oxide at 116 nm/min.  We then know it etches SiNx at ~ 500 nm/min.  Ie, pretty fast.  Again, this is a bit guessy, so I still say we stick wtih 5:30 - 5 min etch just to be safe.

Before oxide etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/AE8A55A7-647C-4D13-AF95-6047715747F1_2/how6hMSvVpNivXhiPkVOdmANSarPC9iCzK1jvq5DKDsz/Photo%20from%20Library.jpeg)

During oxide etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/2D12365C-F838-4EEB-8DEA-8E77A8163FC5_2/yRt63x5vZsOgx3SAI6VCgEn9O8aMgjlhseJMCzt1tl4z/Photo%20from%20Library.jpeg)

We now run an 8 minute clean.

Now, 5 mins on EcoClean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/47C25B0D-9B60-46CA-8A7F-F1CBB9A30C69_2/w9ELq0M17N3jbU67tkdrQsb12eUtpb0R5cc1p5LLyfIz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/41931109-C623-404D-A024-69896127EE86_2/CfKyzHTIfJ8h7hgY9nsuqf8Q7Il6ehLxtTvKirNT3moz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/C354527E-C132-4EB9-88B7-23114F6B588C_2/qQCt6UgsRTXh7a0r8NRXLBXFBuo0F1VgPsOxeYdEPYMz/Photo%20from%20Library.jpeg)

Before piranha

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/C6DE096A-1ECA-4D82-A83F-949118EE383B_2/sqqNgH7qMCjG4Oz9RItF4vKSs7dhSA1wzTsqR7fHxHoz/Photo%20from%20Library.jpeg)

Before nitride season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/E3B83299-C69D-49B2-8938-EB284B1077F8_2/TJr6vtTteebAnTtGPU2qEr0HGv9JsWxvSOTA15x64PUz/Photo%20from%20Library.jpeg)

After piranha

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/65E8D8C0-DECA-42ED-BD03-EE9257EE6447_2/aSZBspmrCLxdzKGwXCIKLe1Typ51ZZ4BHD1or0Oc7XYz/Photo%20from%20Library.jpeg)

Ellipsometer was taken, but I am assuming I had some resist left.  I don’t think I over etched.  Lets do 5:15 SiNx etch

Before

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/367078D0-8F05-433A-B34E-01D61C425308_2/zfjxLKXRL4RjcNKAQIK2YmABT9SJ1o9AEALepbD8oD8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/0738D17E-E765-457A-97DB-37DDFEB137F9_2/atnxYQVubtFOqgy0nEnkQClDloq4VZY9tDTL2ufDMHgz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/9C6685A8-0A7A-4343-8DD8-73666E31F24D_2/OuEAPLiB4NZZuc1NlkREyqKFau4CpCYdZEX0ZyoDfRcz/Photo%20from%20Library.jpeg)

 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/766A1209-9FF9-43AE-9580-127301294B5A_2/miTps0SwzCOpVKZXAD9IXFbG3y5eMLVy7PcgC0Hqw28z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/D7804318-BE9F-4FAC-97C7-9E6F965D4C14_2/Ye7dMoQFqfRqYQObc89WSTuKNbLHbPnutKllzPr09LIz/Photo%20from%20Library.jpeg)

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/193126CE-0E48-4787-ACF5-D0516423762B_2/GkT1dUA73ymv7vACNfIKD0CQPyS9OjTyfPAYHoYVHwcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/C08BABB5-E6FF-4AD6-A892-6A79840F4513_2/wHDS2uQd85vzaxggFxKCn4Tp0R49p5nkXa1LGohiTEsz/Photo%20from%20Library.jpeg)

Profilometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/6D2B02FE-C535-4A64-804A-F0A27DBCEC07_2/nomyRqSIW5xUYQmRrRc48CMeKKpqOC2Xz4O0YGxb9Fkz/Photo%20from%20Library.jpeg)

Another piece

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/1D55618F-AF4B-48CA-B1BE-6033938E7859_2/EqrMdEQPSzdWSyiBtASmacA294zxp93wVnjVr0wp9u0z/Photo%20from%20Library.jpeg)

This piece was more from the edge, so there could be some etch difference. Still, it is tough to tell whether I have much oxide left

Another center piece

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/71A5455A-FF46-46AD-9541-8BF65002D850_2/em7ACBcjwNbRmlPcv8reEK6i8KkgVqOJxGcXg1144HMz/Photo%20from%20Library.jpeg)

After 1 min BOE

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/6837951E-C031-4D57-833F-CE51C84D9AB7_2/C0Toz7lUmWOCoX4jB8ZWe4CNTOXGIfh37Z6tS6iPNZcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/8E0EDA35-DFD7-4188-8624-8EC4D90182B2_2/dRKy7mVxGvNF9IQ1OiZq3CVeYD8HSyOJZVBZrRTgcREz/Photo%20from%20Library.jpeg)

The rough conclusion here is we did not have enough top oxide. It seems, as best, we had 100 ish nm left. This is probably why we could not see it in SEM. Or the BOE did not really remove the oxide. Let’s leave a chip in BOE for 10 mins and see what we get

I don’t think 1 minute of BOE did much is the conclusion. I don’t think we lacked for oxide, as ellipsometry and the Profilometer numbers could not agree if that were the case

After 10 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/5E36CEE9-9D31-4B1B-B44C-2C137C1CA83F_2/H09WQSjyhcxbzeyUBAwbKJk1vyOSmVQz0sfShKxqGawz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/379EF5C3-A5D8-4386-BB88-6D3DE7E11281_2/7wMKaa8y2WuDi22VdIDxyinDWRCkLVclE1E1MWFu3yIz/Photo%20from%20Library.jpeg)

To be honest, I can’t really say I have learned much so far.  The things I know or have issues with are below:

1. It seems that nitride does not etch very fast.  If we trust Aaron and Yongqi’s numbers that oxide etches at ~130 nm/min, then we expect that SiN etches at ~20 nm/min.  This could still cause roughness, but we can say over a minute that very little changes
2. We notice very little difference between 1 min BOE and no BOE.  One challenge of this measurement is it was done on different chips, so there might have been some difference in etch depth as a function of position.  That being said, if we truly had 100 nm of oxide left, I feel like we should notice some difference in profilometer
3. From the ellipsometer and profilometer results, I am rather confident we have ~100 nm of SiN (as the ellipsometer could not fit without it).  Profilometer is a direct measurement, so I would suspect we do have ~2100 nm of height after SiNx etch.  So the tough thing is that we expect 200 nm of oxide, but can’t detect it yet
4. SEM images were inconclusive.  They were taken from different parts of the wafer, so the height measurement might not be useful.  I was not able to see any top cap, but at 100 nm thick, it might be hard to get a strong contrast.
5. The only thing I saw in the SEM is a small lip that might indicate an oxide.
6. We over exposed, causing our waveguides to be 1 um narrower than spec

I think the next best thing to do is take one chip, and do all the measurements (aside from SEM) after 30 second BOE dips.  This would allow me to easily detect any changes.  If I don’t notice anything after this, we might want to fabricate a new wafer with a slightly thicker top oxide.

Before etching 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/0B408FA3-0499-40F2-8A33-1B4FE1FCC119_2/gv47Xx5jJiPWsyS8Vk6yztrrkA7eKX8vN1lXyqF0FN4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/CFBCD91A-F92E-4B17-8FDD-4477DBB6C8DB_2/ha1TwEjAeyjZxlKY09VIlrEPHs5bBnSpYMW4B0WLVGsz/Photo%20from%20Library.jpeg)

After 30 seconds

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/D50E8172-E6C8-4918-A26F-8861EBAC93F0_2/dXkEkuJJe4jvXmnhoNyd1TixchXVLaU7NLjrmIltMPcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/30609918-CBFB-475B-8DB7-D87F40236E46_2/aSzO91xhNzy8rM769l7ixOJWzjxaggdyeh5J5xlyHxEz/Photo%20from%20Library.jpeg)

After 1 minute

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/5F7DCA45-656C-43B7-94FE-6C16C55E5199_2/vGEQCjG5nQtxKl75oC5RbcR0RLJ0xXNEXJ1etN1LcyQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/8608E9A8-CEB4-4C97-94CE-52CD135CC169_2/ox1Sd0MbPKtxU5kfkl4nnTxtnpxiewaO45UBVeep5nkz/Photo%20from%20Library.jpeg)

After 1.5 minute

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/8B976360-EDE1-489A-9522-CDEEAF2DE395_2/5ausyq5KdFnjH4fx0PJLY6ykz26OuhgnCCEwtho3pF8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/75898A5A-2449-4799-AC27-9DFB9D673C72_2/lbXbb7sz143LFAADrslTU3U9yrOMzYOYwLlrO6buG8oz/Photo%20from%20Library.jpeg)

After 2 minute

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/87C18CB8-C265-4FB1-8B1F-D822F29CDCE5_2/sOJIRJCDNThndpFul9wi3XN9HJoQ85diRXkBt8QDxG8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/A9F71944-3850-488B-8852-8A5C7C0E1DAA_2/6HbgyEk3jYkorscaYQZnSzLltLfEhWy8svgNYy40EJMz/Photo%20from%20Library.jpeg)

Results

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/22FFBF3E-5248-42B1-9F1D-2F3472BC1324_2/XmkYxTwRGiO7ZDZBKtsyR3TdCaYswlcqIyalVo1Ob20z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/A2A1568A-0D0D-477E-B9CF-DBC53AC981FD_2/D8ZH3zVHTvXROWuvbNLyiws4dE9vSmyMc1F54tMehVkz/Image.png)

Below are SEM images

No BOE



![NO_BOE017.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/FDFF91AB-CF8F-417B-A06C-7D52071F5385_2/3L91wiyOOiNDJOv14dmKMEop1DgEARHu0Xe6CWGdez0z/NO_BOE017.tiff)

![NO_BOE018.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/7E8BBE77-B53F-4B08-867E-5C1F931D6112_2/mWHJcBIlvKw7FyxT8AtqZ9VOwavIOTdteG9xEHKjOx0z/NO_BOE018.tiff)

![NO_BOE019.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/B5182CD7-1950-42CD-927D-E8A50CEF37CC_2/5Lpzx1uXBy6iuaxDbhM83cKR8xrGHRYOuN9Dxdcjjxcz/NO_BOE019.tiff)

1 min BOE

![1min_BOE012.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/0295B907-B2EB-4868-87C8-392E64265BFB_2/iluumFAppN1dyyTQTHcK7ExvifnFXy0vPvnssZwbv2kz/1min_BOE012.tiff)

![1min_BOE008.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/730A5E5E-21F5-4882-AAC9-4612842B5DD3_2/6dQr9gWPsIXmEVsQFmHiHy91Blwy74Aes3yrk7y0qosz/1min_BOE008.tiff)

![1min_BOE008-2.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/1A9A7581-A47E-4DAF-8D4D-9D5098413A55_2/C6pIeMWPK3tofxyycKePopt7Jtm3OyAqQFxsacKv4Tcz/1min_BOE008-2.tiff)

![1min_BOE003.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/D9E592D2-3C7E-4C37-91DE-2B24EBBB32C2_2/lbxzERWZVMHyUqPBlTsdie4qp8xuwyiZmupY4rDxf7cz/1min_BOE003.tiff)

![1min_BOE009.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/0599FB52-ED07-4AD8-928E-E1CE0A71A964/A2E160BD-9FC1-43A9-857B-5D5801FE1769_2/4O1Ql03VpRynAyuV1L43x3BxDPfKBHHf5H27uVr0ix0z/1min_BOE009.tiff)

Waveguides are also ~1um too narrow.  Below are some next steps before we do final SRN3 fabrications:

1. Check dose.  It seems that 22 gives us a 1000 nm too narrow (though this was 500 nm in the past). Lets do something that is a dose of 16-17.  I don’t mind a bit thinner, but not too much thinner.  We can also adjust the dose size for the thin and thick waveguides.
2. Check loss with and without BOE strip just to check that everything is ok.  Cap in the meantime as well and take SEM images just to check all the geometry looks normal
3. Try etching on SVM wafer with slightly thicker oxide just to make sure

I generally feel like 3 is probably a waste.  I am fairly confident I can do that, and ultimately nothing will tell me the exact recipe I should use on SRN 3 to get the exact depths I want.  I have a pretty good intuition in my opinion.  I think 2 is the most important.  It is a bit of a bummer that the wafer is no longer full, as it might be a bit tough to clean.  Acetone and IPA are fine, but not really enough in my opinion.  

