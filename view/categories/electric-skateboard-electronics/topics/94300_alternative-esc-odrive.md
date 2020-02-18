# Alternative ESC - ODrive

### Replies: 33 Views: 1296

## \#1 Posted by: xatonic Posted at: 2019-05-19T04:47:33.515Z Reads: 296

```
Hey guys I've been building a new board using some out of the box parts to bring to the hobby and I've been looking at the ODrive for a bit now becuase it's more reliable than a vesc or iterations of the Vesc. Now that I've seen it in action here at maker faire I'm really sold! I also talked to the founder and he's working on a V4 card that is single channel it should be considerably cheaper with other improvements. It's got a peak current of >100A, Continuous current depends on cooling but it's 50-70A, FOC, opensource hardware and software.
```

---
## \#2 Posted by: JLabs Posted at: 2019-05-19T04:53:18.198Z Reads: 295

```
I almost bought one a few months ago, I just don’t have the time to tinker with it and set it up. If it was more intuitive I would be all over it. Encoder support really has me salivating
```

---
## \#3 Posted by: xatonic Posted at: 2019-05-19T04:56:40.162Z Reads: 286

```
Yeah that's why I'm super excited about this v4 card but the current card would still be great for a dual motor setup
```

---
## \#4 Posted by: Acido Posted at: 2019-05-19T10:28:14.251Z Reads: 255

```
Seems really interesting, especially because it can go up to 13s !

Will probably get one for science in the summer :D
```

---
## \#5 Posted by: linsus Posted at: 2019-05-20T11:38:31.860Z Reads: 208

```
[quote="xatonic, post:1, topic:94300"]
it’s more reliable than a vesc or iterations of the Vesc.
[/quote]

This is a very bold claim. Be careful with spreading missinformation.
```

---
## \#6 Posted by: trampa Posted at: 2019-05-20T15:04:48.358Z Reads: 190

```
[quote="xatonic, post:1, topic:94300"]
it’s more reliable than a vesc
[/quote]

How can it be more reliable? There are no issues with VESCs. 
Maybe with clones, but for sure not with VESCs. 

Please also note that 90+% of the work is in the software.
VESC-Tool is a very advanced piece of code!
```

---
## \#7 Posted by: xatonic Posted at: 2019-05-20T16:15:54.350Z Reads: 179

```
It's just so sensitive that it's easy to blow out, sorry for the bold claim I just think we should be looking into a new board
```

---
## \#8 Posted by: Acido Posted at: 2019-05-20T17:01:16.364Z Reads: 176

```
VESC is on another level compared to other ESCs, its easy to blow if you do not know how to use it
like everything else
```

---
## \#9 Posted by: akhlut Posted at: 2019-05-20T17:34:18.803Z Reads: 172

```
This right here

https://www.youtube.com/watch?time_continue=31&amp;v=FUh36RUHzdU
```

---
## \#10 Posted by: davewood1982 Posted at: 2019-05-20T18:06:18.217Z Reads: 163

```
id be interested in this, hate how fragile vesc's are... iv been using the basically bulletproof hobbywing max6 esc's and i love them for reliability, plug and play and power but their fairly expensive and the breaking noise isn't great lol. where can i find more info on these Odrive esc's and possibly a few reviews? are they plug and play or easy to setup?
```

---
## \#11 Posted by: xatonic Posted at: 2019-05-20T20:31:08.340Z Reads: 147

```
They have a website with all the info and I believe a GitHub project as well. And for the plug and play aspect they should be pretty ok
```

---
## \#12 Posted by: linsus Posted at: 2019-05-20T20:45:05.508Z Reads: 145

```
Please elaborate on the manufacturers of the vescs u been using. And what hw verision.
```

---
## \#13 Posted by: davewood1982 Posted at: 2019-05-20T21:41:09.164Z Reads: 137

```
Thanks ill take a gander:+1:
```

---
## \#14 Posted by: xatonic Posted at: 2019-05-20T22:50:55.311Z Reads: 131

