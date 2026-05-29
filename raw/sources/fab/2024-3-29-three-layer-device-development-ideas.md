---
type: craft-export
title: "2024-3-29 three layer device development ideas"
craft_document_id: 6E04AFA9-70CE-4C2B-B4C8-511C9185FA1A
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-3-29 three layer device development ideas
The purpose of this document is for me to detail my thoughts for the best way to procede with a three layer DC device.  While we should probably take a closer look at the possible photoconductivity of my doped oxynitride films, for now, we have not noticed any.  So we can assume these films have constant conductivity.  As a reminder, below is what we have produced so far. 

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-001.png)

I think the B4 point is probably an outlier.  It also seems that the films basically behave linearly for higher E_Field.  This effect could really bit us in the but if the field goes down substantially.  Given this, I may want the bright and dark state to be more closely match to make sure I don’t slip into the highly resistive regions.  I can ask about how this will work as the conductivity of the films will change as the fields inside change.  I want to know if the linear project saw this effect, though my field contrasts are much higher than their’s.

My most recent films (B7 or B8) are close to the type of films I would like to use (B8 specifically).  My guess is that they are between 1e-9 and 1e-8 for conductivity.  Given my RC constant calculations, I would really prefer to operate a device around here. I can work at a higher conductivity, but my worry is the optical quality won’t be great (as we could clearly see the difference between a films deposited as 5W and 10W).  

From here on out, I am just going to be digesting Ryo’s previous logs for his SRN depositions.  The hope is use the core as the photoconductive layer.

In this document: [https://tdwg.craft.me/87RJ6djM5AYWuk](https://tdwg.craft.me/87RJ6djM5AYWuk), Ryo first experimented with SRN back in December.  Below is his result with Low stress recipe (a = 5). (a = 4) looks very similar.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-002.png)

Ryo got a rather low index of 2.07.  This is very closer to stoichiometry SRN.  His dep rate was around 40 nm/min, which is totally doable.

In this document: [https://tdwg.craft.me/H0gn16fBwtDkBN](https://tdwg.craft.me/H0gn16fBwtDkBN) of the same samples, Ryo found that the samples above had a resistivity of 2e-10

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-003.png)

These are quite resistive.  Martin’s previous SRN characterizations for a=4 are below

![image (1).png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-004.png)

Martin shows much more conductive SRN than Ryo did.  If anything, I massively prefer Ryo’s films right now.
In this notebook: [https://tdwg.craft.me/Zx8NYF4l6Y8SPB](https://tdwg.craft.me/Zx8NYF4l6Y8SPB) Ryo took some ellipsometer data in October of alpha = 10 and alpha = 8.  He got n = 2.6 at 600 nm and n = 2.36 at 600 nm for alpha = 8. Below is Ryo's hit for a = 8

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-005.png)

We would likely see an index of around 2.2, which is totally fine.  We just really want to stay above 2 if possible to have usable confinement.

In this note: [https://tdwg.craft.me/HgQcysOe5CsYco](https://tdwg.craft.me/HgQcysOe5CsYco), Ryo just seems to be depositing a = 10 and a = 8 films.  The most interesting bit here is that Ryo observed quite a bit of non-uniformity.  Below is a = 10.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-006.png)

Below is a = 8

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-007.png)

For a = 10, using the filmetrics, Ryo observed thickness of 211nm, 371nm, and 397nm across different parts of the chip.  So almost 200 nm of variation.  This is troublesome as we go thicker.

In this note: [https://tdwg.craft.me/jxiBPkT8kyOsJD](https://tdwg.craft.me/jxiBPkT8kyOsJD) (back from September, so take it with a grain of salt), Ryo took conductivity data for alpha 10 and alpha 4.  Below are the results: 

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-008.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-009.png)

Ryo noted that there was ~17.5x increase between bright and dark state for alpha = 10 and only a factor of 3 for alpha = 4.  If I can get this alpha = 10 back, then I really want to use it, as it gives me some room to manuever and have the correct conductivity for me.

 In this note: [https://tdwg.craft.me/mFCoaU4rpmuNp7](https://tdwg.craft.me/mFCoaU4rpmuNp7) (taken in the middle of December) Ryo measured the properties of high frequency recipes.  Below are some of the results: 

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-010.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-011.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-012.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-013.png)

Ryo does not note the uniformities, but it does seem that his high frequency recipes are a bit more uniform.  Otherwise, A = 5 for low stress is a great recipe.  It is interesting that we must use blue light to make this all work, as the birght state conductivity is a bit pathetic when we use green light.

Below is what Ryo achieved for his high frequency recipes.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-014.png)

