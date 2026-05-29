---
type: craft-export
title: "2024-6-6 mark optics call and polishing research"
craft_document_id: 8D190332-AD29-42E4-8E41-4C97B5FBCD33
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-6-6 mark optics call and polishing research
The purpose of this document is to write down any of my thoughts from the Mark Optics call.  The general objective (based on previous simulations) is to get about 2um of lithium niobate thin film onto a doped-oxynitride subtrate.  Ion-slicing presents the issue that we need to anneal, so our film properties might change.  The other idea we had was for a company to bond a full lithium niobate wafer to our substrate and then polish it down to be 2um thick.  Likely the starting thickness of the lithium niobate wafer would be 500 um, but it is entirely possible that it could be different based on the vendor.  Again, the main advantge of this process is that we don’t have to do ANY annealing.  It is a bit unclear how strong the bond between the subtrate and bonded lithium niobate wafer will be, but that is an issue for another day.

Jelena’s group at Stanford seems to have figured out a way of starting with Bulk crystal, bond it to the substrate, and then thin the bulk crystal here: [https://www.nature.com/articles/s41566-019-0556-6#Sec6](https://www.nature.com/articles/s41566-019-0556-6#Sec6)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8D190332-AD29-42E4-8E41-4C97B5FBCD33/7812E949-C7B6-4B91-ADA3-C3741D78F681_2/V5gpmyFe3ezGVobVwufqx7yu3ZKNEs9HJ65UkLXhecoz/Image.png)

Obviously they are not going to give me all the sauce, but it seems that they grind the bonded wafer down quite a bit and then use CMP/Dry etching after that.  They grind the wafer to 15 um, and CMP to an unspecified thickness.  Their final thickness is 350 nm.  It would not suprise me if they cMP it to 1-2 um and etch from there, mainly because CMP lacks precision and etching is precise.  They also use very thin final films.  They talk a lot about the bond strength.  This makes me minorly worried about how strong our bond is.  I should bring this up today with the polishing people.  Remember, grinding != cmp.  We should clarify which the people at Mark optics will use.

These people did wafer thinning on Lithium niobate: [https://iopscience.iop.org/article/10.1143/JJAP.45.3822/pdf](https://iopscience.iop.org/article/10.1143/JJAP.45.3822/pdf).

They did their process at room temp (which basically seems to just require that the substate and lithium niobate are clean when they are brought into contact.  This seems to imply that a good bond can be achieved by someone who knows what they are doing without adding an adhesion layer or heat.  That being said, based on our previous research, it seems that an adhesion layer does increase the bond strength.  These people have a lot of documentation on the exact parameters to get a good bond (not totally relevant to us).  The more important part is that they document the best ways to polish their wafer.  It seems that they polish their 500 um LN wafer down to 2um in three steps.  The first two are long steps that are meant to remove a lot of material fast.  The troubling part with these steps is that they seem to get a lot of cracking.  They then polish slowy at the end ot get rid of the cracking layers without introducing any new cracks.  They seem to be successful with this procedure.

These people ([https://ieeexplore.ieee.org/document/9593341](https://ieeexplore.ieee.org/document/9593341)) thin LN down to very thin films (160 nm).  It seems that, at some level, CMP stops working for us.  I am just not sure at what thickness we stop getting good thinning results with CMP.  Anyway, they basically use ion milling.  This is just very slow, as they don't want sputtered ions to cause film cracks, so their etch rate is 7.5 nm/min.  Not exactly fast.  We also don't have a recipe available from the CNF to etch LN, so this is not a good path

These people: [https://www.sciencedirect.com/science/article/pii/S0169433217302829?casa_token=BcQkF5nbnCMAAAAA:XoaygyqMt4slt9CVQG_tc0Dtd__fbsIMUYIFyjBmb19U6gYmwrCzu5GeXNb11-w_mu9yUHNabtI](https://www.sciencedirect.com/science/article/pii/S0169433217302829?casa_token=BcQkF5nbnCMAAAAA:XoaygyqMt4slt9CVQG_tc0Dtd__fbsIMUYIFyjBmb19U6gYmwrCzu5GeXNb11-w_mu9yUHNabtI) give a good summary of the field for thin Si substrates.  I think the idea of thinning with CMP alone might be tricky.  They mention that around 5um it stops being useful.  This seems to not only be because of roughness concerns, but also surface variation.  They investigate etching, but that is obviously not a concern for us.

This paper gives a brief description of how ion milling works: [https://www.sciencedirect.com/science/article/pii/S0925346704003787?casa_token=pD87BldA24kAAAAA:ska6Z1xO443RnAA-_TWPjUAuDR7H9EmEcLG-q_SWKe9hbuaZnPRe_BBGwCU-Tk4DctrZ6f7PTic](https://www.sciencedirect.com/science/article/pii/S0925346704003787?casa_token=pD87BldA24kAAAAA:ska6Z1xO443RnAA-_TWPjUAuDR7H9EmEcLG-q_SWKe9hbuaZnPRe_BBGwCU-Tk4DctrZ6f7PTic).  It seem to be quite similar to electron lithography.  I wonder how Martin and Hiro thin down their wafers with nanoLN, as this does not seem to be scalable to an entire wafer surface.

In case the idea of thinning is appealing, here are a few more companies that can do thinning:

1. These people seem to offer general thinning services, but not LN specific.  Note clear how thin they go: [https://www.syagrussystems.com/wafer-backgrinding?campaign=1654276521&content=667031360525&keyword=wafer%20thinning%20services&gad_source=1&gclid=CjwKCAjwvIWzBhAlEiwAHHWgvW7vSz-BXiq23v3dxy9KQ_y6DsZP2itoCeNv66tlBIuuMRG3mUn1RBoCyzUQAvD_BwE](https://www.syagrussystems.com/wafer-backgrinding?campaign=1654276521&content=667031360525&keyword=wafer%20thinning%20services&gad_source=1&gclid=CjwKCAjwvIWzBhAlEiwAHHWgvW7vSz-BXiq23v3dxy9KQ_y6DsZP2itoCeNv66tlBIuuMRG3mUn1RBoCyzUQAvD_BwE)
2. Not sure if they do LN (or the thickness they do).  Something to note is that it is unclear if these websites are refering to thinning a sole substrate or a layer ontop of a thicker substrate. [https://semiconductor.alfachemic.com/services/wafer-thinning.html](https://semiconductor.alfachemic.com/services/wafer-thinning.html)

This is a start, but I must admit, there was not a huge variety after first look.  Will look more later if this is a possible path.

Below are the questions I would like to ask the Mark Optics people:

1. How thin can we get?
2. Will we have issues with cracking if we go around 2um thick?
3. What type of roughness should be expect?  Do you think if we used the CMP in our academic cleanroom we could beat that?
4. Will there be thickness variation across the wafer?  Is so, what should we expect?
5. Would it be easier if we use a smaller or larger substrate?
6. What type of bond strength should we give you? We will need to pass this information onto whomever does our bonding.
7. Does it matter for you how thick the LN wafer we bond onto the wafer is?
8. Are there any treatment steps you use besides CMP and grinding?
9. Logistics of getting the wafer out there.  Should Partow (or another vendor) send the wafer straight to you, or should it come back to ithaca and we send to you?
10. Price and lead time



After talking with Julie, we got the following out of her:  They have only polished down to 10-12 um thinnest.  We probably can reliably get 20 um on first go with them.  So this is progress, in the sense that 20<500.  But 2<20.  They expect us to have a micron or two of thickness variation across the wafer.  They also mentioned that we could have parts of the wafer could flake off from bad bonding or other issues.  They did seem confident that we could get several 1cm squared regions to work.  The lead time is a month and I guess that the cost with be a few thousand dollars.  We are also being charged on a best effort basis.  

I must admit, I am not as optimistic about this process after talking with Julie.  If we copy Jelena’s process, we should etch down the remaining thickness.  This would require ion-milling, which the CNF can do ([https://www.cnfusers.cornell.edu/node/114](https://www.cnfusers.cornell.edu/node/114)).  It seems that Qiang Li from U of R uses the CNF for LN etching 

[s41467-020-17950-7.pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8D190332-AD29-42E4-8E41-4C97B5FBCD33/6A41346A-C919-4781-B17C-28DA129EA425_2/3K8lw4VyLkds9BkvxXcAeCLMKvuRR8lRRBzKNP08PZQz/s41467-020-17950-7.pdf)

They only etch 300 nm down though

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8D190332-AD29-42E4-8E41-4C97B5FBCD33/3EB72EA4-75AD-4A4B-B8D2-961403A4AD1B_2/v5WchehTk91I0gU0VQ8yzll4yCOORZcI6EFGofwr8D0z/Image.png)

They etch down along the X-cut axis.  I doubt Z-cut should be different, as this is a physical, not chemical) etch.  I wish we knew of a faster way of etching.  I will each out to Aaron about this.