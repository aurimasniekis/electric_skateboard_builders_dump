# Choosing a BMS and charger

### Replies: 33 Views: 4389

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-05-02T06:29:47.883Z Reads: 414

```
This is the second post I'm making about this subject because I am confused.
So I'm upgrading my board and I want an easier charging solution, I read about BMS's and it seemed like the best (and only?) option.
I figured out how to connect a BMS to a board, where to solder and stuff, but what I still don't understand is the difference between a 3$ 6s BMS and a 50$ 6s BMS.
The only difference I can spot is the difference in Amps, does that mean the speed it's charging at?
How many amps will not go too slow for two 3s 8000mAh batteries in series?
And am I supposed to use one of those cheap eBay chargers?
When I thought I had it figured it I was thinking of getting these two:
http://www.batterysupports.com/22v-252a-7a-lithium-ion-battery-charger-6s-6x-36v-lion-lipo-p-476.html
http://www.batterysupports.com/22v-24v-6s-45a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-477.html
But the shipping to my country alone is 110$, thats too much.
If anyone knows where to get these parts on another site that would be great too.
Any help aprecciated
Thanks
```

---
## \#2 Posted by: Quezacotl Posted at: 2018-05-02T07:26:50.267Z Reads: 394

```
Usually the amps highlighted on the BMS ads are the discharge amps, meaning that you can put that much current through to electronics until the overcurrent protection kicks in.

Quality is also an factor when you compare them.

If you want cheap, then Aliexpress and eBay.
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2018-05-02T09:43:02.901Z Reads: 376

```
You have any specific BMS's to recommend?
```

---
## \#4 Posted by: Migro Posted at: 2018-05-02T09:58:04.351Z Reads: 367

```
So your setup is 6s right are you using a vesc or what? if you are you can choose to buy one of the cheaper ones since you can then bypass the discarge. Beacuse the cheap ones are rated to 10A depending on which one. Chargeing dosent require that many amps i think my charger is 2 Amps. But if you are using a bms for dischare it needs to be alot higher since the motors is taking alot. 
The pros with the expensive one:
-Safe charge and discharge, meaning your cells is being messured when chargeing and discharging.

The pros with the cheap one:
-Its cheap, and many people finds that this is enough. With a vesc you can set voltage cut off limits. 

Im not sure how much your motors is drawing at its high. But could probalby find a cheaper charger. 
https://www.ebay.com/itm/Power-Charger-6S-21-6V-22-2V-25-2V-2A-For-Li-ion-LiPo-Lithium-Battery-US-Plug/222567512106?hash=item33d20eb82a:g:wfkAAOSw1BlZWSLp

Thats the one i've got, but mine is for 12S meaning a 52V or so. The voltage doesnt really matter aslong as it is more than your batteries max.
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-05-02T13:19:12.325Z Reads: 330

```
Alright, yeah I just bought a vesc, it's on its way, and I really only need a BMS for charging and not discharging.
Do you have any BMS's you recommend? I can't seem to find any just randomly searching online
And about that charger, isn't it too slow for 16000mAh? 
Thanks for the response
```

---
## \#6 Posted by: RazzleDazzle Posted at: 2018-05-02T13:19:16.632Z Reads: 317

```
Do you have a recommendation for a good BMS for a 10S4P with the samsung 30Q batteries?  The price isnt that much of an issue, i'd choose quality over price.
```

---
## \#7 Posted by: petter Posted at: 2018-05-02T14:01:52.821Z Reads: 318

