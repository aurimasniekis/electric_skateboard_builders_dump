# MiniM&rsquo;s PRE build thread

### Replies: 29 Views: 1299

## \#1 Posted by: Minim Posted at: 2017-06-17T08:00:42.921Z Reads: 148

```
I felt that this had nothing to do in the build section so I'm starting it here. Hope some of the more experienced guys can chime in with tips regarding what to get and not to get so I don't go in all the traps a newcomer can get into :slight_smile: 

I'm today a Inboard M1 rider but I came across this  forum when searching for problems with the  Evolve carbon GT. It looks like the evolve got all I need but it's tempting to go DIY instead since I don't no one to blame if somethings goes wrong then :D I've had my Inboard for 1-2months and allready had a replacement board due to a broken hub motor and a issue with the main board. I do however notice that the price I'm getting up in is similar to the Evolve carbon GT so maybe it's be

So in short I have started reading up and came across a few designs that I really liked. Kaly.Nyc had built a nice trampa board and I'm tempted to go that way myself. Only thing I came across was the VESC hijack that trampa was a part of and I'm not sure I want to support that (correct me if I have mistaken this situation tho). 

Enough of the booring stories and onto the project :) 

**Goal:** 
-Can be used on a variety of surfaces 
-Can survive Norwegian road quality 
-20km++ realistic range in combined riding
-30kph speed 
-Can climp most hills (paved) that I can come by without me having to carry it (no go with the inboard..) 
-Can handle the weight of a 90kg rider. Even better if it also can handle 90kg rider + 20kg luggage for rare accasions. I'm missing accleration and stopping power in my inboard.

**Shopping list:**
-VESC6 (I'd really like to find alternatives to trampa's that run the latest vesc software but seems hard  to find..) 
-2x 6374 190KV KalyNYC motors 
-Kaly NYC motor mounts for carver 
-Pulleys/belts from Kaly NYC 
-ABS battery enclosure from Kaly NYC 
-Urban carver board w/ 7"
-12S4P 18650 Samsung 30Q 15A batteries  
-18650 Welding station + flat wires and welding "strips"
-Some kind of remote?
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-17T08:17:28.800Z Reads: 133

```
For remote I've had reliable use of the Nano v2 remote so far. The benchwheel is my other remote which is pretty reliable as well.

For the VESC, I'd say just get a VESC 4.12. They're still super reliable and are definitely not becoming obsolete anytime soon. 6 is still brand new and I'm not even sure if other suppliers will get the designs for it. £300 is insanely priced and 100% not worth it over the 4.12
```

---
## \#3 Posted by: Minim Posted at: 2017-06-17T09:56:47.288Z Reads: 121

```
Thank you. I will look into both those remotes :)  

I just figuren that since im a heavy rider at 90-95kg i will put a lot of load on the vescs and the vesc6 looks like it has a superior cooling solution. Also having access to vesc tool and more functions is tempting as a tech geek :p Isn't the design open source anyways so others can make a vesc6 and call it sk8board esc6?
```

---
## \#4 Posted by: Minim Posted at: 2017-06-19T19:02:00.734Z Reads: 101

```
Got two questions popping up. I was set for 6373 190kV motors but I see now that they are a bit high RPM for mye goal so I need to find lower kV options I think. 

66/13 gearing that trampa has is a 5.07 ratio and the 62/16 that kaly sells is 3.87. With a 190kV@12S that's 9500rpm at top and assuming it's a 7 pole motor that's 66.5k ERPM and above the recommended 60k limit of the VESC so that's not good either. Another thing is that with the gearing from trampa/caly I will end up with a way to high gearing and bad hill climbing. I'm planning to use 7" (180mm) or 97/100/107mm (big) longboard wheels. Here is what I got from the setups mentioned. 

66/13 - 5.07 - 190kV 180mm = 63.57km/h - 39,45mp/h 
62/16 - 3.87 - 190kV - 97mm =44,82km/h 27,85mp/h 

