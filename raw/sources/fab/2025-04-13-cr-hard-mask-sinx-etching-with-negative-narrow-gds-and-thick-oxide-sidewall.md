---
type: craft-export
title: "2025-04-13 cr hard mask sinx etching with negative, narrow gds and thick oxide sidewall"
craft_document_id: 584C0829-76D8-4C0C-8630-7D82F8DA350D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-13 cr hard mask sinx etching with negative, narrow gds and thick oxide sidewall
Despite many hours of hard labour, we have not totally perfected a device for bends.  We have roughly discovered the following:

1. We need thick sidewall oxides to prevent outcoupling from the sides at bends (in the form of radiative losses)
2. We need shallowing bend radii and narrower waveguides to prevent leakage out of the fundamental mode
3. We want to use a Cr hard mask for now, as I suspect that 1813 resist masks are tough to remove, and we would just like a working device

See [2025-04-08 Negative Narrow Snake and Sprial Etching](craftdocs://open?blockId=5D47CED5-2FA4-452E-8329-2745A412C448&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8) and [2025-04-07 Special oxide deposition and etching for reduced bending losses](craftdocs://open?blockId=CC67967E-0650-4044-8C24-17BF920C8645&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8)

Below is the GDS file we are going to use 

[pad4 pass1 (positive).gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7B23CCF2-B6B5-4235-B49B-B37E97FF444A_2/kQQouzZimxAR5jyM8RtC44yh8LhCuLJNrrHJTowjpOcz/pad4%20pass1%20positive.gds)

[pad4 pass1.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/3BA20ACA-285B-4A72-96E0-96CFE6E927AC_2/v20eG8FBcyZvziodJt7VTvzgCR8zWt20Lx3cwLmFfxwz/pad4%20pass1.gds)

![Image.png](../../assets/fab/2025-04-13-cr-hard-mask-sinx-etching-with-negative-narrow-gds-and-thick-oxide-sidewall-001.jpg)

The process steps are below:

1. RTA clean of the SiNx.  This improves adhesion for later and removes any dust that could cause loss
2. 300 nm pad oxide.  This is protect the SiNx from the hard mask (might be worthwhile for resist in the future too).  This requires 1:15 high rate oxide deposition
3. Cr hard mask sputter.  Requires Cr sputter for 1210 seconds at 7 mTorr of pressure
4. Resist coating.  Spin P20 and 1805.  Use 3000 rpm, 8000 ramp, and 45 seconds coat.  Bake at 90 C for 1 minute
5. Exposure on MLA (using the same GDS as before, attached above).  Use a dose of 53 and defocus of 1.  This is a bit of a guess, but we saw that our previous structures were 700 nm too narrow
6. Develop on hamatech, using 726 for 1 minute (recipe 4)
7. Resist descum.  Clean the 81 or 82 for 5 mins and do a 50 second descum
8. Cr etch.  Season the Pt 770 and etch for 8:30 using the Cr etch recipe
9. SiNx etch.  From the previous fabrication run with a full wafer, we guess that we should etch for 11:30 to get roughly all the way through the SiNx.  Of course, we don’t need to go all the way down.
10. Strip Cr hard mask.  Put in Cr etchant for 20 mins and do BOE dip for 15 seconds
11. Cleave out 2 pieces. Do RTA on the chips.  Do 650 C for 3 mins with 20 C ramp
12. Measure the loss of the waveguide
13. RTA wafer.  Do 650 C for 3 mins with 20 C ramp
14. Smooth oxide deposition for 3 um of oxide, and then oxide etch in Oxford 100 to thin the top
15. Measure the loss of the waveguide
16. SRN deposition
17. ITO sputtering
18. Measure the loss of the waveguide



---

# [`Sun, Apr 13`](day://2025.04.13) CNF process

# RCA cleaning

Temps when RCA got started

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/95D3757B-7D80-4E4B-8BB2-E49B085B2172_2/WiSOvl31haNWUTzUswEHVzyFua3VwpKWhRPQ7zFy3yEz/Photo%20from%20Library.jpeg)

I am going to Cr hard mask two wafers in case anything goes a bit funny

# PECVD for pad oxide deposition

## Cleaning 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/A06C4E9F-D40A-43A0-9656-6A355F7A164C_2/LTUv73ehjlYSiqHhGOahESWFjTyXrOmNACDjlOH7g0kz/Photo%20from%20Library.jpeg)

Previous user did some cleaning 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/DC575331-F18E-495A-A0C0-C1EEE054DE35_2/jgi9kdECoakcE7ZmRJy2azk0RlpyS06XePGXUAa9zh4z/Photo%20from%20Library.jpeg)

We do 10 mins cleaning to be sure

9:35 Done

## Seasoning

