---
type: craft-export
title: "2025-02-25 reactive sputtering for al2o3 literature search"
craft_document_id: 7931E304-D658-420A-9BF6-DCC3EE26BD37
craft_collections: [fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-02-25 reactive sputtering for al2o3 literature search
It seems that I currently have a bit of a scattered literature search on Al2O3 sputtering for UV waveguides.  Lets put this in one spot so it is easy to see what knowledge we have gained on the subject.  The first two papers are the ones I have been suggested/have been working with thus far

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/0040609086903913?via%3Dihub)

This is an older paper that carried out optical loss measurements at 633 nm.  While they did not do reactive sputtering (which is what we eventually want to do), they document RF sputtering decenlty well.  They use an Al2O3 target

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/4D185D66-55ED-4F6D-B468-4DE9AEB4AC6A_2/fMDBVUAYny9nMER1dhhCSlb6Jxx2qHniH29MMjwaNm8z/Image.png)

Above are some important constant process parameters.  The O2 here must be inert, as it should not be reacting

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/FE1E7FEC-CDC5-4497-8BAD-0EAB3034264C_2/LQWGuUpm2F2bGKQ71oTdFAYomk1zWFJIkpeaYz8Fx2oz/Image.png)

This figure basically shows the importance of annealing for RF sputtered films to have low loss.  It seems htat 800 is ideal.  Oscar mentioned that Al2O3 crystalizes above this point, so that is probably why they want to work at that point.  Unlike PECVD, they should not have any H impurities (which is why I have annealed those films in the past).  So I wonder what the impurity is here.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/BC8D5884-DE20-4ED4-B92F-F1A9517F2BD3_2/bh9XH9eomxTqd7h3oG92eDpDU73f8fWorrglvKbJRk4z/Image.png)

While this is not mentioned in this chart, the e-beam films do not have good adhesion.  We don’t want to purse that path right now, but good to know. In theory, if we wanted to purse that path, we would just e-beam evaporate Al2O3 and HfO2 (as I don’t think reactive evaporation with O2 exists).  This would be hard anyway, because I don’t think any tools can co-evaporate.  Maybe if stuff could be thermally evaporated this could work, but I digress.

For the chart above, all the films were annealed at the optimal tempurature and the best loss was reported.  The ideal anneal tempurature varied from process to process, but it seems that the smallest loss did not depend a lot on the applied power

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/65E98B33-A5AF-4503-ADF1-CCFE38281C42_2/dLee7BdcytTJcgLWX0tO7zp4nc59v6KcLikjyTdlcfEz/Image.png)

While the films densify like PECVD ones, I am surprised how little the index changes.  I suppose this makes sense, because PECVD films outgass hydorgen, which lowers index.  I think here the films just become more dense but don’t chemically change as much?

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/06838E14-25F0-4005-B76C-994A267EDD39_2/zzaQ6WhSW0Fu8Mnc9kitIFy9eE7cmyuyFcFVEMPd0q8z/Image.png)

This kinda makes no sense.  They claim films are very compressive at the beginning (which is possible), but that stress disappears with annealing.  This is not explained by our recent experimental results on Si and SiO2.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/A171DBD4-4325-478C-9D20-64736B434F8A_2/duLGJxmwUxNQYWhNHa8GJuFltgZATrsytLLhFxhxdh4z/Image.png)

An important note is that the applied power and bias voltage seem like seperate variables.  Anyway, it also seems that applied voltage mattered quite a lot for loss.  For our baseline recipes that we deposited the other week, we used 94 V_bias (though it is a little hard to tell reading the recipe).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/0C446CB1-49F9-4A3C-BCEF-508C0173AF0A_2/YNn8ePcxEPoWx0RQTmVnkOUyIflyecqmsK0X6wFVQwAz/Image.png)

While the chart above is for e-gun-evaportated Al2O3 (which is very different from what we do), it generally goes to show the benifit of extra oxygen.

**Summary:**

1. Annealing RF sputtered films at 800 C seems possible to getting low losses (a couple of dB/cm at 633nm).
2. Ideal annealing tempurature seems to vary slightly based on deposition paramters, but deposition parameters don’t seem to have a huge impact on loss after optimal annealing

