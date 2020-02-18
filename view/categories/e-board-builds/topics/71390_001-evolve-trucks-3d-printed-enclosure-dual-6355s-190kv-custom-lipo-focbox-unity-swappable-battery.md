# #001 &#124; Evolve trucks &#124; 3D printed enclosure &#124; Dual 6355s 190kv &#124; Custom lipo &#124; Focbox unity &#124; swappable battery

### Replies: 43 Views: 1992

## \#1 Posted by: Sinned800 Posted at: 2018-10-16T08:51:48.179Z Reads: 380

```


Hi Guys,

After a while reading and gathering information I’m going to start my build thread. What keeping me busy was finishing my workshop after we moved into our new flat so within this weekend it should be mostly completed and I can focus on my build.

**Main focus for my build:**

* Use standard parts
* Make it easy to assemble
* Really clean build without loose or hanging cables
* Safe
* Easy to maintain

**CAD:**

I was developing heavily with catia in my previous job and now in private swapped over to fusion 360 with this build and I love this cad program.

**Battery:**

5 Graphene battery’s with 2S 90C discharge in series with 4600mah are going to power this little fella.

All in a swappable battery to enlarge my range or make it accessible for transportation. So for the start with one battery and try to build it up as easy as I can to enlarge my set up afterwards. With a travel save battery and long range battery etc.

* Bypass bms from bestech
* Pcb internal connection (no or at least almost no cables)
* Laptop style charger with Arduino and an e ink display for my curiosity of the cell values.

**Enclosure:**

The enclosure is sitting flat on the board because I really hate all the gasket screwing directly to the board. So it is going to have some nice revision cover with plastic screws and thin silicon seals.

**Deck:**

DB Freeride 38&quot; very similar in shape to the Evolve

**Truck &amp; Wheels &amp; Mounts:**

Evolve Trucks with Evolve AT Wheel set &amp; Unik Board CNC milled aluminum holder

**Motors:**

I think im going with dual eskating 190kv motors 6355

**ESC:**

Pro ordered the Unity

For now. I ordered most of the parts except the motors, pulley, remote and some little stuff. I’m going to make my design open source if someone of you want to copy my swappable battery system afterwards feel free to use it (just started and not released yet)

I really appreciated the effort all of you have been putting into this platform and hope I can give something back with my cad skills and get a bit help from you designing my pcbs.

Cheers, Dennis

![Longboard%20v8detail2|625x500](upload://tKFzIR6ofV03sg316IQs4P5L1sg.jpeg) ![Longboard%20v8detail1|625x500](upload://6j7bVtRyn6VdkTsRtluuITuzRGd.jpeg) ![Longboard%20v8ohnebat|625x500](upload://v35f14Wt3OklV2y8QmuE8SUoANu.jpeg) ![Longboard%20v8|625x500](upload://jz9ZHFlJflIGa8wXEmKrvG7LZkM.png) 

![longboard|690x220](upload://xxu8PqzprdOVOUiBp0MTuF1Bwyi.png) 

![IMG_20180918_201626|666x500](upload://hFtIrHDMUnbQrD1lvGGkKswo74.jpeg) ![IMG_20180913_081154|375x500](upload://wN0tgOjMZAXxun1lrdAmvqdvAfw.jpeg) ![IMG_20181006_114501|666x500](upload://xyE8VEuTM9n1jIlITCSEp7wG9OI.jpeg)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-16T09:29:54.291Z Reads: 340

```
looks great! how does the flex on that board work with 3d printed enclosure?
```

---
## \#3 Posted by: Sinned800 Posted at: 2018-10-16T09:37:54.903Z Reads: 340

```
as far as i could test it: juming on my board :sweat_smile: it is quite stiff. All the parts inside the enclosure are only held to it and not directly to the board so any bend and wiggle shouldnt effect the parts inside the housing due to 3mm print thickness.
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2018-10-16T12:45:19.687Z Reads: 324

```
That tool wall......this looks really nice man ☺
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-10-16T13:03:21.507Z Reads: 323

```
Nice one, I’m curious how you will measure the cell voltages with the arduino, I couldn’t find a way without putting a bunch of transistors to turn off the voltage dividers so it wouldn’t unbalance the pack
```

---
## \#6 Posted by: Sinned800 Posted at: 2018-10-16T13:14:56.723Z Reads: 307

```
Thanks.

