---
type: craft-export
title: "2025-04-05 reactive sputtering of hfo2 literature review"
craft_document_id: 011E815F-795F-4344-89FA-8393D9932E81
craft_collections: [fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2025-04-05 reactive sputtering of hfo2 literature review
We now roughly understand (both from literature and from experiment) how to deposit low loss Al2O3 waveguides using RF Reactive sputtering.  Now I would like to get a sense of how HfO2 is sputtered, and possibly look into some cases of reactive co-sputtering so I can get an idea of how those processes work.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0040609012008863)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-001.png)

O2 = 2.5 sccms, pressue = 9 mTorr (once units are converted).  Ar flow = 22 sccms.  Temp = 300 C.  Power = 30 W

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-002.png)

It seems you can sputter this quite thick, though I imagine it starts to crystalize before these points.  The rest of the people did not really give me many characterizations that were valuable.  Below is the index data, but everything else was not really useful for us.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-003.png)

The above used DC reactive magnetron sputtering by the way

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0040609013011905)

These people use DC reactive magnetron sputtering.  Below is their process

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-004.png)

They use a bit of a higher pressure, a lot more O2, lower power, and lower tempurature.  They studied how hydrophobic the matieral is, which is not exactly relevant to us, but they did take a few pieces of data that are more relevant than you think.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-005.png)

Evidently lower pressure is better for us, which we kinda knew before.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-006.png)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-007.png)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-008.png)

To be honest, their optical data was not great.  They do not specify the wavelength they got their index at.  At the very minimum, it is clear that crystals decrease index nad increase roughness (which we don’t want).

[Homologous substrate-temperature dependence of structure and properties of TiO2, ZrO2, and HfO2 thin films deposited by reactive sputtering](https://pubs.aip.org/avs/jva/article/37/5/051508/245962)

Below is the high level description of what they sputtered

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-009.png)

Deposition parameters

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-010.png)

As a summary, they used 25 sccms of Ar, 5 sccms of O2, and a pressure of 3 mTorr.  Nothing about power is noted

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-011.png)

Deposition rate is a bit low, but I would suspect this is a function of the lowish power.  They deposited 400 nm, so arcing can’t be a huge worry if they got that much film without any issues.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-012.png)

While the idea of the composite material is that we don’t see these crystals form.  Still is interesting that higher tempurature causes more crystals to form.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0169433206005782)

While this paper seems niche, it seems to suggest there is a way to prevent larger crystals from forming in our films, which would be very useful.  

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-013.png)

They also use DC reactive magnetron sputtering, which is nice.  This makes me believe that we will use Al in RF and Hf in DC.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-014.png)

I am not sure how to convert this power density number into something useful.  Either way, this is at least a confirmation that they use a similar procedure to us.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-015.png)

Apparently we could have some uneven roughness across the wafer due to charge ion bombardment.  Later in the paper they say this is oxygen ion bombardment

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-016.png)

It seems that pressure has a marginal effect.  It some seems to reduce one type of crystal growth as you use a lower pressure.  The main point is I don’t see a reason to be concerned about still using 3 mTorr.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-017.png)

Higher tempurature casues more crystalization.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-018.png)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-019.png)

Two interesting observations.  One is that they use some very high oxygen flows.  It also seems that higher oxygen flows can supress crystal formation.  This gives me some hope that we have a wide window to optimize the O2 flow in.

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0921510704006750?via%3Dihub)

This paper seems more relevent to us, even if it uses RF instead of DC sputtering

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-020.png)

2 Pa of pressure is 15 mTorr, which is kinda high.  200 W is reasonable, though the 110 sccms of total gas flow is a bit high.  They deposit at room tempurature (this was mentioned earlier in the paper).

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-021.png)

They take data over a wide range of O2/Ar flows (they define this ratio as R).  It seems that higher O2 flows lead to more crystal growth

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-022.png)

It seems their dielectric constant is rather stable for lower ratios, but gets oddly high for the end.  So clearly too much O2 flow can do something weird.  They mentioned earlier this can lead to larger grains and therefore more porous films.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-023.png)

Another confirmation that there does seem to be a middle point where you get the densest film, but we seem to have a wider operating window here.  They claimed that R = 0.2 was best

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0022309302009766)

They simply present another recipe for sputtering HfO2.  They do this for gate dielectrics.  An interesting thing to note is they sputter a very thin layer of Hf, which oxidizes, and then continue with HfO2 sputtering.  Below is their recipe

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-024.png)

