---
type: craft-export
title: "2024-3-23 photoconductor and cladding thickness scan"
craft_document_id: 744EB8CB-D934-41A9-AF3E-559E1F0E32D8
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-3-23 photoconductor and cladding thickness scan
To write a complete slack post for the DC device parameters (and to inform which waveguiding core I pursue) I would like to see what effect the thickness of the photoconductor and cladding has on my device in DC.



For photoconductor thickness, the main idea is to see, if I use a photoconductor with a higher resistivity than the core in dark state (or bright state) does using a thicker of thinner one matter much in DC.  If it does not matter much, I can just deposit less photoconductor and not have to worry about saturation.  Below is a screen shot of my device

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-001.png)

We can try an etched version later, but for now, we are going to keep it unetched.  The period is 6um with a 2um bright state in the middle.  Below are the other constant parameters.  All the layers aside from the photoconductor are 1um



PC_dark: eps = 8, cond = 1e-11

PC_bright: eps = 8, cond = 1e-8

Clad: eps = 4, cond = 1e-10

Core: eps = 27, cond = 1e-10 (side note that we should scan over core eps at some point)



We will scan from h_PC = 0.1 um to h_PC = 4, with the steps of 0.1, 0.5, 1, 1.5, 2, 3, 4

As an observation, we really only see the contrast go down when the resistance of the photoconductive layer was comparable to that of the core (at 0.1).  So already we know 0.5 works.  Now lets try decrease the dark state conductivty to 1e-12 and see if we get the origonal pattern back.  This one is named with a prime.  It causes the pattern to come back, so there is NO advantge to using thicker photoconductor in DC. We will include the graph for this later.



Now laters do the top cladding.  I am going to to use the following constant values:



PC_dark: L = 2um, eps = 8, cond = 1e-11

PC_bright: L = 2um, eps = 8, cond = 1e-8

Clad_bot: L = 1um, eps = 4, cond = 1e-10

Clad_top: eps = 4

Core: L = 1um, eps = 27, cond = 1e-10



So we are not just seeing the effects of greater resistance as we increase the cladding’s thickness, I am going to make sure the ratio of L/cond_top is the same to keep resistance constant.  Below are the values I want to scan over

(0.5um, 0.5e-10), (1um, 1e-10), (1.5um, 1.5e-10), (2um, 2e-10), (2.5um, 2.5e-10), (3um, 3e-10)

Once I am done with bottom oxide, I will develop the nice graphs.  The basic takeaway, however, is that thickness DOES MATTER.  We will need to figure out a way of getting thinner top claddings at the least. For bottom oxide, we are going to do the same experiment with the same values scanned over.

The result, before formally graphing, seems to be that small bottom oxide thickness (below a micron) hurt the contrast at the top of the device.  As the bottom oxides get thicker, the top contrast is basically the same.  The lower contrasts, however, seem to get bigger.  This is useful information and says we want THICKER bottom oxides.  Lets do a quick test of what happens if we increase the thickess and conductivty of both claddings by the same amount (so they both change values as we scan but have same properties on top and bottom)

Scanning through (1um, 1e-10), (2um, 2e-10), (3um, 3e-10)

For refernce, SRN experiments have that in the same TO → top oxide, BO → bottom oxide, 2O → two oxides (what we are going now).

When we increased the thickness of both at the same time, while we saw the differing effects at the top and bottom flatten out, we also saw far less contrast (almost an order of 10 decrease from 1um → 3um thick).  We can still get a working device, but this obviously hurts.

Below are the graphes for SRN thickness

Top:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-002.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-003.png)

Middle:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-004.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-005.png)

Bottom:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-006.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-007.png)

Prime vs unprime

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-008.png)

So our earlier intiutions are confirmed here.  The thickness does not really matter once the dark state impedance dominates over the core.  So you can hace thin and insoluating and that is fine.  This is good news, as we won’t have weird saturation problems with something thinner.

Next we are going to do top oxide:

Top:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-009.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-010.png)

Middle:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-011.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-012.png)

Bottom:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-013.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-014.png)

This does confirm that our device does do better with a thinner top.  Now onto bottom oxide...

Top:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-015.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-016.png)

Middle:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-017.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-018.png)

Bottom:

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-019.png)

![Image.png](../../assets/fab/2024-3-23-photoconductor-and-cladding-thickness-scan-020.png)

As the marginal increase across the device is more limited than I was expecting.  Increasing bottom oxide thickess seems to help all levels equally, but the added benifit is a bit muted.  So we can turn this up, but don’t expect it to yield huge performance increases.  Obvously for a chi3 it will be a bit more helpful, but chi2 less so.

While we can try differnet conductivies for the top cladding to see if anyhting works, I am not super certain much will help.  If we get higher resistiance, then we over impede the stack.  If we go lower, we create a flat electrode above the waveguiding layer.

One possiblity here is that we are simply using too small of a period, and etching or using a larger period might help more.  This is possible, and we could potentially even etch the cladding down in certain etched areas to make sure we still get the contrast we want.  Nonetheless, that would introdcue all sorts of loss.  

Some follow up quesitons include:

1. Eps of core (should not matter too much as we are in DC, but worth writing down)
2. See effects of seed layer
3. What etching period is best (or no etching period).  See where we get best contrast and things saturate.
4. Whether we can use a thicker top cladding with higher or lower conducitivity
5. Effect of core thickness

The bottom three are probably more interesting.

