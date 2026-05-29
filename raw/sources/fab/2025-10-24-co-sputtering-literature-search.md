---
type: craft-export
title: "2025-10-24 co-sputtering literature search"
craft_document_id: ED0092EF-866D-4E80-AB02-4675F5C14610
craft_collections: [fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-10-24 co-sputtering literature search
While we have a short-term plan to test slightly higher O2 flows for cosputtering, I am not the most optimistic this will work.  In that vain, it would be nice to find a couple more sources showing some longer term things we could try if this short term plan does not work.

[Shibboleth Authentication Request](https://pubs-aip-org.proxy.library.cornell.edu/aip/apl/article/101/8/082905/111975/Co-sputtering-yttrium-into-hafnium-oxide-thin)

These people co-sputtered Y2O3 and HfO2 to get ferroelectrics 

![Image.png](../../assets/fab/2025-10-24-co-sputtering-literature-search-001.png)

First major difference is they use dielectric targets instead of metallic targest.  Fwiw, even though I know most people use metallic Al to get low-loss Al2O3 films (because they want lower densities), there is a fair take that this metallic approach is actually quite off for co-sputtering.  At least they are consistent with varying power to increase or decrease incorperation.  Given our current deposition rates, however, I would truly expect that we are getting quite a bit of Hf.

We had decent reasons before to assume that 180 W of Hf power was giving an equal amount of Al2O3 and HfO2 (given that they had the same O2 poisoning point and similar room-temp deposition rates).  But given the recent dep rate findings (high power co-sputtering gave 40 nm/min, and low power gave 20 nm/min, with baseline Al2O3 giving 10 nm/min), it could be possible that my origonal hypothesis was wrong.  Perhaps we should make Al DC to make sure it dominates (though this could cause other loss concerns).  Or it could just be the co-sputtered complex is just less dense or expands faster.  Who knows.

[Shibboleth Authentication Request](https://iopscience-iop-org.proxy.library.cornell.edu/article/10.1088/1361-6528/aa7624)

These people co-sputtered ZrO2 and HfO2 almost the same way we want to (though they were looking for ferroelectric films, so not quite the same).  They to use dielectric targets though.  This HZO is thing is something Ryo has connections to at U Tokyo.  This paper claims to be the first to look at ways (other than relative power adjustment) to get better films.

![Image.png](../../assets/fab/2025-10-24-co-sputtering-literature-search-002.png)

They mention the problems we kinda know about.  Their source on cluster formation was not helpful, but the vibe I get from chat GPT is that this is where metal atoms bond to each other before reaching the substrate (as the atoms ideally reach the substrate one at a time).

![Image.png](../../assets/fab/2025-10-24-co-sputtering-literature-search-003.png)

They also presputter.  I don’t think this is critical (and our wait time before might effectively be doing this), but it is still a trick we can play in the future.

![Image.png](../../assets/fab/2025-10-24-co-sputtering-literature-search-004.png)

Another annoying possiblity is people do seem to anneal to get new crystal phases of HfO2, so we may want to deposit at a lower tempurature.  Of course, this runs a bit counter to what the Dutch group did, but whatever

![Image.png](../../assets/fab/2025-10-24-co-sputtering-literature-search-005.png)

Above shows what happens when you co-sputter HfO2 and ZrO2 with different oxygen ambient partial pressures to Argon.  While this does give a denser film (which we like), it seems the main downside is we still have crystals.  This is not perfectly analagous to Al + Hf, but this still has me concerned that people are not getting amorhpus films with Hf.  And given that there HZO films are like 10 nm thick, I wonder how easy it is to simply go thinner.  

[Reactive co-sputter deposition of Ta-doped tungsten oxide thin films for water splitting application](https://www.nature.com/articles/s41598-025-92008-6?utm_source=chatgpt.com)

The elitist in me wants to say this article might be a bit BS, as it is from Scientitifc Reports and the english is at best a bit choppy.  Nonetheless, the actually science seems solid.  They are trying to n-type dope WO3 using Ta

![Image.png](../../assets/fab/2025-10-24-co-sputtering-literature-search-006.png)

Shockingly similar to what we are doing overall.  One really important difference is the dopant is set to RF power, not DC.  So it is possible, in the future, that using Hf as RF and Al as DC is the play.  This is not what others do, mostly because of Arcing concerns.  That being said, I have not observed any arcing yet, so I am honestly not sure how substantial of a concern that is.

[NCBI - WWW Error Blocked Diagnostic](https://pubmed.ncbi.nlm.nih.gov/15306279/)

The above paper is just above metal cluster formations.  The general gist I get is this happens when you cool the plasma somewhat substantially.  They used liquid nitrogen to get the atoms into a lower energy state where they would start to condense.  So I think our atoms are generally energetic enough that I doubt this happens.  I also think there is the fair arguement that we should have seen this from Al sputtered by itself.  The best response is we simply have way too many atoms now.  We still have not found much on tempurature yet.