The important points are room temp deposition, 4 mTorr, 100 W of power, 3.6 sccms of O2, and 18 sccms of Ar.  This is fairly close to our current Al2O3 recipe.   They do DC magnetron

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-025.png)

While deposition temp and annealing temp are not exactly apples to apples comparisons, it seems that one set of crystals forms at 650 and another 800.  I am not an expert on the different crystal phases of HfO2, but it seems that the one at 800 is the one that kills Oscar’s work.  It is interesting that this can stay amorphous after deposition.  These are gate oxides, so obviously they are quite thin

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0040609003012458)

These people seem to sputter dielectric HfO2 (not reative sputtering with a metallic target).  They use an RF source to prevent arcing.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-026.png)

It is a bit strange to me that they get such an insanely higher sputter rate.  I should also mention that they are going for 150 nm of film.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-027.png)

While this is not relevant, it is crazy how easily you can see the polycrstaline grain formation.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-028.png)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-029.png)

Again, something of a tangent, but it is cool how they use this bilayer model to fit the HfO2 film.  

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0040609015008950)

These people RF sputtered HfO2 targets, but also examined the effect of changing the O2 flow.  This is not exactly what we are stuyding here, but I figure we can add it to the list.  Below is their deposition proceedure.  

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-030.png)

Temp = 100 C, power = 200 W, Ar flow = 20 sccms, O2 flow = 0-6 sccms, pressure = 3 mTorr.  Below are the results

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-031.png)

Obviously, they make their films pretty thick.  An interesting observation is that they can reduce the grain size my flowing more oxygen.  So they get a film that is effectively oxygen rich.  They also go pretty thick too.  So I guess even sputtering dielectric still has a chemical reaction.  They seem to believe the lower refractive index from more oxygen flow comes from filling oxygen vacancies with more O2 flow.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-032.png)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-033.png)

Above are the ellipsometry fits.  Seems like the higher the index, the lower the loss.  This probably is because the extra O2 helps densify the film.  This is a neat trick to reduce loss as well (though this still has crystals, so we can’t use it outright).

[Iop](https://iopscience.iop.org/article/10.1088/1742-6596/1859/1/012066/pdf)

These people did normal DC magnetron sputtering of Hf targets to produce HfO2.  Something to note is they don’t scan power exactly, but instead they scan the applied bias voltage.  This means the same thing, but the conversion is not exactly one to one.  

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-034.png)

While they don’t mention deposition pressure or raw gas flow, it seems they have an O2/Ar ratio of 0.2.  They use a tempurature of 300 C

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-035.png)

They also deposited fairly thick films.  They gives me some confidence that arcing should not eb a huge issue.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-036.png)

They note that their films are fairly poly-crystaline.  This is fine (as this is why we co-sputter), but it is good to note

[ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0257897206009108)

They do RF reactive magnetron sputtering of pure Hf target. 

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-037.png)

They use 5 mTorr pressure, 260 W of power, and seems that (as they say later), they keep tempurature below 52 C by attaching wafer to heat sink.  They see a deposition rate of 0.2 A/s, which is somewhat in line with what we see with Al2O3.  They don’t mention the gas ratio, which is what we really want

