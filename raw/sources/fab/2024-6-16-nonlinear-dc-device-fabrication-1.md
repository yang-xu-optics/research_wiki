---
type: craft-export
title: "2024-6-16 nonlinear dc device fabrication 1"
craft_document_id: D4B79F0D-E4FA-46D1-A865-90790BC20B96
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-6-16 nonlinear dc device fabrication 1
The purpose of this document is to detaily my first Nonlinear DC Device fabricaiton.  Below are two design documents that help understand the device

[Nonlinear Waveguide DC Design (1e-12).pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/8ACD3252-9FB6-468B-B292-0CE6337B5FCF_2/PZ3YyxlH219ssQPBxMCV3AxZMwGcNlCeZYG1zUxVTbYz/Nonlinear%20Waveguide%20DC%20Design%201e-12.pdf)

[Nonlinear Waveguide DC Design (1e-11).pdf](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F2CAADE5-3AFA-4C51-900C-3F1DDBFAC66D_2/XNxTaYeJBw3fFxhx7Cjg6ltyPdF2rqXrzg10rwzFGfQz/Nonlinear%20Waveguide%20DC%20Design%201e-11.pdf)

These are guesses at the conductivity of the SRN layers.  I ended up deciding that the SRNs probably have nearly constant conductivity in the high field, as that is what Ryo’s data seems to show.  At the very minimum, these seem like genuinly good results.  I am going to keep the claddings thick just in case of substrate loss for low index contrast and, if the core’s have some dependance on field for conductivity, it would be useful to compensate for that.  

I am going to deposit 3um of the following film:

B8:

Temp: 300 Celcius

Pressure: 1800 mTorr

Silane Flow: 40 sccms

DiBorane Flow: 133 sccms

Ar Flow: 475 sccms

Power: 10W

N2O flow: 160 sccms

It is kinda silly, looking at the deposition code and the fact that I made this recipe 2 months ago, that I spent 2 extra months refining recipes to not learn a lot for the nonlinear device.  These simulations are quite helpful it seems.  FWIW, my refined reicpes (B12 basically) is the future for linear devices (or honestly even something done at 350 degrees).  It did not help that I was believing constant conductivity to be possible, when exponential conductivity is the reality.  The nice thing about the above recipe is that they will also have high breakdown.  

I am going to do 1 min season before hand, stop deposition at 1.5um clean, season, deposit (plus a 10 min anneal in-chamber at 350) and clean.  The previous dep rate we found was 62.2 nm/min.  This means we want to deposit for 48 mins.  We will do two depositions for 24 mins.  I will clean for 25 mins as well.

The Si wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/BEA20369-F34A-4AB0-8AAC-661B5788C700_2/1PzPrcSIQ4FyGK46JZLvPvq78hQiMxOcRPuQuMzwQcIz/Photo%20from%20Library.jpeg)

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/54ADDC45-9D56-4CC0-8B07-C58A14DBCF53_2/HONugT4NlLMyzstJv6HHNxnw7gwqYKz4ljLPg7AFlEwz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/8A7D981C-4718-4BC3-9F19-78D9750891C1_2/ll1YHxartqsqgWI83Cdc8Ev6ijhwSQKBZMZxu2t6A88z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/B5BECA24-15E8-41BE-91EE-9C5EC7CC4CF2_2/aX714boGMCJ4x6QqWogGGMZnQtTgXMMJeMxvngxhUeYz/Photo%20from%20Library.jpeg)

Before dep 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/80EC9AA0-84C0-4C49-AAE9-966E5F777584_2/nbt9koGrNAMnMMgJp35e8bLXz6xp83ZKYiDWA5eoKqUz/Photo%20from%20Library.jpeg)

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/574D0295-C7AA-44E4-9480-9CD792B57412_2/xs3SztDyPC1zyJ2pjv61hZ0ru3dE2fwhoYxJlGjaRiIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/633BDFA6-4B87-4DB6-84AF-1F8A3E833425_2/CvjYxNj86lwCxKnDuOBN2wkfuZh8MHuknkQffrrIiVoz/Photo%20from%20Library.jpeg)

I think, for the conductivity pad, I will do a 350 C anneal. I will use RTA for that. I will do it for five mins and ramp at 5 C/s 

