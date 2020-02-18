# Is a smooth throttle cutoff possible with vesc?

### Replies: 17 Views: 892

## \#1 Posted by: Apolo Posted at: 2018-03-13T02:52:44.974Z Reads: 152

```
Not sure if the wording is right, but what I'm trying to say is to have a feature where if you suddenly let go of your throttle, the motor doesn't just suddenly go to zero power but instead, have it automatically ease the throttle off. 

I'm pretty sure boosted has this feature. 

I'm nowhere near an expert with a vesc so if I sound dumb, it's because I am.
```

---
## \#2 Posted by: Deckoz Posted at: 2018-03-13T03:18:07.183Z Reads: 151

```
You could do this with a remote. Photon has something like this. Where you can change the sensitivity of how fast the "input"  is allowed to change.

It's not quite exactly what you are saying. But the result is almost the same.
```

---
## \#3 Posted by: Apolo Posted at: 2018-03-13T03:20:52.590Z Reads: 149

```
possible to do it with a standard ppm or firefly nrf?
```

---
## \#4 Posted by: Deckoz Posted at: 2018-03-13T03:30:46.878Z Reads: 148

```
You could use an Arduino in between the receiver and vesc to smooth the ppm stream.
```

---
## \#5 Posted by: AssaultedPotato Posted at: 2018-03-13T03:46:04.956Z Reads: 147

```
Is this not the setting in question?
![image|690x462](upload://n74UK3NZMVs0J7jNo11GM5Hys68.png)
```

---
## \#6 Posted by: Apolo Posted at: 2018-03-13T03:50:14.939Z Reads: 137

```
I think that's it! I wonder how I missed that, I literally spent 20 minutes going through all the esc tool settings looking for something like that

Will try it out tomorrow and see if it works

The positive ramping time sounds useful too. So far I've been using the throttle curve adjustments to get a smooth acceleration. I feel like positive ramping time will give me a much smoother take off
```

---
## \#7 Posted by: Deckoz Posted at: 2018-03-13T04:02:39.344Z Reads: 134

```
Nice  I didn't know that was in the new 3.x firmware
```

---
## \#8 Posted by: E1Allen Posted at: 2018-03-13T04:31:46.403Z Reads: 130

```
Is that option in the regular BLDC software? 2. Whatever
```

---
## \#9 Posted by: Apolo Posted at: 2018-03-13T04:33:12.263Z Reads: 132

```
Don't think so. Just flash your firmware to 3.xx and use the new vesc tool. Much better
```

---
## \#10 Posted by: kyletrainy Posted at: 2018-03-13T05:53:45.400Z Reads: 119

```
What values are you guys going to put on negative ramping time? Also thanks for this thread! Lol I’ve had this annoyance for a while now and didn’t know what it was
```

---
## \#11 Posted by: ShutterShock Posted at: 2018-03-13T06:46:07.446Z Reads: 105

```
I've never been able to get BLDC detection to work in the VESC Tool with 3.xxx

What are you using?
```

---
## \#12 Posted by: Jammeslu Posted at: 2018-03-13T07:33:25.436Z Reads: 95

```
Should be possible to implement it on the firefly
```

---
## \#13 Posted by: AssaultedPotato Posted at: 2018-03-13T08:15:55.143Z Reads: 92

```
Positive ramping definitely helps keep the board from launching with sudden flicking of the throttle
```

---
## \#14 Posted by: AssaultedPotato Posted at: 2018-03-13T08:16:38.326Z Reads: 92

```
FYI I'm using ACKMANIAC's VESC Tool
```

---
## \#15 Posted by: Slak Posted at: 2018-03-13T09:48:21.866Z Reads: 89

```
And what IF the Arduino fails or "get crazy" with your PWM signal ? I'm not sure having device(s) between your VESC and your receiver is a good thing (more electronic = more possible fails, and when it's about the throttle, it can be called unsafe IMO)
```

---
## \#16 Posted by: Deckoz Posted at: 2018-03-13T13:19:21.984Z Reads: 78

```
Anyone using an. nRF like solid geeks remote, ervinelin  or the photon has an Arduino in between the receiver and the vesc...

So while I agree, I disagree.
```

---
## \#17 Posted by: Slak Posted at: 2018-03-13T13:53:11.921Z Reads: 70

```
True ! But the fact nobody had issue doesn't mean it can happen. Same reason why I won't get a remote based on Arduino for now but instead will enhance a GT2B, one heavily tested and debugged remote and signals is a bit secured as well iirc. This was only my 2 cents for those concerned by the safety and electronics.
```

---
