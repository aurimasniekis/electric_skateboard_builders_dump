# Random drv error dual 6355

### Replies: 26 Views: 807

## \#1 Posted by: Bjork3n Posted at: 2018-04-01T16:06:58.930Z Reads: 111

```
Hey guys!
So i finshed my build a couple of weeks ago but i have issues with the vesc.
Im using maytech vescs that i bought from eskating.

Running 60 motor amps and 30 Battery max everything is fine no fault codes nothing.
But as soon as i raise battery max or motor max i get drv fault codes on acceleration.

Board cuts out under full acceleration and shows the drv 8302 error but works as normal 2-3 sec after.
 (At 16.08 drv fault , acceleration) Works normaly afterwards.
https://metr.at/r/dx0j8 

**Settings** when fault code appears.  (using single setup at the moment)
Motor max 70-80A
Motor min 50A
Battery max 35-40A
Battery min -8 

Startup boost 0.05
Current ramp up step 0.04

**Hardware**
6355 190kv motor (running sensorless)
samsung 30q 10s4p battery.
Maytech vesc 4.12 with ackmaniac fw (tried stock same problem)
83mm wheels with 16/36 gearing.

Went out using 60/30A and was no issue with full accelerations , no fault code and no cutting out. 
https://metr.at/r/dtjqX
Is this due to the quality of the vesc or is something in my settings wrong??
Want to be able to use the full potential of the parts without errors...
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-01T16:13:20.397Z Reads: 92

```
I can think of a few things off the top of my head.
1. Overheating issues. Solved by putting a small 5v fan on top of drv/mosfets.
2. Bad assembly job. Inspect vesc for abnormalities.
3. Bad drv. Replace drv with a genuine one.
4. Battery wires longer than 30 cm. Shorten wires or add caps.
```

---
## \#3 Posted by: Bjork3n Posted at: 2018-04-01T16:15:21.423Z Reads: 91

```
1. Not possible, temp is below 50C when error appears
2. Looks ok , problem occurs on all 3 of my maytech vescs.
3. Are there really copies of the drv chips?
4. Battery wires are max 10cm long.
```

---
## \#4 Posted by: RedEagle Posted at: 2018-04-01T16:19:17.923Z Reads: 87

```
1. Yes it is. Chinese parts have a lower tolerance. So while 50c doesn't seem much for say focboxes, for cheap chinese hardware 50c could be too much.
3. Yes.

What remote are you using? Have you checked your setup for any abnormalities? (exposed wire, missing caps)
```

---
## \#5 Posted by: Bjork3n Posted at: 2018-04-01T16:23:46.173Z Reads: 80

```
1. If temp was an issue over 50C then how come i could go up to 80C on the 2nd ride with no issues (Lower settings).
2. Never heard of any drv fakes but maybe youre right.. 

Remote is Eskating Remote V2, max and min pulsewidth  setup done.
```

---
## \#6 Posted by: RedEagle Posted at: 2018-04-01T16:31:44.052Z Reads: 74

```
Because you used different settings.

You have a bad drv. Replace it and I would also suggest checking the board for shorts etc.
```

---
## \#7 Posted by: Bjork3n Posted at: 2018-04-01T16:36:43.601Z Reads: 70

```
Yes but i really cant see anything bad with the settings i used that may cause a drv error.
And if there where shorts, there would be issues with lower setting aswell?

Im so close to buying focboxes to get rid of this issue but first i want to get to the bottom of whats causing it.
Would be sad to blow focbox aswell.... :/
```

---
## \#8 Posted by: RedEagle Posted at: 2018-04-01T16:44:02.042Z Reads: 67

```
Your settings may be good but hardware side it's a different story. You are using cheap vescs. 
Here in the esk8 community the golden rule goes 'buy cheap, buy twice(or how many times you blow something).
 You will end up spending more because you initially used cheap parts that failed. You're better off buying expensive parts and never worry about faulty hardware.

I also use maytech. Mine died because of water damage and corrosion. But that's totally my fault. Seems I got a good batch (and I totally ruined it xD).
```

---
## \#9 Posted by: Blasto Posted at: 2018-04-01T16:46:27.143Z Reads: 68

```
Honestly, i don’t think counterfeit drv8302 chips exist. However the components like the caps, thats another story
```

---
## \#10 Posted by: Bjork3n Posted at: 2018-04-01T16:47:52.322Z Reads: 69

```
I have two of my previous maytech vesc on drv repair after the same issue, "randomly drv faults".
Worked fine when i shipped them but i didnt want to gamble with them.
So they will have 2 brand new drv8302 chips (orginal ones).

Thing is im afraid that they will blow once again if i try to go with higher settings...
Hence the reason im thinking of buying focboxes and be done with it. 

I only use BLDC btw.
```

---
## \#11 Posted by: RedEagle Posted at: 2018-04-01T16:52:45.067Z Reads: 63

```
ESCape and b box are also an option. Make sure to report back if the repaired vescs work or not!
```

---
## \#12 Posted by: mmaner Posted at: 2018-04-01T21:43:18.681Z Reads: 57

```
[quote="Bjork3n, post:1, topic:50872"]
Motor max 70-80A

