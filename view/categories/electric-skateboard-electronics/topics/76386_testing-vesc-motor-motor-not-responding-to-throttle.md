# Testing VESC/Motor, motor not responding to throttle

### Replies: 13 Views: 129

## \#1 Posted by: RazzleDazzle Posted at: 2018-11-28T18:20:41.406Z Reads: 39

```
Hey Guys, i just finished setting up my dual VESC (from TorqueBoards).  I had it setup to a 12v5A power supply to do the initial setup with the VESC Tool.  Everything seems good after i flashed the firmware.  I also setup the 2.4ghz remote and paired it (the light was solid blue once paired).  

once all that was squared away, i connected the VESC to one of the 6355 190kv motors to see if the throttle would work.  Unfortunately it didnt.  Im wondering if its because i'm using only a 12v5A power supply and its not enough juice to spin it or if its something else.

I didnt do the motor setup wizard yet because I dont have my batter pack finished (10S4P).  Is that potentially the issue?

Also, this may sound stupid, but the 3 cables coming from the motor, do they have to be connected to the VESC in a particular way?
```

---
## \#2 Posted by: torqueboards Posted at: 2018-11-28T18:22:25.101Z Reads: 38

```
Probably hitting low voltage cut off at 12V so you won't be able to detect. You either need to change this or use your full pack. No need to run it with a power supply. Just wait for your full voltage.
```

---
## \#3 Posted by: RazzleDazzle Posted at: 2018-11-28T18:24:02.882Z Reads: 37

```
I just want to check the vesc are working ok.  BTW, im going to run it sensored, so do i select the hall sensors?
```

---
## \#4 Posted by: torqueboards Posted at: 2018-11-28T18:25:57.646Z Reads: 37

```
I'd test on BLDC first and run sensored later after you've successfully programmed in BLDC. More moving parts when running sensored. Run motor detection but you'll have to change your low voltage cut off if you use 12v.
```

---
## \#5 Posted by: RazzleDazzle Posted at: 2018-11-28T18:35:06.238Z Reads: 35

```
So i finished the motor setup, it spun the motor and spit out whatever values.  Im running it on on that 12v supply.    Once i disconnected the usb, and pressed the throttle, the motor still isnt turning.  The voltage settings are 12v and 10v
```

---
## \#6 Posted by: torqueboards Posted at: 2018-11-28T18:39:52.490Z Reads: 33

```
Make sure your app confit is configured properly.
```

---
## \#7 Posted by: RazzleDazzle Posted at: 2018-11-28T18:43:46.143Z Reads: 30

```
i stepped through the app wizard like the how to on your site was.
```

---
## \#8 Posted by: RazzleDazzle Posted at: 2018-11-28T18:48:56.958Z Reads: 27

```
Actually i realized that i never clicked "apply" on the "current no reverse".  Now the remote works.  one thing though is when i press the throttle, it it spins for a little bit then stops even though im still holding it
```

---
## \#9 Posted by: torqueboards Posted at: 2018-11-28T19:34:04.358Z Reads: 23

```
Not too sure what that one is.. Probably better off emailing us as we need more details on what you're using. Check the tutorials if you haven't seen it already.
```

---
## \#10 Posted by: RazzleDazzle Posted at: 2018-11-28T19:36:16.724Z Reads: 22

```
I messed around with it some more, when i pull the throttle slow it spins.  If i grip it fast, i notice the lights on the vesc go red then it seems liek the power cuts out.  Not sure if its because the power supply im using (12V5A)
```

---
## \#11 Posted by: torqueboards Posted at: 2018-11-28T19:37:02.247Z Reads: 24

```
Possibly, yeah. Try when you get your battery pack. You've tested it works already.
```

---
## \#12 Posted by: RazzleDazzle Posted at: 2018-11-28T19:39:28.534Z Reads: 24

```
Yup, will do.  Im assuming when i get my battery pack, i just need to go through the motor setup wizard again and input the proper values for the 10s power pack.  Then write the firmware to each of the VESC's again right?  Just plug each one in and clikc the write motor config?
```

---
## \#13 Posted by: torqueboards Posted at: 2018-11-28T19:44:52.725Z Reads: 23

```
Yeah, you'll need to set all the values up again for 10S and motor detect again, write, etc. :smile:
```

---