[UV-waveguide-final.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/CF926AC1-5F80-439B-BDFF-36FA1B716D8E_2/RGdD93YXYAChFCuRqsG5sem5JEggl8p7iXSkEaYXzpkz/UV-waveguide-final.pdf)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/A51DA9D6-3330-48AE-8C0F-2E53B751EE1E_2/MBTc6tJdqpU6eFQx6K52vetGYoR9nVIzcaCsYstN7Soz/Image.png)

This is a summary of the main result at the end of their introduction.  Interesting that they use RF sputtering, as it really feels like using an Al target is better with DC sputtering.  An important note is they do a post-anneal at 1100 C, which is surprising because one would really expect there to be severe cyratallization up there.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/FAB3E2D1-4558-4BBE-A17E-C96423C1DBB5_2/LVyk6gTWZ6u5VCSW5hhXuiFVefHgcxtk3uRM5znzrqUz/Image.png)

They do in fact use a pure Al target, so the RF part is hard for me to explain.  Maybe they want a lower Al sputter rate so everything oxidizes?  It seems that the substrate tempurature and oxygen flow are most important.  They also use slightly thinner films than us, so maybe that helps them with stress later.

They also use a metricon, but measure loss at 377 instead of 405, so their losses should be higher than ours

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/DE3CDA65-4A2D-446B-BC4D-E553F526B927_2/1iL51byD1oQSm4xtxpQwRfTZ3VZ5i3w13bOxqoFzWEoz/Image.png)

This is an interesting and important note.  They polish their waveguides before annealing.  I would suspect that our roughness values will be similar to their’s.  Fortunately, I do have an idea of what polishing recipe is best should the polisher ever be repaired.  It is also worth noting the index so we know what we should be matching (I assume the index is at 377 because that is their test wavelength). 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/FF563C10-0767-425F-83BD-FC22A258DE45_2/3fVwNir9IilnAy3wh5txrNNFWFqkJGm8ES1Kl45tanoz/Image.png)

The part cut out was SiO2 LPCVD.  Given that they deposited at mid 700 C, the films should survive 800.  They used an N2 environment to anneal, so it does not seem that AlN is formed by this.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/0FA66155-B81D-4943-8C85-78C2DDE56171_2/Y4x2cdIH16QMQyCTh1Cwy5iesuVmhbpVyu8xnFhppAEz/Image.png)

Above is slab mode results

**Summary:**

1. Even if you use reactive sputtering, you don’t need DC
2. While the paper did not totally back this point up, it seems that deposition tempurature and oxygen flow are very important for reducing loss
3. Polishing will likely be nessesary.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0040609012008863)

These people DC Sputter HfO2.  They don’t do optical studies in the UV, so I have no idea how good their films are optically speaking.  This is just to get an idea of how they do it

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/F6419920-BF05-467E-91B4-96F771DCCD9D_2/kO8Dr6mldGJEQjyrChCLmDLQRcyLPyI6ArCrHmvvuvoz/Image.png)

One sample was annealing at 800 C for 1hr in air

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/401A444E-8252-4BB9-961D-AD835C2A16F5_2/FM2IZBRzOCsotCLQcIIMn5tWQt2ViA9FfAjRTiWsYfoz/Image.png)

The above plot just gives some idea that roughness will be an issue.  The rest of the paper is not super useful, but has some nice references that we may want to come back to.

[Low-loss and low-temperature Al2O3 thin films for integrated photonics and optical coatings](https://pubs.aip.org/avs/jva/article/42/6/063402/3314948)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/C6441B35-9CE8-4D9D-A423-2F82BE4D5B7B_2/vfmbxU5VXp7CqFc3DWXXJ2YA9B7Lc6JRis6SyxnMZaAz/Image.png)

Abstract above says the important part.  This is low temp sputtered Al2O3 with decent loss for 638 nm (1 dB/cm).  Not exactly what we want, but we can pull some of these parameters for our own means when designing recipes, as I imagine annealing will help.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/918CC9D3-393F-4228-A67F-EBEA8C5D55CD_2/U6w4noelt7ecKtxK5vuNshiQ0aLo0HUtqCzlC5XqeuUz/Image.png)