[ScienceDirect](https://pdf.sciencedirectassets.com/271582/1-s2.0-S0042207X06X04566/1-s2.0-S0042207X06000972/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEOT%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQCVKuSdU%2FDka0PA5X9h%2Fa4yl2Yg5%2B%2BupbhRTw1OQ2NOdgIhAPGa%2Bwam%2FXQo9AeqQx56qVFHfsPIVu6QeI2LP7oudOGbKrMFCF0QBRoMMDU5MDAzNTQ2ODY1Igzx99ot%2Fvhxnh%2B%2BYREqkAUA0aEXZPfrR4rHFCv13C%2F7MoxHVxgoBnSFjuE3L5KPExpRQDVLO5x34w4NkChrOoye9NC%2FxKHBLCfB9GVuL3%2BJxP14peVoDMJ6yAH2aYLKBD2hNvP2727D%2BX7txzsO3Z6ubBlNRbXYlnf81l3wdAYNpsL8e%2FJVNqlW3ncqM75I5qZmcb1LULt87aukSlcDrUx6TjEi1%2Fn9Vo8x8P%2FuKsAPfPrAxYi25TiFOkNi34ue%2B3tSntvoQSy1XlNduXVahHWglmQC%2BRAppPmXjIpHoqIvf5u1161jZqulbDp4vRarYV%2B%2F7EZU5G%2F2uSB7ott5Edm8xOI60lffgxCefetVyYK0QTOxvobemuEQqXSEr0%2Fl6N7Q%2BjyfmYnmje5p3zjPNUDC%2FOaIx%2BSsTaTj40WPjo10rlN053QCt2TcIbCB2zkGQKJoEQwBHU6i%2BvFL%2BTLB%2BEGsCNJKxtrYd5kI2quQ30VL5XdhS%2BZrV94AZc2NkBK4H95JwcEPh71p7umhogiTQrvaFi8%2BtmZdL47SavZbCotm4jK6kOzm0dr1LfriVZ1pRvVxb3NxtJW6AB729CLkiJ%2FrhYQKJagzyFoq%2B3mH%2BPB9Q03v8gDLwd53LHEexD8oFCX0P0Jt6ZoXUNwLNMiGy81PG5k7ujxlgiaBjYXijcOVia1944ukSjyHhIk6H2hoYP6Zssp5Z6iC6lWTLwKAAugkRUjwJpKWUkTO3j9p4jv6zEkVfWtbFA9giLeD1kIzpPCyRdzE7u6P6rSZ9zkTLoZC7OaQTGxGIV5S%2Bev37xxo2bxAe6Enxk76du%2F8aU5VOoCmXW5Ns2Ldk7V%2Fmh5NrhRMGXAwVTCrvlWtAQz4bCKT8fNR2RpwOl7pDyiXCcMHizDI%2B86%2FBjqwAUe3co7iA4pOAiZmnsvhk6DYJHvAuc88DPxhIlK36YrkXQvSJf7DiVq9ZYGVLQ%2F2xC2nZ1%2BHnqzNB0aIlXXlQAWmGT5WXinlUYsLMqAtgEMQImj1nAem8CEGY6Q4PYIOHLShufdm710PnaXr0qe7fvlHUeu03Cjc3L3jqcJXLBc60g6WBVbmgz0Ge1871y90CWWcjMOnHV3%2FeFuSsKOzlQM6LDGsu384PwlB4szdEm2d&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20250407T123903Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYW6Q5EDOK%2F20250407%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=7ff43d1b8ba1621df9e04a50ae33a412446ab783381f668274c9917241fd036e&hash=37991c3ca31d248f58c61c8b120eef77e023a358975b72ded7a33cfb0503c34a&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0042207X06000972&tid=spdf-b37909f4-8e69-4d1a-8a2b-e8ee95565d8d&sid=c17b93822b17764c859aa00767a5f00c37c4gxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=0f1556500358595a065858&rr=92c995e77a6d939a&cc=us)

These people are a bit closer to what we want.  They vary the O2/Ar ratio for DC magnetron sputtered HfO2 films.  

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-038.png)

They deposit at 1.5 mTorr (Which is kinda low).  Other constant parameters are not described.  Their deposition rate is somewhat close to what we would expect.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-039.png)

They seem to stick close to ~ 30 sccms of total gas flow, which is what we already do.  They use a huge variety of flow ratios, but it seems that we can do lots. 

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-040.png)

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-041.png)

While I am no expert at reading these transmittence curves in the context of waveguides, it seems that we want higher O2 flows.  1:9 corresponds to a ratio of 0.11, and our currently ratio for Al2O3 is 0.14.  They seem to suggest that 0.33 is better.  It seems like the loss method here is oxygen vacency.  This means an oxygen is missing, and your get more metalic behaviour.  

