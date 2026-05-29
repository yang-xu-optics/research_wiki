---
type: craft-export
title: "2024-7-29 srn dc device expected values"
craft_document_id: 24746401-5942-4C96-9F85-FA8937B4409E
craft_collections: [dc-device-full-fabrication]
source: Craft local PlainTextSearch cache
---

# 2024-7-29 srn dc device expected values
We have now done a tonne of characterizations of the delta_n of some of my SRN DC waveguides.  Now it would be nice to try to explain the results doing some conductivity sweeps.  The hope is that we can also do some conductivity characterizations of the SRN chips such that we have more data to work with (ie, data that is experimental), but we also have two data points and some rough estimates to get started with.  This might even help us estimate the chi3, as I genearlly trust our conductivity measurements.

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/3E149073-95FD-42EF-B7F0-6347F67DCAAD_2/iuWHHGNPexgIIbAJ6O4xQwU0MjfJTIQNNKwr0d2xIPQz/Image.png)

Above is our predicted indexes for the DONs.  As I will show below, I get very good fits for the SRN values and index of DON to predict the conductivity.  The fits are below

![Screenshot 2024-07-28 at 3.19.15 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/4A974D9B-5CB7-4FE8-9E3D-5C13E09340B7_2/BnoASiDIBzDLyCBHuUVtwFFY58mQid4CXjwmeCY7CVYz/Screenshot%202024-07-28%20at%203.19.15PM.png)

![Screenshot 2024-07-28 at 3.19.05 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/FCA38B99-434C-440C-960B-EE9528D438C8_2/0mwFz0xZu0MFh5TSdbWtgjupgR8aicERllW2pJZOOcYz/Screenshot%202024-07-28%20at%203.19.05PM.png)

![Screenshot 2024-07-28 at 3.18.55 PM.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/3A78143B-4CF0-47BE-95FB-D07BF0C655F8_2/DxO7CNmkBFQdgemPboi504qb5tf2XKCoCPSGYxpA6VIz/Screenshot%202024-07-28%20at%203.18.55PM.png)

We can insert the index and/or silane flow to get the predicted conductivity fits.  FWIW, I am not certain if the bright fits are perfect, but we will start with them and tone down the cond0 in case the fields seem too high

Below are our predicted fits

Bottom Oxide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/B38C3B95-1021-4790-99E0-F164080B50B3_2/nSBROM8LkiLaJWuJx3GG3Xe40zFBvNJmCnlEnCh37coz/Image.png)

Top Oxide

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/272BF939-9424-4BA7-A4C8-52FF2E857FCC_2/SqJv96oskpmdM2lIkTjhd8FKPoqcvHMARfAZ56g8a1oz/Image.png)

I just updated the values in my simulation

Now doing 3.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/4D8BF04B-49CD-4BB8-BDDF-C5065D1C5A2B_2/e4qmWwHxTbd6ZG9aya28H1v4Bw0tLasxZg3BtM6D4vIz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/C54AE420-BDE3-425A-8E44-F9F0D937B8CD_2/HSvEsws3iYfRZlnDlnwxPWtxELPz0YauLBsyVID1SRkz/Image.png)

Below are the results after simulating Thickness = [3, 2.5, 3]

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/431284D1-5B6D-468A-8339-9E69AFAB0345_2/V532myIc6x24Kd1NljALYMecEUNSEvrku9IUK2mECJMz/Image.png)

Now for the experimental result

![Image.png](https://lh7-us.googleusercontent.com/slidesz/AGV_vUfA9JnKYvaEKaXlaodT9Zk9-yKqb2gvKsvFfsM4g6n2MRfHjxy7sI_6O8fPWGWB8dxs4Flc2BPaaPJMcCPa3jNo9cbNk5V38KfpK1-o9P9onGbGJigzT5drN6ghlGiwMo8IWITbm8JzKgdWb9IKoyZVImUUbQQ=s2048?key=Zw5904JDi7aqPuXefBvH6A)

Not totally dissimilar, though these are really though fits as we don’t know the size of chi3

SRN4

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/24D44B0A-8C45-4441-88BC-2D4FF6070DA5_2/Deh42WWUJdVT6xJcg4clH4zxa4Y3aHKS9kCayyTx3uwz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/93618A1C-0D7E-433F-B9A3-44B8E8197914_2/mQ6qzARnRTcZWw6UAp4X6NzhZ9aYLYKKJMf4qsLJFxsz/Image.png)

Experimental Result

