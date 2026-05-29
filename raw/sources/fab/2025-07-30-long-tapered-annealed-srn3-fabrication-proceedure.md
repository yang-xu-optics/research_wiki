---
type: craft-export
title: "2025-07-30 long tapered annealed srn3 fabrication proceedure"
craft_document_id: 6038A08D-2D03-4A1D-A6B7-982B8F08DC0C
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-07-30 long tapered annealed srn3 fabrication proceedure
Winter is coming.  It seems we have finally gotten to the point where we can make 10cm spirals!  We are going to exactly copy the proceedure shown here for one wafer: [https://tdwg.craft.me/fqaECr3nRcY0Bj](https://tdwg.craft.me/fqaECr3nRcY0Bj).  When we measured the stress on the SRN3 wafers we deposited here: [https://tdwg.craft.me/idzUWVVxdYBYsl](https://tdwg.craft.me/idzUWVVxdYBYsl), it seems to be neutral.  We can check the stress again and do another 3 minute, 400 C RTA if needed.  That seemed to work in the past.  I suspect that stress is some type of transient thing.  

The one thing we might want to change is whether we put a cap oxide onto the wafer or not.  The reason to put a cap oxide onto the wafer is we know that process works and a warped wafer might not be good in the 100.  There could be He leakage and bad cooling.  In theory, this would only effect the oxide, but still.  The reason to do this is it might allow the SiN to reflow and outgass better, further reducing loss.  The Lipson guy also made it sound like this is the better approuch.  At the very minimum, we should put a thermal oxide wafer into the furnace anneal just to see if it warps, as it would be nice to know whether this is going to be a common problem in the future.

Below is the proceedure we are going to follow (I list it out for easy reference in the future, including the SRN3 deposition steps):

1. RCA clean of 1um thick SiO2 wafer
2. Deposition of SRN3 for 65 minutes.  This gives 2um
3. Deposition of top cap oxide using smooth recipe for 6:35 mins.  This gives 1100 nm of film
4. If needed to account for wafer bow, 3 minutes RTA at 400 C
5. Spin coat ARC on gamma (recipe 1002) and 800 nm of DUV resist (recipe 1206)
6. Expose in ASML using defocus of zero and dose of 18.  Do edge clear first
7. Develop in gamma using recipe 2010
8. Descum in Oxford 81/82 for 1:20
9. Etch oxide in Oxford 100 for 6:40 using CH2F2/High He recipe
10. Run 5 minutes in YES ecoclean and then run piranha clean
11. Etch nitride in Oxford 100 for 5:30 using CHF3/N2/O2 recipe
12. Perform piranha clean, ~ 40 second BOE etch to strip remaining oxide, and piranha clean again
13. Deposit ~3um of SiO2 using smooth recipe.  Do this with 8 minute deposition followed by 9 minute deposition
14. Thin top cap oxide (while preserving thick side oxide) using CHF3/O2 etch recipe.  Run this recipe for 9:30.
15. Perform RCA clean, and then anneal in 1200 C B2 tube for 5 hours in Argon.  Load at 300C, ramp for 2 hours, and cool over night.
16. Once annealing is done, cleave chips into their respective rows
17. Deposit SRN8 for 32 mins to get 2 um.  Do this 4 times to get 8 um of photoconductor with 19 minute cleans and 1 minute seasons between.
18. Sputter ~30 nm of ITO (including the material sputtered beforethe shutter is fully opened.  Cleave facets at this point and potentially polish facets

### Lithography

Stress before

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A781C459-8A5C-4790-8364-689A56B74777_2/yzasT3wwWD99fiUrKpAXB6bzx7aBO4wLp8cupKxIoO4z/Photo%20from%20Library.jpeg)

Good there

Ellipsometer 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A97C17A5-3C4C-45BA-B40A-2D120254A27A_2/iLfqd8bCQOLhBdxia854WiurkgBZzGy29VAIxXaYzWcz/Photo%20from%20Library.jpeg)

Other wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/AB44AB1F-AF65-4F3C-990E-714940DECB30_2/7BBaOZrzc2gne3SxxxRKn3U10SUE6pEDCIiSfXOfY0Yz/Photo%20from%20Library.jpeg)

Before arc

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/DCEDD0AF-B9E9-42B2-B403-F8462B36A6A1_2/RYzP0tJwlrDRcOYGhSBbZueLaIwxRaiEE10ldvHSuMoz/Photo%20from%20Library.jpeg)

