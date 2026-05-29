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

![EtchedWaveguide208.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-001.tiff)

8.016 um

![EtchedWaveguide309.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-002.tiff)

7.516 um

![EtchedWaveguide414.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-003.tiff)

7.125 um

![EtchedWaveguide516.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-004.tiff)

6.442 um

![EtchedWaveguide621.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-005.tiff)

6.023 um

![EtchedWaveguide725.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-006.tiff)

5.407 um

![EtchedWaveguide828.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-007.tiff)

4.873 um

![EtchedWaveguide931.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-008.tiff)

4.287 um

![EtchedWaveguide1034.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-009.tiff)

3.774 um

![EtchedWaveguide1140.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-010.tiff)

3.206 um

![EtchedWaveguide1243.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-011.tiff)

2.628 um

![EtchedWaveguide1346.tiff](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-012.tiff)

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

![Photo from Library.jpeg](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-013.jpeg)

It claims that we etched 2075 nm deep (at this point, the Cr mask was off).  We expect that the pad oxide as ~300 nm thick, so we etched 1775 nm deep into SRN (so a remaining sidewall height of 225 nm).  Lets annotate our dispersion graph for these waveguides

![Labelled Preliminary Dispersion Plot.jpeg](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-014.jpeg)

Keep in mind that there are 3 stars missing

Ryo measured the values below for our dispersion

![Image.png](../../assets/fab/2024-11-26-dispersion-calculation-sanity-check-015.png)

He did this for the fattest waveguide (but we can kinda infer from our plots what we should see).  Everything agrees quite nicely