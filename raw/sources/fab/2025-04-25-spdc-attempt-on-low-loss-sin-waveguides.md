---
type: craft-export
title: "2025-04-25 spdc attempt on low-loss sin waveguides"
craft_document_id: 5D1104D8-6C8C-451E-B605-71D4687AE89A
craft_collections: [dc-device-full-fabrication, etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-25 spdc attempt on low-loss sin waveguides
[`Fri, Apr 25`](day://2025.04.25) note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-001.jpeg)

We test the waveguides fabricated in [2025-04-18 Etching Full Spiral Device with CHF3/O2/N2 recipe](craftdocs://open?blockId=57996FC7-96C4-412F-9D45-00B42342483C&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8).

# E-FISH measurement

## Elmo

We first couple ELMO in

We see 1.85 mW / 8.3 mW = 1.85/8.3=0.223 transmission. Not a bad number for ELMO.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-002.jpeg)

Electric contact established.

We move to SHG characterizations.

Note that we have both ND filter and the dichroic on the way. We apply 3 Vpp,

![2025-04-25-ELMO-baseline-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-003.png)

![2025-04-25-ELMO-baseline-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-004.png)

14.1 um

Realigning the setup. We found the horizontal alignment and focus of the imaging was off. Setting the bias to 0.7 and taking data again.

![2025-04-25-ELMO-baseline-aligned-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-005.png)

![2025-04-25-ELMO-baseline-aligned-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-006.png)

Higher order peaks are suppressed

## Santec

### 1570 nm

We have 15 mW coming in

![2025-04-25-santec-baseline-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-007.png)

![2025-04-25-santec-baseline-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-008.png)

Optimizing the signal

![2025-04-25-santec-baseline-realigned-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-009.png)

![2025-04-25-santec-baseline-realigned-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-010.png)

Signal level is much higher. 

#### The side peak indicates that there is an issue with the imaging. We want to fix that in the future!

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-011.jpeg)

### 1616 nm

Changing the wavelength now.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-012.jpeg)

![2025-04-25-santec-baseline-realigned-1616-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-013.png)

![2025-04-25-santec-baseline-realigned-1616-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-014.png)

Optimizing the signal

![2025-04-25-santec-baseline-realigned-1616-fine-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-015.png)

![2025-04-25-santec-baseline-realigned-1616-fine-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-016.png)

Power: 3.7 mW / 14.4 mW = 3.7/14.4=0.257 

Now, with santec installed, I will try to couple the maximum amount of light into the fiber at 1616.  Once this is done, I will optimize coupling for 808.  At that point, we already know the back side is aligned to capture 1616 well.



---

### [`Mon, Apr 28`](day://2025.04.28) note added by [`Ryotatsu Yanagimoto`](craftdocs://users?id=aa2c0de3-4c5f-8aaf-eaf7-3b949f6279ad) 

# SHG

## ELMO

We couple 2.2 mW / 9.5 mW = 2.2/9.5=0.232 

Bias voltage 0.7

![2025-04-28-elmo-baseline-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-017.png)

![2025-04-28-elmo-baseline-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-018.png)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-019.jpeg)

## Santec

We now combine the EDFA to amplify the signal

![2025-04-28-cw-baseline-1570-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-020.png)

![2025-04-28-cw-baseline-1570-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-021.png)

Optimizing the coupling

---

Somehow, things got misaligned. Need to realign the coupling.

## ELMO

We see SHG. 0.7 Vpp bias.

![2025-04-28-elmo-baseline-2-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-022.png)

![2025-04-28-elmo-baseline-2-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-023.png)

We see more power but this is without the asphere.

## Santec

![2025-04-28-edfa-baseline-2-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-024.png)

![2025-04-28-edfa-baseline-2-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-025.png)

Using EDFA

We align the imaging setup. It seems quite sensitive, which is a good news. Got some nontrivial improvements.

![2025-04-28-edfa-baseline-3-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-026.png)

![2025-04-28-edfa-baseline-3-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-027.png)

It helps to first set the poling period to a longer side and optimize the SHG

![2025-04-28-edfa-baseline-4-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-028.png)

![2025-04-28-edfa-baseline-4-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-029.png)

Further optimizing.

![2025-04-28-edfa-baseline-5-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-030.png)

![2025-04-28-edfa-baseline-5-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-031.png)

A very beautiful sinc! Extending the scan window.

![2025-04-28-edfa-baseline-5-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-032.png)

![2025-04-28-edfa-baseline-5-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-033.png)

### Vanilla Santec　

We now remove the EDFA. 

![2025-04-28-santec-baseline-1570-1-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-034.png)

![2025-04-28-santec-baseline-1570-1-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-035.png)

### 1616 nm

![2025-04-28-santec-baseline-1616-1-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-036.png)

![2025-04-28-santec-baseline-1616-1-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-037.png)

Good curve.

Optimizing the coupling.

![2025-04-28-santec-baseline-1616-2-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-038.png)

