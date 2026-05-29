---
type: craft-export
title: "2024-11-11 first sinx waveguide etching"
craft_document_id: 3930A969-E6EA-428D-AF79-19F766336B02
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-11-11 first sinx waveguide etching
This document will detail how Ryo and I fabrciate our first etched SiNx waveguide.  The broad steps I want to follow:

1. Pad oxide deposition.  I will put down 300 nm of high rate oxide
2. Cr sputtering.  I will put down 225 nm of Cr.
3. Photolithography.  Probably have a rather thick resist from past experiments, and it would be nice if we could use something a bit thinner.  Maybe something on the order of 500-600 nm will do.  I will use the YES oven to prime the wafer and then spin the resist (though primer will probably be fine)
4. Descum and Cr etch.  I will desum for 90 mins, which will remove 180 nm of resist.  I will copy previous recipes for Cr etch time
5. Nitride/oxide etch.  This will be a bit guessy, but we will try our best.
6. Cr mask removal
7. Pad oxide removal (optional).  Either BOE or RIE
8. TEOS deposition
9. SRN photoconductor deposition
10. ITO

Quite the process.  I am honestly a bit proud of this.

For the pad oxide deposition, we previously did 53 seconds for 200 nm ([https://tdwg.craft.me/mHWJ9IfqJ9l98w](https://tdwg.craft.me/mHWJ9IfqJ9l98w)).  This means we have a dep rate of 230 nm/min.  So for 300 nm, we should put down for 1.3 mins, or 1:15 seconds.  With a two minute season beforehand, we should be fine.

For Cr sputtering, I will do 1210 seconds, which should give me 115 nm.  I previously found that the etch rate of the PT770 to be ~20 min/min.  It has roughly 1:1 seconectivity.  I will etch for 8:30 mins, like I did here ([https://tdwg.craft.me/aKB3RiJNItgyAk](https://tdwg.craft.me/aKB3RiJNItgyAk)).  I wish I had mentioned the amount of Cr I started with, but I can pretty easily infer that number.  I am overetching by 3:30 minutes.

Before Cr etch, I will descum for 90 seconds.  This means, with the Cr etch time, I will be getting rid of 350 nm of resist.  So, after using the YES vapour priming oven, I will spin with 3000 rpm, 8000 ramp, for 45 seocnds (I might even increase the speed slightly).

For the nitride etch, we preivously found that oxide etches at 150 nm/min and SRN etches at 170 nm/min.  This means, if I want to get a micron deep into the SRN, I should etch for ~8 minutes.  I will make it 8 minutes and 30 seconds to be safe.  Our Cr etches at a rate of 6 nm/min, so the most I could etch here is 51 nm.  I would say I am safe on that front.  So the steps are below.

- 1:15 minutes of pad oxide
- 1210 seconds of Cr sputter for 115 nm
- Yes vapour priming oven
- 3000 prm, 8000 ramp, 45 second spin 1805 resist
- Bake at 115 for 1 minute, exposure, and develop (I will probably stick to beaker develop, though I could use a hamatech)
- Descum in 81 for 90 seconds
- Cr etch for 8:30 (after 10 minute season)
- Oxford 100 etch for 8:15, after 5 minute season and 5 minute pre clean
- Cr mask removal with wet etch

I spin cleaned the sample and wiped the box down with acetone. I ran a 5 min pre clean on Pecvd. Now I will do a 1 minute season with high rate oxide 

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/042E3498-6181-4419-8B3F-E26426195601_2/xqoqXUc5Q1QLQUt0QWiet7jt1o8sVOueiGElA6AAXlQz/Photo%20from%20Library.jpeg)

All my recipes were ran with the carrier. I will use carrier and heat for 5 mins instead of 2

Before deposition



![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/74B344D1-9B90-457D-9939-A31E54B7EC48_2/5uYcycmc9siP6F65XvzDtbY3xdadvrYa3MCaOLCcM2kz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/2497AD66-23E0-4EC3-A6BE-3D83DC9B8523_2/j09vyekPgNoQAZGQY089OgrUpxndUt5CZbvesXF5uKAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/79D15BE5-FFF5-4C27-B59E-EF9869EDEFA8_2/Jd72boypVbKQwu7GdyPK5IJGhvL2PrMyzPRqh2qk0woz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/387BEECE-26BC-4FC9-9D91-AB0AE81C8D01_2/7fncjSRLtuq8fKEB9LFxP5ilL6CWBHkiObjYxBBbnIwz/Photo%20from%20Library.jpeg)

After oxide deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B3935FE7-E831-4F10-9AB5-C2BAC0D902C7_2/GVESni7rN3XDE6JAjQ80CI7ycVsdneaIEKsUDScLIPkz/Photo%20from%20Library.jpeg)

We now mounted our wafer and are ready for Cr

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/DCBA7BC0-828A-4205-86B8-109AE77F9F5C_2/VT6nPtLOIffxfbvogj9JhLWPFKqF41ebKiZ9HtjeSrMz/Photo%20from%20Library.jpeg)

The first day did not work.  I came back, cleaned, remounted, and tried again a week later.  I should mentioned that a screw did fall on the oxide surface, so it could have been cleaner

During sputtering 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/3286A98F-2A13-4900-8372-8A9ACE6881EE_2/R8gcQSe0012ZxvaPcjd505wFzPkb4QiAwq7DsnSWiHUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/ADB3B7F2-9FD8-4565-9CC2-7E78BEAA1A85_2/5lfRmGRQksON2x8yibm6505arrWljEba5BqYqQPK05Uz/Photo%20from%20Library.jpeg)

