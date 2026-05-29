---
type: craft-export
title: "2024-4-21 etching for mandar 2"
craft_document_id: 4127292A-F60B-463E-8D26-ED0F6CDE44AF
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-4-21 etching for mandar 2
This document is going to detail my etching process to create new phase gratings for Mandar’s project.  The issue with the last set of phase gratings was that they had a lot of gunck on the back side to due the cool grease used during the etching process.  This time, after chatting with Ryo, I believe there is a new way for us to approuch this process and not have to use cool grease.  



One other quick comment.  Last time, I noticed that one of the photoresists was a bit different in thickness than the other.  I believe this will require me to spin the primer on a bit faster.  The process flow will be as follows:

1. Spin primer and resist.  Then bake resist
2. After mounting samples on carrier, we will do an exposure and then develop the resist
3. I will do a 90 second descum in the oxford 81.  
4. Wet etch using Cr etchant.  I will tell when we are through when I can see through the substrate
5. Once the Cr is gone, etch the oxide using the oxfrod 81.  I think I will clean and reseason after every 15 minutes of oxide etching
6. Once the oxide is etched (which I should be able to measuing using profilometer), I will wet etch away the Cr mask

The advantage of this process is there is no cool grease used, whatsoever. 

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-001.jpeg)

Mounted sample

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-002.jpeg)

Moved by 5000, 5000

Exposure going

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-003.jpeg)

After exposure 

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-004.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-005.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-006.jpeg)

Looks perfect to me! Now let’s do a 90 sec descum.  I am first going to do a 5 min oxygen clean

Before descum

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-007.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-008.jpeg)

Result after descum

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-009.jpeg)

After Cr etch 

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-010.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-011.jpeg)

Now lets do oxide etch

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-012.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-013.jpeg)

I think we should use the CHF3/O2 recipe.  It seems to etch at about 44 nm/min.  This implies we want to etch for 17.7 mins (so 18).  Lets do 9, get our etch rate, and see from there.  First I am going to season for 3 mins

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-014.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-015.jpeg)

For real etch

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-016.jpeg)

After 9 mins

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-017.jpeg)

Resist is still on, which is a bit suprising

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-018.jpeg)

total depth of 668 nm.  We know we have a 184 nm Cr mask.  But the resist left, I would guess that we have about 200 nm of resist.  This means we etched 284 nm, or at a rate of 31.5 nm/min.  We would have guessed that we were 396 nm deep.  In all honesty, I have a really hard time gauging where we are.  It could be possible that we only have 100 nm of resist left.  I say we go for another 8 mins and see what we get.  I am currently doing a 15 min clear and will do a 3 min season after. 

Next etch

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-019.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-020.jpeg)

After etch:

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-021.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-022.jpeg)

So obvously we are not through yet, but we do have some more signs about how things work (now that just the Cr mask is showing).  I am going to assume I have 165 nm of Cr mask on my sample.  I have a total etch depth of (including Cr mask) of 699.  That means I have etched 534 nm of oxide.  I have done 17 total minutes of etching, giving a rate of 31 nm/min, which is what I guessed last time.  I want to etch an additional 250 nm of oxide.  This means I want to etch for an additional 8 minutes.  

Before etch

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-023.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-024.jpeg)

After etch

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-025.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-026.jpeg)

I probably have around 100 nm of Cr mask left (though I probably slightly under etched).  I am going to wipe the back side off and then remove the Cr.  There is still a bit of stuff (not idea how it got on) on the back of the chip, but it is not around the numbers so we should be good.

After Cr etch 

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-027.jpeg)

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-028.jpeg)

After spin cleaning

![Photo from Library.jpeg](../../assets/fab/2024-4-21-etching-for-mandar-2-029.jpeg)

The central residue was removed after a quick wipe of the back side with IPA.  So the main achievement of this chip is that we now know we have a recipe where no grease will get on the back.  

Unfortutnately we only etched 700 nm down.  We etched for a total of 25 mins, so this implies a general etch rate of 28 nm/min.  This is pretty slow.  We had 180 nm of mask left, so we can assume Cr is bascially industructable in this etch process. It seems that the etch rate slows down by a nm or two per minute over time, but this effect is pretty neglebable.  Assuming the nexy leg has etch rate of 26 nm/min, we will need to etch for an additional three minutes.  We will know for next time I guess