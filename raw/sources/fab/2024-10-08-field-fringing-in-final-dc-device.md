---
type: craft-export
title: "2024-10-08 field fringing in final dc device"
craft_document_id: C842F988-0591-44F5-AA5E-157A29A810EC
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-10-08 field fringing in final dc device
[`Tatsuhiro Onodera`](craftdocs://users?id=f29d5eb2-0053-2367-3d34-105e91d4189e) looked over this in detail

To answer Hiro’s question, I am going to do a quick simulation using some existing infrastructure to see how the fields fridge in my final DC device (and prove that we will not have any issues with voltage divider splitting).  

Below are the transient parameters I used to derive my fields.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/0515954F-EC73-47EC-A4A8-A7F308C3EC42_2/dMisuKKy0O4Du8W1vSe3yoSgPmQSYPWNTIMm1LbO2W4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/05C1285A-658D-481E-8AC1-71D381C22AFE_2/ckYTRU2qxkVsgYB3aUx7CN0tsFsnCjKj7SVck7bVdyEz/Image.png)

After doing a quick Poole_Frenkle fit, I got

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/32967FDF-C73F-43E0-9FA5-F546A94C23C0_2/IfYuowWdAcu3Vs7rzGWyUm8OxDoC5x6EAxBaiwIO7wEz/Image.png)

Use those conductivities and the fact that I applied 460 V

Below is the geometry of our product

Software: Ansys Maxwell

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/386BE600-3859-49DC-A06D-D093F3A85AE3_2/rpwfBeyvYTOxZbI4ZIe3Q5AFGP4XWqF3vjuNHp9l0Coz/Image.png)

I now adjusted the conductivities and permitivities accordingly per my above calculations

Period of 10

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/D2A23B1A-19A6-4FBD-A975-331244333FDF_2/C3x6UgNsr0KRWUZNFTnlmNFWRWBpYSO8PiglOfxY1ngz/Image.png)

Period of 7

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/A0166540-F44E-4177-82CD-27C7085F92B7_2/cRbdtRfUFANBsPQ597ShTCbi9nTQhCogIlW6eP9BLSEz/Image.png)

Period of 4

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/99E77850-CA3F-45C5-921C-D89D2830978B_2/GGNeBmj2X9Nt7LAUMYGkKmKNU856Lpry0N8UIOgxqO8z/Image.png)

Period of 1.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/9E7E3990-FC38-4629-A3BA-067827C8D0DF_2/8rRRup1OoUXNfCVbsdkxQtM4t9OybTptojeekpRB410z/Image.png)

Period of 0.6

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/A81068CA-074B-4D09-9494-9CF954794EC4_2/2hSYfKUw2dBlMgyrOFNwIC7A6N7R8BBL9jPn9QAxdo0z/Image.png)

Now the other direction

Period of 13

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/99FE79AF-3E5B-4EDC-9A2E-83C11D98FBDC_2/iyFeFXJjuHfj7fFbJxeBaqareyduyth055HtgliNn7Qz/Image.png)

Period of 16

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/D39915D0-F068-4F37-AC89-78526A94E6DA_2/OtCWZ8pb0QZH0s8c9Ou6MuPqhZDhTYfhwCC3mIdLqigz/Image.png)

Period of 18.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/3B866BE1-3DF5-4118-84ED-8E6FA3A4C546_2/vzseMFxfjvuf92CRISZhGPxK74Jbg5gb3cjBRqg1AGoz/Image.png)

Period of 19.4 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/63A0FE80-BA83-4E17-881E-D3AF1FAF629E_2/yWhjS6o7U7UJZoSJnDwoglcgzbtOwWIG5RKyrbmP1ksz/Image.png)

Results:

Top:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/BBC6FE7E-9792-4808-A347-3D004AD84F8C_2/wcRuKvmTNvqlNIAHSXxsTdAQHF3ZQP3gDBun72VkZlkz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/7451CE6B-6481-42EF-A0F5-2651BD502B15_2/GyqvwWzcBmkrUrLe3nW9XaXyg5GQrLqUFtVpnggxjygz/Image.png)

We have resolution up to almost 1um!!!

Middle:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/773C950E-7F74-4FC0-8197-EBC0EEDA8259_2/NTgiAFQKgk18jVsmJCaoxkjCyLZGyf6FIQctK3jLSygz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/3184846D-5792-4A6D-89A6-D349DA5D9AE8_2/QPOnC9A4zzyRteyB61ZcTRTeREAfTiEfLNIHuzhbmVoz/Image.png)

Bottom:

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/3237CB9E-AF0B-4430-9A1C-94F6BE5FA5CB_2/1RPxtcQm8M2JsyEaZniqP2i1ap5xRgBh1j9Ov9KZJQUz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/C842F988-0591-44F5-AA5E-157A29A810EC/16B7BD11-DFB1-4666-A582-607B58B042A1_2/lXy2b0ce9myK6xuJrx1RAtIc76B5JsYJy99t7olEN6Ez/Image.png)

There does not seem to be a huge bias on the direction of the duty cycle.  We probably have peak contrast around 5um resolution, but we can go a bit lower