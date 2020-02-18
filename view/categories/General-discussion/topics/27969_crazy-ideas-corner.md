# Crazy ideas corner

### Replies: 31 Views: 1992

## \#1 Posted by: jotatsu Posted at: 2017-07-18T18:22:05.444Z Reads: 277

```
Well i haven't finished my first build, but here are some ideas that i've while doing it:

- Pressure sensitive dead man switch: Something between the trucks and the table that senses if there is weight in the table (up to certain number of force), if there is none, cut the power afters x seconds.

- ADAS: control independently the torque in dual drives, help with turning and i think with an accelerometer and some reinforce behavior learning it can nullify speed wobbles

- Cruising disconnect: Just power down one motor in cruise mode to help save battery, dunno how much it can help.

- Autonomus driving. I think a gps, lidar module and a lot of computer power. Totally useless , but cool none the less. 

Share your crazy ideas if you have. :D
```

---
## \#2 Posted by: Martinsp Posted at: 2017-07-18T18:26:53.408Z Reads: 272

```
The pressure sensing was done by one guy... He made a video about it.. his channel is great scott just search for it and he has the video somewhere :D that is actually not so crazy..

the autonomous driving is crazy! :D
```

---
## \#3 Posted by: lock Posted at: 2017-07-19T02:54:12.216Z Reads: 237

```
Trucks to have standardised interface for attaching motor mounts. Just a few bolt holes, nothing too fancy. Although it obviously works, the current solution of using grub screws/etc seems like a bit of a hack. It also doesn't seem to work if you need good alignment as you would for gear based drives.

Suspension. Currently thinking about a 'street' version of a BajaBoard, just needs to be half the weight and cost.

Bevel gears and mounting the motor(s) vertically. Not quite sure why (for science?!), may free up some packaging space behind the truck for that suspension system ;-).

Differential system. Some potential to save money/weight by using only one motor and speed controller, but then I can't see you coming out ahead considering the work that'd need to go into the drivetrain.

As mentioned above, some form of stability control. Seems like a bit of a waste having two independently controlled motors and not doing something like this; developing and testing 😬 could be a bit of work.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-19T03:22:34.387Z Reads: 217

```
Autonomous control of RC vehicles is fun to mess around with but don't think I'd trust it enough to stand on it.  Main problem with that one too is the steering is only based on tilt, throw a servo on there to turn the trucks and it could work just like a big ol' RC car but again I wouldn't try standing on it at that point.  I built a few little autonomous vehicles, I used a pair of small geared tread hobby kits (like $20 a piece) an arduino and a servo to sweep a ultrasound left and right and would just dodge left if it saw something to the right and left if it saw something to the right.  Tried upgrading to a Traxxas as the platform to drive around but the batteries I had were crap and I didn't understand all this stuff well enough to know how to deal with pumping up the capacity (which I now know just means more cells in parallel) and with low capacity only had about 10-15 minutes of intense autonomous crashing into things since it couldn't read the ultrasound sensors and decide what to do before it would run into all sorts of things.

Love great scott too, lots of good content and info.

