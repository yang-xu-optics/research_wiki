---
type: craft-export
title: "2025-04-16 mask design to eliminate dust"
craft_document_id: 6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-04-16 mask design to eliminate dust
Despite our persistent efforts, we will have dust after SiNx etching with a Cr hard mask in the oxford 100.  It would be nice to figure out the optimal etching process so we can easily design new waveguides in future runs.  Below is what we have observed:

1. After a 12:45 etch of oxide in the oxford 100 (no mask), we don’t see any dust
2. After a 9.5 etch of nitride in the oxford 100 (resist mask), we don’t see any dust
3. After a 10.5 etch of nitride in the oxfrod 100 (Cr mask wet and dry patterned), we see dust
4. Using the oxford 82 for 25 mins for fused SiO2 (Cr mask wet patterned), we don’t see dust

So there seems to be something about Cr in the 100 that is the issue.  So we are going to try two new approuches:

1. Thick pad oxide with resist on top.  We use the resist to set the step height, but we intentially etch through the resist so we don’t need to deal with the impossible task of removing it later.  We also have resist on top of oxide to minimize any optical loss.  We etch with oxford 100.
2. Use our existing mask design, but etch in the oxford 82 for a longer time.  The hope is the different etch chemistry will save us

Personally, I am more of a fan of 1.  My personal explaination of what is going on is the Oxford 100 is sputtering our Cr layer, which is causing us to redeposit a micromask.  So while I hope the Oxford 82 is a bit more gentle, I really think using a resist is a more sure way of doing things.  We are going to do the following (at a high level) today:

1. RCA clean a new SVM wafer, deposit 300 nm of oxide on the PECVD, and sputter 225 nm of Cr mask from the AJA1.
2. Pattern the Cr hard mask wafer using the same photolithography process as yesterday (and same GDS file).  I will also use a long piece of SVM wafer with 1 um of oxide on top and pattern it the same way
3. Descum both wafers for 50 seconds
4. For the Cr wafer, use wet etching for ~3.5 minutes to wet etch the mask, giving us the pattern we want
5. For the oxide wafer, we will immediately go to the Oxford 100.  I say we do a 10 min preclean, 1.5 min season, and 3 minute etch.  This should give us an idea of whether it is even possible to get no dust with our proposed process.  If there is no dust (and we are able to characterize the thickness of all the layers), we can proceed with a longer etch to get through the SiNx.
6. For the Cr wafer, we cleave it up.  We then go to the Oxford 82 and run a 20 minute oxifrd etch using the CF3H chemistry.  We can then characterize the etch rate after.  We will not etch each piece in case different chemistries work better or worse

Below are the two GDS files we are using (2 for the Cr wafer, 3 for the oxide wafer)

[pad4 pass2 (negative).gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/21C2A93C-D660-41AC-AAF0-400AB54BAC45_2/UiKYGVmWZuOxfJui4xAug7ZMJkYAXKOew7DxPjVRV2sz/pad4%20pass2%20negative.gds)

[pad4 pass3 (negative).gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9A39E0E7-727E-445D-AACE-05A133336BB2_2/NjtyFcksLyX2hCRGfsplivPsgFWa7TVCxihmwckbjYUz/pad4%20pass3%20negative.gds)

I am currently running RCA clean and 10 min pre clean of the Pecvd 

Below is the old wafer I want to use, though I will also check it with ellipsometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/E7AD3244-8509-4E41-96C6-B224C226116B_2/XN7sDfVYfnGdE04Oc3TgocPx5Cg1zrOeJMcSRI734y0z/Photo%20from%20Library.jpeg)

Ellipsometery 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/1913305E-82DB-4232-8A16-DFF00041DC74_2/YG4bTcDJZDAxJ3IJ6hjvLwpwVxUkff5xZEhTbmDema4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/B1525E77-9231-41B2-AD71-AA57B33633ED_2/Rt9aQxONdagmnxBwyQDk51j6QLShsJV2XKmarisXdoUz/Photo%20from%20Library.jpeg)

Below is a note from the tech session:  People did not seem to believe Cr was the issue.  There was broad concensus that we should use the oxford 100.  It seems that the more basic CHF3/O2 recipe is best.  There seems to be concern that we are having polymerization issues.  We might want to run shorter etches.

### Pecvd

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/6DECAA17-9AB7-448F-8A0C-4E2EC66B2D1A_2/4eB5xxjx4wCxPWbfa7H2bTxwQAJ5O7wxEHVzhlZFA5Mz/Photo%20from%20Library.jpeg)