```
Hi ShakeNBake

I'm actually sort of in the same situation as you and looking for a BMS/charger solution. 

But i can give you some insight into how capacity and charge time works:
* You have a 8000 mAh battery, even though you are using two 8000 mAh batteries. This is because you have them in series, if you put them in parallell it will make a 16000 mAh or 16 Ah battery. 
* To figure out a rough charge time, take your battery capacity(8000 mAh/8 Ah) and divide by the charger current(2 A): 8 / 2 = 4 hours.

In reality there is some powerlosses to heat when charging, say 10%. But you also will not be using the stated 8000 mAh, doing so will destroy your battery. Most likely you will only use 6000 mAh or maybe 6500 when the battery is completly flat, so this will put you charge time at 3-3.5  hours. 

So now it's up to you to decide if that is a good or bad charge time, personally I'd say it's quite alright. if not then get a stronger charger, at 4A you will cut the time in half. Though i'd recommend that you don't exceed 6A, slower charging is better for the batteries.
```

---
## \#8 Posted by: Migro Posted at: 2018-05-02T14:19:01.644Z Reads: 284

```
The problem with the charger is that what i understand that its safer, but you could go for a 4amp charger. Like petter said. 


For you @RazzleDazzle you need to find one that suits you i bought mine at http://bestechpower.com/
The only problem that you need to buy atleast 2 units at once. Mine was lipo so dont know about diy li-ion packs. And again you can choose to get one with low amps continues or a higher one that suits your motor draw. So that it protects the cells when chargeing and dischargeing. :slight_smile:
```

---
## \#9 Posted by: ShakeNBake7000 Posted at: 2018-05-02T15:03:45.957Z Reads: 279

```
Thank you! that makes more sense, 4 hours is a little too long so maybe the 4A charger that will be around 1.5 hours?
I've been looking around on http://bestechpower.com/ and i cant find a non-discharge bms, do they not have them or am i missing something?
```

---
## \#10 Posted by: Migro Posted at: 2018-05-02T15:52:23.476Z Reads: 268

```
You need to look for the ones with a low continues current.
And then find at topic in here on how to charge only. :slight_smile:
```

---
## \#11 Posted by: petter Posted at: 2018-05-02T16:22:12.215Z Reads: 258

```
Yeah, what i think Migro means is that you buy a normal BMS, connect it but still leave your ESC and motors etc connected just as they are now.

![image|216x233](upload://tdpKmLpqRWQHO87rJ353OHDUVki.png)
This picture for example is wired for a BMS with a high discharge rating, say a 60A BMS for a 50A load?
Should work fine.

If you instead have a low discharge BMS and still need to pull high amps you can bypass the BMS with the discharge wire. That is, in this picture you would move the black discharge cable from P- to B-.
```

---
## \#12 Posted by: ShakeNBake7000 Posted at: 2018-05-03T00:41:39.301Z Reads: 237

```
Thanks for the responses, So in that picture, where does the xt90 connect to? the battery or the vesc?
```

---
## \#13 Posted by: petter Posted at: 2018-05-03T08:27:10.048Z Reads: 228

```
The xt90 connects to the vesc :) 

The stack of red and white circles on the are supposed to represent the battery
```

---
## \#14 Posted by: ShakeNBake7000 Posted at: 2018-05-03T09:13:10.774Z Reads: 225

```
Oh lol, how didn't I figure that out haha
The diagram shows a discharge+charge connection? So if I want a "charge only" BMS, I need to put both the + and - of the battery on the b-? so the current won't go "through" the BMS?
Another thing, BMS's capable of high discharge are more expensive, and I don't need/want to have another protection because I already have a vesc to control the voltage, so I need to look for a bms with a higher charge rate (30-50A?) and the lowest possible discharge rate? (just to drop the price considering I'm not going to use the discharge function at all) don't know if that logic is stupid or fine.
Thanks
```

---
## \#15 Posted by: petter Posted at: 2018-05-03T12:19:28.664Z Reads: 216

```
Um.. No.

It's actually quite simple but a bit confusing.

* You connect the vesc to the battery. Just like you probably already have.

* connect charge cable to bms and bms to the battery. 

That is all. This is also why its charge only, since the vesc is not connected to the bms at all.
```

