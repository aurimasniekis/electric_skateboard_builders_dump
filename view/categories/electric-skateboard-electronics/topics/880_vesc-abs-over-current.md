# Vesc abs_over_current

### Replies: 13 Views: 2548

## \#1 Posted by: DougM Posted at: 2016-01-03T04:39:37.829Z Reads: 189

```
I have built up several VESC's with the 4.10 boards and they all work great, except on the last build I switched from Turnigy motors to a Tacon motor.  All the configuration steps go great, but when I go to actually drive the thing it spins up and then generates  an ABS_OVER_CURRENT fault and shuts down.  I can then drop down to brake (PPM, current with brake) and come back up and it will repeat the spin up and the error.

Has anyone seen this error before?  My next step will be to swap out the Tacon for another Turnigy and see if it is an issue with my particular motor.

Thanks,

DougM
```

---
## \#2 Posted by: EnertionSupport Posted at: 2016-01-03T05:08:03.057Z Reads: 189

```
Do you have some more info, such as;

Motor KV?
What battery Voltage?
What Motor Current Limit do you have set?
Did you run the motor detection on the Tacon motors?
```

---
## \#3 Posted by: DougM Posted at: 2016-01-13T02:59:08.035Z Reads: 171

```
Yes, sorry for the delay in response, I've been ditzing around with this and have found some interesting things.

The error is not consistent across VESC's.  I have 3 of them (one from Chaka, 2 home built) on various motors and have found that of the ones I've tried none of them drive the Tacon correctly, but the one that was consistently generating the over_current error drives Turnigy 5055-280's just fine but does not drive the Turnigy 6374's (either 168 or 192).

However, the one I got from Chaka and one of the home built's drives the 6374's just fine.  So that's interesting.

So I shelved the Tacon for now so this isn't all that critical, but I'd still be happy to spend some time diagnosing it for the greater good.

In answer to your questions

1) The Tacon is a 5335-245KV

2) the longboards are all 6C LiFePo, but the bench is running 24v lead acid, so should be comparable

3) the current limit I set was either 35 or 40A both accel and regen.  I think I also tried it with the default 60A, but can confirm if need be.

4) I did run the current detection on the Tacon and set appropriately.  I'm running BLDC, not FOC.  I think I know what I'm doing since I was able to setup the other motors successfully but it's possible I don't know what I'm doing.

Lastly, the Tacon was an unloaded bench test.

Thanks,

DougM
```

---
## \#4 Posted by: cmatson Posted at: 2016-01-13T03:10:05.275Z Reads: 156

```
very strange indeed.. 

Do you think it could have anything to do with your battery setup? the vesc can run a 50mm turnigy motor, but once you step up to a 63mm tacon or turnigy, it stops working. The most confusing this is that 2/3 vescs are workings, and they all behave strange with the tacon! 

I would say maybe it's a faulty motor (rare, but not completely unheard of), but the vesc doesn't work with your turnigy 6374 either...

I'm not sure, just throwing out ideas here. 

Maybe @psychotiller has some thoughts as I know he has been using the tacons for quite some time now. Although I'm not sure he has set up a board with a VESC yet, or if he is still using castle esc's.
```

---
## \#5 Posted by: psychotiller Posted at: 2016-01-13T03:21:44.659Z Reads: 152

```
I finally set up a dual with vesc's, but I used 2 63mm g160s. I haven't paired a tacon to a vesc yet. I'm going to order another vesc soon though and I'll give it a try.
```

---
## \#6 Posted by: cmatson Posted at: 2016-01-13T03:45:32.574Z Reads: 152

```
[quote="psychotiller, post:5, topic:880"]
used 2 63mm g160s
[/quote]

ahh yes, for some reason I thought they were tacons..
```

---
## \#7 Posted by: psychotiller Posted at: 2016-01-13T03:54:50.541Z Reads: 147

```
Maybe I'll switch them out with tacons if I get board enough.
```

---
## \#8 Posted by: chaka Posted at: 2016-01-13T15:17:20.828Z Reads: 143

```
@DougM

I have encountered this a few times and it usually a faulty motor connection or insufficient current from the power supply.  If you end up blowing a chip in your quest let me know and I will get you up and running again. You seem to have the skills though. :wink:
```

---
## \#9 Posted by: DougM Posted at: 2016-02-15T03:16:51.680Z Reads: 134

```
Update, I've got the Tacon running on one of the homebrew VESC's.  I did update the firmware so it's possible that there was some tweaking under the hood that affected the problem.  (which is to say I didn't change anything that would explain it).

Unfortunately it's been raining here nonstop so I haven't had a chance to get it on the road.

I'm looking forward to the 1.12 rev of the HW so I can start playing with FOC.  @Chaka, are you going to have these available soon?

Thanks,

DougM
```

---
## \#10 Posted by: chaka Posted at: 2016-02-15T14:14:47.294Z Reads: 129

```
Yes we have implemented the 4.12 revision. We are currently using a larger capacitor at C18, doubling the capacitance as per Vedder's instruction.
```

---
## \#11 Posted by: solarcross Posted at: 2016-07-07T06:49:09.243Z Reads: 111

```
I haved tried a Tacon 245Kv (10s) on an e-bike with reduction..
HW 4.7 - FW 1.2 - twist throttle
worked flawless - amazing fun!!!

updated to 2.18 - motor detection wouldnt go properly..
loaded XML from 1.2FW pressed the (throttle) arrow key in BLDC tool and boom  - DRV failure..
```

---
## \#12 Posted by: DougM Posted at: 2016-07-07T15:04:57.875Z Reads: 98

```
I wonder if the 2.18 firmware was ever intended for the 4.7 hardware.  Any experts here can talk to this?
```

---
## \#13 Posted by: elkick Posted at: 2016-07-07T15:17:23.370Z Reads: 96

```
Yes it is. But it's not a good idea to load an old xml file from FW1.2 into FW2.8, there have been to many changes in between. And if motor detection is not working it could be that the DRV was dead before that anyway.
```

---
