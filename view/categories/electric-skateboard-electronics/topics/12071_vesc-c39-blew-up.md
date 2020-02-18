# VESC C39 blew up

### Replies: 38 Views: 2616

## \#1 Posted by: Stefan Posted at: 2016-10-28T12:13:37.524Z Reads: 218

```
Hello everyone,

recently, the C39 capacitor on my VESC blew up. I took a short ride on my board, had to cross the street and picked up the board. On the other side, the board did not accelerate. So i connected the VESC to BLDC tool and it did not show any fault code. It even says there is current in motor when triggering the throttle on the remote but the motor will not spin. When i power the VESC it does not blink three times on start up. Later i recognized that C39 blew up. I contacted the supplyer (Enertion) but the do not respond since 4 days or so.

So my question:
What is the C39 for and can i repair the VESC on my own or should i try to send it back to Enertion if they eventually will respond? Also, do I have any warranty on the VESC? I purchased it roughly 1 month ago and wrote the board for an overall of maybe 5-6 hours. Moreover, the capacitor must been blown up when there was nearly no load on the board/VESC what seems to me like it was not my fault and even something like a production failure.

<img src="/uploads/db1493/original/3X/3/d/3d5217e2cebb9c0a895d50c0387c4fbc649b10ad.jpg" width="690" height="364">
```

---
## \#2 Posted by: IDVert3X Posted at: 2016-10-28T12:53:25.115Z Reads: 206

```
Enertion has no warranty unless you buy it separately.
You should be able to repair it if you have soldering iron and some SMD soldering skills.
It's 10uF 50V cap, SMD1206 package, order code: 963-UMK316BBJ106ML-T
```

---
## \#3 Posted by: Stefan Posted at: 2016-10-28T13:06:26.915Z Reads: 206

```
I do have a soldering iron. But are you sure it can be repaired like this? To me it seems like there is no connection to be soldered to on the burned side. or can i just add a good ammount of tin on that side?

I found this, do you think this is compatible?
https://www.amazon.de/Tantal-Kondensator-10%C2%B5F-125%C2%B0C-B45196H7106M509/dp/B00N7IKY9E/ref=sr_1_2?ie=UTF8&qid=1477657176&sr=8-2&keywords=kondensator+10%C2%B5f+50V

And how could this actually happen when the board imho was not under load?
```

---
## \#4 Posted by: chinzw Posted at: 2016-10-28T16:58:49.700Z Reads: 175

```
If the trace is burnt and lifted, you can, with a lot of care, scrape a bit off the protective coating and  bridge to it.
```

---
## \#5 Posted by: Stefan Posted at: 2016-10-29T00:21:11.802Z Reads: 151

```
I scraped a bit off and got some conducting material beneath it. Between GND and this the resistance i measure increases over time to over 20k. Hopefully this is the right connection.

But i still do not know how this could happen when the board was not under load...
```

---
## \#6 Posted by: Svenska Posted at: 2016-10-29T00:36:47.243Z Reads: 144

```
That cap is for input cleaning. Most likely it was blown by a spike as you plugged it in.

Here you can see its position:

https://raw.githubusercontent.com/vedderb/bldc-hardware/master/design/PNGs/Schematic-7.png
```

---
## \#7 Posted by: Stefan Posted at: 2016-10-29T00:47:55.220Z Reads: 128

```
But should the VESC not function normally even without that capacitor?
```

---
## \#8 Posted by: chinzw Posted at: 2016-10-29T01:37:14.664Z Reads: 125

```
In theory it should still power up and every thing
```

---
## \#9 Posted by: michaelcpg Posted at: 2016-10-29T04:05:03.205Z Reads: 124

```
Pretty sure that Enertion has several months of standard warranty on their electronics?
```

---
## \#10 Posted by: IDVert3X Posted at: 2016-10-29T08:35:20.948Z Reads: 116

```
No. On VESCs, they don't, unless you buy it. 
They have warranty on Raptor for example.
```

---
## \#11 Posted by: solarcross Posted at: 2016-10-30T01:28:16.820Z Reads: 103

```
How many volts is your battery pack ??
```