Before annealing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F0542004-D3C4-42AB-97EB-D6F76B556641_2/WSIsOYyny3M5c7aY07sJESqNUOwrGbxwJ9rHWUMfPaoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9797497B-6D4A-4B5B-9C75-CB717AF9302C_2/gxldgxKT0VokmXI9HETOz62NuLzcOwKliuyyoN5BCL8z/Photo%20from%20Library.jpeg)

Calibration run of RTA

Temp sensor is a bit weird 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/03733A48-455B-4C76-A5D1-B4EA5298F873_2/XMwD5NPryupXxUcIWSvpYz8Nmu5mxsL0ZJg3WztFJaYz/Photo%20from%20Library.jpeg)

Honestly, I don’t really care, as we just want calibration 

During anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/E1E16CF6-0116-4CC0-98C6-DC11BEFD9FE2_2/kHZF9QVXFBKwi4pKhka1Da7n7azJ7OUk88wrZeoeAJkz/Photo%20from%20Library.jpeg)

Ellipsometee after annealing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/D0BD058B-E188-4FEB-A318-40097DD14796_2/P7x2NCGdlMZNUohEju31joVlOotf00LKyyqAWxPvMUwz/Photo%20from%20Library.jpeg)

To be honest, that feels excessive, based on previous measurements. I think the temp probe is just broken, so we will analyze this again later. I was also applying a shit ton of energy, so that might have been an issue too

Side quest, conducitivity characterization 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/20762EDF-7A53-4E35-8CC1-D1B27E88FDDA_2/UrK77AH1HDFMZ9szR3eQx7OO5lXM92M6UMYydkedjZAz/Photo%20from%20Library.jpeg)

From left to right, B22, B8, B21

Life is good

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/35737F62-A105-4027-A091-F0A285CEB0EC_2/7whBpes8tzcpyF1Szxi1boGEbFte6bQ5y2uoQqtEoiAz/Photo%20from%20Library.jpeg)

For Ti

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/E3275BFB-CC9B-4D8D-BFA3-202EF7555BE8_2/oVyo83Hx90yH3xiya6H6xcI3cDN8epWcHEHAiQTHmhYz/Photo%20from%20Library.jpeg)

The gate is closed, so I will just kinda get a bit of Gold onto my samples and call it quits 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/61E0CAB2-3EE3-46AA-B778-73C350B67BE5_2/yDISnlkgZDAqdI5gJIyPn02h53iZ5uQ3BlFkauPrqQsz/Photo%20from%20Library.jpeg)

Jeremy thinks we should be fine to anneal in the chamber (though he recommends Yes oven for the future).  I would say 15 mins at 375 would be ideal, as I am worried about any outgassing.  

Earlier index results for similar anneals

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/b051365b-dc9a-bb48-33ae-9e3d41af874c/T63T7UJRh7IX2jTSc6PVv0x6Y4xJYS913BX5iZuITQkz/Image.png)

I would expect index to go up by 0.01, which is totally fine.  Jeremy says we will notice the difference when we see outgassing.  It is not hard to observe.

Before season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/317F1B05-A6AE-4F54-B73C-1273634C0B0E_2/vNo15sPcqVwv9LW47Jyqih7FSMPTN226MkyCL5fbge4z/Photo%20from%20Library.jpeg)

During first season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/25D3D5D5-6D28-4428-AE66-CCA41C805B37_2/VJLr0xn1H3HwsDS0yJcbA6PEkxIOVCilmynZnJoypkkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A0D0ECBA-32A6-4BDB-9662-05BE43B476F7_2/WZmrZTCJu7ydayD6W38DU5i36EejvgCgbk6sdsTtnTMz/Photo%20from%20Library.jpeg)

What anneal should look like

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9B1983E0-A37A-4B2A-BCD6-B406A8C2AFEB_2/Od4kAvY1sqUwZ87954XltlkQ1PHIN3PTxTfNMk5RFqAz/Photo%20from%20Library.jpeg)