Before resist

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/D9CAA582-48DA-4397-BD26-B80B60001A7E_2/wGliEV27mp3oQkvqI52u0rWLgXlausH9Nn78Qx9WUzcz/Photo%20from%20Library.jpeg)

Before edge clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/04D77BE9-49F4-46A6-B69D-B9BD1C4829B7_2/WXLeOmylR3FCVXDMS83aAhu1MFUFdv3GvCw39woKBXoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/E5FDCD23-65CF-4CB5-97F5-65B218BBC1DB_2/Z6mxZjTi8jpK1AIJjlYLzyesGo7C8BlWBhIxR0NqO0cz/Photo%20from%20Library.jpeg)

During each wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/66A7F43E-47A6-4B13-912F-D90FC16E8411_2/rdN1KT0SFJQn5GZT8pUiivTo6lAyGDzOyKsG33xeH70z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/E0CA1576-AB5E-4691-8026-D40AFB9C583D_2/iqGLzgDcX3YnzB3zSY1xxhCWphjd51smA8K9mCIgcq4z/Photo%20from%20Library.jpeg)

Before main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/7020E11B-B757-41BD-B4A2-DC9D3F7F6416_2/JFx20OauBU5vlYIpPepQxWmCyxVebOzyz7tlEYf4zNMz/Photo%20from%20Library.jpeg)

During each wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/4EE3A93B-2D49-4F19-B39D-AB468D7818F2_2/R5FkNkjoSczG54gy89ie1OjdKUB5WbAJs9pPZ3Figakz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/57203CAD-8901-45F2-83D0-186F04F945D0_2/eIpfQ1yWmk6IoYv6yz4SV4ndikbl165ecbA00AJxb3Qz/Photo%20from%20Library.jpeg)

Before developing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/890D9139-BF4F-4EF6-B47D-4860F9AAAB94_2/IdPA1mreVSyPKK9Zq7BCelj0VZwRAgwuJ6KWWxkMRIIz/Photo%20from%20Library.jpeg)

### Etching

We start 5 min pre clean on 82 and 10 min clean on 100

Before descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/075A773B-741B-4A8F-A4EE-36EAE3D8F304_2/iov65PxQWc5C8nLd9jFF5jUKPU5pJIgX5JoFq3UR7QMz/Photo%20from%20Library.jpeg)

Before oxide season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/33C29E13-3FCA-4615-A3E9-406EBCB4589B_2/ZoyOW8YVhpcmB0JK5ZwsDzqNBymh7ayb6AJ2lPpzycsz/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/4403F67D-A8AD-46A9-B278-F151C3E21B63_2/Fqt6OyyV6LG7ZmBnNYtzyDCmo5BVBF9zsYDqh6sDJPYz/Photo%20from%20Library.jpeg)

He flow is a bit high, but not catastrophically high. 8 or 9 is where I worry.  Lets see if the main wafer has this issue.  

Before oxide etch on wafer 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/88014915-3811-4E16-AC1A-8C9E627DFA97_2/IdTRGco5AIRLpVBX4UHnhs0uVcg9PdbPLXtmjFHtHQcz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/9918AA81-13DD-4040-9952-56092A22FC5E_2/SY8FjyxGXN6YB48fOHJRNyyIllzxzdW7mcq146dZ46cz/Photo%20from%20Library.jpeg)

He flow is good again

Lets now run an 8 minute clean

Before Ecoclean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6FB235AD-7CF5-4570-8472-15F5ECEDE7F7_2/HC5ZvyjfB1McnEHxfOCZinvI6pzQHvD71ElABy0VXiQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/EF7B18C8-62EF-4BDF-AE4D-0736A9F72DD2_2/RxMI5xOKS5nYqyywEqMgr7Lix4VFM67Mb94cGI2rbJoz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/DEC9A684-FE2E-4232-9C08-458DDA71FB1E_2/9PL30iHk3EPKBYn2U0zJlGjTRyI71gCnxnJuP5X0PLUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/730726C5-69EC-48D8-84C8-A37F003D27B5_2/aHdrDI0aHzTN8kgy08Ivsnj2WCwWEEH0llABMepaaKEz/Photo%20from%20Library.jpeg)