![2025-04-28-santec-baseline-1616-2-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-039.png)

The power is good. Even better than 1570 nm.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-040.jpeg)

12.3 mW / 2.2 mW = 2.2/12.3=0.179 but the power was measured with the 780 nm gauge 

For fiber coupling, we get 250 uW with single mode (with 800 filter 177 uW). The multi mode has almost no loss (so 2.1 mW). The method we used we collimating each lens to infinity, doing two beam overlap on mirror close to fiber objective and output waveguide objective, coupling into the multi mode fiber, and then slightly perturbing to get into the single mode fiber 

We now couple 800 in, being very very careful not to mess with fiber alignment. We can break 1616 input alignment, as we no longer need it 

Below is power with red light

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-041.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-042.jpeg)

We see 19 mW input power from laser

With 450 mA on laser, we get 166 mW 

20 mW after the waveguide with red light on. So no burning, as this is consistent with 10% transmission 

# SPDC attempt

We plug directly into SPAD

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-043.jpeg)

Use ID Qube as software. Box behind is how you turn SPAD on. We set voltage to 7. SPAD takes a while to turn. 



---

[`Tue, Apr 29`](day://2025.04.29) we will start from recovering the baseline. We first couple the ELMO laser into the chip.

# SHG

## ELMO

Used for alignment. We took away the dichroic, so the signal is brighter.

![2025-04-29-elmo-baseline-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-044.png)

![2025-04-29-elmo-baseline-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-045.png)

0.4 Vpp

## Santec

Moving to Santec with 1616 nm pump. No filter on the way. Previously, we saw 0.017.

![2025-04-29-cw-baseline-1616-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-046.png)

![2025-04-29-cw-baseline-1616-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-047.png)

Signal is a bit lower,

Optimizing the imaging setup a bit. Not a significant improvement, though.

![2025-04-29-cw-baseline-1616-2-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-048.png)

![2025-04-29-cw-baseline-1616-2-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-049.png)

Turns out that the vertical alignment is also important.

![2025-04-29-cw-baseline-1616-3-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-050.png)

![2025-04-29-cw-baseline-1616-3-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-051.png)

Signal level increases. We move on then.

14.4 mW in, 4.3 mW out.

4.3/14.4=0.299 transmission. Pretty good value!

# Spectrometer

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-052.jpeg)

Aligning

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-053.jpeg)

We measure the spectrometer output

![2025-04-29-calibration-multimode.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-054.png)

Single mode fiber

![2025-04-29-calibration-singlemode.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-055.png)

Wide range calibration

![2025-04-29-broader_scan_1550nm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-056.png)

![2025-04-29-fit.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-057.png)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-058.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-059.jpeg)

After coupling Santec through waveguide, fiber and spectrometer, we get

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-060.jpeg)

We have 4.5 mW out of waveguide and 1.5 mW on spectrometer.

# SPDC

We couple 808 nm light in.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-061.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-062.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-063.jpeg)

450 mA pump current.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-064.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-065.jpeg)

Make sure that the Santec is off!

Connecting SPAD to the spectrometer.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-066.jpeg)

7 Vpp bias.

![2025-04-29-SiN-fluorescence-no-poling.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-067.png)

![2025-04-29-SiN-fluorescence-poling.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-068.png)

We see fluorescence..

## Scan

![2025-04-29-SiN-SPDC-base-period.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-069.png)

Switching between two poling periods. We then reduce the pump power a bit.

![2025-04-29-SiN-SPDC-base-period-3.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-070.png)

![2025-04-29-SiN-SPDC-base-period-down1.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-071.png)

![2025-04-29-SiN-SPDC-base-period-right1.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-072.png)

---

# [`Wed, Apr 30`](day://2025.04.30) Stimulated emission tomography 

# SHG 

## ELMO

![2025-04-30-elmo-baseline-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-073.png)

![2025-04-30-elmo-baseline-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-074.png)

We optimized the alignment of PMT

## Santec 1616

![2025-04-30-cw-baseline-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-075.png)

![2025-04-30-cw-baseline-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-076.png)

Optimizing the imaging 

![2025-04-30-cw-baseline-2-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-077.png)

![2025-04-30-cw-baseline-2-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-078.png)

12 mW in, 3.3 mW out. Coupling the light to the fiber. 1 mW fiber coupling seen.

![2025-04-30-broader_scan.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-079.png)

![2025-04-30-fit.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-080.png)

Calibrating the spectrometer

Pump light wavelength: 804 nm

1/(1/804-1/1630)=1,586.586 

---

# Continuing on [`Thu, May 1`](day://2025.05.01)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-081.jpeg)

1586 nm we see 1.1 mW after the spectrometer 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-082.jpeg)

k= 0.0216

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-083.jpeg)

![Drawing](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-084.jpg)

We use A220TM-B for the 804 nm

![2025-05-01-calibration-singlemode.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-085.png)

![2025-05-01-fit.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-086.png)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-087.jpeg)

We have 6.3 mW coupling through the waveguide.