Before deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/A54F4EF2-ECC4-4274-9BA3-03950C34F786_2/dmHwlWqUPJNPI4MWu6ktfDX3LLoYZ4omkrBjOxzA6Owz/Photo%20from%20Library.jpeg)

During deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/06A17D05-51D4-442E-970E-9D87BAC6BA62_2/LzhQNQkbwEsIGNo7CIsUrCL34P7N8xJlMEcILDEiwZ0z/Photo%20from%20Library.jpeg)

### Aja sputtering

Pressure when loading

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/DB889DB7-DD1C-4D17-9097-03EF681E7483_2/SRlglehqBW9Bw9hQ4miReoKhexZWuEHScmrKnVu691oz/Photo%20from%20Library.jpeg)

Our process

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/BC67543B-EE08-4D2F-BD5B-29C943D95D36_2/aRiHPqrGg03lyB0YVyddJNlVinxLvUyz9ZFm4xGPNy8z/Photo%20from%20Library.jpeg)

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/20175394-8C36-4A69-B758-AF392F70E2AF_2/0LRK7HJB8mJyOUFiyoc0tAkW1FeK7vSwwZK6SIdXtvIz/Photo%20from%20Library.jpeg)

### Photolithography

Spin recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/A448EE70-0620-48EF-A53D-7562449E8FD0_2/q4s2D5BLumfUK5KBW4WRFgeZIQ59ZwSJUWZeXjCc0OUz/Photo%20from%20Library.jpeg)

We also do 90 C for 1 min

First exposure

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/59453DE7-FC15-4C1A-A996-AFD0D39F2A00_2/ToS2h3AGqjdj1LKyo1wNtG9EsDj9cUPsU2uGVL11IOUz/Photo%20from%20Library.jpeg)

Use same dose of 53, 0

Second exposure has hard time automatic centering. The piece is a lot longer than wide. I am using the mask package to proceed

It is a bit confused about the size, but oh well. It should still expose where it does not think there is wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/DDAA56AB-149F-4874-9B43-259F64A4F0BF_2/3Du6WDD5wv7E3xyVsC98vWAOMNtFrrPyh7s2nx7ToRgz/Photo%20from%20Library.jpeg)

It seems to be writing over the full piece, which is good

Development of 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/D672FA79-4815-42CE-A4DA-3DA26356BA8B_2/hPsHyRXVSponkuP7NGuU3lnN2y5y1IyuN10rNZyNZvcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/258B58E8-2905-4E80-8D67-C8E87223D6A3_2/ky0yNV6qjxcbc0B1tU9TlDnT7BXFSLGgeDwr0Y1qucIz/Photo%20from%20Library.jpeg)

Second develop foe 1 min

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/6E6B0730-8A8D-42A9-AF39-1CC3BB2050A1_2/9BcykLQwfGUTlKHy3yGUwVhNSoB6oxawePceTel3QE4z/Photo%20from%20Library.jpeg)

### Descum

I am doing the descums seperately

50 second descum after the 5 min pre clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/0A2DEFED-EF02-4633-831C-AEDBFCE7D833_2/9zLcJcNKnYHS0R5Mz7MebPSCxvtZY7Z8ptfmfGyuivQz/Photo%20from%20Library.jpeg)

During descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/B4472BFD-D0C7-4212-B99D-C9E41D18A844_2/WyMxNqYylS9JqvuwBmvyRXkh9aMiGooJFET5rcRctHQz/Photo%20from%20Library.jpeg)

Resist thickness after descum is 400 nm

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/A9F5F9F3-E1E4-430D-95A3-AB59546A6B9B_2/j5oa5KejZvr2Gj1DpiKf17zSqZbKQjZbysTKvpin9jwz/Photo%20from%20Library.jpeg)

# Cr etch

We do 3.5 mins of wet etch.

### 82 etch

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9B8B37D3-0AFC-47D3-8FFA-CA818BFCF39A_2/pxp7B0CoxF3r4ndtnyxFGzO16UadWWGJ1AArRICJwZUz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/4C26BF5B-8846-43B7-90FD-E798EF4309DB_2/HyS4xTQxFZ0oEHnsdx0LIvd50biQM4gFGTUlYHm7Vxkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/583912A0-CE61-428E-A27A-DC9ECD059234_2/KlC91VKZfriVsOLURymbN7mzWQEixdBtsRZpRuxEf4kz/Photo%20from%20Library.jpeg)