Microscope

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/AE83E5F1-4390-4D86-AF93-F31532168962_2/aPvVVd0GmqyLeRxzuI8mXJIDZwLZJSMNPnqwc3n3LZoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/B9BB6218-3458-4753-9DD6-CCA72C1A93AD_2/5GHgOjJpQTFxddGH4rt06etnQhkHWLE1xrqKcL2SfzUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/D3856A08-34A3-477C-965C-987BA92FCCC7_2/BqW6ue52n098KxpyjZe3xdUAOooRYzheC4yequPGHp8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/EF0D86D5-AB3B-4ED9-81EB-221BA7F0BF7E_2/TqSCJyQ1sBnXqgvBVoZ5kEH5sqZtx54xGuj7vhOhb5Ez/Photo%20from%20Library.jpeg)

We now run piranha clean

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/E0B1CDFF-8C3A-4EED-9C87-A40A1D51DC3F_2/9JJuQoFSywiSMywMVcGXnbsgKEttskPwuDxaSZmSjesz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/0F39705E-BD3D-4B66-B0B1-D38141467DB9_2/cCJxy77lw5IM4xvyhVuc9Z8umMYL1wNyWkuX7BJRyF0z/Photo%20from%20Library.jpeg)

Before second etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A9153792-9E4A-40FA-AE77-9A8F2496CAAE_2/x6l57CxoyctiCw7fyd9ZamsmSJSFKhxIJywfRk1zL4Uz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/AC9DDCD8-18E2-4151-A7EB-0C9071F2A83B_2/keyGDoP4OxwnMpjg1ec4aqDotwEIkZJ3SzOJO9g3jkQz/Photo%20from%20Library.jpeg)

Run 10 min clean

During eco clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/FD0229DF-2004-42E9-900B-268794F95783_2/lVJb9d1BMFC4cPpDXaaJAuULSMC3SySRyOVpaQ7vxFkz/Photo%20from%20Library.jpeg)

We now run piranha clean

Before nitride season on 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/07A2F5E6-BE7D-4E02-AADE-F5E82E490134_2/TCuPSzBE6J7sun8MQ3uSLkI9V2y6M6VIvzyd8tbKEk8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/3AE37193-C049-4F8F-AE94-13C0CBBEE400_2/lmVqb1wExDaiozF7JqMu1aNKityUKyP7C7FzvMV9oecz/Photo%20from%20Library.jpeg)

Before nitride etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/5B1CD3DD-0AAA-44AF-B2D8-B25A95F2AC24_2/ISgs4W6l6P0ugf16zN3av8NOju6aHiM0Dt8VLdEpflIz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/DFADC6E9-84DC-4B84-9D3D-280244E5069C_2/nccGYvMFqbdzh3jNUMEA6GmcRoAhHBv4Z0dkb9k6lfkz/Photo%20from%20Library.jpeg)

My wafer got stuck in the tool after this, so I have to stop the process here.  It does not seem that it will be damaged by being left in an inert chamber, however.  Roughly 24 hours later, we resume.  Start 8 minute pre clean on chamber

we pirnaha clean the second wafer again.  After etch data below

We over etch a bit

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/07744890-AFE4-4AAE-8D89-00CF703F671C_2/enRty9DhfKL6tC0DzLy49zwL2kyeg5UbyF65Phpd94Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A8C97BA4-CBF9-4E1F-A956-7AF3A5950A04_2/7D1sX8JNOJBAIn0IAoux7xQrn7xSnKKCQUH0K08fBd0z/Photo%20from%20Library.jpeg)

Let’s do 5:20 next time. We are running piranha on water now and will move to BOE soon

BOE is done. We now piranha again

During second nitride season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/067019F7-4385-4C9C-9DB4-84FE69BD14FA_2/yV15lz4rG3bNW8ZubE6Dls0TrR6jGecHBoGaxjJA4Xgz/Photo%20from%20Library.jpeg)

He is high. Hopefully it is just bad mounting. 

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/8986220B-0F56-4FDA-876C-7C8AAAC9F6DA_2/zTE33oPT6BYrT2z3fcSQgj5zmm84lzYDV3u5gu9KORIz/Photo%20from%20Library.jpeg)

During 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/78841508-E16D-4271-84ED-1028BF593FDE_2/tCiaNtn5hsItX9xf3ZPPSsLXGkchsBUN0iGH5n8PLMoz/Photo%20from%20Library.jpeg)

