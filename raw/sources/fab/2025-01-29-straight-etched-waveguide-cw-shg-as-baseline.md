---
type: craft-export
title: "2025-01-29 straight etched waveguide cw shg as baseline"
craft_document_id: 8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-01-29 straight etched waveguide cw shg as baseline
After aligning the pulsed laser, we get the power below

![Photo from Library.jpeg](../../assets/fab/2025-01-29-straight-etched-waveguide-cw-shg-as-baseline-001.jpg)

Tbh, it could be a few 0.1 mW higher, but I don’t want to mess with the back objective 

One peak that I found

![Photo from Library.jpeg](../../assets/fab/2025-01-29-straight-etched-waveguide-cw-shg-as-baseline-002.jpg)

Poling period is 14.03

Second peak

![Photo from Library.jpeg](../../assets/fab/2025-01-29-straight-etched-waveguide-cw-shg-as-baseline-003.jpg)

Centered at 14.82. PMT is 0.55

Both peaks seem to be the same height, so it is hard to say first is first vs second. Intuitively, shorter periods are for more mode mismatch, so I generally believe the longer one is what we want.

Below is the power with the Pulsed laser. This is with the fan running and everything

![Photo from Library.jpeg](../../assets/fab/2025-01-29-straight-etched-waveguide-cw-shg-as-baseline-004.jpg)

This is shockingly comparable to the bent waveguide case considering how much power power we should have

With CW laser in

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/B619CBED-32D9-47A4-B66F-066EF73F18B9_2/iZEzViyMrQm3l8NbxfkTn5RUhSZTZrzpv9oEimichMQz/Photo%20from%20Library.jpeg)

First go with CW 1580, no dice

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/D069B096-532D-4331-93E7-50058402194D_2/pENq1IixVNYyRxR4xMoQd9FgHryC2cy52zxS7ldiO04z/Photo%20from%20Library.jpeg)

I am going to try with 1560, which is the center wavelength of the pulse

No dice again

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/B044ABEC-69A0-4A07-96F2-7DC4523FF3ED_2/cnu0YPUWkKopQeZOMY6FgBnRgZPntR0cxRSG3TFirbIz/Photo%20from%20Library.jpeg)

Let’s try the other poling period for 1560

No more luck

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/5968BFCB-59A1-43E7-8186-8F9061BA5855_2/yD6mKRYLXvNDBoxjFvb5drq3GiSyRI9pvgdUcJgsO7oz/Photo%20from%20Library.jpeg)

Lets try a wavelength scan.  Below are Ryo’s previous results

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/da293f76-2dd2-49c6-2419-ff81884ee0a8/0AKdy3W7IxBzPYtRN1BpVOn0JxvUja5AYO8Q02uE7O8z/Image.png)

Another option is to do a longer scan (with like 400 points). between 14 and 15.  What is surprising is that I don’t see anything in the spectrum of the pulse peak.  I really feel like I have enough power.  

Another thing we can do is an output power scan.  Maybe I did a bad job coupling things

Nope on longer scan

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/83654D47-4085-41C5-A2D4-B00129A0FEF9_2/o9M4kifyE7e7BQZYHyR8eKYtZwagY34fZyCkiw214loz/Photo%20from%20Library.jpeg)

Let’s measure power

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/D8A01BAE-9766-41C0-8F8B-5BB3C350478A_2/XuQoMFvHapRPEbHa7xwcmF5m5ItCmBQnWr306RQ9NeUz/Photo%20from%20Library.jpeg)

Seems a bit low. Let’s get this up a bit

Forgot to remove ND filter, we are now good

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/7698537C-7AE3-43B6-9983-B309A327E6A2_2/qNGGFiktAgZQjxW6OpEOanftlDXxLTNUyFHWTWfTJVgz/Photo%20from%20Library.jpeg)

We are starting to have a signal

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/B8C7BC3C-FACE-4BB2-B9D3-A6D86167C2C7_2/Lf7olO6bFnA3AlXVASFVyHXjxAnxrNQtmDel86tyCxsz/Photo%20from%20Library.jpeg)

