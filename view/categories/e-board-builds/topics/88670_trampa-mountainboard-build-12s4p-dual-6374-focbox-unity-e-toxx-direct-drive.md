# Trampa Mountainboard Build (12S4P, Dual 6374, Focbox Unity, E-toxx direct drive)

### Replies: 72 Views: 1350

## \#1 Posted by: RyuX Posted at: 2019-03-29T09:22:51.802Z Reads: 248

```
Hey Guys.

For those who seen my thread on the Evolve Bamboo GTX All Terrain and how I canceled my order to build my own mountainboard - this is the thread were I will document my progress.

So basically the Idea is a Trampa Board with the following setup:
1 x VERTIGO Mountainboard Deck with CNC lite 12mm HOLLOW Axle Trucks 
     - .
: 35º HOLYPRO Deck Shape 
     - .
: 16ply 35º HOLY PRO MTB - Stiff 
     - .
: WHITE Powdercoated with Blue logo VERTIGO Baseplate 
     - GREEN DAMPA's - 75a Firm Steering
     - Powder Coated BLUE Springs
     - .
: Please fit 5 Spoke SUPERSTAR Hubs 
     - .
: White Gloss Blue Logo Rim 
     - .
: BLUE Anodised Spokes 
     - .
: 8 Inch BLUE Primo ALPHA Tyres 
     - .
: BLUE ATB Bearings - 12mm Axles 
     - .
: RATCHET Style Bindings please 
     - White Strap with Blue Foam Footstraps 
     - WHITE with BLUE logo L-Brackets 
     - BLUE Powder Coated Ratchet Buckles 
     - .
: Heel Straps with BLUE Ratchets

From the Motor side I decided to go for 2x 6374 150KV from BioBoards.

I will use a FOCBOX Unity (once shipped) to drive those puppies.

My Battery Setup is a 12S4P (for now).
I designed the battery holders myself and printed them out on my 3D Printer - this gives stability and makes it a overall nice package.
Range is not my main focus - I want to see which range I can get on a 12S4P and later on if needed I will upgrade the parallel pair if the range is incredibly bad.
I use a 12S (80A-100A) BMS on this battery pack.

To round things of I decided to get a E-Toxx mini direct drive with helical gear setup.

Here are some photos for the start - will update them once there are news - and once again thanks for convincing me to cancel my Evolve Order and go DIY. I already have some experience from my other ESK8 Longboard Projects so this should be fun.

![20190327_125729|281x500](upload://1CX0w07CNF9MfgalDe0NG3P6eQQ.jpeg) ![20190327_125736|281x500](upload://afpTwq1CoYLsjfpQ63KZpK2JgQi.jpeg) ![20190327_163137|281x500](upload://pwxY2L1N0lsTT7JG3xQRDXO81DA.jpeg) ![20190327_163143|690x388](upload://nIkJ8dqSXUi7Krg26M0DCnspur0.jpeg) ![20190327_165053|690x388](upload://pO5fy4mBg6ulKKV6EOm47Xfq99y.jpeg) ![20190327_171557|690x388](upload://u5e3DNY59gcsgX6mWnNyO2dX0YE.jpeg) ![20190328_072504|690x388](upload://6fFub7OLBh6AqPlRrMiRfatN9zS.jpeg) ![20190328_072512|690x388](upload://7FZSVmkt7smCzQQYqP1YgQr6hWu.jpeg) ![20190328_183008|281x500](upload://u203zDI5uO6HERCzJV4LuQPlucX.jpeg) ![20190328_183020|281x500](upload://AefW85nOaF9Rl1ZUIrfu2ZF1cKF.jpeg) ![20190328_183030|281x500](upload://mdZu3MVbliOLpZE3W9nZzltSo6W.jpeg) ![20190328_202437|690x388](upload://mBtCPHdVI1M1jU7wysVF2qGydce.jpeg)
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-29T09:32:11.644Z Reads: 218

```
good decision!
do you have some pictures from the battery inside?
I´m interested how you connected the packs with each other.
Are those taps on the cells the stock taps you can order them with, or you welded them on by your own?
```

---
## \#3 Posted by: RyuX Posted at: 2019-03-29T10:40:16.073Z Reads: 217

```
Hey andy