2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0C855A57-B467-40D0-B7BB-C76D34D74A9F_2/l2yblOMZUM6fdFWSrUz6dMeunE6grppMkodX6Fumxbgz/Photo%20from%20Library.jpeg)

9:38 Starting

9:44 Finished

## Main run 1

1 min 15 sec

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2F3B4554-AC80-4E3F-82F1-212E14F61B49_2/aGIZCkbGDwPv0Yp8oJpFg72lXrn1fspE7j5IcmjfAvgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/819E6CCE-81D1-49C1-B016-37B5A025BFFE_2/phq9I87vcrAfAKby7kED5kKi2xyUvmHW30KRHcsYsdwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/DFC3733A-3C2A-465C-8E64-C485FA35EC55_2/CSVMa5YxkXqMutYyjyXfBgXr5wIPtQhstyjqoPILFEoz/Photo%20from%20Library.jpeg)

Starting now

9:46 Start

9:52 Finished

## Main run 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7226711A-1F20-4A22-A6F1-7787C9C7ED23_2/KnRaGdmw5W6Mv7wEuZ3ywcvtuXUg5WDmXG4DYbfK9yQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/E3CC7063-A4F6-4650-9646-59E3AFBB910E_2/AjRkE3y6aZiXAwMBFk62SVG1sL8yE8y0Wv52eVAhyxgz/Photo%20from%20Library.jpeg)

9:55 started

10:00 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/AF0C11C6-4825-4E02-8547-7FE666CA8D83_2/4K1opml5OEMDCxA9HqvdXddB0tpvjxjSZvMwGjzqt6cz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/A85BC8C8-2218-42C5-9877-2446D866F8AF_2/0BgjfQ8AFRZXYnqcIski1mMMSL4vc41yz1gno1DZzWsz/Photo%20from%20Library.jpeg)

## Cleaning

15 mins

# Cr deposition with AJA

## First run

Recipe for Cr depostion

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/DF4F773F-D5F1-4DAC-8FD1-7382F386AF8D_2/4yicxUBkSsnEvgBdqUB1V32fG5met0Xta1wPNLQqSvkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/F8C2726E-82BC-461C-8320-58707A53E318_2/e2FTsNDqtNEzIVXoZ2yXBxAQDOUILMOQvILQlyzMruQz/Photo%20from%20Library.jpeg)

Pressure when loading

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/4DFE9B9E-72CA-4930-B508-B54A70A39659_2/DaYuSHrpRuqAxCH0ayfJ2i2nZpEdUhWCEjzpmZczBPAz/Photo%20from%20Library.jpeg)

During depostion

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/1AD686C9-B2F3-4BC1-BEEB-290C928848AA_2/Ooyn4OIxLFyLpt75g5ZFaiYkJ7d5emyVze68FKBBaU0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/9C666FA7-8239-4592-B092-6BBAE02F9BEF_2/xh24Eynzfot3yq0mMyHi9Si9qLkc8PT0tyB3HDXFC3Iz/Photo%20from%20Library.jpeg)

10:26 Finished

## Second run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/C9BFEB27-A520-42D3-B682-596042C76266_2/IhVKajcDycUryIfoPFpsB4nf8E9WtWeH0p9jT5n4ps0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0E6D95B5-E2BC-4EC1-A51D-4EC99E17525E_2/U3yJvVCh9Jc68tAXLKeQ8RL5jYKmxL3HbdMtpx3mSloz/Photo%20from%20Library.jpeg)

Pumping load lock 

We wait till the pressure is below 5e-5

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/3EA2E2F9-A548-4E63-90BA-135D7B74EE08_2/EQt1Xb7MyixvmVsNxxqDMxCjNOOc1O2F2gAafK1DzTgz/Photo%20from%20Library.jpeg)

Cr in the target

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2232554D-09D0-4440-994F-391207A69767_2/iSKNQ1fRyx660zjwC4ySoD22rEMUxL5bEnQTc8WJN3gz/Photo%20from%20Library.jpeg)

Now the pressure is low enough

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/94923F76-450F-48C5-B8BC-6872A801FF74_2/DGBusJwV4xrxwYSABU1DOcIsx019PLc5jCwvJO6K4pYz/Photo%20from%20Library.jpeg)

10:38 Closed

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/4CBC78A7-CD3C-446F-9937-7595BD40B7C2_2/KgMO84zpd2olQNAnioyNbF0Qk6R8TwcFHCHxxsycq2Ez/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/A6B6E68A-E7EA-4312-A0AC-525A4C82286F_2/EWmxmy0ANyGOMyRH5xFfXJVVUGjpuqLxYoFdJGFgxyIz/Photo%20from%20Library.jpeg)