This is not about their fabrication process, but it is interesting that they seem to suggest RF is best for low loss, but requires high anneal temps.  They also give a tonne of references, which will be useful

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/4A88F459-46FA-48D5-80C7-BDE3F4D91D02_2/jCy5asDSiiM6L0idya1cPN9F6N9vBgSAb5T96gZO3Akz/Image.png)

Another interesting point about how sensitive the process is to temp.  I do hope we beat the dep rates, but 6 nm/min is still way better than ALD.

One thing that I don’t think we can fully replicate here is they use an additional plasma source to enhance reactivity.  Apparently this helps make denser films.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/B01292B9-A2E4-4DE7-B55A-05D8FF0682BF_2/HrG7I3B2hOVZZFf4VrwpA1VrD2wN1qAMgUmaGrcpgDQz/Image.png)

Above is the description of what makes this somewhat novel.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/B0B9302D-1881-4BD5-B70F-3AEC27CF1DD7_2/UE83Z5FWWMkWbsCM4vNfyLx2vwQsgTpp03FAC3mWO6Az/Image.png)

This make a point to say the chamber should be preheated before deposition under high vacuum.  The way this allows the films to be of high quality is still a bit unclear to me, but this might be a trick we can play later.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/98364357-6071-41A9-9C40-C8513BD9DECF_2/PxCV14waZMrwh9MyrPWmd1L7ISKGx7k1J5RllHFnGNkz/Image.png)

This excerpt is most nice in explaining how RF and DC magnetron sputtering work.  It seems that RF is more stable and prevents Arcing, which is whyere you get a discharge from target to substrate.  The reason is DC mangetron sputtering can form a static charge build-up as the process goes on, as the target will inevitably get a bit poisoned.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/AAEA4021-379C-426F-8E4C-1855BF0A6EB1_2/Vbj2wCNUMVpi6CCD0veFiMe7MXc6cNlMxQSTUedKkVcz/Image.png)

Again, just a nice description of how reactive sputtering is tricky.  It does seem that too much O2 is bad, because even though you get a nice dielectric, you substrantially decrease deposition rate because there is no new source of Al to sputter (the target is covered in dielectric)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/4DF9D28E-97AE-48FB-9909-51E4B002C94E_2/q3hrVx5BhT70noEx0YyWsIcM7GOUErOxfe8qvQhw3xQz/Image.png)

This shows the hysteresis, where too much O2 flow effectively stops despotion.  So you would seem to want around 14 sccms

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/529FEED4-F77F-40D7-928D-FCDA7CD555E7_2/hzuVJlnqJn1yh31C0xftPhpxxzXEuLHxKKBWbC9K5Goz/Image.png)

Annealing seems to help with loss (no surpirse here).  They do N2 annealing for 4 hours (which is a bit long)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/F315356D-99C8-4786-80F1-18D4693EFBD6_2/Ko5vZCMTI1x3nhE8HG56FQxhQFwiSJ8uyUipbbSociMz/Image.png)

It seems that having some active votlage feedback mechanism is best for maintaining good deposition, but I cna’t seem to understnad the discussion more from this.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/B9959720-EA04-411A-83F4-8CFEFAB81118_2/kE1QdV9V85g6SRViE9t7fhkybDcjQsEbKyZ1LAy1H3Mz/Image.png)

Other deposition parameters are power = 1300 W, Ar flow of 80 sccms, pressure of 0.8 mTorr, and tempurature of 150 C.

**Summary:**

1. There is a strong hysterisis with O2 flow.  It seems like saturating O2 flow will reduce deposition rate at the very minimum, and may lead to arcing
2. It seems that RF sputtering is a more established process for getting films that display low optical loss.  We don’t care about high tempurature, so that route should be fine for us.



[Rare-earth ion doped Al2O3 for active integrated photonics](https://www.tandfonline.com/doi/full/10.1080/23746149.2020.1833753?scroll=top&needAccess=true#d1e511)

This is a quick summary of RF reactive sputtering, but it gives a nice graph below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/21B65B0E-0460-4C50-BCF9-B647C4D99D26_2/tBQWVxBSVbYA0gzoiei7OGPahU4uh9CIEhgqkAkRyP0z/Image.png)