[ScienceDirect](https://pdf.sciencedirectassets.com/271590/1-s2.0-S0272884215X00058/1-s2.0-S0272884214020628/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEP3%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJGMEQCIEClTHjlGKxU7%2B6HUOjhiAzMFeM0BBSLT15HbqHoGhGtAiBDz2gsLTHtorg047H7kOkjEclO8YwKRJ1DmE8OuL3p2yqzBQh2EAUaDDA1OTAwMzU0Njg2NSIM%2FjmzAV%2F8KDhCZ7WMKpAFAaPX6TQGNk%2FOcsK%2BuD0e%2Bq1BX18YP%2BMYbERhX791LpONQ2FtvjHO2MBJeXYqf7UTUoc5HGoxj0%2FrUSlJQnXm711Eqr2yllmEhpXqTvWhDvGbFBglZU5NySm3CDb%2B%2FDzGjTNuttynR9OCNuJkxunOQbNJq2ORbiH45kMYG3gr2xPiN4YVidFKPLX%2FpW7Svb2H2bsb6Ete2whw66VY8hRIa7jB8mtALLu7l2msV8xcHBb%2BMDJmQ686K3UjO2Pk0QMUEWA1umY7k%2F4C1X6Dzawf99Jt97vbtCS0BNkFtU9tQrTg4GvbUp7uvRwINgI4eu5oE0zYa8XFjnuXxT0FgUI423gSOaECPYIt47Jmkl2c1jUwo4lF%2B9GGe3TYsanSbmf3QcY%2FCcwefreBpeo5GEZjD7%2FBV8p5FaFdOcLUmLK2GGn1m4NMo7d5N1fHpfm9YnnJCxeo5ZsoZwSkq4ut30%2BLtpqjmqy%2FxWVA06SjuihU7XQ1AGc3CH%2Bg5%2F%2Fvnw2MHMCXuQLpkQbDViE1epjDEQKQQMGcU4fQiKSvHaOjjz79kvxjPsw%2Fh61OWmzehhAgSC1NUD99JAzDYue4PHDz6%2Fx%2FhC4gLlkIa9NZyRwLXvq9tHHF8npqn6vHenmw6tVEuMUDfXB1sRbKLKPaFt9%2FbvYNmaeRtQgYvAUZSfbNBH%2F4mG86T86wJt90WAarO%2FBhWem0EdFZfnPfu%2Bt346dtYADkq0Ex0Qg37Hgg9ZIInFKNirNaup8Ekxx1eA9m1sOffSTTk3FYqckn7foZ5pDvPuz9u1Ku4Jy6tWgFUnfFU1d0xfa8I33xQFNd5AF4dig%2F7NQGBTjRr0WytB0pGQaJIdHjHzlZjPU0LxKgQ1gVyxRlbGkw3LLUvwY6sgFSM%2FXiBZPOtfxbBAZl0pZ5SiZmCT6fZHPFAK9PUFCtV1Dycpdo1%2F6PlRj9R%2FLes2wB2zOINeVfuq3fuPt0tJ3A4o8RaAVIggzB8ohEqYGHJHCSjgMYVjRf6oICh67VaxnEwahgpmCPREJFsaudYUlh7tJNV%2BSSbSTgNl9BudEI7z94gJDt6mFS8wow8z5LuysF%2Br%2FPjlhmuu%2Bzv0m0ywL5%2BH8dIJF4SAW9r%2Boq%2FTUqX%2FdR&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20250408T130946Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYS3A6C7E6%2F20250408%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=7dbee9d76ea25b8cd2350bf38e9bc8c30562d3e0e0e28719453316c1dc9713e5&hash=d286d280c723e0c33a461dcd2cd40f13ff83c9895a7c2eb85b7b4bde0b7c6854&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0272884214020628&tid=spdf-766f15e7-28b4-4518-92e4-97557e327da3&sid=c17b93822b17764c859aa00767a5f00c37c4gxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=0f1556500453505f575c56&rr=92d200439e1b5e60&cc=us)

They use RF reactive sputtering. 

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-042.png)

They presputter and make sure to pump down to a low pressure (we do the latter).  They use a deposition tempurature of 300 C and a power of 100 W.  

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-043.png)

From this plot, it seems as though there is a bit of a Vbias curve.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-044.png)

While this is less interesting, it would seem that having more O2 is still better.  I would also not look down on the dep rate above.  While it decreases, it does not go to zero like the Al2O3 case.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-045.png)

This shows effectively that too low of an O2 flow gives you something matallic, while increasing the O2 flow a lot does not change the metallic vs dielectric nature.

