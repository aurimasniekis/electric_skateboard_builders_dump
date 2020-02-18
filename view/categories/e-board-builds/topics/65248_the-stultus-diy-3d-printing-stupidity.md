# The Stultus - DIY/ 3D printing/ stupidity

### Replies: 8 Views: 445

## \#1 Posted by: xilw3r Posted at: 2018-08-18T08:00:11.001Z Reads: 170

```
Hello good people of the interwebz. 

This here is a journey of my first "e-board" being birthed (quotes, because most longboard riding people will probably shriek in disgust of this abomination).
Stultus means idiot in latin.

At a glance:
**Board** - shitty chinese thing. I literally got ripped off here. It came with crappy cast aluminium trucks (regular skateboard style, had casting failures in the forms of holes) and hard plastic "tyres" which were more like something that you would expect on a toy car... yeah. Also, the ends were less wide and with all the things mounted it bottomed out, so I had to cut off the ends. Not much space left for feet now...
**ESC** - vesc 4.12 at first, soldered by a local student.. quite shit actually, blew the DRV in 20 minutes, couldnt even detect FOC, motor was almost knocking at low rpm in bldc. Now I slapped in a FlipSky FSESC6.6 (big thanks to @b.sk8 !) , oh boy, what an improvement. Driven by some idiot level (my level) arduino code, just feeds ppm into the esc. Oh, fitting the Flipsky ESC was a pain, I had to put the BMS in the originally vesc's spot and also remove the loop key, not to mention a lot of dremeling to barely fit everything. I kind of need to reprint the battery box now for a nice fit. And I want that loop key.
**BMS** - from Alien, 50A discharge with an e-switch.
**Remote** - printed in PLA, quickly thrown together in CAD with a 18650 cell and an arduino nano. NRF24 is the tranceiver here and a potentiometer for input, a safety trigger exists. Oh, more idiot points are earned here by using a gear reduction for the potentiometer (i wanted a smaller travel for the full range) and a spring loaded cam mechanism for returning the thing to center. Yeah..
**Battery** - DIY 10S4P VTC6, cells and the "technology" supplied by my workplace, so I cant really show much of it or I would get sued :zipper_mouth_face: Lets just say it has a shit load of fuses.. per cell. And also a lot of copper is involved, that much you can spy in the photos below.
**Battery case** - designed and printed in PLA, could have been made smaller in hindsight, nothing fancy.
**Motor** - E-MAX GT5345, when I got this SK3 were out of stock for months. It is size equivalent of a 6374. But to be honest does not impress, rather large air gap between stator and magnets, the magnets look like they were glued inside the bell by a todler, unequal gaps, some are at an angle, ammounts of epoxy vary all over the place. Would not reccomend.
**Mount** - self "designed", come on, its just a 5mm stainless steel plate, laser cut, with a diy idler pulley.
**Pulleys** - HTD 5M steel 16 teeth for the motor and printed in PLA 85 teeth for the wheel.
**Trucks** - DIY, basically NoSno rip offs, but from steel. Yes, they are heavy. The axle is 25mm diameter. Solid. Shin breaking stuff. "Bushings" are industrial vibration isolators, with sides cut off. Hardness is 55A if memory serves. Let me tell you, cutting them with a knife sucks a lot. WD-40 helps immensly.
**Wheels** - 225mm diameter (8.8 inches), steel hubs, basically cartwheel stuff. Making mounting holes is nearly impossible without a mill, so I designed and printed a hub for the driven wheel (PLA)


Lets start with the end, so far it has seen about 30-40 km of shitty pavements. Which are also the main reason why I went pneumatic wheels. Urethane just would not cut it in most places. I reached 25 km/h so far, for me, that feels like a lot right now (no boarding experience), but I want more hill climbing ability (is it even possible to get up a lets say 20% hill with a single 6374 motor on enourmous wheels?) and the motor gets rather hot rather fast. But i love riding this anyways.

Single drive, because I am a cheapskate.
![IMG_20180817_172618|690x388](upload://smu23WGC218ttS9QazjDAAQNu5A.jpg)
![IMG_20180717_083522|690x388](upload://4TFLMHETQWwaNmQLDtzYuNp9c86.jpg)
![IMG_20180716_225402|690x388](upload://8Z4wvkWOGuITL9DqDQ1cXkd36QU.jpg)

The (also DIY) printer that birthed all the components. man, it took some effort to upgrade this thing for reliable 24hour prints, and I still have this annoying wobbling of the Z-axis:
![IMG_20180619_181725|690x388](upload://5bagfjGIZs4ZVLnkMu7DFaoJLfE.jpg)
![IMG_20180701_122352|690x388](upload://qCy0vBp1aGxSlt2EXx2HnovtM1O.jpg)
![IMG_20180419_220820|690x388](upload://2CByTXYN93TAi5o5w19VVNF9SA7.jpg)
![IMG_20180630_230242|690x388](upload://xvO8svraORjVGH0t6V37erbxq8C.jpg)

Base plates and motor mount plate- mount (lol) after welding. My first "functional" welds (with a MIG, so I guess I was cheating):
![IMG_20180310_205055|690x388](upload://agdWIJggq3mNevSEOewayqOr8so.jpg)
![IMG_20180310_205103|690x388](upload://4vQvnBwcwcOa2pynnQwfTFtrLRk.jpg)

Laser cut mounts (got them for cut free cause Im such a nice fellow) and a freshly hand turned pulley:
![IMG_20180222_173559|690x388](upload://qsdhmJ8m85jtqK6KfTUAovu1OoK.jpg)
![IMG_20180607_224308|690x388](upload://aRNdxWEj1n8Iy0slFLk68JiWN9H.jpg)

How the board looked originally and next to it you can see the original "wheels" and my replacements:
![IMG_20180313_183119|690x388](upload://s8Dr7d7NbmtX0WZP7hUWjI4NP7W.jpg)

Front axle up close:
![IMG_20180716_090035|690x388](upload://v4sezSSSpxHqrJt89OCLFL3H7c8.jpg)

Loop key:
![IMG_20180327_134520|690x388](upload://4Iep0XmLu9kf0ZE1HSaYrF3rOmd.jpg)
![IMG_20180327_125943|690x388](upload://8jCUmZUdmcwAyNwlu0gd9xUf6Yz.jpg)

Before deciding to print a hub completely I was expreimentally arriving at the most correct shape for the existing hubs by printing some flat profiles. Ended up with a massive new hub anyhow:
![IMG_20180217_233505|690x388](upload://n5Vjgn431XvwNz2ZLKwPVl8nRNb.jpg)
![IMG_20180624_092023|690x388](upload://bNCqXzh0x7QKCsW1PS8ebFIsK3m.jpg)

NRF-arduino unholy union, still missing the 16V 22uf cap in the first picture:
![IMG_20180630_213103|690x388](upload://AnGh0HvcFlxBIKjgRuZmhBAMcum.jpg)
![IMG_20180814_203751|690x388](upload://3LLYMHYEysutgTYfNR0pSkjN4nh.jpg)

Battery in the box already. Its a weird construction, my second battery (first one was for a motorcycle :wink: ) We had scrap copper plates, I sodlered them into groups with a nasty 200W iron (each connected by 2 fat copper wires- 6sq mm each), then welded the cells. The pack is a two part construction that was bent into shape after completion, you can almost see the bent copper wires in the middle back:
![IMG_20180708_235404|690x388](upload://geuKzgRMhzp5NGk0iUwjr3p7RO0.jpg)

A nice group shot of most of the remote pieces, battrey and the bms:
![IMG_20180701_183630|690x388](upload://hlaBnf0kEu3VCdJoU0BaCv3QWRi.jpg)

Finished remote:
![IMG_20180701_230533|281x500](upload://4AusJRYtCbdhlnVBpWeFD0rQlyj.jpg)

Everything mounted into place (vesc had a little holder printed for it, I know the plastic basically touching the FET's is not a great idea, but it didnt melt in the first 20 minutes :D and now its all gone, the BMS sits there at an angle now:
![IMG_20180716_085958|690x388](upload://g4x6tE6znSDAcJDsf4Xj9MUmJ7O.jpg)

And last but definitely not least - the sketchiest charging solution you could come up with: an old ATX supply with a DC-DC boost converter from aliexpress. Its quite a cool thing, can set up any charge current and voltage, has CC CV, only thing is, it screams an annoying high pitched sound, but it was 14 euros for a basically universal charger, so I think im fine with it. For now:
![IMG_20180815_213918|690x388](upload://pGWMyCB2WznAwsXqIoENUASUgGY.jpg)

Questions? No? Class dismissed :D
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-08-18T09:08:49.933Z Reads: 122

```
but hey, it looks great
```

---
## \#3 Posted by: rojitor Posted at: 2018-08-18T09:38:13.912Z Reads: 112

```
Awesome job mate.
```

---
## \#4 Posted by: b.sk8 Posted at: 2018-08-18T09:51:30.950Z Reads: 107

```
Nicely done and  I am glad FLIPSKY worked well!! You get me curious about the battery secrets...Very beefy copper bars interesting. Let us know how it rides.
```

---
## \#5 Posted by: xilw3r Posted at: 2018-08-21T05:06:28.792Z Reads: 79

```
It rides better than expected.

