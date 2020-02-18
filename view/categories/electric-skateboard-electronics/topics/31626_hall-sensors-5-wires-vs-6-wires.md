# Hall sensors 5 wires vs 6 wires

### Replies: 36 Views: 9336

## \#1 Posted by: Brad Posted at: 2017-08-28T06:58:28.519Z Reads: 459

```
Hello

I wish to transplant my Evolve Bamboo GT onto another board and replace the motos with two red MayTech 6555 170Kv sensored motors.
<img src="/uploads/db1493/original/3X/e/1/e150fb9b3ac2b1f40b3f85d63df64e5137d83994.jpg" width="690" height="423">

The Evolve wires for phase leads is actually a three pinned plug which won't be a problem as I will just simply solder the phase wires onto the three pin plug.
<img src="/uploads/db1493/original/3X/6/1/61a791b51837586ac72655a6e26e620a2e4f675a.JPG" width="500" height="500">

My headache is with the hall sensors. The MayTech hall sensor has 6 wires of which only 3 of these has colors that is the same as the Evolve sensors. 

The Evolve sensors only has 5 wires and only have black,red and yellow that my MayTech sensors have but does not have orange, green or brown.

Can you guys and gals help me out here?

Image as below. (Black plug is MayTech and white plug is Evolve)
<img src="/uploads/db1493/original/3X/8/b/8b9e73cd78364f61ab713c0b603203c796e4bbe3.jpg" width="386" height="500">
```

---
## \#2 Posted by: Pimousse Posted at: 2017-08-28T07:05:55.789Z Reads: 433

```
Probably the temperature sensor missing on the Evolve one.
Temperature sensor is the yellow wire on the Maytech connector.
Build a 6pin to 5 pin adapter skipping this one and you should me fine. ;)
```

---
## \#3 Posted by: scepterr Posted at: 2017-08-28T07:06:52.275Z Reads: 429

```
Do a little transplant surgery
```

---
## \#4 Posted by: Brad Posted at: 2017-08-28T07:09:41.528Z Reads: 434

```
@Pimousse So you are saying that the wires is in the right order from black to red despite the colors? If so, then I can just cut off the yellow and transfer the rest over.

@scepterr Doing that!
```

---
## \#6 Posted by: Brad Posted at: 2017-08-28T07:15:00.682Z Reads: 411

```
Good thing I have this and various other sizes. What made me go out and buy these was the VESC6 due to using larger plugs which was a blessing in diguse. :joy:
<img src="/uploads/db1493/original/3X/4/2/42b0505d09dfa3760323efd7b35ffe5beacf2238.JPG" width="666" height="500">
```

---
## \#7 Posted by: Pimousse Posted at: 2017-08-28T07:15:54.530Z Reads: 399

```
Sensored brushless motors use the same pinout as it is a standard.
Even if Evolve is this case does not comply completely with the standard using 5pin connector, I can't see them mixing 5V and GND (see black and red wires at the same place as standard ones). A,B and C hall sensor can be mixed up, in any case, you will run a detection through BLDC Tool.
Should be fine. ;)
```

---
## \#8 Posted by: Brad Posted at: 2017-08-28T07:19:11.848Z Reads: 389

```
I do not see a USB port for me to do BLDC or any other means. but I could just do trail and error with the middle 3 wires till it works right.

On second thoughts, I will see if I can dig any info on the net on which ABC in which order they set it up.
```

---
## \#9 Posted by: Pimousse Posted at: 2017-08-28T07:22:28.527Z Reads: 381

```
Oh sorry, I was assuming you wanted to run Maytech motors with a VESC.
Well, that case, you will need to try different combinations of the 3 power leads of the motor to match the A,B,C sensors order.
```

---
## \#10 Posted by: scepterr Posted at: 2017-08-28T07:23:34.302Z Reads: 367

```
Sensor order doesn't matter as long as gnd and v+ are correct
```

---
## \#11 Posted by: Brad Posted at: 2017-08-28T07:24:42.019Z Reads: 362

```
@scepterr That is good to hear! :+1:
```

---
## \#12 Posted by: Brad Posted at: 2017-08-28T08:07:31.767Z Reads: 373

```
Ok, looking good. Sensor wires are so fine but no problem stripping the insulation off.

Phase wires is not what I expected, thought it would be copper but is not.

Time to solder it together!
<img src="/uploads/db1493/original/3X/2/1/21c67a6e27d4965e89c04712d23ddae8b5b30398.jpg" width="566" height="500">
```

---
## \#13 Posted by: scepterr Posted at: 2017-08-28T08:12:27.376Z Reads: 358

```
Phase wires are tinned copper, I would've left that mt60 connector... pretty sure the female vesc leads plug right in(4-5mm)
```

---
## \#14 Posted by: Brad Posted at: 2017-08-28T08:14:43.325Z Reads: 363

```
The mt60 connecter is from the old Evolve 5565 motors, I cut it off so I can transplant it onto the MayTech 6555 170Kv motor phase wires as it had bullets instead and the Evolve has mt60 connecters.
```