Im going to make it only while charging and then all cells at the same time (probably non permanent just to check and satisfy my curiosity)  

Taking the single cells to ground creating an voltage divider with same resitor to unload the cells equal was my plan.
```

---
## \#7 Posted by: Pedrodemio Posted at: 2018-10-16T14:59:44.871Z Reads: 291

```
And you will make it turn on when you connect the charger? I would really like that, I have 5 leds boosted style on my board to show charge level, but they only work with the board powered on, couldn’t find a way to power only the arduino when charging
```

---
## \#8 Posted by: Sinned800 Posted at: 2018-10-16T18:33:10.013Z Reads: 276

```
yes just when charging up the battery. but let me get further into design and then i will come back with a clear picture. fist things first now and thats fitting everything into that enclosure
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-10-16T18:46:56.967Z Reads: 278

```
No hurry, my problem with the “I will first get it running and then do that” is that I never come back to do “that” :upside_down_face:
```

---
## \#10 Posted by: Sinned800 Posted at: 2018-10-17T08:20:30.801Z Reads: 294

```
got further into design. finished the bottom side of the battery housing with all the cable management, bms holder, xt90 socket and the locking mechanism. <-- super proud of this. hopfully it works in the end![bathousing|625x500](upload://lOVp4z2vvJ557RWoNcaNBAwVhcr.jpeg) ![locking|625x500](upload://7UMOtcR2TDNGUqLSBKBvlyjboxa.png) ![locking%202|625x500](upload://fG3I77PK7tnKFBZHcGJSmEQ3Ddi.jpeg)
```

---
## \#11 Posted by: Sinned800 Posted at: 2018-10-20T07:11:35.851Z Reads: 278

```
Enclosure is almost Done:

Things to do when i get my unity ( cable management; cable feed through)

As a start i am printing the battery and test the fit (assembly etc)
test print the enclosure and locking system V1 to test the board fit and locking system.

As you can see in the details i got a Labyrinth to ensure sealing and screws are not metric they are plastic self cutting

Enlcosure height is about 33 mm from deck to the top
:star_struck:


![CAPS|625x500](upload://1JcNuHeyRC3cZamQY3OqQQw49x5.jpeg) ![Body%204|625x500](upload://lmt5GVusyThdf6NtsWBjU9QHjsz.jpeg) ![Body6|625x500](upload://nY3UOzXmPJgDqPwF7xRDxfxNrYP.jpeg) ![BAT|625x500](upload://hiAqTLTXljr3kyYIwBUY1HZ1j56.jpeg) ![Body%207|625x500](upload://iDBd4OK1WtBKnwbpBYzKmcPCrIx.jpeg) ![Body%203|625x500](upload://4xrL2AMShu9c8THFHCNie58TA4x.jpeg) ![lock|625x500](upload://l46pZwKwHGpSueImcHYm2J2TcAL.jpeg) ![body%20deck|625x500](upload://7zqPhHlINoHm7hYxLEnGSYpLiUO.jpeg) ![Body%202|625x500](upload://tYNIEC4BFBTCN3PvP4bbKnlpuwk.jpeg) ![Body|625x500](upload://lYhfQ8lNwjcGqHCcxJpuAtl1hSM.jpeg) ![Body%201|625x500](upload://8YbyoemioqRLL8RtttJZqMxLmiv.jpeg)
```

---
## \#12 Posted by: AreaKruzer Posted at: 2018-10-20T07:25:38.251Z Reads: 236

```
Looks hella professional
```

---
## \#13 Posted by: AreaKruzer Posted at: 2018-10-20T07:31:18.032Z Reads: 233

```
Just to check, what is the blue button for?
```

---
## \#14 Posted by: pat.speed Posted at: 2018-10-20T07:32:11.174Z Reads: 240

```
Release button maybe?
```

---
## \#15 Posted by: Sinned800 Posted at: 2018-10-20T07:34:25.316Z Reads: 240

```
its the Clamp/release for the swappable battery
```

---
## \#16 Posted by: Sinned800 Posted at: 2018-10-20T14:06:24.690Z Reads: 242

```
35 hours to go .. just for the battery body 
https://photos.app.goo.gl/U5FCqzN2o9CtGPvr9
```

