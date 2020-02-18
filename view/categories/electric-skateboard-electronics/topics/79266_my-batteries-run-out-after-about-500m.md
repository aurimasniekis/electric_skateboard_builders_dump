# My batteries run out after about 500m

### Replies: 114 Views: 1112

## \#1 Posted by: FirstTimeBuilder Posted at: 2018-12-28T21:56:48.514Z Reads: 286

```
Hey everyone, 

Firstly like to introduce myself, im Jake and im new to e-boards but im a maker so i decided to build a custom board. 

The board is built and works great but the issue im having is that the batteries run out after only like 500m of riding, basically to the end of my road and back a couple of times. 

I have dual motor and using the followowing

Motors
https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html

Batteries
https://hobbyking.com/en_us/multistar-high-capacity-5200mah-4s-12c-multi-rotor-lipo-pack-w-xt60.html

Vesc
https://flipsky.net/products/torque-esc-vesc-%C2%AE-bldc-electronic-speed-controller

I'm new to the setup of the motors so any advice on what the parameters should be.

Pretty straight forward setup, 

batteries to vesc's via diy antispark switch to motors

Thanks for your help in advance
```

---
## \#2 Posted by: AlanZhou Posted at: 2018-12-28T22:01:59.524Z Reads: 260

```
Did you configure the battery settings on the vesc??
Like the throttle voltage and the cutoff voltage??
```

---
## \#3 Posted by: dareno Posted at: 2018-12-28T22:07:54.074Z Reads: 259

```
How many of those lipos do you have and whats the configuration?
```

---
## \#4 Posted by: FirstTimeBuilder Posted at: 2018-12-28T22:15:18.655Z Reads: 262

```
Hey both,

Yes configured using the setup wizards on the vesc tool. I have two of these lipos in series
```

---
## \#5 Posted by: AlanZhou Posted at: 2018-12-28T22:19:40.468Z Reads: 256

```
So you have 8s and so you cutoff voltage should be 24v (lipos cannot dip below 3v per cell so 3x8= 24v)

And your throttle voltage should be 25.6v (your performance should start to decrease at 3.2v per cell)
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-12-28T22:44:53.415Z Reads: 238

```
Never set lipo cut off at 3v/cell. Use 3.6 as minimum or they will start puffing uneccesary fast.
```

---
## \#7 Posted by: AlanZhou Posted at: 2018-12-28T22:47:12.376Z Reads: 224

```
You know that 3.7v is nominal of lipos right, lipos only become damaged below 3.0v

Lipos are basically lions but in a pouch
```

---
## \#8 Posted by: FredrikHems Posted at: 2018-12-28T22:49:17.096Z Reads: 214

```
You know that lipos shouldnt be discharged more than 80% of full capacity? 80 % is 3.6-3.7v/cell depending.
```

---
## \#9 Posted by: AlanZhou Posted at: 2018-12-28T22:49:41.111Z Reads: 211

```
The main reasons lipos start puffing is because their only rated at 200 discharges/charges and higer end lipos like turning graphine can match 18650
```

---
## \#10 Posted by: AlanZhou Posted at: 2018-12-28T22:50:04.814Z Reads: 206

```
You can go on any rc fourm and they know it best 3.0v is ok and it's fine
```

---
## \#11 Posted by: AlanZhou Posted at: 2018-12-28T22:52:46.366Z Reads: 199

```
Edit.
10 char

Just search up max lipo discharge voltage

Also I think what you mean is that a lipo should not be at 3.3v under load to avoid damage

If you worried than set the throttle voltage to 3.5v
```

---
## \#12 Posted by: FredrikHems Posted at: 2018-12-28T22:55:57.716Z Reads: 190

```
Been doing rc stuff for 10 years. Ask a trusted lipo user around here and ask them if 3v/cell is good for longevity or not. As said earlier, 3.6-3.7v/cell is optimal for longevity. 3v/cell is way to low especially for hobbyking lipos..
```

---
## \#13 Posted by: AlanZhou Posted at: 2018-12-28T22:57:08.631Z Reads: 190

```
A lipo can stay at 3v without issue but it cannot be under load at 3.3v I think that's what you mean I would stop flying at 3.2v usually

3v for not a long time like a week

That's why I said set battery cutoff at 3v and throttle at 3.2v but if you want to be safe set it to 3.5v so the vesc would ramp down amperage
```

---
## \#14 Posted by: FredrikHems Posted at: 2018-12-28T22:59:22.663Z Reads: 182

```
Well when riding a board, the batteries are cleary under load. The board wont cut out before 3v/cell with the settings you suggested, and by then the lipos would be damaged.
```

---
## \#15 Posted by: AlanZhou Posted at: 2018-12-28T23:00:52.641Z Reads: 178

```
If you set it to 3.5v the vesc will ramp down aclearation as I said and theirfore the battery won't be at full load

**_The plates of lithium won't be damaged untill below 3v_** this is the point that I'm trying to get across

