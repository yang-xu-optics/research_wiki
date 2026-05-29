---
type: craft-export
title: "2025-11-1 svm 10cm cw broadband poling"
craft_document_id: A47F76C5-1651-43FE-8F1E-955DBA0FDC6B
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2025-11-1 svm 10cm cw broadband poling
While the SRN3 waveguides showed nice broadband poling, there is some hope that SVM will show higher baseline conversion efficiency at the cost of higher loss.  So even though some of the shorter wavelengths may work worse, my hope is that we can demonstrate that higher Si-content can get higher raw numbers at certain wavelengths.  I already fabricated a SVM device with 12um of SRN8, so if any device can do it, it is this one.  It should also have a higher breakdown voltage.  So I think we can take it up to 12 Vpp at least.  We are going to follow the exact same alignment proceedure as before, and we will still try a broadband section.  Who knows, perhaps the higher slope efficiency will compensate for higher loss and make this overall better.

## Alignment

We start by coupling 10X filtered EMLO light into square spiral.  We use peak illumination power.  This is not a perfect apples to apples comparison, but so be it.  We see 2.5 mW out with asphere, which is roughly 2x less then before.

Initial vertical sweep

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-001.png)

After first certical alignment

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-002.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-003.png)

These are a bit high.  I am going to reduce the voltage to 0.4 Vpp.  There has always been a bit of an asymettry between hertizal and horizontal.  Perhaps it is hgiher now because of loss

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-004.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-005.png)

There is still this funny focal aberation too.  I don’t know why the peaks are so wide, but perhaps there is soemthing to be said that, having more background SHG and low voltage, it causes this to be wider.

Now lets move to the main spiral (5um).  We see 1mW out with 10x filter and asphere.  Closer to (but still less then), before.  A lot of this comes down to how nice the facets are too.

We see a lot of background SHG, so I am going to use 5V bias. This makes our background the same as before (and prevents too much saturation).  Now we want to align with the ciruclar spiral.  We should probably run a quick poling scan just to get an idea of what the best poling period is so we can align the illumination.  I suspect, because of loss, this one will be a bit more biased to the top.  I feel like a hand-alignment might also be fine.

After first pulse alignment

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-006.png)

Focus aberations are probably more of a camera thing.  We run the same range as before, so we can compare how much aberation there is.  Results of first scan are below.  We are seeing impressively higher conversion efficiencies right now, so I am hopefully (cautious, but hopeful). Top and bottom seem a bit off

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-007.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-008.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-009.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-010.png)

An impressive amount of signall, but we can do better.  I think the horizontal and vertical position of the illumination is a bit off.  There is also just a chance that, unfort, do do have some focal aberation near the bottom.  Lets try to better align the horizontal in code and twist the imaging light a bit.

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-011.png)

For some reason, I still feel like we are clipping the bottom.

I think the big mirror was a bit off

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-012.png)

After

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-013.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-014.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-015.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-016.png)

Bottom region still sucks, but we see less poling dispersion.  I say we go with this, and we can correct later.  As for wavelengths, lets start with the longest and work down.  We will only use just santec for everything.  So 1630 is where we start. 

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-017.png)

The above alignment still is not great.  I wanna shift spiral along the x=y axis

## 1630

Course alignment.  We do all optimizaiton at 9 Vpp.  Afterall, if it can’t handle this (with thicker SRN), what is even the point.  It is neat that even in these waveguides, there is a bit of background SHG

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-018.png)

We shifted spiral again very slighly, below is our alignment

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-019.png)

We use pp_temp = 15.1, and now we just run long man scan. This 1630 data was taken with 16 averaging for the most part (my bad), so the interference curves might look a bit funny

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-020.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-021.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-022.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-023.png)

I still need to realign the optics, and because averaging was bad, I suspect that the perturbative will help.  We also need the up the voltage.  So I am optimistic this is higher than before, but how much higher, I am not sure.  The ending points were with higher averaging, so it might be worth it is to do a second pass man scan, as I suspect some of these are not at their needed average

After perturbations

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-024.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-025.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-026.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-027.png)

For some reason, I still think the origonal man scan is bad.  I realigned the optics, so I feel like we should be close to the ideal point there.  Lets try one more man scan and see if it gets better.  For reference, we saw about 0.2 in the past.  So I still think higher voltage can get us there, but we are not showing demoninatingly better performance right now (as I really expected a factor of 2-3 better than this).

I think in the future, a problem I notice is the course scan sometimes leads more astray.  I think it would be better to just add a bit more resolution and range to the phase-pp scans.  At least, in our current system, if the ideal point is near the edge, one would figure that the perturbation scans would correct for that more easily than being far away (Where the loss landscape is more challenging to traverse)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-028.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-029.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-030.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-031.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-032.png)

The above image basically says, during optimization, it seems a few opints were found to be slightly off.  Perturbative is not really working, so we are going to use above chat to sorta predict where we could squeeze a bit more out of.

We now increase voltage to 12 V and get ready for final data.  Surprisingly, as we played around with things, we found 10V and 6Hz to be best.  Applying higher voltage actually hurt the system, and higher frequency could not account for it.  I suspect something interesting happens in the photoconductor. I was at least able to do a bit of realignment.  I see 17 mW out of laser and 1 mW out of waveguide

Forward Pass

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-033.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-034.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-035.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-036.png)

Backward Pass:

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-037.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-038.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-039.png)

Perhaps I overcompensated a bit with a loss guess of 0.55 dB/cm.  As this predicted more power in my waveguides than before.  While that is possible (as coupling efficiencies can change), I am personally a bit doubtful.  Better loss numbers would help tremendously.  This higher voltage effect is also kinda of annoying, as it really is make it more challenging for us to push numbers higher.  I will have to measure 1D waveguides on this chip to confirm things a bit.  I will also be curious to see how much background PGE we have.