---
## \#12 Posted by: Stefan Posted at: 2016-10-30T01:52:01.029Z Reads: 102

```
It is about 25V, 6s.
I am waiting now for the capacitor to arrive. But I am sceptical if this will make the VESC boot and function normally again (did not blink three times at startup) since the blown up capacitor only was for stabilizing the supply voltage of the drv.
```

---
## \#13 Posted by: chinzw Posted at: 2016-11-01T17:57:08.704Z Reads: 90

```
Well, shorted caps usually just start conducting as a normal wire would, so if that's the case then you would have a short to GND.
```

---
## \#14 Posted by: Stefan Posted at: 2016-11-03T22:27:05.407Z Reads: 88

```
So now I soldered the capacitor to the VESC but still no change. On startup it does not blink three times, but led 1 and 3 are always on. Bldc says there would be current in motor but the motor will not spin. Motor detection gives a failure. But no drv fault code (NONE)...

If this might be helpful, here is a picture with the soldered capacitor:

<img src="/uploads/db1493/original/3X/2/5/25cda33277e33d3d2e84e8c6fde88d63535a3aa5.jpeg" width="375" height="500">
```

---
## \#15 Posted by: chinzw Posted at: 2016-11-03T22:44:42.912Z Reads: 82

```
Is that solder bridged to the pins on the DRV chip? or what is that white thing over the first 2 pins closest to the cap?
```

---
## \#16 Posted by: Stefan Posted at: 2016-11-03T22:47:15.674Z Reads: 82

```
I knew this question comes up :smiley:
But don't worry, it's just some hotglue to isolate the drv from tin coming close to the contacts of the drv. The (faulty) behaviour of the vesc did not change at all..
```

---
## \#17 Posted by: chinzw Posted at: 2016-11-03T22:48:59.192Z Reads: 82

```
I would start by crossing things of the list.
Check the 5v rail, check resistors, caps, etc.
```

---
## \#18 Posted by: Stefan Posted at: 2016-11-03T22:55:56.611Z Reads: 81

```
I am not shure what the 5v rail is. If it is the round component right next to the drv, it is 5v.
Unfortunately i do not have a multimeter that can measure the caps..
```

---
## \#19 Posted by: chinzw Posted at: 2016-11-03T23:09:33.496Z Reads: 81

```
5v rail is any part of the board that is supposed to have 5v running through it, you can test the +5v pin on the canbus or uart port. For the caps, you can at least test if they're shorted.
```

---
## \#20 Posted by: Stefan Posted at: 2016-11-04T11:43:35.504Z Reads: 70

```
Everything seems to be normal, i could measure the 5v at several different spots. Resistors seem to be ok, too.
```

---
## \#21 Posted by: TarzanHBK Posted at: 2016-11-04T12:00:12.339Z Reads: 66

```
I´d try to reset it from ground up. So new bootloader.

Otherwise test the other components, might be an other blown part somewhere due to a short
```

---
## \#22 Posted by: Stefan Posted at: 2016-11-04T13:06:47.957Z Reads: 65

```
I flashed the bootloader and the firmware again, but no change.
```

---
## \#23 Posted by: TarzanHBK Posted at: 2016-11-04T13:09:27.168Z Reads: 61

```
so if there´s nowhere a visible damage like a short, i guess one of the chips fried or an other component has an internal damage
```

---
## \#24 Posted by: Stefan Posted at: 2016-11-04T13:18:46.552Z Reads: 60

```
I think so, too. Thanks for your help anyway. So i need to buy a new VESC. Which one would you suggest?
I am not sure which one to buy. Enertion has it's new VESC-X, many people suggest a VESC from Chaka (Ollinboards?). There is also one site where i can buy a VESC for ~120€.
```

---
## \#25 Posted by: TarzanHBK Posted at: 2016-11-04T13:35:31.114Z Reads: 54

```
depends on where you are located.

If you bought in from enertion, try to contact enertion support via email. If they don´t respond, try to get in touch directly with @onloop here and tell him about it.
He will probably say that you´ll be able to buy his "warranty" (insurance) and could sent it back to repair with no questions asked.
Thats the cheapest option i guess.

Otherwise like i said earlier it depends on your location for a new one. You can get one from @chaka if you´re in the US or @elkick if you´re in the EU - just to name 2 of the best vesc vendors around.
```

