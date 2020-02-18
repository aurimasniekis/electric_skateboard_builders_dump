# Cheap ebay BMS Good or Bad?

### Replies: 50 Views: 2181

## \#1 Posted by: Orin635 Posted at: 2017-09-29T19:07:37.971Z Reads: 213

```
Would experienced esk8 builders recommend a cheap balance bms from eBay

Link: http://www.ebay.co.uk/itm/Protection-Balance-Module-BMS-PCM-12A-for-6S-22-2V-Li-ion-Li-Po-battery-6S12W003/321790732770?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m1438.l2649
```

---
## \#2 Posted by: jmasta Posted at: 2017-09-29T19:40:46.166Z Reads: 209

```
It's only 12A, so you'd have to bypass it.  Personally I am not a fan of bypassing your BMS because you lose so  many safety features

For 6S, just use a balance charger. It will work much better than that thing
```

---
## \#3 Posted by: scepterr Posted at: 2017-09-29T19:41:09.425Z Reads: 204

```
[quote="Orin635, post:1, topic:34306"]
Would experienced esk8 builders recommend a cheap balance bms from eBay
[/quote]

No..lol
10
```

---
## \#4 Posted by: Orin635 Posted at: 2017-09-29T19:43:00.922Z Reads: 193

```
I am definitely not using a balance charger. what features would I be bypassing with the cheap BMS? also what BMS would you recommend
```

---
## \#5 Posted by: Orin635 Posted at: 2017-09-29T19:44:07.456Z Reads: 183

```
why is it bad?
```

---
## \#6 Posted by: scepterr Posted at: 2017-09-29T19:46:10.834Z Reads: 180

```
They fail or don't work right from the start
IMO BMS should never be the cheapest part in your build
```

---
## \#7 Posted by: Orin635 Posted at: 2017-09-29T19:46:39.405Z Reads: 175

```
I'm seen plenty of videos saying they're fine. how do they fail?
```

---
## \#8 Posted by: scepterr Posted at: 2017-09-29T19:47:01.465Z Reads: 174

```
Bad components , bad assembly
Do you really feel comfortable protecting your vesc and battery for $15-$20 from a noname manufacturer.
Expensive ones fail too just usually not in way that'll ruin everything, switch might die, etc
```

---
## \#9 Posted by: Orin635 Posted at: 2017-09-29T19:49:40.884Z Reads: 173

```
I am using an esc since it's a cheap build so does that make a difference
```

---
## \#10 Posted by: BoostedBuilder Posted at: 2017-09-29T19:54:02.475Z Reads: 171

```
Basically what he is saying: if you are willing to put your life/body in danger, go with the eBay BMS))
```

---
## \#11 Posted by: Orin635 Posted at: 2017-09-29T19:54:51.654Z Reads: 167

```
I'm just confused what can happen isn't the bms just used for charging?
```

---
## \#12 Posted by: dickyho Posted at: 2017-09-29T19:58:09.274Z Reads: 165

```
12A can not use for electric skateboard. will burn when loaded too much, or during sort while. 

imaging when you driving fast, then suddenly lose power, and can not brake......
```

---
## \#13 Posted by: Orin635 Posted at: 2017-09-29T19:59:46.328Z Reads: 160

```
I see. what is that 12A for? isn't that for discharge?
```

---
## \#14 Posted by: SORRENTINO Posted at: 2017-09-29T20:00:34.867Z Reads: 157

```
He could use it for charging only by bypassing it, but I still wouldn't buy a 12 dollar BMS  :sunglasses:
```

---
## \#15 Posted by: Orin635 Posted at: 2017-09-29T20:01:29.389Z Reads: 154

```
I just wanted to use it for charging I didn't know it could do anything else :p
```

---
## \#16 Posted by: jmasta Posted at: 2017-09-29T20:02:07.359Z Reads: 153

```
> Over charge detection voltage:	**4.325**±0.025V

Not to mention, that thing has a over-charge detection voltage that is way too high. It potentially could charge a cell all the way up to 4.35V before cutting off

That cheap BMS could destroy your batteries. Get one from SuPower or Bestech that is rated for the current you will actually pull.  Or use the hobby charger. It will work much better
```

---
## \#17 Posted by: Orin635 Posted at: 2017-09-29T20:03:37.468Z Reads: 147

```
Sorry, this is my first time hearing all this :P what is charge detection. how much do the BMS's from SuPower or Bestech cost?
```

---
## \#18 Posted by: krloz Posted at: 2017-09-29T20:04:32.518Z Reads: 148

```
So the thing is: 
You cannot use this for discharge.  It WILL cut out power in the worst moment
You can use it for charge if you are willing to risk the low quality and can't afford better
You will get what you pay for

Bottom line.  I use a cheap bms only for charging my 10s. But i can't use a hobby charger
```

---
## \#19 Posted by: jmasta Posted at: 2017-09-29T20:05:01.551Z Reads: 144

```
Don't mean to be rude, but get on that Google machine

  More searchy searchy. Less posty posty :joy:
```

