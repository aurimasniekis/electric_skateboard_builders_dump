# Unnamed &#124; custom deck &#124; 10S5P &#124; Dual Hub 90mm &#124; 3D-designed first board

### Replies: 30 Views: 773

## \#1 Posted by: HansPeterHaastrup Posted at: 2018-07-26T08:32:00.445Z Reads: 195

```
Build a longboard they said - It will be fun they said. And yes! it is!
This is my first voyage into the world of longboards - electric and analog alike. The reason: 14km commute to work where the bike path is generally in excellent condition. Electric bikes are limited to 27,5 km/h which is a bit to slow for my taste.
So - the idea of getting an electric longboard was conceived.

I work in a fablab so the thought of building the board from scratch (or at least getting some parts and putting them together) seemed appropriate.

**Wheels**
I know that a lot of you guys spend a lot of time getting specific trucks and specific wheels for your rides but since I had very little knowledge I thought it best to get a set. I ordered a complete 90mm kit with dual hub motors, trucks, front wheels and ESC from Alien Power System. 
I've later found that those kits can be found on ebay but well... Now I have them. The most annoying thing was I have to wait for 5 weeks to get them - what to do?

**Batteries**
While waiting I ordered 50 cells (18650 type) from nkon.nl. I chose some 30A Sony cells rated for 3120mAh each (https://eu.nkon.nl/rechargeable/18650-size/sony-us18650vtc6.html). The plan is to pack them as 10S5P but since I can't charge a 10S pack I will do 2 5S packs instead. I know more charging time and less automated but Just for getting the board on the road this should work.

**Deck**
Now for the fun stuff! I had 5 weeks to burn so why not try to design a shape myself? I had very little to go on The only picture of the trucks mechanical layout was a vague description with some inch measurements on. well, I tried and came up with a general idea. The overall length of the board is 1m because.. it felt good when I looked at it.

I'm designing in Onshape and things got a little out of hand. Now I'm designing everything, from the battery mounts to the covers to the electronics bay. I will try and post pictures of all the parts as they finish on the 3d printers.

![esk8|690x375](upload://tUxoDX0hBUUj8IqrY7JJovaKHbD.jpg)
This is a rendering from last night.
```

---
## \#2 Posted by: bartroosen12 Posted at: 2018-07-26T08:41:51.321Z Reads: 176

```
Why you can't charge a 10S pack?
You gonna build a awesome vct6 pack and gonna split it whut? 😅
```

---
## \#3 Posted by: Grozniy Posted at: 2018-07-26T09:14:57.602Z Reads: 161

```
Get a BMS from @koralle and voila
```

---
## \#4 Posted by: HansPeterHaastrup Posted at: 2018-07-26T09:28:21.154Z Reads: 165

```
Well - I can't charge a 10S pack yet.. I got a cheap balancer/charger along with the cells from nkon but it can only do 6S.
i do plan on building a BMS for the whole 10S pack but just to get the board rolling I will start with the two 5S packs I know it's not optimal but it's a start.
```

---
## \#5 Posted by: HansPeterHaastrup Posted at: 2018-07-26T09:30:16.204Z Reads: 167

```
Thanks for the tip!
I see that a lot of people on here produce their own stuff. However, I would like to build it myself. It's about my pride about building the thing from the ground up. Specially the electronics since that's what I do for a living :slight_smile:
```

---
## \#6 Posted by: HansPeterHaastrup Posted at: 2018-07-26T09:39:17.752Z Reads: 165

```
![received_1904349682941573|235x500](upload://nXfaAa1Jj9jUkGLkRP1oRxKgce.jpeg)
The deck fresh from the CNC (Maslow CNC which is a whole project in itself)
I have did it in 18mm plywood and thought it was way too stiff but after jumping into it I think it has just the flex I want.
I'm a heavy guy (100+kg) so I'd rather have a thick board that can handle the stress...

![IMG_20180724_134439|666x500](upload://kC9wv1fsO4sa3DaWHGDCiGZTNw4.jpg)
First picture with the wheels on! Looking pretty neat! But it's my first and only board so I really don't have anything to compare with ;)

![IMG_20180725_201544|666x500](upload://nWL0Bu7ecA7URAc4i27RWMJWzSB.jpg)
Close-up of the P part of the pack. I've redesigned this part a few times to get it right. To handle the board flexing the screw mounts are oblong in the flex direction. Inter-cell connections will also have some bending properties
```

