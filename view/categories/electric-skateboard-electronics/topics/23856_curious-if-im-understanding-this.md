# Curious if i&rsquo;m understanding this

### Replies: 39 Views: 1910

## \#1 Posted by: multiplexor Posted at: 2017-05-25T01:57:30.233Z Reads: 194

```
Trying to understand the battery power to motor type deal... :D

If I had a Turnigy 6364 245Kv motor...  Specs say I can send it 2700w, 37V, 70A.

If I have a 10s1p Setup, I have:
1 cell = 3.7v @ 2900mAh

10s1p would equal 37 volts, and only 2900mAh
W = V * A, thus at 100% power I'd be sending 1 motor only 107.3watts.

Shouldn't I be trying to send it more along the lines of 2500watts and 50-60A instead of 2.9A?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-25T02:01:31.119Z Reads: 185

```
Capacity =/= Discharge rate. Your capacitance is 2.9 amps, but the maximum discharge potential is much higher. For 18650 cells it varies to about 15-25 for high discharge cells. For lipo your can get much higher discharge, usually 100a+
```

---
## \#3 Posted by: multiplexor Posted at: 2017-05-25T02:24:09.648Z Reads: 174

```
Yesss true! I was reading that. For an 18650 25R, it can discharge at upto 20A.

I had to youtube a couple vids to get my brain into it.

Thus, if I understand correctly, in the scenario above, I'd have 37V, and 20A available if needed. 
So, technically the motor (at 100%) will want to try to pull all 37V and 20A because it can take 37V, and upto 70A.This would probably cause the batteries to get pretty hot, given that it's alot of amps to pull.
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-25T02:26:35.809Z Reads: 149

```
The current pulled from your battery depends on your ESC. If you get a VESC you can limit this current so you don't damage your battery. 1P is not a very good idea though which is why I can never recommend boards like landwheel or spectra. Anything short of 40 cells will lead to a short cycle life.
```

---
## \#5 Posted by: multiplexor Posted at: 2017-05-25T02:34:46.888Z Reads: 135

```
Makes sense. From what I'm reading, you can program your VESC to only pull a specific amount of amps.

Then, if I were to use a 10s2p setup, I'd have roughly 37 volts and 5800mAh or a max of 40Amps at max discharge rate. I could then use the VESC to limit the output to 20amps to keep it safe.

In terms of Watts, that would give 37V * 20A = 740W.

Considering the motor can handle upto 2700W, should I be aiming to send it more amps, or is there a safe number I should be sending it?

EDIT: In my example I'm using simple 10 as a number. I'm starting to see the 40 cells required though

EDIT EDIT: Also... thank you for the help, it's helping clear the brain lol
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-25T02:38:29.015Z Reads: 114

```
if you were running 2P, I'd set the battery current to 40A so you can have on demand power, it won't pull 40A all the time. Motor current can be higher, I have mine at 80A per motor.
```

---
## \#7 Posted by: multiplexor Posted at: 2017-05-25T02:52:25.562Z Reads: 115

```
True, even though it can max at 40A, it doesn't mean your going to be at 100% full throttle for the whole time.

And finally... lol... if I have a 2 motor setup, I'd ideally want to have the same setup twice? Namely twice 10s2p, two VESC's, and obviously 2 motors.

Given that 37V * 40A only gives 1480Watts. Should I look for a motor that has a lower max wattage?
```

---
## \#8 Posted by: jmasta Posted at: 2017-05-25T04:18:42.422Z Reads: 112

```
[quote="Jinra, post:2, topic:23856, full:true"]
Capacity =/= Discharge rate. Your capacitance is 2.9 amps, but the maximum discharge potential is much higher
[/quote]

Capacity (Ah) =/= Capacitance (F)

Just a mixup of terms, but it could be confusing to new users
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-25T05:25:09.777Z Reads: 112

```
[quote="multiplexor, post:7, topic:23856"]
Given that 37V * 40A only gives 1480Watts. Should I look for a motor that has a lower max wattage?
[/quote]

Better not to get a weaker motor but to get a stronger battery.
And there is another factor for you to get your head around and I didn't see it mentioned yet and that is Voltage Sag.
If you have a battery capable of 40a and you draw 40a from it, the voltage will sag excessively  causing loss of power and range.
This situation is not as much of a problem when riding on flat ground at moderate speeds.
However, if you plan on charing up hills or experiencing the thrill of fast acceleration, Voltage Sag can be a real problem.
To avoid this, you need to over build the battery. The more you over build it the  better.
If I was going to build a Lithium ion pack, I would not go less than 10s4p
```

---
## \#10 Posted by: multiplexor Posted at: 2017-05-25T12:18:20.700Z Reads: 100

