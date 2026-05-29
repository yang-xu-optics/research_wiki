---
type: craft-export
title: "2025-05-23 asml fabrication pass 2"
craft_document_id: 4CB064B0-38AE-44EF-A3E8-434F531BEEAD
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-05-23 asml fabrication pass 2
In our first ASML fabrication run, we seem to have broke our waveguides.  There are two likely explainations:

1. We did not remove ARC when removing edge bead, which means that we contaminated the wafer during the BOE dip
2. We annealed with Takachi oxide, which can’t handle higher tempuratures

Today, we will try to rectify these issues.  I will make new wafers, and be more systematic about testing loss as we go.  We will follow the same proceedure as before, which is:

1. RCA clean
2. 500 nm of pad oxide with 3 mins smooth deposition
3. Cr sputtering for 1210 seconds at 7 mTorr
4. ASML with existing recipe, dose 15 mJ/cm2, arc and 600 nm of DUV resist.  Develop and coat using gamma.  Make sure to use edge removal
5. Descum for 1:45.  
6. Cr hard mask etch for 3.5 mins
7. Oxford 100 CHF3/O2/N2 etch for 7 mins with 5 min season
8. 20 min Cr mask removal and 15 seconds BOE dip
9. 9+8 min smooth oxide deposition (in seperate steps)
10. 12.5 oxide thinning using CHF3/O2 recipe.

Below is Oscar’s recommendation for ARC removal

![Image.png](../../assets/fab/2025-05-23-asml-fabrication-pass-2-001.jpg)

We can even use 2 mins.  

### Mask prep

Just finished RCA clean

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-002.jpg)

Before season (Jeremy cleaned when he was fixing tool)

![Photo from Library.jpeg](../../assets/fab/2025-05-23-asml-fabrication-pass-2-003.jpg)

During season (we changed to smooth deposition becayse we hope this will slightly reduce roughness

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/CF0E7158-85AA-4C9E-86BB-BB82063C50E4_2/EQtG5gyaJCNIxnklU2S9Omx7FMP0DWMJA9Hh0ydEdDwz/Photo%20from%20Library.jpeg)

Before deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/746EBD83-D56A-4AA0-8FD6-062DAA6A0849_2/LODb79Amd5FR5EndGxyhMx3fRVsi0xlq8AO3Inx7HNsz/Photo%20from%20Library.jpeg)

During deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/5519A470-BD81-434E-890E-EE285A941858_2/8CtN5X0C2TUXUxLnnWAPDmZ8mx9z0tYqmavWlAv87jwz/Photo%20from%20Library.jpeg)

Before second deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/EC47570D-4FAC-4660-A0B0-D5EC17CC7091_2/q98Ph9lNXx3NUiVVAS6QDyviFyN7S6vAotAxWi6y4tgz/Photo%20from%20Library.jpeg)

During second deposition 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/2B420DF3-2DF1-4ABD-9D4F-23A2618A2632_2/JpC4nln0rQAVFJygnjrGizpjhENO5QDHV3ZyuqMqkisz/Photo%20from%20Library.jpeg)

During sputter 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/78A916BA-96F9-4EB2-A94B-E942A2825E3A_2/ZMsq4sHNbJau7YAVakfGVUHoVk59TJSGvOp494IyQcIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/FE05DC10-12B0-4E16-AD43-21D67B2E86A2_2/b6fU2woTE7WRoxS2m1fpNIz6YTGcNHuTDIwYQPbfoD8z/Photo%20from%20Library.jpeg)

During sputter two

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/B252973D-C060-4038-8C27-FA6A5F317AE8_2/7LwytaaGwSI0OIJ9ElaxbyI3Iji0aD49ALuH7hQge4Ez/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/B58E63E7-73C2-427E-84EC-75BFD925A543_2/L5nTQkh43epag4zeWc3NMrgxOU1bgll22jgxjP8VZp4z/Photo%20from%20Library.jpeg)

# Resist coating

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/969EFB17-94DE-4252-86F2-715DFAE47A55_2/JYtpfuqFpBiPwnClwhP6Yom1NqTC0tCec1JwixOPowIz/Photo%20from%20Library.jpeg)

Dummy in slot 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/455E9C4C-9B9E-4BA5-8602-A0119789342B_2/B4ZfuwhcG0rX9rmmJ36k3pj9LFl94MB5UnnporHwmhkz/Photo%20from%20Library.jpeg)