Caly setup could be solved by dropping the little wheel to 13 tooth as speed then would be 36km/h or 22mp/h and that is perfect for me I think. I have a feeling that sourcing a lower kv motor is the way to solve this tho as I would get under the recommended 60k erpm. The 118kV motor that Trampa sells is just perfect with the 66/13 gearing as it would give me 39km/h or 24mp/h (but only 27km/h with street wheels). Still think that would climb pretty decent but then I sacrifice on motor power since that motor is "just" rated for 2.4kW. If it could stand that without overheating I wouldn't worry but I suspect thats max max max power and that it will get pretty hot uphill if I use it hard or am I wrong? I want crazy climb power without being afraid of heat :D 


So over to second question. I've done a lot of reading here but I can't decide on a battery solution. I would like to keep it simple. I got a charger for lipo that can do 1400Watt with balancing 6S. That is a PITA to move around with tho and I will be using my boards when traveling/living in hotels mostly so integrated BMS is preferred even if it is a extra cost but a last chance could be a separate charger like the one I got. So what do I choose between lipo/18650/123/26650/life/lifepo4 and what are the pro cons that I'm missing. I aimed for Samsung 30Q 15A discharge 12S4p pack but I see that LG HG2 has a version with 20A discharge and 3000mAh capacity. In a 4P that would give 80A max discharge and 520Wh if my math is correct and close to my aim with 30-35km realistic range from what I read here on the forums. I will then need a spot welder, bms system so the cost is going up with 18650 choice vs lipo. Any thoughts?
```

---
## \#5 Posted by: Minim Posted at: 2017-06-21T05:31:53.287Z Reads: 83

```
might be asking in the wrong place here but is the Trampa mountainboard eletric kit a good place to start? I'm considering it even if I would like to use  street wheels from time to time also. It was just in stock and tempted me with those sexy blue wheels :D
```

---
## \#6 Posted by: Minim Posted at: 2017-06-25T07:41:05.892Z Reads: 83

```
Can anyone give me some pointers on what to go for of the urban carver/mountainboard? I can't decide.. As I understand it I loose the possibility to run street wheels with the mountainboard but will I ever look back after trying mountainwheels? 

Also trampa doesn't sell 6374motors in their kit and the vesc6 is heavily discounted when bought as a kit.. is it possible to get a decent price when selling 6355 trampa motors again to fit 6374?
```

---
## \#7 Posted by: Minim Posted at: 2017-07-15T17:39:43.163Z Reads: 75

```
Sort of bump to my thread again. Been fighting back/forth on what to do and Im not much further than last time I asked here :D Mountain/street/urban and motor setup is still the hard choices. If it's barely better than my Inboard is now I won't bother upgrading but if it can be all I want then it's a no brainer.. Will dual 6374 also have troubles like the raptor 2 on steep hills, barely walking speed on top of long hill?
```

---
## \#8 Posted by: Minim Posted at: 2017-12-23T08:39:30.543Z Reads: 61

```
This has taken way to long. I've been waiting on the Raptor 2 but it doesn't look like 2018 will be the year for them either so I have to start planning to build my own board for the summer. 

Another thing that makes it even more tempting to build my own is that I just refurbished a CNC mill so I'm no able to make some of my own parts. I'm leaning towards belt driven since it's simpler to machine but should I look into hubs?
```

---
## \#9 Posted by: Grozniy Posted at: 2017-12-23T08:46:05.884Z Reads: 59

```
If you do motor mounts, you could sell them ;)
```

---
## \#10 Posted by: koralle Posted at: 2017-12-23T09:06:54.599Z Reads: 58

```
* you mentioned tough roads and high power hill climbs - don't go with hubs!
* "66/13" - don't use 13t pulleys, they mess up your belts. 15 apparently is the smallest pulley you're supposed to use.
* dual 6374 motors on a 12s4p setup already gives you insane power. Your 190kv motors will easily climb anything, even if you dont have crazy gear ratios. You might not always be running your motors in their sweetspot but you will still easily get 30km of range methinks.
* do your own wheel pulleys and mounts if you want to use your cnc
* if you care about style, get 107mm abecs, if you dont, go for the at wheels.
```

---
## \#11 Posted by: Minim Posted at: 2017-12-23T10:31:27.322Z Reads: 57

```
ok. I just supposed I need low gearing since I'm 100kgs. The Inboard I had was useless :P 

