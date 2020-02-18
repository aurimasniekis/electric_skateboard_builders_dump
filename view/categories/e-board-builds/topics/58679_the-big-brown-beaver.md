# The Big Brown Beaver

### Replies: 13 Views: 991

## \#1 Posted by: squishy654 Posted at: 2018-06-12T20:21:09.818Z Reads: 267

```
The Big Brown Beaver (named by my daughter) Is a novel electric skateboard made for joyriding solo or in tandem with a child. It features dual motor power, 12s4p battery, LED lighting and integrated Bluetooth music.

Rozzi herself modeling the build
![image-20180427_180511|375x500](upload://kOLJgN0YpP6qncdnyO5YOXhI2NP.jpg)

She picked the name, the colors and stated the deck should "look like a deck", so I took her literally and we painted it like the pattern of an backyard deck.
![image-20180427_180535|375x500](upload://3Ut8aAPt9s94PsYWNkppAueVbWi.jpg)

The shape isn't that bad, I cut the nose off and left the tail as-is, not bad for a free deck from a friend. 
![20180502_112113|375x500](upload://uI0X2iEUUyhiHs2IjW3PjrSKfba.jpg)

-Used and free Skateshred deck with the nose cut off to make a bottle-nose, rear “beaver tail” kick, this was given to me by Loppy, a builder not in these forums.
-TB218 trucks for dual motor clearance, of course with Riptide bushings and pivots, front has a Caliber 50 baseplate wedged another 5’, rear has a 44 Caliber baseplate de-wedged 4’, giving me a 55/40 split on a long wheelbase. Tuned with fatcones and barrels.
-Zealous bearings wrapped in Abec11 107mm wheels
-Hobbyking 15mm wheel and motor pulleys
-Dual Ollin 50mm 190kv sensored motors
-Custom motor mounts thanks to @korryh right here in these forums
-HTD5M 255mm 15mm belt
-Dual Maytech VESC (1st time testing these out)
-Mini remote from Amazon
-Handcrafted MDF battery/ speaker enclosure
-Torqueboards 12s4p Panasonic battery with usb charge ports, built in solid state switch and voltage display
-Voltage regulator set to 12.2 volts
-Dual external toggle switches for turning on and off accessories 
-HitLights LED Light Strip Music Controller for SMD5050 RGB Multicolor LEDs 
-Supernight LED strip light 5050 SMD, 300 LEDs waterproof RGB color changing lights
-Icstation 2X50W Bluetooth Digital Stereo Audio Amplifier 
-Dual 4inch full range auto speakers
4inch Speaker grills
-Painted top (wood deck pattern) under clear grip tape, bottom painted flat black, enclosure in a steampunk brown (needs brass brackets and corner guards)

The drive is as solid as any I have built before, these mounts seem strong.
![20180310_074625|667x500](upload://vqIWXlhRItIsG50YjUxXTvBhVrB.jpg)

Finally gathering the final parts list in a pile
![20180502_112101|375x500](upload://vcX1MckPA2iagp30CV7c4ikFiDi.jpg) 

I have been slowly working on this project on the side, I wanted a board that was tacky, loud and included things which I would never put on a skateboard. Realizing I had a giant battery was the 1st revelation instigating the novelty questions, “what could I possibly power with this thing in addition to the motors?” I asked myself. 

I had included flashy LED lighting on one of my early builds, a buddy made me a LED controller using an Arduino and I patched in a hefty voltage regulator to make it function. It was a neat and novel addition and aids with safety on night rides. It reminded me of those cyclists building cool party bikes with LED’s and music playing and cup holders for the critical mass gatherings and parties they have. I wanted to make something similar but in skateboard form. So, adding music was the obvious next step.

Shaping the enclosure to match the deck 
![20180505_113348|667x500](upload://xJMpNkYuJ9VniqrNR0EdERq8HYI.jpg)

Cutting out speaker holes and battery switch access
![20180502_114216|375x500](upload://pZg3qvrtkZRqSdy7CfRt1kubgDK.jpg)

Mocking up, or should I say squeezing in..
![20180427_170320|375x500](upload://hq3fB801jpNP0DdoLqKlvJpNZev.jpg)

Test fitting still, nothing completed here, lol
![20180503_074825|165x220](upload://5ltWjebLgHMOatxy0URdrwnNL3p.jpg)

I 1st purchased a Bluetooth speaker and I was going to simply attach it to an existing eskate, but that didn’t last long, the battery wouldn’t last long and it wasn’t loud enough for what I was going for. As you can see I went all out, integrating the Bluetooth and constructing the whole thing entirely from scratch the key part being those little amplifier boards now on the market. These are small boards with Bluetooth and an amplifier built in, but the power and quality is lacking on most of them. I bought various kinds to find something that works, finally deciding on a 50watt version. If you do this, just get the best one you can afford with the most power. I think I blew two of them while testing and some of the cheap ones were even dead on arrival.


The low cost ollin motors came with some "who knows wtf" jack on the sensor wires, I'm just going to cut and hope to get the pin-out correct, I have jst's. 
![20180416_200324|667x500](upload://61SPvKJnziLcBNiqjGelXlSzlJD.jpg)


As for actually building this thing, it was a lot harder than I thought, but I think I asked for it by trying to fabricate the entire enclosure myself. It's a MDF at like 5mm, glued and screwed together, I am barely able to squeeze in everything and still fit it on the giant deck. There were numerous problems to overcome along the way I did a lot of building in my head and rearranging parts before ever securing anything. Bart, a another local eskater, provided the last few solutions and "just do it" attitude to get past the cruxes and problems that kept stopping me. The speaker grills were a bitch to figure out, the hardware was difficult to source, the mounting brackets were a puzzle, the sensor wires still need to be adapted to the Maytech vesc's and I have not bench tested the motors yet, but I hope too tonight.

Bart tag teaming the solder work, we had to assemble this within the box obviously.
![20180611_234027|243x500](upload://j47UjCpg2JdQUyLt9A88BuYY6Cl.jpg)

I used a basic regulator, to get the high voltage of 12 cells down to a controlled 12v needed for the accessories. It needed ample amps (pun intended) to power the amplifier and LED lights.  The music and lights are on separate switches on the side of the case to save battery MAH for range when needed. I should measure the draw from the regulator to see how much of a dent I am putting on my range while running the music and lights.

Close up of the regulator, LED controller and 50watt Bluetooth amp. I was figuring out where to put the VESC's, lol.
![20180504_145508|375x500](upload://wjJwI965CQGp2JrIyAaMJjVRmBt.jpg)

I still haven't heard the speakers from the sealed box yet, and I'm hoping it doesn't need ports because there's little room for a tube to tune the air pressure, I'm hoping a leaky sealed box of MDF and some filler will do the trick, but there isn't much volume. Also, the speakers are facing the ground, so most of the sound will be reflected unless the whole board is chilling and leaning up against something, then it's louder than most self-contained Bluetooth speakers you could buy and bolt on.

Here she is on the solder bench getting assembled, just about done with the hard parts.
![20180612_002935|690x335](upload://nrEHs4mHJFRPKamIAszZjFGpz7W.jpg)

And this is how she sits as I type this, waiting for me to button it up and configure the VESC's.
![20180612_004224|243x500](upload://tC0vFm3JziWdGXamFpnFNpffew3.jpg)

This is the Bluetooth adapter and amp I used: https://www.amazon.com/gp/product/B075JHJ1ZR/ref=oh_aui_search_detailpage?ie=UTF8&psc=1 

Stay tuned for more as I button this monster up and take her out on a maiden…I am open to suggestions for to how to best mount the cup holder, and look for Rozzi's review in the future because we are going to take this out and paint the town RED!!
```

