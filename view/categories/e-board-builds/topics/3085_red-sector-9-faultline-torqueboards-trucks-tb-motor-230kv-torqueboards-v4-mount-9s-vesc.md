# Red &#124; Sector 9 Faultline &#124; TorqueBoards Trucks &#124; TB motor 230kv &#124; TorqueBoards V4 mount &#124; 9s &#124; VESC

### Replies: 27 Views: 5073

## \#1 Posted by: mcfly777 Posted at: 2016-05-10T18:20:23.737Z Reads: 518

```
Hello there
Been reading the forum for a while getting some ideas and trying to understand as much as possible. I'm putting my first build together

- Loaded Dervish Sama deck (flex 2) --> Sector 9 Faultline
- TorqueBoards trucks - ordered
- 83mm E-Power wheels - ordered
- 16/36 pulley system, 12 mm belt TorqueBoards - ordered
- Turnigy SK3 245kv --> changed to TB 230kv motor
- TorqueBoards mount V4 - ordered
- 2x Turnigy 5000 mAh 20C batteries - ordered
- VESC from TB

I still have to decide on a controller but I think I'll get the GT2B and print the modded enclosure. A lot of this stuff is backordered so it will take some time for me to get started.

My goal is simple: safety/reliability. Ability to commute 6mi to work (all flat, no hills). Ideally I would not have to charge at work. I also want it to be a clean build.

Things to get worked out:
- design and print an enclosure for electronics
- mount the motor to the back or under the deck
- how to wire the batteries so that charging does not mean having to pull the batteries out

Since it's my first build I'll suspect that some of these choices will change once I have everything running, but it's a start.
```

---
## \#2 Posted by: lox897 Posted at: 2016-05-10T18:27:18.169Z Reads: 467

```
Hey @mcfly777 , welcome to the forum! The GT2B is a good choice. Are you thinking of using the BadWolf 3D printed enclosure or the one that @FLATLINEcustoms is putting on thingiverse? Are you going to run 6S? 5000mah probably isn't enough to get the range to and from your work. Especially if you are running 6s.
```

---
## \#3 Posted by: mcfly777 Posted at: 2016-05-10T18:44:02.596Z Reads: 454

```
Thanks. @lox897 
For the GT2B i'm waiting for @FLATLINEcustoms to put it there. But I can also use the BadWolf one, not sure really one is better than the other, any ideas?

For batteries I am running the 2 batteries in series, so 6S total. I figure it doesn't have enough juice. So I may just pick up another 2 packs but wire it in parallel as I want to start with 6S (slow) before moving to lots of speed. OR, would you suggest wiring it in parallel and just limit the speed?

Leo
```

---
## \#4 Posted by: mohammedex Posted at: 2016-05-10T19:32:01.939Z Reads: 421

```
Well that depends are they 3s or 6s batteries? if you wire 3s in parallel you won't go anywhere because it wont have enough power to push you around. 

I love the Loaded Dervish Sama but the flexibility of the deck might not be very suitable for lipo batteries, they are not very flexiproof.

I imagine that if you have a flex 2 deck you probably weigh around 70-80 kg like me. I can go 8.5-10miles on a charge. Hope this helps
```

---
## \#5 Posted by: Ulfberht Posted at: 2016-05-10T20:14:35.577Z Reads: 411

```
[quote="mcfly777, post:3, topic:3085"]
So I may just pick up another 2 packs but wire it in parallel as I want to start with 6S (slow) before moving to lots of speed. OR, would you suggest wiring it in parallel and just limit the speed?
[/quote]

Keep in mind, my friend, that the higher the pack voltage the fewer amps the motors will draw and less heat will build up in your system. 6s is good, but 10s is better suited to your application. 
SInce you are using the SK3 running @245kv with a VESC. There is a formula. 
Here's a cool link from Benjamin Vedder to help out with selection:
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
My favorite calculator for running virtual rigs:
http://toddy616.blogspot.de/2013/07/electric-skateboard-calculator.html
```

---
## \#6 Posted by: lox897 Posted at: 2016-05-10T21:48:19.819Z Reads: 365

```
I think @FLATLINEcustoms one is going to much better and easier to use. I am not sure how long it will take him to finish it though. I would get two 6s 5000mah (more mah if you want) and put them in series. That would give you the range you want.
```

---
## \#7 Posted by: mcfly777 Posted at: 2016-05-10T21:48:47.615Z Reads: 366

```
Thanks both. I canceled the 3s batteries. Looking into 4s. But essentially looks like the only game in town is hobbyking? Not to mention lots of stuff is backordered. Not sure when I'll be able to get my hands on the 245kv motor. Was thinking of getting the 149kv that is available now but that means I'd have to go to 12s....
```

---
## \#8 Posted by: willpark16 Posted at: 2016-05-10T23:53:50.963Z Reads: 358

```
u could use 10s with it
```

---
## \#9 Posted by: mcfly777 Posted at: 2016-05-11T15:09:54.258Z Reads: 363

```
Found a 230kv from TB so will use that instead. Will go for 10s.

Leo
```