```
Ah yeah makes sense. You'll have more amps available to keep it up there. 

In terms of using 2 motors and 2 vescs... Should I look at using 2 sets of 10s4p. Each connected to their own vescx. Or is it possible to connect both 10s4p together and then split the big battery to goto both vescx. Technically I would end up with a 10s8p
```

---
## \#11 Posted by: multiplexor Posted at: 2017-05-25T12:38:40.525Z Reads: 88

```
Scratch that question... Lol. I'm checking out 10s8p sources hehe
```

---
## \#12 Posted by: chaka Posted at: 2017-05-25T13:08:06.585Z Reads: 91

```
Here is my take on battery packs. You want a pack large enough that has an average discharge rate less than or equal to 1c. I average at about 25 amps @36v but the average rider will pull roughly 15 amps on average. This means a pack consisting of "at least" 60 cells is the minimum for a long lasting battery pack with plenty of discharge potential. What you get is a pack with a flatter discharge curve and more watts per mAh do to the lack of significant voltage sag. 

If you plan on punishing your system and riding like a beast you may want to jump up to the sanyo 21700. With 60 cells you will have a 24 Ah pack @ 36v. I have been testing these cells for a few months and they out perform everything else on the market in a 10s6p format. We are featuring them in our upcoming "FreeRide-Pikes Peak Edition"
```

---
## \#13 Posted by: Bataleon Posted at: 2017-05-25T13:51:35.081Z Reads: 91

```
Ouch, that's over 2.5 kg of cells. What would you recommend to somebody wanting to build a small, light and portable city cruiser? Something like A123 26650 LiFePO4 cells?
```

---
## \#14 Posted by: multiplexor Posted at: 2017-05-25T14:04:42.206Z Reads: 89

```
Exactly, I'm looking at it going a good distance too. I expect the board not to be light light, but not overly heavy too.

For a lighter setup, I assume you'd have to simply put less batteries? Something like a 10s2p setup?
```

---
## \#15 Posted by: Print3r Posted at: 2017-05-25T14:05:08.253Z Reads: 93

```
I would advise waiting for the $800 EBB Proton board which will soon be released for preorders. It will have a 33km range, 20mph max speed and super fast 2h15 min recharge time. The deck is planned to be 33" long and made by jet boards (very portable and high quality). All other parts of the board are also really high quality - eg for the wheels are planning to use Orangatang Kegels. The board will only be delivered though end of August as it will be built by fellow builders from the community and some parts will take some time to arrive as the shipping packages will be rather large (aiming for 50 preorders).
```

---
## \#16 Posted by: AJesk8 Posted at: 2017-05-25T14:11:24.251Z Reads: 89

```
i will definitely be getting one of these they look so good!!
```

---
## \#17 Posted by: chaka Posted at: 2017-05-25T14:12:58.712Z Reads: 94

```
I would still use 18650 cells but I would gear it down to decrease the load from the motor/s.  The average load should correspond with the capacity of the pack you intend to use. A123 cells are a little too big to use in a slim deck but they do work very well in small configurations.

@multiplexor A deck with 60 cells is actually not bad. You wouldn't want to carry it around the mall but the ride quality is somewhat enhanced by the added density of the deck. You can use less cells but you can lose cycle life significantly by doing so. Going big can give you potentially thousands of charge cycles while using them in a high discharge state will net you 200 to 300 cycles. Going big saves you $$$ in the long run.
```

---
## \#18 Posted by: Trans-amers Posted at: 2017-05-25T14:34:45.417Z Reads: 88

```
The protron seems legit
Might wanna buy one
```

---
## \#19 Posted by: Jinra Posted at: 2017-05-25T14:36:49.991Z Reads: 85

```
Meanwhile on the other side of the spectrum, we have Spectra, Landwheel, Inboard, etc with 1p 18650's. I wonder how long they'll last 🤔
```

---
## \#20 Posted by: multiplexor Posted at: 2017-05-25T14:54:51.642Z Reads: 94

```
In terms of Board... Would something like this be decent?

https://www.muirskate.com/longboard/decks/72068/sector-9-downhill-division-jimmy-riha-pro-model-longboard-skateboard-deck-w-grip

It would have a bit of a kicktail to it.

Because It's mainly for distance, and not for tricks, etc... I'm looking at bigger trucks
Something like these: 

http://www.trampaboards.com/the-ultimate-truck--black-hanger-powder-coated-baseplate-with-titanium-axles--kingpin-p-12299.html
```

---
## \#21 Posted by: Print3r Posted at: 2017-05-25T15:00:30.298Z Reads: 86

```
The Proton will have a 10s3p battery of 30q cells .... huge range!
```

---
## \#22 Posted by: longhairedboy Posted at: 2017-05-25T15:01:26.249Z Reads: 85