I programmed the tool for 1210 seconds (~20 mins)

I am now sonicating the witness sample for 6 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/BBCFF9D9-80D3-44CB-864E-668B97D1D648_2/TRVPet7EvlmsVE8tW6LWeyCsFXfeE3tGRzSAy0xxu7gz/Photo%20from%20Library.jpeg)

Bake at 90, then do 60 as dose. 

Characterization of witness sample

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/031A9CE5-1B40-44E5-8865-83D403F6EC95_2/WY0qIO8erSjyHfoxKiFJRF6Mj47WfFKGia8QurOjK6Yz/Photo%20from%20Library.jpeg)

Roughly 100 nm

I am vapor priming the wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/99F0B462-F172-4C0F-B9AF-D7724929374D_2/REY0vQa6dCT2w0MZRBHrYPFUKVctDgLX8tXl0TGWqQAz/Photo%20from%20Library.jpeg)

I will now spin 1805 at 3000, 8000, 60 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B449DBC0-99FA-4922-8E07-665CD69373A1_2/9aqxlwYQKqHa59Rmvz0t9rTae3wdni7eCsKuGvHQyDcz/Photo%20from%20Library.jpeg)

Bake for a minute at 90

After spin and bake

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/EB3970BC-4C79-43B3-B9C5-313CAFAE0197_2/TEf5UWhG8k3ofU3Xhf3AYvwOVyCrsW8is1FUwfSPgnIz/Photo%20from%20Library.jpeg)

Looks quite good. I will remove edge bead after exposure 

Picture of my file on computer 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B24E8BFB-DD23-4005-AE29-DF39137F84BA_2/j1XgvnUCrWhyNJiWIvuvojVlekPoeDSUK94JU7nxwiUz/Photo%20from%20Library.jpeg)

Before starting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/0FCEB913-F62C-4A1D-82DB-1D759D0624DB_2/xey1wlz2ypX6afpVPhxq7AxFW1wMeFTk1pxWEyXum3Qz/Photo%20from%20Library.jpeg)

Does is 60. I also clicked wait for conversion

I will want to do 726 for a minute development 

# Note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/86AAB2A9-CF05-4CB7-BF6C-BB3282613BB5_2/eZN1KsFPjgQLFVMckJzSitq6S53uwe2xdxryEk6yZ1wz/Photo%20from%20Library.jpeg)

15:25 Process finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/9156E486-8BF7-4818-ACC7-2F453A535AEC_2/NZ8njy7n8Jurx0CHa3vWi255i9dq6Goc8OsV9UZrxZAz/Photo%20from%20Library.jpeg)

Taking out the wafer.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/8059A5A3-7D9C-44D2-B4D6-B6D4381B08D3_2/HYfxyPIVy148VwaO8IBiuY85Esi0kZNRyDttBQoVbnMz/Photo%20from%20Library.jpeg)

15:27 Water development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/5A56F395-79B8-4513-AF5D-93EF8B037CB1_2/9TLOSjy59XD6C7EkIRjhNYKN8Zw4A5QoxWfGFU7YiYQz/Photo%20from%20Library.jpeg)

15:30 finished

