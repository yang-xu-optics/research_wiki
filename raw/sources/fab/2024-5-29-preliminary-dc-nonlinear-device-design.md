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

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/528B0DFF-01C7-4699-A931-8DB203E82091_2/zWsnXoRy45Wm1KeBIUzjS8zge0S86NovyccBpelWtKoz/Image.png)

This is a quick confirmation that I am working with the correct poling period.  It is somewhat interesting to me that I get slightly different poling periods for this device for the two wavelengths.  One of the above solutions is a numerical solver, while the other is the analytic solution.  They are only off by ~0.4 um, so not a big deal.  It seems, for thicker cores, the poling period is a lot less sensitive to device changes.  Ryo might want us to work with a lower index than SiH4 = 4.5, but for now, I will proceed this way.  It also helps because I believe I could continue to use my existing oxide recipes.

Below are the modes

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/33892EA4-EA2B-4EF5-AB24-198E8F8082E0_2/6bFQijK1E7MRoyOTCnNcSURPiBqM4Vgq95MzBtkpBwAz/Image.png)

Confinement looks good, so for the moment, I am going to prioritize some of my transient solution results.  I don’t know my conductivities perfectly, so I am going to make a few assumptions (which will be detailed below).

Claddings are B12.  This means cond0 = 2.081e-12, expo = 6.275e-8

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/0d117d5d-203e-c9f3-01cd-e6af678d55ab/q6yZuyGGvyNN7Zbmi73kyJpqQ5YnwDx8yMdXT4cbNj0z/Image.png)

Core is assumed to be SiH4 = 4.5.  Below is Ryo’s data for a flow of 5sccms

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/91e26082-aba5-7e24-3214-0a2909f5ef87/bLyjyDcejKgjecrRVq70pPL6AA6cpEPYri9N0JctlFkz/Image.png)

I would assume that SiH4 = 4.5 is lower.  I am going to say the following:

SRN_Dark: cond0 = 1e-10, expo = 1e-8

SRN_Bright: cond0 = 1e-9, expo = 1e-8

We can refine these numbers as we go…

For the above numbers, we get (operating at 700 volts):

Dark

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/259BDD22-5148-4BAB-BB55-CB1AB8B1D8DB_2/VpXZyiQoOTaJKB33uZ5ib0DqQi647T2yjFob95iWntkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/39D38681-4B8A-4D46-929E-E23757F455A7_2/YJTy7wFkv6LHQuQB3j7O1BK8h51GuWYktsY8Rx0kffsz/Image.png)

Bright:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/349BA765-44C3-4552-9BF2-41F455390D23_2/WpvLzxeKo8xqvRkF3KvXiLFVcNjt96H6qFjdyfe1Kq8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/F6D0FCED-46DD-4779-9BA0-8EC36ECF07B1_2/SyaRAhQ988G7jjbwTxATyjHP8LLZBJcA1ZP2ABpTSRYz/Image.png)

As switching goes, this is awful (220/140 = 1.57).  The voltage is probably a bit inflated because we are using thick films and we can pack more voltage into the SRN.  The first improvement can probably be thinner claddings, as the mode seems fairly well confined.

As a side note, I do notice that my simulations work less well when I apply really high voltages.  This is something to consider (as we should not get negative voltages)

Lets do 1um claddings (operating at 600V)

Dark

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/37AEE57F-D83D-4A70-B753-D6773E58039B_2/dSotgUwHk4IkyHyKUwZ9LFXRlx726Hdx7MO3opyXZhQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/F12F6E12-C553-4011-B19B-3F893939731A_2/xmDNRZrR8yXJfFtYxozxAcWdNZdMpQVRnGKwkV1802Qz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/0958CB7D-F888-4D9D-BBB4-CC0F793E07A9_2/JZyr5w4NToAuilWH1jEjTUyC6r5vvZquIUkQiw3xvu8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/D6E75208-9C61-4EA4-ABE4-E5576243DF5F_2/SF4rW495gmgV2YGC2fzaBCA33vcjhO7dDlU80wRoovUz/Image.png)

