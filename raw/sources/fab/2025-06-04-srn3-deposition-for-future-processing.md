---
type: craft-export
title: "2025-06-04 srn3 deposition for future processing"
craft_document_id: D24A6B2B-EE96-44BF-9682-8614E8C83433
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-04 srn3 deposition for future processing
From our annealing results, it seems that we can get SRN3 to have less than 0.5 dB/cm loss at 1550 if we anneal at 1100 C.  This is a pretty useful result, as it means we can make really high perfomance waveguides in the future for very long poling distances.  Given that we are in a bit of a lull experimentally (where we are simply running some very long scans), it seems reasonable to start fabricating some new SRN3 wafers.  We can store these in the background so we can use them for final devices when the time comes.  

We found, from previous tests, that SRN2.7 is generally bad and SRN3.5 is worse than SRN3.  SRN4 is broke by annealing.  Obviously, these results are not perfect, but they generally give the impression that there is a narrow silane flow window of SiNx recipes from in-house PECVD that will work to give us low loss.  We could either just deposit one SRN3 wafer, or try to deposit a couple wafers with 2.9, 3, 3.1.  Eventually, we want to anneal these films at 1150, which I think it fairly achievable.  The one thing we have not proved is that 2um etched films will work.  We have technically only showed that 800 nm thick films work.  I generally believe 2um should work, as SVM showed no obvious cracking and I am not convinced annealing caused other issues.  But still.  

We are going to deposit 2um of SRN3, with the knowledge that it will probably densify to 1.7-1.8 after annealing.  We previously found that 24 mins gives us 750 nm.  This means, for 2um, we deposit at 31.25 nm/min, so we deposit for 64 mins.  Personally, I am of the belief that we should not break up the deposition, as that could add a weird layer in the middle.  We would only need to clean for 20 mins, as the deposition rate is so slow.  Lets deposit for **65 mins** just to be safe.

Afterwards, we will put on 500 nm of oxide.  I have not yet decided if we want to try Cr hard mask or oxide hard mask.  The advantage of Cr is I know it will work.  The advantage of a hard mask is that it will allow us to go to 1150-2000 C (making our device more broadband) and it is the way we fabricated the preivous round.  With the 800 nm thick ASML resist, I feel like we should be able to etch through everything, but I could be wrong.  Given the high tempuratures we are going to, I really want all the SiNx to be etched away, as I don’t want any possible stress issues.  From our previous characterizations, we can probably assume (after coating ARC and 800 nm of DUV), we will have 650-700 nm of resist.  We previously did 1:30 descum and lost 150 nm of resist.  We could probably make that 1:15 to try to get some more resist, but that might be risky.  Lets assume 650 nm of resist.  We then have a 120 nm/min etch rate on resist, and 180 nm/min etch rate on oxide.  This means we can etch 1 um of oxide.  This is not enough.  At some level, we really just want a differnet oxide etch chemistry.  Either way, this justifies my hestitation.



Per Jeremy, we can use the CH2F2 etch we used to use with resist and oxide.  He says it is a very clean etch in that situation and gives twice the selectivity, making the whole scheme possible.  



We are doing two wafers. Check that we have thermal oxide on both

![Photo from Library.jpeg](../../assets/fab/2025-06-04-srn3-deposition-for-future-processing-001.jpg)

![Photo from Library.jpeg](../../assets/fab/2025-06-04-srn3-deposition-for-future-processing-002.jpg)

Check ellipsometry of previous 3 and 4 films just in case I got something confused

3 below

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/7D39B04C-4121-4DA0-8814-6D90C7EF2816_2/yBEmCM2TkjX3Ok2I2nbM3iW73rpL3ifChytoyxVxwfcz/Photo%20from%20Library.jpeg)

4 below

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/E0B6E285-E4D0-4832-B15E-6D5B300FBC85_2/WOMiTXQdvmg6yPxBJ508J0dTg770GS1OfKmQS2nxXD0z/Photo%20from%20Library.jpeg)

4 has more peaks, so I believe I was right. I can also check filmetrics

3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/0D7A1F72-80A8-40A3-8738-A1D818A40698_2/CyfXpwGZrbvpeiAisnwPcmyNDyhs2HvaIVonigyh7YEz/Photo%20from%20Library.jpeg)

4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/2B803B98-53B3-40C1-B612-887410537F8F_2/qCoq76hxZztlyTksVIw1PRYeWbQJKEsD5Rp9BlxyauIz/Photo%20from%20Library.jpeg)

Not super convincing. I think the best test is color. Below is Takachi annealed

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/B3722C7E-98BC-4E1D-BCAB-2C1215FFD632_2/rG2MyS1QYyDuh3b1CIJr4iNEq7ZzDDwAoD0xNHgydU4z/Photo%20from%20Library.jpeg)