Sry not good at udeing the correct terms
```

---
## \#16 Posted by: AlanZhou Posted at: 2018-12-28T23:04:45.799Z Reads: 175

```
The battery he states might be a issue it's only rated for 62a and turnigy usually overrated their battery, would recommend 20c at least and 30c to be safe
```

---
## \#17 Posted by: FredrikHems Posted at: 2018-12-28T23:05:39.473Z Reads: 171

```
Well you wrote 3.2v for cut-off start, and 3v for cut-off end earlier. Even if the load isnt at max, there clearly is a load. Sure that the lipos **Shouldnt** be damaged before 3v **in theory**, but I am talking from real life knowledge of hobbyking lipos.
```

---
## \#18 Posted by: AlanZhou Posted at: 2018-12-28T23:06:52.491Z Reads: 169

```
My lipo is over a year and a half old, cutoff is alawys 3.0v with zero issues, it's s bit puffed but Its to be expected from a year and a half old lipo

Also charged at 1c the whole time

But my point was lipos won't be damaged untill 3.0v and I'm outta here
```

---
## \#19 Posted by: FredrikHems Posted at: 2018-12-28T23:10:29.076Z Reads: 161

```
I dont know man.. You keep changing between 3v hard/3.2v soft cut-off, and 3.2v hard/3.5 soft cut-off. Either way, you are talking theory, I am talking real life experience.
```

---
## \#20 Posted by: AlanZhou Posted at: 2018-12-28T23:11:00.212Z Reads: 158

```
Some of them were examples some of the I explicitly said if you want to be safe

Quotes " I'm s talking theory"

Even though I have a lipo in s board that's a year and a half old
```

---
## \#21 Posted by: Erniechan Posted at: 2018-12-28T23:11:12.270Z Reads: 154

```
Lipo gets damaged beyond 2.7v point of no return. Permanent damage. You can use It to 3.3 or even 3v. Longevity is highly increased if you discharge to 3.7v but lipo has a short lifespan anyway. Long life or long range .... Pick up a choice. The best choice is 3.7 but there's nothing wrong on using them beyond that.
```

---
## \#22 Posted by: dareno Posted at: 2018-12-28T23:12:48.071Z Reads: 143

```
I used to set my lipo cut off to 3.0v when I was racing because I didn't care about the packs if it meant I won.  Killed plenty of packs in my unsolicited attempts at glory.  Didn't win much either.  12 c is a bit low is it not for esk8?
```

---
## \#23 Posted by: AlanZhou Posted at: 2018-12-28T23:13:47.299Z Reads: 140

```
It seems most of us are fpv racers? What's your best ever top speed?
```

---
## \#24 Posted by: FredrikHems Posted at: 2018-12-28T23:17:28.890Z Reads: 134

```
Exactly. 3v/cell is way to low if you want to keep your lipos. Maybe the high-end lipos can handle it, but I can for sure say that cheap lipos of hobbyking definetly cant. Also. There is so little capacity to gain between 3.6v and 3v, that it makes abseloutely zero sense to risk brand new lipos for maybe 5% more capacity..
```

---
## \#25 Posted by: dareno Posted at: 2018-12-28T23:22:54.774Z Reads: 125

```
Cars dude.  Forayed into drone racing but it was too expensive (I crashed a lot) so I moved into this cheap alternative.
```

---
## \#26 Posted by: AlanZhou Posted at: 2018-12-28T23:23:10.293Z Reads: 124

```
Graphine should handle it but don't quote me never used them before, my motto was alawys buy cheap turnigy lipos use them for mabye a few times and toss em
```

---
## \#27 Posted by: AlanZhou Posted at: 2018-12-28T23:23:46.943Z Reads: 125

```
Damn the struggle is real but even if you crashed the car and the lipo Went for a nosedive it would still go poof anyways
```

---
## \#28 Posted by: Erniechan Posted at: 2018-12-28T23:25:49.881Z Reads: 127

```
You are right but i think wrong numbers. The discharge curve drops at 3.3v so i think 3.7 to 3v 5%+ capacity is underrated
```

---
## \#29 Posted by: dareno Posted at: 2018-12-28T23:26:54.895Z Reads: 130

```
One of my 3.0v forays ended up in a flaming finish line crossing.  Killed a very expensive set up.
I had a 6s truck short and implode during a bash session and it was this reason I went with li ion for esk8.
```

---
## \#30 Posted by: FredrikHems Posted at: 2018-12-28T23:26:57.119Z Reads: 130

```
Graphenes should be better, however I wouldnt trust them to 3v/cell. Might be better than the standard ones, but graphenes are also way more expensive to fuck up.
```

---
## \#31 Posted by: AlanZhou Posted at: 2018-12-28T23:27:57.392Z Reads: 128

```
What you mean is too expensive to f up and not more expensive to f up
```

---
## \#32 Posted by: AlanZhou Posted at: 2018-12-28T23:28:29.826Z Reads: 125

```
Or you could've gone gas if that was legal near you lol.

Alright stop hijacking this poor man's thread
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-12-28T23:29:12.146Z Reads: 125

```
I cant say for all lipos, but for a pair of mine turnigy flightmax its pretty accurate. Its for 3.6-3.5 to 3v though, not 3.7.
```

---
## \#34 Posted by: AlanZhou Posted at: 2018-12-28T23:32:45.540Z Reads: 122

```
Flightmax Is made by zippy btw
```

---
## \#35 Posted by: FredrikHems Posted at: 2018-12-28T23:38:13.385Z Reads: 121