The x-axis is a bit unclear to me, but it seems they mean oxygen flow as a percentage of the total Ar+O2 flow.  They do give a starting idea of a recioe (though no Ar flow).  These people odn’t do an experiment, but they mostly seem to be doing summaries.

[Optica Publishing Group](https://opg.optica.org/ome/fulltext.cfm?uri=ome-10-6-1451&id=432163)

This is another good paper from that group in the Netherlands

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/95B66781-0CA9-4500-8958-DEB6014F2A8C_2/0qsTiy7n2a8mx9xgC1b1UwwmQubRubJoxBOuAK8HeA0z/Image.png)

This is actually a very interesting point.  We only go to 50 uTorr before we open the chamber, so it seems we really need a much better vacuum in the loadlock before we start.  Granted, when we open the loadloack pressure does go down, but it seems we should wait longer.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/F79EB23B-1E8B-4303-A54D-4E57425D2C54_2/b4ck6ZZ7jFm4ApcwYL8Tens10PWI1FwjAxpaPBnqZoIz/Image.png)

Power = 200W, Ar flow = 25 sccms, O2 flow = 2-2.8 sccms.  This is a lower oxygen flow rate than their previous work, but I suspect this is because of the tempurature difference

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/E5FFB3FB-A82D-4525-AA6E-3765CD44F79B_2/WAqLCTmM1CxKtjFZr11xoC31jiUEFRqLyFRJ1LQvkYIz/Image.png)

Temp = 580 on the check and chamber pressure is 4 mTorr.  Given the tempurature difference on the wafer, I suspect tempurature is something we will have to spend a good long time calibrating.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/65376254-ADF5-4EC6-A073-2AEAA1A9B112_2/yBlX5yySJskqgZulxLlFQnBgRtBseUI8guyCDNeseNsz/Image.png)

This is an interesting discussion of these voltage bias curves, and helps clear this all up for me.  It seems like we don’t control bias voltage, rather it is a feedback mechanism from the tool.  They are also interesting that they calibrate this each time (which is a procedure we ought to develop fast) and they pre-sputter the target for a while before deposition.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/D0EA7B0F-2F1B-4CD0-BC0D-0439234223F6_2/ixPhz99RI9CsbqHVY7l5PONkDUT6TMdcp4vGVho5J1Qz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/0CFD69E1-F360-4768-9D62-13399011EE2F_2/Zahfez3B9yRTE9b1f7D7ZFSriay6CpXDuqmxRL38xS4z/Image.png)

Above is a summary.  An interesting note is they really try to work in the zone before transition.  They want the end of the metallic region.  It seems like the main benifit of being there is you get much faster deposition rates.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/5A9B43BB-8138-445D-8C8D-4E4DCBC00667_2/v9K53eWBAjLR6GvczPEZx7N2SnI8x5MrmZpwjzH00gIz/Image.png)

We should also see the ideal bias voltage change with use, so it may be prudent to recalibrate this every-so-often (though it seems like ideal O2 flow is the same).

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/2BCC683C-2E0C-4DD4-8E8D-5633B65635FB_2/b8W7Ei2OtSn2NwOoLP4JKpLdpghGt6QBpmth5EE1ii0z/Image.png)

This is another interesting bit about loss (all indexes are for 633 nm).  Basically, if the index is too high, then you have a polycrystal.  If the index is too low, then you just have incomplete oxidaztion.  This should be helpful in characterization films.  They seem to say having an index between 1.665 and 1.685 is the best.

As a last note, they seem to make a big deal of the oxidation potential of the target.  They suggest having this value at 5.  This seems to have to do something with the aluminum target degrading.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/12910E95-E45C-49FC-BD70-8E669338E684_2/mS68CVOiVAbqN03G7p1E43ut0n2UQShhWc1gVITWGiwz/Image.png)

Notice the same scale, so each individual sputter should be fine.

**Summary:**