---
## \#20 Posted by: krloz Posted at: 2017-09-29T20:05:57.957Z Reads: 138

```
And also what @jmasta jmust said

Edited the m in. Sorry.  Had too
```

---
## \#21 Posted by: Orin635 Posted at: 2017-09-29T20:06:31.484Z Reads: 126

```
Yes I'm sorry for all the questions I have done a lot of research and watched a lot of youtube videos and a lot of people use the cheap eBay BMS's for charging their 6s lipos so I was confused why it is bad
```

---
## \#22 Posted by: Okami Posted at: 2017-09-29T20:07:09.439Z Reads: 122

```
If i were to buy it i would probably check whenever it does the balancing action nicely.. i think this might be biggest pitfall with these sort of bms that they balance slowly or only at very end of charging, so u got to check / know when really balancing action has been completed (especially / more important for lipo probably)..

and not just rely on light telling u that charging has been ended when in fact it might be that volts have been reached but cells are not balanced yet (ive heard.some people leaving chargers on for the night also but everyone should.decide for themselves if they wish to do so)

Other.than that i would like to believe it should work for charging purpose but i would probably still check first times that it does its job nicely.

I suspect 88ma balance current isnt the worst or slowest. I think ive seem something around 40 ma for other bms while hobby chargers tend to do 100-200 ma i think. 

So if the specs are true it might not be the slowest bms balance module
```

---
## \#23 Posted by: dickyho Posted at: 2017-09-29T20:07:39.614Z Reads: 113

```
I do have 10S banlance charger, but expensive,so I don't what to sell on ebay....
```

---
## \#24 Posted by: Orin635 Posted at: 2017-09-29T20:08:57.224Z Reads: 108

```
I am using a 6s setup
```

---
## \#25 Posted by: krloz Posted at: 2017-09-29T20:08:59.470Z Reads: 109

```
It is bad because it id's cheap
The specs will certainly be exaggerated
I have my cheap bms with mounted battery cell alarm monitor because of what @Okami explained
```

---
## \#26 Posted by: Orin635 Posted at: 2017-09-29T20:09:09.065Z Reads: 109

```
So what do you recommend
```

---
## \#27 Posted by: Orin635 Posted at: 2017-09-29T20:09:40.242Z Reads: 106

```
How much would that cost to do?
```

---
## \#28 Posted by: Orin635 Posted at: 2017-09-29T20:11:23.084Z Reads: 108

```
Could someone please watch this: https://youtu.be/jxHQjlHv1y4?t=29s  

just for like 2 minutes
```

---
## \#29 Posted by: dickyho Posted at: 2017-09-29T20:12:53.543Z Reads: 105

```
about 200us included shipping. I wonder how could someone will buy a 200us charger.....
```

---
## \#30 Posted by: Orin635 Posted at: 2017-09-29T20:14:44.121Z Reads: 102

```
My whole setup will cost around 200usd :P
```

---
## \#31 Posted by: Okami Posted at: 2017-09-29T20:15:39.948Z Reads: 103

```
I think people usually order.from bmssupport / s page. What i would watch out would be the bms bulkyness. Though i think.this only happens for these beefy high discharge.bms.

Why people tend to recommend to go with good.quality bms is probably because they tend to fail or.not work probably quite often. Though i think this.might be specially true when they are used for discharge purpose too, so.u might be somewhat covered that u would use it.just.for.charging (hence one plug, no need to carry around smart charger and set it up each time.)

Otherwise.. wish u find info from someone has tried it, havent used it, so cant tell whenever it works good
```

---
## \#32 Posted by: Orin635 Posted at: 2017-09-29T20:16:55.656Z Reads: 101

```
Ok, thanks could you watch that video, please?



here's vid again:  https://youtu.be/jxHQjlHv1y4?t=29s

I just want your guy's opinion on what he says
```

---
## \#33 Posted by: Okami Posted at: 2017-09-29T20:25:50.760Z Reads: 96

```
Yeh, he is also on forum. So if u order try to make sure your power supply outputs 25.2v or so.. otherwise bms can mess up your cells a bit by overcharging them to 4.3v or something.. 4.3v is not immediately critical but probably not something good for their health / cycle life.

Of course it doesnt mean that 27v will overcharge but use 25.2 just to be safe like he said in video.

@VladPomogaev maybe can shed some more light how these bms perform?
```

---
## \#34 Posted by: Orin635 Posted at: 2017-09-29T20:26:40.460Z Reads: 95

```
I will be using a 25.2V charger
```

---
## \#35 Posted by: jmasta Posted at: 2017-09-29T20:28:39.999Z Reads: 96

```
I don't agree with Vlad on that.  An over-charge detection voltage of 4.325V +/- 0.025 (4.35V max) is way too high.  If you are using the BMS for charging only, it's only purpose is to balance the cells and keep them from over-charging.  That cheap BMS could technically charge them to 4.35V before it even notices.  Any BMS with an over-voltage protection of greater than 4.25V should be avoided
```