---
## \#7 Posted by: HansPeterHaastrup Posted at: 2018-07-26T09:47:26.118Z Reads: 151

```
![electronics%20bay|690x439](upload://cFwvjSQMe1oroOBQRbb6xc126OH.PNG)
Some more details on the electronics bay.
This was modeled from the motor driver that I've got. The square pieces on top of the (green) PCB are the heatsink mounts for the FETs. The height of those is matched to the recess going around the perimeter of the enclosure. I have made a heatsink that fits into the recess and thus closes up the electronics bay when installed.

The part on the left side is a cover for the wires that go to the motors. I only have a single wire to each motor fo the part slides down and fixates them. it's secured with two M3 screws.
```

---
## \#8 Posted by: HansPeterHaastrup Posted at: 2018-07-26T09:49:24.474Z Reads: 149

```
![IMG_20180725_164436|666x500](upload://3siPBxzyxVB8ueubnwylgnqrMIP.jpg)
The electronics Bay and te corresponding heatsink

![IMG_20180725_164500|666x500](upload://v9mMwKj5WKf2UTVAk7KVS8ORuFK.jpg)
Aaand on top of each other.
The cooling find will be downward and my hope is that the airflow will keep the heatsink cooled
```

---
## \#9 Posted by: Grozniy Posted at: 2018-07-26T09:52:38.718Z Reads: 150

```
If you're CNC ING your deck, why not do it like @Hummie deck? 
![board%203|375x500](upload://rXpUpc9dmjiXM3UU48BaeXeffJ.jpg)![board%202|666x500](upload://fZAPjCnOc6aCAV5MVUaZrTbaZqN.jpg)
```

---
## \#10 Posted by: HansPeterHaastrup Posted at: 2018-07-26T10:19:43.737Z Reads: 135

```
dang, that looks sweet!
I do think that he's got some double-sided machining going on and my cnc don't do that happily.
Also I'm as green as it gets with regards to building boards :smiley:
The recess for the batteries look really nice! That's something I didn't even think about. Maybe I should redo the whole battery protection thing I have going on.. Currently it's 3D printed all the way byt a plywood enclosure would be far more durable.
Thanks!
```

---
## \#11 Posted by: pat.speed Posted at: 2018-07-26T11:28:14.463Z Reads: 129

```
Nice build going here, I’m thinking of doing the same for my deck. Did you just use normal plywood? And I would be careful as the most likely point to fail is the nose and tail, maybe some fibreglass would help to strengthen it. HobbyKing has cheap fibreglass if you need it
```

---
## \#12 Posted by: tex Posted at: 2018-07-26T11:32:09.514Z Reads: 127

```
Very good work. ;)
```

---
## \#13 Posted by: Narnash Posted at: 2018-07-26T12:04:24.086Z Reads: 130

```
Just as a hint this could also be a -maybe temporary- way to charge with a 6s (or 5s in your case) charger and drive with a 12s (or 10s) board.
https://www.electric-skateboard.builders/t/how-to-balance-charge-a-12s-battery-pack/48705/21

Or to get an excuse to get a nice LiPo / LI-Ion charger like a junsi 3010b for example 
I like to go with a balance charger rather than a BMS for the extra features they have also the flexability to make beefe packs for other projects.
```

---
## \#14 Posted by: HansPeterHaastrup Posted at: 2018-08-01T18:19:12.637Z Reads: 101

```
Hey! sorry for not answering sooner, been so busy with printing parts and a lot of other stuff..
Yes it's normal plywood - at least I think it is. I don't really know.. I moved in about a year ago and the plywood was there when I did.. so I think it's normal but it's 18mm thick. I was really worried about the stiffness but I really like it. It's flexible enough for me (105kg)
A friend of mine is riding 12mm but he's only about 80kg so he can afford it ;)

Nice tip about the fibreglass! I want to use this board for cummuting so it's important that it doesn't break in the middle of nowhere
```

