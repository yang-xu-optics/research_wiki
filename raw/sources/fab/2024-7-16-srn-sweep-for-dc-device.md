---
type: craft-export
title: "2024-7-16 srn sweep for dc device"
craft_document_id: EDC92B59-F000-4251-975E-6E9F7D098467
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-7-16 srn sweep for dc device
Previous measurements have shown some stocastic results for differnet SRN recipes.  I feel that SRN8 and SRN6 are actaully fairly similar, and around 400 V, things start to break.  Anyway, there is stilkl a huge different between SRN3.5 and SRN6.  The hope of this experiment is to sweep the region in the midde and see what happens.  We also want to make a lot more B8 substrate, as it will likely be useful for future SRN DC device fab or general characterization. 

I also hope to fabriate some waveguide devices where we can test loss on B8 and create a device to test the linear delta_n of these films, as Ryo suggested some of my results on the SRN3.5 stack might have been because these films display hgiher DC kerr than we would like.  I am not sure I buy that explaination, but it is a good measurement nonetheless.

The SRN I want to test is between the SRN6/8 data and the SRN3.5 data.  I am going to try SRN 4 and SRN5 at the very least, but will likely try SRN4.5 or SRN5.5 as well.  Below are the relavent previous characterizations.

SRN4 41 nm/min

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-001.jpeg)

SRN4.5 43.45 nm/min

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-002.jpeg)

SRN5 46.15 nm/min dep rate

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-003.jpeg)

Below are the confinement plots for each of these recipes on B8

For SRN4

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-004.png)

For SRN4.5

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-005.png)

For SRN5

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-006.png)

Ideally, lets get 1um of SRN on each one.  We can adjust for modulation eff later

After running some course simualtions for conductivity, it seems that having a thicker core causes longer RC constant and the need to operate at higher voltage.  The upside is that it also lends itself to greater bright/dark contrast.  So the question is how long do we want to spend making these bottom layer.  My take is that it is probably best to do the full deposition of a 3um bottom oxide layer.  This will give me a more fair comparison to the other films.  This is just going to take sooo long.  I will do this on a full Si wafer, so I won’t have to do this again for a while.  This will probably help increase breakdown too, as I am worried the oxide might actually be the ones breaking first.

So the plan is as follows:

1. Break up the DON deposition into two steps.  Do season, 24 min dep, 25 min clean.  Then do season, 24 min dep, 15 min anneal at 375, and 25 min clean. Do this on a full wafer and cleave it up.
2. Deposit 1um of SRN4, 4.5, and 5.  This means do 24 mins, 23 mins, and 21.5 mins respectively. 
3. Deposit 1.5 um of B8.  We want to do this on the 4, 4.5, and 5 samples.  We would also like to do it on some of the loss wafers (hopefully an oxide, 2um Ta, and 0.8um Ta).  We can anneal some of these later.
4. Evaporate electrodes

This is going to take a while.  I would estimate 8 hours.  Big Gulp.  

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-007.jpeg)

Ellipsometer is broken, but we can see that right wafer has right color

Before season 1

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-008.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-009.jpeg)

During dep 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-011.jpeg)

Before season 2

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-012.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-013.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-014.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-015.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-016.jpeg)

During anneal, the wafer got up to 350 by 10:50. 375 by 7:15

Ellipsometer 

Using full water map

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-017.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-018.jpeg)

Wafer map

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-019.jpeg)

One outlier

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-020.jpeg)

Now high quality center point

Short

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-022.jpeg)

Long

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-023.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-024.jpeg)

Before 4 dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-025.jpeg)

I heat for 6 mins before. Witness is on top

During dep 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-026.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-027.jpeg)

The plasma looks more turbulent than usual. Plasma noise seemed to go down later. Maybe I should have been more careful with cleaning and seasoning at the beginning

￼after dep, we are not looking good

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-028.jpeg)

We should have done a better job pre cleaning. This is disappointing. But not the end of the world. I think most of what you see on there is dust that should have been cleaned off. Not sure if these will make for good waveguides, but we can try it out

Before season

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-029.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-030.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-031.jpeg)

After dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-032.jpeg)

This confirms my suspision that the guy before should have cleaned better.  Oh well I guess. 

I am redoing Silane of 4. Below is the recipe before seasoning

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-033.jpeg)

During season, the gas looked stable.

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-034.jpeg)

With 6 min pre heat

During deposition 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-035.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-036.jpeg)

There were no issues with uniformity after this one.  Really goes to show the importance of cleaning

Before 5 season

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-037.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-038.jpeg)

With 6 min pre heat

During dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-040.jpeg)

Before B8 season

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-041.jpeg)

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-042.jpeg)

Bottom is oxides. Top is SRNs increasing silane from left to right

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-043.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-044.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-045.jpeg)

Now onto thin oxide layer (probably 8 min dep) for the loss measurement 

Before season

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-046.jpeg)

Before dep 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-047.jpeg)

2um on the right 

During dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-048.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-049.jpeg)

