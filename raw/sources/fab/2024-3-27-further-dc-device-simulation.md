---
type: craft-export
title: "2024-3-27 further dc device simulation"
craft_document_id: C14D0783-8840-4D00-99A5-C6436FFEC208
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-3-27 further dc device simulation
The purpose of this document is to do some futher simulations of DC devices.  I am interested in seeing if there is anyway of tuning the conductivity of the top oxide (as it gets thicker) to try to preserve a working device.  The issue, as we noticed in previous simulations, is the thicker the top cladding, we losing a lot of E-field contrast.  We hope to see if there is anyway around this.

After that, I am going to simulate whether there is anyway to implement the 3-layer DC device Ryo and I conspired up.  I will also see if any additional top layers will help the device.  

For top cladding, we are first going to simulate the device with the following constant parameters

Core: cond = 1e-10, L = 1um

SRN_bright: cond = 1e-8, L = 2um

SRN_dark: cond = 1e-11, L = 2um

Bottom cladding: cond = 2e-10, L = 2um

For are going to scan over the ideal cladding conductivity values for L = 1um, 1.5 um, and 2 um for the top cladding.

For L = 1um, we scan over cond = 0.1e-10, 0.5e-10, 1e-10, 2e-10, 4e-10, 6e-10, 1e-9.

After a few simulations, we can clearly see that decreasing conductivity is helpful.  This means our new scan is 1e-13, 1e-12, 5e-12, 1e-11, 5e-11, 1e-10

Below is 1e-11 for 2um thick.  We get maximal contrast when the green curve goes through our middle.  This means we are not getting conductive flattening or resistive domination.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/70420503-0A61-4069-937D-75A1EDED8A80_2/I1mykGAQVeT5UXyqOt6hwPkBid0ddz6tRM5QAcerDFMz/Image.png)

The general trend seems to be that a facot rof ~10 decrase in conductivity for thicker films seems to work.  I am now going to do a sweep where the top and bottom claddings (which will be labelled with a BT) will have the same thickness (3um) and have the same conductivity.  I will sweep from 1e-10, 1e-11, 1e-12, 1e-13 to find the optimal spot.  The gist seems to be that we eliminate inwanted currents with more resistive films.

Below are results for my simulations

Bottom 1um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/B3CBEF98-B6E9-4CE0-B72D-349D8A3EB289_2/YE9kUlgllG4snUja7npsdgA5aMzoK17Ct9xqyiwc2bQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/3588FAAD-355F-4F87-BBCE-11F8B8401A27_2/9qWK2I8XNpYyraCsf82j93x2FxoGlxfsa9ki5sxDo5Qz/Image.png)

Middle 1um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/98789052-BA02-456D-B0F8-E242DB50377F_2/SGO4P6aAK0kONmpFUuLp1nY8Zvmtevlr7gpVsCy1zMcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/FF3415EC-E6BB-469F-B6DB-739CDB89004B_2/6F1HyQtOF1nz5DJscXHkdX3vyLOoEWh42BoZ8ngxn9Yz/Image.png)

Top 1um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/F032B9B7-2FB2-4BFA-9B72-93901748E9CF_2/4aZMyxeDZgg03r6G4yPcwUvGOQkK4RnFLP4yLr1bmtEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/A6BAE294-B228-446E-86D7-2A9DA17D95C0_2/GlidcZMSy5G5dxwPcMFGNWYTiW8UkGNcJR0vFo246dsz/Image.png)

Sorta what I expected.  Matched resistivity for the baseline 1um thick top oxide is the expected result (though I do wish I had looked at slightly higher conductivity numbers to make sure)

Top 1.5um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/0E757500-D984-4D5D-9741-2917E523DE35_2/4sqcDY33oYBzE3B3xhATFJNXBMUB01VGSm6E6gGFQrkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/33A34B83-C3A1-4108-8EA2-7BE5DADF69D6_2/GN3gxUuxEqmTTmmVU6H7vsdxg2vKgCar7cF6B3uLNEAz/Image.png)

Middle 1.5um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/4B0D5FF7-BE8C-4CFB-A924-94941CCC7BED_2/16RaIlUXLsNz267mAOxnaMKKsXTHpsE3yNanM9Tw3nAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/4805E26E-9F93-4886-8662-B5621897471B_2/Xtk5cASLYhxLOJysFKyM1JJlJ364kwRgBIcoFMn5vLUz/Image.png)