Before rep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/B86B31C8-F27D-4F33-A094-B3F0A4A11BB1_2/8gFwTjCyYs7JsiSTItdgBe5SXv3qCwrwrTl3yn9miqQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/09DB61D9-4210-4677-A115-8E29A05C1E19_2/9AAygSw9weIZzH9SX0xliPhzmAdJoN0mVR70Ds3vwHEz/Photo%20from%20Library.jpeg)

Let’s hope this works

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/4FC17C31-A001-4B4E-89BF-86E819DF849E_2/gMC60v90FcEhQQNSroMuglIG7pKZmDTc4beXWr6LV44z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/48824359-9285-465B-8B87-2D79F2DC7FA0_2/gy5UlT5YyLh0V7bCkKYylc0veDyfbTRrIXJzYVQFqv0z/Photo%20from%20Library.jpeg)

Anneal started at low temp

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/7FCC1F89-DFAB-4158-BBF6-1FAB39D86597_2/cqdOhFcTSbu9kJ8o6BmfhdCL33dWkbShLvRwjR4TrM4z/Photo%20from%20Library.jpeg)

I should still get ~10 mins of high temp, which is fine 

This is when we arrived at 375

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/AA6E0CFC-33FF-495B-97DC-DA0683E51D44_2/qsjt5zvmSpjeWURk7c884sUtrAgm1XYfxQeFpxDPUIoz/Photo%20from%20Library.jpeg)

Was above 350 for 10 mins tho 

Ellipsomtery (tough to get good fit)

1550 fit

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/524FF47A-6F96-4824-BE04-67D03450DB5D_2/Eb5Bblur7sLSxqpxL3fcx4SctAbB7HYiaQRhRNE7lZ0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/27938C93-D396-4545-88FA-406013254862_2/vix6Q91jR19lV1P3oIhzCacrg9fBAfy9zxCmzWCm6vYz/Photo%20from%20Library.jpeg)

Another possible that seems more legit

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/100F1C72-20A6-4C88-BAEC-47748CC3AC1C_2/NLdcpONWC4Aba4cLx8xLe63CPNwLFlAsKkaKUjTIoesz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/6E33D7EC-0712-4033-A578-21C9934573A5_2/HWDxIjQWyJKvtCxbZVqKCaiZtYpplunExqtdLL64Jwgz/Photo%20from%20Library.jpeg)

780 fit (not possible)



It is a bummer that these fits did not work, nonetheless, below are the indexes of not annealed to 3.5 core

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/EE75F804-1EEF-4FAE-A314-5711A4522FF1_2/b74YPj53CXTiXQgROIC2xz9vKaYyixgMbclEN6c8bXcz/Image.png)

At 1550, our gap is 0.05, and at 780, the gap is 0.03.  Not small gaps, but not huge either.  Put simply, we should next expect the index to go up by that much.  I also have futher evidence that we over annealed in RTA because I can see some stress issues at the edges of my films.  While it is concerning that I don’t know the exact indexes, I am not panicked either.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/CEA7D216-CDA1-42E0-B0FD-6D36144CEC73_2/CoZJpRHMMfkMJT4DfeXzyIUHvbVyN5Et2YMLxlNvHNYz/Image.png)

Loss (as shown above) should be managable too

Below is what Ryo’s screen looked like for SRN dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/ca277331-9869-21e4-583b-d08e4cce6d18/4Sq3Qn7QOuK6uVkt0EzEah3v9vyT08HYu5xULyOzQAAz/Photo%20from%20Library.jpeg)

His dep rate was 38.25.  Pretty decent.  This means, to get a 2.5 um film, I want at least 66 mins of dep.  I say we do two 33 mins dep, with 1 min seasons, and 35 min cleans.  I will also do a 10 min extra anneal before first dep just to make sure stuff works.  

Before season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/6208F551-8296-4E9F-B9A8-ED430FC5F349_2/T4OVRO9Rm5FtlAR47ipxXQXO6hMGfTmFZsyWvyNBMywz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/3A2DAAC6-0839-4765-92DD-EDB7576F44CE_2/IZIghCj2nzs4yzxc83u1LYVCzez1sk3n3MNLGtvyxAcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A77F829A-6F13-4148-A751-8E3809A8F2A1_2/DepNpoXq6ejqXWDJLSbtv0jbpG7srK0GjmmtXi8ZMKQz/Photo%20from%20Library.jpeg)