## Fluorescence characterizations

SPAD connected.

![2025-05-30-SiN-fluorescence-283mA.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-088.png)

Fluorescence level 

Reducing the pump current to 200 mA

![2025-05-30-SiN-fluorescence-198mA.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-089.png)

Less photon counts now. We keep the pump power here.



Baseline: We send in -10 dBm Santec power at 1630 nm. Pump power is about 200 mW. Poling period 14.18n um. We don't see difference in the signal level.

![Image.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-090.png)



Taking SET data

![2025-05-30-SiN-SET-Pseed=-10dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-091.png)

With -10 dBm, we don’t see anything. The average photon count is around 8 k/s.

![2025-05-30-SiN-SET-Pseed=0dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-092.png)

We don’t see it at 0 dBm.

![2025-05-30-SiN-SET-Pseed=10dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-093.png)

We realize that the alignment was off between the waveguide to the fiber. Realigning.

![2025-05-30-SiN-fluorescence-198mA-after-alignment.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-094.png)

The fluorescence level decreased. We optimize the coupling at 1586 nm.

![2025-05-30-SiN-SET-3-Pseed=0dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-095.png)

![2025-05-30-SiN-SET-3-Pseed=10dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-096.png)

Repeating to see if the features are real.

## Realigning

![2025-05-01-cw-baseline-1586-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-097.png)

![2025-05-01-cw-baseline-1586-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-098.png)

1586 nm SHG. It felt like we were coupling into the photo conductor mode. Now it is well aligned.

![2025-05-01-cw-baseline-2-1586-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-099.png)

![2025-05-01-cw-baseline-2-1586-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-100.png)

More signal now.

We have 1.4 mW after the waveguide.

We make sure that the coupling is into the right mode. Using SHG. The SHG power is good.

![2025-05-01-cw-baseline-3-1586-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-101.png)

![2025-05-01-cw-baseline-3-1586-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-102.png)

We see 1.85 MW after the fiber. 4 mW after the waveguide. 13.5 mW before the chip.

Coupling 804 nm now.

2.7 mW / 40 mW coupling to the waveguide. 

We now move to fluorescence characterization.

![2025-05-03-SiN-fluorescence-206mA.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-103.png)

Poling period has to be somewhere between 14.095 and 14.18. We should scan 0.15 around 14.18 um.

We find that Santec causes scattering and saturates the detector. Instead, we increase the pump power.

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-104.jpeg)

Attenuator.

![2025-05-03-SiN-fluorescence-450m-Aattenuated.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-105.png)

We reduce the fluorescence counts.

![2025-05-03-SiN-SET-Pseed=-10dBm-0.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-106.png)

SET attempt. The signal level is not high enough. Moving to -5 dBm.



---

# SPDC attempt with 785 nm light

[`Fri, May 2`](day://2025.05.02) we installed the 785 nm light source. We would like to get the signal at 1540.

## Baseline

We use 1540 nm for the SHG. 

![2025-05-02-cw-baseline-1-1540-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-107.png)

![2025-05-02-cw-baseline-1-1540-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-108.png)

Optimizing the signal.

![2025-05-02-cw-baseline-2-1540-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-109.png)

![2025-05-02-cw-baseline-2-1540-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-110.png)

1/(1/788-1/1540)=1,613.723 

1.1 mW coupling to the fiber. 2.3 mW after the waveguide. 1.1/2.3=0.478 coupling!



Wavelength of the pump is 788.

## Seed

Seed wavelength is 1613.7. 

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-111.jpeg)

![2025-05-02-cw-baseline-1-1614-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-112.png)

![2025-05-02-cw-baseline-1-1614-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-113.png)

Aligned

![2025-05-02-cw-baseline-2-1614-peak.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-114.png)

![2025-05-02-cw-baseline-2-1614-peak-normalized.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-115.png)

## Alignment of the band pass filter

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-116.jpeg)

We maximize the transmission at 1540 nm. Maximizing the coupling to the fiber.

## Pump coupling

We see 4 mW out for 55 mW in.

# SET

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-117.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-118.jpeg)

![2025-05-02-SiN-SET-Pseed=-10dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-119.png)

![2025-05-02-SiN-SET-Pseed=-5dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-120.png)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-121.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-122.jpeg)

![2025-05-02-SiN-SET-Pseed=0dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-123.png)

![2025-05-02-SiN-SET-Pseed=5dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-124.png)

![2025-05-02-SiN-SET-Pseed=5dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-125.png)

We see the signal!

![2025-05-02-SiN-SET-Pseed=5dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-126.png)

Peak seen

![2025-05-02-SiN-SET-Pseed=8dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-127.png)

To reduce the saturation, we add a 10x filters.

![2025-05-02-SiN-SET-Pseed=8dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-128.png)

We see better SNR.

![2025-05-02-SiN-SET-Pseed=10dBm.png](../../assets/fab/2025-04-25-spdc-attempt-on-low-loss-sin-waveguides-129.png)