---
## \#36 Posted by: krloz Posted at: 2017-09-29T20:32:36.777Z Reads: 94

```
Yeah but it would only overcharge your cells if your power supply is outputting more than 4.2xcells. However it is true the bm.s. will not protect in case the supply somehow fails and rises in voltage
```

---
## \#37 Posted by: Okami Posted at: 2017-09-29T20:32:55.341Z Reads: 94

```
I agree, that is why i recommend for him to check everything if he does make the step to go in this direction. Honestly i usually check everytime that cells are all good, even if i dont use bms (where everything is hidden and checking cells might be a lot harder...

I would sort of advice to install seperate cell checker, to monitor voltages seperetaly outside of bms to see whenever everything gets balanced nicely.. this.might require parallel balance wires though
```

---
## \#38 Posted by: Orin635 Posted at: 2017-09-29T20:40:29.390Z Reads: 94

```
Ok thank you all for the help
```

---
## \#39 Posted by: pat.speed Posted at: 2017-09-29T23:05:39.007Z Reads: 92

```
Last thing if you are trying to save money you can get a IMAX B6 on eBay for about 15-20 bucks then you can just plug it in and it will charge very easy and much better than the bms. And to power it you can use a old laptop charger or something you already have
```

---
## \#40 Posted by: Okami Posted at: 2017-09-30T00:53:46.685Z Reads: 92

```
Yeh, if u go really extreme, i suppose one can "install" b6 permanently in deck. Though ive heard it might not be best if electronics are.not 100% protected against shock there.and something comes loose.. next part.would be to load some auto settings, so u can start charging just with a few clicks after plugging in the power cord.. would see all the voltages and stuff, mah pumped in.. and wouldnt need to.be in blind spot about what is happening with cells on cell.level
```

---
## \#41 Posted by: pat.speed Posted at: 2017-09-30T04:32:30.421Z Reads: 83

```
Yeah man I'm thinking of opening my B6 and putting some relays in there to act as if the switches were being pressed then have them connect to an arduino or picaxe that presses them in a certain order to start charging
```

---
## \#42 Posted by: Okami Posted at: 2017-09-30T07:25:06.513Z Reads: 82

```
Would love to see the implementation of this. I suppose if case is removed at least partly, some space could be gained. Though u would probably still need the "rail" for cooling fets of charger
```

---
## \#43 Posted by: pat.speed Posted at: 2017-09-30T07:56:35.387Z Reads: 76

```
Yes the rail would probably have to stay but I would only need to cut away a smal portion to gain access to the buttons. Do you know if the charger will deplete my batteries if I leave them plugged in for long periods? That is my only concern
```

---
## \#44 Posted by: Okami Posted at: 2017-09-30T08:55:29.255Z Reads: 68

```
I think it only works as output to battery side (does not drain batteries unpowered), though it would probably be best to check this or just install small switch to be totally safe
```

---
## \#45 Posted by: pat.speed Posted at: 2017-09-30T08:59:54.894Z Reads: 71

```
Yes good idea, I think I might have another relay that opens the power first then the others follow with the switches. I will make sure to post about how it goes if I ever do this
```

---
## \#46 Posted by: Okami Posted at: 2017-09-30T09:26:56.787Z Reads: 72

```
Actually there is this small charger also called b6. It doesnt have nice screen but.someone should check how well they work..

https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html?___store=en_us

Specs:
Operating Voltage: 11~18V DC
Charge Power: 50W max
Charge Current: 5A max; Charging process will monitor battery capacity continually and adjust charge current as necessary. 
Balancing Current: 200mA/cell
Lipoly Cell Count: 2~6 cell (7.4V~22.2V)
Dimensions: 116.7x77.8x31mm
```

---
## \#47 Posted by: pat.speed Posted at: 2017-09-30T09:29:36.477Z Reads: 70

```
Yeah, thats the charger I am going to use on my next build. A screen would be nice and the storage function but I guess that can be my excuse "I've got to go ride my skateboard so that the batteries don't get ruined" :joy:
```

---
## \#48 Posted by: bartroosen12 Posted at: 2017-09-30T18:09:10.967Z Reads: 67

```
I use a 10$ 12A ebay bms.
Using it for 5 months right now, all cells are still balanced, I use a 4A 25,2V charger and a 6S2P 10Ah Lipo  battery pack.
http://www.ebay.co.uk/itm/252611077311
I only use the bms for charging and it's just working fine for me.
It's so much easier than a balance charger.
```

---
## \#49 Posted by: jmasta Posted at: 2017-09-30T22:46:39.252Z Reads: 64

```
You use a 6S BMS with a 10S pack?  I'm guessing that must be a typo...
```

---
## \#51 Posted by: Namasaki Posted at: 2017-10-01T02:52:39.707Z Reads: 60

```
[quote="Orin635, post:1, topic:34306"]
Would experienced esk8 builders recommend a cheap balance bms from eBay
[/quote]


Not in a million years.
```

---