Bottom 1.5um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/0B867DAA-8DC5-4444-BDC6-C50DFCDF009A_2/Ue8t7TxNox8NOGw6GLW0nxVQ8G6aw85HzC9QpfnlMjkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/0A35EFDA-91F2-412B-ACC1-DE84F4F30940_2/EUQRTQxjL16IDHrnZbHHDej8x1gqDTjLDj1UnhJ1hHQz/Image.png)

So, once more, the matched conductivity works the best.  A bit suprising.

Bottom 2um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/C3FD7CE8-F3E8-457C-A6BD-0AE6A4EB5914_2/sKz9cl3ZVbXHhLsNLqovSKMnSZfbaYQ4BbFjxgQbmSwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/4AE265B6-112C-4C58-9561-247A85126141_2/KvU6bA0PLe2Wa5xl2Q8FNNdahPdWOe9Uub8syxAybCkz/Image.png)

Middle 2um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/D22B7AEE-2F03-4B7B-A59E-41A7F7E3EDD4_2/yqQMeSqJCiTfJI7GM67m65druI0iToUxPyEeG8Stp78z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/25949966-3C55-4733-9676-E9EDCA945EA6_2/ODQf0BZO8AR6z8JZeMuTNLyZBlZ1GHmrdr0otHcw91Az/Image.png)

Top 2um:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/E6F45DC2-43D7-4799-98F5-92CE3E042208_2/vUZBYULQcE4xMJxuTuejCuTbn7cr9MZFGQtW9sR4oZIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/BA253403-2854-4F95-A298-6D518B123979_2/sX5fp2LaG4smvacHAIXiiIgYfWRax5CJR3dEhoGrnRAz/Image.png)

Lets do the three cases for 1e-10 for the different thicknesses

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/9B2898DA-BE89-416D-8F1D-F9E01A3D4856_2/ri7LYWuziiMf2TQdEy6mzoEKEUa1uNoTfl3DGQkPunYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/48E6DB9D-8E49-42AE-AA11-4B85FD84255F_2/PBl7PX6yqDSVyYlCc2i5FqPQ2KxpmY8lXMSiwQaa7XYz/Image.png)

We still confirm the same result from last time.  

Below are the results from the 3 layer devices

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/1DE6D364-FC6C-4B3C-8D7B-D9A8DB2E7857_2/gdyKr7r6wMgbZjyyK94P5q5Gq0zGYFk1UTswusVO5L4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/AED15078-6398-4935-B631-79DA46EFAABF_2/YpBwrY06ey38T5FkZ4FgyQkWpyETlQnnFFsk7VqWxV0z/Image.png)

These are for the 3um top and bottom claddings.  Notice the above plots are not quite linear

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/FEAF4E89-47F2-4450-AFE6-854CAD8747A9_2/aPxeAWrUxeqDtnOhuKHlBhptxxhP8OtNW9DKLgSOpOgz/Image.png)

Above is the more linear plot.  Lets try some higher conductivties for the 2um device.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/2CB14046-1A19-445A-B2EF-05A1DBFF42B2_2/fRhyLQPqRxiNAhTUBzy17cYtXnABrRlfRhoDfNyy6Qoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/36670635-0717-4F45-A506-935BBEFADBE8_2/PuBxZF5qW9DA1co7P2JticmypFwoAU2nxK4DGC41IY4z/Image.png)

So ya, it bascially seems like there is no way to get around the problem of thicker top oxide.  We really do need to have the same resistivitiy.  

So this puts to bed the hope to get a useful device with a thicker cladding.  Lets now simulate the three layer device (possibly with an added fourth photoconductive layer ontop).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/4B131D08-88E9-4D1B-B9F6-40AEBDFA8663_2/uxyQ4WqkOcQDUGHPZHVLndJDvXEqXvFSwwLhnyKhQEYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/306D3705-D336-4DAE-B06C-70A2A58FF832_2/wE5dGDHy0f688ZDDv4Pcmxc9JKwuyLnnxIyvcWsgKo0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/4B7E72AF-54F8-4BE0-A374-99115E94207C_2/vJareyXtkDoaRiEibK2yixLK0WIXFiJqU8TdnNa4oT8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/C8FBE896-9E42-4E29-A4A9-92F5FB2CAE58_2/6uJRH3xPfJQdByYpK5Iy75NF9t02UB3tT9OUqshkrA0z/Image.png)

Here are the parameters for the above device: 

Top oxide: cond = 1e-10, L = 2um, eps = 4

Core_dark: cond = 1e-12, L = 1um, eps = 8

Core_bright: cond = 1e-8, L = 1um, epes = 8

