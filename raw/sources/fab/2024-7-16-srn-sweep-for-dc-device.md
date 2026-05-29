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

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/1f565a67-48e2-2df3-fc7d-c338964e6e60/2sbE9xw4oqQKorUbyKScF3Ttbkvd0twHGQC18yfFrQkz/Photo%20from%20Library.jpeg)

SRN4.5 43.45 nm/min

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/e9a99981-c653-aa8f-5534-0c5a9c6fb08f/6n6f8BB2Rkbfy7drGf5fqX46D5DlcQase1P6gfP8eCUz/Photo%20from%20Library.jpeg)

SRN5 46.15 nm/min dep rate

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/56225c31-c5ea-a6d5-294e-7e9aab681286/0GtbdNXjKOe94G3ZVlZ2R4NgJHybodZDDq0YhpZ8hN4z/Photo%20from%20Library.jpeg)

Below are the confinement plots for each of these recipes on B8

For SRN4

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/47021193-6C7A-48A8-B3E4-269B4AD1D018_2/UvG4ih84rqclRBTdoV2xltVSaZ3Q8T88lFDiDXt1F2Az/Image.png)

For SRN4.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/7337D954-1FFC-4D74-A54F-93C4E47AD32C_2/6ILEH8sv8Jtf9YHyoaZy8cqPDvwSDVWAoIDYQYGNGAkz/Image.png)

For SRN5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/11D7279F-AF22-4BB9-8980-C0A06D405C26_2/XmYyU5hPSr5tfxPBUYK829JOqelqayzLR4cuBixFiMgz/Image.png)

Ideally, lets get 1um of SRN on each one.  We can adjust for modulation eff later

After running some course simualtions for conductivity, it seems that having a thicker core causes longer RC constant and the need to operate at higher voltage.  The upside is that it also lends itself to greater bright/dark contrast.  So the question is how long do we want to spend making these bottom layer.  My take is that it is probably best to do the full deposition of a 3um bottom oxide layer.  This will give me a more fair comparison to the other films.  This is just going to take sooo long.  I will do this on a full Si wafer, so I won’t have to do this again for a while.  This will probably help increase breakdown too, as I am worried the oxide might actually be the ones breaking first.

So the plan is as follows:

1. Break up the DON deposition into two steps.  Do season, 24 min dep, 25 min clean.  Then do season, 24 min dep, 15 min anneal at 375, and 25 min clean. Do this on a full wafer and cleave it up.
2. Deposit 1um of SRN4, 4.5, and 5.  This means do 24 mins, 23 mins, and 21.5 mins respectively. 
3. Deposit 1.5 um of B8.  We want to do this on the 4, 4.5, and 5 samples.  We would also like to do it on some of the loss wafers (hopefully an oxide, 2um Ta, and 0.8um Ta).  We can anneal some of these later.
4. Evaporate electrodes

This is going to take a while.  I would estimate 8 hours.  Big Gulp.  

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/3A885CEC-3BF5-47A9-B207-B08E4436B5E7_2/4xNc38fHgtseMy4rRVxMzxAUSihyuht2FgH0xm7Ewwoz/Photo%20from%20Library.jpeg)

Ellipsometer is broken, but we can see that right wafer has right color

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/C1A9AC43-69CE-4518-980F-6A51A1E19B1A_2/kUiWuFD9hkyCJI3fvOSAwkurpsQUV2H4QLt7QJqQeqYz/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/4BFCA1F5-73E8-493A-9001-85B4534A9A41_2/kEexxHiNpEYCiTNkSJCGbSbZnC2dagiH3xALRWrG3yoz/Photo%20from%20Library.jpeg)

During dep 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/8A96B4E8-338B-4BF0-B0D3-C80D0B5F9BAD_2/6mfI4BasRVhhxjWRWxDnZMRbxOxlAH7OCPNxAfhJCxkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/F52D3201-D0C3-4FC3-A143-000EFFA16C0F_2/2uKs5MZpxpuySz6dcy0L35nzFxmIMKz3EFlOag1pE8Uz/Photo%20from%20Library.jpeg)