I am going to deposit on three of my six cleaved pieces and do 10 min anneal

Before depositing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/B1FD76BA-4338-493B-A30D-585BD34BFEBF_2/lx6Cuz6TH1ArDoF4olUXNgX6YtXhrZqK3TrfCnmvrvIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/EC5AD20D-DEA2-4839-9254-B9B4D2E51648_2/ZOZXDxZMo17Fjq9GJoIeCNRrJ6kq5w0u6DyjzXgyexwz/Photo%20from%20Library.jpeg)

During anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/51BC6B40-5B2C-4504-B27A-1396E00A7AF2_2/3GSyyvUy2TzbNKnn0q5gtzPTdTjHVpPLb2azo4TFsCcz/Photo%20from%20Library.jpeg)

During dep 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/387DF0C6-813D-4ADE-AC08-52C86C84FF04_2/pCHEOKPoefxN7FAElcpsdvYC2fsE0p3IyuzePoykTr4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9DA88096-D263-46E2-9CA6-3DED5419E56A_2/nnyg0WKwedlNj0kyLU4Mt5Du4NSCnDU12SJQMIERBC0z/Photo%20from%20Library.jpeg)

After dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/D71A8C4C-613F-464E-AE1E-5D87EC0CE4DE_2/FoxeXIyRYo3cFiPTAP9vgaRJRkDh3CmczHH14JGcEw4z/Photo%20from%20Library.jpeg)

No evidence of out gasing 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9A81B8EB-C5B1-46CF-A2F7-71454B425BE0_2/SXk945U7yvWxRbEsJjU6Z78NsWixyhT0deCPyO9Kg0Qz/Photo%20from%20Library.jpeg)

Left side of box. My dumbass forgot a witness sample, but I will add it in next. Plasma was on, so we def got something

Before season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/0A804635-BF21-45C2-BCAE-355949C0C03A_2/ZtIPzyckmwBxGbmfbxE0fdJKXQKrRpEU7fEgDr8in1Az/Photo%20from%20Library.jpeg)

During season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/071F9649-4A4E-437E-9046-EF8248B0CA09_2/HfTAXp1SfL1uQVJcqZmPGZaciTcoZjQBfB3bleWdEdkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/659A4CD2-B08D-4809-B070-24784EBBF256_2/ZlcjjjWhPIEo1tRqgKOfQ8n5l0Gz3uWxjOctIoVHazIz/Photo%20from%20Library.jpeg)

In the future, click the pump to pressure button if the pump step stalls

Film on right is Si witness

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F1B75633-3FCA-449C-85C0-B06614D1A27B_2/Fd9mi8UfjC7WxhVtdF8yE8EyCHZmfMSk8H2w5He7Ph4z/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F9CF23A4-C560-4C4A-8F53-35720A125CFC_2/hyzeUfr1QiSL8dvOFGdFoyHjNHjvn0WCwaDXkZOKmHgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/035D4706-3BB8-410C-8FD7-E8505448ACE2_2/RyviL8fHa3iZCxqB1DmaGFVZuNuhmBli92yHVH6ZsZcz/Photo%20from%20Library.jpeg)

No annealing

During dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9C448C00-35ED-478A-8A66-026374BCC63C_2/QDAABvTzPjPvu5P9O1mxpx6aol8pkGY7UVxxX8ICFWQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/64591348-F39B-4A0E-96B6-430D6BB81D7E_2/N3k9aXpM2PTayXY0uYJmv9VVcx7DZVZlxzb4qefeykQz/Photo%20from%20Library.jpeg)

Ellipsometry on witness 

Short range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/B8AD9132-BAB0-4722-B10F-0D438C564CFD_2/pU2hQy1hnXl9BUUD22IIby5vfVeaxzPqA83PTtPToJMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/35B198B9-DB9B-4849-B798-0039929EABFD_2/s1qgDoF1LC6EnpWMOe4kJ5xeJbIVxOfTyaEwX2Cf1vMz/Photo%20from%20Library.jpeg)