```
You are right, its late here. Both made/sold by hobbyking tho
```

---
## \#36 Posted by: anorak234 Posted at: 2018-12-29T00:07:09.862Z Reads: 115

```
[quote="AlanZhou, post:7, topic:79266"]
Lipos are basically lions but in a pouch
[/quote]

Umm... no. It’s a different battery chemistry which is substantially more volatile. It’s best to treat them like you would a bomb - set that cutoff voltage at 3.6/cell
```

---
## \#37 Posted by: AlanZhou Posted at: 2018-12-29T00:07:45.067Z Reads: 114

```
Well there basically the same there basically cousin's

18650 can be just as dangerous as lipos, lipos puff and smoke but 18650 explode like grenades if the case is bad because 18650 don't have space to expand

Just treat all lithium products with catuation
```

---
## \#38 Posted by: anorak234 Posted at: 2018-12-29T00:10:58.146Z Reads: 119

```
Sure, they’re cousins. But cousins are not the same. And for the longevity of the battery itself and future safety it’s best to charge and discharge within the range of 3.6 to 4.2 volts. With li-ion you can get away with a bit more, but it’s still a negative outcome in the long run when your batteries die early. 

Again, lipos are substantially more dangerous and should be treated as such. This whole discussion is off topic.

@FirstTimeBuilder, multi star lipos have a bad reputation for lower discharge capability than advertised, and that’s probably why they run out so quickly. I highly advise buying graphene lipos or 30Q Lithium ion batteries.
```

---
## \#39 Posted by: AlanZhou Posted at: 2018-12-29T00:11:37.555Z Reads: 117

```
And yet so many things used lipos without issues. 
Sry.
```

---
## \#40 Posted by: dareno Posted at: 2018-12-29T00:25:25.439Z Reads: 116

```
Don't you dare talk back to your mother young man!!
```

---
## \#41 Posted by: AlanZhou Posted at: 2018-12-29T00:26:27.240Z Reads: 109

```
Ughhhhhhh, silence
```

---
## \#42 Posted by: J0ker3366 Posted at: 2018-12-29T04:01:00.929Z Reads: 111

```
[quote="FredrikHems, post:12, topic:79266"]
Ask a trusted lipo user around here
[/quote]
NEVER "RUN" (meaning under load) LIPOS LOWER THAN 3.5V A CELL!  

Whatever rc forum you're on and whoever is claiming to be a "lipo god" (@Andy87 hehe) and tell you 3v is fine, is a fucking idiot and wants you to cause damage to your batteries.

There. You heard it from a lipo god that 3.5v is the absolute lowest you should ever rn a cell in any S lipo.

Edit: you also have to understand, there's is a big difference in rc and esk8. We draw a hell of a lot more power. We do way more damage to any lipo or li ion. We demand power and we snatch it from batteries. Rc doesnt need to do that. So running lipos lower in rc is understandable.
```

---
## \#43 Posted by: rich Posted at: 2018-12-29T04:06:34.589Z Reads: 106

```
[quote="FirstTimeBuilder, post:1, topic:79266"]
run out after only like 500m
[/quote]

Back to topic, my bet is that you set too high cut off values, what's your soft and hard cut off setting for 8s?
Stupid question but did you charge the batteries? :laughing:

[quote="FredrikHems, post:6, topic:79266, full:true"]
Never set lipo cut off at 3v/cell. Use 3.6 as minimum or they will start puffing uneccesary fast.
[/quote]

I can fully agree. All my Graphene Lipos puffed within less than 50 charge cycles because I drained them down to 3.2V per cell regurlarly. Now I finish at 3.5-3.7V per cell. My cut offs are set at 3.5V/3.3V but I only use the last energy to get my ass home in case I'm only 200m far away.

Another story, once I forgot to power off the board and the 10s pack decreased from 32V to 11.8V within 28 hours and the lipos are garbage.
```

---
## \#44 Posted by: dareno Posted at: 2018-12-29T04:06:52.172Z Reads: 103

```
[quote="J0ker3366, post:42, topic:79266"]
@Andy87   is a fucking idiot and wants you to cause damage to your batteries.
[/quote]

Bit rude.  Andy get him sunshine
```

---
## \#45 Posted by: Andy87 Posted at: 2018-12-29T04:41:57.525Z Reads: 98

```
Too early for this....
```

---
## \#46 Posted by: dareno Posted at: 2018-12-29T04:44:35.611Z Reads: 95

```
Not here its not.  :wink:
```

---
## \#47 Posted by: pat.speed Posted at: 2018-12-29T04:49:21.065Z Reads: 92

```
@J0ker3366 is right about he 3.6v cutoff, going lower is also asking for unbalanced cells and one being over discharged. Happened to me last week, don’t do it, stop at 3.6v with Lipo and 3v with Li-ion for the best longevity
```

---
## \#48 Posted by: Andy87 Posted at: 2018-12-29T04:50:50.408Z Reads: 91

