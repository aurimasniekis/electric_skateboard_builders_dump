# AWD battleship of a longboard

### Replies: 14 Views: 1162

## \#1 Posted by: er2528 Posted at: 2016-09-06T13:24:39.975Z Reads: 215

```
Hello :) New to the message boards.  I figured I would share this build I'm doing; it has absolutely no definite purpose other than to be completely absurd.  And fun. I've a surplus of high quality parts and boards all over the place, so what better to do with them than to get creative.  Anyway, I noticed some others were having luck using different motors of varying Kv-ratings.  A fun challenge maybe?

I have assembled two gnarly Scorpion S4020-16s to the front axle, powered by a 16-cell 2p8s LiFePo4 bank (rear is a single string of 10s standard lipo 3.7v / cell nominal).  The rear axle has two SK3 6364s attached (mounts should arrive today).  Front motors are 420kV while rear is 245kV.  There are three separate batteries at two separate voltages. There is timing pulleys for days to mechanically adjust the motor to wheel underdrive ratio.  At first I was planning on a controller in each hand, however, I do believe the receiver remains unaffected as it merely transmits a PWM signal and has nothing to do with the motor/controller supply power.  This is correct, yes?

The disparity of the motor speed to potential ratings seems to be the biggest obstacle.  At any rate, I post this up for consideration; really appreciate the input.  I'll probably break it down and make two boards from it afterward.  Has anyone
else done anything similar?
```

---
## \#2 Posted by: er2528 Posted at: 2016-09-06T14:01:44.735Z Reads: 201

```
I should include some pictures to affirm this is actually happening.

I had to modify the shafts on the Scorpions (reluctantly) as they're almost $200 a piece.  It's next to one of the batteries.  Excuse the mess, bench testing stuff.  Still have one more battery to assemble, wrapped the cells and ready to assemble

Who has experience with the SK3 line of motors?  Should I install only one in the back with a jackshaft?  How are the durability on those?  Has anyone burned one down on overcurrent before?

Can't wait to get this done!<img src="/uploads/db1493/original/3X/6/d/6d1844fd2df04e85bbd517e5debc4946a748dd30.jpg" width="349" height="500"><img src="/uploads/db1493/original/3X/b/d/bdd482a98613efcdb846851e8c965f4df5892f5a.jpg" width="690" height="388">
```

---
## \#3 Posted by: evoheyax Posted at: 2016-09-06T15:48:06.233Z Reads: 172

```
I've been wanting to see a 16s setup for a long time. Do you know what esc you want to use? Thats the biggest hurdle in 16s that I had in researching parts.
```

---
## \#4 Posted by: er2528 Posted at: 2016-09-06T16:52:50.269Z Reads: 158

```
This setup is 3 batteries: 2 banks in parallel up front, and a divorced system, separate in the rear on a different ESC.  I would be curious to see a 16s myself
```

---
## \#5 Posted by: Dornacht Posted at: 2016-09-06T17:50:13.843Z Reads: 150

```
I have a scorpion set up but my enertion vesc fried, replacment should be shipped soon, powering it with the space cell pro 10s4p.<img src="/uploads/db1493/original/3X/c/e/ce8bb8684a33aeca04908019a6ae53679f93da71.png" width="281" height="499">
```

---
## \#6 Posted by: er2528 Posted at: 2016-09-06T18:33:55.046Z Reads: 137

```
very nice!  what kind of peaks loads do you draw on that setup?  Do you have it geared on the tall side?  How's the acceleration?
```

---
## \#7 Posted by: Dornacht Posted at: 2016-09-06T18:55:32.531Z Reads: 137

```
I don't remember the peak power, the vesc only lasted 4 min so don't have to many specs, geared 15/36-enertions 12mm belt setup. I did not reach top speed, the vesc broke when I was costing, so I have no clue what the problem was. The calculations say it should reach 30mph. It's very smooth
```

---
## \#8 Posted by: er2528 Posted at: 2016-09-06T20:10:06.485Z Reads: 132