In this notebook: [https://tdwg.craft.me/k9ZtHOrijjZHlI](https://tdwg.craft.me/k9ZtHOrijjZHlI) Ryo seems to have scanned through his recipes again.  Below is a picture of uniformities:

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-015.png)

After repeating low stress for a = 5, Ryo got a very low dep rate of 16 nm/min and consistent index with above at 633 of 2.1.  He does not make too many more comments about his film other than to say that the thickness varied between 100 nm and 147 nm.  The small dep rate is really what worried me.

In this notebook: [https://tdwg.craft.me/jgYDeACYplpPal](https://tdwg.craft.me/jgYDeACYplpPal), Ryo tried to deposit low stress nitride after the NH3 chamber is replaced.  Below are some of the film uniformities.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-016.png)

Using Filmetrics, Ryo guessed dep rate of about 50 nm/min, which is quite good (though take this with a grain of salt ashe used filmetrics)

Below is low stress a = 3.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-017.png)

Lastly, below is high freq a = 5

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-018.png)

From this, it would seem that, while the film is not quite uniform enough for a waveguide, we could rather quickly get enough film to use on the CMP.

In this notebook: [https://tdwg.craft.me/NPAKjhT9xaiEm3](https://tdwg.craft.me/NPAKjhT9xaiEm3) Ryo took conductivity data.  Below are his results

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-019.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-020.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-021.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-022.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-023.png)

I will say this much, the high frequency recipe is looking very appealing as it gives me a huge conductivity gap to work in.  It also seems to have very little dependance on the applied field. It is a bit weird that Ryo did not use 405 nm light like before.  It is also a bit weird that the dark state conductivity of a = 5 here is much higher.  Considering that these films came from the new canaster of NH3, I would generally trust these numbers to be accurate.  This data would seem to signal that higher Si content or high frequency recipes are best

In this notebook: [https://tdwg.craft.me/C4XSsXdz2FhgFK](https://tdwg.craft.me/C4XSsXdz2FhgFK), Ryo tried to deposit a lot of a = 4 high frequecny SiN.  He did (approximatley) two runs of half an hour and observed a dep rate of 17 nm/min on average.  The films are pretty uniform though

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-024.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-025.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-026.png)

Uniformity is not optically sound, but workable.  His dep rate is concerningly low.  He probably should have stopped and seasoned more often, but that introduces layers that may dramatically increase optical loss.  I am therefore less bullish on high frequency.