We do ARC first

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/7BA67805-75F8-47CA-91AE-73DC520FA4ED_2/rxigQc5XEKx8S1Ei7FLFNLbZ2I6mnxvFiwvIwPujxyIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/E21008C9-6152-483A-ACC8-EBE735BC3659_2/x8Q7Jv8xlkwYwvYhnwiLyBNI4YcF3bb4PxoV0fJC3HEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/96B92A59-C7BE-4488-B6BC-1063C4525FBA_2/luvgbQNsuHfDJtLOcghnyfzrHgcJUoXyxYAKnlJoYbkz/Photo%20from%20Library.jpeg)

Noting N2 is on

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/AD527782-6B9C-46DD-874D-EB4916E1F779_2/D6sD6Rj5Td7U1oB3q80yW76eyD9fQDbSAxxvBivCbloz/Photo%20from%20Library.jpeg)

ARC coating started

Now PR coating 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/02475FDF-54E9-469F-BAF1-006BAC02A5F0_2/8SXiZF5yomte3OPLQcvNxlkFH1vJGJevzBpJu0c9TRAz/Photo%20from%20Library.jpeg)

Start sequence now

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/A57AEFD6-33BD-4521-89EB-4FCE54B3B567_2/heK77hQdxarJmWxeTapI77Mqw701ypnA00N1kvDBuokz/Photo%20from%20Library.jpeg)

Finished.

Turning off the N2



### ASML

Read the mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/E70E424C-2C74-404A-BABB-EE7F8E861EB7_2/kxmKKZDcjm40eTDZbKAoVIqTSaTcaoKmwIU6W1KG1Wkz/Photo%20from%20Library.jpeg)

First, we run edge clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/028B2BDE-B0D0-4C87-AB54-6F054C321298_2/8hyvNJN6HeFPn7Jk7EsmeSWrxsRXWwgWyQNtykkesjEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/8BA5A67A-D8CF-428D-B317-42F60D523405_2/MJ98rPuFndJtHVvhiXSSx00PYRKnTJAdfGDsZFTd9GYz/Photo%20from%20Library.jpeg)

During first run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/4DB402C6-A72F-4A5A-B557-BB832F98003B_2/UgbqDzlGfc89bSTyowvKxx8P4uALHPtE8dnUzPkEvbkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/A7AA3DBE-0D3D-4F9F-9DB3-6FDD3445818B_2/A7WsqL9Mb3q9Y3dTfqE8DuvxNBPbKYaa7HFsInAKhVYz/Photo%20from%20Library.jpeg)

Before main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/06CC0BBF-2BAE-44CF-A659-33F6C652658A_2/8jxJ66DHbbrNl8NDZM3gXSir9nddx1xeWXy6Y3968MEz/Photo%20from%20Library.jpeg)

During main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/8E325DAB-BFA0-400D-9EC1-00F233AB43BC_2/naktO1olvV9NpEhKqAsOPTyKX9Q2WmSqKcDZTpLXgjgz/Photo%20from%20Library.jpeg)

# Development 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0DF180D0-3A64-4316-A087-105505931C32_2/C6Xj224vxKt9rbHM1yheLbIhZIWCagbPakpnxPZ2Oxgz/Photo%20from%20Library.jpeg)

Turning N2 on

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/2774D7E3-B4D8-421F-9B13-F9F7E99B5184_2/yZo3QRlyjhsdAChyczZWW9wK9gYs86JGtu8FgUiQwBAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/4226E6B6-980C-4297-83E9-2A835F1AB505_2/LhBzOoSn9WlTk620VEBEm4eUNtQYeyGkylO5THSxwbkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/7373E17E-740F-42EE-B591-755643A98172_2/LiWCzJY591s00uP8KPdONIEqFHWF9krhzjzvi6WaukEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/7FFFE937-EE2F-4CC4-8023-1D44AC3C0C7C_2/qwTCtOS8h6Wfu12Tm5qJqBZpWMUARFg0CCNOWRofQv0z/Photo%20from%20Library.jpeg)

After development, no edge bead

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/1821A7A0-2F2C-4000-8742-23F97475BA90_2/Vw4yBojSvG178jbPTeJpq6tlCRkSPbviykbuPqUB9e0z/Photo%20from%20Library.jpeg)

### Etching

82 pre clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/4A1EACA3-57FE-4274-A691-3208CCF5DC79_2/uDBHBLMSPbzHUnlNi15RIAxJfRfgSJXylAjFlOAIhaEz/Photo%20from%20Library.jpeg)