A bit later

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/CA9631CB-0AC7-4340-8C88-109A12194800_2/2Z6iExydLAJhsfkBOIaifi5u8ifHRSCmigPMRpN0yoIz/Photo%20from%20Library.jpeg)

We now run piranha

BOE is done too. After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/2A2C0352-8CD2-4E53-A176-73DAF4839F22_2/xgG8apRr71C7s6SUR80fPGmyWvuafVTzlypax2Nuqqkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6F05529E-D5C7-4973-A94C-273FC6165FEB_2/zNxu4KGt1hENDP1h95VGPUzzp9OqqEstoorDeaQAd44z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/2C22CA93-4F21-461A-8AA5-789292F89696_2/bsZNJmZl4KdwlfW5IyK4z2ujnnhb7eawyKHxoEhwyxQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/54C13961-70E1-4AB8-ACD4-522A75E254AB_2/1iVhby7fu5sn8lmWxkZBCsSzAcmTZTDy1v6FIwPhxAQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/57CEE8D9-CA6D-4034-992B-F8AB0D6BD514_2/Rq85MblsYYRZL2O2W1y8xipEYMbFrfhLeEUNCDr61rgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/3CD792F7-CD3A-4218-994A-FBB2D7398D15_2/mQcBazmqLDD50OSMpM6FD1aP5ho1uhMvlKPCNTEJwekz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/2D416E80-1EEA-45FD-B6BF-044EF82E5E12_2/P3tZQvlp9qxogibg1bijXkGaAIvGyrypHzbieDkgOQsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6B2EF384-9E33-4051-A619-CC2B4331D7B5_2/ZoIx1Vyz6LjKPUflyxxxWBW4MMKtcWkSCExCvAEKsc4z/Photo%20from%20Library.jpeg)

Piranha again and we are good 

### Top Capping

We start 10 minute season on the PECVD

Before first season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/F4C408E9-F73A-4A76-820D-7E0559AE4D9F_2/nL2qP0FrBqayhDRwSn3ATyInoj6oHrEcTbQJbAC0INMz/Photo%20from%20Library.jpeg)

Before first dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A725CD74-24E3-4154-85B3-ECC9DDC14746_2/oGi5iNu9NyBGPcRbMxsCekEjbaJu2YCGFncwySOIPdkz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/F810983F-AC5D-4892-8769-20EE7CA9FF91_2/QIIkqzzzNSFPsgkyejDi1wzrT2B3XVgwsOoRU1s5odoz/Photo%20from%20Library.jpeg)

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/CBCF1CA1-8EC5-4832-9367-220BA3874934_2/BEjj8MH1DZvj1Wxb2IbzaiXXQgDRlCymI8MjnyTRFNAz/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/EB4AFCFC-CE71-4CAF-AE8E-D1FB2A9802E4_2/9Ea1ecd5LY4yYUcPdVUUSi17KWTil0nUJPvU5hQADQoz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/94B6B952-7F3A-409C-946E-73C5040B0230_2/bZPPVC1dSesg1elyLbIoxlybtE5rtHlgvyBwoAtIFqsz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/B6312A8D-BD5B-4B15-8C9F-943FEA27E4DE_2/NKzvjXgUXWfU9xDlcTkxypARaQSsI1ZRzs8WY8A9o6Az/Photo%20from%20Library.jpeg)

We now want to etch to 1800 nm, so we want to get rid of 1600 nm

Before 100 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/CCD905AD-E6DD-48CF-9570-216C59D56F75_2/VFpi5bf69d3PkHiDsrtBI0rmbGFGXDruFiWrVU1HhvUz/Photo%20from%20Library.jpeg)

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/FD53367F-ED9A-4259-96DE-172F75A8B307_2/ls7EYO1Wm2f5wnp6lJevZKuqA5d40jVI69IXpSjl3Uoz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/3705A713-C0F2-4725-90B4-061B172916FA_2/5TpHDgdlg52CnM8HOCfxoVrU9yBH3mpgs0OS92KxepQz/Photo%20from%20Library.jpeg)

I am not in love with this He flow, but this step is less critical. Also, I don’t have 8, so evidently there is some seal

After, we got it spot on

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/8FB85FD6-2634-43C3-BD21-849783C94E2B_2/twXjb5a71jPAZImcr7thvmJODi5PyUQVxw39ijN6KlIz/Photo%20from%20Library.jpeg)