I order them with the Tags from nkon.nl
every row of my holder has 8 batteries and there is a total of 6 rows (8x6 = 48 cells = 12s4p).
I connected 4 of them in parallel and then connected to the next pair of 4.
So it means each row has 2 parallel pairs.
For connecting the parallel pairs I used a thicker wire because the tag only would not have a desirable amp rating by itself.

So I just soldered the parallel pairs together with the tags. If you have a soldering iron that can get hot enough and you sand the tags a bit then it will hold up quite well.


Just don't want to invest in a spotwelder that I only use once every 2 years.

Have a good day

![image|672x500](upload://lBulPC05xoETD6W7kHLxet5h1pT.jpeg)
```

---
## \#4 Posted by: RyuX Posted at: 2019-03-29T13:12:01.224Z Reads: 194

```
Connected the BMS and tested the app.. looks good so far. Now waiting for the motors, direct drive and focbox to be shipped.![20190329_140859|281x500](upload://mjzvzhen9R9Qg8EAEmcpQdUz7Kt.jpeg) ![Screenshot_20190329-140838_xiaoxiang|281x500](upload://wTMj92e2e37YviyG9t0yZ4iseSZ.jpeg)
```

---
## \#5 Posted by: taz Posted at: 2019-03-29T14:13:28.323Z Reads: 182

```
That BMS is almost as big as the battery :rofl:
```

---
## \#6 Posted by: RyuX Posted at: 2019-03-29T14:15:14.142Z Reads: 176

```
size matters :smiley:
```

---
## \#7 Posted by: taz Posted at: 2019-03-29T14:17:19.939Z Reads: 175

```
Nonsense. I was told it was all about skill :rofl:
```

---
## \#8 Posted by: RyuX Posted at: 2019-03-29T14:18:36.414Z Reads: 176

```
Yes - it's also skilled :stuck_out_tongue:
I kinda like the approach with the bluetooth module and the app - it's really a good app as I use the same type on my longboard for over a year and it's flawless.
```

---
## \#9 Posted by: taz Posted at: 2019-03-29T14:23:33.912Z Reads: 179

```
I would kill for a charge only BMS with bluetooth that is also small.
The vesc takes care of the current and total voltage and if a p group has a problem I could get a notification on my phone.
Unfortunately the only one I know that fits these parameters is this one but I don't know how reliable it is.

https://www.lithiumbatterypcb.com/product/13s-48v-li-ion-battery-pcb-board-54-6v-lithium-bms-with-60a-discharge-current-for-electric-motorcycle-and-e-scooter-protection-2-2-3-2-2-2-2-2/
```

---
## \#10 Posted by: RyuX Posted at: 2019-03-29T14:25:59.877Z Reads: 173

```
Can't trust this tiny little bugger
```

---
## \#11 Posted by: taz Posted at: 2019-03-29T14:26:37.917Z Reads: 173

```
I meant charge only.
```

---
## \#12 Posted by: Ian-mountainboard Posted at: 2019-03-29T14:27:16.266Z Reads: 169

```
Do you not think that 4p will be underpowerd?
```

---
## \#13 Posted by: RyuX Posted at: 2019-03-29T14:28:31.883Z Reads: 167

```
Ah ok.. makes more sense now :slight_smile:
```

---
## \#14 Posted by: RyuX Posted at: 2019-03-29T14:29:11.823Z Reads: 168

```
I will find out - as I said I don't care much for range. In the worst case I  will add another 2P or 3P afterwards.
```

---
## \#15 Posted by: RyuX Posted at: 2019-03-29T14:36:59.643Z Reads: 155

```
I might wire my BMS to charge only as well. Will have to see how much amps it will use and then decide.
```

---
## \#16 Posted by: RyuX Posted at: 2019-03-29T14:48:28.349Z Reads: 163

```
Oh man.. what a setback.. seems my Focbox Unity will be the last part to arrive :frowning: 

![image|448x177](upload://mGnczMsPqglFs8fQRa0x436VHUM.png)
```

---
## \#17 Posted by: Andy87 Posted at: 2019-03-29T15:19:39.621Z Reads: 160

```
I have that one, but use only as external charge and to monitor the cell voltage.
What if you wire up balance wires out of the enclosure and use a lipo alarm instead?
You can still use this one for charge and monitoring and while driving you will get a notification if one cell goes bad.
```

---
## \#18 Posted by: taz Posted at: 2019-03-29T15:30:56.416Z Reads: 162

```
That is exactly what I (think I) wrote in my post :grinning:
```

---
## \#19 Posted by: RyuX Posted at: 2019-03-29T16:09:11.719Z Reads: 166

```
Finished my ghetto anti spark switch pcb that should be suitable for higher amps.
![20190329_170808|690x388](upload://gse4OyYtAZbuMWX3fqduIHXTJKD.jpeg)

Is a Anti Spark Switch recommended on a mountainboard or should I just go for a wired Loop Key ?
```

---
## \#20 Posted by: RyuX Posted at: 2019-03-29T18:07:05.206Z Reads: 164

```
I also would like to experiment with 63V Capacitors in parallel in a similar fashion to this PCB
(the pcb shown is a rectifier filter - however just to show that the plan is to have loads of caps on one pcb in parallel)

![image|411x285](upload://OCtLyRWzi60jNTKCRvQK4YCMa8.jpeg) 

50x pcs low esr 63V Caps have to help voltage sag.. just not sure if its worth my time.
Of course I would fuse this separate PCB in case any of those caps decides to short out.
```

---
## \#21 Posted by: Davide Posted at: 2019-03-29T19:09:18.422Z Reads: 153

```
Hey @RyuX! I’m curious about one thing, how can the solder tags last with all the A you are pulling in parallel? Are they pure nickel?
```

---
## \#22 Posted by: Davide Posted at: 2019-03-29T19:12:53.032Z Reads: 148

```
Nevermind 😅 you already wrote the anwer earlier
```

---
## \#23 Posted by: Eboosted Posted at: 2019-03-30T02:51:19.461Z Reads: 149

```
I'm glad you decide to cancel your Evolve, this is just much better choice overall, I know you can see it clearly now
```

---
## \#24 Posted by: RyuX Posted at: 2019-03-30T08:22:34.391Z Reads: 143

```
Yes I am glad that people made me aware of the fact that the evolve gtx is only a good board for people who can't build a DIY Board.

Honestly I had to take a lot more money into my hand now for this project but the outcome will be no comparison for sure and it will be my custom own :star_struck:
```

---
## \#25 Posted by: RyuX Posted at: 2019-03-30T08:23:36.424Z Reads: 141

```
Yes - I used some thick wire as well as the tags themselves. According to my calculation it should be good for 120A.

I have yet to decide if I will use the BMS for Discharge or only Charge operation but this will be shown in a comparison test I guess.
```

---
## \#26 Posted by: RyuX Posted at: 2019-04-04T19:02:12.207Z Reads: 136

```
Some progress this week.. 

![20190404_204958|281x500](upload://uPbxB6Rphe4jJ0Op0GG9TbqK0RF.jpeg) ![20190404_204936|281x500](upload://n5267JzsudCkychokDPQutTWRaJ.jpeg) ![20190403_163626|281x500](upload://zMYL1MhepT3IOET3IoUankoTw3f.jpeg) ![20190403_162906|281x500](upload://GpafVTmkfg3lrfX7DBWmfsgAo8.jpeg) ![20190404_204929|281x500](upload://48YEW97MEKLicvIzXCvKpaT9dOu.jpeg) ![20190403_073059|281x500](upload://6ZFYfqQ48rEkofcJCvOmXsiXVlA.jpeg) ![20190404_204925|281x500](upload://jHkntoDuAHoX7WNXiAtAg3BE8Cd.jpeg) ![20190404_194736|690x388](upload://oId5vooXcBXvEjRfPb5pcN4hvOo.jpeg) ![20190404_194251|690x388](upload://2GbsuiBMOK2n5MaNWEoWR7kedir.jpeg) ![20190403_163631|281x500](upload://6AOO1SBmW8oxtul11MxwwXQi9t2.jpeg) ![20190404_194732|690x388](upload://lMe98yE6AqMauzZZ8l0CQihuSLN.jpeg) ![20190404_194301|690x388](upload://5g5pp27S6Ns9jvEBWSflM8XAQEv.jpeg) ![20190404_194255|690x388](upload://eO0rvU6HN2AdDyNwTIXslI2OVcg.jpeg)
```

---
## \#27 Posted by: Saturn_Corp Posted at: 2019-04-04T20:29:51.999Z Reads: 124

```
I like those front lights. Will probably do something similar.
```

---
## \#28 Posted by: RyuX Posted at: 2019-04-05T04:04:59.613Z Reads: 123

```
I really like them.. they are rated 12-80V DC which is ideal for such projects
https://www.aliexpress.com/item/2Pcs-Lot-SUNKIA-U7-CREE-Chip-125w-Motorcycle-Projector-Headlight-3000LM-Motorbike-Head-Fog-Lamp-Angle/32699607864.html?spm=a2g0s.9042311.0.0.22554c4d1SgpOI
```

---
## \#29 Posted by: RyuX Posted at: 2019-04-05T11:29:17.354Z Reads: 121

```
Installed the voltmeter today. The e-toxx drive should arrive today so that's the next thing to do

![20190405_132323|281x500](upload://mgEQ4WfrMTzV3BJVSnX7Qo3ze2m.jpeg)
```

---
## \#30 Posted by: taz Posted at: 2019-04-05T11:43:43.741Z Reads: 111

```
They look nice. We will see how they stand up to the vibrations when used off road.
```

---
## \#31 Posted by: RyuX Posted at: 2019-04-05T11:48:15.435Z Reads: 111

```
yes will be interesting.. worst case I will help with a little hotglue here and there...
```

---
## \#32 Posted by: Sn4pz Posted at: 2019-04-05T12:04:11.683Z Reads: 111

```
[quote="RyuX, post:31, topic:88670"]
hotglue
[/quote]


Use silicone instead, its more resistant to cracking from vibrations :P
```

---
## \#33 Posted by: RyuX Posted at: 2019-04-05T12:29:02.628Z Reads: 109

```
I kinda like the "instant action" of hotglue and I despise waiting over 24hours for something so set :frowning:
```

---
## \#34 Posted by: RyuX Posted at: 2019-04-05T17:39:54.151Z Reads: 112

```
E-toxx assembly time..

![20190405_184051|281x500](upload://kfaFcZsPtGApwaSmBNSkd21a6BX.jpeg) ![20190405_185755|281x500](upload://83GfSkHr6Ox53uJBXbzp9zMJ2zl.jpeg) ![20190405_180854|281x500](upload://16OdHv2gJIn7R4zzVyHUN09ZC32.jpeg) ![20190405_181504|281x500](upload://1JT0hFiwK9WGOBhtKsmmNnT6toI.jpeg) ![20190405_190647|281x500](upload://uOpK6NLqGOLSCQV4DYj5VzvxR57.jpeg) ![20190405_190659|281x500](upload://9sVg4k0XbeUKWlxGgFcONaIDSXX.jpeg) ![20190405_185758|281x500](upload://yanhoHYGOE15WG8pnynQyToqS1I.jpeg) ![20190405_190418|281x500](upload://yjoZQuAiwAd9Roi4TbzDdVczUZu.jpeg) ![20190405_193705|281x500](upload://1CtfCvM9RnXl5LbsRyq8EnnbzRq.jpeg) ![20190405_192209|281x500](upload://aQhtnM0DooNSfZBW6g0aBug6rDl.jpeg) ![20190405_192212|281x500](upload://f3YkWF1RxEF6VIvz3RLDVAP3syn.jpeg) ![20190405_180227|281x500](upload://62To31305Rs5kHm3wuVH7ltCa7s.jpeg)
```

---
## \#35 Posted by: RyuX Posted at: 2019-04-06T06:54:23.617Z Reads: 106

```
Some more progress today. 

![20190406_085241|690x388](upload://slR9p1FE4z4P2NWOiMGwqXOLVYI.jpeg) ![20190406_085219|690x388](upload://9WxODZzmnW4MrnJqEeX9PhtZW1Z.jpeg)
![20190406_095429|281x500](upload://dSEgTjZsWo9BsgiYh7bV8CdYD56.jpeg)
```

---
## \#36 Posted by: Sn4pz Posted at: 2019-04-06T12:14:34.065Z Reads: 100

```
Loving the colour scheme :) 

Maybe blue motor wire sleeves in the future? ;)

I wish jenso would offer more colour options for the gear drives, it would open up alot of options for crazy looking builds
```

---
## \#37 Posted by: RyuX Posted at: 2019-04-06T13:04:22.903Z Reads: 97

```
Yes blue wire sleeves would have been nice - however I could nit find any - so next option would have been white - however white would look dirty after a couple of rides so I decided to go for the middle ground which is grey.
However If a matching blue sleeve will find it's way to me I might change it in the next revision
```

---
## \#38 Posted by: Sn4pz Posted at: 2019-04-06T13:05:23.591Z Reads: 95

```
Grey is still a good colour, it matches your hubs :) (they look grey? Gray? )
```

---
## \#39 Posted by: RyuX Posted at: 2019-04-06T13:17:46.501Z Reads: 95

```
Actually it's white - but my main focus was the blue/white color scheme... However it's impossible to have the same blue shade everywhere - as well as the exact same snow white so for some parts I have to make a compromise.

So only thing left is the unity focbox and the anti spark switch. However Enertion might only ship it sometime in May and shipping from Australia takes quite a while. Well enough time for other details in the meantime :slight_smile:
```

---
## \#40 Posted by: RyuX Posted at: 2019-04-06T13:37:52.739Z Reads: 101

```
Some cable management

![image|675x500](upload://u0cIFzsqft3T1B1x34oBGZO1INe.png)

![20190406_153700|281x500](upload://3BYhwT0I9UwjUHQk5IGcjf4QfX7.jpeg)
```

---
## \#41 Posted by: RyuX Posted at: 2019-04-06T14:31:13.693Z Reads: 101

```
Or better on the bottom

![20190406_163039|281x500](upload://d6xJQhiK3yLNrlh336h2YHNis4J.jpeg) ![20190406_163046|690x388](upload://lvE1RSBdoMNUSWJJM2I1c16yWWB.jpeg)
```

---
## \#42 Posted by: taz Posted at: 2019-04-06T15:43:58.494Z Reads: 98

```
You don't want any of these on the bottom 

![20190403_184744|375x500](upload://6lyGJghnjkXxziInFJL9vPqBFqS.jpeg)
```

---
## \#43 Posted by: RyuX Posted at: 2019-04-06T15:54:28.341Z Reads: 96

```
Damn... it would look so good though :frowning:
Maybe I will build a protection around it
```

---
## \#44 Posted by: RyuX Posted at: 2019-04-06T17:27:17.768Z Reads: 97

```
Cheeking the flex.. the board feels great

![20190406_192532|690x388](upload://lF0GDAxs2UZYZM5tLNAaNcHnrRy.jpeg)
```

---
## \#45 Posted by: taz Posted at: 2019-04-06T17:42:45.858Z Reads: 96

```
You are going to have a blast on that board.
```

---
## \#46 Posted by: RyuX Posted at: 2019-04-06T19:00:25.016Z Reads: 92

```
hope so! however the wait will be hard.. 

One quick question - I have the standard ratchet bindings and decided to add the trampa heel straps to it.. is it even needed or recommended or do you guys ride without heel straps ?
```

---
## \#47 Posted by: Nowind Posted at: 2019-04-06T19:04:37.279Z Reads: 94

```
Nice Colour theme Bro :star_struck:
```

---
## \#48 Posted by: FredrikHems Posted at: 2019-04-06T19:12:10.841Z Reads: 88

```
If you plan on jumping, heel staps are IMO essensial. You will have much better control of the board when offroad aswell.
```

---
## \#49 Posted by: taz Posted at: 2019-04-06T19:16:03.869Z Reads: 89

```
Also if a foot slips out of a binder say goodbye to your knees. Always heel straps off road.
```

---
## \#50 Posted by: Andy87 Posted at: 2019-04-06T19:36:31.753Z Reads: 88

```
Maybe it just looks like in the picture, but do you stand on the board with not inflated tires?
If yes, take care you can damage the inner tube like that. If you inflate them thsn just on the day when you want to drive first time and you directly have a flat tire, that sucks.
```

---
## \#51 Posted by: RyuX Posted at: 2019-04-06T19:39:26.145Z Reads: 82

```
When doing the E-Toxx assembly you have to open up the hubs/tires - I just didn't have a pump to fill them up again :) I won't ride it before I get my Unity Focbox so I have another 2-3 months :open_mouth:
```

---
## \#52 Posted by: Andy87 Posted at: 2019-04-06T19:45:44.282Z Reads: 82

```
I‘m sure you will not ride it like this 😅 but already standing on it like this can damage the inner tube. Just wanted to mention that. I hope in general you ordered some spare tubes and wheels as well. The need of a new one can come faster than you imagine sometimes 😬😂
Don’t ask from where I know it 😂
```

---
## \#53 Posted by: DEEIF Posted at: 2019-04-06T19:47:45.334Z Reads: 84

```
Mind if I ask you what the total price will/is?
```

---
## \#54 Posted by: RyuX Posted at: 2019-04-06T19:47:47.904Z Reads: 85

```
they are so fragile :O ?
Is there a cheap/reliable source to order them from ?
```

---
## \#55 Posted by: RyuX Posted at: 2019-04-06T19:48:11.564Z Reads: 87

```
2400 € if everything works out
```

---
## \#56 Posted by: taz Posted at: 2019-04-06T19:51:52.987Z Reads: 90

```
Get this pump. It is small enough to carry it with you.

https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F322940524745
```

---
## \#57 Posted by: RyuX Posted at: 2019-04-06T19:54:38.398Z Reads: 91

```
ordered... :blush:
```

---
## \#58 Posted by: Andy87 Posted at: 2019-04-06T19:56:45.328Z Reads: 91

```
You never know what you hit on the road.
If you don’t take care during assembly you can also cut the inner tube with the hub parts etc. Million was to get a flat tire.

[quote="RyuX, post:54, topic:88670"]
Is there a cheap/reliable
[/quote]

yes there is 
https://www.aliexpress.com/item/32933085940/32933085940.html?
```

---
## \#59 Posted by: RyuX Posted at: 2019-04-06T21:53:02.958Z Reads: 89

```
thanks.. ordered some spares..
```

---
## \#60 Posted by: RyuX Posted at: 2019-04-07T09:06:04.702Z Reads: 86

```
Still thinking about if my 80A (continous) BMS is good enough or if I should only use the BMS for Charging... Any thoughts ?

BMS is for 12S 80A (continous) and 160A Overcurrent protected.
```

---
## \#61 Posted by: taz Posted at: 2019-04-07T12:26:31.764Z Reads: 85

```
I don't have data from my Trampa but in my Evo with 2x 6374 Maytech motors I have never drawn 80A according to metr . My max battery draw has been around 70-75A and that only lasted seconds. Motor amps on the other hand are another story. Whatever I set the maximum, I reach.

My guess is you will be fine.
```

---
## \#62 Posted by: RyuX Posted at: 2019-04-07T13:36:25.232Z Reads: 81

```
Great.. thought so as well.. with my current Longboard Project I can barely hit 35A with one 6384 Motor so I figured the 80A BMS should be good for 2x 6374.
```

---
## \#63 Posted by: RyuX Posted at: 2019-04-07T13:48:26.341Z Reads: 83

```
Just went to the Gas Station and gave my Tires a good 40PSI wellness treatment and seems all of them are still ok and well :smiley:
```

---
## \#64 Posted by: RyuX Posted at: 2019-04-09T16:51:10.138Z Reads: 80

```
Some pictures.
I put some grip tape underneath the enclosure and strapped it down with two straps.. seems quite stable.

Also put some loctite on my pretty loose bearings, wonder if all Trampa boards have this problem?

![20190409_184438|690x388](upload://8IMvllR3VUODjmJUlqGxA1qJkIY.jpeg) ![20190409_184509|690x388](upload://p3YjzrZBDeDNsctBlGQHwv6jzNV.jpeg) ![20190409_184446|690x388](upload://jwSEhlby13QWiVe4945xz1sXV8h.jpeg) ![20190409_184457|690x388](upload://lzNSKyLrmiXeoBLazGpYQstnUQY.jpeg)
```

---
## \#65 Posted by: RyuX Posted at: 2019-04-11T07:01:24.209Z Reads: 73

```
Trying to slim down the enclosure.. can fit battery and anti spark switch into one enclosure and will make a separate one for the focbox

![20190410_175410|281x500](upload://a9gDFmbOGV6dAlaJ7uENc1sAn3r.jpeg) ![20190410_175413|281x500](upload://shm0O2MBwLRZpRzMUm7mK7mpw26.jpeg) ![20190410_184207|690x388](upload://ccWqtXYNFqbhLCubfp3WK4gytJF.jpeg) ![20190410_194603|281x500](upload://qcSNS6kZZJZysjvCQv9apLl91UZ.jpeg) ![20190410_183226|281x500](upload://dSWUaam3XG93NAeAgvrPDLgyq8I.jpeg) ![20190410_183912|281x500](upload://4xJRVWbqlzvWUiMrW6Ta2w0Wk9u.jpeg) ![20190410_194611|281x500](upload://tZw7cUefFKan2skUqLyFbT9Knbr.jpeg)
```

---
## \#66 Posted by: RyuX Posted at: 2019-04-12T15:10:13.265Z Reads: 65

```
Prepared all the cables for the smaller vesc case that should arrive next week. Quite happy with the overall size reduction even though it makes wiring and fitting quite a task, but since I have some extra time until the focbox unity gets shipped I am just fine with that.


![20190412_121731|281x500](upload://d2dh72mibJXOwpSiYoWzQ8ErHbx.jpeg)

![image|690x347](upload://cJFB4KDTuy8z9XjelF7LvUi4cD8.jpeg)
```

---
## \#67 Posted by: Nemesis Posted at: 2019-04-12T17:04:38.462Z Reads: 63

```
I use the same case/box for my tail mounted Escapes its a bit smaller than the 206 ultrabox and way cheaper.

![finished|375x500](upload://jXd660s3p4LHmC1FFzgb9K21o00.jpeg) 
![finished2|666x500](upload://1EBezCx9w0cAqWE9J5ThoabmOdJ.jpeg) 

Very nice build by the way.... :+1:
```

---
## \#68 Posted by: RyuX Posted at: 2019-04-12T17:12:40.982Z Reads: 60

```
Thanks... your build looks sick as hell too !
Cool to see others used the same case.

I kinda came to the conclusion there is no logical way around two separate boxes if you want to have a nice clean compact build.
```

---
## \#69 Posted by: banjaxxed Posted at: 2019-04-15T03:01:05.453Z Reads: 60

```
Do you have a cad for the mount for the Sunkia lights, tight build bro
```

---
## \#70 Posted by: RyuX Posted at: 2019-04-15T04:12:57.341Z Reads: 57

```
I used the mount that was included with the lights.. With some bending I was able to fit it on the trucks.
Not sure about how stable they are once I get going with the board - but this has to be tested :slight_smile:
```

---
## \#71 Posted by: banjaxxed Posted at: 2019-04-15T06:04:05.969Z Reads: 55

```
Even better! They are like handlebar mounts, that could suit MBS
```

---
## \#72 Posted by: RyuX Posted at: 2019-04-17T16:43:39.413Z Reads: 51

```
Small update. Got my focbox case and installed the wires already. Have to go on a business trip and will hopefully get the focbox when returning and finishing this thing up.

![20190417_183910|690x388](upload://msOU0oNomBCcMtFzxFE3MhHsWyQ.jpeg) ![20190417_183907|690x388](upload://9TaNbsxmsniGhCsuZEbBfLG5cxQ.jpeg) ![20190417_183901|281x500](upload://he1Anq08SevqcBtIzeSEjd86OyG.jpeg)
```

---
