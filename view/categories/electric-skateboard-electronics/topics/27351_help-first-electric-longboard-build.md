# Help! - First Electric Longboard Build

### Replies: 23 Views: 1922

## \#1 Posted by: TeslaAlex Posted at: 2017-07-11T15:31:59.649Z Reads: 127

```
Hi! I recently heard about DIY electric longboard building. 
I got really excited and searched around the web for information. 
I picked a couple of components that was recommended on the forum and that wouldnt break my budget (around 300 dollars). The important thing is that everything should be located in EU, because of cheaper shipping (i live in Sweden). 
Since i am an absolute rookie, i am asking for help. **Will these parts work together?**

Motor: **[PROPDRIVE v2 5060 270KV Brushless Outrunner Motor]**(https://hobbyking.com/en_us/propdrive-v2-5060-270kv-brushless-outrunner-motor.html)
ESC: **[Hobbyking® X-Car 120A Brushless Car ESC (sensored/sensorless)]**(https://hobbyking.com/en_us/hobbykingr-x-car-120a-brushless-car-esc-sensored-sensorless.html)
Batteries: **[ZIPPY Flightmax 5000mAh 3S1P 20C]**(https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html)
Transmitter and reciever: **[2.4GHz Radio Remote Controller Receiver]**(http://www.ebay.com/itm/262779892776)
```

---
## \#2 Posted by: aigenic Posted at: 2017-07-11T16:09:10.154Z Reads: 111

```
No...your system should use at least 6s battery~22.2V...the ESC can take just 11.1V (3S), you need higher voltage...Motor is OK, if you will have two of the battereis connected in series then ok, transmitter+reciever are also good, just chagne the ESC :)
```

---
## \#3 Posted by: Decdog Posted at: 2017-07-11T18:03:53.359Z Reads: 100

```
[quote="TeslaAlex, post:1, topic:27351"]
Batteries
[/quote]
He will have two batteries
```

---
## \#4 Posted by: Decdog Posted at: 2017-07-11T18:06:36.759Z Reads: 97

```
This esc will work. https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html
```

---
## \#5 Posted by: gee Posted at: 2017-07-11T19:08:12.296Z Reads: 94

```
your budget is $300? I hope you own a 3d printer
```

---
## \#6 Posted by: pat.speed Posted at: 2017-07-11T19:29:57.211Z Reads: 95

```
You don't need to have a 3D printer to make a budget board. This is my build that cost me about $230 usd

https://www.electric-skateboard.builders/t/350-esk8-build/25252
```

---
## \#7 Posted by: TeslaAlex Posted at: 2017-07-11T20:06:33.647Z Reads: 89

```
Ok, thanks for the quick replies!
[quote="Decdog, post:4, topic:27351"]
This esc will work
[/quote]
I´ll change to the ESC you recommended!
[quote="gee, post:5, topic:27351, full:true"]
your budget is $300? I hope you own a 3d printer
[/quote]
The other parts are actually quite cheap!
I have built my own board and i will buy a set of trucks and wheels: [ Paris 180 Raw Longboard Trucks Wheels Package Bigfoot 90mm](http://www.ebay.com/itm/371958681319) 
I´ll also buy this pulley kit with motor mount:[DIY Electric Skateboard Parts Pulleys And Motor Mount Kit For 83/90/97MM Wheels](http://www.ebay.com/itm/351923420520)
```

---
## \#8 Posted by: wafflejock Posted at: 2017-07-11T20:08:39.464Z Reads: 81

```
Yeah 3D printer is nice to have and can save you a little bit here or there but what you save in $$$ you typically pay for in time.  If you already have a deck and trucks that will work that can cut the cost down quite a bit can definitely do it for a few hundred when it comes to just the electronics to get it working (ESC ~$80-110, batteries ~$60-80, motor ~$60-80, motor mount assembly ~$30-100 controller/receiver $20-100, shipping probably another $30, so about $280-500 plus need to have or get board and trucks).

Obviously if you go dual motor or have a custom battery and/or BMS that all adds quite a bit to it but for a budget board I'm pretty sure those are the essentials (ah forgot a charger and loop key, both pretty essential)
```

---
## \#9 Posted by: TeslaAlex Posted at: 2017-07-11T20:14:12.528Z Reads: 68

```
Ok! Well i already have a charger (I have a RC car) but what is the loop key´s purpose?
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-11T20:27:58.726Z Reads: 69

```
Loop key is just a XT-90 or XT-60 jack with a small loop of wire connecting it to itself so when it's not plugged into the female jack there is a break in the circuit between your batteries and the ESC and rest of the electronics.

http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

It's basically a fail safe and you can connect everything else up and double check it without power going to it and then plug in the loop key when you know everything else is good.  If something goes wrong either while you're bench testing or more importantly while you're riding it's good to have a loop key you can just pull out to cut power (also if you lock it to a bike rack or the like to go in a place good to pull the power from it so it doesn't do anything squirrely while you're gone).  Good to make it accessible from the top of the board as well (basically at the edge sticking out) so if you ever need to cut power because something is going crazy you can do that quickly.  There are switches but it's more complicated than it sounds to make a solid switch that also allows all the power you need to flow when it's closed, loop key is a cheap alternative to a switch.