15:37 Edge removal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B4BB978A-C8EB-4FA6-8CF0-5D676958D14C_2/niTCXVXnWszrIkjTACVc6hb3y9aYObHEtHsAZAaLN14z/Photo%20from%20Library.jpeg)

15:46 Profilometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/9B27784D-2E0A-46A2-ABCC-BF010A220559_2/xd2t3AoI9nXGuUaL0HJBd216BEHx7vj5GeRfa28orEgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/4E73CB94-0B94-40F7-83A9-8191D830B52B_2/k0KQ8T0WKTPgE26HeWBLV3BH9fpxhif91fpjOJgT5iIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/35CE0AD7-9A0B-4821-A680-338FCB977F0A_2/BJDsVFftMXEsZsCuHyxMGFzjvWOSqLZfjuTPhCkgXckz/Photo%20from%20Library.jpeg)

550 nm resist

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/96C3703C-5042-4D6A-939E-D69730BF9D03_2/f5t0TESMUOFJDBKToC9fZaHkBvzUvetsWrZVUcOshvgz/Photo%20from%20Library.jpeg)

17:03 after descum, we find 413 nm left

## Oxford 81

I will now do a 5 min clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/7D856480-D394-4ED5-8E18-39D10D2D0639_2/VvwAkwhyBxTfrXcFNomVx75AyJCRGaai9GYnpy5rATgz/Photo%20from%20Library.jpeg)

16:04 Starting mild descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/AF83CBCA-18D8-4535-AD8A-FA531AD1004A_2/ttm5hBkVL2Xsy9dw2NTiQFxhPGQS3UPf6oxIuJNdhHUz/Photo%20from%20Library.jpeg)

During descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/FB5C2309-739B-4B92-B679-E7CEDBCAECD7_2/zq9gs4j0UxIKGRaTBj0eXcvYrPaPeY4keuPYAagdGiEz/Photo%20from%20Library.jpeg)

16:11 Finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B2DAACDE-415A-48EA-A893-774BA783BAB1_2/5Qv259KATExC3NzDgjd59A6n2laHglNmxFB6BfvmFtEz/Photo%20from%20Library.jpeg)

## PT770

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/62A2BE30-D952-495D-AC31-96C7F2537ACC_2/hVjyQRBKim0xTrbad7CYovYgf3GXYFBpDWDApedDWQgz/Photo%20from%20Library.jpeg)

16:47 Carrier wafer for seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/E3CD995C-034D-4D48-9DB4-224F7B3D60D5_2/0P3wgl12cyxIG1g5omhMzxHpygEBqqcmB0lG5HNdKcIz/Photo%20from%20Library.jpeg)

16:51 Started

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/4BC94F6A-B604-4904-8775-71E14CFF9423_2/GFAtTqLyU2B0zgfRcR4raxdCG59g3weQzhd6xYWgDXEz/Photo%20from%20Library.jpeg)



17:22 Done

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/5CD4B2B7-13F8-4A50-9016-DE283EACB3CE_2/fGZQPtiB6s3cMKeQtz2hDodlBEvpBAoo5xNfLzGwoQMz/Photo%20from%20Library.jpeg)

## Oxford 100

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/7A4D8C9F-8871-4C1C-92DB-260732DF0AC6_2/nzr9I5Jkn8p0aooBYdh7Ky8yawLbPDYFa3NtJVEeHLkz/Photo%20from%20Library.jpeg)

16:52 we do cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B0E008F3-7DD5-4B6D-AC05-896012452371_2/yysjCXxSOICgOBDwglPRIlLQyczjnUPofey93TaxHaIz/Photo%20from%20Library.jpeg)

10 mins cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/E4BBEA42-FDB5-4305-A0B4-A7A12FC15F83_2/xq8xGK1dmOhAC8NFySoe2Fw5W2wtl6W7xwGsdgsH5mgz/Photo%20from%20Library.jpeg)

We use 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/FFBFADD6-ECAF-4D6D-AA8A-DE231F137D08_2/BcqtqyemeL5iQSHkVOsaMnIyOvztxjyTzpZR5R3iGNUz/Photo%20from%20Library.jpeg)

17:16 Venting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/50BBF45B-B305-4534-85A1-E7EF881945ED_2/JgurhXhTYsAWf2ic7SIhqNWoGGYCognoL4j8U2fKxJ0z/Photo%20from%20Library.jpeg)

