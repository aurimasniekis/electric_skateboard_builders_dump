# Where to find a good BMS

### Replies: 28 Views: 5635

## \#1 Posted by: Brando Posted at: 2017-02-12T03:02:41.211Z Reads: 403

```
I have built two esk8 boards, but have not included a BMS on either. I am building a third and forth, and decided to look into BMS so that I dont have to use an annoying LiPo charger.

I am having some trouble finding a good one but I came across [this](https://bmsbattery.com/bmspcm/733-10s-16s-50a-lipo-bms-system-battery-management-system-bms-pcm.html)

I'm looking for 8S or 10S. Does anyone have recommendations for a site or specific product?
```

---
## \#2 Posted by: barajabali Posted at: 2017-02-12T04:14:23.795Z Reads: 405

```
If you find a good bms or even ANY bms in the US, let me know. 

far as i know they only come from china
```

---
## \#3 Posted by: Brando Posted at: 2017-02-12T04:24:17.495Z Reads: 402

```
Dang. Ill take the U.S. part out of the title. Question still stands though. Where are people's favorite/fastest sellers?
```

---
## \#4 Posted by: willpark16 Posted at: 2017-02-12T04:25:31.787Z Reads: 404

```
battery supports is so far the most reliable or besttech
```

---
## \#5 Posted by: Eboosted Posted at: 2017-02-12T04:26:43.585Z Reads: 405

