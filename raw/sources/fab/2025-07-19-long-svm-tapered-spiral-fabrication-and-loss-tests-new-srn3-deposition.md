---
type: craft-export
title: "2025-07-19 long svm tapered spiral fabrication and loss tests, new srn3 deposition"
craft_document_id: 70310769-37ED-4D7D-ABE9-98186D77650B
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-07-19 long svm tapered spiral fabrication and loss tests, new srn3 deposition
We recently had a lot of success fabricating low-loss, 7cm poling spirals.  They poled extremely well in experiment, so the goal now is to fabricate our final extremely long waveguides that we collect our publication data on.  We will start today by fabricating new SRN3 wafers that we will eventually anneal.  We will use 1 um oxide wafers that Gui ordered and make two new SRN 3 wafers.  We will first RCA clean, and then we will deposit for 65 mins after a 1 minute season.  We will post clean for 22 minutes.  Make sure to enter time as 1 hour + 5 mins, as that is how the tool likes it.

Confirmation of oxide

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-001.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-002.jpeg)

Beginning of RCA clean

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-003.jpeg)

### PECVD

We do a 12 minute pre clean and will then do a 1 minute season

Before season

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-004.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-005.jpeg)

Before main dep 1

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-006.jpeg)

During main dep

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-008.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-009.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-011.jpeg)

We run 23 min clean after. Index is slightly higher, but this could just be fitting noise

Before second season

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-012.jpeg)

Before second dep

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-013.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-014.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-015.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-016.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-017.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-018.jpeg)

We do another 23 min clean

We now do a 6:35 deposition of smooth oxide.  To make my life easy, we will do 1 minute season, 6:35, 6:35, then a 30 minute clean.  We will eventually want to do 3 minutes at 400 C if the stress looks off.  This is in preparation for the gamma

Before smooth season

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-019.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-020.jpeg)

Before dep 1

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-021.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-022.jpeg)

Inspection

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-023.jpeg)

No bow after

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-024.jpeg)

We should double check that later 

During second deposition 

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-025.jpeg)

### DWL 2000 Mask Writing

Something that we noticed recently is that our current long spiral is getting dangerously close to the maximum imaging extent of the SLM.  Our current spiral diameter is 4021 um, or ~4mm.  We know the maximum imaging extend is 8e-6 * 1200 / 2.16 = 4.4 mm.  8e-6 is the size of each SLM pixel, 1200 is the number of vertical pixels, and 2.16 is the demag.  So we don’t have a tonne more space.  We would really like to have a structure with 10 cm of poling distance around the spiral.  That is just a nice number.  We can throw longer structures on there as well.  The new design is below

[ASML3_Pass2_Final.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/70310769-37ED-4D7D-ABE9-98186D77650B/E31A4417-AB2B-4B3D-8F1E-12A02E0E9713_2/kM7NykD39MgDSQcC4htA49vp7lUahhtcH2PZ8ICAuvMz/ASML3_Pass2_Final.gds)

[ASML3 Pass2 Positive.gds](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/70310769-37ED-4D7D-ABE9-98186D77650B/1B674C25-3DA2-44B3-92E7-0AB2FC5B8138_2/Cd0K9r6kugXrXLNrccI4RpaGl7CFBsGx3gOyPFnK6xAz/ASML3%20Pass2%20Positive.gds)

I rotated, centered, subtracted, and reduced the vertice count.

For the longer bottom spirals, I have 70 um between waveguides.  Smaller than my currnet 115, but that is not undoable.  The top ones have 43 um between, which is going to be a bit tight.  The max possible poling distance is 14 cm, while the other ones will give me 10.  The bottom structures have a diameter of 4.3 mm (which is a bit close), while the top 10 cm spiral have a diameter of 4mm.  The inner radius is 687 um (so fairly forgiving), and the top is 500 um (so not unreasonable, but a bit less forgiving).  The top most diameter is 4.2 mm.  So this should all fit, but it will be tight.

Below is verification the two bottom spirals work

![Image.png](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-026.png)

![Image.png](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-027.png)

Now I quickly check the top longest spiral works

![Image.png](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-028.png)

![Image.png](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-029.png)

This will require careful alignment, but is might be possible. 

Our pre converted file

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-030.jpeg)

Setting up the job

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-031.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-032.jpeg)

Once job starts

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-033.jpeg)

