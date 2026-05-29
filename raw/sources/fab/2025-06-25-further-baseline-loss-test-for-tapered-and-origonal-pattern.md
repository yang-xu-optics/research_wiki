---
type: craft-export
title: "2025-06-25 further baseline loss test for tapered and origonal pattern"
craft_document_id: 052442E1-763A-4798-AA5D-A06F0C6B218D
craft_collections: [etching-sin-waveguides]
source: Craft local PlainTextSearch cache
---

# 2025-06-25 further baseline loss test for tapered and origonal pattern
We are still having issues with Loss in the tapered waveguides.  The losses are still a couple of dB/cm, far higher than the 0.5 dB/cm we expect.  We are going to try to exactly replicate our previously working oxide hard mask on the new SVM wafers that gave us 0.5 dB/cm.  If this does not work, I am biased towards either blaming the tools in the CNF, or simply say this new SVM is just bad.  I really don’t have a great reason to suspect this is going to work, but hey, we did it before, and nanofab should be reproducible.  We can add some eco clean and piranha steps if we want, but that should not make a huge difference (it should theoretically only help). 

The hope from this baseline is that it would somehow help us to understand whether one of the tools is broken, and hopefully give us a baseline understanding of the SVM loss, as we could not simply use the longer spirals as a more reliable baseline.  Maybe we could at least compare spiral losses on the two wafers to see how bad the taper is.

### Photolihography of baseline wafer

Before arc

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-001.jpg)

Before resist

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-002.jpg)

Before edge clear

![Photo from Library.jpeg](../../assets/fab/2025-06-25-further-baseline-loss-test-for-tapered-and-origonal-pattern-003.jpg)

During edge clear

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/5D26BC1A-6490-4466-BA0D-4219BDDE5F6F_2/eTvaUF6OjJotSxHUulb8RAeGs9i608Z3VUxuuwiJmUYz/Photo%20from%20Library.jpeg)

Before main run (using exact same recipe as before)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/CF8D3337-6A5F-4A87-894E-9909A13B21EB_2/OzAkZxS1rcJeLwmNyfijN8B6gKCrPgiMUqHN323JbaUz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/7612A260-558F-4304-9775-B8C9F1FFA29B_2/LqcPlBmvxTisg3WCfQHrhMIvrTvKXUsTkxBn6Q7fS1cz/Photo%20from%20Library.jpeg)

I adjusted both doses. They did not start out the same, so past device might have different waveguide widths for medium and long

During run

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/CFF02555-0A21-48FD-B3EE-AC13D837AEBE_2/4dqfWxEP7Ukot0pxvRgogcw5s1C24yxzjhfy49dlNnYz/Photo%20from%20Library.jpeg)

Before developing

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/883EED48-7E72-4A84-865C-D73721E66E46_2/FrdgpnNTHGeZQyHkbWIFzVMeH2xwn6vJOZWyAZHcxwwz/Photo%20from%20Library.jpeg)

Images of tapered mask

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/6829B073-B4BB-4281-8126-FF7DAE0ED0AA_2/STCgj6uEXH5DEMjjY9c4aa42flkCX0JyG8xIlsydxxMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/471C98DC-13D3-4E60-A24D-FD8C742E5B15_2/Uf4Y623cLWdgDhv3R3uHkjoAK690xUxuJd90QprxJ5kz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/CA9D3F44-AC5E-4AA2-9870-9563865E8E8D_2/dMxPa6I5lMvg96jLvaEnSuZWmEdr0HFwRiTSld4QgJkz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/782C28AC-E9B5-48B9-BEDD-CE3927609AD8_2/DnUcXzebycxEZUfV7wmQhAxL83gDHMxROEb6nSNxNYkz/Photo%20from%20Library.jpeg)

### Etching

We do a 5 min preclean of 82 and 100.  We only need to descum one wafer.  WE spinly spin dried the other

Before seasoning oxide of 1

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/1450098B-CBBC-44B3-8C30-5B9C71B3EE8C_2/TIjjEulN06TuFcV7X0brXaQyZ3pKd44JmcIfwqF4tNoz/Photo%20from%20Library.jpeg)

1:20 descum

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/28FD398A-E4DD-40A5-9AE3-FE4624359863_2/cpnBvMJPF8zEd48xJfpKMxSxwyFDqM59ANqLc7RHWz0z/Photo%20from%20Library.jpeg)

We now do 9.5 minute etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/742173FE-B742-4B2D-A516-69CFCBD15ABB_2/DyDGObqCeb8jr2O67kSdEZEzYopraxLyjIYKt4ywNZQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/AEC088A0-FFF3-4107-84F3-8270851631A6_2/M0Skpe40pftR2HpJvyeQiJcYw4BVQ5zyL59N0fPwbYkz/Photo%20from%20Library.jpeg)