1. It seems that Al targets degrade over a long time
2. You really want to characterize your hysteresis curve for Al2O3 to see where the optimal O2 flow is
3. RF reactive sputtering seems like the norm for low loss (not DC, as it seems like lead to arcing)
4. They provide they deposition parameters, but I suspect matching their tempurature will requrie some characterization.

[Reliable Low-Cost Fabrication of Low-Loss <formula formulatype=“inline”><tex Notation=“TeX”>$\hbox{Al}_{2}\hbox{O} _{3}{:}\hbox{Er}^{3+}$</tex> </formula> Waveguides With 5.4-dB Optical Gain](https://ieeexplore.ieee.org/document/4810183)

At this point, I am mostly just looking for more recipes so I can start to get my average to converge to the true mean.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/5D18F56F-4C76-4A77-8604-2447D8D14138_2/CbwqrCdQD2cHyuZyfw33IPHBi2w64n0CMkHEa0U0gU4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/C2CA5284-8691-4279-9B44-6219BF04AF9B_2/2yVDcxOqIx4H0kBJwgWlt2k2tkK9u0NY203JYKiSxCIz/Image.png)

It is interesting that they again make a point about this long vacuum time as a way to reduce the amount of OH- in the film.  This is definately something we need to pay attention to going forward.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/67363151-0431-4A7C-9184-5907C95B9106_2/OGgAuLMihaAId8gXbwNxGzFS6Oh9gDfj5V55DbgpWo8z/Image.png)

It seems that power really only effects dep rate from what they are saying.  As expected, DC is faster.  At least they give us a DC recipe, as it seemed most other groups were a bit scared of that.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/F0494A65-5D35-4A35-9FA4-61F09F5908B8_2/yKc4lo52LqqVRhEX69fKvqJ5xxF5HOh0rMSrTJVN2BIz/Image.png)

An interesting bit here is that apparently, because of this arcing behavior, DC films are less dense than RF ones.  It generally seems like denser films (from RF dielectric sputtering) are better.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/2B11BEEF-05DA-47ED-9CC6-209EE625B517_2/9eCVws1y00tXMM9LZ4G6naycuRSg8ErNqlGPqIqHyJ8z/Image.png)

From this description, it seems like a lower pressure is best, as higher pressures cause clusters to form which lowers film density.  Maybe this is something that can just be annealed away?

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/C555F788-2A4C-4F38-888F-BC8042B0DF26_2/gn38GhRlmnya3WN1TxpxNQ0kznxntlHnwdyKWxKGc5sz/Image.png)

A really nice comment here about refreactive index and loss.  Their main point is that index at first increases with deposition tempurature, but than starts to go down.  The two main sources of loss are Al-Al bonds and voids.  I feel like some of this can be solved with an anneal, but this motivates RF very well

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/F9D14DBB-49C3-43C9-966C-5F730EB0A2D5_2/atyiFnJgyqsoyAxP8F4bwTSTrNr7qLoERx30qRCp6Ncz/Image.png)

This loss is for 633.  Goes to show that higher dep temp is better.  They mention later that losses could be better for higher dep temps with RF, but their measurement system is not sensitive enough to measure those effects

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/4F07ECB4-B36F-412D-8A6F-028EDD7CAD28_2/CVHxY79NkxWOT5Qhu1oQyinwKNzB3tmTdZ7FmPsQGDoz/Image.png)

It seems that pressure, power, and flow rates don’t matter for loss a tonne.  That being said, it seems that less flow, less pressure, and more power are slightly better.

The rest of the article is about Er doping to make waveguides with gain, which is probably not relavent to us at the moment.

**Summary:**

1. It seems like higher deposition tempurature is genearlly better.  No one really seems to have a good explaination for why you should not deposit at the maximum tempurature, but maybe their tools are just limited
2. This once again confirms that RF sputtering is better than DC, but at least they give a recipe for DC
3. We want fewer Al-Al bonds and fewer voids, as these are the sources of loss.  I feel like voids can always be solved by annealing.
4. More power means more kinetic energy of the deposited atoms, which allows them to fill voids
5. Lower pressure means a longer mean-free path, so atoms have more energy when they deposit and don’t form clusters before deposition
6. Lower flow rates are nice if possible, but the hysteresis behavior from before is the most important.  Considering that we don’t need crazy high dep rates, I bias towards lower flows
7. We want to leave the wafer in vacuum for a while before deposition to get rid of OH- groups.