Let’s turn up the gain slightly and get rid of all pollution.  I put the black shield up and turned all monitors and lights off.  I made the PMT 0.7.  I may increase the voltage in the next iteration

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/78C7547A-7F95-4495-B837-0D7AEB22D392_2/qIWSzej7uJEu5RoYI5d3v06n1KMZR8vUn7zH1h4a69Yz/Image.png)

Lets make the voltage higher as well (3.3 instead of 3).  I also zoomed in on the scope.  For ref, this is with 1580

strongest lock-in signal.  Below

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/00D6CC61-E77E-4526-A670-57B0F25D28A2_2/2uFWIqjRyKLrxSiwZgx75tKaJQApVMDTDrLuXqKZsXEz/Image.png)

It is just not very strong

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/107C20D5-75DE-4BD6-A7B5-52E2518A8B1E_2/3XAYP2aD0dxHe2OTBmyeBzyWoixGBsxxLeCvkoC59yUz/Image.png)

So the peak is obviously higher, and I feel pretty strong that we are def seeing some signal.  The question now is how do we see more.  It is impossible to align to this by eye, so it still feels like I would need to plug the pulsed laser back in with this idea poling period and try to increase the power.  That is also kinda hard, as the sensitivity at this point is not great.  I am going to try the other poling period real quick.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/BDB38A13-2842-4144-B7EB-F986EE75B69E_2/IUGQAzeQytmCxnM5xNnythBCeZlvqbqDFf4QD7JRxe4z/Image.png)

This peak is def stronger.  I could just be off on which mode is which lol.  

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/CE294548-722D-49C8-A866-21F97DC9189E_2/6dgs5ABTVcC8GXclpPx68HmaFS9x9qA5WYjbYKsyluEz/Image.png)

Above is strongest SHG signal, which still is not great

As a more general point, it seems like CW light will always really struggle because the peak power is not high.  We know the bent waveguides work insofar as we know that we can pole pulsed light and see signal.  The issue comes down to loss.  I am generally of the opinion that we should not have poled any small sections of the waveguide, as poling the ending regions will suffer from loss of pump and the beginning will struggle from loss of the SHG.  Obviously I am not certain, but I am seeing slightly more than twice as much output pump power for these shorter waveguides.  

In theory, if we pole the bent waveguides correctly, I feel like we still should be able to see signal.  It really does seem like the ideal poling periods we measure for 1580 are very close to the correct poling periods.  Even though the waveguides are lossy, there is a longer interaction length.  The issues we will face are as follows:

1. Optimizing coupling
2. Getting the phase slip between different poling regions correct
3. Getting enough signal if the poling period is off by a bit

In general, some long-term solutions are as follow:

1. Annealing waveguides for loss
2. Using higher power CW light
3. Applying higher voltage to the setup (which feels very nessesary at this point)
4. Getting rid of all background noise.
5. More photoconductor

I am still a fan of the 3 layer device as more efficent.  I am just not sure if the photoconductor will still work after annealing.  Also, in the future, please remember to align the top objective a bit better

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/C5D2F0AE-5E30-4D78-9340-6C451EF5FD68_2/1dxoR3QxvLqubC6wzJJr9gvrg6EWywciUCNtN9dZsJUz/Image.png)

As a note, the above picture is with the correctly align projection pattern (by shifting the mirror.  It is really essential to do this.  We were doing it before on the bent waveguide, but we now have 3X more signal, which is quite important.  Above is with 3.3 Vpp

As a quick next step, I am going to see if the waveguide can withstand 4Vpp.  I don’t want to break this waveguide, but I really do need to apply as much as possible to the bent structure

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/FA69E44F-97B8-46F9-8217-8DCA9CA88630_2/zdgY2lC4mhe6wey6yCwOD8i0bOrIMRybXxx1E7s2vaQz/Image.png)

Abobs is from Ryo.  I don’t think we have much more use for these waveguides, and once polishing is back, we can easily make more.  So lets push things up and keep taking data (though maybe with fewwer points)

Near peak

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/A0568560-2DEC-4864-880D-2AB61B828FE3_2/xGhkPRQlGmPWolrLw1TpFtGoRWgDDtVEN99WfsCCGQgz/Photo%20from%20Library.jpeg)