---
## \#15 Posted by: HansPeterHaastrup Posted at: 2018-08-01T18:20:39.184Z Reads: 102

```
Thanks man!
That's exactly what I ended up doing.
I had a look on the Junsi 3010b - it's pretty expensive! I can live with charging two packs until I make a BMS. well - I have to ;)
```

---
## \#16 Posted by: sk8l8r Posted at: 2018-08-01T18:25:22.024Z Reads: 101

```
Really like the heat sink!  :slight_smile:
```

---
## \#17 Posted by: HansPeterHaastrup Posted at: 2018-08-01T18:29:58.011Z Reads: 112

```
Okay, time for an update. A lot of pictures of pack building and assembly. Hope you'll like it!

![IMG_20180727_181600|666x500](upload://3HBKxUHaVENc3kaZvOc5F2a9VRs.jpg)
Finished all the printing for cell mounts. Took a few days on/off

![IMG_20180727_205049|375x500](upload://ej25OMB009zvvQfXAalOmWnFOf3.jpg)
I figured the easiest way to solder (I don't have access to a spot welder) the nickel strips was to use a hole puncher for each cell. Then I could solder in the half circles.

![IMG_20180728_094721|666x500](upload://hNne6wOYfQkx938NHVqNiQ6tSz0.jpg)
Started working the balancing plug on the first pack. Also I mounted the connection between the positive on pack 1 and the negative on pack 2. Be sure not to short anything now!

![IMG_20180728_121627|666x500](upload://A1LyCIQajcp77fkofTlUJylEO5J.jpg)
Close-up of the charging port.

![IMG_20180728_121640|375x500](upload://4XBZuo3yysFWWaNjwaW8zToRanv.jpg)
This kinda summarize the pack

![IMG_20180728_130832|666x500](upload://6OJevqrhf2jshiTz1zFRI4Mx6Ag.jpg)
But I really like the way it looks! 

![IMG_20180728_152331|666x500](upload://fOeHJQYHP75t2Ra4RtnVUYlFOq0.jpg)
Such a shame to pack all that work behind black plastic.

![IMG_20180728_153454|666x500](upload://2OEmJ34NXtuZNFLVgNVBINH7ivM.jpg)
Sooo, looking pretty nice on the road. Now for some testing.
```

---
## \#18 Posted by: HansPeterHaastrup Posted at: 2018-08-01T18:31:05.709Z Reads: 104

```
Thanks!
I have a thing for machined parts - and hey I had a huge block of heatsink lying in the corner just waiting for this.. well, actually it was waiting for an amplifier project but hey..
```

---
## \#19 Posted by: moon Posted at: 2018-08-01T18:35:55.266Z Reads: 105

```
What was your experience with soldering 18650?
```

---
## \#20 Posted by: HansPeterHaastrup Posted at: 2018-08-01T18:42:46.712Z Reads: 107

```
I'm positively surprised!
The nickel strip was super easy to solder on but that was more or less expected. I had expected the solder to ball-up on especially the negative side. but I took my biggest soldering iron and it was actually pretty painless. I used a lot of solder but I'm super scared that if I make a bad connection the whole thing will just explode in my face.
The positive terminal have 3 thermal-relief pins so that was super easy but I was trying to avoid too much time on the terminals.
```

---
## \#21 Posted by: legend27 Posted at: 2018-08-01T20:33:51.772Z Reads: 94

```
Nice project! It looks pretty stealth. But one thing im concered about: Are you sure that one nickel strip at the end is enough? The maximum amps this battery can draw is 100A and that nickel strip can probably take a maximum of 20A?
```

---
## \#22 Posted by: HansPeterHaastrup Posted at: 2018-08-01T21:33:28.859Z Reads: 94

```
uh-oh..

I haven't really considered that. I just thought, hey 10mm nickel strip that's what everybody else is doing.
You're right though - I have to reinforce the strips and not just the end pieces - it has to be all over the place!
I'll admit though, I was pretty generous with the solder for this specific reason but that won't help all the potential current-bottlenecks that I have been creating.
Thanks forthe heads up!
```

