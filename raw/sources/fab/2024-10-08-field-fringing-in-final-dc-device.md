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

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-001.png)

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-002.png)

After doing a quick Poole_Frenkle fit, I got

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-003.png)

Use those conductivities and the fact that I applied 460 V

Below is the geometry of our product

Software: Ansys Maxwell

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-004.png)

I now adjusted the conductivities and permitivities accordingly per my above calculations

Period of 10

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-005.png)

Period of 7

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-006.png)

Period of 4

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-007.png)

Period of 1.5

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-008.png)

Period of 0.6

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-009.png)

Now the other direction

Period of 13

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-010.png)

Period of 16

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-011.png)

Period of 18.5

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-012.png)

Period of 19.4 

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-013.png)

Results:

Top:

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-014.png)

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-015.png)

We have resolution up to almost 1um!!!

Middle:

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-016.png)

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-017.png)

Bottom:

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-018.png)

![Image.png](../../assets/fab/2024-10-08-field-fringing-in-final-dc-device-019.png)

There does not seem to be a huge bias on the direction of the duty cycle.  We probably have peak contrast around 5um resolution, but we can go a bit lower