```
An Olin vesc, esk8 Vesc, and I'm about to set up the focbox. was running the latest HW there was
```

---
## \#15 Posted by: linsus Posted at: 2019-05-21T07:28:13.533Z Reads: 114

```
Imagine if you bought the real thing right away instead :thinking:
Or a version 6 HW atleast.
```

---
## \#16 Posted by: xatonic Posted at: 2019-05-21T07:49:04.008Z Reads: 110

```
I'm not trying to be rude I just know alot of people that have been having issues with it because it's sensitive and I was trying to find a way for new people to have a really simple esc
```

---
## \#17 Posted by: linsus Posted at: 2019-05-21T09:14:01.576Z Reads: 103

```
[quote="xatonic, post:14, topic:94300"]
was running the latest HW there was
[/quote]

Then dont say stuff like this, cause clearly you werent running the latest HW.

The vesc 4.x is obsolete. The hardware is flawed compared to the hw 6. Using obsolete HW with the risk of it giving you well known faults? Sounds pretty logic to me.
```

---
## \#18 Posted by: Andy87 Posted at: 2019-05-21T09:38:17.239Z Reads: 96

```
Nothing bad in looking for alternatives. More options for us consumer is never bad.

But your claims about the VESCs is not 100% correct like this.

I´m sure you know that there is a difference in VESCs and VESC based controller as well as there is a big difference between the HW4.xx and HW6.xx design.

I also wouldn´t call a VESC or VESC based esc "sensitive" they just give the user a lot of possibilities to adjust there parameters.

The majority of defects happen either because you don´t know what you are doing when you install and set up your VESC/VESC based ESC, or you ride your VESC based ESC on the limit.

There are cases where faulty components caused a defect, but I personally heard only of maybe 1 or 2 happend on a VESC. The others where on VESC based ESCs.
```

---
## \#19 Posted by: davewood1982 Posted at: 2019-05-21T11:56:21.647Z Reads: 93

```
Sorry should of been more specific, i meant various Vesc4s.. and yes seen many cases of blown chips ect, you only have to search this forum to see its fairly common, never tryed a vesc6 because their way to expensive plus im currently using the  Hobbywing Ezrun MAX6 160A 8S ESC which i got because of theses issues with the vesc4 (before the vesc6 was released) and its ROCK solid i so can't justify spending another £300/400 on a vesc6 when my MAX6's do exactly the job i need them to do! This is why i asked about this Odrive esc since it may be better value for money as another option later down the line.
```

---
## \#20 Posted by: linsus Posted at: 2019-05-21T12:12:02.959Z Reads: 95

```
[quote="davewood1982, post:19, topic:94300"]
so can’t justify spending another £300/400 on a vesc6
[/quote]

No worries, I can come across bit harsh as well. 

The vesc6 from trampa is 225£ and there are cheaper hw v6's out there. 
225 is probably what you spent (or more) in total on the blown hardware put together. PLUS you support Vedder. Which close to no other vendor does. 
Trampa gives you a new vesc if it for some reason is faulty and are usually very supporting. (doesn't cover user errors obv.)

Buy cheap = Buy twice = might as well have bought the real thing.
```

---
## \#21 Posted by: trampa Posted at: 2019-05-21T13:14:06.620Z Reads: 83

```
[quote="linsus, post:20, topic:94300"]
(doesn’t cover user errors obv.)
[/quote]

Even in such cases we have been generous.
```

---
## \#22 Posted by: linsus Posted at: 2019-05-21T13:14:44.291Z Reads: 81

```
I know, just trying not to fanboy too much :slight_smile:
```

---
## \#23 Posted by: xatonic Posted at: 2019-05-21T13:41:28.996Z Reads: 77

```
It seems that I've overstepped my boundries and made some bold claims. I haven't tried the HW V6 yet and I'm not sure how it's going to go so I'm sorry for those claims.
```

---
## \#24 Posted by: slick Posted at: 2019-05-21T13:48:36.349Z Reads: 78

