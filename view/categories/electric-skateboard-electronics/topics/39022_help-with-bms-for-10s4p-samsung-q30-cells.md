# Help with BMS for 10s4p Samsung Q30 cells

### Replies: 25 Views: 2276

## \#1 Posted by: Olloxan Posted at: 2017-11-22T23:38:31.211Z Reads: 237

```
Hi, 
I am planning on buying the the 10s4p battery from enertion that is is in the Raptor2, the Enertion Spacecell Elite, that is made of Samsung Q30 cells. I want to use it in a DIY Project and look for a BMS.

<img src="/uploads/db1493/original/3X/3/2/323817fb26eb5be25bd60eb22352d39f3e394e76.jpg" width="666" height="500">

I was thinking about using the [HCX-D223V1](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html). My Problem is that I don´t know how the balancing cables of the battery should be connected to the BMS:

<img src="/uploads/db1493/original/3X/2/a/2a5d470863ee4d430a8307a255c6fb3ff1fd7d40.jpg" width="375" height="500">

There are 11 cables coming out of the batter, 10 red ones and a black one. But the scematic of the [HCX-D223V1](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) shows only 10 balancing cables:

<img src="/uploads/db1493/original/3X/5/f/5fc0104f705e884f0c95aa8e084dad878495e3ac.png" width="385" height="500">

**My Questions:**

-How would the battery be connected to the BMS?
-on the website it says that certain parameters of the BMS are adjustable. How are they adjusted?
-Is there a better BMS that I could use?

This is going to be my first build and I have little to no experience with batteries.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-11-22T23:55:50.138Z Reads: 226

```
The connector on the space cell will not fit the Bestech  10s bms.
The bms comes with a cable/connector set 
You will need to remove the balance connector from the battery and splice in the cables that come with the Bestech.
Be careful to snip the balance wires one at a time and don't strip them until your ready to splice them. Then do one wire at a time.
You can easily identify each wire with a voltage meter. 
Connect the black ground probe to the Black main wire of the battery then check each pin with the red probe.
The pin with the lowest voltage is cell 1. the pin with the highest voltage is cell 10.
Cell 1 and 10 will be on the outer edges of the connector. The rest will be in numerical order on the connector.
Best to start with pin for cell 1, snip it's wire and splice it to the wire that goes to pin 1 on the bestech bms and work up in numerical order from there, pin 2,3,4,5,6,7,8   9,10
The Bestech 10s bms comes with two cable sets, 1 with 8 pins for cells 1-8  and 1 with 2 pins for cells 9 and 10.

I have been using this particular bms for over a year on 2 builds and they have been rock solid.
They are very robust.
It is highly recommended that you use some type of static protection while handling the bms.
I use a wireless anti-static wrist band that absorbs any static build up.
https://www.frys.com/product/6932367?site=sr:SEARCH:MAIN_RSLT_PG
```

---
## \#3 Posted by: Olloxan Posted at: 2017-11-23T00:08:14.327Z Reads: 206

```
Cool, thank you very much. On the website it says parameters like the overcharge protection und Overcharge release voltage are adjustable. How are the adjusted? And it seems the minimum I can buy is 2 units? Did you get your BMSs from thier site too or is there another site I can buy it from?
```

---
## \#4 Posted by: WARMAN Posted at: 2017-11-23T00:08:35.775Z Reads: 195

```
You could try and find the raptor 2 bms,maybe someone with a raptor 2 could show you a pic or point you in the right direction.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-11-23T00:12:25.559Z Reads: 191

```
I bought mine directly from Bestech. The settings are adjustable at the factory so you have to request any changes during the ordering process.
I don't know of any vendors for these.
The min order is two.
I have ordered at least 8 of them, 2 of which are on my 2 builds and all the rest I sold on this forum except for 1 that I got for a local skater.
```

---
## \#6 Posted by: darkkevind Posted at: 2017-11-23T00:18:14.076Z Reads: 188

```
[quote="Namasaki, post:2, topic:39022"]
The connector on the space cell will not fit the Bestech  10s bms.
[/quote]

@olloxan

Whilst that is indeed true, you needn't cut the wires off the BMS' to resolder them if JST connector is of the same family as the one on the Enertion pack.
You can simply pop the pins out of the male connector (female pins) on the space cell and pop them in to the one that comes with the BMS....
```

---
## \#7 Posted by: Olloxan Posted at: 2017-11-23T00:21:31.072Z Reads: 185

```
I own a Raptor2 but I am not shure if they make thier own BMS.
The BMS they use is very small, its the circuit below the display (this is the best Picture I have right now)

<img src="/uploads/db1493/original/3X/5/3/53faf48d119b2c9d4ae5f01742114cc64b5e88e0.jpg" width="666" height="500">

I will have a look if I can see anything printed on there.

[quote="darkkevind, post:6, topic:39022"]
Whilst that is indeed true, you needn't cut the wires off the BMS' to resolder them if JST connector is of the same family as the one on the Enertion pack.
You can simply pop the pins out of the male connector (female pins) on the space cell and pop them in to the one that comes with the BMS....
[/quote]


@darkkevind
thanks thats a good Idea
```

---
## \#8 Posted by: Namasaki Posted at: 2017-11-23T00:28:30.492Z Reads: 172