![Image.png](https://lh7-us.googleusercontent.com/slidesz/AGV_vUf1a5sNAue6XWw8RzqHv6vX_ayNshADxgrbWDNJPESP1xgXw1IOeQVMNFJtWu5vbQSm6QE1KhCQHObRGg-fYmDOZGdkuB-XpL57KqbJ5Nbyoc_MSa6EF1zRL8cVc9i1ExSLn5MsDQl3u5cTqEeidLvDPSsv_9IV=s2048?key=Zw5904JDi7aqPuXefBvH6A)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/F42E68CB-64A7-4790-B943-AD9638094DA2_2/uvdhb9RcDaokjv2iVfUgjzfZxo6pHkLqCXwPEVqCYtcz/Image.png)

SRN 4.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/9B94618D-9BD7-4512-896A-DA1C86A7377F_2/dzZfVkPdTNhGZK1Dk5E9j2IV5IBvtm2J4xtRO61di34z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/C586CE4F-A5C2-4E2E-AFC0-1E4CBBCEAA81_2/RgPd5kDZDbfNFoVgGoYx9W14jnrvKtY9NvWgH0A5Tegz/Image.png)

Experiment

![Image.png](https://lh7-us.googleusercontent.com/slidesz/AGV_vUckguOE5VJVLwCS0mVkUAudl-TRwgO5rsbTtREfRqgfqvZxzc6evnbAaQ1Es0k1VCK8HJgdpu61v31E3eWIxiPY-mIfYnJBq5GOl70oYCCIPuNUyLPI_0CON__qsneCcdUJWeoycDyfMUqkYtITnhMwmEl_9SAC=s2048?key=Zw5904JDi7aqPuXefBvH6A)

Simluation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/A25105E8-A23D-4368-8D8A-B92D2482CA90_2/i3zW5Y12OLQ8Ozvb6fVfNluiaq5WmjnWo5EpR5IWAQsz/Image.png)

SRN 5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/5D5796E5-4928-4BBA-978A-73A1FB9B175C_2/yQjqpa5pOv5DyMXU23FyiVlMTeTKThsbGwQ9W5k29swz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/6695C686-8E51-49C7-9B90-810F1E6E3CE5_2/Oyz4wVyES3SxJA1xhBesB6RHfmrxxCQNHJQryQaBBX8z/Image.png)

Experiment

![Image.png](https://lh7-us.googleusercontent.com/slidesz/AGV_vUcyRAtbzEXt8YZfnpaAVed531tX0uDBUzjcHAx-y4X-8mEMl4ad5pq7tnHuZbsR6z07JhgqiML_4tJCzgong2bBdHzFG9GbktdLpGwX_DAupfOf9XS0QkOcJyx8n4R2T571e1zZJBze6ybtJSoZ0IYzbpf2R78v=s2048?key=Zw5904JDi7aqPuXefBvH6A)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/CCEA4D47-4788-47C2-8712-4A78AEBD9C22_2/MqrndvO1PY33ypDKC3aXrgIF0EDUnPVK8J96dpLCntsz/Image.png)

SRN 5.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/46C0C4B1-A71F-4603-AE9F-64A191444C57_2/kXG1pfz3HDjoVscdJsHMZT9pLdLzZRFBveycJfrpVN4z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/187C1557-5E03-4266-8983-738A6180785E_2/CvtWKslj9u8mDxxjtDYpSdPUxPzNwyeZpyadzYy7eQwz/Image.png)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/7274A8D3-FED8-40B7-ADCE-D1A1D4BADC45_2/P7OgplwKxt6pm9ZvBRAxxUBH1E767XkBtWdMjzUZdqwz/Image.png)

Experiment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/deb388e7-3774-4d1d-dd27-f1817cb95d7c/jDMiXVncrkmH9uVZj7cRwwxamkMW0YQ7uyCLkNtCdKgz/Image.png)

SRN 6

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/0C3B7A55-425B-4472-B860-D935E26F7C89_2/dqZsyPjXZNte2Dbf5lhxYLd6kgpo3yaHkxVoq0syynsz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/F4BB82CF-D48D-4E08-B92E-14465E06FD58_2/3MA2MCDmM4i7VklXRy6hn6F1vl3U2mPH6KPXTc0IjOQz/Image.png)

Experiment