Inspection

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9737832B-8EF1-49F7-BAFD-DC8711D898C0_2/Jr2tE96oEZl3kwAsN1MjgSUdabQ7CAbZGq6WOLUjJ68z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/B6B74158-6CE2-436C-9208-0F4EE01B41B5_2/lKriFGH1zTm1nHhEPfGGjybuEDvhIyYeXqUgUtZMf1cz/Photo%20from%20Library.jpeg)

Profilometer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/232F5BC6-C2DC-430B-98D6-1116E43565C1_2/qEtXx1tUzGaaasu36XWORUFQifO8yKjhPdvUb6Hp5g0z/Photo%20from%20Library.jpeg)

### Etching

By the end of the development and descum, we should have 8 pieces that have oxide hard mask and 9 pieces with Cr hard mask.  I say, at the beginning, we put 3 of the Cr hard mask pieces into the Oxford 82 for like 20 minutes.  This will still leave us with plenty to play with.

For the 100, we should start by cleaning for 10 mins and seasoning for 5.  We should then do a 3 minute etch of an oxide hard mask chip.   Lets see if there is an issue there.  We then will keep iterating every 3 minutes.  I say we start with the CHF3 recipe.  We should also measure the resist thickness before starting.  We will then, if things work, do one longer etch.

We can do the same thing with the CH2F2 recipe.  Or we can use the CHF3 recipe on a Cr hard mask.  Either way, I say we take it slow.

# Oxford 100 for the first piece

![Drawing](https://resv2.craft.do/user/preview/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/53AE567C-8373-4079-B951-FDD8199BA970_1/uqtxmOTFeg25xZDamHm9pxut0jvy7lEIx6WoNKPxKakz/Drawing.jpg)

Just started the 10 min pre clean 

We are going to try the recipe below for 5 min season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/1C16410E-3DE4-4942-B0BD-839DA35FAFC2_2/aNu6Cd7lBBrRKLVwpY3mS4g3nIVNSZgsbeZ3211TQW4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/EC3F3554-3F80-4C9F-A4E5-EBE1096554EE_2/ShQtkSTuVd0CTT5Hn63f1o5Mt7br9iPk31GRV6xlFsYz/Photo%20from%20Library.jpeg)

19:37 Finished

## First etch CHF3 recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/F11C4E60-AA2C-47A3-961E-260D445A6B18_2/6U92bVTAovJxN3C7nFOT1Vt9TUPMaSq9sDgvPrnjT2cz/Photo%20from%20Library.jpeg)

We use this piece

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/874C0C3A-FC5E-4551-8BEA-B0BB82B3BED7_2/pNoxOS9p2xNFIIuzlye4E3qDKg4jRpnSJMjiGvncav8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9B05602F-FFC6-4509-823C-CD4F8B588A74_2/lTkHosnf94ByLAexj9156gNV0OCkk7FwxweOaOmdtVgz/Photo%20from%20Library.jpeg)

Mounted on the wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/C01E21F9-CFFB-402B-B45C-AC652FAA8A74_2/qDgpxlAsB89nyEROUv3b7FCoREjZYqEMN3OjuCWP7TUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/EACA6F79-1813-4ACF-8E60-70321C01266F_2/gqRSYQ2fxNjsT3SNW8CJ5C0HySftIdgkX45hCVjexywz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/70247377-8595-4FBA-B401-622932C3C7BC_2/Wh8F73WhcfHsHf1i5cxeXcluPYT3CXSWvLWai4PMqusz/Photo%20from%20Library.jpeg)

19:42 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/7EA619BD-2E97-4184-BAF4-4568F6C1688A_2/6YIZQ2816MkPQevIUfNTCGJTH0Tx7jf8gImvw0Lm2acz/Photo%20from%20Library.jpeg)

Looks good. The plasma is on and bright.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/FCAED518-8249-4A85-BB17-D23B9D701881_2/P75lnHs8cfRrjxrMmF1VEM2A4IEHku84ZtEeyFjzbnQz/Photo%20from%20Library.jpeg)

He flow is also very low.

19:50 Venting

## Inspection

![2025-04-16-first-etch.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/D814BFE1-C08E-47EB-B3D1-690CA4E0A0E4_2/7xcqRV75Sj654oxFWZ23wieXbw2TsH9xNP2VjTVi4fUz/2025-04-16-first-etch.jpeg)

Small amount of dusts observed under dark field microscope 