We will do eco and piranha clean

We do 11 min clean on 100

We do 2 min strip on eco clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/A04B431F-9C3F-44BE-AAA7-12A566F2A3E0_2/pHplS3YBlkQLdCzHNHWbGBTkf2OVpOYIkaJIx1ehT0gz/Photo%20from%20Library.jpeg)

Seems to be going

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/6C1B418F-A589-4CD4-884E-B120B553AE5B_2/cjuqESQ75O8yMnifWG0DdWVzgyxOTWWjqBQv2JwhKxcz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/F10A1A87-6316-4308-9598-8673F0D9A2B8_2/9CBAe4SYSP2DKIwi9uGKYoa7rYXGZ57CRFvY8qCddq4z/Photo%20from%20Library.jpeg)

During piranha

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/B340B9DD-1C86-4890-920B-87222D65B811_2/mO59pEiDpgqgZfAs46zXEpZW67Eo2i8DmKKc8igMUuoz/Photo%20from%20Library.jpeg)

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/C14E274B-7B0C-4ACA-A8D5-717B7D4A5B3A_2/rAKjbbrC15yGjgJYRtyWLYktDhdFAz0B1XnhwiAawMoz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/D601B0A5-F4DB-4639-8396-E5C2A17BAE74_2/CxGFOD1L4iZQFXJQEt0GbjdwA4TPTDwnmpFCTIUGUJQz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/DC6B2302-43F8-465D-831A-8ABEF4AB89EB_2/Hp6fppptg38q31JPZyNY6I3GsuNsA5IipmKdLw9dgM0z/Photo%20from%20Library.jpeg)

Spot on etch, and the numbers check out 

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/BCAF5532-E1BC-4F54-9DC9-8FA0E66C1F15_2/WDEUlM0gJFjHNvaM79MHzB48irmuyAOamiwSdu5x6MIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/0FDC48AC-1288-4D2C-80AA-60EED7A12DC0_2/vieyC6J3u5Obzcp6dYqxtxlQNsv1Xx2h2nd0kyMYOy4z/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/9B9AFE33-9851-40B4-90F3-2092E695F71C_2/5CH4llYczi2kHgurUGhw9MvDYyy2UiRvRulOy2yjvkgz/Photo%20from%20Library.jpeg)

Everything looks very clean.  I have not noticed any issues with these oxide etches either



Before second oxide etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/68015A19-F5DC-4226-8E8E-CDF6919FE1CB_2/6WSFQ9lVI8b89PjS42REjY3j9pPfmj654Eyopd0FcO8z/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/E9E7D001-55AE-4399-97A1-F33400D2629F_2/QWn4780aH7cxMOC5mqigHX8jxbO1Cig1qXFrA73d280z/Photo%20from%20Library.jpeg)

We run ecoclean again

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/86286CF2-8177-459D-9FCA-132C3136FF48_2/ylTI4iiF2wRGHWKgnCw3D8lAOwLOquoAKPHdH07wA7sz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/3603065E-6D06-4E95-B492-AEF9BA13BF2F_2/lZf2PAHr832hFm9LFdfMcxgI9IFRyEFoYg7aFJTUpoAz/Photo%20from%20Library.jpeg)

During second piranha clean

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/6E445A06-1178-4EC7-B1FD-877C6FAEBD32_2/3QP2ezEnILj7gC0TY576D5tPXluogx7YSgYr5FyRtQ0z/Photo%20from%20Library.jpeg)

Let’s do 2 minute season for nitride etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/B72E126E-819B-4DD5-A9CC-64D40602818B_2/cOY4EddJHdVjLA8X3CxH1lFRPmgWZccBZhoXpc0HQiwz/Photo%20from%20Library.jpeg)

We do a 6 minute etch on the tapered wafer

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/CA86A702-4D73-4E0A-B3CA-853C7CDECD1E_2/PR1dAqeyBaKcQwAl5gn0fbbeMnS1OL2rwI5YHycjOGQz/Photo%20from%20Library.jpeg)

Given the amount of O2 flow and the fact that we did not clean there last time, I am good going straight to the cap.  I will take images beforehand.  I will clean chamber for 6 minute

After

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/FE0CF5E2-7586-473F-A3B7-D16E2B1E24A4_2/LB4TsIlwyvUbaaZAefxuUOfpjgHUpdeEfyaW8rxQUyIz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/BE99C721-59AC-45A0-A45C-1D8F61E74FAE_2/RcC7QG4RUwC9KogEERyUsMdlCbCna0eaNAQ7yjC1C0kz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/86795E49-C27E-4A5E-A104-CB211E174608_2/P5hgBgTJqWTC9nAnzAbRizpfkDzePy3am2P9teawtaMz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/9D8A1926-04F3-4117-8B83-1F2ADC8C1D96_2/k0mWezqc7LvWYH2h91n65ovf83votiTyR7WaHRqexzYz/Photo%20from%20Library.jpeg)