---
## \#2 Posted by: squishy654 Posted at: 2018-06-12T20:54:03.957Z Reads: 186

```
Here's a short clip from Bart with it powered up and bumping: https://www.reddit.com/r/ElectricSkateboarding/comments/8qmgwj/integrated_50_watt_bluetooth_speaker_with_led/
```

---
## \#3 Posted by: slick Posted at: 2018-06-12T20:57:22.503Z Reads: 186

```
Hehe. Your daughter gave it a fitting name.  Now all you need is some fur for the tail to make this build legendary! :grinning:
```

---
## \#4 Posted by: squishy654 Posted at: 2018-06-14T01:28:16.118Z Reads: 148

```
Maidened successfully,  needs smaller wheels..   
![20180613_181648|243x500](upload://xhuSfTJPj7Hp9K5oAswVDzarEcU.jpg)
```

---
## \#5 Posted by: lrdesigns Posted at: 2018-06-14T08:17:21.666Z Reads: 117

```
[quote="slick, post:3, topic:58679"]
fur for the tail
[/quote]

This would be awesome!
```

---
## \#6 Posted by: squishy654 Posted at: 2018-06-15T15:56:15.893Z Reads: 106

```
oh man this thing needs 40 tooth wheel pulleys....

I put on some 97mm classics instead of the 107 to help with the gearing problem, but it was still too much, we were able to hit 30mph and there was more in it, lol...I need to gear it down to like 25mph with some torque for the 107's..

Current calc is 12cell liion with a 15/36 gearing with 200kv motors...I am thinking of just changing it to the 15/40....any help would be appreciated, the motors are only the ollin 50mm sensored.  I would like to get the speed to 20-25mph and increase the bottom end for more acceleration and climbing ability..

the best part was that I forgot I picked out this installed voltage regulator for a 10cell build, now that I have it all buttoned up, bolted together, I charged it beyond 50v and blew the regulator as soon as I turned it on, so no working lights or sound!! insert sad face here... next step is to open her back up and replace the regulator (I already have a beefer one to drop in that can handle the voltage) and then get her back...

Over-all, wonderful maiden, I think we did about 18 or 19 miles and we didn't loose a belt, have connection issue or anything. Motors ran a little warm with this gearing but they hung on and this thing is a dream to ride, it's a like a Cadillac, huge and heavy, and yet surprisingly capable...stay turned for more!
```

