---
type: craft-export
title: "2024-12-3 annealing resistant gds file"
craft_document_id: B907B968-D22C-4649-AD99-872E7A833532
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-12-3 annealing resistant gds file
Our previous devices seem to be performing up to expectation!  Now the goal is to device a new GDS file that will allow us to make devices that will not crack when we do a high temp (1100 C) annealing.  The idea here is that these high tempurature anneals will help us drive N-H and Si-H bonds out of the SiNx layer.  This will hopefully reduce loss at 1520.  It might also give us smoother sidewalls as an added benifit.  The general idea here is for us to get longer propagation distances, so we really want lower loss.  

The general approuch we are going to take is to etch trenches across the wafer that will help stop the stress cracks (which we found to work in earlier tests).  We will also try to anneal a larger piece, as it seems that all the weird effects happen at the edges.  A beta test version of this pattern is below

![Image.png](../../assets/fab/2024-12-3-annealing-resistant-gds-file-001.jpg)

![Image.png](../../assets/fab/2024-12-3-annealing-resistant-gds-file-002.jpg)

From Ryo, he would like us to use a waveguide width range of 3-5.  Because of the 0.5um broadening, I will do 3-5.5, which will really be 2.5. - 5.  I will do 12 iterations again. I will try to make the waveguides closer too so it is easier for Ryo to find them.  



After doing a bit more figiting, below is the final set of generating code I used

![Image.png](../../assets/fab/2024-12-3-annealing-resistant-gds-file-003.jpg)

![Image.png](../../assets/fab/2024-12-3-annealing-resistant-gds-file-004.jpg)

Below is a screenshot of the final centered, rotated GDS

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B907B968-D22C-4649-AD99-872E7A833532/BA416D8E-88E5-458C-ABB1-BFC5DDCD5975_2/ntuyingSxy0rpg16B00ygh2mmmdmy817bkqgu0Sex9Uz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/B907B968-D22C-4649-AD99-872E7A833532/F2B38AE0-EDD9-42F3-9360-D522C71D7924_2/uR7fqloRqcKxFfklZss1lChXRUf4vhazgdE4yfGX5T8z/Image.png)

Overall, turned out well.  Lets hope this works!!