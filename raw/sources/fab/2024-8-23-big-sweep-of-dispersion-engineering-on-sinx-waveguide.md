---
type: craft-export
title: "2024-8-23 big sweep of dispersion engineering on sinx waveguide"
craft_document_id: DA201A8F-E6B1-426F-AFFB-624B600DF00D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-8-23 big sweep of dispersion engineering on sinx waveguide
The purpose of this document is to show my efforts to do a large data sweep of etching for the nonlinear waveguide.  I now have code setup such that I can sweep height, width, and side wall thickness for my waveguide.  I now just need to put it all together.  I also want to simulate the effects on teh first two modes, as it is not quite clear what the conventino is for TE and TM in the simulation.  So I need to add a feature to the simulation to save the two highest order modes.  The other misc task is to enter our index data in for SiNx so I am not just using their data.

Last point.  I am going to scan 100 widths, 50 heights, and 60 etch depths.  I am just keeping it easy on myself.  I also want some varience so, if there are any dimension problems, I will find them.  I am also sticking to 3 frequencies.  

I am going to scan from 300 nm to 6 um for width, 300 nm to 2 um for height, and I am going to keep etch depth percentage at 75%

Mode 1 should be TE, and mode 2 should be TM.  We should be more interested in TM, as it seems to define the transverse direction in the x, not the y, direction

To put it mildly, the number of iterations above is just insane.  If we assume that each computation takes a second (and they take longer), then it would take 250 hours.  Not reasonable.



Lets try width = 20, height = 8, etch depths = 10.  This would give 20*8*10*3 = 4800

4800 / (60*60) = 1.8. hours.



The simulations finally finished!!  Below is the dispersion for full etching

![Image.png](../../assets/fab/2024-8-23-big-sweep-of-dispersion-engineering-on-sinx-waveguide-001.jpg)

![Image.png](../../assets/fab/2024-8-23-big-sweep-of-dispersion-engineering-on-sinx-waveguide-002.jpg)

And below is the index data for full etching

![Image.png](../../assets/fab/2024-8-23-big-sweep-of-dispersion-engineering-on-sinx-waveguide-003.jpg)

![Image.png](../../assets/fab/2024-8-23-big-sweep-of-dispersion-engineering-on-sinx-waveguide-004.jpg)

The index data does look a bit exotic.  Keep in mind, I did use the fit that Ryo provided for me

Below is the data from the default Ansys Lumerical SiNx model

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/36CD4792-AC43-49CF-B01B-1D3187740B43_2/Vxpts9XkdL6hbLQxpk5ArEmQFoNPTTCdIDyf1lrs9fAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/0A529188-F5AB-4612-8DEF-8990D7FA2059_2/kTicblBuz0v4gIYc8WdzNPkJTaxicReByp0DciXwlGkz/Image.png)

So there is really quite differnce netween ng 1550 (with the ansys material having this higher).  The ansys material also had higher neff as well for both 1550 and 775.  So something with more Si is not bad.

Below is the origonal Disperion plots with Ansys material (Full etching)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/91F553EE-DE5C-4722-8E9E-DBC07A222EEC_2/vm1OXVX5v94yZK71j7ygVstDiUnJxru8bpSfZPIUPpEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/97C207C1-99BB-46AE-960E-23638845F8DE_2/dyyQeC9taLrqZN4yyC3BiKftcCtzxEydUhMYu6nSqSkz/Image.png)

Compared to Ryo’s SiNx, Ansys has slightly larger poling periods, lower GVM (though this might not be true if we zoom in a bit more) and lower GVD (though again, if we remove the very thin waveguides, that might not be the case).

Above is for the TE mode.  When looking at the TM mode, we get something a bit different (below is index data)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/D28DBC0B-8390-4E0B-AA74-A86665D42A16_2/Wj8XWSZWLCrCjWDTe7R8xxIAlKl4ESsa63XHtzwRGTUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/A871B273-6282-4668-B6C7-CA4878360445_2/vOCJAQk24JRDY1jnzbRB57Xx1E21SHb2dh8ey0uygMYz/Image.png)