---
## \#26 Posted by: Stefan Posted at: 2016-11-04T14:09:36.984Z Reads: 50

```
Is there really such a big difference between the VESCs that there is a price difference of roughly 50€/$ ?
```

---
## \#27 Posted by: onloop Posted at: 2016-11-04T14:10:10.264Z Reads: 50

```
We have instant replacement warranty available.

http://www.enertionboards.com/electric-skateboard-parts/1yr-vesc-replacement-warranty/

As we don't make the old vesc model anymore you will get a new vescx as the replacement when they roll off the production line later this month.

Be sure to submit a ticket with support@enertionboards.com and they will help you with any order questions.
```

---
## \#28 Posted by: Stefan Posted at: 2016-11-04T14:13:57.445Z Reads: 48

```
That does not mean that i can buy the warranty and send you my VESC back and get a new model, even though i did some major modifications like soldering new cap where the old one blew up, right?
```

---
## \#29 Posted by: onloop Posted at: 2016-11-04T14:16:53.044Z Reads: 46

```
Yes you can. The warranty covers all faults & user error.
```

---
## \#30 Posted by: Stefan Posted at: 2016-11-04T14:19:35.477Z Reads: 47

```
Well okay, this seems to be the cheapest solution since i then do not need to pay the full price for a new VESC.
I just do not want to end up sending the VESC back to the US (it came from there) and then get informed that it would not be part of the warranty in my case.
```

---
## \#31 Posted by: onloop Posted at: 2016-11-04T14:23:59.492Z Reads: 46

```
You don't need to return the vesc. Our warranty was designed to solve these issues quickly without the hassle of posting stuff back and waiting for repairs and back & forth emails etc....

We just ship a new one. 

Of course feel free to return the faulty one as we will definitely investigate the fault.
```

---
## \#32 Posted by: Stefan Posted at: 2016-11-04T14:26:28.087Z Reads: 46

```
That sounds really nice.
So i write an email to support@enertionboards.com telling that my VESC broke and i would like to buy the warranty to get the VESC-X as soon as it it ready to ship or do i have to log in into my account at your site and just buy the warranty?
```

---
## \#33 Posted by: onloop Posted at: 2016-11-04T14:35:42.509Z Reads: 45

```
Actually you need to do two transactions. 

1. Buy the warranty.
2. Buy the vescx 

We will give you a discount code to get the vescx at zero.

So I suggest email (or chat) with one of my guys, that way they can guide you.
```

---
## \#34 Posted by: Stefan Posted at: 2016-11-04T14:39:00.638Z Reads: 43

```
Okay, so then i will buy the warranty now and send an email to the support, telling them that i bought the warranty and was told that i will get a discount to get the VESC-X at zero. If they give me the dicount code, i can buy the VESC-X and enter that code, right?
```

---
## \#35 Posted by: TarzanHBK Posted at: 2016-11-04T14:39:16.794Z Reads: 46

```
this update sounds really good for that pricetag!
```

---
## \#36 Posted by: onloop Posted at: 2016-11-04T14:41:38.413Z Reads: 45

```
Yeah basically....
```

---
## \#37 Posted by: E-Boarding Posted at: 2016-11-04T14:48:34.842Z Reads: 46

```
So you are basically selling an upgrade from a VESC to VESC-X for 65Eur but I've to break my old VESCs first but there is no proof that they are really broken...
```

---
## \#38 Posted by: Cloud_Gnash Posted at: 2016-11-04T15:08:14.654Z Reads: 43

```
I just had my motors stop working mid ride this AM on my raptor...not sure if my VESCs blew up...one motor stopped rotating at all, and the other only slowly rolls backwards when given throttle. I havent had a chance to open the lid and check it out because i had to get to work, but ill be posting a video later today. @onloop i sent you guys a support ticket but i thought i'd post here as well for community input. Love the raptor....hoping to get it back and running
```

---