I mean lets be honest its a creaky piece of shit, but i love the flying feeling when going on a board like this.
Flying here is subjective, because I reached max 26 km/h on this thing. It could probably go to 30 with a full battery, but 25 is faster than I am comfortable with at the moment anyways, it becomes a bit unstable at that point. I tightened the nuts on my rear truck to preload the bushings more, that helped.

But not all is great, It does not climb hills good at all. Even not so steep ones. I mean come on VTC6 cells in 4P should give me plenty of power, right ? I see people using even 2 motors with 4p packs here on 30q, which is pretty much the same in amp output as my pack. I can only figure that my motor is truly a piece of crap? 

In vesc I have:
battery current 40A
phase/ motor current 60/65A (dont remember), sure I could go higher here, but the motor gets hot enough as it is. I am designing a better fan to bolt on its end, see if that helps at all.

Another thing, even if I have the low battery cut off start in vesc at 33V, I get somehow low power when climbing a hill with lets say ~35V at sag. Almost no torque at all, and then in a more level area its a sudden jump in torque, even gets me out of balance. Could this be that low voltage limiter on the vesc thats doing this ? Or is it perhaps the FET temperature limiter?

I need to battle the heat on all fronts. Having the esc enclosure in a sealed plastic box aint too bright. Time to design a new box along with that motor fan
```

---
## \#6 Posted by: brenternet Posted at: 2018-08-21T08:50:42.348Z Reads: 62

```
This board is horrific. Love it!
```

---
## \#7 Posted by: xilw3r Posted at: 2018-08-21T13:36:02.005Z Reads: 64

```
Modeled up the end of my motor bell and made a fan that bolted on with the first try, yay.

