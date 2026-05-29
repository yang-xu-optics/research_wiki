---
type: craft-export
title: "2024-9-1 dispersion with don cladding"
craft_document_id: 059C421D-B07C-41EC-992D-90EB95EAFCA8
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2024-9-1 dispersion with don cladding
We have done some previous simulations with normal oxide claddings, but so far nothing has been able to give us zero GVM.  I still think it would be cool if we could see that (even if GVD is a bit higher).  So I am going to scan over some conductive oxide claddings and see if any of them give us films with more useful dispersion.



First, I am going to start with B8 and see if this works

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/e2810bbc-332e-af84-2f6b-60eb3ab39aae/KqYZR7kf5JxxoahgNZe8K8AYKySyCfusX0cbfsikWlAz/Photo%20from%20Library.jpeg)

I got code working that gives me the correct Urbach tail (shown below)

![Image.png](../../assets/fab/2024-9-1-dispersion-with-don-cladding-002.jpg)

Anyway, lets generate a txt file from this plot and export it to lumerical.  I am also going to generate a few more plots while I am at it, and all my plots will be for SRN 3.5 for the moment.

The material imported correcly and I get confined modes for SRN 3.5.  So my first simuations are with SRN 3.5 and DON B8

I am also going to import some more index sweeps just to get a broader understnading of how things work

B25:

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/19800b1d-617f-dcc1-0788-d48add6a51be/rBbhBmsUNSNPrpQaAaYx1ddqdCx3Y0etHYMYNDXpUyUz/Photo%20from%20Library.jpeg)

For some reason the k did not fit here, so I am going to use the same k as B26 

B26

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/e53c1655-e0fb-bc66-c0d3-0dc8485b1f3c/zcoaKqx1OXBBBA0GD2gxPJdJXPCjMVtxhrOri9yNutsz/Photo%20from%20Library.jpeg)

B27

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/ae425f90-fd66-b8d6-beb7-7f33602616b9/qPI3vKjiauiVf0ho4eKwC0RMMZHWh5Cjozuuonp3Jx4z/Photo%20from%20Library.jpeg)

**As a side note, we need to make sure our dispersion analysis only take the real part of all these indexes, as we might get some imaginary bs going on**

At some level, I am not sure how much to test the urbach fits on these, as I did not fit a wide enough of a range.  But we shall see I suppose.  I guess it just seems odd that hte k-cectors at almost 10X higher than B8, when that should just not happen.  We may end up nerfing that loss a bit more, or just resuing B8 loss.  If anything, lets just reuse B8 loss.  It is probably a good approximation

I reduced B25 as cladding for 10 widtsh and 5 etch depths, as the simulations kept crashing and having issues (I should also mention that these custom claddings take much longer to simulate)

Below are the results for B8 cladding

![Disperison plot for Height0.5.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/198C4539-5CB9-4DF8-8DD2-5B95282E2870_2/75damFk8opafYBCyVfYzLHfqTyBcxY69aa4TDDxQ9PMz/Disperison%20plot%20for%20Height0.5.png)

![Disperison plot for Height0.7999999999999999.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/C16E8CDD-701B-4367-B46D-EEF05919F400_2/rxhUnOxD0cgPyseLODmxRVbP8uPzX2NCAY3eDaKG97Iz/Disperison%20plot%20for%20Height0.7999999999999999.png)

![Disperison plot for Height1.1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/EB5CC4F9-6E2D-4ED5-90B9-C20CABE8F5C8_2/sEiH9Ya5a3CxkdAikyUMsKI2nAbMyV0o2PxvFwX0nk4z/Disperison%20plot%20for%20Height1.1.png)

![Disperison plot for Height1.4.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/9EB4A148-C4B0-4953-9CA6-91A1B987B380_2/5EiT1hyYzY7RrvHjGtJtA47YJFPwHnDolaY7xPihFqoz/Disperison%20plot%20for%20Height1.4.png)

![Disperison plot for Height1.6999999999999997.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/8C484B39-BF0C-4411-8A97-354E2C2D275C_2/A4aHgNKxUwoPiwW6zrJoxRyXM2bBE9Sc92UddAcxOEQz/Disperison%20plot%20for%20Height1.6999999999999997.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/DF370D24-2BDB-452F-8EE5-C5040702F0F4_2/8saqOoNJL8LjYlEAWnQg6vaeiUk26PtdhcwOVP9hAx0z/Disperison%20plot%20for%20Height2.0.png)