If you use one of the anti-spark XT-90 plugs it has the added advantage that at higher voltages it won't have big sparks as the current rushes in to fill the capacitors on the ESC (at 12S they can be bad enough to melt the connectors, below that it's just a little spark if anything).
```

---
## \#11 Posted by: TeslaAlex Posted at: 2017-07-11T20:34:11.429Z Reads: 61

```
OK, thanks the good information! Could you link me a cheap and easy Loop key?
```

---
## \#12 Posted by: wafflejock Posted at: 2017-07-11T20:42:10.500Z Reads: 62

```
Actually not sure about where to get cheap premade ones I just bought a pack of XT-90 Male/Female pairs I think from an Amazon.com vendor and one antispark one to make the loop key (along with some 12AWG wire, others recommend 10AWG I'm not sure you get that much voltage drop with the slightly thinner 12AWG wire given the short distance but might be better to go with 10AWG especially with a lower voltage setup, ie something less than 10S)

https://photos.app.goo.gl/p2swB3p3r55mFCmj1
```

---
## \#13 Posted by: sl33py Posted at: 2017-07-11T22:11:07.253Z Reads: 60

```
[quote="TeslaAlex, post:11, topic:27351"]
cheap and easy Loop key?
[/quote]


cheap and easy is the loop key you make yourself!  It's not hard - there's even pictures you can follow to do it yourself.

Some really tall and _strikingly handsome_ gent posted a how-to even!  ;)

If you aren't comfortable soldering - you can skip a loop key - just get used to the spark and replace plugs every once in a while as they wear out from the arc.

GL!
```

---
## \#14 Posted by: flywithgriff Posted at: 2017-07-11T22:14:58.774Z Reads: 61

```
If you want a budget build I have some parts from a 6s build that are all in like new condition. 

https://www.electric-skateboard.builders/t/parting-out-6s-build/26869
```

---
## \#15 Posted by: korryh Posted at: 2017-07-11T22:48:53.948Z Reads: 60

```
I would use some sort of VESC or whatever is Politically Correct now days.  I had the same motor, LifePO4 packs from Hobby king and Hobby King 150 ESC.  The HK ESC caught fire, then tried TB ESC, that stopped working half way to work, then EZ run ESC which I sold when I got the VESC.  Moral of the story spend a hundred bucks and get a good ESC or 300 on multiple ESCs.  When you upgrade the battery and motor you can still use the same VESC.  My .02
```

---
## \#16 Posted by: wafflejock Posted at: 2017-07-11T22:52:39.170Z Reads: 56

```
Basically same for me but change the fire to just sparks and smoke.
```

---
## \#17 Posted by: sl33py Posted at: 2017-07-11T23:53:31.243Z Reads: 55

```
Agree wholeheartedly with you and @korryh!

VESC when used moderately (not bleeding edge like FOC and 12s) - at least the reasonably affordable 4.12 and similar - are really quite durable (easy to kill by stupidity, but harder to damage in use w/ correct config).

I just recycled two 4.7 VESC's for brother's first DIY build - at least 2 years old and still going strong.

Similarly my GF's build is on old 4.7 and just got new motor and gears - running GREAT!

My choice in order of preference would be:
Chaka Direct FET VESC / or non-direct - both with heatsink!
Enertion FOCBOX
Axle VESC
DIYes VESC

Personally i'll never use the Maytech and similar VESCs due to no $ going to Ben.  Gotta support to get improvements and super nice guy.

And if $$$ is no issue - get the new VESC Six!  gorgeous and no 60k ERPM limit (can run 12s FOC and >200kv motors if you want)
```

---
## \#18 Posted by: TeslaAlex Posted at: 2017-07-12T07:22:15.015Z Reads: 45

```
[quote="sl33py, post:17, topic:27351"]
My choice in order of preference would be:
Chaka Direct FET VESC / or non-direct - both with heatsink!
Enertion FOCBOX
Axle VESC
DIYes VESC
[/quote]

So to summarize, a VESC is the way to go! How much does Chaka charge for the VESC + shipping to Europe?
Another thing I was wondering about is the wiring, do all the necessary wires come with the motor, VESC and batteries? 

I plan to wire like this:
<img src="/uploads/db1493/original/3X/b/f/bfe669b137d56e3964132e8b6a18a28d7e5f966f.jpg" width="556" height="500">
```

---
## \#19 Posted by: pat.speed Posted at: 2017-07-12T10:17:22.584Z Reads: 41

```
You will most likely need to buy plugs for the Vesc unless they are pre soldered with Vesc and adapters from the battery to the Vesc if needed
```

---
## \#20 Posted by: TeslaAlex Posted at: 2017-07-12T10:34:01.690Z Reads: 41

```
But apart from that the connections should be identical as if i had used an ordinary ESC?
```

---
## \#21 Posted by: pat.speed Posted at: 2017-07-12T11:29:58.789Z Reads: 41

```
Yeah should be
```

---
## \#22 Posted by: Ket Posted at: 2017-07-12T13:32:07.692Z Reads: 40

```
[quote="wafflejock, post:10, topic:27351"]
at 12S they can be bad enough to melt the connectors, below that it's just a little spark if anything
[/quote]
I'm planning on building a 12s, VESC and 6374 motor and use anti-spark xt90 rather than a switch. Does that mean I'm gouna have a problem?
```

---
## \#23 Posted by: wafflejock Posted at: 2017-07-12T14:47:30.877Z Reads: 36

```
All good with the antispark plug (sparking was only a problem without it).  Only issue with the antispark is if you don't insert it entirely the power will flow through the resistor  in the plug and basically burn it up otherwise strongly recommended.

---

Personally just have a female jack between where the two batteries connect and I put my loop key in there to complete the circuit and make the final connection between the two batteries for power to flow.  You can really put a female jack anywhere on the lines between the battery and the ESC though to open the circuit when the loop key isn't inserted.
```

---