Error showed up, but this is not a real error.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/041963FF-4CEB-434F-9A3E-8A0E7B048AC9_2/6qyVaDZDJxF03AGEoQQTPiPhSYvbhpkckmaoc5T5Qdkz/Photo%20from%20Library.jpeg)

10:41 Cleaning started.

11:05 Finished

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/901C2A2D-661D-4F3E-B51E-7F838C603155_2/tQy2OZyfOXxW3Szvi97cMf3gx2U4tTAxfJ2cQ4qNi3Mz/Photo%20from%20Library.jpeg)

Closed

Venting the load lock

11:10 Pumping

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/B22C927C-213A-4352-AF90-6BA0CEDD7D96_2/Uff1cyrgC1RLNJ1rn7qYnPLsS9AYq9PL3eJZUORe3Qoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/08D2A7E5-3051-49FC-92E7-818F6ACC3E56_2/HDrVfMS9tHFT3ioxVgvPHcRdXJedA54nByjkg1rijXwz/Photo%20from%20Library.jpeg)

# Photolithography

Below is recipe we are using

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/6513221B-36E2-4F1F-9A37-DC0A291F31B5_2/hfwBWL5r2FCQqmdCQnDHN0y71cUIiB5wsi2oGlDyNqUz/Photo%20from%20Library.jpeg)

Now baking

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/6702AB21-0318-49E3-8684-6423C862A46F_2/8loe9YCeOC1IcJNhN5Z33Al1hzUyJ4p5KYqZXUnvmXAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/D774191E-7196-4A96-A857-EC80DC30B73B_2/bWDq1Z7kyQIebEalDLFCgQxYtxaX21V6CoyitytI2L4z/Photo%20from%20Library.jpeg)

Now mla

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/09394FD7-D56C-4706-9558-069FF5E1ABC2_2/NG4ravpyZVfxXoQckF3w5U6hG7U4OIk9WRAkLAtex6Mz/Photo%20from%20Library.jpeg)

We will use dose of 54 this time and defocus of 0

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/77EE4164-2C50-4515-8CC3-AA3808A5EA33_2/pIlxXSAU9B5nkxjVf6La7y2yYvx98E1zKrQSI2qhDl4z/Photo%20from%20Library.jpeg)

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0A070356-3BF8-4CE1-92C9-79F4B0CE1C47_2/ssRBvrTHNeVCUE2nNjfux7j2xPjDLiHiKvPTRBuquZcz/Photo%20from%20Library.jpeg)



# Development

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/BFED37AE-DAEE-40E1-AFBB-B30DF9FA55DD_2/amAbHfWTzCVpELtAyCsAQicFxwDjwJIsj8V7vsT2HEwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/587F4838-7FBB-4F30-A6D2-D72744655608_2/2wHC8fZki9xgFhaQmiblE3t2ipvIY8f0L9NqI8cWbGIz/Photo%20from%20Library.jpeg)

# Oxford 82

5 mins pre cleaning

## Cleaning

11:40 Loggiing in

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2B72DE38-0220-4563-B8C2-B7B709F3276E_2/WoQpcWn8hHXomEu8xWTOA1iv3KkwzHW0rHKkjKCF57Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/9E2823B7-2187-43F0-BE24-A04B4D11916D_2/4gDgZGi4pP2qWoe92wpzPWl9Tc7BQPTU0Bh1pU1SeYEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2260BFB5-DA0E-4C80-8DB5-67E18A04421F_2/0blYFKh4G23zn5v4jW3F7zf0xyGAyx6xPle3yjRK7RIz/Photo%20from%20Library.jpeg)

5 mins cleaning

11:47 Finished. Venting.

## Mild descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/F495340C-6E35-4234-B403-C093D4A64790_2/hVMMBxvgvjfdrMyCnIvERZ72HUlzmym1IgwNZ8mn83Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/99B17F7B-F5FD-40FF-90B6-4C147DF34744_2/OJiyIr2ef0sN1wFTcqaLP4PgrDCpSvRaAYcONdQM5eYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/C580215A-52C9-49A6-BB77-8B644E320A2B_2/49RXtcaK5iTI5Xiwd5Mqt79TRTGtnyXh7o7blKeTlmcz/Photo%20from%20Library.jpeg)

11:53 50 seconds. Starting.

11:55 Finishes. venting.

# Microscope

![20250521-5xbf.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/275AFB10-5C91-4DF7-B652-A108AA71D4C4_2/U2ODhnfiVxxN8S8HrNkRibnCN5OSMPQhOOIuHsnouqgz/20250521-5xbf.jpeg)

![20250521-5xdf.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7C61FB56-BF99-437E-B20F-F04C882E07FB_2/dVOFmcZbSrX9dZGMjs0zc3BCyNUMY5yO11w6Rr6dObEz/20250521-5xdf.jpeg)