Before season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/655A2B25-1322-4B7A-B875-8418817B226B_2/V9zb7t25vb5Cv73FkvRSf2yxdA8bW8rDxrlwjymLynMz/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/23B929FA-644B-4AC6-88C9-39DC0744E828_2/HxO8YRiHFHdKZoLLxXQp3IYmTggi6Y2Rf3wxnx5i7QEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/DC02EF58-EA7B-413E-A816-B28631F962B6_2/yzekxqqSDnMUsiqNk4fKSI6oLT2YuoQ6mpu3DjW3y24z/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/98489205-1275-47DE-9BBB-E455E700CC64_2/vqdLW8TLrDpPpGkpMAnn4fFeEiKmQrIiGNy8xWnSpooz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/DD6024B0-5217-49D5-8A12-745412D18293_2/xW8gpHwZYsFOguZYVxyxvM1bMqFwdxaFYwVFkv6L3qgz/Photo%20from%20Library.jpeg)

During anneal, the wafer got up to 350 by 10:50. 375 by 7:15

Ellipsometer 

Using full water map

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/157A4DD8-C22D-4033-B5EE-C9DFE60B1F76_2/nH21UbjsNxSkR4Rh1DPxY55v5bBrGwEYlsuFwnGkeDcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/6C27F8AC-DCBD-4EDF-B4CA-0F7CB578F118_2/YnF0TrVmKbxVQIq1xEyxpAGOr2B1nXIqM03HstwKEvcz/Photo%20from%20Library.jpeg)

Wafer map

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/88AE4C2D-7C89-49B8-81B0-BE95011CE73C_2/FdDpsA9EzHh5fkPkRGaXU2Z9YzNvYBw5ka8aniM3KT8z/Photo%20from%20Library.jpeg)

One outlier

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/3988E4A2-F3BB-4CF6-808B-8AD0C38166DA_2/XrnPAXoCsZrEBIYolYhOZ4F6rQlXdVqBILjOqe970yYz/Photo%20from%20Library.jpeg)

Now high quality center point

Short

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/1C10FEAE-F265-4CBE-B85D-A88823124B02_2/gQo9BWyaPDnOROyXeSIgWsOyM5tneKLE7btzoEJuw08z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/33ECEE0C-CBA6-44D0-BECC-7C9C8C74AB06_2/6WmSPhTzKQzlnZO1yVYxTsoyFlsx5cJKdKbkLSCixHsz/Photo%20from%20Library.jpeg)

Long

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/69E483D4-1EDD-4D3D-AD15-D976F6BCDC8D_2/M2mf8fvI1gCQN2gFHp4I1ASJa16h36n8dcIFBLaksP0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/142A514E-245E-4B05-A958-5EE649507F63_2/iT2mSV1SVWtUQl8mcbBkDlWCxt0J48hb3PxZZ8o1QHIz/Photo%20from%20Library.jpeg)

Before 4 dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/E8C67A03-4525-410A-B4BE-775321250A97_2/DFjBal5QqAlzu2vnpNwqwDv5L9Q9b71EuVCVeZLMWUoz/Photo%20from%20Library.jpeg)

I heat for 6 mins before. Witness is on top

During dep 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/3E22F1AF-B156-4BB6-A38D-49D7DE11CF5D_2/G9bDxfOYV0OwvfrrcbmmejeJ0S1xOwH1VUwJ5VGuyisz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/163F222C-2A37-49C1-B56D-742B328558CA_2/oyaMBVuKVcyy6grbxWoWzHy5TC9B8HZ5RxrsAYaczToz/Photo%20from%20Library.jpeg)

The plasma looks more turbulent than usual. Plasma noise seemed to go down later. Maybe I should have been more careful with cleaning and seasoning at the beginning

￼after dep, we are not looking good

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/607FF143-E591-441B-8209-39F7922CC793_2/bjDSgvHdLBfL9f0xfUwzBP7vd5j5YIsGzrbSmUVUAOUz/Photo%20from%20Library.jpeg)

We should have done a better job pre cleaning. This is disappointing. But not the end of the world. I think most of what you see on there is dust that should have been cleaned off. Not sure if these will make for good waveguides, but we can try it out

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/95FBCF63-D8B9-4A23-BA1C-7A4ADB04ABA2_2/UXB0qaGWCZxluJ3znj3nxUhgqKLgAtYbAbT87CsuXbkz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/A0D796D3-690C-48E3-B9AB-2D884C60A77E_2/I5vokwXGtDBhy8NuYip8RdNx5CpopvAu0erCEEgVos8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/1A5933A2-478B-46F3-955E-06D4C3FB091F_2/tcyq6D4ZepONO6N3STYxz7kLejbFpTYP6dVxsUb7T8Qz/Photo%20from%20Library.jpeg)

After dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/0BE8959F-75BA-46D5-9F8F-B0A0ED15337F_2/HO824gyiJwRrKfsNc5FhxmOWzc39Anp3ygKnLbxUqxEz/Photo%20from%20Library.jpeg)

This confirms my suspision that the guy before should have cleaned better.  Oh well I guess. 

I am redoing Silane of 4. Below is the recipe before seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/CBDDF477-BA4B-48AB-8000-57711FD795EB_2/wAAqXY4Xm4x4OFyLVwhXXRLh55KnkHfptcVZrdQCuGsz/Photo%20from%20Library.jpeg)

During season, the gas looked stable.

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/5786FADA-C4D7-4323-99D5-773B0B2807CA_2/dFytiyDIdj0m1Hy33JFq6e9NNKyF40ly4kUCzCy5WR8z/Photo%20from%20Library.jpeg)

With 6 min pre heat

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/D82AA565-5947-4BE1-A7DC-757E759F315E_2/toraXuhQpOISMPNvlYRnt5Z8uubq8ayDRjwH00NxWLUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/BAB33F54-0129-418F-9490-F080003641EB_2/fCyAUCRoY6OUcCTVOTITxKBK3IV0UzOozi9AyxhsB0Qz/Photo%20from%20Library.jpeg)

There were no issues with uniformity after this one.  Really goes to show the importance of cleaning

Before 5 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/C02C7503-9839-4461-8479-C9B69565A6A8_2/gPLEA8zEz5adWeDkoHC3oEx7DgmGFHe0WfyC09PemAAz/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/7F3AFBB1-67BE-46F0-B815-3970E209C01D_2/ByWNCpxt7noE52wOo9RGGK6M1NInheV88rjNPvHtGy4z/Photo%20from%20Library.jpeg)

With 6 min pre heat

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/09E2A673-55DB-4D80-8C05-FF798DE0D63E_2/dYHG4XLGxQxlzdM3S0ZLz8j2HYni9CUU4ih7jkYyyu0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/9CAA96C7-70B9-4E85-947A-DE428AEA216C_2/Dh8VMpD5Hy9eye67IoPbX6r4yGIuchpVHk7DwfUE7Y4z/Photo%20from%20Library.jpeg)

Before B8 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/D4AA9E1F-046C-4CA6-944F-D6706DEB9851_2/x4syJAUniScpXRCBhikRbik37y9yvQ9XmlVSwfULXPQz/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/D4ACDF6F-270D-4EF1-8024-B4587D1E70C2_2/ajQLXTjtS51syYHvxysfo7YZ6caAX6k5k5d6Eqb8FTcz/Photo%20from%20Library.jpeg)

Bottom is oxides. Top is SRNs increasing silane from left to right

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/612989E4-0005-4FC3-9A88-04FC7750725D_2/yu53NFsYoe43VRoZIzwWNor481PxSUymEUP0jBIisSgz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/BF80EAB5-FFC6-4C2D-9E88-44A0FE6C6395_2/yyxpzEKkH1RUbbTy7cS6Kws5NCjW9sMtjVehLCQPyusz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/E9AF4B3D-FC60-4178-A736-E0C1D0122144_2/hlHJJ3wbGx1IdIH7lUC6LPLCWYC7TlypeeW1h6SN9ikz/Photo%20from%20Library.jpeg)

Now onto thin oxide layer (probably 8 min dep) for the loss measurement 

Before season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/B2AA3A42-1A86-4008-B896-E632763F2E03_2/Gca1ZtkMO6n8UO2tYoNW6UHUvgQV7ixFra56GEJ9LDUz/Photo%20from%20Library.jpeg)

Before dep 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/993E8701-A998-4174-BBCB-61BB0054178D_2/2foNYBE5pO3hJNh69QV7Mta3Krs0XfqGhqiELAyGgKQz/Photo%20from%20Library.jpeg)

2um on the right 

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/D33ABF34-8BCF-484D-8BC8-914E13341BF3_2/X1HfzOPdASRFKij5BVN6opHDqUMgY3FWvcsOAia4k5Mz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/F873D2AC-02D8-4C08-BE33-39681792D7D4_2/lACSg68SiyNJs3CeZkQphJIlN1DBoW3EhxpmEzKnB7Az/Photo%20from%20Library.jpeg)

Calibrating anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/372A1964-D179-49D8-B5E1-904436B0EEAA_2/hCNV65JexxSGbe97GnsDIVZ3TeYYf5pY7yMe1jYAuqYz/Photo%20from%20Library.jpeg)