```
[quote="darkkevind, post:6, topic:39022"]
You can simply pop the pins out of the male connector (female pins) on the space cell and pop them in to the one that comes with the BMS....
[/quote]


That is a good idea as long as they are the same size.
I've been at Fry's electronics and seen several tools that they sell for removing the pins.
I think it would be well worth having the tool.
https://www.frys.com/product/1651636?site=sr:SEARCH:MAIN_RSLT_PG
```

---
## \#9 Posted by: thisguyhere Posted at: 2017-11-23T00:31:59.786Z Reads: 166

```
[quote="Namasaki, post:2, topic:39022"]
Be careful to snip the balance wires one at a time and don't strip them until your ready to splice them. Then do one wire at a time.
[/quote]

please, please heed this advice. 

I've melted balance leads snipping them all at once. instant short on a 10s pack is frightening.
```

---
## \#10 Posted by: WARMAN Posted at: 2017-11-23T00:32:52.189Z Reads: 163

```
I doubt enertion make it,too time consuming,if you can find the serial number/model number then your on to a winner,post it here if you do,it will help others out!
```

---
## \#11 Posted by: Olloxan Posted at: 2017-11-23T00:34:41.325Z Reads: 163

```
Ok, cool thanks for your help everyone, I´ll have a look
```

---
## \#12 Posted by: WARMAN Posted at: 2017-11-23T00:36:12.241Z Reads: 163

```
No worries,I might upgrade soon anyway,so if you can find it happy days.
```

---
## \#13 Posted by: darkkevind Posted at: 2017-11-23T01:04:39.106Z Reads: 162

```
No need for fancy tools... I just use one of these....

<img src="/uploads/db1493/original/3X/2/1/211d1b862c61055011959927ed7ee695fd469831.jpg" width="200" height="">
```

---
## \#14 Posted by: Olloxan Posted at: 2017-11-23T09:45:01.197Z Reads: 154

```
Ok, so I have opened it up again and I believe the BMS used is a [BWPB-277](http://www.china-nengyuan.com/product/122976.html). The problem is, my chinese is a little rusty :joy: So I don´t know if its worth the efford to get one of these. I found it nowhere else but on this site. If you have any ideas on how to get one please let me know. And if you know anyone who sells a single [Bestech HCX-D223V1](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) please let me know as well since I can buy them only in batches of at least two from the manufacturer.
```

---
## \#15 Posted by: willpark16 Posted at: 2017-11-23T09:48:41.238Z Reads: 153

```
I've got one of those
```

---
## \#16 Posted by: Olloxan Posted at: 2017-11-23T09:51:57.638Z Reads: 155

```
[quote="willpark16, post:15, topic:39022, full:true"]
I've got one of those
[/quote]

Hi. What are the exact specs on it? (I ask because on the datasheet they say that you can adjust certain paramaters). I live in Germany, would it be possible for you to send it here? How much do you want for it?
```

---
## \#17 Posted by: willpark16 Posted at: 2017-11-23T10:14:57.686Z Reads: 145

```
What did u need it for? I have t tested it so I don't know if it's functional
```

---
## \#18 Posted by: Olloxan Posted at: 2017-11-23T10:35:10.397Z Reads: 142

```
A 10s4p Battery with Samsung Q30 cells
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-11-23T16:25:00.840Z Reads: 135

```
I dropped my pack on my finger cause I accidentally shorted balance wires lol

my pack weighs 7lbs :joy:
```

---
## \#20 Posted by: Olloxan Posted at: 2017-11-26T13:08:42.235Z Reads: 134

```
So if I buy the [HCX-D223V1 10S 37V](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html) BMS, I would adjust the parameters for the Samsung Q30 cells as follows:

overcharge detection Voltage: 4.2V
overcharge release voltage: 4.1V

overdischarge detection voltage: 2.6V
overdischarge release voltage: 3.0V

what should the Over current detection voltage be?

Would this setting be ok for the cells?
```

---
## \#22 Posted by: Lobap Posted at: 2018-02-15T23:39:31.545Z Reads: 106

```
Any news on this? 

I just got a Raptor2 battery for my DIY build, so i will need a BMS.
```

---
## \#23 Posted by: ZackoryCramer Posted at: 2018-02-15T23:54:17.523Z Reads: 106

```
Looks like you need to strip open heat shrink and solder on the BMS balance leads yourself since most of the bms' balance plugs are of smaller size. :cowboy_hat_face: 
Or get a lipo balancer and manually plug the balance leads in for balancing.
```

---
## \#24 Posted by: Olloxan Posted at: 2018-02-19T08:18:43.328Z Reads: 99

```
No, no news, but there is another threat [DieBie JTAG 12s BMS | Gauging Interest | NONPROFIT](http://www.electric-skateboard.builders/t/diebie-jtag-12s-bms-gauging-interest-nonprofit/20947/371). I am looking forward to this BMS
```

---
## \#25 Posted by: Boxer86 Posted at: 2018-06-25T03:23:32.494Z Reads: 70

```
I was just wondering how you went with the bms for the raptor 2 battery as I am looking at doing the same thing? If so what bms did you use and what settings? Thanks heaps
```

---
## \#26 Posted by: Olloxan Posted at: 2018-06-28T06:46:53.401Z Reads: 61

```
Hi, 
I haven´d had time to work on that project but at the moment I am waiting for a BMS like this: [DIY 6S to 12S BMS with CAN](https://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639/290)
```

---