![20250521-20xdf.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/8A6C7611-CFE4-4D8C-BEA0-3A1961BD4BAA_2/yMWIykWnyfbJXMekHlIuykD8mzptxrlaIfAHWLgYxvAz/20250521-20xdf.jpeg)

# PT770

## Seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2F4589FD-525E-4E31-BFD6-ADC012DFFDCE_2/eiCV5n380xVMbemXEpZ9vBiY3nZ2FJitCiCu46cepxoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2D178481-225B-417B-AA39-CF6E67809E1D_2/yKAIRLubCuwegmZGhh6bvADz0wBQ4Z1T7n40QXpQP1gz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/3CBE39EE-BF5A-48DA-96E1-AAF0D3C8D254_2/3mG5Qrz3BydQ5qIvE7ejeLaAlNJ5bh37E3mLp2yeRTQz/Photo%20from%20Library.jpeg)

## Main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/81F52B2D-4DF8-4BA9-B761-0326A6D7D62B_2/DUf8nlG9LMrY17Sm8mCywgq3DKhDyFjSxbWNInkNvzUz/Photo%20from%20Library.jpeg)

During etch 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/DE880C75-277A-4403-935F-FBD2F02D5DDC_2/SxpXApgEaaD3xNqAWi6NvUW6Bqku8dydS6tfA3J8Cxoz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/B206B8B4-C7DB-4E26-8818-A98A2921B040_2/6sFwbelZ05mtFb64W4BCrIjbVi1pG0F4eDEKidrE8RMz/Photo%20from%20Library.jpeg)

# Oxford 100

## Cleaning

Running 15.5 minute pre clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/865C4D9F-BBEA-4A5D-92BF-FB715D90C0BD_2/lWDePLb5VONwnMKGyIZ6gKWnPhYr1c8Juy8xwFyp0Fwz/Photo%20from%20Library.jpeg)

During clean 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0AB1319C-2B7A-48B0-984C-FA66D35930A3_2/1EGvO8E80ScYwoEwcXU8k0kNNZWNnCE4fxI9GwInhOEz/Photo%20from%20Library.jpeg)

## Seasoning

We do 2 mins seasoning.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/A6883974-C755-4572-91FD-D66A11214AA1_2/T5xR9p4DhB7KbAIvvbmszMUdf4hwGRktCDh3RZJrGnUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/B70AAC85-A85B-4823-AF6B-D6C2EDC7F30E_2/MPeknI0A4BDdwkUwdnZJXv3FNrbUOGwrAZ9hJwub4NEz/Photo%20from%20Library.jpeg)

12:28 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/A0E130CE-266D-4002-A111-0941AFE4B380_2/60a2BjfPWEj9wRyYLmENMF9E2g0Cg7iAAVI52xR60mwz/Photo%20from%20Library.jpeg)

The He flow is a bit high, but not going beyond 5

12:33 Finished. Venting.

## Main run

10 mins 30 secs

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7CEDA2A1-B37E-4B39-A6F2-FDBC19020214_2/lPxvhxy97C2xupde6CxqQULw5K98Bp8GXLKYyTptt1Qz/Photo%20from%20Library.jpeg)

12:37 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/411E2944-F57C-4102-8427-5C06B24C8E51_2/i5MZaRjCwIQ0FrCTWtVNDGgi33SzA9vFN7Kkg9mXxkoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/73A5E808-82DD-43C2-AB85-41F3DCB58805_2/Zs5dpHLP2Y2vFrZRJGyqYtCu8AAOFm3GUd2HIty8n90z/Photo%20from%20Library.jpeg)

12:53 Venting

## Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/54EC6A2F-06F5-4F62-9E27-CAD1366DBDE7_2/byWENUU7jJvVGCrW2DFDn2BX30PQkYXy3VmPZpvGRjEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0B1B5710-1A32-408E-97B9-35B96BC9B5E9_2/nqMQiMSJOCKJwY7i5k3GFymp150lNaccyTMPji6WUtAz/Photo%20from%20Library.jpeg)

15 mins

12:58 Starting

# Microscope

![20250413.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/C598F9B2-DD85-4BC5-B644-50A77B3F7245_2/LHzZESyUs7RGir5jejSmvzjK8BrV3bGaa1upbZOCe0gz/20250413.jpeg)

Etching introduced quite some dusts. Hope they clean off by the Cr etch.

# Cleaving

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7C4B4704-DF25-45F1-AF06-F9FA4DF216C9_2/MRg9hHXtfhjuP3QvEj39M08JyQBB48y6PqCag36LHtkz/Photo%20from%20Library.jpeg)