Grozniy I could prolly make some if I could make something useful. Been test running lately can I get 0.01mm accuracy so it should be more than enough for mounts. 

<img src="/uploads/db1493/original/3X/9/6/96d4c9a9c52936eaa82ae19e3fa426e93df5f209.jpg" width="666" height="500">

https://youtu.be/pm27Hr5Z1M0
```

---
## \#12 Posted by: Grozniy Posted at: 2017-12-23T11:23:54.503Z Reads: 52

```
Just remember: simpler design is better, stronger and faster to cut and to assemble.
```

---
## \#13 Posted by: koralle Posted at: 2017-12-23T11:26:27.979Z Reads: 52

```
be sure to read this
http://www.electric-skateboard.builders/t/revisit-bad-motor-mount-designs/37075
```

---
## \#14 Posted by: Minim Posted at: 2017-12-23T13:35:32.656Z Reads: 44

```
Thanks for the link :) Is alu the goto material for this? What about 316?
```

---
## \#15 Posted by: LukePL Posted at: 2017-12-23T14:04:55.697Z Reads: 44

```
If you need vesc6 check @stewii and his ESCape 😉
```

---
## \#16 Posted by: Minim Posted at: 2017-12-23T14:26:56.568Z Reads: 41

```
Will do. If I can avoid supporting trampas trademark bullshit I'll do that. I will try to find another board and trucks also even if they look like a nice product :S
```

---
## \#17 Posted by: koralle Posted at: 2017-12-23T14:45:28.488Z Reads: 41

```
[quote="Minim, post:1, topic:25562"]
VESC hijack that trampa was a part of and I'm not sure I want to support that (correct me if I have mistaken this situation tho)
[/quote]

Yes you have mistaken the situation. I thought the same at first but after some reading it turns out they, together with Benjamin, the creator just registered the trademark "Vesc" so someone else doesn't do it and so that anyone can't just call any inferior product the same. Didnt hurt anyone. They still let people sell already made *Vescs* with just some marker across the name.  What they also did was create a basis for Benjamin to finally start actually making some money with this thing. everyone else is still allowed to copy and they are working on further improving software and hardware for everyone. 

They just get annoyed with people who create splintered versions of the software, doing some quick hacky upgrades instead of waiting and going through the (slower) right channels they created so everyone can work together on the same version the way open source software is meant to be developed. They can't do anything about that though except ask. 