Below are 3 and 4, 4 bottom 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/786EEBF7-FBB7-40E5-A340-88B248F3ADBD_2/hZHUqWsCgoEETDVQ6GKJdi1IMEPCgOakpCEhr5sQcqgz/Photo%20from%20Library.jpeg)

We expect 4 and Takachi to have similar index

During RCA

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/FCC8FDE8-B506-481D-87BF-EDCF749763B9_2/Y0itjr1yxtGSKMSAOuHLFycsurtHBlaaqMtXCNYUGy0z/Photo%20from%20Library.jpeg)

### Pecvd

Pre clean for 10 mins

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/C9BABE43-EF2B-4CAF-9D6C-CF2690061D72_2/f3WlQ0U7TaaAkYOCRhLGanGefS4fmg6NloADxRDxQzgz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/7B043413-2C49-42CB-9A26-0DC1A6A0FAA8_2/8vky0VH4uGoy4vUIwhJDthnvK3Eaoz7UTURACpZjKLcz/Photo%20from%20Library.jpeg)

Before main dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/561A71B8-7111-4D7E-873B-A9B9DBA782CC_2/D8uOyMgPiBynBrx7hOKrhWkHEa3SnBoNQZWPA6DkTnMz/Photo%20from%20Library.jpeg)

It is going a bit short, I forgot to use hour notation

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/E13E8FD2-1AF6-4C96-9286-6A8804C6CE64_2/LjqNqjFB4lQjpktIBeOmIyGumCDPZUtS7fTvBCgtWecz/Photo%20from%20Library.jpeg)

So we still need extra 6 mins. I think wafer should be clean throughout if we just do two stels

Below is before extra 6

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/CD2FFCC1-0342-4B15-9F93-AA3E0237E464_2/CkVkexkksxLeg7xnekpxZ7TezjPYl4W1cnWxtyztW7Az/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/26F0A376-8BDE-4236-830A-20AD967980CF_2/8ye45ZxUL7dhTTV3JpllhY6hjCI5ExcoBGv1OBKSiqYz/Photo%20from%20Library.jpeg)

Ellipsometer 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/E6028FD2-028A-46BA-B53E-0A94BBF9378F_2/f8OysCX6j3YmvhhTpHzqjrgxkV8WIyyX8pHmkO45BSsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/31BC5088-20BD-46F8-B71F-D6545094A958_2/y5rFocMS7JJnP5BHsiVQuxkxEaUHHMhRtydJg8xIJ0cz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/CCDBD1CC-3D2F-484B-BB5E-756B208CB2B2_2/3vxPyviVfk8xZFQAi9tXP64jYZNx1cIA8fW67JakZfMz/Photo%20from%20Library.jpeg)

Index seems uniform

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/545D9356-8110-4928-87AA-87A426AFE929_2/EDKGDImR0v3J3MWCIt2knoY64UH7HFe5ex0VZ8yjZGQz/Photo%20from%20Library.jpeg)

Index is slightly lower, but there are not perfect fits.  Looking at old data from oxide capping definately confirms this.  

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/179664B7-0BBA-427E-B73F-F855B354FA31_2/dH5nyVHIQgW675NKlUdck4sOioUWBDxWDacPJlNpHPoz/Photo%20from%20Library.jpeg)

While the other films were a tad thick, I say we stick with the same recipe

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/3131456D-F689-4885-8345-CDE22CE15A39_2/4Z06pDvMysxG9d2LofvyHeNV9IPbAKuxx4Mfytl1ydIz/Photo%20from%20Library.jpeg)

During second run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/51FD665A-0987-4FAD-8BF9-43935E9894A4_2/UNVhHicBgVlkcU4RjzucgWkHPFIjokJCfXaxDwfSTw4z/Photo%20from%20Library.jpeg)



I am going to do top oxide capping another day and RCA beforehand.  We do this with SVM anyway, so it’s no big deal. Back wafer is 2, which still needs ellipsometry

I transfered these ewafers to the SVM box.  They were found at the back of the DON box.

Wafer 2 ellipsometry

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/316170A9-D692-4C4D-97C4-2C9E0C959BAD_2/NCkxzYTEWyIwLM7AX51InsnnmeGFBKyTGVSJ6cxeMPcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/4A2C18C8-78F0-4E6A-BBE4-3CE0DE65DCEC_2/PMBh4W3vVm3FyqofjkafbBiZvvpoBqZiFSvLpyga7AEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/E661572A-52F2-4F80-8577-036748115EB0_2/LyMurgTgStnTSeVzptG6YV2Luz9K2oxWyyTAnrfxQg8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D24A6B2B-EE96-44BF-9682-8614E8C83433/87DA955D-6535-4A7B-8C62-002D0B46D04A_2/NeyJK41Sdql49n6CixqoDmEL1CaUyita6gM3h7fPXgcz/Photo%20from%20Library.jpeg)