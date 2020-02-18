# Choosing a Lipo charger for specific BMS setup

### Replies: 25 Views: 1162

## \#1 Posted by: eranmo Posted at: 2018-05-19T07:04:38.121Z Reads: 118

```
Hi Guys.

I am designing a BMS setup for charging purposes only for my 2 x 10,000mAh 6S Lipos in parallel (bypass the discharge).

My design (Attached) is to connect a cheap 25.2v/10A BMS to each of my 6S Lipo batteries and connect a single 25.2v/25A Power supply to both Lipos when charging(since I do not want to have 2 chargers for 2 Lipos – each of the BMS will pull 10A), I choose 25A charger instead of 20A for safety/manufacture error reasons.

Does anyone see any issue with this setup?

-	What is the best approach when choosing a BMS & DC power supply in terms of charging parameters?
a.	Have the BMS limit the charging current.
b.	Have the DC power supply limit the charging current going to the BMS?
-	I read on couple of places that it is not safe to charge any Lipo with more than 5A, even if the Lipo 1C charging rate is higher than 5A (10A), is this correct? 

Thanks all
I will add a video once I complete the setup :slight_smile:![dual BMS setup|690x468](upload://nbw63VAVFYIrUew38rlPKrKaPNd.jpg)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-05-20T02:16:40.197Z Reads: 87

```
Hey mate,
Yes there are multiple things wrong with this setup so i'll list them.
1. You shouldn't use 2 BMS's as they cannot communicate with each other and therefore will mess up balance voltages etc. If one cell is at 3.8v and another in the other pack is a 4.1v, the batteries life will be significantly decreased. Just use a 12S BMS and a single 50.4v laptop-style charger. (this is what i've heard at least)
2. A 150A relay switch sounds good in theory but will not be effective whatsoever. The contacts of the relay will die within a few weeks as the inrush current from the capacitors in the ESC upon connection causes enormous sparks (i used an AC mains switch rated at 80Amps and i thought it'd work perfect. Instead it shot a 1m long spark which was 42v @840a at my mum (she's fine dw)). Instead of a relay, use something like @psychotiller 's anti spark switches or even just a simple XT90 Anti Spark loop key (you can find these antispark plugs (which are different to standard xt90's) on hobbyking in a set of 2 for like $7 or something)
3. For your question, i recommend making sure your charger is rated at 50.4 Volts at no more than 5 amps like you said. This will take about 2 hrs to charge your board.


If you have any other questions feel free to ask 
All the best my friend
```

---
## \#3 Posted by: eranmo Posted at: 2018-05-20T04:08:52.481Z Reads: 78

```
Thanks Mathew.

1)	The 2 Lipos in my drawing are set up in parallel, each Lipo is individual so I don’t understand from your response why the 2 BMS should communicate with each other if each BMS is charging a different 6S pack, did I miss something?
2)	This is very interesting, you got me worried here… I will run some tests.
actually I am not using a relay such as the one in my drawing, I am using an SSR relay rated at 150A, I read somewhere that the main cause of sparks as you mentioned is when switching the relay during load, I always thought that if everything is connected when turning on the ESC with full throttle or that the  ESC is off when switching the relay on/off – there should not be any sparks, what type of relay did you use? Can you recommend one rated for 150A?
3)	Good to know Mathew I understand now that it is not recommended to exceed 5A charging current so I will stick to 5A.
do you know what is the reason behind it? I mean… it is confusing, the Lipo is rated 1C and 1C is 10A charging so what is the logic behind the 5A rule?

Thank you!!
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-05-20T04:23:10.733Z Reads: 68

```
It is safe to use two BMS's in parallel controlling two separate packs.

A solid state relay is fine to use.

Also, he should NOT be using a 50V power supply. These packs are in parallel. It needs to be 25.2V
```

---
## \#5 Posted by: eranmo Posted at: 2018-05-20T04:35:44.886Z Reads: 70

```
Thanks David.

So do you see any issue with 2 x 25.2v/10A BMS and a single 25.2v/25A charger Or should I limit the BMS charging current to 5A?
```

---
## \#6 Posted by: TowerCrisis Posted at: 2018-05-20T04:52:06.071Z Reads: 70

```
You just need to get a charger that is limited to 10A. Since it's charging both 10A will be fine.

A 25.2V 10A charger will work. It must be a CC and CV charger.
```

---
## \#7 Posted by: eranmo Posted at: 2018-05-20T05:03:13.757Z Reads: 69