---
## \#16 Posted by: ShakeNBake7000 Posted at: 2018-05-03T13:28:09.459Z Reads: 204

```
Oh, thanks for explaining
Only thing I still don't get, is how I choose my bms. I see so many models in here and I cant tell the difference:
http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/
How much continues current do i need?
```

---
## \#17 Posted by: petter Posted at: 2018-05-03T13:49:35.681Z Reads: 198

```
![Screenshot_20180503-154417|281x500](upload://23WRYGgaiXlJHbWlk2sYGtbxbdm.png)

Here you see both charging and discharge. Of these it's only charging that you are interested in.

But even with a 4A charger, pretty much any bms will be good enough so i'd say pick one you feel will fit in your enclosure.
```

---
## \#18 Posted by: ShakeNBake7000 Posted at: 2018-05-03T13:53:18.041Z Reads: 189

```
I cant explain how much youve helped me, thank you.
One last thing, i looked on amazon, ebay and aliexpress and couldnt find 1 4A charger, only 2As
Am I just not looking right or an i supposed to buy them somewhere else?
Edit:
talking about a 22.2V-25.2V charger for 6s
```

---
## \#19 Posted by: petter Posted at: 2018-05-03T14:44:13.939Z Reads: 193

```
Glad i could help :)  Also since i'm pretty much looking for the same thing it's nice to see all the options

https://www.alibaba.com/product-detail/Amazon-hot-selling-Scooter-25-2V_60747602423.html?spm=a2700.7724857.main07.156.442f1e27hHVqqQ

You are right though they were not very common, there seems to more of this style: 
https://www.amazon.com/25-2V-Charger-Li-ion-Battery-Aluminum/dp/B075162GVD

Just remember to tell us what you decide to get in the end!
```

---
## \#20 Posted by: ShakeNBake7000 Posted at: 2018-05-03T14:47:53.297Z Reads: 185

```
The 4A one looks good, thanks! ill look at all the bms's and choose one, problem is i cant see the pricing so it makes it harder to pick one
```

---
## \#21 Posted by: ShakeNBake7000 Posted at: 2018-05-03T18:52:49.810Z Reads: 180

```
![2018-05-03_21h51_34|633x500](upload://sMYDdMrTwlTxon1i10Ef5BGx00X.png)
So the 4A charger can come with many different tips, which one should i get?
Do I need the female counterpart as well? and solder it to the bms?
```

---
## \#22 Posted by: petter Posted at: 2018-05-03T20:12:19.362Z Reads: 171

```
Yeah, you need the female as well. 
I'd go with one that atleast have some protection, maybe this one. There is some other threads where i read about these connectors, i have not tried this one myself but it's probably good enough. Otherwise you could consider getting a proper high quality plug and change the connector on the charger as well, but i'd probably try this one out first

https://www.ebay.ca/itm/10pcs-Iron-5-5x2-1mm-DC-Power-Female-Jack-Socket-with-Waterproof-Cover-Ring/321888973907?hash=item4af213f453:g:My8AAOSwo0JWF4Kv
```

---
## \#23 Posted by: ShakeNBake7000 Posted at: 2018-05-03T20:18:39.177Z Reads: 166

```
So where do i connect the port to? somewhere on the bms?
Edit: 
I prefer a bigger port, sturdier one, which one of these is the best one or is there no actual difference other than looks?
![2018-05-03_23h41_31|690x324](upload://2v4TgpxW7UfiCAnnchKgoNVwoC8.png)
I can choose which port I want on the charger so why not get a better one :slight_smile:
```

---
## \#24 Posted by: petter Posted at: 2018-05-03T21:14:18.035Z Reads: 154

```
Yeah, the charging port usually connects to the battery positive and P- on the bms. But there should be a description of this for the actual bms you choose.

Also, lol. That is some unusual set of plugs. I guess you could get the XLR or the GX16 but they might feel very big. Also i'd check first for a waterproof port for the board. Even if you have a sturdy port it's no fun if it's full of dirt.
```

