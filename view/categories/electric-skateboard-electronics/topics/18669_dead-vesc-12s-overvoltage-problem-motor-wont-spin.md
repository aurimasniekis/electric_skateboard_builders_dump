# Dead vesc? 12s overvoltage problem/ motor wont spin

### Replies: 34 Views: 1385

## \#1 Posted by: OleksiiF Posted at: 2017-03-07T00:23:09.775Z Reads: 130

```
i run 12s and on fully charged batteries and with connected receiver i got over voltage error. 1 setted max voltage to 60 and problem never solved, i did connect another bms to receiver and it solved problem with over voltage error, but my motor isnt spinning. (i did set it back to 57v) and i remember that motor stopped spinning when i put 60v on max voltage. (i thought it was another problem like over voltage.)

so now i dont get any errors, but motor isnt spinning.

did i kill my vesc? can i somehow repair it?

realtime data showing no faults 
<img src="/uploads/db1493/original/3X/c/9/c9a5eddbcc7b1e534a380182f7bfd18622ed4f26.JPG" width="690" height="444">

remote set up correctly, 
when i push trigger, green light turning on vesc

app configuration - ppm mode
control mode - watt with reverse<img src="/uploads/db1493/original/3X/e/2/e282e79e6d42a3cbe91c725cd6961abc4db43e90.JPG" width="690" height="444">

if i connect receiver to the vesc thru build-in vesc bms , then voltage varies +- 5 volts! and it shows always higher voltage.
im 100% shure that my batteries are not overcharged

screenshots with 12s batteries and reciever connected only to vesc 
<img src="/uploads/db1493/original/3X/7/a/7abbf719268d9b9319f84ffa2a52cb125f92fda8.JPG" width="649" height="500"><img src="/uploads/db1493/original/3X/e/5/e5d13e7d0147ad86eac3f32b5f98755e5c78db10.JPG" width="652" height="500"><img src="/uploads/db1493/original/3X/7/b/7bdbe8f2045c3d6e711706822c5fdfaabf48339e.JPG" width="650" height="500">

is my vesc dead? can it be healed?
```

---
## \#2 Posted by: OleksiiF Posted at: 2017-03-07T00:24:19.902Z Reads: 112

```
photos of vesc with external bms <img src="/uploads/db1493/original/3X/7/d/7dcd0ceba36221c8fbebefab2825d4dbddb62add.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/7/07de27b2851f8dd4032ec12208715d7520b7e0c3.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/1/71c2bddfe056a47c32df71895631df822ada8096.jpg" width="666" height="500">
```

---
## \#3 Posted by: Sander Posted at: 2017-03-07T09:21:36.058Z Reads: 98

```
Can you show us the motor configuration?
```

---
## \#4 Posted by: OleksiiF Posted at: 2017-03-07T09:23:05.267Z Reads: 99

```
DRV8302
3-Phase Brushless Motor Pre-Driver with Dual Current Sense Amps and Buck Converter
are damaged

any ideas why it got damaged?

motor sk3 190kv
```

---
## \#5 Posted by: Sander Posted at: 2017-03-07T09:24:17.228Z Reads: 98

```
I see whats wrong
```

---
## \#6 Posted by: Maxid Posted at: 2017-03-07T09:29:44.886Z Reads: 98

```
Why are you using an UBEC?

Also for fault analysis type "faults" in the BLDC Tools Terminal
```

---
## \#7 Posted by: Sander Posted at: 2017-03-07T09:29:51.719Z Reads: 100

```
<img src="/uploads/db1493/original/3X/6/f/6f7e8a858f7a8ed1b6865486aef23a3c30789829.png" width="690" height="388">
Switch place with those two
```

---
## \#8 Posted by: Maxid Posted at: 2017-03-07T09:32:07.033Z Reads: 98

```
Wowowow - don't do that
He supplies voltage from the UBEC to the receiver and the way he does it is the intended way. Just look at the markings on the receiver. He has the UBEC power in the right spot on the receiver. What would switching get him?
```

---
## \#9 Posted by: Sander Posted at: 2017-03-07T09:32:48.983Z Reads: 96

```
what do you mean? They have a common power line.
```

---
## \#10 Posted by: Maxid Posted at: 2017-03-07T09:34:52.102Z Reads: 95

```
Also if he has a fried DRV the receiver is not the problem.
```

---
## \#11 Posted by: Sander Posted at: 2017-03-07T09:35:32.682Z Reads: 93

```
He has the SIGNAL WIRE on WRONG PLACE! On the top it says S + -, that MEANS SIGNAL, VCC and GND.  And LOOK he has NO wires going to the SIGNAL pin for the RECIEVER, so he gets NO signal for the VESC, and thats why the MOTOR do not SPIN!
```

---
## \#12 Posted by: Maxid Posted at: 2017-03-07T09:36:19.766Z Reads: 91

```
What are you talking about? The top one is just VCC and the one with three wires is the one coming from the VESC in CH2 - which is correct
```

---
## \#13 Posted by: Sander Posted at: 2017-03-07T09:39:20.126Z Reads: 92

```
No he has not connected it right. He shall connect the VESC PPM output on the TOP of the Reciever where it says S + -. That thing gives him the PPM signal from the potentiometer. The Channels has nothing to do with this. They are only LOW - HIGH output for lights etc. And the power input is the VCC thing right below it.
```

---
## \#14 Posted by: OleksiiF Posted at: 2017-03-07T09:40:08.504Z Reads: 93