# Cr etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/60993077-0BED-4B43-9D29-9BD50BCB110F_2/8y8B0aPLV9s77VN28A5VkylcPHvzQ8UU3HjoyNLEHDoz/Photo%20from%20Library.jpeg)

13:11 20 mins Cr etch

# Microscope

![Frozen.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7D51B67F-674C-4534-9DB1-47A0CED318C3_2/GSE7hOYB6W3yhfFVaU5j9uOg6PftwcEzP8HXmvScEwwz/Frozen.jpeg)

Dusts still around

# RTA

Calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/236CF92C-8440-445A-B71C-2343F5858A5C_2/hCpNHlkhJmvELl9abdhvuw1DZKCD94aLVxp7xWCE6yQz/Photo%20from%20Library.jpeg)

Overshot a bit, but that’s fine

Main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/19568D1C-78A9-42D2-8941-E20A94BA3E86_2/JdaPBcgueASWmRyuy2iyuy2P6vnTRw01wGcfNQytLtUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/DD38473C-DE3C-4794-BF73-1D6A8CCD2B6F_2/NfSMsI8em4RxBP5xVAB8khJxZ6RZbyEHMwSXNTHeViIz/Photo%20from%20Library.jpeg)

---

# Loss measurement

## No RTA

### First straight

2.7 mW / 49 mW= 2.7/49=0.0551 

### Second straight

4.1 mW/49mW = 4.1/49=0.0837 

### Third straight 

4.4 mW / 49 mW = 4.4/49=0.0898 

## RTA

### First straight

0.09 mW / 49 mW = 0.9/49=0.0184 

### Second straight

0.092 mW / 49 mW = 0.092/49=0.00188 

### Third straight

10.4 mW / 49 mW = 10.4/49=0.212 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/CD30EA03-7BBF-4107-8E27-F796990D4C76_2/4v8N6NyH6jpk4j20ZyYIHyOEcjEwxQzE4I54d2liUSsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/FEEBAD87-4612-4DB4-B7CF-3BE4724935F7_2/9nyEIhXyCT4kxORaiWy02PvxbgobxdjNWJOQo3BNx3kz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/FDC34073-BD58-41CD-9D2A-31EC94883112_2/5kM79HQyFqynmqFF6vCWK32SXCyFVZMpuT38d7uUbBMz/Photo%20from%20Library.jpeg)

The coupling is a bit more critical, but we can find good modes

### Fourth straight

10 mW / 49 mW = 10/49=0.204 

### Fifth straight

9.6 mW / 49 mW = 9.6/49=0.196 

### First snail

0.029 mW / 49 mW = 0.029/49=0.000592 

### Second snail

2.7 mW / 49 mW = 2.7/49=0.0551 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/714D7EF5-BE99-4FC0-B450-76ECD658CEA5_2/KivlwDcxvyJ0TBlfzf9hw1lnoxYbDMip4Cl5zHC7xJYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/9B949C7E-CE1A-4D98-81DF-2A0752F93CCB_2/5kyu5XoG740kT3MTduws9ExjXxD8OOjfm6IEBAGqDJAz/Photo%20from%20Library.jpeg)



---

### Second RTA

Calibration run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/74B576A3-8998-4EF7-B7A2-D36C64D2B057_2/QKAfuhCqx2rm7cnEWnbIaBNVlbBRa05IaIl5LHh0a6Ez/Photo%20from%20Library.jpeg)

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/DBC9DB73-7FA2-4CCB-BB98-98B8AB415FEE_2/CVS3FMGwovLkmTF3iEHWyDa4f3597WoQkGTfyA3pTwAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/5499F05B-7621-4420-90BB-42D903997023_2/LtjbvuqgCpTJ3n7swQc0RfD9bratkSgaQNd7DyNmWYEz/Photo%20from%20Library.jpeg)

Small piece

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/4AB6AB3A-E50F-4A8E-A864-CB2EC21D6F9F_2/KrUeHJCHzp0ZhxEBo9u6yTSv3D5VdHny6TRUiv47xWYz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/982E05E3-E95F-4644-BDD7-C6B86292E037_2/kst6QErSGMmAX17eyW3EQrkxZ2jkyEp9M59YLqxYnukz/Photo%20from%20Library.jpeg)

During 800 calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/1A7B4CFE-BA2D-45C6-9839-29A5FDE032EF_2/amyA8fRgndKVTGibP1WYYeNw6HJyclO51gAJqim9hKkz/Photo%20from%20Library.jpeg)

During 800 run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/20AFEA16-746F-44E8-B208-CA8F21816005_2/RNDFwybJPxhkQ8paEqSJ6eurx8RZdUJB9FkemwNvRIUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/02ACD352-E5F5-430E-A647-4CAFA2DFD3F3_2/PBZkyImGfttpLoKTyL15nZI7cSdkYrQlgXKvEcPXMsAz/Photo%20from%20Library.jpeg)