```
@FirstTimeBuilder like @rich already said, double check first that your cut off voltage is set around 3.5V per cell (or 28V in total)
If those new cells they came with a storage voltage and you first need to charge them up.
I guess you did, but there have been done which didn’t do that and had the same issue than you, so I think it’s worth mentioning 😉

One last problem is, the multistar packs already rated not sufficient rated and tests in the past have proofed that the real rating of multistar lipos you use are around 4c what would be a max current of 20a or 10a per vesc you can run them on.
Sure you should get more than 500m out of them, but you really can’t expect much with this packs.

As you build a Mountain board i can just recommend to get the highest c-rated packs you can afford. If you have the money for it the graphens from hobbyking are probably the best you can get at the moment.
```

---
## \#49 Posted by: rich Posted at: 2018-12-29T05:01:39.164Z Reads: 91

```
@Andy87 are you human or robot?  It seeems like you never sleep :joy:

@FirstTimeBuilder just to explain what happens when reaching cut off limits (in case you don't know). When reaching the soft cut off the power gets limited but you can ride slowly, when reaching hard cut off... game over.
```

---
## \#50 Posted by: Andy87 Posted at: 2018-12-29T05:03:43.199Z Reads: 89

```
😅 i‘m on my way to work...
and here it’s already 8. the question is, what you doing up so early, or still up so late 😂
```

---
## \#51 Posted by: Namasaki Posted at: 2018-12-29T05:03:48.753Z Reads: 90

```
I would not run my Lipos down to 3.0v. 
I like to stop at 3.6v and if that doesn't get me far enough, then I need more capacity.

@FirstTimeBuilder  The reason your batteries are running out so fast is because of their specs.
5200/12C/8s
12C x 5.2ah is not gonna cut it on an esk8. The voltage sag will be enormous and especially at 8s.
If your gonna run low capacity Lipos, you need the highest C rating you can find. At least 60C and preferable higher like 90C. Then you will see a big difference. 

I'm running 10s 5ah 60C and I get around 12 miles with a dual setup and weighing 195lbs
```

---
## \#52 Posted by: pat.speed Posted at: 2018-12-29T05:17:22.842Z Reads: 89

```
The cells should atleast get him 4-5mi tho, he is getting 500m which is very short
```

---
## \#53 Posted by: Namasaki Posted at: 2018-12-29T05:26:25.056Z Reads: 88

```
I am not at all surprised that he is only getting 500m with those batteries.
Their true current max is probably less than 20a
```

---
## \#54 Posted by: pat.speed Posted at: 2018-12-29T05:31:18.369Z Reads: 87

```
Yes it probably is, but 500m is not just the batteries. Something else is not right here. 

I could get 500m using my drill battery to power my board

I’ve used 6s 5000mah 20c batteries before and gotten up to 10km on a charge
```

---
## \#55 Posted by: Namasaki Posted at: 2018-12-29T05:40:55.484Z Reads: 92

```
There could be more wrong than just the batteries.
But that is where I would start.
```

---
## \#56 Posted by: taz Posted at: 2018-12-29T08:01:51.451Z Reads: 97

```
[quote="J0ker3366, post:42, topic:79266"]
Edit: you also have to understand, there’s is a big difference in rc and esk8. We draw a hell of a lot more power. We do way more damage to any lipo or li ion. We demand power and we snatch it from batteries. Rc doesnt need to do that. So running lipos lower in rc is understandable.
[/quote]

Can't agree with you on this one.
This little birdie sucks through a pair of 6S 5000mAh Thunderpower packs in 6 minutes. Wanna see a graph with the current draw it takes to do that?

![20180215_185553|666x500](upload://3cfPVuXZdiHh9jaSw6g58ZwR00c.jpeg)
```

---
## \#57 Posted by: dareno Posted at: 2018-12-29T08:14:25.649Z Reads: 92

```
Yeah my e revo has a 150 amp esc.  It draws some nasty current.  Does 85mph  That chopper would smash the batteries.
```

---
## \#58 Posted by: J0ker3366 Posted at: 2018-12-29T08:22:42.749Z Reads: 92

```
That thing I don't doubt draws a shit ton lol. Got any videos of you flying it?

Also I redact that quote lol
```

---
## \#59 Posted by: taz Posted at: 2018-12-29T08:33:00.768Z Reads: 98

```
I fly alone so there is nobody to film me.
I only have a couple of very old videos when a friend came with me. I was not very good at the time so please be gentle :smiley:.

https://youtu.be/fZ_80rjsLe0

https://youtu.be/72h0M_KnASw
```

---
## \#60 Posted by: J0ker3366 Posted at: 2018-12-29T09:25:30.574Z Reads: 91

```
Bruv I couldn't even take off without crashing lol.
```

---
## \#61 Posted by: taz Posted at: 2018-12-29T09:53:55.358Z Reads: 83

```
Yeah, RC helis have the steepest learning curve of everything I have tried.
```

---
## \#62 Posted by: totalgeek9224 Posted at: 2018-12-29T10:13:43.340Z Reads: 84

```
[quote="taz, post:59, topic:79266"]
I was not very good at the time so please be gentle :smiley:.
[/quote]

**proceeds to do multiple barrel rolls**
```

---
## \#63 Posted by: taz Posted at: 2018-12-29T10:28:45.483Z Reads: 84

```
Lol, you guys give me too much credit.
Here is someone who knows how to fly RC helicopters :sunglasses:

https://youtu.be/pCrhPUL20vk
```

---
## \#64 Posted by: totalgeek9224 Posted at: 2018-12-29T10:30:16.987Z Reads: 82