Below is dispersion

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/A28F9163-E366-4B82-88B5-ED910FAA44DE_2/X4dfJ2pY2Ru2bQ5zDmXIExyrwpcXSJsGjAxd6c669HEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/06AB95A7-AC19-4217-8512-C0BE77513D3A_2/YnPodzQTlzzC2TW98le1QakBDgm1ceVt8xDIXmXSzbkz/Image.png)

GVM looks similar to TE, same for poling period.  GVD for 1550 is really just a tonne larger (though it might just have an outlier). Ng 775 also looks a bit funny, but that might just be a nuance of the structure that I can’t understand.  Below is the full data for both modes

Mode 1

![Disperison plot for Height0.3.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/37335A48-F18A-4C98-BE58-5FF711B69133_2/byMoAcOZ4EGbQCYCrlnLKgwDDzoFy1wjMq1V5DPCZmcz/Disperison%20plot%20for%20Height0.3.png)

![Disperison plot for Height0.5428571428571428.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/CF3208A6-F21D-456F-8E40-6D070F97E760_2/FZUbgzXv0jNAbIoKXHJArOIQs3V4jeFOXVN43EwDCB4z/Disperison%20plot%20for%20Height0.5428571428571428.png)

![Disperison plot for Height0.7857142857142856.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/2AB67BB2-F511-4AE5-A5B0-D9FA7A88B47E_2/71HRlmgONOTcKFCSss0iWHYVwtYX8xFu92vNKYrYnAAz/Disperison%20plot%20for%20Height0.7857142857142856.png)

![Disperison plot for Height1.0285714285714285.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/CC2DBBE7-BB34-4053-9EBC-91E090C27653_2/4nKLspPtbJrnazKvTQzPmYy1C2UXyWyNsD4TCIfAC8Yz/Disperison%20plot%20for%20Height1.0285714285714285.png)

![Disperison plot for Height1.514285714285714.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/9FD73777-B8B0-4026-A057-3D370676130B_2/k57kPIyx6aHqx32x0833S0EXdEnihvASnxIVLQWf5B0z/Disperison%20plot%20for%20Height1.514285714285714.png)

![Disperison plot for Height1.2714285714285714.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/A3139AF1-ED94-4EC6-B286-4416DC3CBA59_2/vhP4FiBkGxbExhbXtkgdkQPHlhPO9LtlDLI86mXjaG0z/Disperison%20plot%20for%20Height1.2714285714285714.png)

![Disperison plot for Height1.7571428571428567.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/9241A6EE-6471-47E7-BB0F-4F3FCA4AA2B5_2/Uay8VdmzH0V6YnuMTnv5cqloRqvSsTsXrdxBy0k9CV0z/Disperison%20plot%20for%20Height1.7571428571428567.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/A488599B-484B-4D60-B1FB-72BE552741C7_2/XqgSYW2beTCaEiOg97ewnMkiwqg0eEQYPYRRIGP4TYcz/Disperison%20plot%20for%20Height2.0.png)

**Mode 2**



![Disperison plot for Height0.3.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/5F54A254-7B06-46BE-B16A-8FBD5A750984_2/xaimKKcaOpMDIOftxDhmpbBnybKTZymIiiidEDYDoR4z/Disperison%20plot%20for%20Height0.3.png)

![Disperison plot for Height0.5428571428571428.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/042503C8-E25E-4152-A042-6B346D15963D_2/DyGARWTumU7kBqBpTPztpy4Rx82rtyi9dwyhKJIaIFQz/Disperison%20plot%20for%20Height0.5428571428571428.png)

![Disperison plot for Height0.7857142857142856.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/63ED8242-5440-481C-A238-73A17C25FABE_2/Y0oKzRhXOMDQwq9JoThJKtYe6Z41KiMwR6yXJnnxxwcz/Disperison%20plot%20for%20Height0.7857142857142856.png)

![Disperison plot for Height1.0285714285714285.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/969E7D24-1902-4A06-A7EC-4AE6B94EFB2D_2/om9aQilxwXz4rQoBruy2coBjzGSt7PsNNcdMI6n35CYz/Disperison%20plot%20for%20Height1.0285714285714285.png)

![Disperison plot for Height1.2714285714285714.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/9C33C3EE-D33E-40B5-AC52-4A4F25623230_2/LYxjjw5cSJXoLUlW4xgA44TDOB5lXIS5YloLbT3dwP8z/Disperison%20plot%20for%20Height1.2714285714285714.png)