Long range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/4FE0572D-15D2-4A2C-8A09-76665138BFDA_2/4IuOq9at8x4yI02T4IRJKBS96xJDhD3FxIQD1JFC2m8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/739811E5-C895-4839-B2F3-AC0C8D3FF4AD_2/wzMX0xZ6z4KCCqyOFICejq1v1hcNhCq5C28yUfRgRQAz/Photo%20from%20Library.jpeg)

Retake of substrate

Ultra short range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/B588F7EA-F331-4643-AAF3-A02C28DD5D86_2/Zi3n1WVqcZ1X9VZ7gGUIla6TUW8qqxvU4g0etKI0NbAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/0B3A42F3-8A44-452A-B250-0584807D9198_2/RxWu9t3GkW6t9ppExq0LRsUup7Q2DDFDR5zztYHaxsAz/Photo%20from%20Library.jpeg)

Short range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/921B6FF4-0FE1-4AE4-BED2-A4A522B0FF07_2/timSfu3ztK5ibtXRfUHjWKPe1JYOZR3vGCJTibtWWygz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/AA037BA3-F8D6-4B4E-8A53-A207AAFF43B3_2/GPvivub2OpE47yPx5dHg5Hq7cVFabH9tNJNDbvkZxhoz/Photo%20from%20Library.jpeg)

Long range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/DF6F73F7-8F36-4CF0-A22E-4AC92806FF24_2/M6ydVyQmyBq5h2GIqOjpzlypcx8hZd9qxkkqlO6ycdoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/462F92A6-08E3-480A-8131-0D7DF731D5E5_2/KqYZR7kf5JxxoahgNZe8K8AYKySyCfusX0cbfsikWlAz/Photo%20from%20Library.jpeg)

We can def see that k is higher here. 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/C506124C-2BBD-496E-B7BA-27CF1E2959C4_2/6NLp4abQhHESo0ERB5BXY3JKxFVstz71XiO1Gqdq4Vwz/Photo%20from%20Library.jpeg)

Left side has SRN

Index of SRN looks very similar to before (maybe a bit lower).  But our characterization seems to indicate that the indexes should be ok.  We will confirm tmrw in the lab

Below are the characterized losses

1550

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9D31F7A4-D015-44CA-BBED-23DC6E3FB27F_2/YZiNOmptdYVDpH9ebWkIvXpFAq3nPbfNMYsA7q645GEz/Image.png)

1064

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/66ADA431-4362-4039-AA6E-5BD8BAB18572_2/H68Sxyz4UngdtFv9eGZ4MtTj68xQoTxChRHC53WEKi0z/Image.png)

780

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/362B12C1-98F2-4752-8341-A2D651EDD0CC_2/dVgXthyxw6pXTDh2I2XM0kWLQVc5pLaLTskHUbghxIsz/Image.png)

Before top cladding season 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/4B6D965D-CE14-421C-A622-8D999743AD82_2/Cix8sAlv2u7ZLF6xKxhKrJ8SUTNWYQGlmbQjkC1CrKgz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/3E4EC8A7-6DCF-45D7-8179-8419A664EF11_2/E9cLubPcwHSNsDJ1q3ZSFUIykJ1nyLyTnHTSm4DJzqMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/5CB10499-2E70-4ED8-8751-8BE9D3443C08_2/HFEktebNfQuc3k5kMQB3Sad1T893iX8tVMVO8Su7df4z/Photo%20from%20Library.jpeg)

During deposition 1 top cladding

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/326FDDBC-6F15-4799-A3E7-BCDFB40D658E_2/TJJLqEqhJY67EDSExKgKzx1P2luyFyQBySWSWJMiiDcz/Photo%20from%20Library.jpeg)

Witness on right

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/27F769B2-47A5-4479-8F82-E2547FA84E12_2/tuqz2C3KD15q74VLsmAyiVwa9KM5ZbU2lIP99LDIkHgz/Photo%20from%20Library.jpeg)

During dep 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/37B06567-8236-4EB9-89A0-69A2F8BCBB7F_2/PZFeAHsRhXYQkUcSE5xByNjiyTLOoU7eT6T0noxr3hEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/B4B077E2-8C5A-4606-988D-B2CF3A7F567D_2/D1mScy8HHTTZG488NIOnYeFswaLlbPBWeGcys7aGIkUz/Photo%20from%20Library.jpeg)