```
Looks like a glitch in the Matrix
```

---
## \#65 Posted by: taz Posted at: 2018-12-29T10:31:35.187Z Reads: 84

```
When Tareq flies, the Matrix reboots
```

---
## \#66 Posted by: FirstTimeBuilder Posted at: 2018-12-29T12:00:39.311Z Reads: 84

```
Hey, wow, i feel we've gone slightly of topic. So in short i need better batteries? or do i just need to change my settings? 

Thanks
```

---
## \#67 Posted by: Andy87 Posted at: 2018-12-29T12:15:21.797Z Reads: 82

```
you need to check your settings (cut off) and charge your packs eventually :sweat_smile:
and other packs would be good too :stuck_out_tongue_winking_eye:
```

---
## \#68 Posted by: pat.speed Posted at: 2018-12-29T12:54:06.186Z Reads: 79

```
Start with your settings and cutoffs if it doesn’t improve then check battery capacity. Then get new ones if it’s got the correct capacity as stated on the lipo
```

---
## \#70 Posted by: jadatmag Posted at: 2018-12-29T15:57:30.675Z Reads: 76

```
[quote="J0ker3366, post:42, topic:79266"]
you also have to understand, there’s is a big difference in rc and esk8. We draw a hell of a lot more power. We do way more damage to any lipo or li ion. We demand power and we snatch it from batteries. Rc doesnt need to do that. So running lipos lower in rc is understandable.
[/quote]

Sorry but I got triggered here :grin:

A [small quadcopter](https://www.banggood.com/Eachine-Wizard-TS215-215mm-FPV-Racing-RC-Drone-F4-5_8G-72CH-40A-BLHeli_32-720P-DVR-1200TVL-BNF-PNP-p-1259022.html?rmmds=search) can output 4x 40amps @ 4/5s. Please find me a 1200 mah battery that can sustain 160 amps :sunglasses:
```

---
## \#71 Posted by: AlanZhou Posted at: 2018-12-29T16:02:27.541Z Reads: 74

```
Agreed lol you can count any quad as a 4wd basically because it is
```

---
## \#72 Posted by: jadatmag Posted at: 2018-12-29T16:04:47.494Z Reads: 73

```
Puffing is the name of the game. I think the average race battery lasts 0 real deal races. It's puffed before the end of the race.
```

---
## \#73 Posted by: rich Posted at: 2018-12-29T16:19:06.547Z Reads: 73

```
[quote="FirstTimeBuilder, post:66, topic:79266"]
we’ve gone slightly of topic
[/quote]

We :joy:?

You don't answer any question dude! It seems you don't want to solve the issue.

BTW this is no answer: 

[quote="FirstTimeBuilder, post:4, topic:79266"]
Yes configured using the setup wizards
[/quote]

We don't have more input from you. This thread has 73 posts up to now and 3 are from you :thinking: and we still know nothing...
```

---
## \#74 Posted by: Sebike Posted at: 2018-12-29T16:47:18.340Z Reads: 67

```
Just to make it clear to you;
 
We still don't know your settings.
What are your voltage cutoffs? 

Post screenshots of your vesc settings!
Pictures and a diagram of your wiring setup would help as well.
```

---
## \#75 Posted by: FirstTimeBuilder Posted at: 2018-12-29T19:09:12.301Z Reads: 66

```
@rich

I agree that ive only posted 3 times but if you look at the thread around 65 of the posts are of people arguing about 3v or 3.6v and then talking about flying RC helicopters. 

Im getting the board back out in about an hour so will post some settings. Like i said, im very new to this as in my fist time building a board so even using the vesc tool is a maze to me.
```

---
## \#76 Posted by: FredrikHems Posted at: 2018-12-29T19:13:30.227Z Reads: 63

```
Well the arguing about lipo voltage is very relevant to your question, so I dont see that as «off-topic». The heli and rc post’s is another story tho..
```

---
## \#77 Posted by: FirstTimeBuilder Posted at: 2018-12-29T19:18:34.749Z Reads: 64

```
oh i agree about the lipo part but there isnt much i can input to that which is why i didnt post anything. Let you guys argue it out between you lol
```

---
## \#78 Posted by: rich Posted at: 2018-12-29T19:33:37.151Z Reads: 70

```
Connect the master vesc to pc and open Vesc-Tool
Motor Settings/General/Voltage here you see the cut offs (in this case 3.6V/3.4V for 8s).

![8s|690x401](upload://s1vvb9EfOgtTX0uIL5j6hmD6rAA.png)
```

---
## \#79 Posted by: dareno Posted at: 2018-12-29T19:43:19.364Z Reads: 70

```
[quote="FirstTimeBuilder, post:75, topic:79266"]
but if you look at the thread around 65 of the posts are of people arguing about 3v or 3.6v and then talking about flying RC helicopters.
[/quote]

Welcome to the forum my friend.
```

---
## \#80 Posted by: FirstTimeBuilder Posted at: 2018-12-29T20:39:09.714Z Reads: 69

```
Ok, 

I think i know what the issue is, the batteries are dodgy, One now wont charge and the other is coming up as 3s not 4s on the charger.
```

---
## \#81 Posted by: Andy87 Posted at: 2018-12-29T20:45:41.442Z Reads: 70

