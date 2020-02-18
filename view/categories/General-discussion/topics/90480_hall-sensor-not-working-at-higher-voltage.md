# Hall sensor not working at higher voltage

### Replies: 2 Views: 130

## \#1 Posted by: Morgs_mcgyver Posted at: 2019-04-14T10:47:47.418Z Reads: 40

```
Hi all - long time reader - first time poster
Hoping there is a simple fix...
I’ve just finished my new board I’m trying to set up the VESC to sensor mode. As recommended for my first power up of VESC I used a power supply -12volt. I started hall sensor detection and it all went fine, applied and wrote to VESC. Motors spun up and all seemed good. When I switched over to the battery -36volt-  the motor just makes a noise and won’t spin...? I’ve gone back into VESC  rerun sensor detection using the battery pack and it tells me I have a “hall detection failed” - motor won’t spin up. 
So with no changes to VESC other than input voltage the hall sensors work and then don’t work? 
I’m running a duel motor and VESC and have the same issue on both so thinking it’s a software rather than hardware issue? Plus at the lower voltage everything is fine and I get a correct detection so also eliminates incorrect wiring or faulty hardware. Also if I go back in and turn VESC back to sensorless everything works fine - at both 12 and 36volts. 
Can someone point me in the right direction as it’s doing my head in? 

Hardware;
Hobby king VESC - 
# Racerstar 5065 BRH5065 140KV
36volt lipo
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-04-15T06:19:47.891Z Reads: 20

```
Make sure your battery voltage is correct in the vesc. Also, make sure your motors are not connector to belts or wheels. Any drag or resistance during detection gives bad results
```

---