[Synthesis of Alumina Thin Films Using Reactive Magnetron Sputtering Method - IOPscience](https://iopscience.iop.org/article/10.1088/1742-6596/850/1/012022)

This paper is not super detailed, but it provides another recipe for us to form a better mean

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/F8340364-6B41-46CB-AD44-4A810DE803A1_2/s9X8Uinw9rM6S97OMFW7XzdgTYK289AF4uFahjxiJigz/Image.png)

They use a tempurature between 350 and 400.  Oxygen flow between 2 and 8 sccms.  Dep pressure of 6 mTorr.  They pre-sputter and sputter at 100 W.  They used 5X more Ar than O2.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0925346720310326?via%3Dihub)

This paper mostly covers Er co-sputtering with Al2O3.  They do have some nice characterizations of the films with just Al2O3, which are below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/795E055C-AF2E-430F-B05A-AE956C242A1F_2/yl95pUiHN1suLiPCKKDw30xju3dcONb4xAy6FxxSM4Uz/Image.png)

An interesting note above is they seem to show that using the highest possible tempurature is not always the best thing.  They use O2 flows similar to others, in the low 2-4 region.  I am not sure what this substrate bias number is about.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/C1C97553-1E95-44F8-9E1E-207A7370B3A6_2/LIni9KFujdxZ1FQxsd9WwLxtOCPBFLw2bBTgKg3I3QUz/Image.png)

They use a lot of Ar flow compared to others, but the consistent use of 200W is reassuring.

[1036987539-MIT.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/5B4476C9-6A9F-4DAA-BD8F-4E5CFE0D133F_2/2uqNadHfGzZKnBkKOaVmMoomTxUNAQVjf10lsMvb6D0z/1036987539-MIT.pdf)

This thesis is mostly about Si photonics, but it does have some helpful notes about Al2O3 deposition

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/0B2E602F-79BC-4043-AEFE-2142E597B2B4_2/cMyAPIXmvaG8r12eWWKLlYxPaNyJnSulzdPC6RfxtVMz/Image.png)

An interesting note is that we actualyl have one of those Lesker Sputter machines in the CNF, but it is mostly used for ITO (which makes sense, because that is a reactive tool).  Maybe we should investigate that tool as well.  The pressure seems reasonable and the O2 flow seems reasonable.  They use a higher power than other papers, but most of the previous papers did not show a negative effect for higher power

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/853935A5-F5BC-45AA-9823-806948A78952_2/yCiW8vRnvVU6amOm9sACmKXPCT7eYx2x4w0wWZdlf4Yz/Image.png)

This substrate bias is interesting, and I don’t fully understand how it works.  Here, they show some seriously negative effects to higher tempuratures.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/A80B1E84-3E51-4F4E-91A3-203E74D4F32F_2/Jkdo6v4VbMxC1pi52tcmzCmyxUKfBdibJr8ZsELv7t0z/Image.png)

The explaination of low temp problems is consistent with what we previously read about, as the lack of kinetic energy forms clusters.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/90429E58-8231-4647-ADFF-82C531C794FB_2/3wPeZtdmu1ZqLupSsGHBlKoRzYVDhGmJzmZpSs2Uy2sz/Image.png)

This is the first time I heard about poly-crystaline formation for higher temps (though this makes perfect physical sense).



I think we have seen enough papers to start forming some initial impressions.  The general conclusions from this search are below:

1. For O2 levels, we need to do a Vbias scan.  The idea is we want to work ritght before the Vbias starts to drop, so the edge of the metallic region. 
2. We want to leave the wafer in fairly high pressure for a while to get rid of all OH- contamination
3. We should do a 10 minute pre-sputter with the shutter closed to get things in equlibirium before we start the real sputter
4. The main modes of loss are voids, Al-Al bonds, and nanocrystals.  It seems like the latter is caused by tempuratures that are too high, while the former is caused by tempuratures that are too low.
5. It is unclear what the best tmepurature conditions are.  For annealing, others used an N2 environment, so I am not worried about AlN formation.  It seems that post-deposition annealing was really only used on dielectric sputtering, not so much reactive sputtering.  Some papers used in the 700s as the sputtering tempurature, while others used lower.  I think the crux here is (and one paper mentioned this) is that the deposition “tempurature” is not what is actually expereinced by the wafer.  It seems like we should start a scan at 200 C and work up till 600 C
6. RF reactive sputtering seems fairly common.  The advantage of reactive sputtering over dielectric sputtering is RF sputtering has faster deposition rates.  DC sputtering seems likely to lead to arcing issues if we want nice dielectrics
7. For deposition pressure, anywhere in the low mTorr range seems fine.  It seems low is slightly better at preventing clusters
8. For Ar flow, it seems like 30-50 sccms is roughly fine. Others used 100 sccms.  It seems like a slightly lower is better, but I don’t think this knob matters much.  The people in the netherlands use less.  I would probably say we go lower to stick with what the dutch did
9. Power seems to be fairly consistent at 200 W in most of these processes, though higher was used.  This knob does not seem to matter much.

Below is an additional paper I was sent

[Reliable_Low-Cost_Fabrication_of_Low-Loss_hboxAl_2hboxO__3hboxEr3_Waveguides_With_5.4-dB_Optical_Gain-2.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/5A8A5AAF-B00A-4D25-96A3-8B16B4150B5B_2/Jn9RmYM4tjVEKgZCOTzpnT9TQYI6lgZp7h5jUBdeDmIz/Reliable_Low-Cost_Fabrication_of_Low-Loss_hboxAl_2hboxO__3hboxEr3_Waveguides_With_5.4-dB_Optical_Gain-2.pdf)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/DB57DC68-A3F5-4887-BBA4-5F32D4E74771_2/btGdd7Fn91xIurvNOfFyJ82rx9z3FVScKnsxvWzSw6kz/Image.png)

Above is their process, which is largely in-line with what we expect from the Dutch group

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/1CBDFEF8-4C61-43CC-8FEF-A487D0866F15_2/7Dl1zUHS0ewh3xxJajZFxb4tWxTioMHwvNmYvJJ2pnAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/8923E5DF-EBFA-4832-A3A3-2BE73F46B876_2/NNTDAEKHvgej4yo2vfGPDeoet73qTBLUEvfoHAsyxHwz/Image.png)

They also do the same tricks as others with higher vacuum before sputtering and a 10 minute pre-sputter, which seems sensible to me.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/9752D8F8-7DEB-4321-ABAD-25E706573284_2/TOfCq849Llm8FnWQOZ80PvwUAmlsRTwVf9Dzy4uwOpUz/Image.png)

They confirm the intuition that lower pressure is better

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/E915DB58-3A4B-4678-B992-54B6C8BE61A5_2/1HyWvvdTTjxhRuKdZxe0b2ZVpMlqrBMaOidgcOo0bKoz/Image.png)

They seem to confirm the previous intuition that sputtering above 200 W is kinda pointless

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/A689D46C-2FE6-405F-825F-CE26030C9538_2/ZxxnO47iUPeVwaaIdLsAcpJdpGNywfRHLXB5ro2gwhkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/7931E304-D658-420A-9BF6-DCC3EE26BD37/2399ED41-4160-4AAD-845A-B63B7E27C7BF_2/hstuLDgQq6HVt7WkMO2C8yLZMILd7CALiyScjrdl7Boz/Image.png)

Unlike a few other papers, they seem to say going higher in tempurature is better.  The index of refraction discussion is similar to what we expect, with increasing n for most temps until you get high enough that you oxidize away most Al-Al bonds.  They also say lower pressure and lower flow help with loss because they eliminate clusters and voids.  They also don’t mention substrate bias power, so I don’t know if I fully understand that yet

An idea for a final deposition process is below:

RF reactive sputtering

Ar flow: 30 sccms

Pressure: 4 mTorr

Power: 200 W

Tempurature: 700 C

O2 Flow: 2-4 sccms