```
Sounds like you already over discharged them last time.
```

---
## \#82 Posted by: Sn4pz Posted at: 2018-12-29T20:51:13.351Z Reads: 70

```
please read up on the dangers of attempting to recharge fukt lipo cells before you attempt anything.... The risks outweigh the benefits
```

---
## \#83 Posted by: FirstTimeBuilder Posted at: 2018-12-29T20:57:00.486Z Reads: 72

```
So ive been looking on Hobbyking and have found these which are in my price range. 

https://hobbyking.com/en_us/5600mah-7-4v-70c-lipo-car-pack-2s2p.html

or these but im not sure if i can stretch that far for two.

https://hobbyking.com/en_us/turnigy-graphene-5000mah-4s-75c-lipo-pack-w-xt90.html
```

---
## \#84 Posted by: AlanZhou Posted at: 2018-12-29T20:58:15.751Z Reads: 69

```
Definitely get the graphine

Or this might be good enough.
https://hobbyking.com/en_us/turnigy-heavy-duty-5000mah-4s-60c-lipo-pack-w-xt-90.html
```

---
## \#85 Posted by: FirstTimeBuilder Posted at: 2018-12-29T21:23:37.157Z Reads: 66

```
Thanks guys, am in contact with hobbyking so will be back with an update with what im going to do but thanks for your help so far.

Thanks
```

---
## \#86 Posted by: FirstTimeBuilder Posted at: 2019-01-15T15:45:12.215Z Reads: 61

```
Hey guys, 

So bit of an update, i went out and bought new batteries. I went with these
https://hobbyking.com/en_us/turnigy-graphene-5000mah-4s-75c-lipo-pack-w-xt90.html

I then got an itch to buy different motors so went and bought these
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

So now im back to the setup of them. My questions is whats the cutoff start and end that i should be setting these too so i dont cock them up?

Thanks in advance
```

---
## \#87 Posted by: Indiangummy Posted at: 2019-01-15T15:53:48.826Z Reads: 56

```
You dont want to discharge lipo's under 37v. That should be the hard cut off. Especially if you aren't monitoring individual cell voltgates with a alarm.
```

---
## \#88 Posted by: FirstTimeBuilder Posted at: 2019-01-15T16:33:57.582Z Reads: 57

```
@Indiangummy  im assuming you mean 3.7v?
```

---
## \#89 Posted by: Indiangummy Posted at: 2019-01-15T16:34:42.949Z Reads: 56

```
Yeah 3.7 per cell. 37 pack voltage if you are running 10s.
```

---
## \#90 Posted by: FirstTimeBuilder Posted at: 2019-01-15T16:58:13.447Z Reads: 61

```
Im running 8s as got two 4s batteries.
```

---
## \#91 Posted by: Indiangummy Posted at: 2019-01-15T17:08:51.179Z Reads: 60

```
Then 3.7v *8= 29.6 v should be the pack voltage cutoff
```

---
## \#92 Posted by: FirstTimeBuilder Posted at: 2019-01-15T17:50:35.330Z Reads: 58

```
This might be a really stupid question but if the batteries are 14.9v each that gives total of 29.8v so how does that work?
```

---
## \#93 Posted by: Indiangummy Posted at: 2019-01-15T18:00:13.709Z Reads: 59

```
@FirstTimeBuilder because you are putting two 4s batteries in series. When you put batteries in series you add the voltages and capacity remains the same, if you put them in parallel you add the capacity of the cells while the voltage would remain the same.
```

---
## \#94 Posted by: FirstTimeBuilder Posted at: 2019-01-15T19:23:31.128Z Reads: 56

```
Is this where i put the cutoffs?


![Sketch%20(11|690x460](upload://dXOhTHx8dt5NXBSf453JnJB3hIQ.png)
```

---
## \#95 Posted by: AlexBE Posted at: 2019-01-16T05:31:58.052Z Reads: 50

```
Well that is the current settings, not the voltage settings, but that is the general area. I would not use 3.7V per cell as the cutoff for those batteries, you will get no range. I would start with 3.5V under load and see how you go with that.
```

---
## \#96 Posted by: Indiangummy Posted at: 2019-01-16T06:32:17.527Z Reads: 50

```
I have never discharged my lipo's under 37V and get 12miles of range consistently (medium to full throttle). It's generally accepted that you don't want discharge lipo's under 37-36v. It decrease's the life span of the cells.
```

---
## \#97 Posted by: AlexBE Posted at: 2019-01-16T06:53:14.125Z Reads: 51

```
I'n not sure what kind of board or battery you have, but that range is very low. Nobody I know uses 36 or 37V as a cutoff UNDER LOAD. Maybe you are talking about the voltage the cells recover to. Not relevant for the vesc settings.
```

---
## \#98 Posted by: TowerCrisis Posted at: 2019-01-16T08:47:40.690Z Reads: 49