1.1 um deep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/BE03E402-C04A-48B5-946E-D89E814AA364_2/0j0UHxvKW29aVj0vXfFYKToh3xYt1vHRP4O914uZInMz/Photo%20from%20Library.jpeg)

## Second etch CHF3 recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/A0A90379-9C74-4B96-9CC7-9E781C4F70FC_2/CjI63rK4Uwxa03c5m4IPjE9uZupbxG3nLXb9Ctytgp4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/5E221414-5FE8-489D-9877-1BC809F1EE3D_2/WDd9uJODzdU9Ke4kkqaMyJuOaKrRoF1KNYPSkHFgbnMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/29AB4148-C83C-4A8D-9687-2F3D1640C92C_2/Id5PGFRAUpAFGioyj4ty87gIaFqyAOumRHFK7QdNVuUz/Photo%20from%20Library.jpeg)

20:02 Starting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/54DB433E-F5CD-4DD3-B047-6606AC88D438_2/yAu62ge89nJriYaBQuawRHXhCe8i5XjN1xyYHOJAYxoz/Photo%20from%20Library.jpeg)

20:08 Low He

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/3670F65B-15AF-4AE1-9100-ABBA1D2281F9_2/Oa98gfMCrANcV1ywNLwpTu3xoDgfYMDCYevcB2hGlMUz/Photo%20from%20Library.jpeg)

20:11 Finished.

![2025-04-16-second-etch.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/A2343C92-258C-4316-A9C8-44B8E8F0F87B_2/bQLMZh0FulE0n5SCwWfEUoV4UwdKo76h1X8bU51pPDQz/2025-04-16-second-etch.jpeg)

The amount of dusts seemed to have decreased!

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/F5BF2A00-E895-4C6D-82FF-C3BC45E0FD7E_2/2WKBLAxZBe0YjKRa8sQGIr3N8f8ng311pSkOzlLQ7hkz/Photo%20from%20Library.jpeg)

Etched 2.4 um.  If we etched 2.4 um in 6 mins, then the rate is 400 nm/min.  Lets etch for 5:15 mins.  We will leave a small amount of nitride left

## Cleaning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/2B740E38-65FE-456C-96FE-016E26289C28_2/KoGyJTRevqx2bwIK2q2Bs9Gr4uWFSMnEoR4vgbghQ20z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/BA73EC6E-4B8C-4369-BD54-118969D8B155_2/H4sBYvV64EzbYyH9qE5BN8qvdMxHMNVEthBoDTenHdsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/F0515E52-857D-4528-9DC2-97C1DB12DFE9_2/2V3yOU2td5msSU1vHO24eyxODcbsjPwKXtLJyUiNC44z/Photo%20from%20Library.jpeg)

## Wet etching

![2025-04-16-after-wet-etch.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/B36A7011-6608-4063-9A9C-7A28A09D0768_2/YRvijI6rivvGwBfB0Mhd3zEoTsRwX5XfYW1qcPdJRTEz/2025-04-16-after-wet-etch.jpeg)

No visible increase in the amount of dusts



# Larger Piece Etch

5 min season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/1349841C-6A0D-4E1B-B4C3-2BBD5EACD879_2/YleWVuEDkxL1EXjzSHCfADn707SivMimeQxouS9jVsgz/Photo%20from%20Library.jpeg)

5:15 etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/29F25EB1-90B3-4EF8-84CB-7A3141167987_2/qht3UmFUtSMjQi3BmsNoPOayrU6d0JQ8VZcFn8cKEyoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/D1FB5C78-BA59-405F-9AB6-DB400F154DBF_2/9SARJxZMPWlqLUXf9rDgvSBn6zaOGzrcXHMgVAt1muAz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/F6E7AD0A-C4D7-431F-8653-1165D27333D4_2/9mC6lw49ztw9vTTV2wAOQHUqADmoSp1PVRsJBBVmevMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/44674861-1483-4221-ACDF-56C516473DE2_2/9h6nKYmHfyJGhpily16iwPYJVGG14ABmg1T3tlAlgUwz/Photo%20from%20Library.jpeg)

## Inspections

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/EDE5CB77-5B06-40D7-9F1E-CDEAE66D9A50_2/A5avqhoHLCkVcmyKJ0jeDqpMuZCx8qkktBhMfJqGpxEz/Photo%20from%20Library.jpeg)

