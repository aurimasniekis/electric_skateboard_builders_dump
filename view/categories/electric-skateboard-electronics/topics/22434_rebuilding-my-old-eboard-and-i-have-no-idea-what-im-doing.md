# Rebuilding my old eboard and I have no idea what I&rsquo;m doing

### Replies: 10 Views: 756

## \#1 Posted by: oct0f1sh Posted at: 2017-05-05T02:00:30.014Z Reads: 99

```
Late last year I built my first electric longboard. I did it with almost no experience in soldering and electronics and it worked decently well. I'm about to be going to school in San Francisco, and I wanted to rebuild my board to be able to handle the hills in San Francisco more effectively. I'm going to be reusing my torque boards 6355 195kv motor and torque boards vesc. 

My goals:
*I would like this board to be able to handle the terrain of San Francisco reasonably well, this includes being able to go up the steep hills and also being able to go down the hills with good breaking and without overcharging the battery (again I really have no idea how this stuff works)
*I wanted to make my own longboard deck using the tools at my local makerspace
*I would like to have a range of a couple miles, likely I would be riding a mile and a half to and from school. I don't really care much about speed, I'm usually scared to go faster than 20 mph anyway.

My plans (some are more ambitious than others):
*Make my own longboard deck
*Either buy individual 18650 cells and create my own 10s2p (is this enough for what I want?) battery pack or buy one.
*Attach addressable LED lights to the bottom of the deck and match the speed of the lights to the speed that I'm traveling
*Use a loop key (or whatever it's called) to prevent other people from using it
*Attach a kayak handle for easy transportation
*dual motors (again, is this something that I need?)
*LED headlights

The parts that I have right now:
*Torque boards 6355 190kv motor
*Torque boards VESC
*Enertion motor mount
*Enertion (I think) pulleys and belts
*Some chinese 6S battery that I got off amazon for like $100 that I probably won't use for this build

My questions are:
*It seems too good to be true, but is this any good? It seems too stupidly cheap to be real. http://www.ebay.com/itm/BALANCING-SCOOTER-LG-36V-4-4AH-LITHIUM-ION-REPLACEMENT-BATTERY-PACK-6-5-8-10-/172648854096?hash=item2832ac7250
*How would I go about powering something like LEDs?
*What would I need in order to prevent any damage from regenerative breaking down steep hills? Is this even a problem?
*Is there a way I can get the current speed from the VESC?

I've recruited some friends of mine from my college's computer science club to help me with figuring all this stuff out, but there are still a lot of grey areas. Any help would be greatly appreciated.
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-05T02:26:45.690Z Reads: 78

```
Hello fellow bay area eskater!

For SF, you'll definitely want dual drive. Not just for uphills, but it'll really save you if you end up breaking a belt going downhill.

2P wont be enough, you'll need at least 4P @ 20a/cell = 80a. You can also go with lipo for easy power.

The battery listed is either fake, or they're unsuitable for esk8. $1.75/cell is too good to be true, not even including the other electronics in that calculation.

I don't know much about LED's, but you'll probably want something that runs on 12v with a step down converter to power it. See [here](https://www.getfpv.com/12v-step-down-voltage-regulator.html?gclid=Cj0KEQjwoqvIBRD6ls6og8qB77YBEiQAcqqHe8laOnvlyqjvTfrQkCRU0WKoYe1uo_oixfPmlUGCn6YaArN98P8HAQ)

Regen braking has never been a problem for me. Some people have had issues with regen braking with a full battery, but you should be fine if you've at least throttle a bit before going down a long hill.

You can buy a bluetooth module that plugs into the VESC to track speed. See [here](https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483)

Let me know if you want to meet up sometime and we can discuss in person as well!
```

---
## \#3 Posted by: oct0f1sh Posted at: 2017-05-05T02:34:30.897Z Reads: 74

```
Thank you! That bluetooth module looks pretty awesome, I'll have to look into that. You say that 2P isn't enough, is there a cost effective way to do 4P? If I did do 4P, should I stick to 10S or would it be ok to do something like 8S?
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-05T02:37:07.921Z Reads: 72

```
10s4p would be my recommendation, 5 or 6p would be even better if you could fit it.

I built a 10s4p pack using cell level fusing and it cost me about $250 in parts to give you a general idea.

$165 for batteries (Samsung 25R)
$15 BMS
$10 voltmeter
$40 anti-spark switch
$20 misc wires and such
```

---
## \#5 Posted by: oct0f1sh Posted at: 2017-05-05T02:42:06.475Z Reads: 70

```
Awesome, in that case I'll probably go with 10S4P then. I'm looking on imrbatteries right now and it looks like they have pretty good prices for Samsung 25R batteries, if I did 10S4P should I get just 40 batteries or something like 43 in case I screw something up?
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-05T02:43:04.043Z Reads: 67

```
I did exactly 40, thankfully I didn't mess anything up. But hey, better safe than sorry, can't hurt to pick up a few spares.
```

---
## \#7 Posted by: landonkun Posted at: 2017-05-05T03:42:27.211Z Reads: 60

```
Another option would be to get a BMS with a built in e-switch, essentially eliminating the need for an anti-spark switch.
My 10S BMS from BesTech was only $40 with an e-switch, and the actual push button I got from Amazon for like $10.
```

---
## \#8 Posted by: oct0f1sh Posted at: 2017-05-05T03:49:35.358Z Reads: 60

```
Interesting, any chance you could send a link for those?
```

---
## \#9 Posted by: landonkun Posted at: 2017-05-05T04:20:33.071Z Reads: 62

```
Sure can! This is the same as the one I got, but for 12S:
http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

Not sure how the price might differ. You basically just e-mail them, tell them you want that, and they will get back to you with pricing and all that. They might say it's a minimum order of two, but you can keep one as a spare or just sell it on here (I did the latter, and it was not hard to find a buyer cause these are great BMSs).

The one "catch" to having an e-switch rather than anti-spark is that your board will be powered on while charging. I don't think there's been any proof that this affects the board negatively in some way, but some people are still paranoid. I haven't been having any issues doing it this way.

Then you buy a nice switch like this and you're good to go:
https://www.amazon.com/Ulincos-Latching-Pushbutton-U19C1-Suitable/dp/B017KP67FY/
```

---
## \#10 Posted by: oct0f1sh Posted at: 2017-05-05T05:55:19.875Z Reads: 52

```
Awesome, thank you. I don't think I really have a problem with the board being powered on while charging, so I'll definitely look into using one of their BMSs.
```

---