---
## \#7 Posted by: squishy654 Posted at: 2018-06-19T16:01:46.027Z Reads: 92

```
video of the speakers on the bench...1st test and already annoying the neighbors..lol
https://www.facebook.com/pirateSquishy/videos/10155636380008697/?query=this%20is%20how%20we%20do
```

---
## \#8 Posted by: wafflejock Posted at: 2018-06-19T17:40:38.643Z Reads: 86

```
Your daughter a fan of primus?

https://www.youtube.com/watch?v=aYDfwUJzYQg
```

---
## \#9 Posted by: squishy654 Posted at: 2018-06-19T19:39:30.328Z Reads: 78

```
I grew up in Pleasanton, CA, my very 1st rock concert as a teenager was Primus at the Greek Theater in Berkley CA...so yeah, she is...and Primus sucks!!!

I just had a completely successful shakedown cruise of about 13 miles doing one of my known loops through town playing the speaker the whole time on top volume, I ended up at 36% battery, and I think she wasn't fully charged, so not bad...its totally functional most likely reaching 20+miles with ease while the accessories are turned on.

I actually didn't wanna stop riding because riding and listening to music on that thing is just so much damn fun, it adds a whole new dimension to the experience and works best in the quiet woods away from city traffic..Pantera, Gesaffelstein and Zhu made for great tunes while riding..

The speaker sucks considerable juice, the board is fast as hell and very capable, I was cruising near 25mph and having to slow down on curves on the bike trail...I was flying, prolly went faster than 25mph plenty of times, I need a new speedo app now I can have the speed read to me (through voice telem), and everyone else around, while I ride...or have it speak GPS directions, lol...what a novel joke this thing is...I'm enjoying it..

Here she is in the wild, running 97's in classic and finalized trucks angles, I think I need to soften up the bushing a little, and she's tuned and ready for group rides to embarrass everyone!! Bring on the tacky flashy lights and loud ass obnoxious music!! It's the party board!![3636693665254711669|690x335](upload://b9ZtDxzoVzUP3XBW11BBJ7QJ1hL.jpg)
```

---
## \#10 Posted by: justsidewayz Posted at: 2018-06-19T19:45:16.840Z Reads: 73

```
Much rad wow!

I can hear it now!!!
https://youtu.be/PPzIWFJU_3s
```

---
## \#11 Posted by: oldskater Posted at: 2018-06-19T23:40:07.327Z Reads: 67

```
I have some 40t wheel pullies that Jeremy printed for the beaver.
```

---
## \#12 Posted by: squishy654 Posted at: 2018-09-06T21:01:36.650Z Reads: 53

```
https://www.youtube.com/watch?v=iQPahujNtHg
```

---
## \#13 Posted by: Sebike Posted at: 2018-09-06T21:41:33.649Z Reads: 42

```
Love this! That's one epic build. Nice job!
```

---