After dep 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A48FA1AA-B801-48BD-83E6-75B2B8167007_2/sV9Sj9ByGLRH1k9bGLZ6Kt4Qy04xKdK5mdL31J6Q330z/Photo%20from%20Library.jpeg)

No evidence of cracking or anything like that

Ellipsometer

Short range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A15831B9-EB27-42F9-90BA-4A98F5DCB5BE_2/FWie2ao9eWSf48kykOjI21z9uko86N8ejIzgxzURhMMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/9441E3FD-8681-4668-AA34-65CED6183C6B_2/Fx7t7v2KRfnhNwggRNMDYzvRXFXG8qY1P128AQNB1yAz/Photo%20from%20Library.jpeg)

Long range

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A960DB35-4DD7-47BD-A346-FE32EA783438_2/VbSnD6pkmZTRN7UjcgrQ2lXZasrsC8aTt9UnY3WbGyUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/0551AC10-8688-444B-B598-1810451D21AA_2/uQFZJYYyG3bTQhAHi26wV3R7t9GmxWbmMaE7lqWW3Pgz/Photo%20from%20Library.jpeg)

Before season 2

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/C63EE35A-4013-417C-B53F-545ED03D73CA_2/cu6UWTGepSO3mOZDipRKDsqWGOnyhoo3aqjUCrPsLOgz/Photo%20from%20Library.jpeg)

During season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/8AA421EB-DCBA-4572-9E42-B3683708DFBA_2/8DLEiLz5xPMRxtHHV6PNVOOaaqKiJtj4vXmdAjTX310z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F8CD9437-5E11-459C-AB29-B099D693745E_2/mztVlCZgVVs5E2YacD9rXElfrqg0CemBcFOvNgCsAMcz/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A9059F67-4E8B-49C8-9364-0BF733B12DF7_2/xb8sJjISoo2ZVob3ucxhVzyIVcyvYb2a3AIgVVKHLGMz/Photo%20from%20Library.jpeg)

During second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/88F86CC2-2245-4A38-9C15-0BD3645698E0_2/Bj4q2OQNuQQ7NR59myBD1A2S10aHITolilCqiUxrLzUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/96C1A77F-4B2E-49AD-B107-42F1D6C383EE_2/5T3uBTu5ybB59zRnRwdgynvxHB84j5QsxHkDz8hpAEEz/Photo%20from%20Library.jpeg)

Tapes pieces

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/F6717068-1D76-434F-8C39-1B1C510B51F6_2/hn37oHQBuLtHkcxtljxSZrOgRe01X9iQKVpf4rPFHuUz/Photo%20from%20Library.jpeg)

Top is device, right SRN, left DON

Side note: Ryo’s direction 1 is the shorter propagation distance

Full stack at 780

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/5F9976A8-27A3-4193-A7AF-4C2FA1619C48_2/CQJR7qX3VIFpVIlubNeXythXsDNZvNxxN1Sc7ykapJcz/Image.png)

Keep in mind, the light had to travel 2cm in my device, so the fact that we saturated is not a huge deal

Ryo stack (short direction at 780)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/E8CF50F8-649A-4B9A-B1A4-1122019397A7_2/zzM9bimiwygFaOt2CowNnWKiHCeCn2zZbWE9kDfjrbgz/Image.png)

Ryo stack (long direction at 780)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/A1A1AB40-6224-49A7-B26F-09B75F848854_2/4my5TSodouUc8xOXHhYAONYD0I88UzxuQ4J4UFSqXowz/Image.png)

Ryo Stack (short direction for 1550)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/170B2FED-6AC0-4363-97F4-C907D5F0FE5C_2/agWbmLtTJ6D8CcfyZ6gdMWMqBA16ZBduiWrvspp6rG0z/Image.png)

Ryo stack (long direction for 1550)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/D4B79F0D-E4FA-46D1-A865-90790BC20B96/CDDDDC22-49CF-45F1-B222-8CC73C2C14E1_2/q6mDr9G6V4zHviPHywPfIidfnG4iLny1y2FHnncnygEz/Image.png)

So my stack is probably 2-3 dB/cm at 780, which is much lower than I expected.  The only weird thing I find about Ryo’s stack is that he has a grating structure