```
Uh I really don't think so man. I've always fully discharged from 4.2 to 3.2V (under load). Discharging to 3.7 would literally halve my range lol. Use quality cells that don't have ungodly voltage sag and you can easily discharge further. Vesc settings will kick in to prevent voltage sag (cutoff starting at lets say 3.4V, hard stop at 3.2) is more than effective at protecting cells.

Also, you really don't need individual cell monitoring (assuming there isn't a hardware failiure). You shouldn't be using cells that cause you to worry about voltage drift from a single discharge. High quality lipos are just as reliable as 30Q's.

Also, in talks to cell manufacturers I've been told 4.2-3.2 can be guaranteed 500 discharges (before capacity hits 80% of initial), which would last me 2 years easy. So I'm not too worried about lifespan.
```

---
## \#99 Posted by: deucesdown Posted at: 2019-01-16T17:23:28.834Z Reads: 46

```
[quote="TowerCrisis, post:98, topic:79266"]
High quality lipos
[/quote]

Please list them up, and also the brand/model for the 500 cycle ones.
```

---
## \#100 Posted by: Indiangummy Posted at: 2019-01-16T18:09:38.102Z Reads: 44

```
He's probably referring to garpehes. I'm using 90c 5600mAh garpahene. IMHO I don't think it's a good idea to recommend below 3.7 dischrage on their first build especially if it's a charge only set up. you don't wanna have a runaway discharge on a lipo. So better to be safe than have a fire on hand. Again, just my opinion. But Do as you wish. I'm not going to discharge my garpahenes under 3.6 at most which is plenty of range for me. Hell I only charge my boards once every 3 days.
```

---
## \#101 Posted by: deucesdown Posted at: 2019-01-16T18:48:25.141Z Reads: 45

```
This is resting voltage but there's not much energy available under 3.7v

https://www.rcgroups.com/forums/showpost.php?p=6660057&postcount=7

[quote]

Avg Resting V % Remaining Capacity
By cell
4.00V--84%
3.96---77%
3.93---70%
3.90---63%
3.86---56%
3.83---48%
3.80---43%
3.76---35%
3.73---27%
3.70---21%
3.67---14% 
[/quote]

There are a few other similar tables, most agree there's not much left under 3.7v.

https://www.helifreak.com/showthread.php?t=333661#post3189291

https://www.rcgroups.com/forums/showpost.php?p=16448635&postcount=3

https://www.rcgroups.com/forums/showpost.php?p=31022976&postcount=6

Granted it's different model to model, but I've found from reading a lot of places, that RC lipos are full at 4.2v, 50% around 3.85v, and for all usable energy, empty around 3.7v. These are **resting voltages**, not under load.

There's a few good reasons to be conservative with the cutoffs:
- there's a "knee" in the discharge graph, where when you get to almost empty, the voltage starts to drop very quickly. The actual knee will be at a different point for every cell in the pack. If you get close to the average "knee" point for the pack as a whole, some cells will be well above their knee, while other cells are most likely quite a bit below their knee and dropping fast.
- there's not much energy to be squeezed out when the pack is near empty, at high currents. And as voltage drops, drawn current will increase (watts = volts * amps)

I'm ignoring HV stuff for sake of brevity.

HK Graphenes are kind of a category buster, but still they'll be happier if you don't abuse. I'm interested to know if there are other high quality lipos that can cycle more than 300 times and have very high discharge.

IMO the best advice, stay above 3.7v in all cases.

EDIT Say you can get 500 cycles going from 4.2v to 3.2v. If you usually don't empty your packs, would you not prefer to get 1000 cycles going from 4.1v to 3.7v? I think it maybe be sensible, if you have packs that can take it, to set cutoff at 3.2v, and try to never ever hit the cutoff.
```

---
## \#102 Posted by: wafflejock Posted at: 2019-01-16T19:06:23.316Z Reads: 42

```
Personally use 3.7 as soft cut off per cell and 3.4 as hard cut off, agree it depends on the cell but good to start with conservative values then see how much your battery actually sags under load using a bluetooth module to get your data and then can adjust accordingly (can also check voltage "drift"/difference between cells after discharge and can check internal resistance of individual cells if your charger does it or can get a separate meter if you're interested enough in checking individual cell performance).

---

Also, to note here I don't typically actually run the batteries down to "empty" where I actually hit the cut offs they are there just in case, but usually I'll recharge at about the 3.7-3.8V range back up to full (believe best option is actually to go a bit less than 4.2V unless your batteries are rated for a higher voltage as deucesdown said, but since I charge two lipos separately it's just easier to let them both fill up and balance).
```

---
## \#103 Posted by: bartroosen12 Posted at: 2019-01-16T19:46:37.699Z Reads: 41

```
I should also not run them below 3.2V I have had several hot and swollen batteries when I discharged to around 3V.

Cutoff around 3.4V looks fine, at 3.6V there's only like 10% capacity left in the battery so it doesn't make sense to discharge them furder.

Those multistar packs must give you more than 500m.
From my experience: I had a 10S1P 10C 5.2Ah multistar pack and got a range around 12km (the esc pulled max 20A with a low voltcutoff 3.2V)

Those packs gave around 4V sag when pulling 20A so I shouldn't pull more amps.
```

---
## \#104 Posted by: TowerCrisis Posted at: 2019-01-16T20:50:32.134Z Reads: 34

