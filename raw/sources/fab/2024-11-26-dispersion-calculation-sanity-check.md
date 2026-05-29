---
type: craft-export
title: "2024-11-26 dispersion calculation sanity check"
craft_document_id: 789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-11-26 dispersion calculation sanity check
From SEM images, we found the following below for the waveguide widths

8.575 um

![EtchedWaveguide208.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-001.jpg)

8.016 um

![EtchedWaveguide309.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-002.jpg)

7.516 um

![EtchedWaveguide414.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-003.jpg)

7.125 um

![EtchedWaveguide516.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-004.jpg)

6.442 um

![EtchedWaveguide621.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/DD863403-E05E-4775-9C59-EDA6950C7D50_2/RJj1Qpf1xAvpHAFxop1my0s7oghFjZPKTKa0ZQYoyM8z/EtchedWaveguide621.tiff)

6.023 um

![EtchedWaveguide725.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/ED7874E1-9B65-470B-B767-D3868F05CCF2_2/0ymwCvowG3Cqmq5DSxKSh1e0Yc09BraZpgvuzWVC1Aoz/EtchedWaveguide725.tiff)

5.407 um

![EtchedWaveguide828.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/254F7B5B-D534-473F-9B81-12C0E98A6035_2/yk3bSGh2sQbOdhfryGiilsfUniVCF1QNR1t0Iuw2GLAz/EtchedWaveguide828.tiff)

4.873 um

![EtchedWaveguide931.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/2B49905E-73CB-4AA7-A202-6E920A5FEACB_2/isMhh9ojHLc38J2PXB5d1UAPso4JoSC8zZclW9FRoJcz/EtchedWaveguide931.tiff)

4.287 um

![EtchedWaveguide1034.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/70FEDD11-178C-4C28-9083-A2327950DD38_2/w3LCbRypKiCJzNR0Los7UOr3RnJB1w2q36HyOpkvvNYz/EtchedWaveguide1034.tiff)

3.774 um

![EtchedWaveguide1140.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/0889A3BD-6A8C-439A-9B43-280F00719700_2/M01ntXXnDOpyJC80z1TY2oNCz4DXQ7zNuMZxjOkxs2oz/EtchedWaveguide1140.tiff)

3.206 um

![EtchedWaveguide1243.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/122E1E7A-0E02-49D1-9448-54E34FCC1330_2/Ug5Sb5yLAejxi2gq9EDDDuFUwyHmnMIcGlmA6E8x0JUz/EtchedWaveguide1243.tiff)

2.628 um

![EtchedWaveguide1346.tiff](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/2EABEF5A-264C-48B4-B5DF-BF73A09F3759_2/K7UHXrMJbGC1SAV7LiWAb3Y9t9WZIcYRjKdj5cbhgtcz/EtchedWaveguide1346.tiff)

Our conversion table is below (from expected to measured)

| Design Dimension (um) | Measured Dimension (um) | Fabrication Error (um) |
| --------------------- | ----------------------- | ---------------------- |
| 9                     | 8.58                    | 0.42                   |
| 8.45                  | 8.02                    | 0.43                   |
| 7.91                  | 7.52                    | 0.39                   |
| 7.36                  | 7.13                    | 0.23                   |
| 6.82                  | 6.44                    | 0.38                   |
| 6.27                  | 6.02                    | 0.25                   |
| 5.73                  | 5.41                    | 0.32                   |
| 5.1                   | 4.87                    | 0.23                   |
| 4.64                  | 4.29                    | 0.35                   |
| 4.09                  | 3.77                    | 0.32                   |
| 3.55                  | 3.21                    | 0.34                   |
| 3                     | 2.63                    | 0.37                   |

The error seems to average around 0.36 um (ish).

From our lab measurements, we same the profilometer below for the height of the etched region (which is a mesaurement I trust a lot)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/ac5c797e-c8c0-f5cb-73ad-debe1f7b9f0d/yaLDlAQJltVnEUmue1rjGCP4fnND9XWR2xswMrpa3f8z/Photo%20from%20Library.jpeg)

It claims that we etched 2075 nm deep (at this point, the Cr mask was off).  We expect that the pad oxide as ~300 nm thick, so we etched 1775 nm deep into SRN (so a remaining sidewall height of 225 nm).  Lets annotate our dispersion graph for these waveguides

![Labelled Preliminary Dispersion Plot.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/FC6ED2D0-8215-4994-B9D2-3D031B8A712C_2/fVguErbyLf7y79NiQofWRxdKjysV1gjAlNCxaPgbmxAz/Labelled%20Preliminary%20Dispersion%20Plot.jpeg)

Keep in mind that there are 3 stars missing

Ryo measured the values below for our dispersion

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/789F8C09-BBC8-4E7B-AEE6-2DE82F45BF1B/130CEB19-7DF3-4B40-A0DE-76317744BD35_2/i3xv4KOltTCyzPwgQn4J7BFWDPTUFRPDqsnmXLWwaFsz/Image.png)

He did this for the fattest waveguide (but we can kinda infer from our plots what we should see).  Everything agrees quite nicely