Bottom oxide: cond = 1e-10, L = 2um, eps = 4

I am overall very happy.  As DC devices go, this is really as good as the contrast will probably ever get.  There are still some werid corner effects and I can’t tell if they are numerical aberations or not.  Either way, I will try to export this to python so I can take more cross sections.  We are both interested in core and cladding field, as both will give some nonlinearity.  Thinking about it, if the claddings display some amount of DC linear behavior, I could also get effective delta =_n from cladding getting bigger instead of core getting bigger.  After all, both will push the effective index in the direction I want.  This is just such an optimal device.  I just hope no loss.

Below is what happens when we export this data to Python:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/9B26BF04-A0EF-4536-81D9-6A44D8F377E7_2/ZxroJGiDYYvlx7aBvhVimzdatgo6enfSg6yhnfS1zNYz/Image.png)

So I pretty much match what I see above (we can disregard x and y parts of field, as they really don’t matter).  Below is the X field

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/97998B64-6BAA-4AF9-A456-DF32BBF17F78_2/bwixoIvhWPStJ4Bu3FhNzVtFHFGIyfzaopwdnAGZrJ0z/Image.png)

Below is Y field

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/50CAF888-1484-4D1D-9548-4071181365C7_2/QYKvNywrJEexcxUgzYRRI8U8JVtwT3tFxIkxC5IQ0Osz/Image.png)

I think Y is a bit scuffed.  X does have a bit of field along the edges.  This might be important to share in the future. 

Below is X field where you can see the sign.  Z field is not effected

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/6659933F-9D4A-4142-A81D-B2D30F430BB7_2/MJyt7WXnJ7Pym9jX9Dm8wugIYjetRj2JGAcl0CuaMe0z/Image.png)

I have defined the positive z direction as down, and positive x direction as to the left.  Just a notational thing

Below is the high resolution version

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/2E5299DC-D3E3-4074-9698-DCF58CA38D6E_2/wjsqQGBaLDGwoOnu7bNPCYdtUj8ghXU43AVAKxFRHJIz/Image.png)

Now lets take a few cross sections.  Please refer to the above image for the scale of each of the axes.  I am also going to ignore the bounaries between the layers, as that introduces difficulties.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/2427DEE4-FEE9-48B4-B805-A87D50FCF6E5_2/ne1I1OxDrpfpAoJ7KSX0EjkwCAFEdx0abud7kHqAdTQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/0C4ECA38-0BDC-4635-AB1A-6785852D903F_2/pdvy4D4TfXy02PrnxlR61twdcJnf6uyfmGCyl6zOp34z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/FB2DC39D-4B55-45EE-8AD6-3647F992DA4B_2/yilXUAqqnzvTuW5OW9z51Xlj7wZamSaZTypeBzRHg8Az/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/966E01FF-4163-44DA-B282-158380FA67D8_2/C9dFvIJchoyoiHIixBtZA625s1M8J14nsqJGzcbkJoEz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/8CA2C35F-587F-4719-9618-C12B6CE328D0_2/cedG56d6UgnNtgJHmp3wXujYvEFp0X2emS64Fy3vxisz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/9D8858BE-6488-41F3-91DC-6C9ADAD044F6_2/yDRore04QZt04LjXjp790cZMjQCJp8OUSVqxiogTrQoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/F1EA5890-4E8A-48C9-8A42-954ADB8DADD5_2/ZPxXAaqGSbRnfksxMVRChu5QFZv4bj3aimINqNMkBOMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/4450AC2A-C342-49D9-AFFB-2E3F2B90BCBB_2/Z4LItwnROIkTu0KCCCYLXflLPdFYB7bHY3CmNW5tAMMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/C73DE173-87FF-41E7-90DF-622DD595CC1E_2/Y5uIMQMZzajt8rcbWRBKQYRKCrwwnmWYW6CzRqB2PxUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/E7320824-07AF-4382-90CE-604D35B2055B_2/tN7jRbHkbunHDko2rui54m8UqZ5WYVnRkbxVntH7omsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C14D0783-8840-4D00-99A5-C6436FFEC208/61F19664-3D2A-498E-B8C5-A691F79B6CAD_2/kNmZo18msmNDggJRBIitU52oyIuTtudsmlwOzQTkdmcz/Image.png)

The core has a very nice looking field.  It is about 100 times less in the middle, which makes sense, as that is the ratio between the cladding and bright state conductivity.  The contrast seems to flatten as we move further from the core.  We get some weird effects near the corners of the core which I am not sure I understand super well, but a lot of field seems to get there.