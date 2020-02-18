# DRV8302 and motor still running! Need help diagnosing

### Replies: 12 Views: 674

## \#1 Posted by: Sebike Posted at: 2017-09-30T16:10:26.049Z Reads: 90

```
Hi!

I went for a 20 min ride about 7 km. Pretty hard accelerations and some downhill braking. Batt was around 38v at beginning of ride. 

Hit a few small rocks, but other than that a smooth ride. Didn't experience anything odd from the board apart from the (usual) motor screech at higher rpms that was addressed in a previous thread (bearings issue?)
https://www.electric-skateboard.builders/t/motor-making-knocking-ticking-sounds-at-low-speed/33700/19
Getting back from my ride I see this error in the Ackmaniac app
<img src="/uploads/db1493/original/3X/8/e/8ef37800fc89fc09a875ae3bd00f1666389cc5ea.png" width="281" height="500">
The motor runs ok just like before the ride and I have no idea when this happened. The fault code gets me a bit worried though and the current (325) seems crazy high, no?

I'm currently running a single motor setup with a FOCbox that was configured for FOCmode using the extended BLDC-tool FOC-wizard.

Motor is a sensored 6374 from euskating.eu and batteries are 30q 10s4p with a SuPower 60A BMS. I can rotate motor by hand with no resistance from motor.

What might hav given this fault code, and should I worry about FOCbox getting fried? Something that is OH-NOOO in my VESC settings? 

TY

settings;
<img src="/uploads/db1493/original/3X/8/1/81bfc14efbb00294ce8bc12dc3176bf991ec2602.gif" width="690" height="387">
<img src="/uploads/db1493/original/3X/7/3/735dd2b44adbbe497d90ddba77866fd00e0885d2.gif" width="690" height="387"><img src="/uploads/db1493/original/3X/2/9/2940a8635cdc121ef110cce32f99c5df5e537ff2.gif" width="690" height="387">
<img src="/uploads/db1493/original/3X/5/5/5584e5d8738d77693ff10e620854c9414ec42077.gif" width="690" height="387"><img src="/uploads/db1493/original/3X/0/7/0717f66f4b65bcfc256d2285bc137d3b866370ac.gif" width="690" height="387">

Edit; Getting the same fault code in BLDC-tool
```

---
## \#2 Posted by: scepterr Posted at: 2017-09-30T16:16:27.619Z Reads: 75

```
It's possibly a loose connection somewhere caused the spike and error not anything with the vesc itself
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-09-30T16:19:22.394Z Reads: 73

```
looks like loose connection. 300 amp should kill ur mosfet and motor not to mention drv chip. and u have bms so... 
but i had drv on my focbox,so reflashed to 2.18 before. now i dont have any problem. seems like 2.18 is most stable at the moment apart from 3.26,
```

---
## \#4 Posted by: Sebike Posted at: 2017-09-30T16:19:27.140Z Reads: 73

```
Could a loose connection be at either side of the VESC giving this fault code, ie, could the batt side connection issue cause this as well as the motor side?
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-30T16:20:19.170Z Reads: 72

```
I'm not sure, haven't encountered that scenario personally, only loose connection on the motor side(the connector didn't look loose, just the bullet was bad)
```

---
## \#6 Posted by: Martinsp Posted at: 2017-09-30T16:21:25.871Z Reads: 67

```
I am not entirely sure what causes this but Benjamin on EndlessSphere I believe once explained that these non-latching faults are caused by under-voltage on some lines going to the DRV which caused it to malfunction and send a fault code to the MCU. I would not be worried about this fault as a DRV error but rather loose connection that got disconnected and then connected again which caused a current spike and a voltage sag which goes back to the DRV.
```

---
## \#7 Posted by: Sebike Posted at: 2017-09-30T16:26:35.753Z Reads: 64

```
Interesting.. You mention voltage sag, shouldn't the voltage reading be low then, or how can one explain 41+ v and high current? Regen braking while loosing connection?
```

---
## \#8 Posted by: Martinsp Posted at: 2017-09-30T16:29:49.365Z Reads: 62

```
Sorry, did not explain it enough. I am not talking about battery voltage. DRV does not receive XX volts from your battery in normal scenario. When it does it is usually because the gate gets shorted to the battery lead and that is when the DRV is just destroyed to hell and back. I was talking about voltages that are much smaller. I dont know their names, can not find the thread again, but the voltages might be like 3.3V for logic or maybe even some communication lines. I will search for that thread to confirm my statements.
```

---
## \#9 Posted by: Sebike Posted at: 2017-09-30T16:35:49.611Z Reads: 57

```
Ok, I see. Great info, thanks. Not as worried as before then :blush: 
I'll check if I can find any signs of loose connections.
```

---
## \#10 Posted by: jmasta Posted at: 2017-09-30T23:42:07.976Z Reads: 50

```
[quote="Martinsp, post:6, topic:34388, full:true"]
I am not entirely sure what causes this but Benjamin on EndlessSphere I believe once explained that these non-latching faults are caused by under-voltage on some lines going to the DRV which caused it to malfunction and send a fault code to the MCU. I would not be worried about this fault as a DRV error but rather loose connection that got disconnected and then connected again which caused a current spike and a voltage sag which goes back to the DRV.
[/quote]

So you're saying that if your BMS cuts off power because of voltage sag, it could trigger a DRV8302 fault code?  

I've had a lot of cutouts lately. Sometimes it gives a DRV8302 fault, sometimes an under voltage fault, and sometimes no fault code is registered.  VESC resets and keeps working after.  I believe the underlying cause is a degraded cell which drops voltage so much under load that it hits the 2.9V BMS cutoff.  It can't be a loose connection on my end; everything is taped or shrink-wrapped, and properly soldered. However I am concerned that my DRV chip is failing after so many faults
```

---
## \#11 Posted by: Martinsp Posted at: 2017-10-01T09:37:44.833Z Reads: 39

```
[quote="Martinsp, post:8, topic:34388, full:true"]
Sorry, did not explain it enough. I am not talking about battery voltage. DRV does not receive XX volts from your battery in normal scenario. When it does it is usually because the gate gets shorted to the battery lead and that is when the DRV is just destroyed to hell and back. I was talking about voltages that are much smaller. I dont know their names, can not find the thread again, but the voltages might be like 3.3V for logic or maybe even some communication lines. I will search for that thread to confirm my statements.
[/quote]
I was talking about fluctuating voltages that are not battery voltage. 

If you are getting undervoltage errors try to have a look at the batteries. What could happen (happened to me once) is that due to vibrations and in some cases also due to board flexing one cell can get disconnected and the parallel pack now has less capacity. What happened to me is that my 10S3P pack had one of the cells disconnecter which did not change the voltage of the whole pack but it changed that I had 9 series banks that are 9000mAh and one that was only 6000mAh. So of course that one discharged faster and the BMS disconnected the load and that caused some cut outs for me. Have a look at that to eliminate as many variables. Also what you could do is check the voltages of all cells (after a short ride so that the voltage difference will be visible)and if they dont have all the same voltage ,assuming you used new cells, there is some connection problem inside the battery pack.

I am not sure if faults can damage the DRV... I think not because the fault code is there to prevent the damage from spreading etc..  Also half-broken DRV would not explain undervoltage fault.
```

---
## \#12 Posted by: Sebike Posted at: 2017-10-05T19:21:43.742Z Reads: 31

```
Went through the connections yesterday and found one of the bullet connectors having a slight bend on part of the male connector. Probably caused by going over rocks and connectors slammed against each other, and the little extra room probably made one bullet loose conection for a fraction of a second..
```

---