![2025-04-16-main.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/F5085531-4E1F-4448-B825-A93AB5747A6D_2/9EvH81c5UarchJtUxnGXE4B4M3zvdT7HNwt2k9UZEMkz/2025-04-16-main.jpeg)

Very few dusts!

### RTA

We are going to do 2 dies at 800 C and leave the other at room temp

Calibration run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/3F248B2D-1B7B-4B4D-A8AB-44006AC04C1F_2/AH0q13Z3mFNu16yAAJWcPUw3miA7WLEIfWO0lFCxQDwz/Photo%20from%20Library.jpeg)

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/7995AB8A-4A33-4615-971F-676E2A0432AE_2/WMaWBp8QkZGbkYrJZwGRvw2xxvcAnEoKTQ88cY58gBEz/Photo%20from%20Library.jpeg)

Final RTA

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/89CC2591-5BF3-49BC-AF46-E93D62E27B12_2/tKCAjpkys2zMlgKFAJ21ukCW7rWDkGvdmQX6yAII5nwz/Photo%20from%20Library.jpeg)

I am using a clean carrier as well

During 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/731C8F53-A5DB-4EEE-AE9C-184F51ECC8CE_2/KQQkRwlNqydifyUDGgeDxQEfutStMnSGqDXQUds0znsz/Photo%20from%20Library.jpeg)

Inspection after

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/C4E9C80F-3FDB-4649-8601-399D08F5F039_2/S3SaD7eyqIXSeczOV3I8gfZq51re6NoOiWN5iWyG6iwz/Photo%20from%20Library.jpeg)

It seems that the SiNx burst off. Below is filmetrics of the holes

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/193BB5DC-94B2-4514-8129-17087E1B2A6F_2/yNgDrBjmKu27shrplFglxaQ4cTSDaSQW63mSj7RKmTwz/Photo%20from%20Library.jpeg)

Of the film

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/CAE973E0-2555-4585-9C46-18F5074F4A5E_2/EDvPX9qKWerNnIROI895ALxpS5xRTt9O0HIzcFGKMgcz/Photo%20from%20Library.jpeg)

Microscope 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9DB552D4-1B49-4406-97E9-3942DDED4C58_2/oOTNK8KcmAtII5PWSrLVmbFU1FGq9LWp0xG4BFYkGQIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/F676BE23-967D-4446-A07E-00734B75A2B4_2/Ff22WGpZTpK7Oy2jSt6mbgJvPd7PWhMXYkoVNveKBFQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/666A1DEE-6CEB-482B-9DBB-23C02A40F74E_2/y3Ucxl2CWxdFMV6t5GVyITyGQPftmY7SwR1eSZIJpoAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/4B90EDF6-6A0E-4B63-8B39-2AE7A1562C89_2/XJhmbjFw4KfbPD9wCNaW2lV26YKIzs2TFqsXP3GTJXkz/Photo%20from%20Library.jpeg)

Everything else looks safe, with no cracks on waveguides

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/B961F7F4-5618-4CDC-A716-4433EBA80527_2/uIxfFhiTURUodvmMvjrmew0FsZa96F2fLxhxAojDCWcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/15EC22C3-FD0C-4109-8F93-20B336763C1F_2/KUL4xJqhwBKexgzTELpyjMkjr23B1IvKkOGgLsgLDskz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/0445FBC6-6DE2-4F22-B857-9F73158E48DF_2/E5sursdp81pX45Zs827LIPqX3gDL9MluwNWjNJpGeHAz/Photo%20from%20Library.jpeg)

---

[`Thu, Apr 17`](day://2025.04.17) 

# Room temp chip

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/24B29F02-61F8-4CAB-98DD-FA8030F7FBBD_2/qojAS1Z9uTCyPgCAMDYzGldIl0FOyx1dyMys9BfCsmcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/AC1AF6E7-672F-4EFD-B25B-42327EC369A4_2/hpifBQBJwD4HX3NG0gtaWV69YHUGVRk2E99VORhjimAz/Photo%20from%20Library.jpeg)

### First straight

4.7 mW / 49 mW = 4.7/49=0.0959 

### Second straight

5.1 mW / 49 mW = 5.1/49=0.104 

### Third straight

5.2 mW / 49 mW = 5.2/49=0.106 

### First snail

0.3 mW / 49 mW = 0.3/49=0.00612 

### Second snail

0.28 mW / 49 mW = 0.28/49=0.00571 

### Third snail