Transfer Function

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-040.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-041.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-042.png)

After releasing power, we saw 1.4 mW out with 17 mW in. Perhaps loss is just lower.  Below is updated version assuming loss = 0.4 (same as before), with 1.4 mW in.  In the above, I used loss = 0.55 with 1 mW in.

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-043.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-044.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-045.png)

Suprisingly little difference. Lets move on.

## 1610

We will be doing all measurements, from now on, at 10 Vpp with 6 Hz

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-046.png)

After manscan

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-047.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-048.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-049.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-050.png)

Interesting how the end part looks.  I can almost feel some multimodeness in the middle.  I did an error correct that only made things a bit worse (unfort), but we will do a manual realignment and then proceed with final data.  Pert did not help

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-051.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-052.png)

Slight lower, but whatever.  No manual optimization and final data.  Funny enough, I found that 11.5 Vpp and 6.5 Hz to be best.  I found 1.9 mW out of the waveguide.  These differences in output power compared to the SRN3 waveguide are a bit annoying, as I can’t do an easy apples to apples comparison.  In theory, if everything is normalized, we are only slightly better right now, or we over-estimated the previous waveguides or underestimated the current ones.  A lot of this can simply be how nice the facets are.

Final data. 17.6 mW out of santec. 1.9 out of waveguide

Forward pass

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-053.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-054.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-055.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-056.png)

Backward

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-057.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-058.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-059.png)

From the scalings above, it is quite clear that fundamental loss is still a much bigger issue then SH loss

Transfer function

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-060.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-061.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-062.png)

## 1590

We do optimization scans with 10 V adn 6.5 Hz.  We will up the voltage later when we do the final realignment

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-063.png)

After man scan (we have not seen, up to this point, the perturbative optimizations help, but who knows, they might come through at some point, so we always let them go for a little bit).

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-064.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-065.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-066.png)

Pert scan did not improve anything.  We do slight realignment.  We also notice that interference fringes get a lot weaker as you go through the waveguide, so it is possible the loss is still fairly high.  There is a fair (though unfortunate), argument that we should try some shorter waveguides with thicker SRN8.

We see 1.6 mW out of waveguide.  We see 11.8 V and 6.5 Hz is ideal.  I think this small variance in voltage compared to before is reasonable.  I am still surprised that 1630 required so much less votlage, and it might be worth it to go back there at some point and double check.  It might also be the case that the photoconductor needs to be activated somehow, as we did observe those kind of effects in the past. 

Forward pass:

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-067.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-068.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-069.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-070.png)

I really just have to wonder, even on the bad peak, why we are always still out of phase.

Backward pass

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-071.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-072.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-073.png)

Fwiw, when comparing to the results on the straight waveguides, we get ~10x improvements on these devices.  In that sense, they are basically what we expected.  I guess the scaling on SRN3 is just a bit nicer (so added loss and higher conversion efficiency kinda cancel out)

Transfer Function

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-074.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-075.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-076.png)

eh, about the same as before.  We can start to see the effect of loss though.  Lets start 1570

## 1570

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-077.png)

Now we get man scan going from 14.6 to 15.05

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-078.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-079.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-080.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-081.png)

After Pert 

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-082.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-083.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-084.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-085.png)

Now we do some small realignments and take final data.  I feel like we are starting to see the effect of loss.  As a reminder, all this optimization scan data is taken with 10 Vpp and 6.5 Hz.

For final data, I saw 1.4 mW out.  I used 11.8 Vpp and 6.5 Hz

Forward pass:

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-086.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-087.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-088.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-089.png)

Backward pass (same dramatic backward scalling.  I fear this is only going to get worse as we go to shorter wavelengths)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-090.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-091.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-092.png)

Transfer function

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-093.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-094.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-095.png)

We kinda get bs too far away.  This is because of loss.  I can see we are heading in lossy territory though, and I think 1570 was right at the edge

## 1550

We only see 260 uW out, so we def notice the loss right now.  Once more, we optimize with 10 Vpp and 6.5 Hz.

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-096.png)

We now do man scan

![Screenshot 2025-11-07 at 12.50.37 PM.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-097.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-098.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-099.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-100.png)

This is like insanely bad.  Given that we expect the input signal to be comparable to before, this is some really bad conversion efficiency.  I am going to run more more man-scan, as some of the early points are uniquely bad.

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-101.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-102.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-103.png)

Above is after reoptimization with perturbation.  An interesting note is that we see decent scaling for forward pass.  This almost inciducates we are at a SH resonance.

We see 250 uW out of the waveguide.  I am going to assume a loss of 0.65 dB/cm, but it might be higher. We used 11.5 V

Forward pass

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-104.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-105.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-106.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-107.png)

Backward:

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-108.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-109.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-110.png)

Scaling will never stop being weird to me.  I may have underestimated loss, so we really do need a better loss measurement.

Transfer Function

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-111.png)

Waveguide got misaligned as I took power data.  I will need to come back, but it is very clear that taking data at 1530 would be impossible.

I think we should just collect some transmission data (get the loss curves), and call it there.  We can retake the transmission for above later.

## Final Results 1

Scaling

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-112.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-113.png)

Really notice the different scaling

Transmission

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-114.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-115.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-116.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-117.png)

My loss prediction at 1550 is bs.  We do show more light at the start

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-118.png)

![Image.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-119.png)

Below is full spiral transmission:

![27A93155-226A-4C1D-8C92-EB7F9D463C4A.png](../../assets/fab/2025-11-1-svm-10cm-cw-broadband-poling-120.png)