Smooth entrance. 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/6006263D-F6FB-49C7-99F5-B5949FABCAAC_2/SncyX7cwikUbkWpchsAtmbE2ij4oxglDcCX5FgcPaWQz/Photo%20from%20Library.jpeg)

Right is 2um Ta. Left is 550 core loss

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/61C94781-04E5-4161-9472-AF6A95418F65_2/CcNMlSSo2zknryoylFskzZYWtgAVN8joWD7spTxjDpQz/Photo%20from%20Library.jpeg)

 The core loss film completely delaminated 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/D6A36FBC-1432-470F-9E55-DBF529FAC4F4_2/BXCpmpt42MtSkF8x2xVTub2mp93nQWl40Gypya5Xx2Az/Photo%20from%20Library.jpeg)

Not consistent with what we have seen before, but I am not going to break something else. I will instead try a core loss measurement with anneal at 425. Maybe there is a compressive stress issue being on oxide. Actually, just extra delta n chips

Ellipsometey

SRN5

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/31196C92-2C44-46C4-9440-4D5A5A7E550A_2/ouy2ZrWbKQoolx93qxBx39ufnCg8u3lW2OowXWxZ2JAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/C1FE2B44-FE00-419F-8469-0A9CB0BE07A2_2/x8sZcVGD3lTAW9CLy6C5BcqgM1TFKVJbpwtcqfyQ1Lwz/Photo%20from%20Library.jpeg)

SRN4.5

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/1EDCE960-1B99-4051-98E7-6DBAF8195D9D_2/SfgPjSGdEZ5tfpxYLVU5qncEy0I3CQLmbn56OmeeLg8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/FE55E363-F52B-4C30-B510-ED017830A8A9_2/QRyy5fpACLPkhbTDiRMgl5IGJU0b3xyy6BTnUxpAX1Qz/Photo%20from%20Library.jpeg)

SRN4

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/64432D60-E2D6-46B8-BBA7-F3B4D853D11C_2/NK3P5XGgeebvr0hBJ2K1JsOJpuGJXP8FCDWFxerwuLUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/0FE389D7-5FFF-478B-B0D8-50C1811D115E_2/rxyHqygQegxuN5yK00jD2yTI7eDkDXHFO52eLPXmCMoz/Photo%20from%20Library.jpeg)

B8 no anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/6BBDE83A-1DE3-4713-BC43-CF0B621D53F6_2/kXYbBXu2zAkxx0WKx6ob4mlyxZy4Bp0WEF3StSG4EE4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/A50B78D7-3920-4013-BDD0-FEB057B93301_2/fflTLywpEzzl8bKWAnAFrxYPtNELfg7Tb4XYPsQx0QMz/Photo%20from%20Library.jpeg)

B8 (stress cracked) at 550

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/FCFA191F-AD3A-4AEB-927B-4710B77DB857_2/GDrHjjNUghcbNBECfhgFSUyyKjLs2gPJhUsYoU54Sh0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/6C8EA18B-C821-4B76-9C8F-D6C20B099650_2/UJnLlTcxWyd5muyyGTX35LFUafzopyYxgC1NLYswx8Iz/Photo%20from%20Library.jpeg)

Surprisingly close to the index we expect 

Before oxide seasoning

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/257753A7-D405-4EBE-9958-33361FCC7588_2/5EzQeZCpS3c43yPfxWENjUiUIjaQvN07fai2YC5njyAz/Photo%20from%20Library.jpeg)

We are going to run the actual dep for 6:20.  Roughly 1.5um of oxide.  

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/6775383C-CA11-4C52-A20A-0A082B2E10EC_2/AkOftHpN0TVzyhZFlDq0OhOT38nCt2JReuj8wy2fqtAz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/33FDF41D-643A-42B9-9E2C-1247AF8D5700_2/fhShbXpDX9PPkffsfzwwtW7BnIe5rcWOIDK7PkOi690z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/9E7BFC8C-AD11-43E3-AC69-85C205C20047_2/stzO8TgvYpExHVh4Jgx6fW8vzvI2SNm0BhErfvUeaq8z/Photo%20from%20Library.jpeg)

Now evaporating 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/8A89CE5C-FDDF-48A2-A3E6-1AD4DD68919E_2/ExS73xsW38xF9G3rGN3x4gXox9xLduwl4wPdBDU1PGYz/Photo%20from%20Library.jpeg)