17:24 Etching

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/BED522A2-B62D-49F2-8D29-38583C2628EE_2/ybjstFCCoUQSMmNsgQdOmVthbtZTfu9niWrVXPxcUyoz/Photo%20from%20Library.jpeg)

8 mins

We could not retrieve the wafer. Coming back tmrw.

# [`Wed, Nov 13`](day://2024.11.13)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/05FFEBFD-1F1E-4385-B069-1F1CD7F28B4D_2/wo0n6k1OgcqrnDFKrT4eolI873Wxha7EkiCW2ZwCF4Iz/Photo%20from%20Library.jpeg)

Jeremy retrieved the wafer

We do profilometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/231C4E46-D7A7-43B8-95FA-B548EAE70AA5_2/h2ImP4kloDGND26R3TmEZ6aJiQsWMDVuQuyexVeBAeUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/E7F37FC3-AA7A-485B-9E88-12FFB591B75F_2/LCjpENwHtxvUpN45bIcBuC0hf9t06z4GnRyWwUn2P2Iz/Photo%20from%20Library.jpeg)

![Drawing](https://resv2.craft.do/user/preview/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/F81D4696-4EFD-4854-83AD-33258407191F_1/rfExR2s3xb3UX9QIywBHImeALRQWy8fLCfn9s4aNI2Yz/Drawing.jpg)

We see 2.1 um etch depth, which is deeper than we thought.

This is non annealed wafer. 

We should have 200 nm of SiN left.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/DA556EDC-1382-4C98-BF39-8327060328DF_2/eBmJNNdHAHd7gyEFoZpnsFOAdqaqkqbr8fPNJkh6WiYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/059D9997-8C8D-428C-AEA0-FC15E2FA3325_2/G0zlnTN7SILa7ES6x9vUh2RR653yUH44x6iW6ColPuoz/Photo%20from%20Library.jpeg)

Combined the chips to a bos

11:57 Cr etch of the cleaved piece. It seems to be taking a while, so we leave it there. It’s been roughly 8 mins since we started.

Under microscope 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/911BF9B7-0B7F-473C-9438-6AB96F03FA77_2/S4ERmNigv4xVskZXM4PO6WtbxXjUVMrjBIWQeM78AxEz/Photo%20from%20Library.jpeg)

Higher mag

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/C9F6EA2F-DF13-4839-94E8-EDB98D285141_2/NsSgEM2FnnFYBWyBxIcI9nOlhtgxEjXBp1fsnwRFEqkz/Photo%20from%20Library.jpeg)

Crazy spectrum, so no Cr left

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/B481CE00-9F9C-400A-A92B-48BCAD350971_2/NHO0l1wRyxYvGvi21xA7vEmPjOy6ytzMa90QvFKYCe0z/Photo%20from%20Library.jpeg)

Under microscope

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/EFC39645-178F-45B6-A51F-4CA9E485A30E_2/Jh2kHvNihxSdkAyaNaoHsdGj0tMMJ4WKuJGyNckcCxkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/6DFF2249-BC89-4803-B397-3B3F531728D0_2/pyppxNWFDk9sIyZTzpEuU3qoVcOKSXeZouhg6sWqkaAz/Photo%20from%20Library.jpeg)

After Cr etch and Hf dip

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/6E405A39-37E9-46A4-B749-A11F671FD754_2/hMPGEywuOGZLn8dk7K0xaqXqkTRhcyoonaTGbZT4tx0z/Photo%20from%20Library.jpeg)

All clean

After wet etched profilometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/C8F59BD0-EB64-4C82-A60A-AA1DD6C66F65_2/yaLDlAQJltVnEUmue1rjGCP4fnND9XWR2xswMrpa3f8z/Photo%20from%20Library.jpeg)

2 um deep. Even plus a little

Oscar sem notes

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/FEEAC55E-6341-41CE-82B5-E5F2F564F62C_2/6pT08ggvOgZDpOmpwAMvO6CQTYiog4T4RGr25c9oYFwz/Photo%20from%20Library.jpeg)

His starting positions

He used 2.5 as the energy

Use aperture 1

Always start with scattering detector

He starts by focusing on the screw (and using the 70 degree tall mount)

His good numbers

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/3930A969-E6EA-428D-AF79-19F766336B02/C2EA5E0C-904D-4593-9BD6-D15C4E912A8F_2/5kCK6usDUcBEclYcTaKWFaFplx9LXX04lMCxaoHEOogz/Photo%20from%20Library.jpeg)

At least as starting points