![Image.png](https://lh7-us.googleusercontent.com/slidesz/AGV_vUfPSgdRbA2dkoVOZlPxxas8eIBhX2CzsqzRYaVIQe8H1O0t28-uMe4DXHhvG6XjZvWVYiZnUsC83XgaA6VQTYvFQPvjHeVxio4igfW7QOkph2JEQs8semhsAJG1Y2w-xjAAlWmTDrio0bDky6KIwWw6MrcE2_zp=s2048?key=Zw5904JDi7aqPuXefBvH6A)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/2BC38A44-8ACA-4DE9-9352-1B81646ADF09_2/Modhk5u9gtH4xJws8stt1BvInbCHEqoeAbQ1iClxIhsz/Image.png)

SRN 6.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/46BB7C64-6484-4130-812C-94DB39ECA1B3_2/qbz5OX3KYaD10W6VLU6LuxK8qusNlFwxoa86Iq8bh9cz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/1684560E-E8EC-4528-A6BA-1DD087772F4B_2/WfVlZdu9Mq3aEiXLcrCOkcFnmQ1dJRneeeDevn5xy98z/Image.png)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/2E23A949-AEDF-4406-B3D7-871D208F7C81_2/3hKMaYkOu2gP7VOAQb17Y3z9UwZWEgpBpl5XgIrVomoz/Image.png)

Experiment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/36647d0d-5ab1-9097-03e1-6a7ee05ebc1d/3xTcjntuBRxLLjYaWDy8Bmyd71zHzDCSeG079dcLxBkz/Image.png)

SRN 7.5

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/8C0F4384-0879-42DF-87DF-91BDABFB93A1_2/PsJsmCsjUBjtQI9aVmTxUAecN4wC6PDXxhqBTcm6yLgz/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/E1D26DA8-5A2D-40AC-B0C6-9BF42BE59B1B_2/yjjSyg1LgusWNe512a0JKL0TyXoLPAjOc78X6xptFSkz/Image.png)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/73A74BE2-2531-4F2F-98B5-D065D4290221_2/N9AyCgMjz0xylYuYioIwoOlK64EBRxubNcoywDPyufgz/Image.png)

Experiment

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/969abd73-85fb-03e4-fed2-b73207344e87/qJoVmBkoHsn1alYLL9DcSqdkXxLXIFN1JL7dj3cKngsz/Image.png)

SRN8

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/023EE554-56A8-4B90-BAB2-483A152EC21E_2/z2UprDfGTBNixCJFXamF5qct65mBCihk1ydFdv5cSA0z/Image.png)

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/C4631C93-958C-46B2-9124-EEF5F5A437C3_2/mh8wtysC1pS1DbwQfIzdgOV5iaLMcxvIixP06mCm4HQz/Image.png)

Experiment

![Image.png](https://lh7-us.googleusercontent.com/slidesz/AGV_vUf8ERNS5rX-xNBqsmOP2debo9W5KS3Bwq5g2UuDT9SxXK0Sidifk9scDoe830kigJth8ClWf4cQCVO6rVzuuNGxStbT6ZNpaL_uNUVrfi0hgmzZ4Wr8qA2BKqyO15o6IJnBEFnS1C0SyYrzDFA8VESKv2xvdXFh=s2048?key=Zw5904JDi7aqPuXefBvH6A)

Simulation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/A078AA35-5B3F-4856-AD87-1BB189818DEA_2/xHiK83fgrKFiYvHYp5AsMAXfnxrRbj29E9Tuv0VeQZ4z/Image.png)

Some basic take aways are as follows:

1. For almost all of these, the bright state conductivity is just too small.  while I think bright state chi3 increases, not by this much.  We were predicting 10000-100000 times more conductive, which is ridiculous.
2. Around SRN 5.5, our dark state conductivities seem to show annoying kinks that we could not otherwise explain.  Either our simulation does not run long enough or (more likely), our predictions are too resistive.  There is something to be said here for just using the raw values we expect

After playing around a bit, it does seem possible for hte bright state to get slightly more field into the core.  Granted, we could just have some numerical BS going on now, but it seems legit

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/A4A26B2A-743D-43C1-92D0-CBF91C32EB82_2/iUjvzLbViZHaRzTtPCpLE8SW729lUTuOxmjERhm3M0kz/Image.png)

Conductivities that I used 

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/24746401-5942-4C96-9F85-FA8937B4409E/69DCD07E-214B-4F0A-80B1-A8BC075A9666_2/eErxFBQSlIgXq0WmVBxoVRTt29Yp24bLhJWCX61RDAsz/Image.png)

And I plotted the fields as a function of time, and there was no shorting