In this notebook: [https://tdwg.craft.me/kRUR9Kvu2dOjll](https://tdwg.craft.me/kRUR9Kvu2dOjll), Ryo did a photoconductivity calibration of the SRN films deposited in the previous part.  He simply found that 530 nm was the best wavelength to work at.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-027.png)

This notebook also details the low stress recipes after the NH3 canaster was replaced: [https://tdwg.craft.me/ugkdG7v9FG3OYB](https://tdwg.craft.me/ugkdG7v9FG3OYB).  The gist is the uniformities were, by and large, pretty good.  I might even believe, if we used a ful wafer, we would get very uniform films in the middle.  Nothing as good as my conductive oxides unfortunatnely.  Below is what Ryo records

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-028.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-029.png)

The index data is taken at 1um.  It seems from this we want to avoid the a = 4 recipe.  

In this document: [https://tdwg.craft.me/ONaRIHmH2JLv1t](https://tdwg.craft.me/ONaRIHmH2JLv1t) Ryo tried to do low stress nitride for very long depositions.  He basically seems to notice the dep rate saturate over time.  My guess is we want to work in 0.5 um thickness intervals.  His index was around 2.2 around 633 nm

In thie document: [https://tdwg.craft.me/LMrkdGoMqtXBAc](https://tdwg.craft.me/LMrkdGoMqtXBAc) Ryo did some more conductivity characterizations and tried to grow thick HF a = 4.  Ryo did not notice the dep rate saturate.  He also noted that the conductivity was a bit higher than last time. but it looks very similar to me.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-030.png)

In this notebook: [https://tdwg.craft.me/wxIhPkM8ENmZTu](https://tdwg.craft.me/wxIhPkM8ENmZTu), Ryo examines the effects of low frequency deposition.  He gets pretty good uniformity with the basic recipe, pictured below

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-031.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-032.png)

Ryo took a dep rate of ~30 nm/min for this recipe and got an index of 1.88 at 1500.  This is a bit low.  We would probably want to flow less NH3 to make this, but I am worried this will kill dep rate.

Uniformity suffered when Ryo flowed 50 50 of SiH4 and NH3, so I am worried the Si rich films will suffer a lot of uniformity issues.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-033.png)

In this document: [https://tdwg.craft.me/4UTQbH9EczM9YS](https://tdwg.craft.me/4UTQbH9EczM9YS), Ryo further expores low frequency depositions.  He was able to get amazing uniformities with the recipe below

![Screenshot 2024-04-01 at 11.32.14 AM.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-034.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-035.png)

Dep rate a bit under 30 nm/min.  At 1550, the index is still 1.97.  This is a bit low.  The unformity might be of optical quality.

For full films from this notebook: [https://tdwg.craft.me/72m5PotwdhO5ij](https://tdwg.craft.me/72m5PotwdhO5ij), Ryo saw fairly good full wafer uniformity:

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-036.png)

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-037.png)

Above is full film uniformity, which is not bad (but would probably require CMP

In these documents: [https://tdwg.craft.me/MhUIgwyoJ07a9M](https://tdwg.craft.me/MhUIgwyoJ07a9M), [https://tdwg.craft.me/bqhwNVEpz4RTfP](https://tdwg.craft.me/bqhwNVEpz4RTfP), [https://tdwg.craft.me/Y2Cmc3TmAdFrrp](https://tdwg.craft.me/Y2Cmc3TmAdFrrp), Ryo seems to have tested films with N2 gas flow dominating the nitrogen.  It seems even a bit of NH3 seems to screw up uniformity.  As a general statement it seems that you really have to balance your gases to get good uniformity.  

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-038.png)

Above shows some conductivity data for the films lacking NH3.  It is just too conductive.  When Ryo flowed less SiH4, he saw uniformity go down.  I should also emphasize that this data is really optimistic, as he was not able to observe this level of swing with other chips.  We also shold note that the 40 sccm SiH4 flow and 2000 N2 is very uniform.

![Image.png](../../assets/fab/2024-3-29-three-layer-device-development-ideas-039.png)

**Here are my take aways:**  It seems that 50 sccms SiH4 and 30 sccms NH3 for low freq will give amazing uniformity (everything will probably still require some CMP).  It also seems to have a steady dep rate, though Ryo did not try to grow thicker.  HF a = 5 seems to have the most useful conductivity data and a = 4 is not far off.  Low stres a = 8 also seems to be pretty usefu.  These films will be less uniform, but I can account for that with CMP.  They seem to saturate deposition around 1/2 um of dep.  The one main advantge of a = 8 is the higher index, so we would not need as thick.