100 pre clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/349DF25C-A2FA-48F1-A88B-38BCA08A347C_2/YTCOIViFGzPmnnfBxOEXY9IIkyYHvqk0AIgfrkLCq7sz/Photo%20from%20Library.jpeg)

We will descum for 2 mins just to be safe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/44F724C2-A7ED-492D-97B4-EA82FD9401EE_2/RUQLsJZYZb1z85oLaQAYOJ7l0RNwW1LYWytci57wt00z/Photo%20from%20Library.jpeg)

Before 100 season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/4BDB7602-EC58-40A3-989E-C0EC959C75E7_2/uxZu6fUnbDxExXmHs124MDaGA9kTAo7m9l1JmBlRDUgz/Photo%20from%20Library.jpeg)

Inspection after descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/D327F546-71B7-47AD-A113-8779B419D0D9_2/JuDzT4WwhVfTtz0aIXjqE2z2m2JmmYTxK4GIKwGJg5Qz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/AE73474E-B056-449A-8566-4B075F0AFA22_2/NLLnbfU15U0rP2hLfPxb6SZqVhsYAEhnm5MlzovrijYz/Photo%20from%20Library.jpeg)

After Cr etch



![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/C315D350-367E-423D-A69B-5EFC3BD8C29D_2/Eva0T3yCBlOHixEt6sXjH2JBI1DTZx3tF4rlGHLZtNoz/Photo%20from%20Library.jpeg)

Before etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/2FBB36A5-31FD-4F37-9777-675C060878F1_2/oIXlv24G2VvoUIaJMxY1YHUriXFfABJEacCETC6Rd84z/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/E3C9961B-5EE2-4C91-9E45-2494E6EEED89_2/46j0nGr0PLVTDG5h0JEOvzxhjFHlMDQRr6xdWHh1mXYz/Photo%20from%20Library.jpeg)

Depth after etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/B1B46D83-9B8A-4E63-B4DF-9ACA1B6D31FE_2/raSjFFVgFyqkQVKyW7TH6ugFNMSbF2qp3gG1DO3XcBYz/Photo%20from%20Library.jpeg)

After Cr strip, I do some Ellipsometer

In trench

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/15FDC270-9FA5-4157-95BC-8257F01402FD_2/wYZWVYhYrvQms3BA4inxpX0RG1j0m11OlNz0icrSriQz/Photo%20from%20Library.jpeg)

With mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/3661C976-6C29-4E8C-A322-976B1A4914DE_2/N4C1M4ErJDfUKtSb4qWuSZQEyxF2HYie9MbMLdetg1gz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/D82729AE-3DD2-41C5-9CC7-CB1D605FC0EB_2/7fl2Fxu32k0Rc7rZyR0FoAiTeTZTmR9QhVR35Dd6tu0z/Photo%20from%20Library.jpeg)

# PECVD

## Seasoning 1 min

Seasoning smooth oxide recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/B590BFC1-DB71-44D3-A782-7ADDCC0D369D_2/Z8iZqdMSe3o7Wmsr2ojgvZUiJx25NFqezpW5aCoLpvAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/6415FD5F-D03D-42A1-8A9C-A397B7608AE1_2/RswGA1LeX0B2lt6CFPmXIscmSNSVkxhT4Ur99z4G7Fsz/Photo%20from%20Library.jpeg)

Last user cleaned it well.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/6589057F-FF10-46DF-96D6-2CABF3094D96_2/wdVgRbZb6MeymULP77JbCjkcU2U7YZ9TFfAy4CWWBGEz/Photo%20from%20Library.jpeg)

19:50 Starting.

19:59 Finished

## Main run 9 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/5B96F8CE-9921-48A7-9C07-66CEC3C11B0A_2/nHOpIjw58VzOdtMpwpCCdyZc4ly9y4GoqaQDWg6xOYgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/ACB53AB7-43F1-4427-9870-F77242CBE621_2/KGIsuDF2T1PTTWrKtPREuLPHxyHXT9vumIUe7ESvrSkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0FA591D0-EE4F-4C90-AB76-F2EA0E854529_2/GROS9rD7HcLyylcbczJyWJI3bwicKXG3FLddgydGE6Uz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/83C45B23-A1C1-44DB-9C7A-56735FD1FF99_2/11IqID8MFIoeMlt449Pu6tRMxB2enwIA2ddLLTu5rqwz/Photo%20from%20Library.jpeg)