```
[quote="deucesdown, post:101, topic:79266"]
These are resting voltages, not under load.
[/quote]

Which is exactly why I specified that these voltages I talked about were under load. You can't continue to discharge a lipo with a high load when it's resting at lets say 3.4V.

Setting your vesc to cut off at 3.7 will grant you literally zero range. Any cell is going to sag. If you're at 4V resting per cell you won't be able to ride up a hill if you set your cutoff at 3.7V.
```

---
## \#105 Posted by: FirstTimeBuilder Posted at: 2019-01-17T09:04:07.822Z Reads: 36

```
OK, 

So to go in the middle (kind of) Ill go with 36v soft and 34v hard cut off.

Im struggling to find the battery current max for these batteries, i spoke to HobbyKing people and asked and he said it was 375? Which even i know this cant be right. Any advice on this part would be great as i think ive got the rest of it sorted. The HK site says the motor current max is 65 so thats fine but its just the battery settings im stuck on here. 

Thanks in advance
```

---
## \#106 Posted by: TowerCrisis Posted at: 2019-01-17T09:14:13.080Z Reads: 35

```
Woahh wait, 34V and 36V does not work out for those 4S batteries. Did you mean 3.4V and 3.6V?

How many of those batteries did you get? Are you using 3 in series? Or two in series?
```

---
## \#107 Posted by: FirstTimeBuilder Posted at: 2019-01-17T09:20:06.054Z Reads: 35

```
Yea sorry 3.4 and 3.6v. just shows how important a . is lol 

Running two 4s in series
```

---
## \#108 Posted by: TowerCrisis Posted at: 2019-01-17T09:29:28.341Z Reads: 35

```
Okay, then your cutoff should be 27.2V and soft cutoff should be 28.8V

Since it's a 5000mah cell, you can at most have 5A of Regen current. (That would be a 1C charge current, fairly standard)

So battery min should be -5A. You'll have fairly weak breaks at higher speeds, maybe bumping up to -7A would work but only if you aren't satisifed with -5A


Battery max is pretty subjective for these. The C rating is definitely very inflated and isn't representative of actual performance.

I'd say 50A battery max would be acceptable and relatively conservative for these cells. Anyone with experience want to chime in?

Also, if you're doing a dual drive, make sure to halve the battery amp ratings (-2.5 and 25) so that each vesc adds up to your total max values. The voltage values should all stay the same whether it's a dual drive or a single though.
```

---
## \#109 Posted by: FirstTimeBuilder Posted at: 2019-01-17T09:33:48.334Z Reads: 29

```
Amazing. Thanks for your help
```

---
## \#110 Posted by: Jumpman Posted at: 2019-01-17T09:46:29.991Z Reads: 24

```
I think these modern lipos have a 5C max charge rate, so you can probably go to -25A total, if you needed to.
```

---
## \#111 Posted by: taz Posted at: 2019-01-17T10:04:28.630Z Reads: 28

```
The cut-off value depends on your current draw.
High quality lipos have very little sag compared to Li-Ion
Just to give you guys an example here is a graph from my RC helicopter

![03|690x388](upload://3X3tkAxWv9xEoxtt5Mn6jTuQkTk.png) 

Notice that at 120A current draw (battery amps) my 2x6s 5000mAh in series (hence 12S 5000mAh) drops from 47.75V to 43.95V.
That is around 0.3V per cell.
Now imagine a few more of those cells in parallel, the battery would not break a sweat.
My mean current draw is way above 30A, something very unlikely to happen on an esk8.
Having a low cut off in an application like that would result in too much bogging to make it enjoyable.
Now if I am flying with low rpm cruising slowly I can lower my cut-off, however I have made it a rule to never - ever discharge a lipo below 25% capacity (around 3.75V resting voltage) and I have batteries 10 years old that are still usable.
Oh and as far as charging is concerned, I charge mostly at 4C and in some rare cases at 8C (that is 40A for the 5000mAh batts)
```

---
## \#112 Posted by: Andy87 Posted at: 2019-01-17T10:16:24.666Z Reads: 30

```
Which packs you use again?
```

---
## \#113 Posted by: FirstTimeBuilder Posted at: 2019-01-17T10:20:10.058Z Reads: 30

```
Using two of these in series

https://hobbyking.com/en_us/turnigy-graphene-5000mah-4s-75c-lipo-pack-w-xt90.html
```

---
## \#114 Posted by: taz Posted at: 2019-01-17T10:21:36.756Z Reads: 31

```
I don't remember exactly which ones I used at that particular flight as I have 1 set of these (the 6S version):

![](http://file.espritmodel.com/battery/tp/tp5000pp65c.jpg)

and 2 sets of these

![](https://cdn-global-hk.hobbyking.com/media/catalog/product/cache/1/image/660x415/17f82f742ffe127f42dca9de82fb58b1/1/8/182195.jpg)

Photos taken from the web, as I don't have any photos with me right now.
```

---
## \#115 Posted by: AlexBE Posted at: 2019-01-20T02:39:23.876Z Reads: 24

```
Depending on how you are charging your batteries..... If your charger tells you the capacity it charged in mAh. Run some settings and check how much it capacity was put back into your batteries to get them back to full charge. I would aim for between 70-80% of their rated capacity. 

Then tweak your voltage cutoffs until you have a good feeling for where 70-80% is. The voltages you end up with will depend a lot on things like ambient temperature and discharge rate (how aggressively and fast you ride).
```

---