Before developing 

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-034.jpeg)

Before Cr etch

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-035.jpeg)

We now do 12 mins in each bath

We spin clean in hamatech at the end

### ASML Job Design

There are two approuches to take here.  One could be space efficency.  In this approuch, we will try to pack as many devices onto the wafer as possible.  We would pick the average size between the baseline alignment die and the spiral dies (the spiral dies are roughly the same size).  Because stuff goes in the middle of each die, this should allow us to maximize efficency of our device density.  Given the pain it is to make SRN3 wafers, this is not an inherently bad idea.  Or, we could simply accept that our dies should be 9 mm tall, and just leave a lot of dead space between dies.  This would make cleaving a lot easier.  This would amont to 4mm of dead space between dies.  Before we had ~2mm.  I say going bigger is probably better, as cleaving before was a pain.  We can make it 3 mm if we feel so inclined, but ya, I would stick with truer-to-form sizes for the large spiral dies.  We will also need to load two masks for these exposures.

Job name

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-036.jpeg)

Cell layout

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-037.jpeg)

Image definition 

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-038.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-039.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-040.jpeg)

Image distribution

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-041.jpeg)

### Photolithography 

Before ARC on SVM

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-042.jpeg)

Before resist

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-043.jpeg)

Before edge clear

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-044.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-045.jpeg)

Masks are read

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-046.jpeg)

During exposure

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-047.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-048.jpeg)

Before develop

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-049.jpeg)

### Etching

We are going to do 5 min pre clean fo 82 and 100

Now descum for 1:20

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-050.jpeg)

Before season for 1 min

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-051.jpeg)

Now lets do 6 minute oxide etch

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-052.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-053.jpeg)

Before eco clean

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-054.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-055.jpeg)

Before piranha

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-056.jpeg)

Before nitride season

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-057.jpeg)

We now do a 5 min and 20 second nitride etch.  We then do piranha and then 10 mins of top oxide.

Before nitride etch

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-058.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-059.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-060.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-061.jpeg)

Index is BS with this little left

Before piranha

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-062.jpeg)

After

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-063.jpeg)

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-064.jpeg)

### Top Cap and RTA

I started a 10 minute clean on PECVD

Before season

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-065.jpeg)

Before main dep

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-066.jpeg)

During

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-067.jpeg)

During RTA calibration

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-068.jpeg)

During main

![Photo from Library.jpeg](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-069.jpeg)

### Loss test

1570 edfa main setup with 10 x objective

Bottom row dies from box, same length, different width

Straight 1

2.2 mW

Straight 2

1.9 mW

Straight 3

2 mW

Euler

0.9 mW

Bottom spiral

45 uW

Another die of same shape

Top spiral

317 uW

Bottom spiral 

200 uW

I rebaselines the setup on some old chips and get 3.5 mW for the straight waveguides. 

Going back to a new die of the same geometry as above

Straight 1

3.5 mW

Straight 2

3.4 mW

Straight 3

3.8 mW

Straight 4

3 mW

Euler

2.2 mW

Bottom spiral

330 uW

Top spiral

540 uW



For the long die chip

Shorter spiral 

423 uW

Longer spiral

Could not find

Another die of the same shape

Straight 1

3.3 mW

Straight 2

3 mW

Straight 3

3.4 mW

Straight 4

2.8 mW

Straight 5

2.9 mW

Euler

1.9 mW

Shorter spiral

420 uW 

Longer spiral

Not found

Another die of the same shape

Longer spiral

75 uW

Shorter spiral 

250 uW

![Image.png](../../assets/fab/2025-07-19-long-svm-tapered-spiral-fabrication-and-loss-tests-new-srn3-deposition-070.png)

The data is a bit noisey, but when comparing the straight, euler, 11.1cm, and 13.1cm spirals, we get reasonable loss.  The longest spiral is still a pain though.  Obviously I wish I had been a bit more rigorous in the measurement, but this feels reasonable.  Still a bit higher than is ideal, but not bad.  That all being siad, the numbers do roughly add up correctly.  2 to 3 also gives me some confidence, but those were also on different chips so….

Either way, I say we are good to proceed with the fabrication proceedure on the new SRN3 wafers.  While this loss is a tad high, we had weird photoresist and we did not do BOE.  This was also an older wafer that might have had flakey oxide as well.  I don’t think we will have any issues with the main fabrication.