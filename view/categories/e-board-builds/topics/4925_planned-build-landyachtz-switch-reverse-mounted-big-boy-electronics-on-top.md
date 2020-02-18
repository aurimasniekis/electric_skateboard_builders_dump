# Planned build. Landyachtz Switch. Reverse-mounted Big-Boy. Electronics on top

### Replies: 24 Views: 2831

## \#1 Posted by: Dan Posted at: 2016-06-20T21:27:11.733Z Reads: 299

```
Hi guys. Total noob here. Been reading through the forum for a while trying to learn but would now love some comments and feedback on a mostly Enertion build I’m planning if anyone has a spare few minutes. 

In my head it seems like a good idea to reverse-mount the motor at the back and mount all the electronics/batteries etc on top of the deck in between my feet (I know some of you guys don’t like this idea but I personally do. There’ll still be loads of room for my feet). So here’s what I’m thinking...

Deck: Landyachtz Switch 41.5"

Trucks, wheels and motor: Enertion single motor kit plus (single 6374 Big Boy motor)
http://www.enertionboards.com/diy-electric-skateboard-kits/single-motor-mount-pro-kit-plus/

Batteries. Two of these:
http://www.hobbyking.com/hobbyking/store/__16225__ZIPPY_Flightmax_8000mAh_3S1P_30C.html

VESC:
http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/

Hand-held controller:
http://www.enertionboards.com/electric-skateboard-parts/2-4ghz-radio-hand-controller/

Charger:
http://www.enertionboards.com/electric-skateboard-parts/200-watt-fast-charger/

Questions I’m hoping people can help me with:
1) Have I missed anything?
2) Would these parts come together well?
3) Is it possible/easy to reverse-mount Enertion’s 6374?
4) Would the 6374 Big Boy be enough to drive a heavy deck like the Switch up hills without frying?
5) If I ever decide to get another 6374 and go DD, would that be a total battery-killer?

Additional info: 
- I weigh 160lbs / 73kg
- My town is hilly as hell so torque is more important than speed

Thanks guys, I really appreciate any responses I get!
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-06-20T21:43:57.053Z Reads: 256

```
Maybe better to use 2x4s batteries to get a total of 8s.
The big Brother: http://www.hobbyking.com/hobbyking/store/__16226__ZIPPY_Flightmax_8000mAh_4S1P_30C.html
and as these are LiPos without bms you will need a balance charger.(iMAX B6 will be good for the beginning.)
```

---
## \#3 Posted by: zk8_builder Posted at: 2016-06-20T21:53:58.722Z Reads: 253

```
IMAX b6 is a 6s charger not 8s unless you want to run at 4s
```

---
## \#4 Posted by: Luke Posted at: 2016-06-20T21:54:58.380Z Reads: 251

```
[quote="Dan, post:1, topic:4925"]
Is it possible/easy to reverse-mount Enertion’s 6374
[/quote]

Don't think so since calibers/enerrtion trucks are not symmetrical, would love to be proven wrong though
```

---
## \#5 Posted by: Jinra Posted at: 2016-06-20T23:16:10.636Z Reads: 238

```
You can do it with torqueboards v4 mount, or some other mount that allows for full rotation of the mount. According to @claudiofiore88 you'd have to make sure the center distance is 66+mm or the motor may hit the truck.
```

---
## \#6 Posted by: lox897 Posted at: 2016-06-20T23:31:22.306Z Reads: 219

```
Enertion's mount doesn't reverse mount. @cmatson has modded it though.
```

---
## \#7 Posted by: claudiofiore88 Posted at: 2016-06-20T23:54:42.527Z Reads: 209

```
[quote="Jinra, post:5, topic:4925, full:true"]
You can do it with torqueboards v4 mount, or some other mount that allows for full rotation of the mount. According to @claudiofiore88 you'd have to make sure the center distance is 66+mm or the motor may hit the truck.
[/quote]

Yeah, otherwise you'll hit the kingpin when using 63mm motors. 50mm may work with a 60mm c to c.
```

---
## \#8 Posted by: Jinra Posted at: 2016-06-20T23:55:45.830Z Reads: 185

```
What if you just lower the angle of the motor so the king pin is out of the way?
```

---
## \#9 Posted by: Dan Posted at: 2016-06-21T00:00:47.081Z Reads: 183

```
This might sound crazy (newbie remember) but what if I just flip the whole rear truck backwards? How would that affect the ride?
```

---
## \#10 Posted by: lox897 Posted at: 2016-06-21T00:04:26.951Z Reads: 182

```
Your board would turn in the wrong direction.
```

---
## \#11 Posted by: Dan Posted at: 2016-06-21T00:05:56.272Z Reads: 181

```
Oh. I thought maybe the VESC could be programmed to run the motor in reverse. Man, I still have so much to learn!