Dead-man switch seems like a good idea, would probably want it independent of the ESC or whatever too though and seems there is mixed reliability issues with the switches used for batteries (perhaps a small robot who's only purpose is to pull the loop-key).

https://www.youtube.com/watch?v=3ht-ZyJOV2k
```

---
## \#5 Posted by: thisguyhere Posted at: 2017-07-19T04:32:45.734Z Reads: 189

```
[quote="lock, post:3, topic:27969"]
Differential system
[/quote]

I'd love to explore this idea but I don't have the tools or skills to even start a concept. And in some crazy world even a two gear transmission.

So with a differential there could be one giant longitudinally mounted motor.

Also a "come here" functionality where the board would know where u are and drive itself to you. This would require gps in the remote and some steering capability, maybe through torque vectoring with dual drive.
```

---
## \#6 Posted by: treenutter Posted at: 2017-07-19T04:38:45.181Z Reads: 176

```
Bushings made of a polymer that can provide variable durometers based on an electrical signal. Soft bushing mode at low speeds, duro increases as speed increases. Kill the wobble but still have a carvy ride at low speed.
```

---
## \#7 Posted by: lock Posted at: 2017-07-19T04:52:50.480Z Reads: 168

```
Probably worth checking out [this thread](http://www.electric-skateboard.builders/t/open-differential-electric-skateboard-single-motor-dual-rear/19814). Hard to see how you'd make something similar without access to at least a CNC, and probably lathe. I don't have the skills either, but that wouldn't stop me from trying.
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-07-19T05:03:01.395Z Reads: 169

```
Holy shit that's exactly, or pretty close, to what I had in mind.
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-07-19T05:15:06.523Z Reads: 161

```
Ive been kinda thinking about some sort of inline Super Capacitor bank for absorbing excess regenerative braking current to prolong LiPo battery life. I have some ideas on how id do it though I personally have no use for something like this as there are practically zero hills were I live (Illinois) though for someone in say SF, then yes definitely lol. Also as I was talking to some peeps about in a dif thread water cooling your board would be awesome, VESC Motor etc. Also this ones kinda dumb but I think it would look really cool is a Nixie Tube battery monitor.
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-19T05:19:40.826Z Reads: 158

```
https://en.m.wikipedia.org/wiki/Electrorheological_fluid?wprov=sfla1

Apparently need to brush up on my use of nano particles and find someone who isn't afraid of 3kV and we're in business :)
```

---
## \#11 Posted by: JdogAwesome Posted at: 2017-07-19T05:29:51.274Z Reads: 149

```
I mean get yourself a MOT and your in business!
```

---
## \#12 Posted by: JdogAwesome Posted at: 2017-07-19T05:34:23.965Z Reads: 148

```
Oh and also some sort of CO2 Fire Suppression System! You could use like a 12g CO2 cartridge and have it just puncture a hole in the tip and vent into the enclosure if it detects to much heat or smoke. I know there are little smoke detector modules for Arduinos or something on eBay.
```

---
## \#13 Posted by: Sander Posted at: 2017-07-19T23:15:06.126Z Reads: 124

```
On my board I will create the power saver mode with turning off one of the VESC digital over my remote.
```

---
## \#14 Posted by: wafflejock Posted at: 2017-07-20T02:19:59.640Z Reads: 127

```
Yeah easy to detect the heat with thermistors might be harder to detect smoke with all that wind rushing by.  For fire suppression think with Lithium fires best bet is actually using sand bags to cover the battery and get it to quickly exhaust it's oxygen supply so it doesn't keep burning (gravity will pose a problem here), haven't done any testing or anything but from what I gather the fire extinguishers usually can't completely extinguish them and they end up re-igniting

http://venturaaerospace.com/news/suppressing-lithium-ion-battery-fires/

http://www.safelincs-forum.co.uk/topic/1572-what-extinguisher-for-lithium-batteries/

I suppose you could wrap your batteries in a sufficient amount of sand bags to contain the fire better but without some sort of powder covering it I think the stuff kind of just keeps on going (like the energizer bunny)
```

---
## \#15 Posted by: wafflejock Posted at: 2017-07-20T02:21:43.601Z Reads: 132

```
Pretty sure we discussed this in another thread reducing the number of motors doing the work is actually likely less efficient and also someone noted the power turning the "idle" motor is still going to be going into the coils and burning up in the mosfets if you aren't putting it back into the battery (at which point you're braking while trying to go forwards which is never really going to work out, no over-unity and all)

---

If you have 1000W going to two motors you have 500W going to each one.  If you are at 42V lets say then that's 500W/42V ~= 12A to each motor, power loss in the electrical components has a square relationship with this current I^2*R (everything before the energy is being used in the coils to move the rotor).  If instead you deliver the same 1000W through a single motor the current through that speed controller and motor is double 24A (same current through the lines from the batteries but double the current through the single speed controller and motor to get the same power as two motors).

Beyond electrical efficiency you are putting less strain on each belt and the rest of the drive assembly and have more gripping friction with the two motors pushing... would be good to get some real world results to verify this but all makes sense in my head :slight_smile:
```

---
## \#16 Posted by: JdogAwesome Posted at: 2017-07-20T04:36:21.322Z Reads: 121

```
Inside the enclosure there isnt any moving air usually and I was thinking more an electrical fire from a shorted wire or whatever. And LiPo's will obviously keep heating and venting electrolyte even with a CO2 suppression system, though the ideas is to hopefully keep the vapors from igniting which is a lot worse than the vapors themself, at least to the board physically.
```

---
## \#17 Posted by: wafflejock Posted at: 2017-07-20T04:41:39.250Z Reads: 117

```
Eh mine is drafty you must have a tight box (twhs).  Either way though just saying detecting heat is typically simpler than detecting changes in the air.  Also with shorts in wires usually from my experience the wire pretty much instantly vaporizes anyhow so time it has to transfer the energy to light other stuff on fire is relatively small, once the cells go up think that's when you have real problems.
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-07-20T04:44:07.368Z Reads: 123

```
Yeah definitely with the amperage LiPo's provide wires do often vaporize. And yeah when your cells vent, then you have a real problem lol.
```

---
## \#19 Posted by: tueboard Posted at: 2017-07-20T09:03:57.056Z Reads: 114

```
i found this video about "Pressure sensitive dead man switch"
https://www.youtube.com/watch?v=e_ktwKirD5o

i like the idea of Cruising disconnect to save power.
```

---
## \#20 Posted by: swashplate Posted at: 2017-07-20T11:35:01.334Z Reads: 102

```
What about attaching batteries and other electronics at top of drop through decks? Like loaded tan tien you have a lot of space for your foot. And with this you wont have any problems with deck flex and clearance.

Also attaching an ultracapacitor between battery and driver. Since ultracapacitors can be charged faster and does not have any charge-cycle limit driver can maximize the amount of electrical charge you can get from braking. And when you need extra power for a short time you can deplete the capacitor, and protect the battery from sudden power surge.
```

---
## \#21 Posted by: jotatsu Posted at: 2017-07-20T13:06:56.895Z Reads: 100

```
[quote="tueboard, post:19, topic:27969, full:true"]
i found this video about "Pressure sensitive dead man switch"
https://www.youtube.com/watch?v=e_ktwKirD5o

i like the idea of Cruising disconnect to save power.
[/quote]

Yep, thats what i was looking for. Not so crazy after all. Seems that  he did go for a strain gauge. I was thinking more in the lines of a Force Sensitive Resistor (FSR)
```

---
## \#22 Posted by: pakue Posted at: 2017-07-20T14:54:43.303Z Reads: 88

```
What about pneumatic cylinders between truck and board? If the valve is open the lean-resistance is nearly the same, but if you close it the trucks become more stiff. You could even adjust the strength by using different sized vent holes.
```

---
## \#24 Posted by: Okami Posted at: 2017-07-20T15:26:46.590Z Reads: 87

```
Lately Ive been speculating whenever something like this for eboard would be possible:

https://youtu.be/3KPYIaks1UY?t=1m45s

Though they do mention it was not a commercial success, as it increased weight of car (was more heavy than conventional suspension.. and probably more expensive too. 

I do know they tend to use something similar in Forestry machines, where the cabin is always leveled. (they also mentioned at end, that they did come up with selling special leveled seats for trucks in the end more or less)
```

---
## \#26 Posted by: pakue Posted at: 2017-07-20T17:26:48.506Z Reads: 76

```
Thats pretty cool!
```

---
## \#27 Posted by: wmj259 Posted at: 2017-07-20T21:51:51.474Z Reads: 72

```
Magnetic suspension will be very expensive and heavy. GMC has some implementation of magnets in their suspension. Lexus had some similar concept with a magnetic liquid cooled hover board. Now the reason it's not feasible, (it can be made, but very expensive) is because it has to be liquid cooled magnets to make them more powerful.
```

---
## \#28 Posted by: jotatsu Posted at: 2017-07-21T18:47:50.236Z Reads: 71

```
What about a wrist protector with integrated controller? , anyone done that?. Seem that those things have enough space and rigidity to mount some eletronics.
```

---
## \#29 Posted by: tueboard Posted at: 2017-07-21T19:13:54.815Z Reads: 73

```
**power switch to turn off/on just one motor**

- it's a bad idea to do this? 
- is better to connect the vescs with can port or use a y-cable?

p.s. sorry for my drawing skills

<img src="/uploads/db1493/original/3X/2/4/243f65eb0eab88a392a22b5b3d3420bfea65c254.jpeg" width="690" height="343">
```

---
## \#30 Posted by: wafflejock Posted at: 2017-07-21T20:24:18.184Z Reads: 70

```
My money says the VESC 2 gets power from motor 2 since you're driving the coil around in a magnetic field so it will generate electrical potential and the power will be driving into the MOSFETs.  You could try but my guess is those end up frying think that power needs to be bled off somehow but then will be definitely less efficient than running the two, would like to see what the difference is with one motor completely disconnected vs two but guess is without fully removing it and the vesc you may be open to drag or worse.
```

---
## \#31 Posted by: FredSaberhagen Posted at: 2017-07-21T20:36:56.985Z Reads: 70

```
It's going to be more efficient to burn current through two motors than one.  Your current in each will be half, meaning resistive losses (i2r) will be 1/4th.  Note that even switching the motor off still incurs the bearing + belt + cogging drag
```

---
## \#32 Posted by: wafflejock Posted at: 2017-07-21T20:37:56.212Z Reads: 69

```
I mentioned this above but people don't believe me :smile:
```

---
## \#33 Posted by: swashplate Posted at: 2017-07-24T09:16:18.124Z Reads: 58

```
Check for carvon controller. They are not wrist protectors per se but you can use it with gloves etc.
```

---