```
Brando if you want to use the BMS to balance the cells at charge, then you could use a lower amperage and cheaper one. 

If you want to use it for discharge as well get the battery support one.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-02-12T04:29:24.153Z Reads: 404

```
Bestech comes with FET heat sinks and a built in E-switch.
I've been using them for long time with no issues.
They handle 80a constant and 240a peak
over charge protection, over discharge protection, overheat protection, over current protection, external short protection
And overcharge protection during regen braking. No shutdown when braking on a full battery. ( I've have personally tested that)
Battery Support look good but I think these are better. And I've personally had difficulty getting parts shipped from Battery Suports. My order was rejected at customs and it would up taking so long that I just canceled it and went with Bestech. 
Also Bestech lets you choose various settings during order process. I don't think Battery Supports does that.
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#7 Posted by: Eboosted Posted at: 2017-02-12T04:41:46.300Z Reads: 370

```
Wow Namasaki that's a great review! 

Have you tested the Battery Supports one and got the VESC shutdown issue? What does the Bestech do with the regen current when you brake with a fully charged battery?
```

---
## \#8 Posted by: Namasaki Posted at: 2017-02-12T04:47:01.373Z Reads: 348

```
It bleeds off excess voltage same as it does when balance charging.
I have never used Battery Suports bms, I tried but they couldn't get my order through customs.
(it's been a while since then, maybe they have resolved their shipping issues.)
I have never had regen shutdown but have heard of others having that issue.
I don't know if Battery Supports protects during regen or not.
I believe those who have shutdown while braking on full battery are either not using a bms or using a charge only bms.
```

---
## \#9 Posted by: Eboosted Posted at: 2017-02-12T04:56:03.312Z Reads: 329

```
Well, I have two boards and first hand experience with Battery Supports BMS:

I can confirm that with my first board 13/36T ratio I have shutdown when battery is full and I brake hard, on the second board 13/40T ratio I don't get the shut down, both with battery supports 10S 60A BMS.

[img]http://www.batterysupports.com/images/36V%2010S%2060A%20Lithium%20BMS.jpg[/img]

I might go with the Bestech one, however I didn't find any "add to cart" button on the link you provided, where do you usually purchase it from?
```

---
## \#10 Posted by: Eboostin Posted at: 2017-02-12T04:59:48.634Z Reads: 306

```
You have two of the same BMS? One shuts down and one doesn't?
```

---
## \#11 Posted by: Eboosted Posted at: 2017-02-12T05:07:05.054Z Reads: 309

```
Yes, that's correct.

Today I started a short experiment, I modified the connections on the board that shuts down on full charge, I'll used the BMS only for charging, discharge will be done directly from the battery, if VESC still shuts down then the problem was never related to the BMS, otherwise the BMS is the culprit
```

---
## \#12 Posted by: Namasaki Posted at: 2017-02-12T05:39:19.060Z Reads: 309

```
Maybe the Vesc is shutting down. Do you have same Vescs and settings on both boards?
Bestech accepts orders via email. 
They also accept Paypal. 
There minimum order qty is 2. 
If you want to place an order, 
Send your order request to
lucy@bestechpower.com
```

---
## \#13 Posted by: chuttney1 Posted at: 2017-02-12T06:35:09.040Z Reads: 305

```
I'll suggest a very good, but not cheap option I found on endless-sphere. It is not a plug and play BMS and requires knowledge from the user to use the outputs to other sensors. I used this model in my build.

This is the Energus 150/750 amp BMS. Peak discharge is 150 amps. Max continuous discharge is 60 amps. Comes with an aluminium heatsink. Can be expanded to 750 amps with an external current sensor and relay. This is a smart BMS. It can take up to 16S and any cell chemistry. Ships from Lithuania. 

<img src="/uploads/db1493/original/3X/8/f/8f47059b50777852dee3f6c4b71c110f674e1559.jpeg" width="600" height="450">

https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36
```

---
## \#14 Posted by: smurf Posted at: 2017-02-12T06:41:13.679Z Reads: 289

```
Bestech has a smart bms

http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/BMS-D338.html
```

---
## \#15 Posted by: Eboosted Posted at: 2017-02-13T06:54:25.680Z Reads: 272

```
Why would anyone need a smart BMS, what are the benefits?
```

---
## \#16 Posted by: willpark16 Posted at: 2017-02-13T06:58:42.758Z Reads: 268

```
Voltage change without getting a new bms
```

---
## \#17 Posted by: chuttney1 Posted at: 2017-02-13T09:08:10.693Z Reads: 263

```
Depends on application, though. Smurf linked one as basic smart BMS. I linked one as a basic smart BMS plus outputs for other sensors and stuff.
```

---
## \#18 Posted by: Tuomalar Posted at: 2017-02-13T14:32:21.929Z Reads: 255

```
I need as small bms as possible only for charging with 4A charger. Any suggests? Low price would be nice too.
```

---
## \#19 Posted by: Eboosted Posted at: 2017-02-14T06:21:08.644Z Reads: 246

```
I'm also looking for this.

@Tuomalar are you going to use the discharge directly from the battery?
```

---
## \#20 Posted by: Tuomalar Posted at: 2017-02-14T06:59:23.194Z Reads: 246

```
That's what I was thinking. 
At first I planned to do "balancer box" so I can go without bms, but frequently plug that between charger and battery.

http://m.ebay.com/itm/142209480707 Are these garbage? I'm very suspicious with these.
```

---
## \#21 Posted by: Akadis Posted at: 2017-07-20T08:18:10.335Z Reads: 204

```

Hey

Is the price tag worth it because i am thinking about buying one? 

Have you tried the expansion with the external current sensor?

can i install the external sensor and use it on 70Amps?

Thanks
```

---
## \#22 Posted by: jotatsu Posted at: 2017-07-20T13:03:01.525Z Reads: 198

```
 [quote="Tuomalar, post:20, topic:17583, full:true"]
That's what I was thinking. 
At first I planned to do "balancer box" so I can go without bms, but frequently plug that between charger and battery.

http://m.ebay.com/itm/142209480707 Are these garbage? I'm very suspicious with these.
[/quote]

Lets just say that those are the things in hooverboards, cheap ones. Look , theyt come free with 20 batteries XD

http://www.ebay.com/itm/NEW-LG-36V-4-4AH-BATTERY-PACK-18650-EBIKE-VAPE-POWERWALL-BATTERIES-20-CELLS-BMS/172630688902?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649
```

---
## \#23 Posted by: chuttney1 Posted at: 2017-07-20T23:34:18.452Z Reads: 188

```
The Energus BMS is only worth it if you can code your own programs for the expansion ports for external sensors and other stuff. The plus side is working with any battery chemistry and setting overcharge and discharge cutoff points. It has a precharge function to not damage electronics on startup. Their external current sensor is way above what you will be using and not really needed unless you have plans to use in an ebike or car. You will not be drawing 70 amps on an eskate. Go with a cheaper BMS as mentioned in the forum.
```

---
## \#24 Posted by: MaroonArcher Posted at: 2017-11-14T04:20:02.565Z Reads: 151

```
Hey guys if I don't hook up the p- on my BED will my bms still balance charge my wires. The p- is shown as the negative load to my device. The bms I have is only rated to 30A and I need 45A<img src="/uploads/db1493/original/3X/9/a/9a251e3941cccb9942241acc03637d7f80e26d8f.jpg" width="374" height="500">

Mind this I am using a 13s bms not a 10s this diagram is in a book I got for diy lithium batteries
```

---
## \#25 Posted by: rich Posted at: 2017-11-14T16:10:41.419Z Reads: 137

```
Of course it balance charge when connected for charge only. Just wire it in parallel, Your negative lead from the battery goes to B- and to negative discharge as well, easy! No need to connect P- if used for charging only.
```

---
## \#26 Posted by: Esk8enginneer Posted at: 2019-01-31T01:34:15.588Z Reads: 51

```
Do they have any that will protect the lipo cells from over discharge.  All the one I see on the site only go up to 3.0v for protection.  3.4v would be the limit for lipo.
```

---
## \#27 Posted by: Namasaki Posted at: 2019-01-31T06:34:05.268Z Reads: 48

```
Ya, unfortunately they are more geared for Li-ions when it comes to over discharge detection.
Best thing to do with Lipos is to monitor your voltage either with an app or with a meter mounted on top or through the top of your deck.
You can also set the Vesc battery cutoff start at 36v and the cutoff end at 34v for 10s.
```

---
## \#28 Posted by: Esk8enginneer Posted at: 2019-01-31T07:00:17.885Z Reads: 50

```
I just got in on the group buy for the 3rd batch of the DieBieMS.  My understanding is you can set it to whatever you want through the config tool.  Thanks for the reply.
```

---