Before first season wafer 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/5E76B91E-4820-42ED-A36F-43AF6D56DDF0_2/evE5olIZiD2pE7zDy90FNCNTWJ6P0TGUAKx6vzmt1rAz/Photo%20from%20Library.jpeg)

Before first dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/B9ED544E-FA89-461F-9B1F-E881DB7EBA58_2/vmdfgQzoBpouPuoqixxyW4gM0AtHrvYPdSsBPy6PonUz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/04E7FC4F-EABE-4DBE-8386-773932C1B8CE_2/l3rSxsso281VBY5eor07sffBVEYRvAuBCsrEJ5TMKKsz/Photo%20from%20Library.jpeg)

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/DEC6584F-F1CA-4F77-BF46-A33F940508E8_2/OBcaU8ycgBjy9xHyFQs8yX07vmPFPM5FjmOAGtQeeC4z/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/DBCC9BAD-365B-4A06-A38A-FDCF8F1249A2_2/avJz8skNgHjQBBNrbPwXftjxz6nUGOyMzQtQ5dq18fgz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/F7BB0068-F265-4FFB-AAEA-D4B3F4CB8701_2/Cv6N5YKMojOEr6eCBRDI5bT0EnuO1JJdAYCUEtyHAPkz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/F16505AD-5A3B-4088-A9D8-357C82755533_2/lSJroHlXLlvUOVq9x3WOrXXD9GfS7zPwyAunHsx5gHYz/Photo%20from%20Library.jpeg)

100 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/9B291566-4708-4999-8596-1BA21432B4B5_2/HdHddO5oFxv8XxIKUnk65Kzo7H6X5NRxFLn6RFYrCAUz/Photo%20from%20Library.jpeg)

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/E270C7C1-6E86-4967-BCC3-3A9F061FCF7B_2/yOkQrV4MRz0NxLKoJXD7UZqzPTuUiWNWrcuSOil6gE8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/C5DFE3D6-43BA-40D2-840E-2B22DC7DE26D_2/DdmLbtntACRZj1Crk6wkbGa393UtMoJxiNaU6Wcoa58z/Photo%20from%20Library.jpeg)

Did not etch as deep, but we also had more oxide left

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A6D66FB2-2969-41B5-A3ED-4B3FD5130660_2/QWJH3FqcWUZ9gaF7yG0zPkDVNNyDDsh6cwWYnYR10o8z/Photo%20from%20Library.jpeg)

### Annealing

While I don’t think it would be a useless test to do something without top cap, given the uncertainty around warping, I am going to put top cap on both wafers and etch both.  I will throw a thermal oxide wafer into the anneal just to see what happens, and this wafer can become a carrier for ITO later.

We have our oxide wafer ready

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/00EB5DA4-8B92-47AF-9759-B56261C6F0A8_2/3AnCWZICXJXTAFv9sw8qtosVsfXVfrtfhfwaexKspeQz/Photo%20from%20Library.jpeg)

During rca, we started at a lower temp

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/424A6C3A-8071-468A-9C17-27F81D26A51B_2/GTQYisikxGHrLMqNi3w3a3GeinC7SEnKGoyemK5nFAAz/Photo%20from%20Library.jpeg)

Anneal is ready

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/AA31492B-2404-4208-81CA-B4F152ABC9B4_2/RGruF1fSBy98GEL3ZwzhmZLHbqwZTMKHmj377zxPFC4z/Photo%20from%20Library.jpeg)

We are loading at a slightly higher temp than ideal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/94DBB69A-EFE3-4FC6-9DEC-1C580ABA21EE_2/G0e2zXee4VJuJ8sHKFUZExvbd75g15pYK0VKrjzI3ykz/Photo%20from%20Library.jpeg)

Either way, I don’t think this is an issue. These wafers can survive RTA after all 

We are ramping

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/88FDE421-68EE-436D-8D0F-6B51082DE83C_2/49pKL4vUSyS6qFwI4K4C7J4v30H3R3RPZB6rWbK4KUMz/Photo%20from%20Library.jpeg)

Our Ar flow is a bit low, but so be it.

Near end

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/CA76DFC1-C7D4-48AC-8819-DC5716A29135_2/xpTTRQ9fLejEJcdCYE25c109FqVMTMbhqoj711LkbMsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6CBCFA88-A799-45F3-B52D-55E0C84E0328_2/7TPoZExAqOHaR8yW1CWxmU9GjNy2yapbedl8q3amJuIz/Photo%20from%20Library.jpeg)

