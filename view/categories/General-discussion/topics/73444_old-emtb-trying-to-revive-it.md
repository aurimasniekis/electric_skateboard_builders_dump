# Old EMTB. Trying to revive it

### Replies: 17 Views: 459

## \#1 Posted by: Sr.Agaporni Posted at: 2018-11-04T20:22:35.467Z Reads: 114

```
Hi folks! I am new to eboards. I have been given an "old" mountainboard that I want to revive for my son. It doesn't have remote to control it. I have been checking everything as it should work, but without the remote I can't do much from here.

Can you help me to fix this board with the cheaper way? At the moment, I am not sure how to proceed with:
- Bushings: there was bushings on the eboard, but they were completly rigid and I removed them.
- Remote: I don't have any, and I am not sure If I can find any compatible with this setup.
- Battery: easy to fix with new PB batteries, but I think I will go with LiPo ones as I have some spare 5s 5000mah from my ebikes.

I am quite confortable with the electronics related to the "E" world as I already bult more than 10 ebikes as a hobby, including a 15kw one. So I only need to learn the basics of the skateboard world.

Some pics I can add:

![20181104_191305|666x500](upload://xOuXRFMw0s1iXAj0yMiLTsIlVqj.jpeg) 
![20181104_191317|666x500](upload://l6GymXmqTlh49ulbAhCrJdv5Z5S.jpeg)
```

---
## \#2 Posted by: b264 Posted at: 2018-11-04T20:30:18.910Z Reads: 92

```
You could put a VESC in it and use a Mini Remote

[quote="Sr.Agaporni, post:1, topic:73444"]
Battery: easy to fix with new PB batteries, but I think I will go with LiPo ones as I have some spare 5s 5000mah from my ebikes.
[/quote]

You need 6S - 11S (some say 12S or 13S is okay, but I disagree) for a VESC.  You could put two 5S in series for 10S.

That's a brushed DC motor.

Could you take a high-resolution photo of that front circuit board and fill out your country in your profile?  That will allow us to help you more.  There may be lower-cost options
```

---
## \#3 Posted by: telnoi Posted at: 2018-11-04T20:34:43.239Z Reads: 85

```
Looks like a mobo 800 type board, brushed motor.. You will find countless rebranded similar looking boards and I imagine the parts for them are cross compatible. 

The trucks at least appear to be identical.
Check the other parts for a comparison.. 

https://mo-bo.de/product_info.php?info=p210_mo-bo-vorderachse-fuer-mo-bo-800-watt--bushing-achse-.html

A replacement remote and receiver alone is around 80 euro or so new. Might find them cheaper.
```

---
## \#4 Posted by: Sr.Agaporni Posted at: 2018-11-04T20:45:59.648Z Reads: 78

```
Thanks! I checked the capacitors on the ESC, it shows 50V, so 12s feels the secure limit as you say.
Here you have a photo of the front board, which I suspect is for the receiver, mainly because it says "xkate GRX1 COM":

![20181104_191311|666x500](upload://1i86WakABBEs5u1IXRmFlL2s2g4.jpeg)
```

---
## \#5 Posted by: Sr.Agaporni Posted at: 2018-11-04T20:47:50.927Z Reads: 73

```
Yeah, it looks very similar, and the motor is brushed as you say.

Can I use the VESC with this motor? I have read about it (open source hardware), but I am not sure if it can handle the brushed motor.
```

---
## \#6 Posted by: telnoi Posted at: 2018-11-04T20:50:18.700Z Reads: 70

```
Yes, you can. 
http://vedder.se/forums/viewtopic.php?t=664

PS, the original was operated at 36V, not 12S.
```

---
## \#7 Posted by: Sr.Agaporni Posted at: 2018-11-04T21:00:38.257Z Reads: 71

```
Nice! So I only need:
- VESC
- Remote
- Receiver

I have found everything in Banggood for about 100€, is it right to fix this monster? I still need the bushings, where can I find them?

![imagen|690x449](upload://hKM2S7r7aPx3deXt3hMizay2GY2.png)
```

---
## \#8 Posted by: b264 Posted at: 2018-11-04T21:04:22.102Z Reads: 61

```
[quote="Sr.Agaporni, post:4, topic:73444"]
I checked the capacitors on the ESC, it shows 50V, so 12s feels the secure limit
[/quote]

No, if the capacitors say 50V -- then 36V would be the most I would use, which means 8S li-ion or 10S LiFePO4 or 3S lead battery
```

---
## \#9 Posted by: telnoi Posted at: 2018-11-04T21:05:58.734Z Reads: 59

```
Get the flipsky 6.x, the 4.x. has issues leading to dangerous cutouts (should be pulled from shops if you ask me).

Are these the bushings? You removed them, hopefully you still have them around (or in memory) to compare

https://cdn.website-start.de/proxy/apps/ilai8i/uploads/paypal/instances/7E25E3CE-A081-4663-9133-665DD7F6FFAA/wcinstances/paypalShop/ac5f9349-7aa1-4c2b-9d67-76cb5e659346/productImage/109.jpg?download
```

---
## \#10 Posted by: luis99945 Posted at: 2018-11-04T21:20:09.515Z Reads: 53

```
or focbox halloween sale
```

---
## \#11 Posted by: Sr.Agaporni Posted at: 2018-11-04T21:20:09.710Z Reads: 51

```
The bushings were half destroyed already, I removed the remaining parts. It looks like the right bushing, are they specific from mo-bo trucks? I mean, is not another brand which makes compatible bushings?
```

---
## \#12 Posted by: telnoi Posted at: 2018-11-05T06:05:01.829Z Reads: 45

```
Just search for 800w mountain board. You'll find a few companies selling these with different branding/then see if they sell replacement parts.
```

---
## \#13 Posted by: Sr.Agaporni Posted at: 2018-11-05T10:41:51.707Z Reads: 40

```
Thanks to all. I finally ordered the parts needed:
- Bushings from powerboard-dealer.de 
- VESC, BMS, LCD display, antispark, transmitter/receiver from banggood.

I will post updates when I update the board.
```

---
## \#14 Posted by: brenternet Posted at: 2018-11-05T11:18:18.255Z Reads: 36

```
Those prices are high.

Flipsky 4.12 on ebay for €50ish (Offer the seller less than selling price, there's loads of these around)
2.4ghz mini remote and receiver on Aliexpress/ebay €20ish
```

---
## \#15 Posted by: pat.speed Posted at: 2018-11-05T12:23:35.566Z Reads: 34

```
I think it is only the 4.20 design that has issues the 4.12 is good
```

---
## \#16 Posted by: brenternet Posted at: 2018-11-05T13:18:01.383Z Reads: 29

```
This is correct 

https://www.electric-skateboard.builders/t/poll-flipsky-information-in-one-place/68940
```

---
## \#17 Posted by: Sr.Agaporni Posted at: 2018-11-06T07:44:14.520Z Reads: 22

```
I read on the forum that Banggood got good offers on VESC, but feels as eBay offers better prices. Thanks for the tip, maybe for next round. 50€ per VESC feels a good choice for future builds in case I go on with this world, at the moment need to learn.

Just in case someone is reading this:
- Banggood: VESC= 68€, mini RC with receiver 24€
- eBay: VESC = 50€, mini RC with receiver 16€
```

---