So this is kinda interesting, we still don’t get a good switching ratio (195/145 = 1.3X).  I mean, this is not dreadful, but nothing near what I am used to.  I believe the key issue is that the claddings are NOT resistive enough, which, I must admit, is a bit of a supring result.  So one easy path forward is to just leave one of these claddings be (so leave the bottom cladding as resistive

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/1B0283B5-6E97-417F-A259-C72182D0322E_2/QsLceGlzUxC2VzTWxaGJX2kGVaKNpv13wj33MqESVfwz/Image.png)

This is currently the extended plot of conductivity.  Ryo says we should look for linear switching as close to 200 V/um as possible.  300 of course would be better.  So lets leave one of these oxides as conductive, and start sweeping the cond0 of the other oxide.

Dark state (operating voltage, 900 V) 1um claddings

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/FE5E2521-489F-41CA-926D-114FCAADBB56_2/vqeyyIZiBHdzk0zxuWcKx35RRvq6YkuWCctKxBpywakz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/1976343D-BCCE-4E68-9F55-06C29BE88776_2/9JPKety5s8O46BnZlHykwEc5OeVL5dIglbw08mODNvgz/Image.png)

Bright state (same as above)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/7E97771B-1234-414F-842E-657D4606DE3C_2/bqMqOAJds8wMBPkRf1Zd6TcLyUylOIkpzau3s0skAaAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/82DB4C57-BC27-409F-B354-DAA854B2885A_2/Rqg4qLusj5zZIzijyVyTTzM8uOma9yZE1KVfIxMkxD4z/Image.png)

It is just very hard to get good swtiching here.  I would proably slightly increase the amount by which the SRN conductivity scales.  I am also going to use a 10W now

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/aa2cedb0-80c3-29a6-3356-1d12a271f1e4/4r80TMlEEHllXX8zMFc2ybxrnLWx0bVIq5eWaxzdkx4z/Image.png)

Dark (900 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/BAEE34C2-BAEF-42AD-AC2B-71945DF0449C_2/yrsixD2iWjBtMWTbqnyUT9Eq5RPuiQxjLsYbxDbzE0Yz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/796192DF-DB50-48BC-AEE3-7F356691CD77_2/quu8Ah59gE8NQy9CWWKMsRNX0xutTQYsCya53yGa7jkz/Image.png)

Bright 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/51A4D0A0-9DD7-4237-A40A-2934212A6DEF_2/CHcQmSSUuNY9cvuobqdQVwHwEGOxCtB1wrMc2VHgxxkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/F38252BA-0CFD-477F-B292-A8EAF5B0E198_2/QpXSkByxySU5uBHDdKLw6gOTOVCf76dBBRZFrbHKmCEz/Image.png)

Wow, nothing.  Lets really kill our conductivities

Dark (900 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/A17EEE86-9770-4E75-9D54-FD58696BFA2F_2/J7dxyt6zqBCrxqHgoQtqREaXyd2gQtVXMzHNgj16A8Yz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/AD6710E9-1EC3-4483-ACCF-CCDD0B8C597A_2/5QOvLN53WiycAMiuoyM1xsBR1xypuXDUQD4ASqAGOIEz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/73437421-D97D-450E-AAD3-D50D74BB590E_2/2hDzmUktKtrkFWtvf8x00K760MxMkfK5Sl6NOjZtPFMz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/0501833C-5B9D-46C8-BF08-A921FC63B472_2/BNG2TCHdER68tF5U8xZyK8mnmRV48bhwXyRynhbRxxYz/Image.png)