```
Thanks David, 
I do not understand, a 10A charger is capable of providing max 10A, if each of my BMS take 10A for charging the charger cannot provide the 20A current both BMS will draw
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-05-20T05:06:53.172Z Reads: 66

```
Ah crap, didn't see that the were in parallel i just assumed the were in series my mistake. Yes use a 25.2V charger. And with the 5a rule i have no idea. It will always be healthier for the cells to charge at a slower speed but fast charging works too. I'd say 5a is just about the sweet spot between fast and healthy.
Also, @TowerCrisis can he not use only one BMS for the packs as the are in parallel? Eg connect cell 1 from pack 1 and cell 1 from pack 2 to the same balance ports on the BMS? 
And also, i read earlier that SSR's will use about 3% of your power when using it as the main switch and that they emit a whole lot of heat which you don't really want.
This guy has designed a big ol switch that seems to look very promising. 
http://www.electric-skateboard.builders/t/fatboy-sparky-switch-300a-60v-anti-spark-switch/51532/52
Also, when will you ever draw 150A? That is a shitload of current
And (2) the spark is usually from initial connection. The large capacitors in the ESC have a very low resistance of between 4-100milliohm upon initial connection. This essentially makes the caps a short circuit before they are charged up. That's where el sparko comes from. 
Hope this helps :slight_smile:
```

---
## \#9 Posted by: mynamesmatt Posted at: 2018-05-20T05:09:07.796Z Reads: 58

```
If a BMS says 10A, that means the maximum current it will TAKE not how much it will DEMAND. 
So what david is saying is, if you use a 10a charger and have the batteries in parallel, each battery will charge at the right voltage of 25.2V but the charger will only push 5a to each battery as its Parallel
```

---
## \#10 Posted by: eranmo Posted at: 2018-05-20T05:22:56.029Z Reads: 54

```
Thank you all guys!