There is an annoying inverse relationship between GVM and GVD at 1550.  Fortuantley, the GVD at 775 is always zero

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/FA1210DD-138F-4480-84F4-0782F57511FC_2/dQWiEXpb7oxOT6F6nzXy5dCLdx9NdQ0HSLyC4ZSiAMMz/Image.png)

The one interesting note is that it should concievably be possible, at some point, to get the ng.  

Below is B25

![Disperison plot for Height0.5.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/6D2EC7BE-9FF6-43E5-9D38-E1EBB8AAF39E_2/1pSp7qNBsw16TVFgHnTB4MYco5rsdxx9mnxcfxEJjEAz/Disperison%20plot%20for%20Height0.5.png)

![Disperison plot for Height0.7999999999999999.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/9175C47E-5B6F-4791-A20E-20B8B00CB6AF_2/rSqdPRrtCbP2f6676xDrVNRtuphTcpjwThTqt660F0sz/Disperison%20plot%20for%20Height0.7999999999999999.png)

![Disperison plot for Height1.1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/BCC28CBD-3E9F-4DC0-B589-3D3725F06F25_2/85ObTWZZyLLpyESo7Pqyoo8wbMKS46CTjeO27MRXZyQz/Disperison%20plot%20for%20Height1.1.png)

![Disperison plot for Height1.4.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/4FCA83BF-7D63-483B-8C4A-9640CC086CD1_2/fyNrV53eJ1KxkXrRn0m0mDpQAyRUM9IAqz4g88v3ZF8z/Disperison%20plot%20for%20Height1.4.png)

![Disperison plot for Height1.6999999999999997.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/DCF46C03-4427-4867-B6E4-816A407D49B5_2/PNUnKJx8HMy4d1sxyRPk82Y9pTMxVDt9X7tQKTWdJyEz/Disperison%20plot%20for%20Height1.6999999999999997.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/7FC7B1F2-E63D-475F-85AB-DDC8B19D8E0E_2/lLU4gPcAPn5UUUF6sBr3G2EfpbaCIpigLPjw972mEyIz/Disperison%20plot%20for%20Height2.0.png)

Once more, we still have note moved GVM quite to where we want it, but we are starting to reduce the GVM for thicker waveguides.  At some point, once we start to get close to our desired GVM, I should just make the core stupid thick just to see what happens. GVD for 1550 is still going to be an issue though

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/BF9937A7-A191-4E9F-91C6-F089EB989676_2/osiqK5tiyujCNxBbcvUhds8YQS2m7iZ2CZJpGJPUYxcz/Image.png)

We are also moving ng for 775 in the right direction.  If we can just make it make it a little smaller, that would be great.  It is a shame that we can’t go very wide, more like very thick.

Below is B26

![Disperison plot for Height0.5.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/BB20E6D1-EE39-40B0-BCC1-02390589D0AE_2/wexyE2drn8EsMsbgQk3gxAL2URmpc5jGSIjCCAzLj9sz/Disperison%20plot%20for%20Height0.5.png)

![Disperison plot for Height0.7999999999999999.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/5574085F-3CBC-4A71-B4F9-D825E7330DBB_2/Waycjb4JLrplk0Bdt0OF0J0miagpeU7N56CwIijoW5Ez/Disperison%20plot%20for%20Height0.7999999999999999.png)

![Disperison plot for Height1.1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/9BFE9C6F-3A06-47EC-B1F6-0682CEF5CBAE_2/v4ywgpZOWlJLTJliIRXQ12FCPEx93LHbbaj7emPIeDsz/Disperison%20plot%20for%20Height1.1.png)

![Disperison plot for Height1.4.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/AAECBEAE-31C9-4D4E-A822-4DCDD0A726FF_2/guelrwNYohO5pXwfy5yD3sD7fU7rLUGjBllP2jMnAYoz/Disperison%20plot%20for%20Height1.4.png)

