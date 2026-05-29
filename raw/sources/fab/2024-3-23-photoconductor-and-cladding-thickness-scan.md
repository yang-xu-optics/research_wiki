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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/3B35FA67-9883-4823-97FB-A475515EBE35_2/tfE6cCYx9wwxdW6mV468aKbjG5z5hYlF88hYOkDs7B8z/Image.png)

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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/065F6228-BBD0-4F47-BC86-93C37CE534E2_2/5W2gLzy8dHamNfFwePrfRlbfx2X9yhyUQokf6YCACGgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/675B504B-7A30-400F-910A-4BED65639905_2/ymundz5a8Zu9eVOqKh0xnEhynv1xaiDlqGCLukQhQzMz/Image.png)

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/68D22310-C252-4394-A233-8D7917954260_2/r9J1Q7IekUcdjjNQ6NNEokJzkfjUD6JN3vKnxhB2jgMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/F9F87C97-3EC0-408C-A4CB-04E2CC5536E1_2/Rt9PTzZL3uExPM2w6DhkevOMnfUbxYQMtz1Gvb6UwxUz/Image.png)

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/84D9CF87-F556-479B-B60C-2461F51F944C_2/LFEGy58bI3yFwY6V17HCxYSv6ej3mXdItw2zByrq5skz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/DA9C5D14-F2A7-4765-96EA-FEC03A0B62F4_2/c3CPyp6D4irZmVUjvXQcz9Irv5Re3xbwUu66g8ywCRUz/Image.png)

Prime vs unprime

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/CEEA0939-B8F6-4903-B10C-40DE45685DEF_2/x89OGWp225MsSLP8CknybLh9cComI8xGafIHqi7t0ZYz/Image.png)

So our earlier intiutions are confirmed here.  The thickness does not really matter once the dark state impedance dominates over the core.  So you can hace thin and insoluating and that is fine.  This is good news, as we won’t have weird saturation problems with something thinner.

Next we are going to do top oxide:

Top:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/F863CDAD-28EF-43CF-99C1-049BD7D40509_2/DEdkb8HLZFL9fYhuoAd8KqfYIePClSrAxjYDbRLFi5sz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/4C8D94FF-A8F3-44A2-BCF7-90BFEC51D6A1_2/cJcw4FnkU0EoIqzGuENJyGb6FqNBdIbhGURxhye1eL8z/Image.png)

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/61031796-B2C1-4821-BAEE-234F1AD24EE6_2/xGoxGJbUKU6vbllVyxcyAVZo8bTcDWJ0noNt7pXCUqwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/A4883C7A-0F5A-47B1-B297-4D2EA403E763_2/TTT7asMyMgBwxG35syBcFDxEZXxxuFCDEpAEsbVGDqEz/Image.png)

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/4814277E-1783-48F1-9442-F79FBC79A8F7_2/g0Z9G7gpWFm9vV82zHPVQBgK9DtPJcWfbF8H7I3Y6Iwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/2BAD0923-32C0-478F-BC9D-2724C5617761_2/HCUIB2tZjRtUscoUiSmdLOVGPUOHj6Npvqvw4QlMqVQz/Image.png)

This does confirm that our device does do better with a thinner top.  Now onto bottom oxide...

Top:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/786DB5D2-496E-459E-BB6E-E0AB2B2A88B0_2/xCqTFIEkLcmxyIV8SxD7GPOEibzOre2p3oy370bZkdQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/E0FC6A4B-D3CF-44D2-8904-4FC8E4AD3665_2/SUNUNgSBgwkYExSYWwPulTNJk1yISIhinvsK8H1l52Az/Image.png)

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/823273B4-2990-47F0-A37A-7E1C6F181C75_2/1xc7QbwCmVqKfvHTac0pjcZlsUUbmgD3Xs2I1QNHUygz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/3BB1AA19-2C50-4547-B35E-5B7E0B54BF82_2/yICOyigu48fahDh0ZpbFwbfp7yRj49vuJxx6B76GxRIz/Image.png)

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/102DE853-947F-4396-879C-8A806BA3AD2D_2/0CaD0uslNHM9NhsUvygOtpetGufBZCiYo2c1Em2Mnpwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/744EB8CB-D934-41A9-AF3E-559E1F0E32D8/047D96C2-4358-4F98-AA22-D1AA0B440548_2/CjYSXBVsunFWZuUfR2WCacgoQyl6HBaxmeYt0Ysswvcz/Image.png)

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