Btw thanks for all the responses so far.
```

---
## \#12 Posted by: lox897 Posted at: 2016-06-21T00:08:40.282Z Reads: 185

```
Putting the motor in reverse would just make the board go in the opposite forward/backward direction. The trucks would change left and right.
```

---
## \#13 Posted by: Dan Posted at: 2016-06-21T00:09:33.701Z Reads: 187

```
And front-mounted motors are bad because... your weight is more on the back end so you'd have less traction?
```

---
## \#14 Posted by: lox897 Posted at: 2016-06-21T00:15:56.676Z Reads: 179

```
Wait, why are we talking about front mounted motors now? Yes less traction.
```

---
## \#15 Posted by: Dan Posted at: 2016-06-21T00:34:49.545Z Reads: 183

```
I was just curious as a side-note. 

Ok, so I guess my best bet is to buy a motor mount that can be reversed and just use it with the trucks already on the board. Guess that saves me having to buy the Enertion trucks. I was hoping for as much out-of-the-box stuff as possible because I don't trust my engineering competence, but I guess for that I'd need a different deck.
```

---
## \#16 Posted by: lox897 Posted at: 2016-06-21T00:36:00.082Z Reads: 177

```
Different deck would make it easiest. Enertion motor mount is pretty easy to set up.
```

---
## \#17 Posted by: Dan Posted at: 2016-06-21T00:36:16.982Z Reads: 187

```

Quick question regarding the suggested 4S batteries... two of those would mean 8S and I thought the Enertion 6374 could only handle 7S total?
```

---
## \#18 Posted by: lox897 Posted at: 2016-06-21T00:36:39.070Z Reads: 184

```
Enertion's motors can handle up to 12S.
```

---
## \#19 Posted by: Dan Posted at: 2016-06-21T00:37:08.604Z Reads: 189

```
Sweet. Ok thanks for all the help man, I really appreciate it. I'll go back to the drawing board!
```

---
## \#20 Posted by: Dan Posted at: 2016-06-21T04:35:04.893Z Reads: 182

```
Hey sorry, I just realised I meant 7 cells, not 7S. Can both the Enertion 6374 and the VESC handle 8 cells?
```

---
## \#21 Posted by: ed713 Posted at: 2016-06-21T04:49:58.045Z Reads: 165

```
The S is the cell count. 7S means 7 cells. the motor would work with up to 12 cells. You should be fine.
```

---
## \#22 Posted by: torqueboards Posted at: 2016-06-21T05:13:43.841Z Reads: 185

```
Our motor mounts here product/torqueboards-single-motor-mechanical-kit/ can be mounted in reverse.

Our 6374 motor here but for hills, I'd honestly recommend dual rear motors 6355 or 5055. product/electric-skateboard-motor-6374-230kv/

Also checkout our new enclsoures. We have an ESC enclosure which can house 2x ESCs, on/off switch and some wiring. We also have a separate enclosure for a 2x6s and 2x3s packs. product-category/electric-skateboard-parts/enclosures/

**1) Have I missed anything?**

Your setup isn't plug and play. You would need a soldering iron to finish the wiring off. And/or you can try our 4mm HXT Series Connector + On/Off Switch which work well with Lipo - product-category/electric-skateboard-parts/electrical-connectors

**2) Would these parts come together well?**

Yeah, parts would work except motor mount isn't a reverse mount but it has been done before see #3.

**3) Is it possible/easy to reverse-mount Enertion’s 6374?**

Has been done before. Cmatson has done it.

**4) Would the 6374 Big Boy be enough to drive a heavy deck like the Switch up hills without frying?**

IMO for hills dual motor is always better. Flat ground doesn't matter as much.

**5) If I ever decide to get another 6374 and go DD, would that be a total battery-killer?**

Dual diagonal with 2x 6374 is overkill and too heavy to be enjoyable IMO. I'd rather run a dual 6355 and you can climb 20-30% inclines easily.

If you wanted to save a bit more and don't need heavier duty equipment. You'd be fine with our product/electric-skateboard-motor-5055-280kv-2200w/ which will work great on 6S or 8S and you'd hit 25mph+ and climb 20-30% inclines especially with your rider weight.
```

---
## \#23 Posted by: Mrmoonlight Posted at: 2016-06-21T05:47:14.002Z Reads: 175

```
You can top mount your Switchblade with no issues and you still get a decent drop. I did exactly that with a Switchblade 41.5. Ended up going for the smaller Switchblade. The shorter wheelbase gave me more traction. I'm a little lighter than you. Still have an unused 41.5, but the holes and foam pad are drilled for an E-GO.
```

---
## \#24 Posted by: Dan Posted at: 2016-06-21T15:16:34.764Z Reads: 159

```
Thanks Torqueboards for such a comprehensive response. If this is Dexter btw then sorry for just accidentally closing our chat on the DIY website! 

Ok, back to the drawing board for sure. Thanks everyone for the help.
```

---