```
This is exactly why i'm moving to 12S5P as the default pack size for my boards. Even on a 12S4P voltage sag happens. It is definitely not as bad as these commercial boards but it can be noticeable at the bottom the discharge cycle for sure, and can even trigger the BMS to shut down if you try to floor it while in the bottom percentages. The most sag i've seen on a 12S4P in my builds is a full two volts, but in my mind that's two volts two many.
```

---
## \#23 Posted by: Jinra Posted at: 2017-05-25T15:01:33.445Z Reads: 83

```
That's only 45A of discharge though. It can be hard on the battery depending on board setup and riding environment.
```

---
## \#24 Posted by: longhairedboy Posted at: 2017-05-25T15:02:56.213Z Reads: 82

```
i'm about to put 40 of those 30Q cells in an evolve bamboo GT. 

i've got two bamboos on my bench right now testing out our hands at battery mods. If it works out we'll probably provide it as a service. 

Nothing keeps us busier than people hating their Evolves.
```

---
## \#25 Posted by: Print3r Posted at: 2017-05-25T15:03:18.653Z Reads: 80

```
It will be limited to 20mph and is intended for city use - it should be fine. It is going to be using a VESC-X probably so we can limit the current.
```

---
## \#26 Posted by: Print3r Posted at: 2017-05-25T15:04:59.341Z Reads: 80

```
It should be mandatory that at the top of every electric skateboard's website page, it says do your research before buying an electric skateboard ... evolves and chinese knock-offs might not sell as well.
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-05-25T16:10:26.841Z Reads: 82

```
that's a great idea. It would make an excellent article, thanks.
```

---
## \#28 Posted by: multiplexor Posted at: 2017-05-25T16:52:05.006Z Reads: 84

```
Curious.. for gearing... I'm thinking of the MBS all terrain black wheels.

https://www.mbs.com/parts/13401-mbs-all-terrain-longboard-wheels-black-4

Do we have gears available for these to purchase?
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-05-25T18:05:31.396Z Reads: 79

```
Any wheel pulley that can be used with flywheel clones will work with those. The cores are identical to clones.
```

---
## \#30 Posted by: Jinra Posted at: 2017-05-25T18:40:41.712Z Reads: 77

```
Evolve pulleys don't look like they'd work given the thicker spokes.
```

---
## \#31 Posted by: smurf Posted at: 2017-05-25T19:03:34.158Z Reads: 75

```
I decided to get 10S8P battery it's on a 42" deck that I got from @longhairedboy and I got two vescs from @chaka I have those mbs wheels as well. I'm sure everything is going to last a very long time.
```

---
## \#32 Posted by: Namasaki Posted at: 2017-05-25T19:19:00.032Z Reads: 75

```
We talkin quality parts!
Did you get the 4.12 Vescs or the Ollin ESC?
```

---
## \#33 Posted by: multiplexor Posted at: 2017-05-25T19:23:12.434Z Reads: 82

```
I'm going to see about getting the Enertion VESC-X ones.

Pulley's I'll try to get from thingverse: https://www.thingiverse.com/thing:1741371

Now, I just need to see how to mount the motor, and about the trucks.. I want stiff ones, but i have to research what mounts fit with what.

Battery I'll probably have custom made once I can get all these items nailed down.

I'm not sure what board to use with 100mm wheels. I want a kicktail for sure... 9mm wide, 40-40 in length
```

---
## \#34 Posted by: chaka Posted at: 2017-05-25T19:46:15.930Z Reads: 77

```
80 cells packs are nice! Roughly 24 Ah @ 36v if using hg2 or 30q cells. You get about the same performance from a 60 cell pack made of Sanyo 21700's... 24 Ah @ 36v.  The 21700's actually take up less space lengthwise and only add a few millimeters in thickness.

<img src="/uploads/db1493/original/3X/9/b/9b5fd3b8a27e388ec7dd93fad93b9e03ccf3d7e0.jpg" width="662" height="500">
```

---
## \#35 Posted by: smurf Posted at: 2017-05-25T21:41:12.765Z Reads: 72

```
I almost did your fuse wires build but I chickened out and got these battery holders instead.

https://www.instagram.com/p/BUh9ZIIli93/
```

---
## \#36 Posted by: multiplexor Posted at: 2017-05-26T00:08:53.717Z Reads: 71

```
ooo neat! :D
```

---
## \#37 Posted by: longhairedboy Posted at: 2017-05-26T01:23:43.204Z Reads: 70

```
evolve pulleys have to be shaved to work with clones. they're designed for genuine abecs
```

---
## \#38 Posted by: Jinra Posted at: 2017-05-26T01:26:16.666Z Reads: 70

```
Yea, that sounds like annoying amount of work
```

---
## \#39 Posted by: longhairedboy Posted at: 2017-05-26T12:09:45.969Z Reads: 65

```
it is. took me over an hour with a dremel to get those damned evolve pulleys to work with the clones.
```

---