---
## \#23 Posted by: pat.speed Posted at: 2018-08-01T21:41:27.178Z Reads: 89

```
Yeah he’s right, if I was you I would just solder a piece of 10awg silicone wire across the gap. I would also do that for your series terminals but with 12awg or add at least 2 more layers of nickel as these strips can only handle about 8amps cont
```

---
## \#24 Posted by: HansPeterHaastrup Posted at: 2018-08-11T09:59:14.166Z Reads: 78

```
Okay, we need to talk about hub motors. I read that they will get hot but how hot exactly???
![flir_20180731T113617|640x480](upload://wIlUkwtGbDWqvwnBoxnhXe1uIGX.jpg)

This is one of the motors after a 10-15 minute trip with some hills. I needed to charge the IR camera before I could take the picture so about 5 minutes after the trip. How hot should those motors get exactly? Anyone who knows?

Also, the point is not even the hotspot of the image. I think it's 95 or 98 degrees (C)
```

---
## \#25 Posted by: bartroosen12 Posted at: 2018-08-11T18:35:53.518Z Reads: 66

```
Damn? After only 15min, that's pretty hot, I have 'ownboard' hubmotors and can do like 35km rides with my battery. After 2h riding the wheels are also very hot but never measured.
But 100°C looks very hot to me.

Which esc do you use?
Maybe they put out to much amps for those motors, I guess 20A each is more than enough.
I run my hubmotors at 10A each.
```

---
## \#26 Posted by: HansPeterHaastrup Posted at: 2018-08-11T19:27:22.276Z Reads: 61

```
Wow!
I was planning on using my board for a 14km commute and should have plenty fuel for that with my 10S5P pack.

The thing is that I've got the motors and controller as a kit from Alien Power System. I haven't been able to find any documentation at all on the (Chinese) controller.
He's still on Vacation but I will ask as soon as possible. If it's just as simple as limiting the output power it would be sooooo nice!
Also I don't have enough power to go uphill but that might be related. 
Do the motor windings saturate?
```

---
## \#27 Posted by: bartroosen12 Posted at: 2018-08-11T19:30:29.974Z Reads: 60

```
You got this kit?
https://alienpowersystem.com/shop/cnc-kit/hub-brushless-motors/bldc-sensored-90mm-hub-motor-and-controller-for-longboard/
Because then I think the ess is like the same, I guess maybe max 30A so 15A each.
Maybe becuase you did hills, those 'cheap' hubmotors are not made for doing hillclimbs.
```

---
## \#28 Posted by: HansPeterHaastrup Posted at: 2018-08-11T19:50:38.112Z Reads: 52

```
Yep that's the one.

I should have read a lot more before I took the plunge and ordered those. I didn't think we had serious hills where I live (Denmark) so I didn't thought that it would make such a difference.
It should still be possible to program the escape to limit the power but I need some documentation on how to do that.

I have been thinking about making a VESC clone for the board. At least that will give me the configuration options for the motor :)
```

---
## \#29 Posted by: bartroosen12 Posted at: 2018-08-11T20:00:49.901Z Reads: 48

```
Well as long as the wheels don't smell bad (like melting rubber it should be okay 😅
I've had a small lou board and it had a single hubmotor, after 5min uphill i checked the wheels and I swear they were really smoking. I guess the insulation from windings were melting and the rubber was hot as fuck.
i couldn't touch the metal on the sides because they were burning hot but with these dual hubs they are much cooler and no problems with hills, but they still get hot but I shouldn't be worried.
I have had a 50mm sk3 belt setup and the motor was also so hot after rides but never had problems with that :smile:
```

---
## \#30 Posted by: HansPeterHaastrup Posted at: 2018-08-12T05:58:14.266Z Reads: 42

```
Wow, that sounds INSANE!
Good to know that they should be able to handle the heat. Usually that kind of heat means some kind of trouble. I have been thinking of milling some heatsinks for the truck since some of the heat is transferred that way. But I think the bearings might be damaged from the heat as well, I don't think the lubricant is rated for high temperature action...
But as you say, I'm better of with two motors than one ;)
```

---
