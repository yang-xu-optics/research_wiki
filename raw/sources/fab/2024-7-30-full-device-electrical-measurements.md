---
type: craft-export
title: "2024-7-30 full device electrical measurements "
craft_document_id: 92D89D26-9B1E-4C14-BB4F-CE5BCF156D0E
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-7-30 full device electrical measurements 
The purpose of this document is to record some full electrical measurements I take of my chips (test pads for DC devices). The hope is that this will let me characterize the conductivity of the layers (specifically the SRN) in my stack.

First I did SRN 6.5. Here is a picture of the data 

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-001.jpeg)

The spike for dark resistance is basically when we started to get data points. Looks good enough to me to save

The chip

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-002.jpeg)

0.4 by 1

SRN 7.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-003.jpeg)

Bottom one. 1 by 0.4

Result

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-004.jpeg)

SRN 5.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-005.jpeg)

Top one. 0.4 by 1.2

That chip broke, so below is pad 2

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-006.jpeg)

Triangle, so divide by 2. 0.7 by 0.5

Result

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-007.jpeg)

It will def be hard to get dark state data now

SRN 5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-008.jpeg)

0.4 by 0.8

SRN 4.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-009.jpeg)

0.3 by 0.7

SRN 4.0

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-010.jpeg)

Top one. 0.9 by 0.4

SRN 8

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-011.jpeg)

0.7 by 1.4

SRN 6

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-012.jpeg)

Failed because it broken down very early

SRN3.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-013.jpeg)

0.6 by 1.8

I could not characterize because it was too insulting. Either way, we have enough data 

After referencing, I see that everything is a factor of five too conductive

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-014.jpeg)

It is kinda weird that our resistances are so off.  factor of 5, but still, as I am using the same values that I think Ryo uses for the same oscilliscope.  We will def need to investigate further the deal with the dark state as well giving huge negative values.  Martin had a good suggestion that I should save the current traces (though, if my eye is to be trusted, I don’t think that will reveal too much).

Likewise, when we fit our data with our predicted fit function, we don’t get a crazy result in the sense that the shape works (below is bright SRN 6.5)

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-015.png)

Below is the fit function

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-016.png)

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-017.png)

So the fit is werid.  The scale factor implies that some constant terms that we have are off by a factor of 1000X.  This is suprising, to say the least.  

I got the doped oxide values from the plot below

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-018.png)

The units above seems to be working.  Again, this really comes down to some issue with the L_SRN, L_clad, or area terms, and there does not seem to be much.  This would imply that the resistance values are fully off.  So we have a good start, but there are some starting terms that we are struggling with.  

Lets think a bit about what we expect the other values to be.  Firstly, the 

I figured out the issues with the ref resistor. Vr is 400, not 200. Now it works

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-019.jpeg)

I also figured out the bright dark issue. Basically, the no voltage current is slightly negative (probably something parasitic). As we increase voltage, we see the current go from slightly negative and get closer and closer to zero, at which point it switches. So maybe we subtract this baseline? Either way, the measurement is legit.

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-020.jpeg)

New data for 6.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-021.jpeg)

After plugging our previous data for SRN 6.5 (taken properlly) into jupyter notebook, we get the plot below.

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-022.png)

Overall, I am happy with this fit.  The good thing is that we get cond0 and slope that are roughly what we expect.  The voltage to field factor is somewhat acceptable.  Remember, E = V/d.  D here is ~1e-6.  So we should end up with something on the order of 1e6.  We end up getting ~0.66e-6.  So actually a bit smaller, but on the order we expect. I still can’t explain the added scale factor issue.  This still suggests that we are 1000X too big on conductivity, but I referenced everything and we are definately not.

I just did a quick check, and the fit is indeed quite sensitive to all these values.  So these seem somewhat accurate

SRN 6.5 bright

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-023.png)

Another fit that works:

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-024.png)

So I got rid of the scale factor.  It is impossible to dark for dark state because it is so resistive

Now our code is working and I believe we have a good method to analyze stuff. The key here is we basically have to let the computer fit for both the SRN and DON conductivity. Let’s retake our data (besides SRN 6.5, which is good)

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-025.jpeg)

Chip is 0.4 by 1

SRN 7.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-026.jpeg)

Bottom one. 0.4 by 1

Ref:

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-027.jpeg)

Overall, good

SRN 5.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-028.jpeg)

0.7 by 0.5, but remember it is a triangle 

SRN 5.0

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-029.jpeg)

0.4 by 0.8

SRN 4.5

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-030.jpeg)

0.3 by 0.7

SRN 4.0

![Photo from Library.jpeg](../../assets/fab/2024-7-30-full-device-electrical-measurements-031.jpeg)

Top one. 0.9 by 0.4

SRN 7.5 Bright fit

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-032.png)

SRN 6.5 Bright State

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-023.png)

SRN 5.5 Bright state

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-033.png)

SRN 5.0 Bright State

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-034.png)

SRN 4.5 Bright State

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-035.png)

SRN 4.0 Bright State

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-036.png)

I think the most disturbing part of these fits is that we basically see that the resistance of the DON layer is the one that is increasing.  This is really not supposed to happen. Overall, it is really tough to say how helpful these fits are.

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-037.png)

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-038.png)

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-039.png)

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-040.png)

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-041.png)

What is kinda wild about these fits is that if we switched the DON and SRN layers, this would make a lot of sense

![Image.png](../../assets/fab/2024-7-30-full-device-electrical-measurements-042.png)

Interestingly, if I switch the layer which I linearize off of, the nature of my fit changes to make sense.  So It seems that we can reverse the titles above (though I will look into the nature of my fits later)