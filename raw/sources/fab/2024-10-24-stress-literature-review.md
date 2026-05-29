---
type: craft-export
title: "2024-10-24 stress literature review"
craft_document_id: 7CBF9868-1E89-477C-8151-0BD893EFE040
craft_collections: [fab-flow-literature]
source: Craft local PlainTextSearch cache
---

# 2024-10-24 stress literature review
Unfortunatnely, I have been faced a lot of stress related issues in the CNF.  This is very annoying.  While I generally feel like having a smaller wafer is the solution, I want to research other methods to controlling and understanding stress.

This is a long but good read ([https://groups.seas.harvard.edu/hutchinson/papers/462-5.pdf](https://groups.seas.harvard.edu/hutchinson/papers/462-5.pdf)).  Below are some of the highlights

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-001.png)

He claims linear scaling with film thickness.  Sorta what we expect (though I am suprised it is linear)

Main modes of cracking are below (From Tensile stress.  You get bucking from compressive stress)

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-002.png)

The rest of the article was a bit too in the weeds for me

This paper is a bit more on-topic for us ([https://pubs.aip.org/aip/jap/article/78/3/1673/489565/Temperature-dependence-of-the-biaxial-modulus](https://pubs.aip.org/aip/jap/article/78/3/1673/489565/Temperature-dependence-of-the-biaxial-modulus)):

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-003.png)

Not clear what the thickness of the film was, but it seems to confirm our intuition

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-004.png)

They deposit at 260, which is a bit below what we currently do.  They have crazy low powers too.

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-005.png)

Above are the films they made.  They deposited for 1 hr, so these can’t be crazy thin

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-006.png)

Ramp must be exceedingly low.  I am really quite convinced we suffered from thermal shock

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-007.png)

They annealed for insanely long periods of time, but I suspect that they saw most of the change in the 1hr long anneals.

Their stress results:

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-008.png)

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-009.png)

So it seems like films with more oxygen survived.  I am worried we might need to go thinner (though they deposited forever.  The biaxial modulus (the term with E) accounts for intrinsic and thermal stress)

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-010.png)

Another old paper that seems fairly detailed: [https://iopscience.iop.org/article/10.1149/1.2113992/pdf](https://iopscience.iop.org/article/10.1149/1.2113992/pdf)

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-011.png)

Their films are remarkably close to ours

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-012.png)

Something interesting here is that a thinner wafer would lead to less stress.  Something to keep in mind

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-013.png)

While this is for LPCVD oxide with TEOS, it seems that boron is good for stress

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-014.png)

Stress is definatley not nice to us at 500 (though they could measure it, so it might not break)

These people did huge wafers (12 inches), and noted that heating helped reduce stress by getting rid of H-bonds on the Si surface: [https://www.sciencedirect.com/science/article/pii/S2666978124000151](https://www.sciencedirect.com/science/article/pii/S2666978124000151)

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-015.png)

The rest of the paper is useless in telling you temp or time, but longer pre-heating (and possibly not using the carrier) seem like good ideas.

I read through this article: [https://pubs.aip.org/aip/jap/article/60/7/2543/12145/Annealing-of-plasma-silicon-oxynitride-films](https://pubs.aip.org/aip/jap/article/60/7/2543/12145/Annealing-of-plasma-silicon-oxynitride-films).  I don't have any great excepts, but it had a good discussion of how the bonds break and reform during annealing

The paper Aaron recommended: [https://www.sciencedirect.com/science/article/pii/S0040609097005427](https://www.sciencedirect.com/science/article/pii/S0040609097005427).  This is a good chemical analysis of film stablity

![Image.png](../../assets/fab/2024-10-24-stress-literature-review-016.png)

It seems that films can have quite a transient after we process them, which is a bit scary.  The crux is that films absorb moisture, which causes a volume expansion