Let me try this bright state with a higher bright state conductivity.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/21F9384A-05A4-4863-B029-47DD679A6C7E_2/L4k43Oq8Uh1oIDWRaV8Tpahkfs3PVmLxwV9xUCuPf1Qz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/A5F20A9D-B2B0-473F-A266-55493A13AA56_2/mEJ7rd1ufVx3Yu9fEsWNpiW5jQ02QBWC3HVWG7zcwxYz/Image.png)

I think what makes Ryo’s films and my films hard to put together is my flims become more conductive far faster than Ryo’s films.  What is sorta intersting, in observing my above films, is that it does sorta seem that the steady state solution does get close to the point when all the flims have the same conductivity.  Not quite, but close.  

I should also add that I don’t want to go much higher than 900V, as we can’t apply much more than that anyway.

Lets do huge switching ratio for blue light (I also changed bottom oxide to more conductive, top to less)

Dark (V = 900)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/38F7B908-2D4F-467D-AC57-4DCB839E3E61_2/tIO0PWxNDwDRauZML9IB8kElePNlwMPDcmqa01Fhajkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/6E19C306-B2EB-45C9-AE63-EEA75BDEDB92_2/w3vMTZQXqx80nmZjAQqTNAsnJpn0dTlx895ZCxmmuM4z/Image.png)

Semi-bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/C8C5CB8A-58F4-45B4-B7E0-FB5D3431FAC2_2/s7pyW8vetkqItmRhsWlJ5ZExr0lKTo6iyYxvrSpA5Z8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/78517CD0-44E4-4764-A6C0-B79A74176BA8_2/NZ7e4xI1ZkyqBw1OT2YlqOeoVGcG2kOr4ZFbr3Wqu14z/Image.png)

Very-Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/FDBD1790-940A-450E-89E1-A237D3C55B89_2/EQW6mwVQLfzIWGF21mceZA27czAQLhHwlBkkiYOAPSYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/855D2D60-84DA-47D1-9F64-5F149B728DC9_2/KQyYbt4gn238YcWxnrw0eR64D4EmJ7prO8gy7RJ3SEMz/Image.png)

To get 100 v/um of switching, we need a very conductive core in bright (huge switching).  It is also interesting that, as we work at higher voltage, the speed of the device increases.  Time constant is not as issue, as we are working in a regime where the fields make the conductivities high.

At the beginning of this exploration, we were able to get almost 100 V/um of switching.  Why is this.  I think the key is the correct operating voltage (higher may not always be better)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/27715A0B-580B-40DF-A9D5-58C0F6B2055B_2/NUadNosf4YDKQ94vgBx1xYglGmivh2L4cOUjy2TSAnIz/Image.png)

Also, after doing the simulation, I was curious to see what the final conductivities were.  They are not matched, so I can’t quite use that to predict stuff.  It really does seem like we must just solve the differential equation. Lets go back to that configuration

Bright operating 900 V

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/74037DF2-470C-41BA-8F1E-E717F5078763_2/KAp12EPfRtPwHAyI38iQ1aDiYvWQDV6SEpj5M8I2FS8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/4DBD0989-7962-4A9D-9C4D-41EF130E814A_2/6yD7RYhLy4yK8ZCet2bEMOQ5xHqPw5seeg28U3aVIRoz/Image.png)

Dark

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/F7906B62-AC4C-4A85-BD7A-5434D393B91D_2/NwGpAPWf4mSePyX6cSkJaOED7Muw21dxLEJpCxG43hQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/422A7E2A-B463-4CCC-888F-8D52C1B44866_2/cstO9bP4gxgTausfbGyqrSq8oIRq8vxkr6UMJ3y4I8Ez/Image.png)

Switching of about 55. Lets just start scanning around the operating voltages.

Dark (800 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/142B8976-74E4-4E4F-BD5E-1CB2AE368FF1_2/j6BcRTAJNebRjvNhqq2AYpbtI4thxKu0FP9rLiXu4G0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/C654C9EC-A9EB-4633-AB7C-B42C1861661A_2/L94uTstVtCmTLySVJ9vdHQLHnaiueRTgx8PIGesXtdUz/Image.png)