```
Interesting. I had a brief look on thier Hompage (im at work) and it seems that you'd need to ensure good cooling if youre planning to go over 40A continous load - meaning a (loud ) fan = more bulk.

That could pose a problem for those that live in hilly areas and/or builds with less space. 

My very first build was a 6S with a Trackstar 150A ESC. That thing had a 40x40mm cooling fan blowing nonstop on a heatsink and was loud as hell. I had puzzled ppl head turning whenever i entered indoors and forgot to turn my board off :rofl:
The fans sound and my battery enclosure definately made them feel discomforted (enclosure looked more like a diy bomb) :rofl:
```

---
## \#25 Posted by: linsus Posted at: 2019-05-21T13:52:58.546Z Reads: 76

```
By cooling they probably refer to the heatsink, I havn't seen any vescs with active cooling yet :D 
I run my vescs at  50A each(100A/2) I probably never hit that level but my vescs never get hot to the touch. They probably would If i were to do something besides city riding tho.
```

---
## \#26 Posted by: Andy87 Posted at: 2019-05-21T15:20:51.463Z Reads: 73

```
I have seen one. I think it was from a French guy with dual escapes in a waterproof box which had two esc size big fans mounted on top. Not sure it was ever necessary to really cool them externally, but he made it.
```

---
## \#27 Posted by: davewood1982 Posted at: 2019-05-21T16:38:07.154Z Reads: 70

```
iv had my  Hobbywing Ezrun MAX6s over two years now and well as i stated, the vesc6 wasn't available or if it was it was in a very early prototype stage at that time,  also regarding the vesc6's price, 225£ i believe? correct me if im wrong but that is per unit  so for so for a twin motored setup your need 2 so definitely not worth it for me personally  since im very happy with my @Nowind  inspired mtb max6 build. ill definitely consider  vesc6 if my max6's ever fail though but having other options will always be welcomed.
```

---
## \#28 Posted by: linsus Posted at: 2019-05-21T17:06:19.660Z Reads: 65

```
I'm glad you like the one you choose, awesome!
But its hard to compare the level of tech of the vesc vs. a massproduced generic esc.


If the price is the problem, the project is opensource, use the schematics build your own pcbs, the BoM is 90 USD. Nothing stopping you.
```

---
## \#29 Posted by: slick Posted at: 2019-05-21T19:17:10.067Z Reads: 61

```
To make it short:
Open air with just heatsinks @ 13.2C ambient temp. - under 40A.With additional PC fan 80mmx80mmx 70-80A. With overkill fan up to 90A.

Read about thermal limits of the ODrive here:
https://discourse.odriverobotics.com/t/odrive-mosfet-temperature-rise-measurements-using-the-onboard-thermistor/972

Honesty, I dont see the Odrive as an alternative to the VESC considering that information. Since the ambient air temperature in summer is more than 13C and we all put our ESCs in enclosures that means that the Odrive needs to be reliably cooled or it will overheat (thats just talking about street boards...I dont see it surviving off-road)
```

---
## \#30 Posted by: Paulycnotes Posted at: 2019-08-05T12:26:57.123Z Reads: 39

```
Hey my man. Can you please tell me more about the ESC first shift spending hundreds and hundreds on vescs and focboxes I would love an alternative
```

---
## \#31 Posted by: linsus Posted at: 2019-08-05T13:25:19.056Z Reads: 36

```
You get what you pay for. 
The BoM on the VESC6 is approx 95 dollars/unit(Mouser). Thats without any profit margin, unsoldered, no heatsinks or connectors. 

Odrive is probably comparable to the VESC but seems like a jungle to configure.
```

---
## \#32 Posted by: Paulycnotes Posted at: 2019-08-05T14:06:08.539Z Reads: 31

```
I would like for you to build me one.... Please.  How much?  Also, is this needed for my new Focbox UNITY??
```

---
## \#33 Posted by: linsus Posted at: 2019-08-05T15:51:10.080Z Reads: 22

```
My hourly fee is 120 eu/hr. It takes 4-5 hours to solder a vesc, u do the math 😅
```

---
