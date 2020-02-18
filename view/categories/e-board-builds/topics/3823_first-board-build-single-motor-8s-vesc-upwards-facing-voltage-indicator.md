# First Board Build &#124; Single Motor 8S VESC &#124; Upwards facing Voltage Indicator

### Replies: 17 Views: 2588

## \#1 Posted by: Rick Posted at: 2016-05-25T16:07:25.892Z Reads: 303

```
Hi everyone, after doing quite a bit of research on E-Boards and electronics in general I decided to build my first one (also my first DIY project). I'm going with the following components:

Enertion Single Motor kit (R-Spec Pro+)
2x5000 mAh 4S Zippy Flightmax 20C batteries in series
Enertion VESC
Diyelectricskateboard On/Off Switch (If you have a better, and more importantly, cheaper idea, I'll be please to hear it :P)
HK-GT2B Transmitter-Receiver

As for connections, I plan to do the following (If you think any of the parts listed here are low quality, or I can get cheaper ones from other sources please tell me):

Series conector: http://www.ebay.es/itm/4MM-HXT-Harness-For-2-Lipo-Battery-In-Series-RC-Car-Plane-Boat-Connector-Cable-/330989322484?hash=item4d108040f4:g:JzMAAOSwNSxU7eDY

I will use this http://www.ebay.es/itm/Lipo-Balancer-8S-auf-2-x-4S-JST-XH-Lange-10cm-Splitter-Silikonkabek-/151972427155?hash=item2362433593:g:-JcAAOSwzhVWskum to turn the 2x4S balance leads into an 8S one, and the use an 8S Voltage Meter to check how much power I have left (I'm guessing that's possible)

Regarding the voltage meter, I planning to:

Buy a deck that has the front and rear "holes" like this one http://loadsofdecks.com/maestro-mini-32/, then I will try to place and glue the voltage meter to the top (and front) of the deck and connect it to the batteries, the idea behind that is that I want to be able to check how much power I have left while riding the board but without having to turn my head all the way down "raptor-board style". <img src="/uploads/db1493/original/2X/2/2cb9bbbbf6ada4079aa172e7ed761ab4f3672557.jpg" width="690" height="210">


As far as the build, I have some worries. I don't know if I should buy a Watt meter, and once I know how much power I may need in the worst scenario ¿set that as a limit in the VESC?. As far as my understanding reaches, @EnertionSupport VESC's don't need many adjustments to work properly, but I'm looking for regenerative braking and lowest battery consumption possible so I guess I may need to play with the settings a bit (correct me if I'm wrong). Also, once I learn about it, I will probably fiddle as much as I can with the VESC.

Finally, as for the enclosure, I'm still considering different possibilities, but for the front one (batteries and VESC will be separated, FRONT-REAR) I'll cut a plastic box (I want to be able to easily change LiPos on the go).

Any suggestions are more than welcome. I'm planning to start building as soon as I get all the parts and when my exams are over.
```

---
## \#2 Posted by: karma Posted at: 2016-05-25T16:31:39.896Z Reads: 276

```
Won't get very far with just a motor xD
```

---
## \#3 Posted by: Rick Posted at: 2016-05-25T16:32:53.594Z Reads: 279

```
Yeah hahaha sorry, I missclicked and I posted it before writing everything :joy:
```

---
## \#4 Posted by: Namasaki Posted at: 2016-05-25T17:28:58.396Z Reads: 264

```
Use the more forward location for the volt meter. 
It will weaken the deck too much behind the truck
```

---
## \#5 Posted by: JLabs Posted at: 2016-05-25T17:39:43.124Z Reads: 260

```
The connectors you will use are just fine.. you can do an xt90s loop key in stead of the tb on off switch. One motor will work fine if you gear it low. I use 14/36 gear ratio, the lower the better.. good luck!
```

---
## \#6 Posted by: Rick Posted at: 2016-05-25T18:06:06.291Z Reads: 259

```
I'm trying to get a deck with those front a rear "holes" to try to pass the cables through it to connect the voltage meter and the batteries, that way I don't have to drill the board.
```

---
## \#7 Posted by: XIII Posted at: 2016-05-25T21:57:52.215Z Reads: 241

```
Why don't you just buy a voltage meter that you install over the 2 cables going from your battery to your ESC.

If you plug a Voltage meter to your balance leads, you will have to unplug it every time you stop. 
Otherwise it stays on. 
If you place the voltage meter between batteries en ESC. and you connect it behind the power switch (xt90-s?). The voltage meter will only turn on when the board is powered.
```

---
## \#8 Posted by: Rick Posted at: 2016-05-26T14:58:11.259Z Reads: 221