Bright 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/CBDB4627-B5CB-4CB0-B07E-F694CE23138A_2/zlxtpPmtdO0HNyMHz9KZnYlNTUnyLyy8d8eCaLVLGmQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/798B2199-19A1-4C63-ABFE-639620B45D70_2/6tGT8q4sW0qfhcvIZz8WN83eNYl38XsK6CMa3y3JWXUz/Image.png)

About the same switching

Dark (700 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/797F8FB4-EBE2-4EB1-8C4F-7CD39874325C_2/14KcufgsyqrJDbOe39Jyu1oC4Lct69CbzT7kbySGa6Iz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/BA82BFC3-3E81-4BD8-B4D4-BE17650C975D_2/mvh8lKQxxWZ0xJumtAVLLNalFYEB5OT0BUzgtDXyt7wz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/CDC0B967-FE87-4976-ABDE-0920BD0DE697_2/bUDvnWF639PldZYIyR3c4NHxyqYQHbbbsuUfDBZM3VAz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/03CB7911-D5AA-46F5-9ED3-EA870FC6A9E2_2/2Jtxzothp7B90OHbLv0yTwKFEguMIx2cGBeNT5MAtx0z/Image.png)

Bright (600 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/5DD96D29-5906-4DA4-8BBF-C0BCCA57228C_2/iuHy3KSINLHq7KJXz3c9jnppSbRvjF5dzDIyFvtiyIcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/D20C973F-92E2-4DBD-94B0-E6CC75E196A8_2/85NJQIFsxqqYJ2YUG52Y1znKAaRLl4vSpa1byrMtPNIz/Image.png)

Dark

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/FD2E6474-6453-4FC0-A844-CCDE4D1BBFE0_2/WRX4exVdFga0bg0cZkxm6ambdI97FTz8xPmQNTiwPQYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/EB855E59-5D81-48C7-9079-29B25FEF1771_2/wMePNsMiCxi9jGxgEWaMTx8s0RxvnWp0RvFLxaMYbQYz/Image.png)

Dark (500V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/097B642C-ED1F-4E24-A81A-BD548B277B7E_2/NCCNKUJSNePMTquDDdcKgILWMKJpwRChSW1ybQ7iU4Mz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/2B5A0B29-5D56-4DCF-82E6-532858D0DEC5_2/VTODxyRm06OKvxGADUX6x2t5TSUBMEkpXc9KS2DF3g8z/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/42B2F3EF-E9FF-41D6-9918-0BF231389F34_2/AyexqNiePjeDn2DeTBaCyCEN4ZFpk8foMioSUBt138Uz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/D402CD9F-3D60-4222-BEFE-3BD75F175F82_2/L4DgwaEcDXMi4bbF1Agu3IgZhmUWa9xMDo3fTzEniicz/Image.png)

Notice, this was the first stack where Bright state SRN went down from capacitor value.  Raw contrast is no better though.  Do notice how using higher voltage does get us a faster device.  So any concerns about device speed were misplaced.

Dark (400V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/007FF29F-A4F9-4530-8D39-3696B1850984_2/DDGah2EtGzGqJbPACo5mffJygKR6KFahoNDXIo8jzPUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/D704B618-20ED-4449-8C76-6D46306D0AC5_2/XHeNsc22Hj605YlbKcpShVIwKxYiDKoCTcyz0BGAJjsz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/31A19B22-6611-4AA9-8B08-ABD762E33BDB_2/ObcR7LwVGC8OGLzqo4fJw2G0hgzhpxYnBtx5GQGIGxkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/4F02337C-E0C4-439A-A1D2-3B83D578D9B1_2/2Jaj4szPNUOvYHW2WFY6ADDmLJRHL4iXAwK9cZtxTyUz/Image.png)