4 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/C1F4B967-9051-4BF7-AE7F-216C3473A5AE_2/7h8zkWZ42NYskIf1LonJR0b7SdSLAGIki4QjxivR5y0z/Image.png)

5 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/C924B0E5-A293-4A0A-A0CC-C51EC58D82A7_2/KyTwseAhClMZaG2cyaZxbamCylnLRU6NlPVmrY8CDzUz/Image.png)

Near peak for above

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/34D5994C-D9D7-4182-BE7E-266344E09724_2/l3u5MLX2TehD2UIvx2y1YuBygbX3XfPQH6xwyKG5VlQz/Photo%20from%20Library.jpeg)

6 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/74C41764-E430-4DDC-B8CD-289A44302D0E_2/p86kIZ3LC1Yw5Yxzv94rSZ6HiY3M19wxyQwEMlqkaesz/Image.png)

Near peak for above

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/6FDB79EA-CC37-4059-BFD8-03F751CD33F3_2/ZcYy8leEzrMGBqsgMBlyW3KsP4rnHeEdti8jmJeozcAz/Photo%20from%20Library.jpeg)

Also, for all these measurements I used 0.7 on the PMT, which can also be increased

7 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/D59B7E1E-97C0-413D-8F6F-391FDB523579_2/zyN5zQ7HjGlIvxXnxSL9tSi3tx4dxmrJyWbCIJth8OIz/Image.png)

Near peak

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/9E3F7883-4B6B-491E-86D8-736C26243D5C_2/nq11Xr2PplA8D9asPv50akoInI77YF8WuAXX7z4VKDYz/Photo%20from%20Library.jpeg)

8 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/077D4189-746B-4667-AE12-2DE2E01E8F0D_2/K1MPmO6FrzTdzKNO7A2w0EbNadN4ERpxgCuFHJCjGy4z/Image.png)

Near peak

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/89EB06E4-AACF-4F24-95B0-3AB5A8F0E952_2/pxQpdDH4xx2SNpJx4OyVPprLponbQSlgpZVASMx03dsz/Photo%20from%20Library.jpeg)

9 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/19A6D51F-0CB6-4B29-A3EC-B6B1915F51D1_2/25lfFh7acsCgUrcqJQyTZwCMmORfsulpEjXN2qRok8sz/Image.png)

10 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/6BD25DB4-8156-4DAB-92F2-2D900C6986DA_2/AGAHOIxDTgaVQhvyORyF5cXqT1txDg2d0rxbLrehB4cz/Image.png)

11 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/679F7BC2-ECA7-4925-9288-897C60744235_2/3s1pC4QeokVpov9kxZ4fYbKIYSWlkB7yytHwuWJ7NW4z/Image.png)

Interesting that the ideal poling period seems to shift

12 Vpp (I also checked the Pylon camera, where the contact is in view.  There is no evidence of breakdown)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/BDA7AEC8-8F71-44F8-AF8C-3903417E3C7C_2/gayZY4rs5EZHBrJIDyng0kZHqCxiVVQnx6YncABw5OIz/Image.png)

Near peak

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/3658D4A6-E37B-4DA6-90A9-456B5595350A_2/fpwyBr2HInBPj1yV5WcJ0yJCIP4RgFyjAp2rD6uvMxcz/Photo%20from%20Library.jpeg)

13 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/8E7CA541-CDA7-46A4-A834-9DC3A247A98E_2/e7O4HDtEJRZgORSQKSX1XOnUexP6KgcKqHtC6q0Uqx4z/Image.png)

14 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/01F057CF-A1E8-46D1-8986-A621B65E4943_2/4AViyYBf00ZLMLV2ydH4ujbxpmu4rzInbKSkn7P3Fhoz/Image.png)

We saw an unexpected drop-off.  Something may have broken.  We can go to 15 Vpp, and call it quits there.  There is no evidence on Pylon camera or current data of breakdown

15 Vpp

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/8B1B4322-473F-4CDA-9A3F-E4D97C9EFA66/D506790B-9576-44A1-B3BF-65A36AA2C824_2/x4kKlxKEn8lvJUNhIxfy1wSwlPMdeeBdM2oDWP5RN6Az/Image.png)

I think we are gretting shuntted at this point