Bottom left is delta n

Bottom right is SRN4

Top left is SRN4.5

Top right is SRN5 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/AE88978B-D3E9-42A1-AD54-FE23C2733D40_2/xIHzlBnCiIKUkybjllxd2nrcPTWxTJDzKRqx7pLkTkMz/Photo%20from%20Library.jpeg)

Life is good

Au in 3, ti in 1

We did have a bit of rate adjustment during Ti dep (I had to lower power). 

For Ti

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/06AE5B85-E156-44C4-912C-1005C80E0AB1_2/5Zku54kSe3uSm1yG7i2qZ65pvU8xPmZ7yAKtnfmrYLMz/Photo%20from%20Library.jpeg)

For Au

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/B01DAD19-8094-4424-9B29-5139E8C7871E_2/ZsXy4ZqV6xDGGehI8Zyh9YMx5E1BypzGpyUC1vesAFIz/Photo%20from%20Library.jpeg)

When doing the automated measurement, I see that the bright state current limits at 450V. Not clear if it broke or not. Let’s scan down and come back to 5

SRN 5 is 0.6

SRN4.5 is 0.9

SRN4 is 0.4

Plots for SRN4 (chi3 = 3.5e-21)

![SRN4 1.0 Plots.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/E574D496-3A28-4C9D-910A-F32346944C51_2/g8nPZo6RjYPyoA9hCPfInd3d45eM6yncZVqQ1Oc1GnEz/SRN4%201.0%20Plots.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/812E43E7-DC56-4CC6-8432-1CAEB758601D_2/HS2i8qNlO129lQhtoETr1IDCV1V0DMvTl2Sf6UHicBAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/33934B53-CB46-4EC1-94BC-279A4B924CCE_2/9rCAFW4uWEYZJFI5jinxx2z7zn1iYiMQZbCEgZi6F0Mz/Image.png)

![Screenshot 2024-07-18 at 8.30.41 AM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/B4FA5363-C542-4CAF-AC1E-1151323881F4_2/PqtCdh2M3JA4ocVOTuCaaI0gAhRMgRJt03eGZx794a0z/Screenshot%202024-07-18%20at%208.30.41AM.png)

SRN4.5 (chi3 = 4e-21)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/D4D1FDBC-D576-47A7-9892-90D20D0BDB72_2/SPzu9c9ezX1we4aLIysdFCg5HYAxej6LXFdgSwYtPIQz/Image.png)

![SRN4.5 1.0 Plots.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/AD08FF81-F158-44E8-9674-2D41541C5068_2/xEhS2srVXsngS7U16tbuvth0mPVSLI3B1vIi66lyjHsz/SRN4.5%201.0%20Plots.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/4B8A3CF0-ED61-4160-AC0C-3C0A101F69CA_2/osMx50cisfELdFt7xp201TEUkIOIkHSBl82N1GqHOxwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/FB2C65CB-ED32-4067-9D19-1EB503F31E36_2/5opoZ94LESJ2pxVUXYgBrxXmvKYkawAv7LymnNWunYcz/Image.png)

SRN5 (chi3 = 4.5e-21)

![SRN5 1.0 Plots.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/56112F17-2281-4BBE-8162-500C88FED63C_2/v6d2hVDsqNaOBtO5PafGq2xntMHc8u3fT509dPOYigkz/SRN5%201.0%20Plots.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/4FE1EAA4-D6FF-43AD-BDF4-268A4973A0CC_2/nzT6qtT8YEbsyCt5QRYYQpwxZX7glEc5tJel0lpnnOAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/85E6DE8E-0F6C-4E32-A0B9-D995F60E22B2_2/m7iXF6boeIUexsychcJsJODP2F1yGgOrl2n2PCqdhAoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/8AE5E2D3-7BD5-4136-B659-914B610ACB01_2/67ZnO5Oy7WtwZhHpv3QsNVHU5YDBm27MGI2HjmIZ5Ocz/Image.png)

Very minimal field contrast and a lower delta_n.  There is more field in the claddings.  Lets do a full plot of all my results including previous measurements.  We should also normalize the voltages axis to the thickness of the core.  It would be a more fair comparison

For B8 delta n, our chip is 0.7 cm long

I get some very starnge results.  Firstly, I should note, this is a purely academic exercise, as the phase shifts here are really small.  While it would probably be incorrect to say that all the voltage we are applying to the stack goes to my doped oxide, it does seem that some decently large amount must get in. 