From this scan, I rule out the idea that lower voltage could lead to better contrast.  We should just use higher voltage because it is faster.  Before, we used claddings that were thicker.  The advnatge of that is the field in claddings can be less, meaning they might not get as conductive.  Lets try some devices with thicker claddings (which is ironic, as we really don’t want that in a normal device)

Dark (2um claddings, 900 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/74F28894-A32C-4254-8527-D7AC4EEB7F51_2/guQ7VrAmcyC8tyjrgHPq9IyHrUQPghqOBxZy27whaowz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/10B4999A-57B4-452C-905D-E80ED1E036C1_2/plaTaBHhZY52EzXjyBt9nzUycZvXPtzbxNV8RpiWvoIz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/CD86CE5C-A06B-44E1-AD19-DB081F1C7FC3_2/Ri9Hu2c4kndEGNFeqUNApfevBjRmdc7Nk6732yshzfkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/1EFC12E7-1139-469D-863C-93E8F8A61E8E_2/Ux7nJCoKZAVAWyEi7YJqE1clg62ruRqBigO2MOSTxg4z/Image.png)

That’s more like it.  

Dark (3um claddings, 900 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/AE4209FE-8952-43AE-A6E3-C3E2B7523CE9_2/yqy48hqeKPV6Qkefa2E6Nz4OLXIrFc6VPhisC8Uss7Qz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/0E2ED496-9260-4B31-A608-9E77482D9F09_2/v44JdctxQYPSTf0ZAg7hsEKw1BAdDI3fsZynkYuCrocz/Image.png)

Bright (3um claddings)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/E88DD0C6-AEC0-4622-BC75-0BFF37EE6A71_2/dUM6Mpz6edx9q8l9MBuymg0QVSGdRB9x0MQ3YWp1CoUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/2650C57A-9821-4CC4-B474-FF9B29A602B8_2/pkixjmJwYZxP2WhHmRKNOcvoykfAddyyckpuOywpP5sz/Image.png)

This is still sorta stuck around 90 V/um of contrast.  If we upped the voltage, it might be better, but we also can’t get a lot more voltage out of the setup

Dark (4um claddings, 1800 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/6798796A-3055-408C-BFD0-5832C1349374_2/AQgsCyw8Qeiuk8ZtMojd21foJEXIbDKToCApAlJasWcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/3FB09C76-39B7-4DBC-A70A-DEDBA046979B_2/6v9aE63WfIzIWDtPivLvfW0Bicq1JjXHfzIQfewD1TAz/Image.png)

Bright (same as above)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/6523FBF5-E402-48B8-9B3E-8102C067C644_2/onx0NwYYTx5rjN872nEqbymdyMd2ZexjIhCLP9nAmxsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/2CC9AF5D-AB00-4DAF-95F2-4BA8A9035E8A_2/erxoTHEmtCtzwgdvz0TZ4nbE6gZYuK9Mi7mmZ52kNx4z/Image.png)

So ya, contrast is a tonne better when we have much thicker claddings and more applied voltage.  The issue is this device is juse not practical.  Lets try thinning the core a bit and seeing what happens

Dark (4um claddings, 1um core, 1800V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/06F477A9-F872-4C3D-BC93-4E534702D40F_2/gCu3Ys21CgwTo7yRzgvLlWcPxWPhT5YsnSxSuxIVzSIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/F30C954D-7637-43C5-8B95-5A5A950C35F4_2/3JbdrR7Aymp6XF68vpxbci0dOXeayf10yldFtYO9avYz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/1D0E6FA9-83A3-4F66-8B94-976B7845EFF3_2/940Tr0M0olLCq9uJjyjYIJhYcBbDaPeSrafG4PwA0tcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/64A58A1D-4E23-4FEF-801E-1757CAEB8DCF_2/hWjY2r9tnKibj0nPwimpxzTJp6nJRHSKff7xlTgMqx0z/Image.png)

