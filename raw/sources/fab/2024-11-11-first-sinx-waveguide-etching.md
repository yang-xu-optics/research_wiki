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

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-001.jpeg)

All my recipes were ran with the carrier. I will use carrier and heat for 5 mins instead of 2

Before deposition



![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-002.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-003.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-004.jpeg)

During deposition 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-005.jpeg)

After oxide deposition 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-006.jpeg)

We now mounted our wafer and are ready for Cr

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-007.jpeg)

The first day did not work.  I came back, cleaned, remounted, and tried again a week later.  I should mentioned that a screw did fall on the oxide surface, so it could have been cleaner

During sputtering 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-008.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-009.jpeg)

I programmed the tool for 1210 seconds (~20 mins)

I am now sonicating the witness sample for 6 mins

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-010.jpeg)

Bake at 90, then do 60 as dose. 

Characterization of witness sample

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-011.jpeg)

Roughly 100 nm

I am vapor priming the wafer

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-012.jpeg)

I will now spin 1805 at 3000, 8000, 60 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-013.jpeg)

Bake for a minute at 90

After spin and bake

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-014.jpeg)

Looks quite good. I will remove edge bead after exposure 

Picture of my file on computer 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-015.jpeg)

Before starting

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-016.jpeg)

Does is 60. I also clicked wait for conversion

I will want to do 726 for a minute development 

# Note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-017.jpeg)

15:25 Process finished

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-018.jpeg)

Taking out the wafer.

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-019.jpeg)

15:27 Water development

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-020.jpeg)

15:30 finished

15:37 Edge removal

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-021.jpeg)

15:46 Profilometer

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-022.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-023.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-024.jpeg)

550 nm resist

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-025.jpeg)

17:03 after descum, we find 413 nm left

## Oxford 81

I will now do a 5 min clean

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-026.jpeg)

16:04 Starting mild descum

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-027.jpeg)

During descum

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-028.jpeg)

16:11 Finished

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-029.jpeg)

## PT770

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-030.jpeg)

16:47 Carrier wafer for seasoning

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-031.jpeg)

16:51 Started

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-032.jpeg)



17:22 Done

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-033.jpeg)

## Oxford 100

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-034.jpeg)

16:52 we do cleaning

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-035.jpeg)

10 mins cleaning

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-036.jpeg)

We use 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-037.jpeg)

17:16 Venting

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-038.jpeg)

17:24 Etching

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-039.jpeg)

8 mins

We could not retrieve the wafer. Coming back tmrw.

# [`Wed, Nov 13`](day://2024.11.13)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-040.jpeg)

Jeremy retrieved the wafer

We do profilometer

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-042.jpeg)

![Drawing](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-043.jpg)

We see 2.1 um etch depth, which is deeper than we thought.

This is non annealed wafer. 

We should have 200 nm of SiN left.

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-044.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-045.jpeg)

Combined the chips to a bos

11:57 Cr etch of the cleaved piece. It seems to be taking a while, so we leave it there. It’s been roughly 8 mins since we started.

Under microscope 

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-046.jpeg)

Higher mag

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-047.jpeg)

Crazy spectrum, so no Cr left

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-048.jpeg)

Under microscope

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-049.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-050.jpeg)

After Cr etch and Hf dip

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-051.jpeg)

All clean

After wet etched profilometer

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-052.jpeg)

2 um deep. Even plus a little

Oscar sem notes

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-053.jpeg)

His starting positions

He used 2.5 as the energy

Use aperture 1

Always start with scattering detector

He starts by focusing on the screw (and using the 70 degree tall mount)

His good numbers

![Photo from Library.jpeg](../../assets/fab/2024-11-11-first-sinx-waveguide-etching-054.jpeg)

At least as starting points