![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/C9C6F0C9-7DE4-42A0-9D1D-4D2DE0AB64DB_2/p6znWaCAx6TgDw0017miuAK4aCFJJv99IWk2vbj6azEz/Photo%20from%20Library.jpeg)

# PECVD

## Cleaning

5 mins

Done

## Seasoning 1

2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/FB9CC044-DC43-4641-BC04-1958F1E33630_2/vbbEu5AfrbGJ5RMBJrTlMyFrKAIV6qCyHybnpqlAyTEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/AACACEC2-FD9E-4C46-B164-E9490BABC251_2/JFnUrTZU1IVza7oazkxgwaLDmm6pjbWrFzpyxGmdOiUz/Photo%20from%20Library.jpeg)

17:08 Starting.

17:15 Done



## Main run 1

As shown in [2025-04-08 Negative Narrow Snake and Sprial Etching](craftdocs://open?blockId=5D47CED5-2FA4-452E-8329-2745A412C448&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8), we do 9 mins 6 secs to get 1.5 um of oxide.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/F4AA2370-BB2C-42DF-B367-83F9CE8192D8_2/lu2sQuSxCT2yknRxt20bIvx5zh2dwxMMi4ZiCKdcIFoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/E9C99108-71A7-4F06-9E57-FB6093B4B2CD_2/Ezbuequpv1p2geuTuGEKWTdpVayATJ8VAU14xluwKB8z/Photo%20from%20Library.jpeg)

17:18 Startng.

17:33 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/D3C0D8D4-7ECF-47A4-9EB2-926CF54B8DA6_2/KXYrGbcjoevbyCXLxLSmr436Kky7ie6xkqPxHy7j1xgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/98191F1E-A929-429F-AE31-CFD5469D08E8_2/9MuqxhjthUmteZvqBYmDcTzFZd73R4zVUDrm49Eyid0z/Photo%20from%20Library.jpeg)

We got 1.5 um of oxide. Almost as expected.

## Cleaning 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/5E27DF15-EAB3-4786-97FF-929C05AFC714_2/voyzUk7iAs6YdhZApwa11aOus4QJVcAJyHvsgNxj1zkz/Photo%20from%20Library.jpeg)

17:36 Starting. 11 mins.

17:50 Done

## Seasoning 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0399F1C2-D953-4327-B7B5-BDEF81726C4A_2/VGKi9lkHXXOTfouliZMiVY3oWymbM0ls4oFNwvz4Vtsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/D8C68396-3722-4263-988A-33B9A51D75A4_2/lCvpK1RLuRccQObuzmykOJ2usKyezGS5a6X0dfU65GUz/Photo%20from%20Library.jpeg)

17:51 Starting.

17:58 Finished.

## Main run 2

9 mins 6 secs.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0F3FB9D6-D28D-467F-9E27-A751177AE0A7_2/3YJJ4mu3Nf1D2RqWLSLDIu2xlG6s8Yrj3Sb9vfFAwiMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/716FA0D8-D66B-40B2-BA78-2A76377553A9_2/JvcmfK9wwiCbed54mNT61giThM0dl2ea3EON66RTZQgz/Photo%20from%20Library.jpeg)

18:15 Finished.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/A5E3FC8C-600F-4D91-BF04-995833FC6070_2/WYe1R9VpKY9XRsY7HGsLEXWpl4fnEb17PBTbU6arO3Ez/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/8C5347D1-BFB1-41AA-8B4A-E4959894620A_2/kuNOFFvCnDyvydg2MpxAmGwNjtaHeyyiN47Wvbyxo4Uz/Photo%20from%20Library.jpeg)

We got 3 um pretty accurately.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/CF04BA08-2F6B-440D-BD20-740B48108084_2/yUFxOpcY2fFvyXhQhLz3wxh7mu6D3OVYjDprJ9IRXtYz/Photo%20from%20Library.jpeg)



## Cleaning 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/F0C578E2-2DD5-4BBD-957F-A55B56836274_2/xeufV2KjiCPyMl29PCv5moQOWYBIMhFeX8Uq7zMEXEcz/Photo%20from%20Library.jpeg)

18:18 21 mins. Starting.

# Oxford 100 for oxide etch