![Disperison plot for Height1.514285714285714.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/0AFD3955-9BE3-49A9-B8C7-C15A776101B1_2/SyKS6qYH9EENRQcyhpNV1IcsoLkAUldNhrj6baEl16Az/Disperison%20plot%20for%20Height1.514285714285714.png)

![Disperison plot for Height1.7571428571428567.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/D73BDC04-94FC-41EA-8F28-68A559BB17A4_2/krtJonI2HtbxIe12GAaxqlaWVT3io4SGPPdtMcmdjGMz/Disperison%20plot%20for%20Height1.7571428571428567.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/1E4222B0-CF21-4C93-A24C-CF29B513F2FE_2/3VEfAKj8Jqsbk2aSNOyWfyat6ysQiorRJCiXu5ldyjcz/Disperison%20plot%20for%20Height2.0.png)

The general trends I notice for Mode 2.  

- As the waveguide gets thicker, wider, or less etching, the poling period becomes larger.
- GVM seems roughly equal everywhere, as long as etch depth is low of the waveguide is wide.  Being a bit thicker seems to help as well
- GVD 1550 seems to have a sweet spot around height = 0.8. Affter that, wider helps lower that value.
- GVD 775 seems to prefer thinner waveguide

I think it would be best to cap some of these values, as I feel like our understanding is being hampered by a few outliers blowing up our data.

After bounding the results, we get the graphes below

![Disperison plot for Height0.3.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/781D8C22-6671-48ED-99E4-9251A7509F84_2/Dsl1RmOEbu6yqnShCGQcwOruIsyoZNyXf0xvlWaUyNUz/Disperison%20plot%20for%20Height0.3.png)

![Disperison plot for Height0.5428571428571428.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/0AE62BF9-BB19-475D-ADD1-520A57DAB042_2/pEAkOOxxjB4z9jQQLXMwbTe5dzj4M2qkFT7m6Wc4uDUz/Disperison%20plot%20for%20Height0.5428571428571428.png)

![Disperison plot for Height0.7857142857142856.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/DC2E87E5-A15B-4678-A2AF-992F43EB0644_2/9xQGJ7SHoA6tIoLWTBLu7hzyerzEFHgXXkFOK9j0JLoz/Disperison%20plot%20for%20Height0.7857142857142856.png)

![Disperison plot for Height1.0285714285714285.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/3F78F007-6541-46DD-B9B0-EA29B7042744_2/4WpKRSERvrJhTH6gWcrxhFcw9Z6nUpNkZoU8QvoMfv4z/Disperison%20plot%20for%20Height1.0285714285714285.png)

![Disperison plot for Height1.2714285714285714.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/422D1E22-A41F-4B32-8866-0C00CD4A9D56_2/FxyW0xvc61kKExWJUWvXJRxO32JiQxTaxakiZFHR0hoz/Disperison%20plot%20for%20Height1.2714285714285714.png)

![Disperison plot for Height1.514285714285714.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/61F39A19-1BB6-47D5-95AE-22E5E4FB5E10_2/91wUSHTOpEKvx0xSylTbPm6kA8xUFce1Pm3bvpYKvBgz/Disperison%20plot%20for%20Height1.514285714285714.png)

![Disperison plot for Height1.7571428571428567.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/0CC390BF-29EC-48F6-93A1-72E257087D64_2/J8apnR1y3glBKIlD68sWjK2AbnaIuG9SJDhEV2AppyIz/Disperison%20plot%20for%20Height1.7571428571428567.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/DA201A8F-E6B1-426F-AFFB-624B600DF00D/FDAC675A-8DDB-4E44-BD2F-D2C4E9B984A9_2/AW8NvDC9e0pfkwMirADhN60FY7kIxUHdXb19yZx2zcsz/Disperison%20plot%20for%20Height2.0.png)

These are much more useful, and we can really see the sweet spot here.  We want to work with a waveguide that is a micron thick.  There seems to be an umbrella feature that opens up where we get reasonable GVD and GVM.  The only issue is that the poling period is a bit small.  For thicker waveguides, while GVD gets fine, the GVM gets a bit larger.  Maybe that would be good for pulse shaping?