---
## \#15 Posted by: scepterr Posted at: 2017-08-28T08:15:57.641Z Reads: 369

```
All good then :slight_smile:
```

---
## \#16 Posted by: Brad Posted at: 2017-08-28T09:56:46.222Z Reads: 379

```
First time I have soldered, sure that it is not the best but it should do for now.
<img src="/uploads/db1493/original/3X/b/0/b07b5e66a46bd098a773d3301789eb2c7c04d6f4.JPG" width="606" height="499">
<img src="/uploads/db1493/original/3X/f/e/fe759851ae4f8d29d373aa46c7017bb1451a8125.JPG" width="652" height="492">
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-08-28T11:33:09.988Z Reads: 366

```
Sorry to hurt your feelings, but those are some of the worst solders I’ve ever seen.  
1. Get a hotter iron
2. With a flat tip, put the iron on top of all the lumps until the solder sinks into the wire
3. Re heat shrink and your ready to go.
Sorry to sound like an a hole, just trying to help.  Your first solder job was better than mine 😉.  Anyways, there should not be any lumps on soldered connections 
<img src="/uploads/db1493/original/3X/3/b/3b362dd31a7d6a3f2673a48799803558a5e6df74.jpeg" width="259" height="194"><img src="/uploads/db1493/original/3X/e/f/ef9cf5a1fe2e1f6fa3fa2a090927d4632fbc60c3.jpeg" width="245" height="206">
@Brad
```

---
## \#18 Posted by: Brad Posted at: 2017-08-28T11:48:08.137Z Reads: 353

```
No hurt at all. This is why I posted the pics, for feedback.

Just the first time I done it. Had the tip set at 400 degrees.

Will re-do it tomorrow arvo.
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-08-28T12:20:23.758Z Reads: 347

```
Yea, the tip should be at somewhere between 600 and 750f (398c)
```

---
## \#20 Posted by: HOPPEMSU Posted at: 2017-10-30T12:51:23.299Z Reads: 313

```
I know this is an old pos that I'm ressurecting, but I'm having trouble finding an answer.  If you arent using VESC, how do you go about testing the order of the sensor phase wires to know the order is correct?  I don't want to blow my motor or esc...
```

---
## \#21 Posted by: Brad Posted at: 2017-10-30T12:59:52.623Z Reads: 315

```
Sensor wire a/b/c order does not matter just make sure that V+ (red) and ground (black) is in the correct order.

For phase wires, if the motor spins the wrong way, just simply switch any two random phase wires and viola, the motor will spin the other way.
```

---
## \#22 Posted by: goodblake Posted at: 2018-04-25T13:42:30.198Z Reads: 253

```
I accidentally pulled out the red wire from the Hall sensor harness on my Evolve Carbon GT, and I am trying to figure out how to fix. Evolve sells the harness for $5 and probably $15 shipping. I know I could get a 100 of these for that and Id rather not give them my business. 

Anyways I am trying to figure out if I can just reattach the one wire to the harness or if I need to cut all the wires and solder a new harness on there?

All of the replacement harnesses I can find have a different wire pattern. I know @Brad said only the red and black wires matter the order. However all the replacements seem to be Blue|Green|Yellow|Black|Red vs the Evolve one that is Black|Yellow|White|Blue|Red. I can't seem to find any that have Black and Red on the ends. 

All help appreciated
```

---
## \#23 Posted by: Brad Posted at: 2018-04-25T13:56:25.762Z Reads: 238

```
You can just ignore the colour on the replacement harness cos it will have to plug into the PCB on your Evolve board and the colour order on the PCB is still the same.

So if that is the case, you can just reattach black into blue as blue will just go into black on the PCB board inside the enclosure. 

That way black(blue as the new ground) is still first and red is still last (same as Evolve setup) and middle colours does not matter.

I hope I understood you right :slight_smile:
```

---
## \#24 Posted by: flocon2001 Posted at: 2018-05-25T06:44:09.469Z Reads: 208

```
Hi Brad , can you tell where you bought all those connectors ?
```

---
## \#25 Posted by: Brad Posted at: 2018-05-25T08:48:35.584Z Reads: 208

```
I bought them off Ebay. You can also buy off Aliexpress.

If you want easy way to connect to JST-PH for hall sensors, you can just get an adapter from [Pyscotiller](https://psychotiller.com/product/sensor-wire-adaptor) or [Torqueboard](collections/electrical-connectors/products/vesc-sensor-wires) or [Unik](https://www.unikboards.com/en/boutique/connecteur-pour-moteur-sensored-vers-vesc/).
```

---
## \#26 Posted by: Josh.V Posted at: 2019-07-03T06:31:12.381Z Reads: 84

```
Hi. Just found this post after I'd almost given up on my troubleshooting. Hadn't yet seen anyone tinkering with the evolve wiring.. I bought two replacement racestar motors for my bamboo GT. Thought it'd be plug and play, but one of the motors spins in the opposite direction when mounted. Everyone had been saying to change two of the phase wires around but these wires have different connectors (the triangle 3pin plug). So if I can manage to re-solder two of these wires around it should in theory, reverse the direction yes?
```