20:02 Loading the wafer.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/C9AEFD1A-FFB7-4DB9-81AC-716D8A9E1CC8_2/29B0ESSGwEODy9AcUYEwuyLxwtzpFDE1Rl7WkE7bkTQz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/A29A74E6-E566-439D-834A-7ED9D9E483CB_2/uS2QuXb9eZ0p85KhZB3y7Myaz27Gmm89DxKdEj3VVcEz/Photo%20from%20Library.jpeg)

We got 1.5 um, to be expected

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/3671E9A3-C6D3-431C-805A-E472DCB694BB_2/Rlb37RMztcGzGasedof3Mp9Xdqs1O3pdgBrB5xXfMZAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/B6C56BBE-65BD-4492-A590-BB12E2A6EAA6_2/I2hAmFbdGWzTagK64uxKGx5vzXzVdTWcobiBdWKxclEz/Photo%20from%20Library.jpeg)

## Cleaning 10 mins

Clean done

## Seasoning 2 1 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/92C2C33B-4EEC-46B6-8FEE-7005C31FE0CF_2/JpP4ecPWAEKdfLOJvnJOKono1cQNxaQCv43efnoavxQz/Photo%20from%20Library.jpeg)

## Main run 2 8 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/2734CDEE-831D-45D9-9722-6CFC9D933AAE_2/1vQB5T9XmMR7PQRfSyCLMDBXBaHvsf7gqVUdUw0mObsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0CA268CE-F209-49FA-B4F5-8B2B64EFE72D_2/Z7DdbuGGTFPFZtTdxT8ywvi9SZqQpBUs2VqV0TeBumYz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/22D4076A-E0B5-4478-B2A1-BAB57D4BF762_2/Hm7Pjpv2ix9oHXC7wK7GLrpN6K86SF54eECowwoTOscz/Photo%20from%20Library.jpeg)

### Oxford 100 thinning

We expect 3.4 um of oxide at the end.  So we want to etch down 2.4 um.  This means etching for 14 mins.  For square spiral, we etched for 14 mins, and started with 3.2 (we used a different pad oxide).  Lets see the final, but plan for 14.  

Before season (I already left chamber clean).  I season for 2 mins.  

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/8F7DFF09-0EAF-4094-B3A4-BD9BE78C20FD_2/KnQurTy4VtyDzdDpvpPfPHT2iELNyseAZhIh7gvjGEUz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/A32FF839-EA4E-496E-B273-4A1F9122F643_2/JOpK50sGh9POMvQ3pemQzYOEMPzgud4PVyo5E6ptHwoz/Photo%20from%20Library.jpeg)

We will do 13.5 to be extra cautious 

Before

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/CA4F06C6-86E8-40E4-86FB-8C679BC9F287_2/AAHuNDgVarX1u7vJEj0Eg9IZFPzqTixg6pua1FYRFpQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/5707EDC8-9A07-46D8-95CF-F80532395AA0_2/IJV4DXSgMQqxGwU6dePY7cCOLTqQgdMJOsvsEBz1pSQz/Photo%20from%20Library.jpeg)

Almost spot on thickness

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/21290469-FCB2-4F58-A9D8-BF90748E4691_2/YCNjgIzMy4aqKusko3wlpx4CGtSkHOW4OHuR9eQCieIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/C0F33C1D-8377-4448-A40D-73FF79D133FC_2/jDm0VxMvxtsPCNLPWIVPK2y9DXAdByAgPZyvhqbU6wYz/Photo%20from%20Library.jpeg)

### Loss test room temp

I used 10 x objective with EDFA. 1570 is the wavelength 

Straight one

3.2 mW for 84 mW in

Straight two

3 mW

Middle square spiral 

120 uW

Middle circle spiral

230 uW 

Looks decent enough. We will try RTA now

### RTA test

I spin cleaned the test wafer

Calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0ACA5B23-C5BC-41AA-B15A-B4B73B57736B_2/xzssiXKLVquyvF5QTizNwwCryWl2JECUv6gmOvrLxc0z/Photo%20from%20Library.jpeg)

During main run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/EBD664BF-C5F2-406D-973E-F7073E416D81_2/6mlwmEdh3uZH7WQhhbdi4ayeO5sfSwpHogL5SRbipb8z/Photo%20from%20Library.jpeg)

Small explosion 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/CC21AE86-D8FF-4B98-B86E-98B7E4D1EC20_2/vKe6njjI520b43ML81ZmHm4pSB5t5MuNOxpGG1ygMUoz/Photo%20from%20Library.jpeg)