```
i use external ubec because with internal i have overvoltage error. even if i set max. voltage to 60v
and in realtime tub it jumps 50v-61v like 10 times per second

"faults" in terminal says there is no faults since startup

signal wire is in right place it worked in these configuration for 5 seconds))

anyone knows where i can buy drv8302 chip? i found a place with 30 bucks shipping(
```

---
## \#15 Posted by: Sander Posted at: 2017-03-07T09:40:20.203Z Reads: 91

```
Connect the VESC wires on top(S + -) of the reciever, and below it on the VCC power output of the ubac
```

---
## \#16 Posted by: Maxid Posted at: 2017-03-07T09:41:59.124Z Reads: 89

```
No - the receiver has a 4x3 pin matrix. the marking you mention is just the indicator that the first column is S, the second + and the third - --> this is true for all rows. The first row is just VCC, the second Ch1, third Ch2 and fourth Ch3.
The first one is used only for VCC supply and will get him NO signal. He needs to have his signal wire in the corresponding Channel row - typically channel 2 - where it is now.
```

---
## \#17 Posted by: OleksiiF Posted at: 2017-03-07T09:42:58.055Z Reads: 82

```
i did it, nothing happens. and when i pull trigger on the remote, green light never reacts by rising brightness. motor isnt spinning
```

---
## \#18 Posted by: Maxid Posted at: 2017-03-07T09:43:35.519Z Reads: 83

```
you can not change the DRV yourself without a reflow oven. It has a ground pad on the bottom. If the DRV is fried it has to be sent in for repair - which is quite expensive.
```

---
## \#19 Posted by: OleksiiF Posted at: 2017-03-07T09:44:46.411Z Reads: 80

```
ill find someone who can do it, i just need to find chip
```

---
## \#20 Posted by: Sander Posted at: 2017-03-07T09:45:20.682Z Reads: 79

```
ohh, okey you are probably right.
```

---
## \#21 Posted by: Sander Posted at: 2017-03-07T09:46:33.043Z Reads: 78

```
Btw does your PPM pulsewidth move when you press in the trigger on the controller?
```

---
## \#22 Posted by: Maxid Posted at: 2017-03-07T09:46:59.389Z Reads: 78

```
[quote="Sander, post:20, topic:18669, full:true"]
ohh, okey you are probably right.
[/quote]

http://i.giphy.com/vEhSzxR4yEmDm.gif
```

---
## \#23 Posted by: OleksiiF Posted at: 2017-03-07T09:47:08.136Z Reads: 78

```
yes, it moves.
```

---
## \#24 Posted by: Sander Posted at: 2017-03-07T09:48:10.571Z Reads: 74

```
but you have no pictures of the motor configuration in the vesc settings that I asked for.
```

---
## \#25 Posted by: OleksiiF Posted at: 2017-03-07T09:49:57.919Z Reads: 73

```
<img src="/uploads/db1493/original/3X/c/0/c0ef85edc181965e5914794c9acdc17aa6debcf6.JPG" width="690" height="436">
```

---
## \#26 Posted by: Sander Posted at: 2017-03-07T09:52:31.612Z Reads: 74

```
I am just guessing here. If you have Motor Max and Batt max at same value it will create an issue? Try to make motor max higher then batt max
```

---
## \#27 Posted by: OleksiiF Posted at: 2017-03-07T09:55:51.072Z Reads: 75

```
how do you think, is this one is good? 
http://www.digikey.com/scripts/DkSearch/dksus.dll?Detail&itemSeq=221101999&uq=636244555750998515
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2017-03-07T15:17:45.728Z Reads: 69

```
The DRV might not be the issue here... look more like a bad ground connection, since the voltage reading is directly on the mcu...

<img src="/uploads/db1493/original/3X/f/d/fd8c20e902257e9a26444be13718fd7963f3110c.JPG" width="500" height="500">
```

---
## \#29 Posted by: OleksiiF Posted at: 2017-03-07T15:21:05.588Z Reads: 68

```
well sounds complicated/ i didnt quite understood everything you told, but ill try to figure it out
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2017-03-07T15:26:15.115Z Reads: 64

```
The reading for the voltage in the bldc tool are not made by the drv, but directly by the mcu. So, if you get a fluctuation on the voltage reading, it is most likely to be a ground problem (bad connection), battery problem or mcu problem (or R4, R3 are not the right value)
```

---
## \#31 Posted by: OleksiiF Posted at: 2017-03-07T15:34:08.892Z Reads: 63

```
[quote="JohnnyMeduse, post:30, topic:18669"]
fluctuation on the voltage reading
[/quote]

fluctuation on the voltage reading are only when receiver connected.without receiver there are no fluctuations
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2017-03-07T15:41:38.561Z Reads: 61

```
Are you able to run a motor detection, and run the motor in the bldc tool without the receiver plug, if so... you probably have a problem with your receiver. You might want to try another one before changing the drv 🤔

If you can't run a motor detection, it's moat likely to be a bad ground connection somewhere over the VESC
```

---
## \#33 Posted by: OleksiiF Posted at: 2017-03-07T15:49:23.823Z Reads: 61

```
no, motor detection is not working, in bldc tool i cant run it with arrows.

i figured out that burned DRV8302. it is seriously damaged. but how did i damaged it? by plugging vesc wire and external ubec wire into reciever in the same time?

 <img src="/uploads/db1493/original/3X/b/8/b87701b5ad080ca845204aed082515833b7fb843.jpg" width="431" height="500">
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2017-03-07T15:52:39.696Z Reads: 59

```
Oh this is these vesc.... If I can suggest you something, Is to buy legitimate VESC. Because routing a vesc is a art and these look badly made.

Probably a bad connection somewhere, if you had problem before connecting the ubec
```

---
