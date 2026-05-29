---
type: craft-export
title: "2024-10-06 final ln dc device design"
craft_document_id: 24FE4A07-302A-4DCA-8604-20E03C8F8EC0
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-10-06 final ln dc device design
This document is merely going to be a concise summary of our design parameters.  Below are the plots for ideal SRN (5e-16 to 5e-11) scanning over DON parameters

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/63aeca24-0d2e-6da2-81a9-17e1eb2beb00/Cqj9xYSrxa8JttzYIQ0QBM6ajSkS7hFBUzXZhbrJjagz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/7d9cb976-c1f8-555b-4917-8249acabbc18/8RlUZu6BvwQ8l8Ol02xbKaJvrmvkZ0C7HUYdzeFNs2Mz/Image.png)

From this, we suspect that, as long as the DON is around 2 to 2.5, we are probably safe with the thickness.  Cond0 is not super sensitive.  Next, we do SRN sweep, roughnly with the conductivity data that matches the annealed films.

B28

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/4a8c56cf-aa03-2d38-84d7-5abbaf6826c4/RrXBBJmj4aUZCRyitIMv9ZQ5JvgNwQQrgklTHArGnloz/Image.png)

Below are the delta_n simulations for cond0 SRN = 1e-15

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/ecf1fd0f-6d21-4c03-eeab-4f157e5680d5/obyUXKIPxd9pJ3BfPkGMAKGjNkKcktxxpwrZnV2ShEAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/b086f65a-553f-48df-3d2d-80d3ce34f70b/mzKXHF68qUpAKRjV6xpKvvqZ10AvJgj9boJv8NE6Hosz/Image.png)

From this, we suspect that a thicker SRN is better (as long as we apply higher voltage).  I say a thickness of 2 um should be fine.  From the plots below on Bright and dark state conductivity, we can find the optimal SRN

![Screenshot 2024-07-28 at 3.19.05 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/ee37a014-9923-fe4d-4209-4aa0b8a5c83c/0mwFz0xZu0MFh5TSdbWtgjupgR8aicERllW2pJZOOcYz/Screenshot%202024-07-28%20at%203.19.05PM.png)

![Screenshot 2024-07-28 at 3.18.55 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/2970c52e-c6bb-b928-e586-115674a74c3f/DxO7CNmkBFQdgemPboi504qb5tf2XKCoCPSGYxpA6VIz/Screenshot%202024-07-28%20at%203.18.55PM.png)

Looking at the dark state, anything between 4 and 5 sccms is good.  More silane is good because we can use lower voltage and have less substrate loss.  Less silane is good because we get better modulation efficency.  Below are the indexes I think I will use

DON

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/b62698e5-39eb-b54a-568a-0261336efadc/s2yzkMgT9QGlSgGMUfxUvgrCZS4GfuC8tqeBIDFYAj0z/Photo%20from%20Library.jpeg)

SRN

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/0271fc2f-8c97-30c8-b578-f415100df683/6n6f8BB2Rkbfy7drGf5fqX46D5DlcQase1P6gfP8eCUz/Photo%20from%20Library.jpeg)

Below are the index related results

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/75D9E445-709E-48B4-9FC7-A5FDDAAB0CB6_2/wSiHOqjz4FNQa0e04WBA05AThrsWd8Xk712LkLUowvMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/257BE42C-2AAE-453B-B73A-8274C608D149_2/zd7cxnhR4ddkPOw4gkDTlA6xZBwnwHMZvVVyPrdU114z/Image.png)

This is probably fairly optimal.  I say we still try to shoot for 2um for each film.  

Our final stack should be 2um DON B28, 0.7 um of X-cut LN, and 2um of SRN 4.5.  For the transient solution, we get

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24FE4A07-302A-4DCA-8604-20E03C8F8EC0/EF76D15E-AA83-4E62-9C8C-0389C86FA471_2/JtxDE3CYwMyL6MdKG1BgEfs013W3bAaDe2rYaSp3EaYz/Image.png)

Bottom is dark state, top is bright state.  We get ~1 Hz operation speed.  Again, if we used more conductivity SRN or cladding, this would probably be faster.  The voltage here is 460.  A little slow, but oh well.  