---
## \#17 Posted by: AreaKruzer Posted at: 2018-10-20T14:43:28.475Z Reads: 234

```
What's the dimensions for your enclosure?
```

---
## \#18 Posted by: Sinned800 Posted at: 2018-10-20T15:21:53.677Z Reads: 226

```
The battery itself is about 300x135x33 mm and the whole enclosure is about 450x195x33 mm
```

---
## \#19 Posted by: Pedrodemio Posted at: 2018-10-22T12:54:55.558Z Reads: 229

```
Loved the designed, really looking forward to how the printed parts hold up

You essentially end up with unlimited range, you could even go smaller with the battery’s, 10S with the Samsung 30T would be dope
```

---
## \#20 Posted by: Sinned800 Posted at: 2018-10-23T09:52:25.626Z Reads: 235

```
quick update... print failed after 28 of 35 hours due to edge warping of bed on the croners :( but fortunatly my new larger printer comes on wendsday and with this one im able to print every part in one shot without going this close to the edge of my build volume

![](https://i.all3dp.com/wp-content/uploads/2018/05/26142256/Anycubic-Chiron-3D-Printer-e1531313708594-1284x723.png) :heart:
```

---
## \#21 Posted by: mikenyc Posted at: 2018-10-26T13:13:02.715Z Reads: 224

```
do the batteries slide out or something? do you need to remove the screws to replace them?
```

---
## \#22 Posted by: Pedrodemio Posted at: 2018-10-26T15:22:48.625Z Reads: 212

```
Best thing you can do for warping is use a large brim and enclose the printer somehow, heat everything and let it sit for half an hour and only then start printing
```

---
## \#23 Posted by: Sinned800 Posted at: 2018-10-26T23:38:46.322Z Reads: 210

```
if you want to change the whole battery you just have to press the blue release button and access the battery. if you want to excahnge single cells of course you have to unscrew the battery to get access to the single lipos
```

---
## \#24 Posted by: Sinned800 Posted at: 2018-10-26T23:39:26.263Z Reads: 204

```
the trend goes to a third 3d printer :sweat_smile:
```

---
## \#25 Posted by: mikenyc Posted at: 2018-10-27T00:17:45.359Z Reads: 210

```
Does that mean it (the battery) slides out all in one piece?
```

---
## \#26 Posted by: AreaKruzer Posted at: 2018-10-27T05:24:38.046Z Reads: 214

```
Yes. The blue button releases the entire battery in 1 piece.
```

---
## \#27 Posted by: Sinned800 Posted at: 2018-10-31T09:23:56.398Z Reads: 218

```
a bit of progress... battery body is done and the fit is snug and good so far. i have to change a few things in my actual 3d designand reprint the part because ocd...

* cable management holder are to tiny so the bms cables cant fit through properly
* bms snap holder are to tight <-- rethink the concepts 
* bit more gap for the batterys to handle the swelling and as well for the xt90 connectors
* thicken up the locking mechanism

Pros: petg print came out super sturdy and pretty with only a bit of oozing and 

![IMG_20181030_172503|666x500](upload://3VSEslnVr3Yi1IPtSWYAODAChJx.jpeg)
```

---
## \#28 Posted by: totalgeek9224 Posted at: 2018-11-02T10:14:40.000Z Reads: 213

```
Really enjoying this project! Keep us updated!!!
```

---
## \#29 Posted by: Sinned800 Posted at: 2018-11-07T21:11:36.594Z Reads: 209

```
Updates updates updates

Reprinted the body with the updates now everything fits nicely. Right now the counter part cap is on the printer. (Should be done within next 20hrs)

Printed everything with clear filament due the fact that I ran out of different colors and thought never mind I paint it anyway but now as a see the lipos and cable shine through that translucent body... Gorgeous...![IMG_20181107_204051-01|666x500](upload://qw5wibpCYLdPSyBTYdKqXMBIjWM.jpeg)
```

---
## \#30 Posted by: Sinned800 Posted at: 2018-11-07T21:12:06.951Z Reads: 210

```
![IMG_20181107_204057-01|666x500](upload://9hT0XCDQKu6Y3mwYZz2bfNgNEs0.jpeg)
```