What absolutely seems to blow trampas (Frank's)  hat off is when people sell these controllers without telling customers explicitly where they can find all the code that has been used. A small thing really for most but apparently required in order to comply with the GPL licence, all this runs under.

In this forum the picture is often painted of Trampa being the big corporate IBM, swooping in and taking all the nice things from poor self made open source underdogs. This is absolute bull. Trampa is not a huge rich company, hardware plans and software of new developments will still be released and public participation is highly encouraged.

With 99% of the different productions of vesc4, Vedder just relies on customers donating once they download the software and apparently these donations have been limited to a *very* small number of (rather generous) donors. Frank and Vedder actually seem like really nice people. they just wanted some type of protection against being run over by China and friends. 
Don't buy into all the mobbing nonsense just because they have crap marketing and aren't the enertion "cool kids"!
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-12-23T14:49:26.677Z Reads: 37

```
Didn’t have time to read through all that, just the first sentence of two.  They are using a strategy of marketing that almost everybody else considers to be  bad. They trademarked “VESC”, no other vendors can use that name. They are price gouging ALOT. there is no way in hell each of those vesc 6’s even cost $100. yet they are still selling them for over $300

Vedder has also turned down offers by enertion to give him a chunk of each focbox sale (according to jason) 

I personally do not like the way they are doing business and will never buy from them. Just my opinion
```

---
## \#19 Posted by: koralle Posted at: 2017-12-23T14:56:55.422Z Reads: 38

```
They are selling a premium product which they put loads of time in at a premium price. If you can't/don't want to afford it, keep using your vesc4 which works perfectly fine and wait for others to produce vesc6 cheaper again but stop crying and send vedder a buck for serving the creators of your vesc4 with awesome plans and code!

[quote="GrecoMan, post:18, topic:25562"]
Vedder has also turned down offers by enertion to give him a chunk of each focbox sale (according to jason)
[/quote]

neither of us knows absolutely scratch about the terms that were offered and thus should not comment.
```

---
## \#20 Posted by: LukePL Posted at: 2017-12-23T14:58:51.536Z Reads: 36

```
To be honest I don't understand this all shit storm around Vesc6 but my only thing against Trampa is the price. Maybe I'm wrong but when you produce somethig you should add 100% to be safe and have a descent profit. Trampa is adding much much more and for me it's not worth the money. 
It's understandable that hard work of BV should be paid but:
- he choose to do it as open source he could expect that won't profit from that.
At this point if he continue as not open source would be also ok but just find descent investor make a honest price and make your money!
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-12-23T15:01:15.538Z Reads: 35

```
I have already donated money to vedder.  @chaka put hundreds of hours into his custom esc and sells it at a premium, but not an insane premium like trampa
```

---
## \#22 Posted by: koralle Posted at: 2017-12-23T15:04:04.861Z Reads: 31

```
yeah so like I said the hate seems to be very strong here although a little misguided (just wait for mmaner to comment :slight_smile:)  . sorry for messing up your thread but you asked for info.
```

---
## \#23 Posted by: mmaner Posted at: 2017-12-23T15:05:44.231Z Reads: 32

```
[quote="koralle, post:10, topic:25562"]
don't use 13t pulleys, they mess up your belts. 15 apparently is the smallest pulley you're supposed to use.
[/quote]

Not true, I've got a dual with 11t pulleys that has iber 500 miles on it and never broke a belt.  Wash them off and the still look new.  Plus you you get more tooth contact with short mounts.
```

---
## \#24 Posted by: mmaner Posted at: 2017-12-23T15:09:13.664Z Reads: 34

```
[quote="koralle, post:17, topic:25562"]
Trampa being the big corporate IBM, swooping in and taking all the nice things from poor self made open source underdogs. This is absolute bull. Trampa is not a huge rich company, hardware plans and software of new developments will still be released and public participation is highly encouraged.
[/quote]

Just because they aren't huge doesn't mean they can't act big...welcome to the internet.   Everyone says they 'will' be release, been hearing that for months but it hasn't happened yet.
```

---
## \#25 Posted by: koralle Posted at: 2017-12-23T15:10:04.975Z Reads: 35

```
just like everyone says they "will" ship soon ^^
there is a lot of trust needed around here ;)
```

---
## \#26 Posted by: Minim Posted at: 2017-12-23T15:11:57.244Z Reads: 34

```
We can cover up what trampa did in many ways but I got my opinion of what they did and will try to avoid buying from such companies. I discussed it directly with frank in the vesc thread also and we agreed to disagree I think. He tried to take a open source product and make it a trampa-exclusive product pretending that helping benjamin was the main goal. C'mon let's be honest here..
```

---
## \#27 Posted by: mmaner Posted at: 2017-12-23T15:12:47.465Z Reads: 36

```
Trust is earned. It's one thing to ship late with an explanation. It's a different animal all together price gouge and attempt to control the market with lawyers.

So many things you've said are just wrong. It sounds like you work from trampa.
```

---
## \#28 Posted by: koralle Posted at: 2017-12-23T15:29:33.967Z Reads: 35

```
I don't have anything to do with them bro. am totally new to eskating. I just don't like bullying. I don't think the way they did everything was a smart move from a business perspective but I think all this rage is a bit weird and the market will regulate things don't worry.
I know you love having the last word so be it I will not comment on this further.
```

---
## \#29 Posted by: mmaner Posted at: 2017-12-23T16:40:57.716Z Reads: 32

```
[quote="koralle, post:28, topic:25562"]
I just don't like bullying
[/quote]

Then you are on the wrong side if this. 

[quote="koralle, post:28, topic:25562"]
I know you love having the last word so be it I will not comment on this further.
[/quote]

Don't start nothing, won't be nothing. You started this, not me. Either defend your position or leave.
```

---
