---
type: craft-export
title: "2025-06-30 loss test with boe oxide strip"
craft_document_id: 104FD5B8-CE5D-4974-B89C-1330FFBAF700
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-30 loss test with boe oxide strip
It seems like we have roughly figured out how do make low-loss waveguides with oxide hard mask.  This will allow us to put our chips in the 1200 C tubes eventually and take advantge of the seeming lower-loss of the oxide hard mask recipe.  It is also nice that we are not basically copying the Lipson approuch almost completely.  While I don’t think we will have issues with sidewall roughness after BOE dip, a reaonsable concern is that we use PECVD nitride instead of LPCVD nitride.  This means our etch selectivity is not as good, so whatever non-noticable effects people have with nitride with LPCVD might be far more noticable for us.  

The first issue is that we have no easy way of cleaning our existing wafer.  We could try putting it rhoguh RCA, but that feels like a bit much.  In theory, we have not done anyhting stupid to it, so spin cleaning should be fine.  We will cleave a line of pieces for no BOE dip, and a line for BOE dip.  We will BOE dip that chip for 30 seconds (as that is what we found to be enough for our leftover hard mask).  We will then put 10 mins of cap oxide on each and do 5 mins 800 C RTA afterwards.

There is a decent chance we will not have enough of each type of waveguide.  What I mean by this is we will likely have one type have a 2um (in reality 1 um) taper, while the others will have a 3 um taper).  I say we do 2um as the BOE dip, as it should make any increased roughness more noticable.

### Fabrication

I spin cleaned all the pieces after cleaving

I did the BOE etch for more like 40-50 seconds

Two inners had BOE

![Photo from Library.jpeg](../../assets/fab/2025-06-30-loss-test-with-boe-oxide-strip-001.jpg)

Before deposition 

![Photo from Library.jpeg](../../assets/fab/2025-06-30-loss-test-with-boe-oxide-strip-002.jpg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/104FD5B8-CE5D-4974-B89C-1330FFBAF700/B0076FB7-76DB-4D1C-9989-4985C2953D47_2/y2pvVgxauWWFqgXvQdLe4q0AGURNydiMvmh2jjs1DBAz/Photo%20from%20Library.jpeg)

Calibration RTA

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/104FD5B8-CE5D-4974-B89C-1330FFBAF700/EC115BDC-775A-4D23-8D6C-3AB97AB0AB8C_2/K3pcA5vtKA0zzPuZFsxOyaTvprtA6wwS00RLU4y7k4gz/Photo%20from%20Library.jpeg)

Main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/104FD5B8-CE5D-4974-B89C-1330FFBAF700/578BA1D4-B96C-4117-BD2B-66A33E22B3F6_2/WESRRFpBxASpxbmNTd4B4dpky6Di2nLxJ0pKCIeUjr0z/Photo%20from%20Library.jpeg)



### Loss test

Main setup, EDFA, 1570, 10x objective, 84 mW in

RTA BOE 2 um

Die 1

Straight 1

5.9 mW

Straight 2

4.9 mW

Straight 3

5.1 mW

Straight 4

5.8 mW

Straight 5

6 mW

Euler

3.6 mW

Short circle

4 mW

Long circle

1.5 mW 



Die 2

Straight 1

5.4 mW

Straight 2

6.5 mW

Straight 3

6.7 mW

Straight 4

6.7 mW

Euler

1.8 mW (a bit lower than expected, probably bad cleave)

Small circle

4.1 mW

Long circle

2.8 mW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/104FD5B8-CE5D-4974-B89C-1330FFBAF700/1BFD9BCE-4538-4A6D-A0F1-68E343BA22FD_2/XSN04BttSMbnVuvwTQpuqtVJo3pgSrkEYXXxbzEWP9gz/Image.png)

No BOE RTA 2um

Straight 1

5 mW

Straight 2

5.6 mW

Straight 3

5.8 mW

Straight 4

5.3 mW

Euler

4.1 mW

Short circle

4.6 mW

Long circle

2.4 mW

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/104FD5B8-CE5D-4974-B89C-1330FFBAF700/5144A8FE-CB42-4AAE-88ED-C023E8A9C1FC_2/tDCyqkrqer0Oyy0gAXMb9xAq8mcjhwlhQ6ajvxGWBL8z/Image.png)