![Disperison plot for Height1.6999999999999997.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/D6AAE872-31F7-41CC-8EAB-528980CD7655_2/FvDYlytiFwnpPUyTF4rxelU26M8HkryGvPFNNqgolN0z/Disperison%20plot%20for%20Height1.6999999999999997.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/A3CDA23D-F3FD-41A5-985B-43C9BC1FB0EF_2/UF5tNQdNDXxqh1qt5UWyFHvfNVsC2IfOsJygXFeVhHIz/Disperison%20plot%20for%20Height2.0.png)

Below is B27

![Disperison plot for Height0.5.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/C47DCDCA-0766-4308-AF40-206F4B3CA3AB_2/ZTRVwqDzIcH0XSo1uINVLryIlhYCCcz5A2VWAkz3vPoz/Disperison%20plot%20for%20Height0.5.png)

![Disperison plot for Height0.7999999999999999.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/743CF4EF-9433-4E11-8C78-D2632ED8F947_2/qnOEUA2LYg4Si5TWJ93F0h5NxtJLodNFTCn1recIUmAz/Disperison%20plot%20for%20Height0.7999999999999999.png)

![Disperison plot for Height1.1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/34D89D68-73D7-4B0C-9137-A1EBD6B6BA96_2/uusI2lFwYdxDLJUYHmntTBp05FiRV32FVf1HtO6hq5Qz/Disperison%20plot%20for%20Height1.1.png)

![Disperison plot for Height1.4.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/D6E45EAE-71B9-41A6-9416-504995DF2517_2/xgAYJlZlMshx8IbzrCnA9NbIfVbFoMwi30l6whOKiQMz/Disperison%20plot%20for%20Height1.4.png)

![Disperison plot for Height1.6999999999999997.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/98EF9C74-D688-4256-8546-FA104D93943F_2/pLH7k11EfeyPC7qPHBlrPBEVxHQxuOWQDJggNHBHEWgz/Disperison%20plot%20for%20Height1.6999999999999997.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/404B1815-581A-4048-9C4F-FBB07ED52587_2/fGhppZyHrf2h3rPJRCGv44r0ORkuBHWnVwF6VXBfi6wz/Disperison%20plot%20for%20Height2.0.png)

Below is B27 with SRN 3 instead of SRN 3.5

![Disperison plot for Height0.5.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/6A28A8B2-CB00-4F97-9911-F70E9CC10862_2/EoixFkzbc1f2Lww7rLIlte9T0xnBfVsFG035inOXGbIz/Disperison%20plot%20for%20Height0.5.png)

![Disperison plot for Height0.7999999999999999.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/0B2C8A4D-6AA9-4C87-BFF9-BE397F392E3C_2/oSVE72riu73zVyLENh1Tc2dxgL6sgubvtS7oemxlOCEz/Disperison%20plot%20for%20Height0.7999999999999999.png)

![Disperison plot for Height1.1.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/AFEE013B-94B2-4684-93B4-DF0B37842765_2/KxGF745YGurDmYBITpCKPob28ewYaWrbym5xuRITUJYz/Disperison%20plot%20for%20Height1.1.png)

![Disperison plot for Height1.4.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/4D642867-5EF1-484E-8344-4B235F92A336_2/d6bKKe0RLJWFusgvb2rwX73mxQ0KRYD174sDhNUScNgz/Disperison%20plot%20for%20Height1.4.png)

![Disperison plot for Height1.6999999999999997.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/1638DDDD-B7A8-4239-A702-E02FF26FE61E_2/7XMv5cfjuxyrz0HdewDs5REK5yZnvcpFgsJMpUPnm8Yz/Disperison%20plot%20for%20Height1.6999999999999997.png)

![Disperison plot for Height2.0.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/059C421D-B07C-41EC-992D-90EB95EAFCA8/75216970-B6F3-4A19-A5F1-F653BCA1D89D_2/gmysndx6NQlOoMNbNKl0njZcDXHQ3DCozoPWxQZTPhUz/Disperison%20plot%20for%20Height2.0.png)

So it really does seem that the cladding did not matter much, but the core matters a tonne!  We really want to push for lower index core, or even try to push the height of this device up (though there are some pretty severe drawbacks towards having thicker cores to maintain good field contrast).