```
Hm. I was hoping to maybe catch a baseline there.


Also, courier just showed up with the rear brackets.  Pulled them out of the packaging and.... Cheesy class A70 stainless fasteners? into an aluminum stressed member?  No!, Bad! Go sit in the corner!

Fished out some class 10.9 plated steel socket caps and 10.9 prevailing torque all metal locknuts.  I keep a spare, well, everything from fasteners to bearings to anything and everything electrical.  In several cabinets fulled stocked with goodies.  Stainless steel has its anti-corrosion advantages, but it hasn't very good tensile or shear strength.  And threading into aluminum without an anti-seize compound is simply asking for it to gall.  Will replace these elevator bolts too, maybe spring loaded heims or something of the like.

These 100mm wheels are making this a bit troublesome, going to have to revisit this.  This thing needs to be just like 5mm bigger :/<img src="/uploads/db1493/original/3X/0/c/0ce059e80b037363624ee6624f1b324df004e337.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/d/d/dd7f5c56e07f8af2b683bdda1b3bf43e1deb8478.jpg" width="281" height="500">

(EDIT: the piercing bolts it came with aren't long enough to reach the hanger. lol.)
```

---
## \#9 Posted by: Mobutusan Posted at: 2016-09-06T20:21:52.601Z Reads: 113

```


That sounds like a crazy build! I’d definitely be interested to see how you deal with the different kv/gearing, etc. 

I’m just about ready to start assembling a 4wd hybrid 12s setup with 90kv @Hummie hubs in front and dual belt driven Torqueboards 6355 230kv motors in rear, and 4x TB 12s ESCs. My plan is use a handheld tachometer to match the unloaded rpms of both drivetrains, adjusted for wheel size differences (80mm/83mm). I’m not sure if there is a better way to sync the rolling speeds, so I’ll be curious to see how your build progresses.
```

---
## \#10 Posted by: lox897 Posted at: 2016-09-06T20:23:51.612Z Reads: 113

```
For science right? Can't wait to see how it looks in the end.
```

---
## \#11 Posted by: er2528 Posted at: 2016-09-06T20:43:48.917Z Reads: 118

```
Well, if there is interest now...

Here's some little neat stuff I made for it.  A little pedestal mount gauge cluster that sits on top of the board.  Each meter for front motors, rear motors.

Edit: Just realized this was a pic before I decided on the dual voltage setup.  Needs reworking

Been doing this stuff for quite some time...when that retarded Fast Furious show came out like 10 (?) ish years ago, friends tried sticking me with that stupid "mad scientist" moniker in my garage.  Irritated the piss out of me.  Just reminded me how long it's been.<img src="/uploads/db1493/original/3X/a/b/abcd9dac7ec18e77ca3d92f49247542e86676105.jpg" width="375" height="499"><img src="/uploads/db1493/original/3X/c/2/c2ad83a890e6f212cf3d6cfe9422b306141271e4.jpg" width="592" height="500">
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-09-06T21:35:44.157Z Reads: 103

```
Wow bad ass!
```

---
## \#13 Posted by: Mobutusan Posted at: 2016-09-06T22:12:37.608Z Reads: 91

```
That's a pretty cool setup. I've got a single watt meter that mounts on the nose, but it's not as pretty as yours. I like the spring mounting system. I just wish they were more visible during the day, so I could see real time amp draw, voltage sag, etc. I made a hood over the screen and mounted a gopro (yi camera) so I can record the real time readouts. It's not a perfect system, but it works for now. Got any pics of the deck and other components you're going to use?
```

---
## \#14 Posted by: er2528 Posted at: 2016-09-06T22:49:45.410Z Reads: 88

```
Yeah, you've the right idea anyway.  To read these meters, you have to bend down and squint to get a read while in motion.  There is a seller, or sellers for that matter, on ebay selling these wireless DC ammeters.  I thought this was on point, so i bought one with the idea of strapping it to my wrist.  Fantastic idea, but don't bother.  Those meters are crap.  The feedback left from those who successfully had gotten it to work reported like a 70% error in measurement.  Mine didn't even work at all.

Well, the only other pertinant asthetic changes were some chrystal pieces acquired from that Svorsky (sp?) and backlit with blacklight LEDs.  Looked sinister, but I don't think I took any snaps of that one.  I've torn this thing down so many times already I forget what revision this is.  I may need a new deck, though.  I'm using a 300 amp marine battery switch to power everything on and off (and to ensure there's not switchgear failures).  I drilled I decent sized hole for access to the flag handle in the board.  I went overboard :frowning:
```

---