2 min season for the next wafer

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/F075B5FB-B6D2-42AE-81EC-C03EB7D939E8_2/fIgoyAgr8vJePW9hlS7S4dyDIEcOWxkLPhtYmHkfDPcz/Photo%20from%20Library.jpeg)

Before second etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/CC5B6D98-9092-471E-B9F9-83C2B8DC3D2B_2/ieEAxBHi3B8WM1LRlR1AjoTaiG9cPT0wcgFGMKy8Ut0z/Photo%20from%20Library.jpeg)

During etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/325BD4B8-0947-4B12-B168-6F4B7269C961_2/x6ulfeybUK3kvnVqm8y6wEBnS0wEV1Xdb2E0YbPMrYYz/Photo%20from%20Library.jpeg)

Inspection after etch

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/DF4A9A33-B75C-4251-ACED-829056F97A8D_2/tLHZyujH986YNoh7x5sK0SCTmj0K8N0F8i6UDfZIq9Yz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/72991BE2-40D1-4C5E-8D3A-87BB62FA590C_2/TybHMvPYgC1z2VLYNOKQbKUMTLs9k0hmo0olTPnCyXEz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/78C69502-A1C1-4691-AB2C-8A7F20D55993_2/t8ZesHq28n5rpa0zymDqVKyxH4bgsKtitwwiLAWDxZwz/Photo%20from%20Library.jpeg)

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/331A3F61-DABA-4093-8543-6341365643D7_2/jgF1jZIT3pFVFOKjCcs6Tx2MfppVpBxxK6uE4uDQqtoz/Photo%20from%20Library.jpeg)

### PECVD

We start a 10 minute pre clean

Before first season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/1BEA9301-3290-43F5-9BEE-0162FB774AAF_2/FRzkT3y7VMdPxgy9aP3KAncvShWPc2xnC7AmkPwgHcoz/Photo%20from%20Library.jpeg)

Before dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/205A5710-49EE-4E6C-876B-2C797BA97328_2/Fxem1sLYVxyxyiRa4LW9BRoKxUwc1XTFvtsxSrkIUakz/Photo%20from%20Library.jpeg)

We now do an 8 minute clean. Hopefully these will end around the same time

Before second season

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/8D1647A2-2BF4-4506-99A9-9DB21D7073B7_2/cVzzhw1mX3MdTI9cW5ye0iBfWMq5LushP4WVzNKmxRkz/Photo%20from%20Library.jpeg)

Before second dep

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/0C798857-8FD8-4D78-BF04-96A9932B3AA0_2/jIeXXNO7DxJKWcZnUxkZQ7ezsYznmrx9afXDxUIY13Mz/Photo%20from%20Library.jpeg)

### RTA

Calibration

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/F08FF15A-58B2-4AC8-8EBB-F9AC0F20703E_2/VOt6ZpTx0cTArpgi03eIuwjImV5SlSSMxkvSqyDrQYAz/Photo%20from%20Library.jpeg)

Before main

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/DDEDF2DD-CDBE-4992-94C0-CCAC74D1C505_2/MqsqPXwOi0q33vcooibtLWexvwMsxaCADYn1rORSkcQz/Photo%20from%20Library.jpeg)

During

![Photo from Library.jpeg](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/C8287570-DC09-4FCC-B31A-B83A51E76116_2/vHhoVwsqxBUlMyA9g9odJYiu44rdVbkNMrzS6I7T6ywz/Photo%20from%20Library.jpeg)

### Loss test

We use edfa 10x main setup at 1570. Input power is 76 mW

Normal RTA die 2

Straight 1

5.9 mW

Straight 2

6.7 mW

Straight 3

5.3 mW

Straight 4

5.2 mW

Straight 5

5.3 mW

Large circle

2.3 mW

Large square

2 mW

Medium square

0.7 mW (weird output shape)

Medium circle

Could not find (might have cleave by accident)

Got a bit dangerously close to the edge on the previous chip



Die 2 of normal RTA

Straight 1 

6.5 mW

Straight 2

5.6 mW

Straight 3

6.7 mW

Straight 4

5.2 mW

Medium square

2.8 mW

Medium circle

2.5 mW

Large circle

2.4 mW

Large square

Could not find



Tapered 3 um RTA

Straight 1

6.3 mW

Straight 2

4.5 mW

Straight 3

7 mW