The idea was to simply extend the fins in order to accelerate the air being thrown out more and thus create a higher pressure drop in the motor. I am not sure how well this works, it still gets warm after driving on a level surface. Need to do some quantifiable tests.
On a side note  I found a bluetooth module lying around at work that I can use with @Ackmaniac's vesc monitor app :) lucky, no need to wait for a month to get it shipped.

Just the fan:
![fan1|690x368](upload://vlCY9g0YL0zTSBLgmmgJxxY8tmk.png)

The funny shape is made to rest against the existing supports of the motor:
![fan2|690x459](upload://knG0oGVgB8nZKaN1NZPg5PbIFQ4.png)

Real life:
![IMG_20180821_162927|690x388](upload://e6iaYBZCPjSF5qx7bckucBKQPGx.jpg)
```

---
## \#8 Posted by: xilw3r Posted at: 2018-09-05T13:49:49.356Z Reads: 45

```
Got myself some knock off bluetooth module MLT-BT05, found one just laying around at work. Lucky me.

Everything seems fine, besides the flipsky measuring the wrong voltage of my battery pack (kinda bugs me that one) and one other thing- I never seem to reach the maximum motor current I have set up in the ESC.

I have set like 73A motor max current, but I only manage to reach 65A, anyone know what might be the issue?  Is it beacause I am in BLDC mode? I saw someone reporting the same issue, only on on 4,12 vesc
```

---