0.1 mW / 49 mW = 0.1/49=0.00204 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9D657780-BF90-422B-8CC1-E2F0EB7D0C19_2/l9QtLwlHJ3PEPaNQWIxiS09TamU2SOwWcriqHEFenJ4z/Image.png)

# 800 C chip

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/8F9F9847-C49C-4CC6-A033-C27734299E88_2/S6tvZgGYgPgLXiS0OZKWMFQuyjU4pgFOZWWG0aYQMDwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/FE0720BF-52F3-4D8D-A267-F5B5D383A07A_2/NRxAX92wgc6pyNkmdDy80DBaD8yDHyvM7dRxaugk5dsz/Photo%20from%20Library.jpeg)

### First straight

1.2 mW / 49 mW = 1.2/49=0.0245 

### Second straight

0.25 mW / 49 mW= 0.25/49=0.0051 

### Third straight

1 mW / 49 mW = 1/49=0.0204 

### Snails

We see only few microwatts from the first and second snails

# 800 C #2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/70796DF2-1FAC-4FD6-8D0F-3D80ADB7EAF5_2/EnGZ2K2IypStiNcall9SAeqSWKOTBlJxpyaQajgONEoz/Photo%20from%20Library.jpeg)

We use the longer one.

### First straight

0.5 mW / 49 mW = 0.5/49=0.0102 

---

New cleaved wafers

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/E148C7EC-0BCF-4C3F-83FD-4C0C9058E714_2/WKj1WYazj8SQIqX9IxPtjqtz2MEyqUeD186JT8WR4Hoz/Photo%20from%20Library.jpeg)

After 800 c

### First straight

7 mW / 49 mW = 7/49=0.143 

### Second straight

7.3 mW / 49 mW = 7.3/49=0.149 

### Third straight

6.9 mW / 49 mW = 6.9/49=0.141 

### First snail

0.55 mW / 49 mW = 0.55/49=0.0112 

### Second snail

0.88 mW / 49 mW = 0.88/49=0.018 

### Third snail

0.7 mW / 49 mW = 0.7/49=0.0143 

### Die 2

### Snail 2

0.57 mW

### Snail 3

0.95 mW

### Longest snail 

0.24 mW

I would still like to test the other die (I was just dreadful at switching the microscope).  I think I have enough to work with now though for loss measurements





Compiled losses are below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/CF9F965D-456E-4FB2-9EAA-3ACA86F7DA56_2/WcOpxIQeyEDkQoPt8yxGzgTQCOmrupCsPGjhKeHo19Iz/Image.png)

Below is a loss matrix

|       | Room Temp | 650 RTA | 800 RTA |
| ----- | --------- | ------- | ------- |
| CH2F2 | 3.148     | 1.963   | 1.525   |
| CHF3  | 3.546     | \-      | 2.475   |



Now I coat resist for oxide hard mask. I use 1813 for 4500, 8000, 45. I want thicker resist because our recipe will etch it fast

Before spin

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/3CB2BE96-3FD6-4ED0-8E31-ECA50EA72750_2/eddUEqYaKqsApkH1rhIcoUC0l04J9tMM0cfExg11wgIz/Photo%20from%20Library.jpeg)

115 C for one minute

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/5D8C6673-B615-44D8-A0B3-299F3E3BAEF3_2/xWJ4XhXTef70ZNI27Dx2OGovCFgTJIrqhGUmseGSVYAz/Photo%20from%20Library.jpeg)

For exposure

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/CA5BF0E5-95E4-469E-9BA9-4F9298C3865F_2/bOzRIJL3m5lrfnbSKZg9AUxtGpQhUx65jKVCR3rAA24z/Photo%20from%20Library.jpeg)

We used 70, -1 last time, so I will do that again

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/6B6C6439-5EEC-436F-AC10-30C62D5E710C_2/eRW64DQPzdA65PxpNtGt5N69XymeGaZfIC9WxGyO7xYz/Photo%20from%20Library.jpeg)

Writing is going well

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/B113B1EB-B40B-4707-B49A-F6BDF373873D_2/spU0Tiqg2dotsOzI8cEeuwzBJRav8ATNlse9wDxKiZ8z/Photo%20from%20Library.jpeg)

Develop in 726 for 1 min

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6BF9DC2A-9FD0-4700-AD2D-C53D5FE8AE31/9D94FBFA-35F6-40EB-B75F-F298595026C7_2/SOK7TMjgFUDp4ixrI0qI4MyezxDfdYxnGmGyh0ycXb0z/Photo%20from%20Library.jpeg)