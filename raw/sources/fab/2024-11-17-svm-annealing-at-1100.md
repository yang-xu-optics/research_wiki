---
type: craft-export
title: "2024-11-17 svm annealing at 1100"
craft_document_id: 115E2573-E1D6-464D-AA1A-9E31BBB64B8E
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-11-17 svm annealing at 1100
According to Ryo, it seems that we can anneal SiNx at roughly 1100 C and get rid of N-H bonds.  Below are some excerpts that seem to suggest why we need to go to these tempuratures.

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-001.jpg)

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-002.jpg)

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-003.jpg)

![Image.png](../../assets/fab/2024-11-17-svm-annealing-at-1100-004.jpg)

At some level, I am a bit skeptical of whether we will see a huge loss reduction, because of the thickness of our waveguides.  I just don’t think all the hydrogen will diffuse out.  Then again, we should see some loss reduction.  Moreover, stress might be an issue.  It seems that other people use much thinner waveguides.  It is also not ideal that we don’t have more etched trenches to take the stress cracks either.  The hope basically is that the waveguides don’t crack even if the rest of the film starts to crack.  Our annealing recipe is below

Gas: N2

Load: 300

Ramp: 160 mins (300 → 1100 at 5 C/min)

Anneal: 180 mins (3 hrs at 1100)

Ramp down: A while (Overnight, I will just log off)

According to the CNF website, it seems that the furnace I want to use only goes to 1100 C ([https://www.cnfusers.cornell.edu/node/63](https://www.cnfusers.cornell.edu/node/63)).  We can manually set the tempurature setpoints in the software.

We are going to start by cleaving and wet etching our samples

# Wet etching

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/00372B66-35C5-4B8A-B2A3-66846ED680CB_2/eYyu5YyuQxeeKXimNGCMyLWcOyzYqyxQaLwt67jqyTUz/Photo%20from%20Library.jpeg)

10:12 20 mins Cr etch



# Furnace

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/81BFC568-5CC3-44A1-A783-C1BF07F29E97_2/covDUjN80TxyUPet54EYFqXhnh8ndbwGUd3UXIg5Jhsz/Photo%20from%20Library.jpeg)

We use this tube

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/4F1201D3-4D42-4E4C-A359-7D05E7C3C13A_2/LbG7yqHwRRk04GCd5ws3M2SJNl5wnxkZJhIxdq8RTWwz/Photo%20from%20Library.jpeg)

In files, we open

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/A300F38D-5042-4854-97B6-52472CBF440E_2/xIJqNHePGQy5pRquTNfsNIp4sB2mBi2VaWu1OOpsdiEz/Photo%20from%20Library.jpeg)

Open tube 3

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/B2C07D7C-7786-43AD-8AE3-787ECB8AD803_2/uhDJAWnUJPzZwJVxfymGITxcI1gNAhfOyTksBLcrkNAz/Photo%20from%20Library.jpeg)

Choose recipe. We then change the temperature and time.

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/09C01E5D-4D6E-4417-9359-281D5482EC0A_2/ZSxb1EysMl4M6AXLV8WkuMifxod11VRAQCojmB1EjSMz/Photo%20from%20Library.jpeg)

Unload at 300

Load at 300

Ramp is 1100

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/FF3529B4-E881-4311-93DC-31E67197975A_2/a25gkzM978QWcraMYmiBhjULzjjmDenmePfVO5pqzJ0z/Photo%20from%20Library.jpeg)

Ramp time 160 mins

Anneal 180 mins

Unload at 300

120 mins

Go to files

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/F419B1D0-E4F2-4D4E-B559-B137D495FFA4_2/HU9g6cn9Bz2pE6Z16yxmjMTLnKa43zOdw5hPy84htlMz/Photo%20from%20Library.jpeg)

Hit save

Overwrite the existing recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/D21EE418-B466-4970-B8E0-D818CAF4E43B_2/0O6dMzaqapg73X0PPpxcD75pJEYR9OFJ8s0s1jey7CYz/Photo%20from%20Library.jpeg)

ITS onrhe desktop

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/B9AA2B7F-CCF5-41DE-98D4-9A6D9BE6D060_2/ec7EbgGB9EbkYqjjLZofmsjbROSyoFeAEUWgkDnU9yMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/C8E53842-79A8-4D2C-92C8-251E221E434E_2/y5YNwEduHyheUnJ8ofq8IAxY0yZBTSCtzHnJx69PiBAz/Photo%20from%20Library.jpeg)

Download

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/9E09B7F2-FB22-4CE1-87BA-14B899BA423C_2/OxrRNx0bypMj2pVGOgz1qZ6XyTuoct7MyNpyAuSpVn8z/Photo%20from%20Library.jpeg)

Begin download

Operate

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/FFD14659-1362-4891-9AE7-54A11C782073_2/kKfi1cTB8u53KUfgwNDJ0o9cD6ltr7yLLUO3H4ZQv4Uz/Photo%20from%20Library.jpeg)

Select recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/761602A1-BE05-4C48-91C9-F5791B6665FA_2/NRtLnqxuPlYGO0FxdjBTQEDqfRqafy2rDgYVvEm2prYz/Photo%20from%20Library.jpeg)

Select the recipe

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/19D87169-D04F-49AD-AB9F-7104A2329902_2/VQCsTqvltsON6y1sxZjnmocWGhLmJy58uXJ4adf2xf8z/Photo%20from%20Library.jpeg)