Ar flow seems good now

We now let it cool

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/F64BEE6A-C4E1-454B-809D-4F29F9823F9A_2/oQRFwrz10DhuoZUeG7E874DhRXxmGF5pwDfyhmj4LM4z/Photo%20from%20Library.jpeg)

After cool down

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/7991B647-AB4B-4D6A-BDDC-0EA79B89E84D_2/Ut2JcHvNefRx2cQN4BA3WecrzG9WvxRhCjxb9qRWocwz/Photo%20from%20Library.jpeg)

After pull out

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/81053326-7C8C-4122-9B95-7150E58CEA34_2/YwaYlpHPp13zxQte0YbtUyvOBN5SIU3uCy4IDt3GzL4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/2A6E1D97-2899-4827-957E-81FB516CAFDF_2/Ja9DsIOCiVUkUrkIvw4f3D2GZwoBBEXPdIRley8mTigz/Photo%20from%20Library.jpeg)

Oxide has no warp. Our devices look fine.  I think most of the warp comes from the remaning SiN on the device wafers

After on wafer 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/43F24434-31BD-4336-8559-91A9672D91E8_2/iQmSV2iKuHGEIKin4VUab7ePmG3b3zl7fPnbYucKxkAz/Photo%20from%20Library.jpeg)

Microscope

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/7855434F-A756-4E49-99A2-0122C0EE1C41_2/tfUWVhyRhlPrMo9SrXsMPStKujUrs4l3M8YnpsRHr7gz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/E81636E4-D8D4-4645-AB5D-15FFAF3E789F_2/SH29rqxseKayjaimHX9EEGLFNQuNjsAnGfMfmvgHdzIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/2957F0EF-498B-41D7-BE0C-9D76965A95F3_2/5juELxGH1zlJfAqgAntJyLxZhSfR1tQ3kVnjZyZxjZ0z/Photo%20from%20Library.jpeg)

After cleaving, 3 very longs, 2 good widths. 



### Top electrical layers 



Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/04B58D3B-CC48-4633-BEA0-A553C884BB64_2/uUTZ8C08JA4gy5llOJXqDO7tNeIpx9OxkndI6a2NpTYz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/3D5D099E-E4F1-48B3-8DF3-619348068623_2/4OYLyCJAwVu4CDyB5QANbOtWXHG4ECk43JiVjdJ103Az/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/96896E3B-CDD8-47D1-9032-A1F5A0660298_2/eO0QdLvxIMwsLddPE4h4C2pNkfFbikoHmpGaH77VN4Iz/Photo%20from%20Library.jpeg)

No plasma issues today

We can only fit 4 strips, so two of each

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/0FBFFC67-6AD3-4EA2-ABB6-0DD74DAD4BA0_2/c8l5ZUAExr6jXFIhMht9anRDMr68SlCD2I4wlb1Dht0z/Photo%20from%20Library.jpeg)

Before main 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/0C088916-9488-43E1-BFE8-048273B55CBD_2/G0yD6WvxY0cVX3x8MHN6hGmERR0f2fXLbUKchfZFIrIz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/C4B55A4A-E2CA-45B6-BF53-ED0B90AC00A5_2/gNmADV2mvV8kJ1KyOanagLTAwtytUUh4yDWmepBIeisz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/997D0651-356A-42B0-BA40-F3091584D31B_2/8RknbWDHDEgiGspbHbDALwVLLhZZ3BZlMyyYfU7B6dYz/Photo%20from%20Library.jpeg)

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/5A3AD353-5853-45EE-BAEE-9C7F8598AD20_2/UEhlRSrMyDFyDzlW4WZqKlBySZK67QZTPgBmbmzfHSEz/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/61637594-7171-48DD-8B26-6DB53CDFAAF3_2/xW2pY37mTEe7hvsbgPdRLOXbbVylB8PHNDT9JrOHpxMz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/82E8E228-9915-48FA-80BB-CE8B40FB3009_2/SbLhU2Aljug1htPxTbjtFx8jRAslF3ZOjJU9NV8rpKoz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/3271CF4C-2948-4BEA-99E8-1E48F3BBAD5C_2/3BFYj2NxOQuTZkUJCCYxmzLbk9SNAfQ9tIWYa2FruOgz/Photo%20from%20Library.jpeg)