Calibrating anneal

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-050.jpeg)

Smooth entrance. 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-051.jpeg)

Right is 2um Ta. Left is 550 core loss

During run

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-052.jpeg)

 The core loss film completely delaminated 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-053.jpeg)

Not consistent with what we have seen before, but I am not going to break something else. I will instead try a core loss measurement with anneal at 425. Maybe there is a compressive stress issue being on oxide. Actually, just extra delta n chips

Ellipsometey

SRN5

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-054.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-055.jpeg)

SRN4.5

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-056.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-057.jpeg)

SRN4

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-058.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-059.jpeg)

B8 no anneal

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-060.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-061.jpeg)

B8 (stress cracked) at 550

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-062.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-063.jpeg)

Surprisingly close to the index we expect 

Before oxide seasoning

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-064.jpeg)

We are going to run the actual dep for 6:20.  Roughly 1.5um of oxide.  

Before dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-065.jpeg)

During dep

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-066.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-067.jpeg)

Now evaporating 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-068.jpeg)

Bottom left is delta n

Bottom right is SRN4

Top left is SRN4.5

Top right is SRN5 

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-069.jpeg)

Life is good

Au in 3, ti in 1

We did have a bit of rate adjustment during Ti dep (I had to lower power). 

For Ti

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-070.jpeg)

For Au

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-071.jpeg)

When doing the automated measurement, I see that the bright state current limits at 450V. Not clear if it broke or not. Let’s scan down and come back to 5

SRN 5 is 0.6

SRN4.5 is 0.9

SRN4 is 0.4

Plots for SRN4 (chi3 = 3.5e-21)

![SRN4 1.0 Plots.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-072.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-073.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-074.png)

![Screenshot 2024-07-18 at 8.30.41 AM.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-075.png)

SRN4.5 (chi3 = 4e-21)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-076.png)

![SRN4.5 1.0 Plots.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-077.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-078.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-079.png)

SRN5 (chi3 = 4.5e-21)

![SRN5 1.0 Plots.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-080.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-081.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-082.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-083.png)

Very minimal field contrast and a lower delta_n.  There is more field in the claddings.  Lets do a full plot of all my results including previous measurements.  We should also normalize the voltages axis to the thickness of the core.  It would be a more fair comparison

For B8 delta n, our chip is 0.7 cm long

I get some very starnge results.  Firstly, I should note, this is a purely academic exercise, as the phase shifts here are really small.  While it would probably be incorrect to say that all the voltage we are applying to the stack goes to my doped oxide, it does seem that some decently large amount must get in. 

I put the camera rate at 48 frames per second, and the frequecny at 100 Hz.  Below are the interesting peaks

For “8 Hz”

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-084.png)

For “4 Hz”

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-085.png)

For “12 Hz”

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-086.png)

Looking at some of our fourier transforms, I don’t really see much evidence for the 12 frequency existing, but our resolution is not great out there.

12 might just be noise, but 4 and 8 and not!! Interesting that there are two peaks.  Lets try to think a bout about the path and what frequencies these imply, as it could be telling about what chi2 or chi3 occur in our material. Below is a quick math proof for why we see stuff at the frequencies we do.  

If we run the camera at a freq of 48 frames per second, this means we have a “wavelength” of 0.02083333 seconds per frame.  

If we run the oscilloscope at a freq of 100 Hz, this means we have a “wavelength” of 0.01.  If we divide the 48 fps wavelength by the oscilliscope wavelength and look for the remainder, we get 0.0008333.  This is the “distance” offset, which means we need 12 frames of the camera to get this distance mismatch realigned (0.01/0.000833).

Because the camera works at 48 fps, it makes sense then that this is what works at 4 Hz, (48/12 = 4, and do unit analysis to see that this is freuqnecy).

So we see chi2 and chi3.  Now we want to normalize this plot for field inside of the core and try to get chi2 and chi3 values.

Below are the fit function (in m/v)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-087.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-088.png)

Nice that we have these characterized now.  Lets do a quick simulation of how fields normalize with loss.  It is still tough for me to understand the bright dark contrasts we are seeing.

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-089.png)

There are using parameters that are quite real.  

Below I plotted something similar.  So it is possible that this is the cause, but I am not confident about it.  

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-090.png)

Could this be an explaination, yes, but I am not exactly confident about it, I can’t lie.  FWIW, the mode solver could stop working with very lossy cores.  Maybe I am in that regime.  I should ask Martin about this.  Either way, these are some nontrivial imaginary indexes.

I figured it out. B8 has a tonne of photo induced loss. I was only able to go up to notch 5 out of 6 before exposure got screwed

![Photo from Library.jpeg](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-091.jpeg)

This film generally seems more lossy. Kinda a shame tbh. But that is probably what is causing the loss shape to change a bit.

Below are plots of everything in comparison

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-092.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-093.png)

![Image.png](../../assets/fab/2024-7-16-srn-sweep-for-dc-device-094.png)

Not as helpful as I hoped tbh