We hit run whenever is ready

10:41 Hitting run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/1243DFED-BE1B-4DE4-B71A-0AEA40CD2617_2/RpICxsfsXS5hvYldAnxyeFoLxRz4EgRXWndnyp8kKsQz/Photo%20from%20Library.jpeg)

We manually unload

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/29A307D7-76F7-438C-A4DD-172FBEF8011E_2/8urDKRyA1hpAgEiLoPyzglpeIAihqalHcrsXM1fkJSoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/6D0668B0-D033-4B39-9C27-6EC4C271EB85_2/SuDQV7pElynlwP1BMc4PoRfZetkKDJhlc7zdltor3j0z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/00300C10-D385-45FC-8713-A3130DA64F90_2/8RgMg1O617y3AxOkzJrOVrsRwmVlxkxNi65nJM0ryXQz/Photo%20from%20Library.jpeg)

Switch to auto mode. 2

Step lets you skip

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/BE4B2F24-8AD8-4D16-9E18-7B7B85CA3B57_2/9HcEN4mYCSeg3lM9WJk7vcGtPSh55y89b2qCoobjySQz/Photo%20from%20Library.jpeg)

Decreasing load speed

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/7EF1B19F-ED60-45FF-9D94-DCF9F180957D_2/zdd4AMJUf2cjDrX3wmz8sCAsYxxU51ghNg6wv9qASesz/Photo%20from%20Library.jpeg)

5 ipm 

After anneal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/B11863EC-1500-40EB-A63D-D8FE3218790B_2/WIAyVN4hyjDaGfWxJ7Mtz46CMNpC3g4gEAtvCebeagIz/Photo%20from%20Library.jpeg)

I then cracked it open and logged off

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/2CC3247A-3B1A-4001-AFCC-82C05CBCE2E4_2/HxIlaBHxAPRHLyXwxyw2Pnr4Y17ih1lId0WwYAyiDwgz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/4B22680A-6BBF-4BA8-9D7D-59C8B8EDD28F_2/A3K59VqD7rwwvSLwNfRYEqBNeHABuystV23ycMFXCg4z/Photo%20from%20Library.jpeg)

It’s hot

It seems to be cooling off

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/99B99A0A-8732-4EF4-AB1F-63AFB7303944_2/cnE67WkikyL69drESir6FQLydDV8SQdtKjyKUoCpBCYz/Photo%20from%20Library.jpeg)

It is dropping a bit fast, but oh well

After 4 hours

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/BEE70CFE-7FCE-4659-B295-947B482078BF_2/947jmZRHQqWxdHiiyfKy8N4eVykV4eMZI5Cef1aVVxMz/Photo%20from%20Library.jpeg)

Now time to unload at 3 inches per minute

During unload

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/0A078C26-AA94-4691-BF06-E8142AA9C80D_2/KQ0rpaXCfXt8ZlgnHLyEXXKNVTQDztyxXIEo4fjmAIoz/Photo%20from%20Library.jpeg)

Image of waveguides

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/7F1A4289-4FE1-4498-91A4-83782E6F1DEE_2/D9b9UnhaKFnFQRYRKYKb65HATHmcauVKT8vPl6RBxQ8z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/74F13134-4818-4418-A87C-E463D2D0A82B_2/rTgPYL89C17Rm8oJXkoQTS3yZyoylpOM1Z90yUByQRAz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/DDF3D5BF-CC61-4E97-BB51-D1AC7C2BDF51_2/fg4G4l2XdpvTdjpfn1mq8B4mfzaLHvIsRTDc2cYvvckz/Photo%20from%20Library.jpeg)

Very close

Other piece

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/708BA97E-4FDA-4771-9712-C132B536523A_2/noAvJt5cCf54D4qIxyysSRlOIE6YX3CZRfFmz9fmIWUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/363C218F-2EE0-4300-81FF-EBE30D367EF9_2/opcq2wYAPzxN7uDiPFRqEx2RnFk2CT5qgqOzUyjvUiMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/23F0F4C8-B958-417C-BF51-D8D3571E782C_2/XkgiwNSLUhkSGrsFshpcxWGHI4WdRYCTEupTiTJG8K4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/4A9C4C30-01BD-4CF4-BCA9-AF2B85ACFFAB_2/lwwSpSzQUxdj3mURg0eHKsuv5qZDPHRD1xcXxeND2GUz/Photo%20from%20Library.jpeg)

Top view

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/D7E6072E-A542-42D2-9BA0-A75287B24C23_2/VVRL8I4fVrzHGXpFQJlyj4MvSNVufQ0tPSuxJfmS5Bsz/Photo%20from%20Library.jpeg)

Observation a couple of days later to see if there is transient solution

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/BB0185B3-29EA-443A-8BF4-538884F3D8B1_2/gyYBDMs7JvfxiLfKWAP7vx9LjNqbQsGufYG9ynqYbzoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/115E2573-E1D6-464D-AA1A-9E31BBB64B8E/60F8F48B-C6EB-48FA-9CA8-363A0004FBD7_2/XA92t30MTLK695lVWPxkspLA7HqNxiv7dh5vk1dBSAMz/Photo%20from%20Library.jpeg)

More of those delamination center than I remember 

But cracks did stop where expected

