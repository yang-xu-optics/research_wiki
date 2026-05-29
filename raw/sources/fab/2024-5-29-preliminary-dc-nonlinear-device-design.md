---
type: craft-export
title: "2024-5-29 preliminary dc nonlinear device design"
craft_document_id: 41F53722-8075-48E4-87F9-19DC380D8B54
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-5-29 preliminary dc nonlinear device design
After the subgroup meeting this week, we decided the following two things:

1. I should not seek to knock my first LN wafer out of the park.  Even demonstrating DC operation with sub-optimal performance would be acceptable
2. We should start by proving that a DC nonlinear device with my DONs works first.  This is definitely a safer bet than going straight for an LN device.  Will make the project take longer, but at some level, that is ok.  On the bright side, I can do this ALL in-house and control each film’s parameters.  

Getting this to work will really help Ryo’s project, as we could get some really crazy switching ratios.  It is also just convinient to work in DC in general, as that could possibly be a selling point of Ryo’s device.  Anyway, after discussing wtih Ryo, we have two options for these devices:

1. Put the mode in the core and use field modulation in the core to induce the nonlinearity we want to see.  Because we are projecting the nonlinearity pattern onto the field, we really want amazing confinement
2. Alternatively, we could dump most of the field into the claddings.  From previous measurements, we have found that the claddings can have quite a bit of induced nonlinearity too.  For this device, we would want VERY weak confinement

The advantage of 1 is that the device is very conventional and easy to model.  It would also have a bit less in the way of fringing effects, as the core in a 3-layer core/photoconductor setup has great contrast in the core.  The disadvantage is, because of loss, we would have to use a low-conductivity film.  This means we would have a long time constant and will probably have to use oxide films that are more resistive than our current breed.

The advantage of 2 is that the device would be very fast (as the SRN would be thin, so lower resistiance).  If oxides can get lower loss than SRN, it would also be good because we would loose less of our signal.  The main downside of this device is we would need exceptionally thick oxides (as that is where the mode would live).  My oxides deposit half as fast as Ryo’s films, which is a bit of a pain.  The other disadvantge of these devices is that we would get some fringing in the claddings.

For now, lets plan on doing 1 (though optical loss measurements when I get back to campus should show which setup is best).  I will do simulations of both setups below so I have some fall backs.  We also need to consider the predicted poling period, as we don’t want that to be too low either.

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-001.png)

This is a quick confirmation that I am working with the correct poling period.  It is somewhat interesting to me that I get slightly different poling periods for this device for the two wavelengths.  One of the above solutions is a numerical solver, while the other is the analytic solution.  They are only off by ~0.4 um, so not a big deal.  It seems, for thicker cores, the poling period is a lot less sensitive to device changes.  Ryo might want us to work with a lower index than SiH4 = 4.5, but for now, I will proceed this way.  It also helps because I believe I could continue to use my existing oxide recipes.

Below are the modes

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-002.png)

Confinement looks good, so for the moment, I am going to prioritize some of my transient solution results.  I don’t know my conductivities perfectly, so I am going to make a few assumptions (which will be detailed below).

Claddings are B12.  This means cond0 = 2.081e-12, expo = 6.275e-8

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-003.png)

Core is assumed to be SiH4 = 4.5.  Below is Ryo’s data for a flow of 5sccms

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-004.png)

I would assume that SiH4 = 4.5 is lower.  I am going to say the following:

SRN_Dark: cond0 = 1e-10, expo = 1e-8

SRN_Bright: cond0 = 1e-9, expo = 1e-8

We can refine these numbers as we go…

For the above numbers, we get (operating at 700 volts):

Dark

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-005.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-006.png)

Bright:

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-007.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-008.png)

As switching goes, this is awful (220/140 = 1.57).  The voltage is probably a bit inflated because we are using thick films and we can pack more voltage into the SRN.  The first improvement can probably be thinner claddings, as the mode seems fairly well confined.

As a side note, I do notice that my simulations work less well when I apply really high voltages.  This is something to consider (as we should not get negative voltages)

Lets do 1um claddings (operating at 600V)

Dark

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-009.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-010.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-011.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-012.png)

So this is kinda interesting, we still don’t get a good switching ratio (195/145 = 1.3X).  I mean, this is not dreadful, but nothing near what I am used to.  I believe the key issue is that the claddings are NOT resistive enough, which, I must admit, is a bit of a supring result.  So one easy path forward is to just leave one of these claddings be (so leave the bottom cladding as resistive

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-013.png)

This is currently the extended plot of conductivity.  Ryo says we should look for linear switching as close to 200 V/um as possible.  300 of course would be better.  So lets leave one of these oxides as conductive, and start sweeping the cond0 of the other oxide.

Dark state (operating voltage, 900 V) 1um claddings

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-014.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-015.png)

Bright state (same as above)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-016.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-017.png)

It is just very hard to get good swtiching here.  I would proably slightly increase the amount by which the SRN conductivity scales.  I am also going to use a 10W now

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-018.png)

