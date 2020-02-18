# Vesc6 no power no light nothing

### Replies: 17 Views: 193

## \#1 Posted by: Tomgianferrara Posted at: 2019-05-26T16:16:27.701Z Reads: 69

```
Ok so I have a new board I just finished and was riding maybe 2 hours total. Then I hit the break and it felt like something gave way. And I checked to see only one motor working. Opened it up and connected the VESC to its own power and nothing no light no nothing. Please help if you can. Thanks.
```

---
## \#2 Posted by: Tomgianferrara Posted at: 2019-05-26T16:17:28.223Z Reads: 67

```
It was the slave if that helps. And I used the new VESC tool to program.
```

---
## \#3 Posted by: kuphjr Posted at: 2019-05-26T16:37:12.383Z Reads: 66

```
Was there any chance the can-bus wire was disconnected? I don't own a VESC6 but I know this will fry a FOCBOX if the can wire is disconnected when they are both on or if they are not turned off simultaneously. Good news is you can just desolder the CAN chip and use split ppm and you are good to go. I really don't see any benefits to CAN, but maybe traction control matters for eMTB, idk.
```

---
## \#4 Posted by: kuphjr Posted at: 2019-05-26T16:38:09.120Z Reads: 63

```
The "no lights no nothing" thing is what makes me think that it is likely a blown can chip which is causing a short circuit.
```

---
## \#5 Posted by: Tomgianferrara Posted at: 2019-05-26T16:56:48.773Z Reads: 57

```
Can that be fixed
```

---
## \#6 Posted by: mutantbass Posted at: 2019-05-26T17:00:17.863Z Reads: 54

```
is it the legit trampa vesc 6? or a clone?
```

---
## \#7 Posted by: Tomgianferrara Posted at: 2019-05-26T17:37:10.331Z Reads: 49

```
It’s the real one and I switch the other out and it did the same. Is my motor killing them some how. That’s the only thing that was the same.
```

---
## \#8 Posted by: Tomgianferrara Posted at: 2019-05-26T17:40:38.067Z Reads: 48

```
I hooked my other VESC to the same motor and it died in 30 Sec. What the heck can do that? And the motor made a slight clacking sound but nothing crazy. I didn’t even use the breaks this time it just stalled.
```

---
## \#9 Posted by: Silverline Posted at: 2019-05-26T18:17:33.861Z Reads: 41

```
Sounds like a short in your motor....
Do you have a LC meter to check the three phase wires ?If not, you could use this "Ghetto metode" :


Disconnect motor from anything else
Connect phase A to B and verify choppy brakes
Connect phase A to C and verify choppy brakes
Connect phase B to C and verify choppy brakes
Connect phase A to B to C and verify smooth, strong brakes

If the first three are not all the same strength and feel, and the last one is not noticeably stronger and smooth, then you have a winding problem in your motor.
```

---
## \#10 Posted by: Tomgianferrara Posted at: 2019-05-26T18:28:25.126Z Reads: 39

```
Can the motor be fixed? If that’s the case? And are the vesc6 dead? I will buy one and test this.
```

---
## \#11 Posted by: Randy_bobandy Posted at: 2019-05-26T18:35:52.592Z Reads: 37

```
If the motor is bad and you want to see if the vesc still work why dont you try it on the one good motor?
```

---
## \#12 Posted by: Tomgianferrara Posted at: 2019-05-26T18:50:25.624Z Reads: 38

```
Because they get no power at all
```

---
## \#13 Posted by: JakeSkate Posted at: 2019-05-26T18:54:14.533Z Reads: 39

```
Try disconnecting your battery and motor, then short the power lead of your vesc together with a quarter. This will discharge the caps and might reset the whole thing if it's just kinda locked up. This worked for me before when My vesc kept thinking that the high cutoff had been triggered.

After that I would try to reconnect your battery to the vesc and see if it turns on. It's kinda  a long shot but better than nothing.
```

---
## \#14 Posted by: Tomgianferrara Posted at: 2019-05-26T19:18:02.913Z Reads: 37

```
I’m not understanding how to do what your saying? What do I do with the quarter
```

---
## \#15 Posted by: JakeSkate Posted at: 2019-05-26T19:55:09.573Z Reads: 34

```
Short the two power wire of the vesc together with it after you disconnect the battery and the motor from it. Kinda like pulling the cmos battery from a computer.

Edit: added photo for reference
![IMG_20190526_125916|250x500](upload://7FXeaIVjZC37N2XXSMrFixcSTBK.jpeg)
```

---
## \#16 Posted by: JakeSkate Posted at: 2019-05-26T20:16:32.112Z Reads: 31

```
Just thought of this but if your motor really did short out or go phase to phase or something and the budget is tight you can try to recoat your motors windings with enamel this would work: [MG_chem_enemal](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=15&ved=2ahUKEwjq_L7mgLriAhXhQd8KHW3dCksQFjAOegQIABAB&url=https%3A%2F%2Fwww.amazon.com%2FMG-Chemicals-GLPT-Insulating-Varnish%2Fdp%2FB00S4H8V1Q&usg=AOvVaw34oaq2e2BCyD_qOQp-w9ep)

If it took out the gate driver IC you can also replace that and the fets if you have to. VESC shematics are open source and make this kinda stuff easier to diagnose
link to ic gate driver: [DRV8301](https://www.mouser.ca/new/Texas-Instruments/ti-drv8301/)

IDK I hope some of this is helpful to someone.
```

---
## \#17 Posted by: Tomgianferrara Posted at: 2019-05-26T23:08:28.855Z Reads: 22

```
Yes thank you. I’m going to try that. I’m kinda new to all this so it’s gonna take some time. What would I need to test this a multi meter?
```

---