![Drawing](https://resv2.craft.do/user/preview/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/FC8ABC7C-ADBF-4A26-8282-6660BA83E292_1/5rPri9RdwrOU2KhpK3UJmZKzjqACjauwwwxWiCbRqhEz/Drawing.jpg)

## Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/51FD2423-FCD4-4B73-A95E-816033BE735F_2/UkcgWpUEkI4YFbcBYkedadT1MLkzFtsB9CvN2RAWVjcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/9EE8B255-EDF0-4CE0-A727-80BF740C6DC3_2/t4F7Btr870DOc5cR7XedzM1kpIyaPGypB0qrFZTOxb0z/Photo%20from%20Library.jpeg)

20:48 10 mins cleaning

## Seasoning 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/03A114B3-49F3-4356-A871-26E6A760CCF2_2/kU7YhFNwhthI8v8awSn6ELSG3nQrv8JUvvAO3pmxGKMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/2F0A250A-1364-4AFD-9C45-96EAFDB925E0_2/DXIhtykSnBQKMxmejtuj6x4r3JWQlhtYjRlNEgiyjR4z/Photo%20from%20Library.jpeg)

21:02 Starting. 2 mins.

21:07 Finished.

## Seasoning 1 redo

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/04EEEA3B-38E2-41E5-A132-4D05F56DAC57_2/VazKvc65yMvJ7sLF3MRsVs3pxZA7lm0Z7pJUSPEqyVEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/8D826256-F6BF-459B-9CF5-07F909B53AE9_2/sRBvWOVWmkpXiAa7IkE0VleogLBOg4w333jkEkA953wz/Photo%20from%20Library.jpeg)

Just realized we did a seasoning on a wrong recipe. Doing it again.

21:14 starting.

21:21 Done.  Venting．

## Main run 1

Following [2025-04-08 Negative Narrow Snake and Sprial Etching](craftdocs://open?blockId=5D47CED5-2FA4-452E-8329-2745A412C448&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8). We do 12 mins 45 secs etching.

![IMG_0601.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/55859EA8-E1BB-4EA5-A8B1-217930058C79_2/yZmONyVZhd040e6MXakK1yWbqtw9b0VsjNk3YGmFA4Ez/IMG_0601.png)

We use witness samples to characterize the etch rate.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/E55DAF7D-A53A-47DD-B0E5-7C17EF27ED57_2/hBMlx0dE1nBAxvcI7XD2H1D1C776iidi1Gdivc8yXbgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/254FAB5A-1394-4194-A371-FA9FF650A9B2_2/wFYTu1vlmh84YmF7ss33huIzZZjIxrUu3Qyb1KuHkR0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/0E15C72C-07B7-4743-AE6D-43D68D94CD86_2/w9xEFcz2i4NjeZzX2ox0txO4w2hsgJA0dOQDs1AkWwQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/800B0757-5ACA-4358-882A-1E3D3CD68925_2/u1YgizCgCje3yy8AG3MTwHxCP6ya6rg7vF3HILVKdvYz/Photo%20from%20Library.jpeg)

12 mins 45 sec

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/89EC8F9D-0496-487C-B863-88D8D1CD0487_2/uHQhVs4i62We6FlPZmJwJQHFPGtLoCvPxmB9d9TFoHIz/Photo%20from%20Library.jpeg)

21:26 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/020FAF2F-951B-46A6-89B1-DDA343250DAC_2/WFghT4x2XaM5ZNKvvx1pMbSV5CXNJX6nFv0NCR7Nzewz/Photo%20from%20Library.jpeg)

He flow is high. There may be some He leak.

![IMG_0603.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/F3FA845E-787F-4459-B2A6-F506FD2D5D17_2/fKKxBKWJG1AMOu9ehqgGL71GFyp2mRGsWM0o7DcYlWYz/IMG_0603.jpeg)

There’s some bad-looking mess

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/7A6C6477-C746-46B9-9C7A-7D2BD20D0DCB_2/4ZVNxq28VaM3Vo5xth7aFxWyvSadLpugYPTzHUO5h9Mz/Photo%20from%20Library.jpeg)

The etching seems successful though. We got away 1.7 um.

## Cleaning 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/11DB8A55-DEA1-42CE-A37F-B8B51912512E_2/W7ywg6rruMDJBFMcvi7Hr24gB6Zg5EJa2qHuh2lVe7gz/Photo%20from%20Library.jpeg)

Cleaning 17 mins．

21:48 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/E9B7CEA0-1E65-42A7-B3CF-855CEA58CB71_2/Bfg333IY7YSW7U8QhKDVI1bXroN1kjQRoB9OkOovzgkz/Photo%20from%20Library.jpeg)

He flow is high again.

The He flow is a bit sketchy. We should stop here before sacrificing the main pieces. The issue is reported to Jeremy and NEMO.

---



# Loss measurement

## Top oxide chip

### First straight

2 mW / 49 mW = 2/49=0.0408 

### Second straight

3.4 mW / 49 mW = 3.4/49=0.0694 

### Third straight