---
## \#31 Posted by: dg798 Posted at: 2018-11-08T00:17:36.320Z Reads: 204

```
this is one of the coolest battery designs i have ever seen.
keep up the great work
```

---
## \#32 Posted by: totalgeek9224 Posted at: 2018-11-08T12:26:23.256Z Reads: 186

```
Firstly, what an awesome design,
Just a lil question, in the CAD design, im not seeing a cutout for the charge port on the main housing (where the ESC's are), which might(?) be an issue seeing the couple of mm the charge port sticks out on the battery mockup, is this fixed now?
```

---
## \#33 Posted by: trancejunkiexxl Posted at: 2018-11-09T02:12:32.433Z Reads: 171

```
What printer did you end up getting 😃
```

---
## \#34 Posted by: topcloud Posted at: 2018-11-09T02:23:52.640Z Reads: 176

```
[quote="Sinned800, post:1, topic:71390"]
I really appreciated the effort all of you have been putting into this platform and hope I can give something back with my cad skills and get a bit help from you designing my pcbs.

Cheers, Dennis
[/quote]

https://media1.tenor.com/images/0d940e6e8d13004bfb633985ff68c9b0/tenor.gif?itemid=10761610
```

---
## \#35 Posted by: Sinned800 Posted at: 2018-11-09T07:31:34.424Z Reads: 168

```
in the picture the chargout isnt fully put in the housing.. its sitting flush with the battery housing, when assembled propperly  :sweat_smile:
```

---
## \#36 Posted by: Sinned800 Posted at: 2018-11-09T07:33:26.721Z Reads: 169

```
Got the Anycubic Chiron. Huge platform, good heat bed and the overall print quality is decent.
```

---
## \#37 Posted by: Sinned800 Posted at: 2018-11-27T12:24:49.751Z Reads: 151

```
Late reply...had to go on several work trips and had a bad back inquiry within the last weeks so everything slows now down a bit but still made some progress beside back pain and pain killer :laughing:

V1 battery cap was now printed and assembled. Sanded the prints a bit but now everything aligns perfectly. Overall print quality of the cap isn’t perfect so i made some changes on my printer the get rid of these issues.

**NOW what’s next:** V3 body and cap are right now on the way including changes from v2/3 + 3d printer upgrades. I started to assembly the internals to V1/2 and everything and it fits quite nicely so you could say the battery comes together like a charm. When the new hosuing then is finished id just have to be swapped to V3. 
For everything else….Still waiting for my Unity. That would be the next step getting foc in hand and finish the housing design but until now nothings here and project is stopping.... Mechanical assembly of the board, motors, trucks etc. is done. So far.


https://photos.app.goo.gl/xVfo6EvzhKeAXZmg8
https://photos.app.goo.gl/4cWVuU9mHh9XdP5o9
```

---
## \#38 Posted by: totalgeek9224 Posted at: 2018-12-18T22:02:20.686Z Reads: 132

```
Any updates? :D
```

---
## \#39 Posted by: Sinned800 Posted at: 2018-12-24T18:14:24.708Z Reads: 129

```
Sorry no updates lately being hospitalised since one week now :( couldnt convince my wife to run an 3d print :smiley:
```

---
## \#40 Posted by: totalgeek9224 Posted at: 2018-12-24T18:15:37.425Z Reads: 129

```
No shit! Man take care of yourself! And i look forward to more progress, but hey, focus on you!
Happy holidays!
```

---
## \#41 Posted by: totalgeek9224 Posted at: 2019-03-12T10:36:11.905Z Reads: 93

```
So how you been feeling? :p
```

---
## \#42 Posted by: practicalprojects Posted at: 2019-03-12T19:51:29.081Z Reads: 85

```
fantastic work so far!
```

---
## \#43 Posted by: Sinned800 Posted at: 2019-03-27T14:06:53.078Z Reads: 71

```
hey chaps. im fine so far... after being hospitalised for 2 weeks under medical observation it was clear that my broken spine cant be fixed without surgery. so long story short the opend up my back and tied everythin back together. Now im home since jan and stricktly instructed to lay flat and stay in bed or sofa....

but good news my design has now a few new features :slight_smile: and i am being completly fine without any long terms..

Stay safe guys wear a helmet. and thanks for your participation.
```

---