---
## \#10 Posted by: mcfly777 Posted at: 2016-05-17T15:13:10.259Z Reads: 380

```
Designed and printed a small battery case. This is a prototype, printed in ABS. Fits nicely but want to improve on a few things.

<img src="/uploads/db1493/original/2X/5/5e841f1f1f47b222309a4a36e38d177d4737a9ba.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/c/c2d5929c4c993f6bff20cc0dd8aeccf2ff2698b9.jpg" width="375" height="500">

Also bought a Sector 9 Faultline board, got a great deal. 9-Ply maple, 40". Should be solid enough for minimal flex.
```

---
## \#11 Posted by: mcfly777 Posted at: 2016-05-30T19:49:50.475Z Reads: 362

```
Designed a prototype 3d-printed enclosure. Also drilled the deck and countersunk some T-nuts so that when I apply grip-tape it is not visible.

For the enclosure, to-do:
- switch to black socket screws
- create countersunk screw holes every 50 mm
- increase height of deck (+ 15mm)

Mechanical and electrical parts still on order @torqueboards

<img src="/uploads/db1493/original/2X/c/cdae69fd5943b75924fe760a283422b4a443c36a.jpg" width="666" height="500"> 

<img src="/uploads/db1493/original/2X/2/24ae892007402ee284071bd2df59f1522f39b9ad.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/3/345fe376179f66b3b40b7f7c04650cf7cb51beaf.jpg" width="666" height="500">
```

---
## \#12 Posted by: torqueboards Posted at: 2016-05-31T19:41:10.218Z Reads: 344

```
Sweet setup. How's the enclosure holding up?
```

---
## \#13 Posted by: mcfly777 Posted at: 2016-05-31T19:57:01.400Z Reads: 337

```
We'll see when I get the parts coming from you :)
```

---
## \#14 Posted by: Pablo_702 Posted at: 2016-06-25T23:30:08.431Z Reads: 310

```
man those cut outs for the connections are so sick!!!!
```

---
## \#15 Posted by: Ulfberht Posted at: 2016-06-26T03:04:28.229Z Reads: 311

```
@mcfly777 I like that enclosure a lot. The 3d printed part just puts that finishing touch on it. Have you considered using threaded inserts instead of bolting the box through the deck? These little suckers are pretty cheap, but leave a really clean look. They are super easy to install too. Check em' out. 
<img src="/uploads/db1493/original/2X/8/8460e012fc1d394c2f0e184cc60861f985bb613e.png" width="379" height="500">
```

---
## \#16 Posted by: mcfly777 Posted at: 2016-06-26T17:28:09.000Z Reads: 293

```
Yes I was going to use those. But the length of these would still make me drill through the board, and I read somewhere that the outside threads can slowly become loose. So I opted to use the T-nuts instead, which will be covered by the griptape, so the end result is the same: a machine screw thread without anything visible from the top.
```

---
## \#17 Posted by: mcfly777 Posted at: 2016-07-10T14:28:26.719Z Reads: 286

```
It lives! Got my parts this week from @torqueboards and it's a thing of beauty. I need to work on the enclosure now (printing), and also decide how I will handle all the wires. Functionally, the acceleration is very smooth, as well as the braking. Have to adjust the turning as well, it doesn't turn as tightly as I'd like it to. 
 
More to come.
```

---
## \#18 Posted by: mcfly777 Posted at: 2016-07-13T17:55:26.721Z Reads: 301

```
Another update. Enclosure is mounted, fits the batteries and the VESC. Very solid.

To-do
- hide the motor wires. I'll route a groove on top of the deck, LHB style. Then I can hide the groove under griptape
- improve the look of the enclosure. The enclosure works ok but I don't like the texture of the material, it doesn't look very good. I'm thinking of plastidipping it so that it looks matte black.
- install the voltmeter where it should be (right now the motor wires are coming through that hole)
- install a bluetooth module on the VESC UART so I can collect data. Alternatively I could use an [open log board](https://github.com/sparkfun/OpenLog) which I have already. Trouble is the programming part that I don't understand well enough yet.
- get an extension for the balance charge cable so that it can come out at the end of the enclosure where it was supposed to be

Pics
<img src="/uploads/db1493/original/2X/4/4ce2b0317e5e6b5eef7f0e92f1fe812547425e90.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/d/d1ff23a6179d9fb762726f51598b1eef7542b8a2.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/a/a565eb3a335f17e14170327baed26a078ffd920c.jpg" width="666" height="500">
```

---
## \#19 Posted by: mcfly777 Posted at: 2016-07-17T14:58:05.094Z Reads: 293

```
Routed the groove on top of the deck to hide the motor wiring. 

<img src="/uploads/db1493/original/2X/8/884400312823e8769e296c5da2fb280593f80533.jpg" width="666" height="500">
```

---
## \#20 Posted by: torqueboards Posted at: 2016-07-17T18:08:25.165Z Reads: 281

```
Nice routed wires :)
```

---
## \#21 Posted by: mcfly777 Posted at: 2016-07-27T22:00:21.373Z Reads: 278