4.7 mW / 49 mW = 4.7/49=0.0959 

### Fourth straight

7.3 mW / 49 mW = 7.3/49=0.149 

### Fifth straight

6.7 mW / 49 mW = 6.9/49=0.141 

### Second snail

Power not measurably low. Not sure why.

Overall, we find the signal from this chip to be pretty low. Hard to tell why. Is it possible that the RTA messed up the snail?

---

### [`Mon, Apr 14`](day://2025.04.14) 

### Loss measurement of oxide deposited waveguides 

This waveguide went through 650 C RTA. Oxide is deposited on top. 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/63F39567-D0C8-45F2-9996-6C5F1C1568E7_2/QnGGEHZ5an49yZ5mfbLwK6bQBgcMgQePZ3nryOJVTscz/Photo%20from%20Library.jpeg)

### First straight

1.4 mW / 49 mW = 1.4/49=0.0286 

### Second straight

1.3 mW / 49 mW = 1.3/49=0.0265 

### Third straight

1.3 mW / 49 mW = 1.3/49=0.0265 

### Fourth straight

1.8 mW / 49 mW = 1.8/49=0.0367 

### Fifth straight

1.2 mW / 49 mW = 1.2/49=0.0245 

### Second snail

Not very bright. Less than 100 um.

We cannot couple light well into the snail.

## Air cladded no RTA chip

There is a finite chance that I messed up the RTA and non RTA waveguides in the previous measurement. Double checking the coupling to the non-RTA waveguides.

### Second snail

0.17 mW / 49 mW = 0.17/49=0.00347 

Double checking this number, the signal looks low.

### First straight

3.9 mW / 49 mW = 3.9/49=0.0796 

### Second straight

Coupling bad

## Oxide cladding chip 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/8A1C7A4E-82C4-40E9-8470-305AD4DCCD7C_2/zWewYLIlxH0S2ktQxZ9lAscErNDlUNExZBBasYfKfy0z/Photo%20from%20Library.jpeg)

### First straight

2.1 mW / 49 mW = 2.1/49=0.0429 

### Second straight

2.4 mW / 49 mW = 2.4/49=0.049 

### Third straight 

2.5 mW / 49 mW = 2.5/49=0.051 

### Fourth straight

2.3 mW / 49 mW = 2.3/49=0.0469 

### Second snail

0.03 uW / 49 mW = 0.03/49=0.000612 

Second snail now working very well..

## Snake waveguide with oxide

### First straight

0.8 mW / 49 mW = 0.8/49=0.0163 

### Second straight

0.8 mW / 49 mW = 0.8/49=0.0163 

### Third straight

1 mW / 49 mW = 1/49=0.0204 

### Fourth straight

0.94 mW / 49 mW = 0.94/49=0.0192 

### Second snake

0.05 mW / 49 mW = 0.05/49=0.00102 

The loss of the snake is high..

## Air cladded chip 800 C

### Third straight 

0.8 mW / 49 mW = 0.8/49=0.0163 

### Fourth straight

0.8 mW / 49 mW = 0.8/49=0.0163 

### Tenth straight

4.4 mW / 49 mW = 4.4/49=0.0898 



![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/584C0829-76D8-4C0C-8630-7D82F8DA350D/C2E59FE0-0506-4579-AD39-BDA89A8AEAD9_2/uG1vJnHWxXBnjP3VxDDsAcWVWFTTL0KcLTTWFaFQHg0z/Photo%20from%20Library.jpeg)

It looks like that there is some visual difference in the amount of dusts on each waveguide.

## Summary

- So far, only one snail waveguide exhibited a reasonable transmission (2.4 mW/49 mW). This was a piece with RTA 650 C annealing and air cladding. This was also a chip with the best transmission on the straight waveguides.
- After annealing this chip at 800 C, we cannot recover the same level of transmission as before. The straight waveguides also have become a bit "weird"; It feels more waveguides do not work well.
- The no-RTA air-cladded device did not show good transmission through the snail. The same behavior was reproduced in the second measurement. This seems to suggest that we did not mistakenly mix the no-RTA and RTA chips; If they were swapped, we should see the same high transmission from the snail and the straight waveguides.
- After oxide deposition, no waveguide shows transmission as good as the air-cladded RTA device. 
- A hypothesis: The loss is caused by the "dust" thing on the surface of the chip. This is suported by we seeing visually less dusts on the piece of the air-cladded RTA chip [Photo from Library.jpeg](craftdocs://open?blockId=C2E59FE0-0506-4579-AD39-BDA89A8AEAD9&spaceId=c10b6666-b4fd-53a0-9177-1696a144b2d8). Because of this, only this chip showed low loss. Then, RTA at 800 C caused other damage on this chip, stopping us from reproducing the result.