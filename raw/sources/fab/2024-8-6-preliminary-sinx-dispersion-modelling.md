---
type: craft-export
title: "2024-8-6 preliminary sinx dispersion modelling"
craft_document_id: 1A00507E-3308-47BE-AFF7-664C9D0EEDCE
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-8-6 preliminary sinx dispersion modelling
Previously (in a somewhat scant craft note), I worked on figuring out the basic mechanics of Ansys lumerical.  In this document, I will try to create the 3 graphs that Marc usually creates that Ryo believes would be best for modelling the disperion of etched waveguides. The three graphes are listed below:

1. Phase matching period.  This is the difference in the betas (Which lumerical can just give me).
2. Group veloicty mismatch.  This tells me the temporal walk-off.
3. Group velocity dispersion.  Tells me how broadband the device is basically.

Ansys gives me all the relevant numbers, so I can just use those.  I will have to do a parameter sweep of both height and width.  I will probaby save the first order mode of the pump (TM) and the first order mode of the generated signal (TM as well) for now, though in the future I might work with more modes.

I am using a mode that is SiN (using one of their default materials), with oxide claddings around.  In the future, I will need to upload the Cauchy fits for our SiN waveguides to get something slightly more accurate and make the waveguide geometry more accurate.  Currently, it is not quite accurate to show the waveguide as a perfect strip, as I might not etch that deep and there will be a ridge waveguide instead.

This link tells me how to do a nested sweep: [https://optics.ansys.com/hc/en-us/articles/360034922913-Creating-nested-parameter-sweeps](https://optics.ansys.com/hc/en-us/articles/360034922913-Creating-nested-parameter-sweeps)

So far, I have a very basic simluation created, where I sweep over two geometric dimensions and frequency.  Unfortunately, I can’t access dispersion or group velocity yet from this model (at least in the sense that the number won’t be given to me).  I will continue to see how I can access it, but it seems to require a frequency sweep, which I don’t know if what I am doing counts as such in the software’s head.  Nonetheless, below shows what I have access to thus far:

Small height

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-001.png)

Large height

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-002.png)

effective index went up, which is what we want

Exporting data seems to be a real pain (this is putting aside all the pain of eventaully manually calculating some of these derivatives).  I can’t get any nice excel spreadsheets like I could with ansys maxwell.

For now, I can just export everything as a text file, chop everything up, and get rid of all unwanted text.  It will require me to save stuff quite dilligently.

**I FOUND A BETTER WAY TO EXPORT THE DATA**.  In lumerical, you want to make neff shows up in script workspace.  To do this, click the top paramter sweep in the nester array of parameter sweeps.  Then, you should see (in the result view window), an icon with neff written (or whatever you named your variable).  Please, make your life easy and try to name things correctly.  Next, right click neff and hit "send to sript”.  If any windows are not open, go to view and then windows.

In the command prompt, save the data by writing matlabsave (“filename”, neff);  Then upload the file to your mac and use the code that I am devleoping now



As for data types that I can export, I can get group index and effective index.  Effective index will give me the phase mismatch, while group index will give me GVM.  I still don’t have direct acces to GVD, as this requires a derivative that I don’t have.  Let me see if I can access it somehow (as it does not like returning anything from the frequency sweeps)

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-003.png)

For reference, this is why getting dispersion will be tough.

I am just going to calculate analytically for now using freuqnecies very close to the center frequnecy.  I am going to run a large simulation overnight to get an idea of what I should get while I develop the code base to process the data.  I will be looking at the TE fundamental mode for 1550, but we can adjust things later if need be

I seem to have extracted the group index (alas, the neff did not quite save correctly, so I will rerun that simulation later) from the large sweep.  Below is the result

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-004.png)

The way the data is saved ia kinda a pain to easily unwrap everything.  That said, it should be possible.  We can already try to unpack things a bit more to get GVD.  I am a bit worried about the datastrucures not quite saving with eveything in the same order, but hopefully that won’t happen.  I would also hope to make scan an integer different number of height and width in the future just to make the distinction a bit easier

Below are the functions I have coded up to analyze the basic values Ryo wants from me

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-005.png)

The GVM and poling period ones are right from the definition.  The GVD is from a numerical approximation, but otherwise from definition.  group velocity is probably a tacky way to derive it, but I was unsure whether taking the inverse of ng would give me the right answer either.

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-006.png)

First plot of GVD.  I can’t really tell how accurate it is, though it does seem like a thin waveguide is best.  We get GVD of almost zero there, which is pretty good.

Below is my algorithm that sorts out a .mat file when given the name and type of file you are dealing with

![Image.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-007.png)

This seems to work well.  I was able to replicate the plot above using a differnet data set with this code.  Now lets see if we can find the poling period, GVM, and GVD using all of my data

Below are my first full plots

![First Dispersion Plot.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-008.png)

![First Index Plot.png](../../assets/fab/2024-8-6-preliminary-sinx-dispersion-modelling-009.png)

I don’t have much of an intuition for what these values should be (though the neff and ng values feel right).  The poling period feels a bit small, but for GVM and GVD, no idea.