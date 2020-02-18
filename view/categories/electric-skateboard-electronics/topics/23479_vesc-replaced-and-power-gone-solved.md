# VESC Replaced and Power Gone \[SOLVED\]

### Replies: 6 Views: 556

## \#1 Posted by: sprocket12 Posted at: 2017-05-19T15:36:55.793Z Reads: 49

```
So I rebuilt the Old Man Cruiser over the winter.  Same hardware, new form-factor: 

Single Turnigy 260kV
8S1P- Zippy Lipo 4s1P 8000mAh (x2) (30A inline fuse)
DIY Electric Skateboards power switch
Enertion VESC 4.12
Torque Boards 2.4Ghz mini remote

During testing, I fried the VESC (shorted something).  The batteries on the fuse were fine.  Appears I burned the dreaded DRV8302.  I was able to read the VESC firmware so I saved off the configuration.  I bought a replacement through DIY Electric Skateboards.  After getting it in, I configured and found everything 'squishy'.  Torque was low, brakes less, top-speed reduced...

I went back to my build thread and pulled my VESC settings from there.  ( here: https://www.electric-skateboard.builders/t/old-man-cruiser-new-re-build/7806) No difference.  Hmmm.  I did my maiden long ride this morning into work.  It is about ~11 miles at around 57F.  I was barely moving by the end and had to kick in a few places.  My top-speed was low, the board was measured at 27mph last September; I may have hit 15mph this morning.  The first battery is now connected to the charger.  The cells showed voltages: 3.83, 3.83, 3.82, and 3.72.  These look right to me.  Won't know mAh charge until later...

What do you think?  I'm thinking my LiPo's purchased in Augut last year are already toast unless I'm missing a configuration item in BLDC Tool.

 and re-applied firmware settings for the motor and batteries, re-set up the remote controller, and went to test.
```

---
## \#2 Posted by: Blasto Posted at: 2017-05-19T15:41:32.641Z Reads: 46

```
Did you have the correct voltage cutoffs?
After reflashing, you redid a motor detection?
```

---
## \#3 Posted by: sprocket12 Posted at: 2017-05-19T15:44:09.264Z Reads: 45

```
@Blasto  the voltage cutoffs were read back in from the save settings, but I re-checked them after my first tests with new VESC, so yes.

I also re-ran motor detection.  Results ended up being the same too.
```

---
## \#4 Posted by: Blasto Posted at: 2017-05-19T15:55:56.069Z Reads: 44

```
[quote="sprocket12, post:1, topic:23479"]
I bought a replacement through DIY Electric Skateboards.  After getting it in, I configured and found everything 'squishy'.  Torque was low, brakes less, top-speed reduced...
[/quote]

can you go in the real time data tab, tick the activate sampling, see if theres an error code
```

---
## \#5 Posted by: sprocket12 Posted at: 2017-05-20T15:17:33.751Z Reads: 27

```
Problem solved!  I went back and found VESC files I had saved off last August and re-applied.  What a difference.  Now that all begs a question.  Here is the area I saw that had been changed:

**Motor Configuration**
Motor Tab
Current Limits
Motor max: 70.00 A **(33 A from file**)
Motor min: -30.00 A (**-33 A from file**)
Batt max: 60 A
Batt min (regen): -15.00 A
Absolute max: 150.00 A  (130 A from file)

The motor specs actually match at 70 A max.  What does this change?  In all my plots, I've never seen the board pull 30 Amps.  The voltage settings were all the same.  My torque, acceleration, and top speed were all affected.  Help me understand.

Thanks
```

---
## \#6 Posted by: SageTX Posted at: 2017-05-20T19:30:07.260Z Reads: 20

```
There was a **_very long_** thread a while ago about the difference between motor amps and battery amps. 

Anyone recall that fiasco?
```

---
