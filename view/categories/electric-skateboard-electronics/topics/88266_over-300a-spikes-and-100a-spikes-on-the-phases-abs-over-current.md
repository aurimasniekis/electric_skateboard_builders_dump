# Over 300A spikes and -100A spikes on the phases (ABS_OVER_CURRENT)

### Replies: 15 Views: 404

## \#1 Posted by: TimothyVaissi Posted at: 2019-03-25T18:41:05.759Z Reads: 118

```
So I've got this problem with my VESCs. If I do a hard acceleration or if the motor needs to do a bigger push, the vesc reboots. After hooking it up to a pc and checking fault codes I get a ABS_OVER_CURRENT for a second and then it the error disappear. The biggest problem is, when this happens the board turn off and I (nearly) goes flying of. 
I have tried updating the firmware, adding bigger caps, shorten the wires, removing all bullet-connectors and lowered all motor/battery settings. But nothing changes :(
The VESC I'm using is the Flipsky Vesc 4.20 from banggood ( https://www.banggood.com/HGLRC-Flipsky-Mini-FSESC4_20-50A-ESC-Based-Upon-VESC-With-Aluminum-Anodized-Heat-Sink-for-Rc-Car-p-1349277.html?rmmds=search&amp;cur_warehouse=CN) 

It's probably the design of the vesc that causes this I would assume, but are there anything you might suspect why this is happening?

![300a%20peak|690x367](upload://unkiWpvzUs1POmoUfPUW6M68Ug0.png) 

![bldc%20settings|690x368](upload://2QF0wAwYFAfIhEPKu3LQ2kpldrg.png) 

I have looked everywhere but haven't found anything about these kind of huge current spikes
```

---
## \#2 Posted by: Santino Posted at: 2019-03-25T19:31:35.726Z Reads: 95

```
You should put more info (motor, battery, configuration); by the other hand...RC esc to run a board at 50A motor max, and 50 of break...I would by another Esc more capable to manage sudden acceleration, like FocBox, Vesc 6. I also will try setting 35A motor max, 30 motor break, 150 absolute current...If thats works good, it might be time to buy a better Vesc to handle those currents. Wish you the best...
```

---
## \#3 Posted by: TimothyVaissi Posted at: 2019-03-25T19:57:21.677Z Reads: 90

```
I've tried running it on a higher absolute and super low motor/battery settings, down to 20A but still the same :/
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-03-25T19:59:18.627Z Reads: 85

```
it might just be the 4.20 actually

what voltage are you running your build at?
```

---
## \#5 Posted by: TimothyVaissi Posted at: 2019-03-25T20:17:25.555Z Reads: 79

```
That is what I'm starting to think too. I'm running 10s
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-03-25T20:18:25.969Z Reads: 79

```
keeps the batt max normal and try to increase your motor max but no higher than 30a and see what happens

**ps dont eat street
```

---
## \#7 Posted by: TimothyVaissi Posted at: 2019-03-25T20:22:41.921Z Reads: 76

```
I tried batt max 15A, motor max 20A/-20A but still the same :/
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-03-25T20:23:04.003Z Reads: 75

```
up the battery max

15a is low

also what battery you got?
```

---
## \#9 Posted by: TimothyVaissi Posted at: 2019-03-25T20:30:28.359Z Reads: 74

```
i have zippy 5ah 20c LiPo's
Still no luck :(
```

---
## \#10 Posted by: AlanZhou Posted at: 2019-03-25T20:53:57.667Z Reads: 69

```
voltage? how many volts is it?
```

---
## \#11 Posted by: TimothyVaissi Posted at: 2019-03-26T07:34:08.694Z Reads: 59

```
it's 10s, so 42v charged
```

---
## \#12 Posted by: lrdesigns Posted at: 2019-03-26T08:10:02.884Z Reads: 55

```
Check if your main capacitors leg broke from vibration? Could be this or some other error in reading currents. 

Did you use it a while before this issue arose or did it do that from the start?
```

---
## \#13 Posted by: linsus Posted at: 2019-03-26T13:30:38.277Z Reads: 49

```
https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824

Looks like the same hardware?
```

---
## \#14 Posted by: TimothyVaissi Posted at: 2019-03-26T21:48:02.192Z Reads: 31

```
Thank you so much @linsus for shearing the post! I'm gonna test the fix tomorrow and it should work.  It have been confirmed by Flipsky that the problem was as described in the post :D
```

---
## \#15 Posted by: linsus Posted at: 2019-03-26T22:00:32.019Z Reads: 29

```
No problem bro, surprised noone of the others didnt already :slight_smile:
```

---