Before third season. 18 is probably minimum clean time too.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6EEDE0B4-8F52-4B3A-BDC0-CD8DA8A994F4_2/k0ANGLCxnuv5IwWyLyw0VSk6xCMnxke2rBe6c9kEZGoz/Photo%20from%20Library.jpeg)

Before main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6EF27C0B-9339-4F1D-A6C3-D0CBF283DBA5_2/ytg545cSwtiBcRZ4FQh2lPCHVdNkoySiyIfGP7jEIdsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6B7AB68A-FBDF-4E6C-8277-F88BCE16651B_2/s51B0tZoOHW7W23fOYgPWwcl67DYOxvGD4xfKdjRkGQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/643D8540-D209-4009-B719-D1B12B997162_2/xbhyukwC1l4y9Syv2qMUlc4K4yZSaTt2xyuJF0lllhoz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/AA56B39D-66D8-4CFD-8FA1-8D86F89C2B23_2/a9nOa3sEWx9TxEiwgbQjbZcngsc87EmoihBVQ0Ap2F0z/Photo%20from%20Library.jpeg)

Before fourth season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/DE363B8B-12C2-43C7-B8B1-FDD9EE85BAA7_2/1reJg425wYWF3AeGak6rDMjw6xLXFdwn4mFry88IEX0z/Photo%20from%20Library.jpeg)

Before fourth main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/CB78BF63-146B-485E-B656-A961057DD383_2/suIoAw1RPT3H9E0yC38yLsiyaNItyfH7k9TCcpZ7PFsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/6E9986E2-D0E6-4981-9BAA-2DA1B74EC239_2/cUlH8zj6yFWCFa750cgQ4ySuy2nf26C2EOc6o9NhNnwz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/B9374197-6AE6-4E1D-9C28-345DC8680B33_2/ckNMKdzS1pAp8jyinBlmbNyBJpD3PXXWNXBvI1nS5Hkz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/A33B10DB-029D-42E4-9750-3CA20363F676_2/OB6yJEveZGoqbDGMsj706AxxPu2m1yW2tfaFxdnX4eAz/Photo%20from%20Library.jpeg)

We now run 18 minute clean

Before season 5

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/7D766E4A-E751-4331-8D49-8CBDE3ABCE0F_2/g4Nwy0lCyYYdbQyZAAHX94F93lTQgXTK6Gi9xGzJFPoz/Photo%20from%20Library.jpeg)

Before dep 5

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/459612B0-5848-4D27-AEF0-AF98EC47499F_2/Wk6uyPSEx8nxkhO6myOPpxQInv05StRafRUJItHyZLkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/4D09B59E-4A20-4879-ABC6-1B56DB82B631_2/JTmF9NC4DqqfLpfzcRfJECTfL8UbqlWBhUJy05nwcr0z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/1A3E5CA9-FCE0-4891-A6F6-667D0F63F0CE_2/MSyiZu3hCWY1bgpvP6OaEYArLxuUJdqTd39oIqDEUUwz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/914EA04D-8206-4E45-A713-ADF899E0E599_2/M39s8TeaDcoYbRXG8yET54Vg3PyxpomVV9T3VT2rGYMz/Photo%20from%20Library.jpeg)

Before sputter 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/FA6C879B-E6FB-404C-ACF2-7BFB8D93A6BC_2/XIv7vagyRMMVuxAsWMdbhOSMfYtxc2ZG2LxNTPuRF2Mz/Photo%20from%20Library.jpeg)

We are pumping

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/D8A59F4C-1216-4DC0-AE3C-A280B9F63581_2/Y7O58njDfsjhYVrcR2mRt82hMGVb7veUnOny1hHReGIz/Photo%20from%20Library.jpeg)

At end of sputter

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/C622E12F-4F75-430D-B2A5-3ADE7FF5B88B_2/Z9IU5N8qf3OZWSiCyzCEElXqU3KYKX4MLCYoGYhjykQz/Photo%20from%20Library.jpeg)

After cool down

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/6038A08D-2D03-4A1D-A6B7-982B8F08DC0C/B6DA79C6-3F54-4363-B7BB-2B60EC9A04C6_2/mkBP4kTUThXXKgSfzWDhpVh6vOaBGxZruUd8t43X3Qsz/Photo%20from%20Library.jpeg)

Perhaps a bit more than ideal, but I don’t think this is going to matter much