```
Still moving forward. 
- The 3D printed enclosure works, however I have to print multiple pieces (4) to make the enclosure, and it doesn't look that good. So I built a vacuum forming table and just this morning bought some ABS sheets. The mold is ready. I plan to try vacuum forming later today.
- The VESC (from @torqueboards) continues to go strong. I raised the default motor amperage to 50, and it works really well. I have connected an ESP8266 to the UART port to connect to it via wifi and without having to remove the enclosure, however I can't connect to it yet. No answers from the VESC forum either...not sure when this will work.
- I designed and printed a piece to protect the motor from small rocks/dust/sand. I unfortunately got one dimension wrong so I had to melt it a bit to fit...still it works but I'll print one with the right dimensions
- Ordered 1 more 3s battery to make a 9s system. It will fit just fine in my new enclosure.
- Need to make the routed wires be flush with the top of the deck, then apply grip tape to make it stealth...maybe I'll need to retouch the routed channel so that there's nothing bulging up.
- Haven't tried FOC but it's tempting!

Lot's of work ahead!

Leo
```

---
## \#22 Posted by: mcfly777 Posted at: 2016-07-31T03:37:40.367Z Reads: 268

```
Vacuum forming was not easy, I designed an enclosure with 2 parts (split), and I got both parts done...one melted more than i wanted and the texture is not the same, but it works.

Also I widened the top groove for the motor wiring so that all 3 would fit side by side, filled it with hot glue, and put some grip tape on it. The top now looks good.

Now that I have the bigger enclosure, I can fit up to 4 batteries. I only have to decide if I'll go 9s or 12s, and the wiring so that I can discharge and charge it without much trouble.

Photos of the top and the enclosure sitting on the bottom (not installed yet)

<img src="/uploads/db1493/original/2X/a/aa84e7e246a40410a2fc8cae650efe5d369896d5.jpg" width="666" height="500">

<img src="/uploads/db1493/original/2X/0/05768122f6d2c0e54be412c985f819fe3aed7eaa.jpg" width="666" height="500">
```

---
## \#23 Posted by: mcfly777 Posted at: 2016-07-31T18:13:01.282Z Reads: 245

```
Upgraded to 9S this morning. This thing flies. Experienced 1 soft cut-off, not sure why. Parameters:

Batt Max 50A
Batt cutoff start 32.4V
Batt cutoff end 31.5V
Max ERPM 70,000

From my calculations max ERPM at this voltage would be around 45k so that can't be....

Leo
```

---
## \#24 Posted by: mcfly777 Posted at: 2016-08-02T21:00:08.097Z Reads: 242

```
I don't like the ABS vacuum formed enclosure. Just doesn't look very professional in my hands. Plus I have all these cables that need to be exposed in addition to the key so I can charge it without having to remove the enclosure.

So back to the 3D printed enclosure plan. I was using it before and it worked well, and it's all modular, built in 10 cm sections. I upgraded the design a bit, moved the ports to the side, rounded the edges some more and made the screw slots flush with the surface. Next is figuring out what I can do to make a smooth surface. 

If I want to leave just the key slot out and a charging port out, might need to get a BMS.

<img src="/uploads/db1493/original/2X/e/e3f0470099d9a88cf027ea27f0ce14edca3c1899.png" width="690" height="456">
```

---
## \#25 Posted by: Deathjunior Posted at: 2016-09-07T16:22:13.735Z Reads: 203

```
See I've thought about printing my enclosure as well my worry wont be delam though since my printer runs a heated bed. It's getting the curvature of the board exactly right. Also I'm sure I'd wind up fusing it together with CA glue and acetone and then I'm still not sure just how well it'll handle being bolted to the deck. To the point that I'm heavily looking into vacuum forming. I'll decide once my space pack shows up but I'm probably going with forming due the the complex shape around the dual VESC.
```

---
## \#26 Posted by: mcfly777 Posted at: 2016-09-07T16:54:25.126Z Reads: 206

```
A couple of updates
- I used T nuts to secure the enclosure for half the board, and as I expanded the enclosure I used wood inserts. One came off (despite being glued with epoxy in the hole), and 3 stripped the internal thread. So no more wood inserts for me.
- As I recessed the torx screws into the enclosure, the base of the enclosure got too thin, and since that is what is holding the enclosure to the deck, those areas broke. So now I have dome-shaped screws with nuts. 
- A 3rd and most annoying (and dangerous) issue is that when I switch off my remote, after a few seconds the motor will go full speed. A friend of mine got my board and caused an accident (board ran into the wheel of a car, thankfully not a person). I think it's due to the default VESC settings for timeout, I will update the brake force to be applied to 0 amps. My current setting has no reverse, so it's not that the signal from the remote goes to 0 and that is reverse. 
- I continue to be very happy with @torqueboards motor, VESC and mechanical parts
- I achieved good balance between stability and turning radius, it took a few tries but I love this board.

Leo
```

---
## \#27 Posted by: noazark Posted at: 2017-02-19T04:23:58.167Z Reads: 142

```
How do you like your sector 9 faultline? Debating between that and a loaded tesseract or vanguard
```

---