Straight 4

5.3 mW

Euler

3.2 mW

Short circle

2.7 mW

Long circle

2.1 mW



Die 2

Straight 1

5.5 mW

Straight 2

5.1 mW

Straight 3

5.1 mW

Long wide adiabatic

4.9 mW

Short wide adiabatic 

4.1 mW

Long narrow adiabatic

2 mW

Short narrow adiabatic 

2.6 mW

Euler

3.4 mW

Short circle

3 mW

Long circle

2.3 mW



Tapered 2um RTA

Straight 1

6.5 mW

Straight 2

5.7 mW

Straight 3

5.4 mW

Straight 4

6.4 mW

Euler

3.3 mW

Long wide adiabatic

4.8 mW

Short wide adiabatic

5.6 mW

Long narrow adiabatic

4.6 mW

Short narrow adiabatic

Low

Short Circle

2.2 mW

Long circle

1 mW 



Die 2 (use middle one)

Straight 1

5.8 mW

Straight 2

5 mW

Straight 3

5.8 mW

Straight 4

4.8 mW

Long wide adiabatic

4.4 mW

Short wide adiabatic

5 mW

Long narrow adiabatic

4.3 mW

Short narrow adiabatic

4.8 mW

Euler

2.8 mW

Short circle

2.8 mW

Long circle

1 mW



Below are the results.  We are going to use the circular spirals to calculate the loss.  I am going to do the brute force calculation of the euler and adiabatic waveguide averages to get a sense of the variability there

Average Euler:
(2.8 + 3.3 + 3.4 + 3.2) / 4 = 3.2 mW.  Fairly consistent across waveguides, where the difference can be a bad job on my end of bad cleaving



Average Long Wide adiabatic

(4.4 + 4.8 + 4.9) / 3 = 4.7 mW

Average Short Wide adiabatic

(5 + 5.6 + 4.1) / 3 = 4.9 mW

Average Long Narrow adiabatic

(4.3 + 4.6 + 2) / 3 = 3.6 mW

Average Short Narrow adiabatic

(4.8 + 2.6) / 2 = 3.7 mW



While there are not perfect calculations, the rough guess is that the width of the waveguide matters a lot more than the period of the taper (at least at the moment).  So we can make the tapered regions a bit shorter.

Now lets calculate the loss of each of the structures:

Normal RTA

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/E7C2083C-AC6E-4634-8649-1802F8079EDD_2/88u77loEaU91eodbOPtxkLRxBpsluxKUqokmubmYkc0z/Image.png)

I just used the straight and long circle from both waveguide dies I tested

Tapered 3um using normal calculation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/990CA334-CB9E-4AD7-99D7-BB61B1840708_2/iN7blPDq6U3OOXNxcgqy4wGAoUGlVwRC5gUjbY7xwPMz/Image.png)

Roughly in agreement, so we know the 3um taper using this exposure process is roughly lossless

Tapered 2um using normal calculation

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/37E60243-F587-4D9D-A8A0-86DB8670A3C5_2/3V3mAgxt98kjfykgUSx6dur9JyMGZ9kXXZyScVTlyNwz/Image.png)

This case is a bit more tricky, as we do notice an increase (by quite a bit) for the loss from straight to spiral.  We see it a bit with 3um, but not as much.  Anyway, the key here is that we can now see the effect (which is decently substantial), from the taper.  With our lithography proceedure, we still expect that we have 2-2.5 um wide waveguide.  This is not that narrow, so I am not the happiest about this.  Lets try to redo the tapered calculations using the baseline loss from the 1 → 2 (which can treat the taper as some normal insertion loss).  We can guess the tapered region as roughly normal.

Using revised calculation method:

3um taper

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/CBFAFF27-F9E0-466A-9E8E-3F2053BD84A2_2/SdvZq5QN4zcRdwlYcrj3EuTgyvyOJ0ExPHLtOiDGipcz/Image.png)

2um taper

![Image.png](https://resv2.craft.do/user/full/c10b6666-b4fd-53a0-9177-1696a144b2d8/doc/052442E1-763A-4798-AA5D-A06F0C6B218D/291FB1D7-DBEA-4747-90A1-32791673BFF2_2/0uCpputyCZBBmHkGh7GfxmNjGxAaWrI6sbTb7CWutV4z/Image.png)

The taper length is probably causing a slight over estimate, as I am counting the full length of the tapered region plus the middle narrow region.  It is a lower bound for the loss in the narrow region, but it gives the useful impression.  It is nice to see that the losses for the linear regions are all incely in alignment.  It is also good that the 3um is roughly not noticing the narrowness.  But the 2um wide waveguides (which are in reality between 2 and 2.5 um because I am slightly underexposing).  