### Loss on RTA

Using 10 X objective, Edfa, and 1570

Straight 1

5.3 mW for 94 mW in

Straight 2

5.9 mW

Square medium 

1.6 mW

Circular medium

1.7 mW

Fast adibatic 

6.2 mW

Fast hump

3 mW

Fast hump 2

3.6 mW

So it does seem that having the structures does increase loss, which is a bit unfortunate.

### Main RTA

I cleaved and spin cleaved new pieces

Below is calibration of RTA

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/285E7247-C161-424E-83F9-F72F641B02F6_2/1gTquzKNyBRyERSYfWyy07szHOdPBn3UEgtsxN5xxhgz/Photo%20from%20Library.jpeg)

Main run

Before

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0ADDB4F9-5E7D-47A9-BFCD-4EC43A4E192B_2/JI4hO4h5XPrS7VNQ1xK9MzWqQ6l7jFcqgkBOrGgk7RYz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/008D2902-169C-4E62-AB94-781999169428_2/eOhxzt9QSvBaEZQ1CE9TlxKOZi0E3FQom6qrDqQsmzoz/Photo%20from%20Library.jpeg)

# PECVD for SRN deposition

We start with some pre cleaning, just 5 mins.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/D7B63369-1BBC-473C-AEFC-F0469C0ACB54_2/Fs3ATcncudBfnhBxkBay0p8h5Py2PK1LiPwdEoT3CT0z/Photo%20from%20Library.jpeg)

Previous user.

16:36 Venting

## Pre cleaning: 5 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/C3E383D7-41C5-4216-879C-1741F2551EF4_2/kmrHgF3jiBKGxyavtGlidFkOSo1BvfuQjHqlTdLmVQMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/238C813E-EC93-4BD5-88DA-05E995BF2064_2/bOSxyzvRVx0xwUHIHL82SvcolKWU2QRKlZh2QHc3jRYz/Photo%20from%20Library.jpeg)

16:37 Starting.

16:47 Finished.

## Seasoning 1: 2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/359AA066-6B35-463F-988C-4CFE18EA361A_2/D13Ul19JUM9ky9CLajATtmIeMh7SGPkVVFEPqgIFYh8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/EEC7848C-B5B2-4EC7-AFB2-601105148148_2/RQOe8bL1WE8yoew0HkZUxzuBrqSgKWyJLx64x66mmfQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/692FCAC9-B84D-4AAC-B830-AAA42C9F1C48_2/temMe4J2rvcGvtmf1bSwUJDXfQhFKEvIxbxmcHaY7p0z/Photo%20from%20Library.jpeg)

16:49 Starting

16:55 Finished

The color of the sample looks good.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/1CE27B64-897E-469F-8054-4ED58D61D646_2/ycupuEtAfaxwezrDJz3rETrGy8u3yf70WFTZnVIwNsgz/Photo%20from%20Library.jpeg)

## Main run 1: 32 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/59CD4431-DFD0-46C8-BEAA-2DAD605BC3DA_2/yPR0ytNYNuOZAaB8Wi3ySpq61JUuSAd5InIkpWgcOBUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/A3BF1B6B-62C9-48C4-8B08-0763948988B1_2/vJd6zc74Habx11Vd47rO3OEQ1EPZH6hZAoR6W5vSvTkz/Photo%20from%20Library.jpeg)

17:00 Starting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/341B2319-474B-45E7-8FA8-EBCC9CD00ED0_2/71q4kXkM9BDJRv9PglAeNeceeNRFcpa1yia701UCJM8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/F5E8CB74-E614-4C39-BFD1-644B62223CB2_2/jREBRBVJoNfi9EoOMWNEvTQwxmsDDYyJ7lLUs5aVXooz/Photo%20from%20Library.jpeg)

17:36 Finished

The colors of the samples look good.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0533E87A-C5CA-4281-9DA8-97A26FDFBBC8_2/e9WUpkYxlj6nVTAKq65U4goRHn5PGqPha7TyNLIS7yIz/Photo%20from%20Library.jpeg)

## Cleaning 1: 20 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/71968D6E-681B-4963-8E05-2C1BDC505BF3_2/cyGdbnxS1x6bUFXNghYy0CK25CBPI8vfMymFzeYsjPoz/Photo%20from%20Library.jpeg)

17:39 Starting

18:02 Finished