That’s exactly what I needed to know…
I am using this SSR (the 150A version): [150A SSR](https://www.aliexpress.com/item/NEWEST-stable-quality-Power-relay-100A-DPDT-12V-24V-220V/480173903.html?spm=a2g0s.9042311.0.0.27424c4deySjbb)

I also have an alternative to install 2 x 5A auto charger (cost about 17$) inside my setup: [Compact Auto 6S charger](https://hobbyking.com/en_us/turnigy-b6-compact-50w-5a-automatic-balance-charger-2-6s-lipoly.html) And a 18v 10A DC power converter: [18VDC Power supply ](https://www.aliexpress.com/item/Regulated-Switching-Power-Supply-DC18V-2A-3A-5A-10A-20A-Swich-Driver-Transformer-AC110V-220V-to/32844538856.html?spm=2114.search0104.3.2.687434ff30xjEU&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10068_5722815_10342_10343_10340_5722915_10341_5722615_10696_10084_10083_10618_10307_5722715_5711215_10059_308_100031_10103_10624_10623_10622_5711315_5722515_10621_10620,searchweb201603_19,ppcSwitch_5&algo_expid=1c316b0d-b846-4822-a4ea-485247a9abd6-0&algo_pvid=1c316b0d-b846-4822-a4ea-485247a9abd6&transAbTest=ae803_2&priceBeautifyAB=0) and achieve the exact same thing as what i draw in my BMS design but 70% cheaper, is that make any sense to you?
	
BR,
Eran
```

---
## \#11 Posted by: mynamesmatt Posted at: 2018-05-20T05:46:08.901Z Reads: 48

```
I wouldnt personally install 2 charger into your enclosure as this would add another half a kilo to your setup and would make it super damn bulky as you already have 2*10ah batteries sitting there. You should only really make it so heavy as you have to carry it ya know! ;)
As i said, an SSR will work but not for a long time, will get hot and therefore use power. I would definitely recommend the FatBoy switch as opposed to some $4 thingo
```

---
## \#12 Posted by: eranmo Posted at: 2018-05-20T06:10:16.531Z Reads: 42

```
Thanks a lot.
I will do as you suggested.
```

---
## \#13 Posted by: mynamesmatt Posted at: 2018-05-20T06:12:39.441Z Reads: 38

```
No worries man, keep this thread updated on how the build turns out!!
:smiley:
```

---
## \#14 Posted by: eranmo Posted at: 2018-05-20T06:24:18.264Z Reads: 34

```
I will :slight_smile:
```

---
## \#15 Posted by: eranmo Posted at: 2018-08-22T14:49:48.420Z Reads: 27

```
Hi Guys.

While building the setup I showed above I realize something in your comments that just doesn't adds up.
If I have 2 BMS's connected in parallel taking power from the same single 25.2v power supply - why does it matter if the power supply is rated at 10A or 1000A (for example)? 
I thought that what determine the amount of Amps going in to the Lipo is the BMS rated Amps and not the PSU, right? 
choosing a PSU with more rated Amps that I actually need (30% more than I need) will keep the PSU cooler and the charging procedure will be more efficient, if both BMS's are rated at 5A max charging current why not choose a 15A Power supply so each BMS can safely take 5A?


BR.
Eran
```

---
## \#16 Posted by: eranmo Posted at: 2018-08-24T06:03:46.914Z Reads: 24

```
Hi Guys, I posted a question on this page below regarding your comments about the PSU, any chance i can get your comment again? i am during the process of soldering everything, need to make sure i am not making mistakes...
```

---
## \#17 Posted by: mynamesmatt Posted at: 2018-08-24T07:28:41.139Z Reads: 23

```
So, what determines what amperage goes into the lipos is the strength of the PSU. Eg if the bms can take 60a, that's the most it can take. If the psu can push 10a, that's what it will constantly push into the batteries. So if you have a 5a bms with a 10a psu it will cook the bms
```

---
## \#19 Posted by: mynamesmatt Posted at: 2018-08-24T08:14:43.430Z Reads: 26

```
The psu will not stay cooler. 50a is what it pushes and it will always push it. The batteries are not drawing power from the psu, the psu is pushing power into the batteries and therefore will run what it is rated at.
The easy solution, whatever charge amperage you want, get a slightly higher rated bms. ez
```

---
## \#21 Posted by: TowerCrisis Posted at: 2018-08-24T16:32:39.957Z Reads: 23

```
What's most important is what the battery is rated to charge at. If you want to preserve the life of the battery you will charge at a low amperage. A 0.5C rate of charge is good for the cells, which means that when in parallel the most you can give the pack is 10A. This is separate from the BMS. The BMS will not pull or push power. All it does is balance cells and nothing else (assuming normal operation).

A lipo cell will draw as much current as it can. You need to limit that.

A 3.2V cell that is fed a **constant voltage** source will draw too many amps and puff.

That is why you need to charge lipos with a **constant voltage AND constant current** source. This kind of supply will have a hard cap on current.

This is the most important thing to understand. A10A 24V CC CV charger will supply as many volts as it can up until either the voltage reaches 24 volts **or** the current reaches 10A. The important distinction is the OR. The voltage will never be above 24V. And the current will never exceed 10A. It limits this by decreasing the voltage until current decreases to whatever the charger is rated at.

You should not use a bench power supply to charge a pack as a permanent setup. You should use a brick charger, lile the form factor a laptop charger has. This is because It is not adjustable by the user. If you're using a bench power supply you could knock a dial or mess up the current or voltage accidentally and end up cooking your batteries. 

You NEED a CC CV charger.
```

---
## \#22 Posted by: TowerCrisis Posted at: 2018-08-24T16:46:02.747Z Reads: 23

```
THIS is a good charger. http://www.batterysupports.com/22v-252a-7a-lithium-ion-battery-charger-6s-6x-36v-lion-lipo-p-476.html

It will charge your pack fairly quickly and is from a relatively reputable source. Please note that you should always be charging these packs in parallel. That way you're only putting 3.5A into each one. If you only charged one pack it would get the full 7A, which will admittedly charge it fairly quickly, but it also isn't particularly great for the cells.

Make sure that the two packs are at exactly the same charge before connecting them permanently in parallel.
```

---
## \#23 Posted by: eranmo Posted at: 2018-08-24T16:57:54.680Z Reads: 22

```
Thanks David.

I agree with you but the problem with CC CV Chargers against plain PSU is the cost and for no reason at all in my opinion, I am talking about few hundreds of $ differences when it comes to high Amps.

I can order a High Quality Fixed & Non adjustable 25.2VDC power supply rated at 50A, connect 5A (or less) Current regulator/Step Down module to each of my 5A BMSs to ensure the BMS will not get more than what i intend to supply - this kind of setup gives me the ability to charge from the same 50A power supply - 10 different 5A BMSs/Lipos **simultaneously.** with a single cable instead of having 10 different 5A Chargers charging each Lipo/BMS

I still dont understand why I shouldn't go with this approach.

Thanks for all your assistance...
```

---
## \#24 Posted by: TowerCrisis Posted at: 2018-08-24T17:21:08.598Z Reads: 23

```
Are you really going to be charging 10 packs at once?
Because a quality 50A 25V power supply isn't going to be cheap either
```

---
## \#25 Posted by: eranmo Posted at: 2018-08-24T18:28:49.592Z Reads: 20

```
25.2VDC 50A power supply cost 110$ including FedEx shipping, on the other hand -  25.2V 50A CC CV charger will cost most likely 4 times than that which i really dont understand why, it doesnt make sense as it is the exact same thing.

Current Limiter based on Resistor cost 1.5$, I can also use 5A Diod which will cost 0.5$, I can place any of these on the BMS to protect the current flow.

WDYT?
```

---
## \#26 Posted by: TowerCrisis Posted at: 2018-08-24T19:19:56.774Z Reads: 18

```
I think I'll need a more in depth description of the circuit to give an opinion. If you could draw up a circuit diagram that would be great.
```

---
## \#27 Posted by: eranmo Posted at: 2018-08-24T19:33:51.919Z Reads: 19

```
Sure, I will draw one thanks
```

---