---
## \#27 Posted by: Andy87 Posted at: 2019-07-03T07:37:56.744Z Reads: 78

```
that´s correct [](http://)
```

---
## \#28 Posted by: hans_maier Posted at: 2019-11-29T09:50:01.859Z Reads: 28

```
It seems I have a similar problem:
I would like to connect the hall sensor cables from this [direct drive motor](https://www.mboards.co/collections/electric-skateboard-motors/products/direct-drive-motor-kit) to this [Trampa VESC](http://www.trampaboards.com/vesc-6-plus-benjamin-vedder-electronic-speed-controller-p-26762.html).

The hall sensor cable from the direct motor has five colors: black; green; yellow; blue; red

![IMG_7533|564x500](upload://fydqCRsKKu4ccG7wrXOqcXUwywb.jpeg)

The Trampa VESC has 6 connections:  V+; Temp; H1; H2; H3; GND

![IMG_7532|374x500](upload://AgrlW69aicE31apd3JF2sTzgEbo.jpeg) 

To which ports on the VESC does black, green, yellow, blue, and red from the motors connect to?

Thanks a lot for your help (from an esk8 novice)!
```

---
## \#29 Posted by: Doneone Posted at: 2019-11-29T13:04:04.838Z Reads: 25

```
I learned that the outer wires are positive and negative current. Should be also the case with your hub motors. Then you got the temp sensor which in your case might be absent. The rest doesn't matter where they connect to. V+ is positive and gnd is ground (negative). Maybe you just need to skip the temp sensor and connect the rest as indicated. Trampa sells the 6-strand connectors but you can also get them anywhere else I suppose.
```

---
## \#30 Posted by: Supervolant Posted at: 2019-11-29T16:04:07.503Z Reads: 26

```
Having the same issue mate, just that I have to find that out for 6 wires.... hope someone knows and replies in here! :slight_smile:
```

---
## \#31 Posted by: hans_maier Posted at: 2019-11-29T21:37:04.320Z Reads: 26

```
Thanks so much! I hopefully assume correctly:

(1)

 `red = GND` [wrong!] \
   `black = V+ ` [wrong!]

... and this is all I need to know!

(2)

`white = Temperature sensor` - this one seems to be missing.

(3)

 `green = H1`\
   `yellow = H2`\
`blue = H3`

Here it does not matter whether `H1` on the motor also corresponds to `H1` or instead to `H2` or `H3` on the VESC etc.

Thus, will get a new 6 pin JST connector and pay attention that `V+` and `GND` are connected correctly from the motors to the VESC. This should work without soldering, right? Unfortunately, I do not know how to do that ...
```

---
## \#32 Posted by: Doneone Posted at: 2019-11-29T21:55:30.854Z Reads: 26

```
I assume you are not assuming correctly. Normally positive is red and black is negative. What you can't do or don't know you will have to learn in order to complete your board. You either have to crimp the connector or solder them.
```

---
## \#33 Posted by: Supervolant Posted at: 2019-11-29T22:00:47.244Z Reads: 25

```
Hey @Hans_maier I do think @Doneone is correct.

Here in this post I found the pinout of an APS motor: `https://www.electric-skateboard.builders/t/aps-motor-sensor-extansion/66451`


It would be very irritating if they switch around positive (normaly red) and negative (normaly black).

This is what I soldered now for, hoping to get an final clarification answer from the manufacturer soon.

Before that clarification, I rather not connect anything electrically up. Just in case... this topic is extremely confusing all over the forum to be honest.

- Rob
```

---
## \#34 Posted by: hans_maier Posted at: 2019-11-29T22:03:02.426Z Reads: 24

```
@Doneone and @Supervolant  Thanks a lot for mentioning!!
I got it wrong:

 `red = +5V` \
`black = GND`

Pictures is this post https://www.electric-skateboard.builders/t/motor-sensor-plug-doesnt-fit-on-vesc-solved/22984/36?u=hans_maier are somewhat confusing; however, it is mentioned correctly in the text.
```

---
## \#35 Posted by: Doneone Posted at: 2019-11-30T00:45:42.894Z Reads: 20

```
You can do it!
```

---
## \#36 Posted by: hans_maier Posted at: 2019-11-30T01:11:49.850Z Reads: 21

```
:slight_smile: Appreciate your help!
```

---
## \#37 Posted by: hans_maier Posted at: 2019-12-09T20:12:41.077Z Reads: 16

```
Ok, I just changed the JST connector from a 5 to a 6 pin leaving out TEMP.

![IMG_7668|375x500](upload://tERvBa6PTX1qf2ownfCAf3j7TMY.jpeg)

![IMG_7669|374x499](upload://u8ih8ekxVn0vqmBtp5XTGJNTk0z.jpeg)

Luckily, I did not have to re-crimp the cables for that. However, after doing so I soon realized that together with the connector the cables will probably not pass through the holes in the enclosure ;-) , unless I make them super-large which I do not intend to ... currently, still waiting for the battery and enclosure to arrive. Thanks again for your help!
```

---