Motor min 50A

Battery max 35-40A

Battery min -8
[/quote]

I would set motor max to 60, motor min is fine, battery max to 30, battery min is fine. See if your problem goes away. 

It could be a BMS issue causing the cutouts. I've got a vesc that shows drv errors Everytime I accelerate but it doesn't reboot or cutout. Sometimes DRV errors are not real, they are related to something else and it just reads that way.
```

---
## \#13 Posted by: Bjork3n Posted at: 2018-04-01T21:50:51.555Z Reads: 53

```
It does goes away using these suggested settings you say. 
Motor max 60A
Motor min 50A
Battery max 30A
Battery min -8

Just wondering what triggers the cutout, is it limitations in the hardware that would be sorted with focboxes? 

Don't think it's a bms issue it should allow for burst. 
I've been pulling over 76 battery amps one time on that battery without it cutting out. 
The vesc don't reboot when the fault occurs it works immediately after without reboot.  You can see that on the metr data, never reboots. 
Did motor detection tonight just to see if it would give fault and it did not, works just like it should. 
It's weird...
```

---
## \#14 Posted by: mmaner Posted at: 2018-04-01T22:05:35.351Z Reads: 49

```
Yep, likely just vesc limitations. As I understand it the Maytech VESC's are rated at 50 amps.
```

---
## \#15 Posted by: Deckoz Posted at: 2018-04-01T22:12:26.696Z Reads: 48

```
I had this issue with original 4.12 bodies.. they would cut out or reboot. I think it's because when you reach batmax under heavy acceleration the fets aren't fast enough to close the gate and the next read of the current is an over current fault from the software.

I haven't had any issues like this since using ESC with direct fets...
```

---
## \#16 Posted by: Bjork3n Posted at: 2018-04-01T22:17:33.367Z Reads: 46

```
And this would display drv error instead of over current fault? @Deckoz
```

---
## \#17 Posted by: Bjork3n Posted at: 2018-04-01T22:18:21.958Z Reads: 43

```
Yeah and I'm pulling below what they are rated for. 
30A no issues , 35A = Fault
```

---
## \#18 Posted by: mmaner Posted at: 2018-04-01T22:20:28.653Z Reads: 43

```
That's what they are rated. That's not necessarily a fact.  I've seen people with Maytech VESC's that rebooted every time they went over 30 amps. I would just leave them at 30 amps and call it done.
```

---
## \#19 Posted by: Bjork3n Posted at: 2018-04-01T22:27:38.958Z Reads: 40

```
Is it the battery max that makes it cutout you think? 
Can I use a higher motormax to increase acceleration and keep it at 30A for the battery?
```

---
## \#20 Posted by: Deckoz Posted at: 2018-04-01T22:32:58.463Z Reads: 42

```
Yea it's drv error over current. Not drv abs over current.
```

---
## \#21 Posted by: Bjork3n Posted at: 2018-04-01T22:35:10.925Z Reads: 40

```
@Deckoz 
Aha ok I was under the impression that once you get the drv error the vesc is finished more or less.
```

---
## \#22 Posted by: Deckoz Posted at: 2018-04-01T22:55:42.624Z Reads: 41

```
There's 12 or so fault codes.. not all of them mean death.
```

---
## \#23 Posted by: Bjork3n Posted at: 2018-04-01T22:56:48.039Z Reads: 41

```
Thanks for that info! 😃👍
```

---
## \#24 Posted by: Bjork3n Posted at: 2018-04-02T16:30:00.065Z Reads: 32

```
Did some more testing today, went over 10km on these settings
Motormax: 60A
Motor min : -50
Battery max : 30
Battery min: -8 

Did full accelerations from standstill and really tried to push the system.
No fault codes, no cutouts , no issue what so ever.

Conclusion maytech vesc can only handle batterymax of 30A (I pulled 28A maxiumum) If you set it higher it will cutout and show drv error as soon as you start to push the system.

Will settle for these settings on both of my motors and hopefully i will be ok. 
I will however get some focboxes to be able to boost up the power up when im getting used to the settings above.

Cant say enough good things of Ackmaniacs watt control, it really makes the board controllable! 
Thanks for the help guys!
```

---
## \#25 Posted by: Berlad180 Posted at: 2018-04-29T17:18:28.489Z Reads: 21

```
I am having a similar issues of randomly cutt off when starting the ride. And a few seconds later the ride is great.
But please could you explain how do you monitor all those parameters after the ride ?
Is it stored on the Vesc some how ?
I dont know how to understand whats going on in the Vesc while riding.. 
Thanks
```

---
## \#26 Posted by: Bjork3n Posted at: 2018-04-29T17:31:19.854Z Reads: 20

```
Im using a METR bluetooth module that is connected to the vesc.
You can buy it here: https://eskating.eu/product/bluetooth-uart-module-for-electric-skateboards-ios-android-metr-app/ Or https://metr.at/shop
```

---