Dark (900 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-019.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-020.png)

Bright 

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-021.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-022.png)

Wow, nothing.  Lets really kill our conductivities

Dark (900 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-023.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-024.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-025.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-026.png)

Let me try this bright state with a higher bright state conductivity.

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-027.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-028.png)

I think what makes Ryo’s films and my films hard to put together is my flims become more conductive far faster than Ryo’s films.  What is sorta intersting, in observing my above films, is that it does sorta seem that the steady state solution does get close to the point when all the flims have the same conductivity.  Not quite, but close.  

I should also add that I don’t want to go much higher than 900V, as we can’t apply much more than that anyway.

Lets do huge switching ratio for blue light (I also changed bottom oxide to more conductive, top to less)

Dark (V = 900)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-029.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-030.png)

Semi-bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-031.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-032.png)

Very-Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-033.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-034.png)

To get 100 v/um of switching, we need a very conductive core in bright (huge switching).  It is also interesting that, as we work at higher voltage, the speed of the device increases.  Time constant is not as issue, as we are working in a regime where the fields make the conductivities high.

At the beginning of this exploration, we were able to get almost 100 V/um of switching.  Why is this.  I think the key is the correct operating voltage (higher may not always be better)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-035.png)

Also, after doing the simulation, I was curious to see what the final conductivities were.  They are not matched, so I can’t quite use that to predict stuff.  It really does seem like we must just solve the differential equation. Lets go back to that configuration

Bright operating 900 V

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-036.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-037.png)

Dark

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-038.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-039.png)

Switching of about 55. Lets just start scanning around the operating voltages.

Dark (800 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-040.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-041.png)

Bright 

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-042.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-043.png)

About the same switching

Dark (700 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-044.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-045.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-046.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-047.png)

Bright (600 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-048.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-049.png)

Dark

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-050.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-051.png)

Dark (500V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-052.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-053.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-054.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-055.png)

Notice, this was the first stack where Bright state SRN went down from capacitor value.  Raw contrast is no better though.  Do notice how using higher voltage does get us a faster device.  So any concerns about device speed were misplaced.

Dark (400V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-056.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-057.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-058.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-059.png)

From this scan, I rule out the idea that lower voltage could lead to better contrast.  We should just use higher voltage because it is faster.  Before, we used claddings that were thicker.  The advnatge of that is the field in claddings can be less, meaning they might not get as conductive.  Lets try some devices with thicker claddings (which is ironic, as we really don’t want that in a normal device)

Dark (2um claddings, 900 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-060.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-061.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-062.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-063.png)

That’s more like it.  

Dark (3um claddings, 900 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-064.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-065.png)

Bright (3um claddings)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-066.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-067.png)

This is still sorta stuck around 90 V/um of contrast.  If we upped the voltage, it might be better, but we also can’t get a lot more voltage out of the setup

Dark (4um claddings, 1800 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-068.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-069.png)

Bright (same as above)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-070.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-071.png)

So ya, contrast is a tonne better when we have much thicker claddings and more applied voltage.  The issue is this device is juse not practical.  Lets try thinning the core a bit and seeing what happens

Dark (4um claddings, 1um core, 1800V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-072.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-073.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-074.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-075.png)

Pretty dramatic improvement.  Lets bring voltage back down to 900 V, as 1800 V is insane

Dark (1um core, 4um clad, 900V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-076.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-077.png)

Bright (1um core, 4um clad, 900 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-078.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-079.png)

Right, contrast is still really good (best we get at 900V).  But using higher voltage is also better.  The key here, again, is we want as thin of a device as possible where the core is much thinner than the claddings.  I should mention that the field in the claddings does not change a tonne.  So we could not use this in the delta_waveguide situation.

Dark (2um claddings, 1um core, 900 V)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-080.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-081.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-082.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-083.png)

Field in claddings does not change much.  We now get 130 V/um of switching.  If we used higher voltage, it would be higher.

Dark (Voltage = 1800, core = 1um, clad = 2um)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-084.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-085.png)

Bright

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-086.png)

![Image.png](../../assets/fab/2024-5-29-preliminary-dc-nonlinear-device-design-087.png)

Interesting, so besides reasons of time-constant, operating voltage can be hit miss.  There seems to be a point where the amount of field-contrast we get saturates.  I have a hard time telling when that is.

Ryo gave me a few more device contraints.  We can apply up to 2kV to the stack (though I would probably cap it at 1500 V just to be sure).  He would really like us to use at highest SiH4 = 4.  From my simulations, I honestly think we could even use SiH4 = 3.  We would already have thicker claddings for device performance, so longer evascent tails is not a huge deal.  This will mean that we will need a crazy thick core, but at some point, oh well.  The main drawback of this device is we will need to operate at higher voltages.  Time constant stuff is kinda dealt with by the fact that the claddings will become more conductive with more field.

So lets do a scan of effective index, pick a core, and the adjust claddings and votlage to make stuff work.