I put the camera rate at 48 frames per second, and the frequecny at 100 Hz.  Below are the interesting peaks

For “8 Hz”

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/159479F5-8EBA-43AC-BD46-6468FB6B02A1_2/zecsLdXBPWbab0piYi4nIwu6OoMhkoTHiDYvZssJtgoz/Image.png)

For “4 Hz”

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/8B209202-EB4A-4BE9-A27E-774EA3CDE1B9_2/KUOOtXss9z7nA4GgWJKalOWg0iHRJb2AtvwxbD9FRyEz/Image.png)

For “12 Hz”

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/A70CB3A8-2087-4A3F-8FD9-C2916D070E6C_2/zR5mN4SsqjeTfIUNjaqe6R3nKAoYX5bFyZAQ5vJvi6wz/Image.png)

Looking at some of our fourier transforms, I don’t really see much evidence for the 12 frequency existing, but our resolution is not great out there.

12 might just be noise, but 4 and 8 and not!! Interesting that there are two peaks.  Lets try to think a bout about the path and what frequencies these imply, as it could be telling about what chi2 or chi3 occur in our material. Below is a quick math proof for why we see stuff at the frequencies we do.  

If we run the camera at a freq of 48 frames per second, this means we have a “wavelength” of 0.02083333 seconds per frame.  

If we run the oscilloscope at a freq of 100 Hz, this means we have a “wavelength” of 0.01.  If we divide the 48 fps wavelength by the oscilliscope wavelength and look for the remainder, we get 0.0008333.  This is the “distance” offset, which means we need 12 frames of the camera to get this distance mismatch realigned (0.01/0.000833).

Because the camera works at 48 fps, it makes sense then that this is what works at 4 Hz, (48/12 = 4, and do unit analysis to see that this is freuqnecy).

So we see chi2 and chi3.  Now we want to normalize this plot for field inside of the core and try to get chi2 and chi3 values.

Below are the fit function (in m/v)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/10BD2C13-83AF-4F7A-ADD1-7B37D980D933_2/G7h2TepYVkrMzafRr3E5HkZpTs2sC7CXkPCRyasnENQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/88B6C236-CAA0-4940-80AB-5D905DA5D223_2/3YanWWEv1vTpJ6fFYGlELFwx72wxcr8fXY2prkXHJVIz/Image.png)

Nice that we have these characterized now.  Lets do a quick simulation of how fields normalize with loss.  It is still tough for me to understand the bright dark contrasts we are seeing.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/F3DC9DBE-2355-4B54-AAE9-6D381C4AE7A2_2/vYP4sPSkntlDUMXKUf8ge9SOAqtYwBDYxYCzjUHPGZEz/Image.png)

There are using parameters that are quite real.  

Below I plotted something similar.  So it is possible that this is the cause, but I am not confident about it.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/C577173C-357C-4DBA-B8D3-F8A6B62BF4F8_2/7xGKESAaxiQYGuNnX1DhXGoAbUeKaEaNcBh0ANvQwpgz/Image.png)

Could this be an explaination, yes, but I am not exactly confident about it, I can’t lie.  FWIW, the mode solver could stop working with very lossy cores.  Maybe I am in that regime.  I should ask Martin about this.  Either way, these are some nontrivial imaginary indexes.

I figured it out. B8 has a tonne of photo induced loss. I was only able to go up to notch 5 out of 6 before exposure got screwed

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/39AA6297-FFF6-4BC0-9756-870C08E8029E_2/mFLNsTB5QKJVxZsvr7iuQmcFqoHzBmB0UYXGvcCj418z/Photo%20from%20Library.jpeg)

This film generally seems more lossy. Kinda a shame tbh. But that is probably what is causing the loss shape to change a bit.

Below are plots of everything in comparison

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/80AE7A4F-62AD-4545-8ABD-9B7B3E7A9AE6_2/5hzPD0xAtYZOGbsX41dZVUvTp21t2txOgpkuANHzyjoz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/E94BA3FF-7758-4861-9379-7BC8E09E971C_2/m1BXJFuCR8RHR7lypZWwr94yUfCQC6AdtEf7yPyxBFAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/EDC92B59-F000-4251-975E-6E9F7D098467/7759331E-BD0F-4F1A-B121-B9170EAC3652_2/yRAjFy1ztZs4XAY5co2HymCOq98kwo1pJGH7SbwGDI8z/Image.png)

Not as helpful as I hoped tbh