```
Thanks for the suggestion @XIII can you recommend me any of those voltage indicators? because in most sites they only sell the ones you connect to the balance leads. Anyway, my daily commute is usually going to the faculty/hospital and coming back several hours later so I will disconnect my batteries quite often (I will do so when I won't use the board for like 2 o 3 hours), so I may not mind disconnecting the voltage indicator as well.

As for the switch, I have decided to go with the xt90s and I will connect it on the positive side of the series cable I linked before http://www.ebay.es/itm/4MM-HXT-Harness-For-2-Lipo-Battery-In-Series-RC-Car-Plane-Boat-Connector-Cable-/330989322484?hash=item4d108040f4:g:JzMAAOSwNSxU7eDY
```

---
## \#9 Posted by: JLabs Posted at: 2016-05-27T02:06:44.980Z Reads: 210

```
Hablas espanol y ingles? It link is the Spanish eBay so I was just wondering.. I am not following ur posts clearly and was just making sure u know that the last link you showed is not an xt90s, but for your batteries.. sorry
```

---
## \#10 Posted by: Rick Posted at: 2016-05-27T08:47:50.678Z Reads: 217

```
Yes @JLabs I'm from Spain :) (You too?).  And yes, I know the eBay link is for connecting the batteries in series, the XT90S will go here: <img src="/uploads/db1493/original/2X/e/e67bbd212fd8671dfc950e3042ebc5d39895a35a.jpg" width="500" height="500">
```

---
## \#11 Posted by: JLabs Posted at: 2016-05-27T10:18:16.206Z Reads: 205

```
Si, muy bien. Soy de Ustados Unidos.
```

---
## \#12 Posted by: XIII Posted at: 2016-05-28T14:00:40.498Z Reads: 202

```
Hi Rick 

A voltage meter that was mentioned in another topic is for example this one: 
http://www.ebay.com/itm/2016-Battery-Capacity-Tester-Indicator-for-12V-24v-36v-48v-CAR-Lead-acid-lithium/172143986261?_trksid=p2141725.c100338.m3726&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D1%26asc%3D20150313114020%26meid%3Dc15551bc7aaa4c58b0d860a219d62251%26pid%3D100338%26rk%3D3%26rkt%3D18%26sd%3D331508332778

Now for your on and off switch. 
You need to use the XT90-s. But don't connect it using this to the battery.
What is easier is to just open and close the circuit by pulling out a loop key. 
and this loop key is made of an xt90-s female connector. Which is connected in between the + of your batterie and + of your esc.
The male side of your XT90-s is a wire that just connects both connections with of your xt90-s. A short . 
Now if you pull this xt-90-s male out. you will have an open circuit and the batteries are disconnected. 
you should mount this loop on the outside of your enclosure so you can easily do this. 

If you don't understand i can sen you a picture of my board.
```

---
## \#13 Posted by: Rick Posted at: 2016-05-30T23:07:44.616Z Reads: 182

```
Thanks @XIII for the battery indicator link, it's way cheaper than I though. And yes, I've already read a couple tutorials on XT 90s loop keys. What I meant in the photo I posted before was that I'm planning to mount de XT90s loop key on the positive cable of the series connector (instead on, for example, the cable between the series connector and the VESC). Anyway, if you send me a photo of your board it may be helpful so I can get an idea of how to place it out of the enclosure, etc.
```

---
## \#14 Posted by: Pablo_702 Posted at: 2016-06-16T01:47:47.743Z Reads: 161

```
would you pls send me a picture of this wiring????

Now for your on and off switch. 
You need to use the XT90-s. But don't connect it using this to the battery.
What is easier is to just open and close the circuit by pulling out a loop key. 
and this loop key is made of an xt90-s female connector. Which is connected in between the + of your batterie and + of your esc.
The male side of your XT90-s is a wire that just connects both connections with of your xt90-s. A short . 
Now if you pull this xt-90-s male out. you will have an open circuit and the batteries are disconnected. 
you should mount this loop on the outside of your enclosure so you can easily do this.

If you don't understand i can sen you a picture of my board.
```

---
## \#15 Posted by: XIII Posted at: 2016-06-16T07:43:33.077Z Reads: 151

```
That's what I meant. 
and you connect the voltage meter on the + and - of your esc. On the ESC side of the loop key, so it's get shut off when you disconnect the loop key.
```

---
## \#16 Posted by: nmagz3 Posted at: 2016-12-07T07:27:02.403Z Reads: 89

```
I'm about 6 months late to this thread but just wanted to give thanks.  This was the most helpful for me as I'm also building my first board and was inquiring on where to place the loop key and volt meter in the correct place.
```

---
## \#17 Posted by: Tord Posted at: 2017-04-26T20:43:58.188Z Reads: 65

```
is, to buy a vesc an investment worth making? or should i go for an ESC? i don't know anything about either
```

---
