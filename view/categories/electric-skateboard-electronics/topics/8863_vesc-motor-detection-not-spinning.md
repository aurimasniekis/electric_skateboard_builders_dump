# VESC Motor Detection (Not Spinning)

### Replies: 7 Views: 1032

## \#1 Posted by: Sleepingalex24 Posted at: 2016-09-03T18:10:36.064Z Reads: 91

```
I have just recently bought a VESC from enertion and tried to get my set up working. I managed to get it to turn on and connect to the computer. However after doing so I noticed a burn spot right above the DRV8302 chip and after that the motor detection wouldn't work. I would click start detection the VESC would blink pink and then I would switch over to realtime data and this pops up, then the motor detection fails:<img src="/uploads/db1493/original/2X/a/a6c7f280d37ef39a79d97454259043ad5e2df4ac.PNG" width="690" height="475">
Also at no point during the motor detection is there a fault code in the realtime sampling tab. 
Here is the VESC:
<img src="/uploads/db1493/original/2X/d/d74e8dc5efd6c56ffb71fad1bd19225400445c3b.jpg" width="281" height="500">
Specs:

* 30A 110V Switch from Lowes
* 4.12 VESC from enertion (2.18 firmware)
* 2 3s 5200mah Multistar LIPOs
* Turnigy SK3 6374 motor 149kv
* HK-GT2B
Here is the wiring (Hooked up in series with a switch):
<img src="/uploads/db1493/original/2X/1/120a46baa32e36bf93b6af345f695f63486d6cbf.jpg" width="690" height="278">
I'm wondering if the problem is the DRV chip and where I could maybe get a replacement or get it repaired. Also wondering if the switch would be a problem in the future.
```

---
## \#2 Posted by: treenutter Posted at: 2016-09-03T20:07:41.737Z Reads: 80

```
That definitely looks like a DRV fault. The large burnt hole on the chip suggests that it is destroyed and needs to be replaced. Sorry @Sleepingalex24
```

---
## \#3 Posted by: Sleepingalex24 Posted at: 2016-09-03T21:03:48.354Z Reads: 75

```
Ok just wanted to make sure before repairing thanks.
```

---
## \#4 Posted by: lox897 Posted at: 2016-09-03T21:23:20.739Z Reads: 70

```
Why do you have a 30amp fuse? I'm wondering if that has anything to do with the fault because when the motor accelerates it can go past 30amps. Also, have you clicked the checkbox so that you can see the faults?
```

---
## \#5 Posted by: Sleepingalex24 Posted at: 2016-09-03T23:46:08.703Z Reads: 54

```
When I decided to buy the 30A switch I thought it would be plenty enough for the system I'm building. I thought that if I calculated the wattage of both then I would know if it would be able to handle the current. Is that how it works? Or do I have to have a fuse that is 60A.
30A x 110v = 3,300 watts
60A x 22.2v = 1,332 watts
Also where is this checkbox is it on the realtime data tab?
```

---
## \#6 Posted by: Sleepingalex24 Posted at: 2016-09-03T23:57:42.003Z Reads: 50

```
I also want to confirm I did all of the inputs correctly for my batteries and motor.
2 x 3s 5200mah Multistar LIPOs
Turnigy SK3 6374 motor 149kv

Motor max 60A
Motor min -60A
Batt max 60A
Batt min -40A
Absolute max 140A
Min input voltage 8V
Max input voltage 57V
Batt cutoff start 22.2V
Batt cutoff end 21.6
```

---
## \#7 Posted by: saul Posted at: 2016-09-04T00:17:16.454Z Reads: 46

```
forsure that vesc is dead. :head_bandage:

dont think its related, but switches and electronics in general are rated for amps, not watts. 
the switch/fuse is probably cheaper, but the aniti spark switch is the way to go, some version have a fuse built in.

Also, your voltage is pretty low for that motor, I use it on 12s. I'd say at least get another 3s pack and run on 9s. but do it before you start using those packs, not good to mix used and new.

oh and i'm using 5200mah multistart pcks too, 2x 6s in series for 12s. 
keep in mind they are 10c discharge packs.
that means 10 x 5.2 = 52 amps continuous. so you'll probably want to keep your max around 45/50...

guess i'll just keep going...
motor min is regen braking, 60a will probably toss you on your face. i would start around -35A and move down as needed,
bat min, is how much amps go back to your batteries, usually you don't want to charge more than 1-2c, so thats 5-10A...i think i use -12A...
```

---
