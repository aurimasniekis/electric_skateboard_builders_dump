# Brake fails in the middle of a hill!

### Replies: 12 Views: 782

## \#1 Posted by: benslmn Posted at: 2017-06-05T19:56:11.559Z Reads: 195

```
I was riding down a steep hill (about 40 feet long) and I was pressing the brake the entire time, but about halfway down, the brake failed and I had to bail. Once I got back on the board, it worked perfectly. All the wires were fully plugged in and the battery was almost fully charged. 

I am using a GT2B controller, 2 5000 mah 4s batteries in series, a single TorqueBoard 6355 190KV motor, and a Torque VESC. 

How do I make sure this doesn't happen again?

VESC settings:
<img src="/uploads/db1493/original/3X/8/b/8b5292b468362df0f1eb79eabcff17b6faa5e8ed.PNG" width="690" height="252">

<img src="/uploads/db1493/original/3X/7/5/75246c3fb04899c2313f6ee0e1c798c69ed60d4c.PNG" width="690" height="324">
```

---
## \#2 Posted by: sl33py Posted at: 2017-06-05T19:57:07.249Z Reads: 187

```
was your battery full?  I know this is a potential problem on Boosted...
```

---
## \#3 Posted by: benslmn Posted at: 2017-06-05T19:59:30.549Z Reads: 185

```
No, but almost.
```

---
## \#4 Posted by: sl33py Posted at: 2017-06-05T20:01:33.338Z Reads: 183

```
I know that i've tripped an ABS_OVERVOLT error on a VESC before - and the VESC resets...  I'd post up your VESC settings for folks to help look at this.  Perhaps adjust some settings and *gently* re-test.
```

---
## \#5 Posted by: ryny24 Posted at: 2017-06-05T20:01:47.072Z Reads: 182

```
I've had the same thing happen!!!! It was a big hill and I think I was close to full. Maytech vesc.
```

---
## \#6 Posted by: benslmn Posted at: 2017-06-05T20:12:48.424Z Reads: 177

```
I have attached my VESC settings @sl33py
```

---
## \#8 Posted by: TSG_AU Posted at: 2017-06-06T04:22:14.269Z Reads: 147

```
It seems odd that you could hit an ABS_OVERVOLT error when you're only running 8S and your Max input voltage setting is at 57V- if that were true you would be in serious danger of damaging your batteries catastrophically. Do you have a BMS?

Other than that just don't charge your battery fully if you plan on going down a steep hill.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-06T05:36:24.315Z Reads: 141

```
Right off I see a couple questionable settings.
Absolute max is at 80a and should be 130 to 150
**This from Vedder's Webpage**
“Absolute max” is checked in every PWM switching cycle and used in case the soft back-off strategy for the other limits doesn’t work. I usually set it way higher than the other limits because soft back-off is preferred rather than switching off the motor with a fault code, but it should never be higher than 150.

It appears that setting the absolute max too low will cause the vesc to shut down rather than initiate soft back off strategy.
I'm not sure if this will cause a shut down during braking but the setting should be corrected regardless.

I go down a steep hill that's more like 100 ft or more riding brakes hard with a full battery and have watched my 10s  voltage spike as high as 42.8  still nothing cuts out and no loss of brakes.
I am running dual 6355's and vescs and have my Absolute max set at 140a on each vesc.

You also have multiple ESC over CAN checked and Enable Traction control.

<img src="/uploads/db1493/original/3X/b/5/b5e26fcee228cf4667ac157ce2a8fe3efff5086b.png" width="690" height="117">
<img src="/uploads/db1493/original/3X/7/c/7c8abd4699c5554bc780cc174933096bdfa854e2.png" width="447" height="100">
```

---
## \#10 Posted by: benslmn Posted at: 2017-06-06T11:10:15.961Z Reads: 107

```
@TSG_AU I don't believe I have a BMS and my battery was around 70% so it wasn't close to fully charged.  Is the BMS part of the VESC or is it a separate part? Thanks for your help.
```

---
## \#11 Posted by: benslmn Posted at: 2017-06-06T11:11:17.143Z Reads: 106

```
@Namasaki What does the ESC over CAN setting do? Thanks for your help.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-06-06T12:29:34.436Z Reads: 96

```
Bms is Battery Management System 
It is not part of the vesc
ESC over CAN is an option when running dual Vescs
Try adjusting your absolute Max to 140 and see if that solves the issue.
```

---
## \#13 Posted by: Jinra Posted at: 2017-06-06T14:44:52.945Z Reads: 82

```
I agree with @Namasaki, don't mess with absolute max unless you're sure what your doing.

Also if this happens again, don't turn off your board. Instead leave it in and plug it into bldc tool, then go to terminal and type "faults". This would be very helpful in diagnosis.
```

---