---
## \#25 Posted by: ShakeNBake7000 Posted at: 2018-05-03T21:17:08.549Z Reads: 152

```
Yeah those are kinda random lol, which plug are you using right now? can reccomend anything?
```

---
## \#26 Posted by: petter Posted at: 2018-05-03T21:38:30.674Z Reads: 154

```
On my raptor there is a 5.5x2.1(or possibly a 5.5x2.5). Works great so far.

So i'd probably go for that one...

But if you want a sturdy one, i'd look into something like this:
https://www.amazon.com/Panel-Mount-Waterproof-Connector-Socket/dp/B00M9AF46Y

Edit: if you do look for a different one, do think about the fact that one side is conncted to a big lipo and the other to a live charger. The barrel connectors are pretty good at not getting shorted for both the male & female end.
```

---
## \#27 Posted by: ShakeNBake7000 Posted at: 2018-05-03T21:45:51.315Z Reads: 152

```
I think ill go for the 5.5x2.1, the female plugs you sent
About the BMS, I wanted a small one and 10A is enough for charging, but how can i actually buy it lol, do i need to email them and ask for a price?
http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCB-D103.html
should work fine right?
or mabye this one?
https://www.ebay.com/itm/6S-10A-24V-25-2V-Li-ion-Lithium-18650-Battery-BMS-PCB-Protection-Board-Balance/322460026383?hash=item4b141d860f:g:Zx8AAOSwzT5ZeE4B
It's very cheap so mabye its not that reliable
Edit:
Just got the 5.5x2.1 charger and female plugs with the waterproof covers, thanks
```

---
## \#28 Posted by: petter Posted at: 2018-05-04T17:35:44.393Z Reads: 147

```
Yeah sure, they both look alright.
```

---
## \#29 Posted by: ShakeNBake7000 Posted at: 2018-05-04T17:55:41.490Z Reads: 148

```
Thank you, I just ordered it, all the parts are on their way
You've helped me so much, from understanding to finding the right product and I Can't thank you enough.
```

---
## \#30 Posted by: Redfire1 Posted at: 2018-06-16T15:15:15.427Z Reads: 132

```
@Quezacotl hi can you help me please to sort out my stuff,I am using this bms and charger to charge my 2 5S lipo,I trying since yesterday but still nothing,what can I check,I get it to charge one time.36V 2A Akkuladung Ausgang 42V 2A Ladegerät Eingang 100-240 VAC Lithium Li-Ion Li-Poly ... https://www.amazon.de/dp/B074W8GK9D/ref=cm_sw_r_sms_apip_8qmEnM1ZPCIi9
DC42-45V Eingang Batterie Schutzbrett mit Ausgleichfunktion BMS PCB Board für 10 Pack... https://www.amazon.de/dp/B07512K278/ref=cm_sw_r_sms_c_api_GKsjBbH9P0GDN![image|375x500](upload://9ODeWUD8ZtQrYMUPBw9OjpDZGgk.jpeg)
```

---
## \#31 Posted by: Quezacotl Posted at: 2018-06-16T22:20:01.709Z Reads: 116

```
That question is not specificly for me. It's a generic question anyone can answer.
And it's too broad, you need to be more specific. All i can tell is to check that the wiring is correct and if the bms is ok.
```

---
## \#32 Posted by: Redfire1 Posted at: 2018-06-17T08:27:10.336Z Reads: 111

```
Thanks I get it to charge don’t know how.I dudnt change anything I just keep plug-in and out and then the red light came on.
```

---
## \#33 Posted by: Gpole Posted at: 2019-05-02T06:54:08.219Z Reads: 53

```
What do you guys think of this charger; https://www.mouser.se/ProductDetail/MEAN-WELL/ENC-360-48?qs=5aG0NVq1C4yrxUDGkAE0zg%3D%3D
```

---
