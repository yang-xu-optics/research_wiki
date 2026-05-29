---
type: craft-export
title: "2025-2-17 perturbative and piecemeal approuch to quadratic scaling 1"
craft_document_id: EDA775BB-E2CC-497F-84DB-B77D257B6C40
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-2-17 perturbative and piecemeal approuch to quadratic scaling 1
This is a follow up study to the preivous efforts to show quadratic scaling of the SHG on the snake etched waveguides.  Firstly, we did not plug in the EDFA correctly last time, so we used the right fibers this time.  Below is the maximum output power that we could achieve.

![Photo from Library.jpeg](../../assets/fab/2025-2-17-perturbative-and-piecemeal-approuch-to-quadratic-scaling-1-001.jpg)

Now, we will run a scan similar to how we ended the last document.  First, we will find the optimal phase for each of the top two branches (assuming the bottom is zero). We will then do a phase-poling period sweep of each waveguide branch, and once the optimal condition is found, we will update the optimal conditions and sweep other areas.  By doing this scan many times over, we might converge to some optimal solution.  My only concern is how repeatable everything will be, so we will need to use a somewhat high n_itr.  We could also start to partition the waveguide into more chuncks and keep doing this

The other option, which Ryo proposed, is to randomly perturb the waveguide parameters (so phase and poling period).  If the perturbation is good, we accept it, elsewise we reject it.  This might be a faster way, though it feels like it may not actually be super repeatable or converging to the global max (instead of local max).

As a quick note on the first perutrbation experiments.  It seems like the code is working, only that we are not really seeing any positive effect from perturbation increasing signal.  I also find there is some RC constant memory for the device to loose the grating

![Image.png](../../assets/fab/2025-2-17-perturbative-and-piecemeal-approuch-to-quadratic-scaling-1-002.jpg)

![Image.png](../../assets/fab/2025-2-17-perturbative-and-piecemeal-approuch-to-quadratic-scaling-1-003.jpg)

We are going to try another scan with longer time between iterations and change of direction (start top right instead of top left).  I am also going to increase the number of points

![Image.png](../../assets/fab/2025-2-17-perturbative-and-piecemeal-approuch-to-quadratic-scaling-1-004.jpg)

Below are some early results from perturbation optimiazation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/4A02F278-B247-41A6-9465-804CF64C2576_2/9ZCqcUylUMjVxreta1H1P3k3aWAJq1ZER28zM6u2u48z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/7B0463FA-F335-43F6-AEDC-E780758152DA_2/G1dpv9JLJO9qovwpb2Rgvhdg4RgdQQ3ivE4K7PJxLogz/Image.png)

Ryo’s inclanation is that I am not leaving nearly enough time between the data collections, seeing the the oscilloscope takes 15 seconds to average new power.  So I should make n_itr 1 and leave 15 seconds between data points.  We could kinda see this earlier as well

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/47A46E70-9829-433F-949A-C6B9649C7881_2/OlbXppmWFalNnjXVKiioRDuyqNj3f1RlPHGRi4KxtAMz/Image.png)

Above is the baseline scan using much longer step time to allow the oscilliscope to do a full average.  Now we will try to do perturbation again

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/CEBA2D0E-3FF9-4DE4-ACDD-F0A421ACF9B4_2/FGDYk6phQcLlK6yz1kMPGOQt0nsnyEcRKDtH3aY8rr4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/80369921-9056-43B6-93C0-383D36D10B57_2/Tib2RfuxH1yIVScOsCsxrOUxp8nGPU5C46fmExcBbXMz/Image.png)

It still feels like we have stability issues.  I am going to try some of the earlier versions for size

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/9C12333C-8D54-40ED-8DB7-2005FB475886_2/BcWMkGW2Eq71H7vMykleKvVyewspQXjlmAfQL17gXjYz/Image.png)

By picking a different point from the optimization, I get slightly better scaling, but not insanely better.  At some level, I am tempted to do a stability test, but first I want to do more perturbations and see if that improves anything.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/58E90CD6-D0D1-4ED5-906A-0EA1F54A4AFE_2/y6jH5NobsVjzC1wc1BppzBxxIUswAPk7RW1n6rrulVcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/886A3091-1C26-472D-9414-249C8539E36B_2/OiVxgRvHwZ9t1gzQQKFEQQkx6BHhIPbqwMArUm3IuFEz/Image.png)

It seems like the perturbative approuch is going backwards.  Honestly, this is pretty disappointing.  I am going to do a few more scans but I think we should focus on stability and homodyne detection

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/95ED7BB9-9AEC-41D2-B4BD-248C311B2E5C_2/gwnVcL7lxZt7boGHrhHVu2ybV40mCcx7lLRkyk3VKz0z/Image.png)

So funny enough, with fewer points, some of the earlier optimal sections are not bad.  I will increase point count and try again

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/A342EE39-9416-4165-BE1C-0AA5C6ADD308_2/WMyt4xE2xZhA4qT2YylJoyycQgMyUKWMONxUgbghV9Iz/Image.png)

I want to do this scan a couple more times to understand my varience

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/C0BB9341-EBCB-4F48-9793-2B66CA8C4B25_2/xdvySOre8iraRRRpeBhtP7e5BcacFtNnAQRiG3ja8iwz/Image.png)

We have some huge error bars.  We are now doing a stablity test by turning on a pattern, leaving it be for 30 seconds, taking data, and doing the same for a totally off pattern.  We will do this 60 times, so this tests stablity over an hour

Video during scan

[Video from Library.mov](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/2B2B728C-D268-445C-98D8-681B4D65B385_2/mrqrg3QaVZhsKkNJMMpGbLh2lbyJyDU3tIAvuS7URM8z/Video%20from%20Library.mov)

Below is the stability plot

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/DA305293-4ED5-4F26-930B-EC5CD721E482_2/6j9zsbdx2WWv9yJqzuyvqOyAl0pc4b2blivxTSaFsUIz/Image.png)

A few quick notes. Please start scan on top left and go to bottom right, as that is how the setup is oriented

Below is angle scan by the way:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDA775BB-E2CC-497F-84DB-B77D257B6C40/EB0139D0-9DFC-4A43-9C43-C7CE7386D8B2_2/7RzBDXWbhyJJC7F2ZXd7N68j3zOCuA5hxLLiyA3zhI8z/Image.png)