## Seasoning 2: 2 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/EFFF277F-3094-42C9-BCC3-0DD25BB30762_2/c6I8GvLxB1VKk5CxA8RipQvMxgALOPDvpWwc4fP7Byoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/22596672-9836-4A88-8F54-551288F427D0_2/kSuOvwulPVbyr5mPpAkDDcdboBztNbEGxfMQrw8UunEz/Photo%20from%20Library.jpeg)

18:05 Starting

18:11 Finished

The color of the sample looks okay.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/AD3C463F-E47E-4E49-8684-CA5C7E7B6A55_2/c2yHZffyVoHwxJxHWVxvJ3KbPbZj621T0WU8jLj6L9gz/Photo%20from%20Library.jpeg)

## Main run 2: 32 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/69859817-ECB7-4E9F-9825-D8575B3CA544_2/xePz3jMxECK3gFB0pkGZt17dhZHzqavFuqXjm9LtWTQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/369FC86E-C0EF-4C77-963F-AC210E6EB0C7_2/pQQDLIo0WAJglK64BOYj6lu8InrCVBDlVxM5uxYjspQz/Photo%20from%20Library.jpeg)

18:15 Starting.

18:52 Venting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/810A25AD-38D2-407F-BC60-80F6141A7D9E_2/nBRhUEPN25lSUx9uRQgy1XJZairv7xAT9ZVqxIqTIbYz/Photo%20from%20Library.jpeg)

## Cleaning 2: 20 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/E30AA486-9D4D-4829-9917-F38F1C114C45_2/mtbKBNqjkB59uRyi71LDLJfnY9mUO0q0qkgJ7bdxmUQz/Photo%20from%20Library.jpeg)

18:54 Cleaning started

19:18 Finished.

## Seasoning 3: 2 mins

We load a witness sample,

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/6E230A99-42CD-4799-B577-B6728216ADCF_2/U9BFxGzd4qe4F8abt9SRzy50sHjOVPCr1S7LXky2ZAgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/F96BBABF-6ACF-4DFC-A356-808D6B01AA5D_2/sKsgoHY5JrEeGWyhz3c3xHVYjCPhW7LsU3DxmhTDBMEz/Photo%20from%20Library.jpeg)

19:20 Started.

19:27 Finished. The color looks good.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/5FE12CC4-D5B2-498D-A438-BACFADC5C89E_2/vGCPlAoUje0llB1WUAHqg6ykVn1YsnKol3KDD8WcSDcz/Photo%20from%20Library.jpeg)

## Main run 3: 32 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/ADE82300-FFB9-4E68-B54E-3B2746B0EFBC_2/4FyT38N5ebE1V93xfpEosPHsjfqyFhT3R5RKyO3BmNsz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/0E93CD17-A4CA-40FE-B1D5-ABD028D01A02_2/1ythpdDbuvBJdPxtRqLyle9SckcWK7B0UtszkJGbkZMz/Photo%20from%20Library.jpeg)

19:30 Starting.

20:06 Finished.

20:07 Venting.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/366DABB2-F5BF-4944-BEFE-14AF4F8C3901_2/QqdDEym3OW1OuFCdvAUP7OJltpycxm40ywtiyBsQCyEz/Photo%20from%20Library.jpeg)

## Cleaning 3: 20 mins

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/2CC76CF8-DB1D-4106-A3D4-E267341030F0_2/hCPh0yA1KGxLvIrzwqJxc4md8JOFVrLeKa6nWoafVB0z/Photo%20from%20Library.jpeg)

20:10 starting.

# ITO deposition

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/5FBB858B-D6C1-4406-A78F-92DD5CEF2E5C_2/FbcGYcQd8gC4JNWqUDf8jfiTbq0Y0d24zAcrpDyqxHgz/Photo%20from%20Library.jpeg)

20:39 starting

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/C08FE258-DA11-450B-9A11-42C2AD35AEB5_2/wgHWaxUoon2OcDB49zs2KAbWoeVL569XrWyXDhFbuxkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/3C8F2BF8-4DB1-4812-B045-8F163C211201_2/KJMWYqaInBRK8P0UQMUIjjHyYr2QzXNKHqTPmMxyIpAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/4CB064B0-38AE-44EF-A3E8-434F531BEEAD/FD3C230E-5B56-430E-ACD4-16CDF4024BB7_2/KJFcQFycJR5rgQz7CQHGCb0fU3diFfiGy369DsRgUTwz/Photo%20from%20Library.jpeg)

Try to make waveguides 1.7 long

### Loss sanity check at end

Medium square

1.76 mW (so same as baseline)