Pretty dramatic improvement.  Lets bring voltage back down to 900 V, as 1800 V is insane

Dark (1um core, 4um clad, 900V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/499E020D-264C-4835-8C42-17E3569E4151_2/Mb8REHpuH85xE8qwXtKxvKHFbcnjfd67Hx9uFQ4mpZQz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/5ED51E0E-9143-4FB1-B40F-30FDA5CF0D24_2/zFFpemlRXKYTsyZ31dzm9M6j9YINxnOoUCLxMDOX1mAz/Image.png)

Bright (1um core, 4um clad, 900 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/447C2405-AA9D-4D3B-A2EC-E3F2E4889BBC_2/cr8OhTNlVw7dZCyMmcmktYnncUgx6MylORU7XA271Woz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/6C8418BB-1997-484F-A7BC-8C38BC0B3FA3_2/HLEf4ZlZyflxXWHDTWu0blxm5mwyxCK5QIeFz3kZuQ8z/Image.png)

Right, contrast is still really good (best we get at 900V).  But using higher voltage is also better.  The key here, again, is we want as thin of a device as possible where the core is much thinner than the claddings.  I should mention that the field in the claddings does not change a tonne.  So we could not use this in the delta_waveguide situation.

Dark (2um claddings, 1um core, 900 V)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/16D6159D-C09E-4722-984F-61CE1BFED3B5_2/y0uSn3Fohu069oqWYglRC7hvTGkm1J0pJ2R6eBIcxdYz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/909C6771-DAC3-48D4-8BCD-F4569266EEA1_2/1qokDmkU2UUDsKWJHJzRrSSut1AXaWgTIsqDkwjTqtoz/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/1A9EC200-5006-4C49-9FE8-A4E277DE25C4_2/6cijLaZJ3ClmyRcfO8MyyjaFysimLsyg7vxG7Bx9rm8z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/4884CEA8-037A-453B-B50F-E2C1F6A9B137_2/qDim1BmpalLyrskzzjTC71mxXfyBdnnvMQwpQJiwttIz/Image.png)

Field in claddings does not change much.  We now get 130 V/um of switching.  If we used higher voltage, it would be higher.

Dark (Voltage = 1800, core = 1um, clad = 2um)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/38ACD8F4-6101-4F6A-B1A8-847F57C74CA5_2/PUYsHmk6bGXPiwkqrz6N35ae8ykdz5T5reBD0buzJCcz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/902661C2-663F-480F-A10D-61904EA69495_2/ZziU6O83jtpAR3QdMQaUTeddw2LeEXWyCtTLjnTphV4z/Image.png)

Bright

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/A53F37BE-DA40-4F40-AFAB-543C547C3477_2/PGxRULEyMfi4xCxJDJxHueOAz0xzldZkV97xHxp32l0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/41F53722-8075-48E4-87F9-19DC380D8B54/87BDECC5-CD7E-466A-8E73-75229F83C57B_2/xYlUiaQNNZrtxgYjuEG0gvk1lXzkwIhi8FTgyDspmYwz/Image.png)

Interesting, so besides reasons of time-constant, operating voltage can be hit miss.  There seems to be a point where the amount of field-contrast we get saturates.  I have a hard time telling when that is.

Ryo gave me a few more device contraints.  We can apply up to 2kV to the stack (though I would probably cap it at 1500 V just to be sure).  He would really like us to use at highest SiH4 = 4.  From my simulations, I honestly think we could even use SiH4 = 3.  We would already have thicker claddings for device performance, so longer evascent tails is not a huge deal.  This will mean that we will need a crazy thick core, but at some point, oh well.  The main drawback of this device is we will need to operate at higher voltages.  Time constant stuff is kinda dealt with by the fact that the claddings will become more conductive with more field.

So lets do a scan of effective index, pick a core, and the adjust claddings and votlage to make stuff work.