[ScienceDirect](https://pdf.sciencedirectassets.com/271621/1-s2.0-S0257897210X00196/1-s2.0-S0257897210007735/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEP7%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEaCXVzLWVhc3QtMSJIMEYCIQDNdSqTmSzpRFJjqfjt2NhuQwPXCIFC5LxJxADY2FFd6wIhAI%2BeuwVsT6vJO0VrR8uMZRLec5e1sIETqxSuyLeX3x6EKrMFCHcQBRoMMDU5MDAzNTQ2ODY1IgxlTMtVUi4qX2n%2BPLwqkAWAt3NB76PH1xridDYBeRQ3xMeGMQ54UwOYzDMa8pylhYyx3ofqMafWE9pNEaHO0sOHnyA8Tuuh2row3Wc9iubPVHdS5ZKrjlzWKwJnFW6pq6JkzMDmevSCeim8NTYPL%2BWxZlGBjgB7tbIwaENurw5xav6EX5yUcasRO%2BVGCegwtlDeo7cb1%2Bk6fhXZal3WqPliY%2Ft75UBMPoZfvaRNRmCa8k3lU2xfGz%2BvOSfDROI4rEPa7pzyG5SPTtfTttnvrh2%2BcfqnWjMj1XLy3yq08HwWZtrMWvudfRDbIvf%2BGJqfq8BdBg4kzgSCJwmmV%2BGWKNHWRxehM6IHgXmpmqFd28EC0gLijK6JSbJPjPl4zuFbbwlOr2y4MJt74kNit6B89k7edX1c8%2FomMn94L7QTtpG%2FdIzDoWc%2F8DOs8CPWOx9jmRN9TVxdUQj7uFv5JLDjEGpCb8BVoS986llI172Pe50ICsm1EVQEI7JuCsN5RcchuxXs5rhVQ%2BiZdaOa9bvbY5F9ceyvMVsB577E4g84ofiBP3LUKpk0wzrnRt69ahhkI6BvP8%2FO77JgyOQviRMs9M28GkVWOHNSx9GXCWjSpu6BEF4VQqTywMa1Xg6ounYJfiUdzbzMxMMYfgOMrstjpQG%2BTRj48YArYjxlR48BbJ1Ijuc6cLH80cGEFgCRu7XTrwnB3QiDHJUqh2%2FrELr5sJQDcMyRspyrzBxEFW2OIlpLqB2Tq6SOuikCZv52No5KfVPKFxtCA8NyAR1VYwyLlKn9sXR0v10Q6p7uWXePaOQCiRFP8Su31g4u%2Boav%2FfhSYi0GNr7ILGt0hva1So9IE6xyYfE2ELrFYHxKk1Thrsm11P8SGE6r%2BnmmY%2F%2F7IgS8QTCLy9S%2FBjqwAUbKoDuj8S7bSrbaQJZZj2CzKxBqu2U6cB2pPz5XHov0RJRt9T0dur%2FUd6spDSqC0DClBOUmJF1yKFK1g%2F00CQ%2BqH%2FHgibHgSmObbGYR7FRoVOdQcdm4GqfaRLXR7D3kfeG0KeSJuEGM6hUGxo3oGIw5xZ75RcXqxe1ZwRIffxKTaDV0DDs1KPOdGKe%2B2Hs0txyKv8JId%2Bcpx3pRY4uFrNwAqnWRJ3IjHEfntwNnCfV4&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20250408T134711Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYUVKBTJ5P%2F20250408%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=30edc0619a17a8347a2e7c2867ed27c84e5c52fbde58c8e32f7521875d4595b3&hash=a4fa4cf91444cb35d1917daf7374f2d5c2f599458820f4f9e29fe8a8f342ad2f&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0257897210007735&tid=spdf-bf014a10-ce1a-489d-ae98-53cfe373ff1a&sid=c17b93822b17764c859aa00767a5f00c37c4gxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=0f15565004535358525a0c&rr=92d23715cd01c540&cc=us)

They use RF reactive sputtering as well

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-046.png)

Power = 110 W, pressure is 1.5 mTorr.  Ar flow = 12 ccms, with O2 flow between 0 and 6 sccms.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-047.png)

They observe the same kind of Vbias behavior here as well

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-048.png)

Their explaination is that, with less Ar atoms as a percentage of the plasma, the engery of the atoms sputtering the target is lower, so less deposition.  I wonder how this is reconciled with the Al2O3 results.

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-049.png)

This is mildly contradictor to the previous paper, where HfO2 had a higher index than Hf.  Either way, this at least confirms we should see some change

![Image.png](../../assets/fab/2025-04-05-reactive-sputtering-of-hfo2-literature-review-050.png)

They claim this higher index is becayse of moisture absorption, which maybe the other paper did not see?

Below are some general high level conclusions

1. It seems people do both DC and RF reactive sputtering of Hf.  There was no mention of arcing in any of the DC papers (which suprised me a bit).  Given this, it seems that DC sputtering will be safe.  Decently thick films were sputtered with DC, so arcing was not a problem after a while sputtering.
2. I really got very little sense how to get the ideal O2 flow.  It generally seems that people used a wide variety of O2 flows to get different crystal grain sizes and control deposition rate.  An O2/Ar ratio of 0.2 seemed to come up somewhat frequently, so I would default to expect that.  Much to my suprise, these was no hysteresis effect mentioned
3. Power and pressure were all over the place, but it seems that 3 mTorr is not unreasonable and we probably want to use on the order of 30-100 W as the power for DC.  RF usually has higher power.
4. It seems that HfO2 crystalizes rather fast.  Just something to note, and Oscar has already warned me of this.
5. It seems that using a higher deposition tempurature is fine.  People were a bit all-over-the-place on this.  One paper went from 100-800 C for DC sputtering.  another stuck at 300 C.  I don’t think using higher tempurature should be an issue