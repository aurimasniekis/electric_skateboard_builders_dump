# VESC shuts off when under load

### Replies: 23 Views: 250

## \#1 Posted by: RedLiquid Posted at: 2020-02-01T02:21:18.177Z Reads: 62

```
Hey guys, I'm trying to figure out why my entire setup loses power whenever I am hard on the throttle.  So far, I've replaced my vesc (FOCbox DRV fried so I replaced it with a Flipsky 6.6) and nothing changed.  I also tried bypassing the BMS for discharge, and that didn't solve the problem either.  In addition, it seems as if the whole vesc loses power, so no fault codes are shown.  Would this be an indication that my motor is causing the shutoffs?  Before this started happening, I *did* drop the motor on the floor while I was tinkering with it, but I opened it up and did not see any signs of shorting.
```

---
## \#2 Posted by: MysticalDork Posted at: 2020-02-01T02:25:28.805Z Reads: 60

```
Post some pictures of your wiring and setup.
```

---
## \#3 Posted by: RedLiquid Posted at: 2020-02-01T02:40:11.856Z Reads: 58

```
Here are some images of the setup (it's a bike!), and the wiring diagram that I made prior to starting the build.


![55551898_571782746634296_2785313968225255424_n%20(1)|666x500](upload://qrEjN6xApwcSveyObvGPlAnqNqK.jpeg) ![54430330_1039076759611554_1940242297622888448_n|666x500](upload://sLqJB5GhfQnyxVMLTwhe4712YHh.jpeg) ![55560371_583533618790122_6778405622355329024_n%20(1)|666x500](upload://xJer1hnHOWJuY4nMFYfIKVF5xTH.jpeg) ![54430471_309886276270896_1173625888378454016_n%20(1)|375x500](upload://nlYHvh6bxMbtalzLUoptRADLlAE.jpeg) 
![asdf|690x376,100%](upload://AuG9CUQnFtTUzfFXWGlMIfbIihM.png)
```

---
## \#4 Posted by: MysticalDork Posted at: 2020-02-01T02:50:02.264Z Reads: 53

```
And you tried shorting B- to P-, and it made no difference?
```

---
## \#5 Posted by: RedLiquid Posted at: 2020-02-01T03:21:46.070Z Reads: 52

```
Yes, exactly.  There was no change in the shutoffs after I made the B-/P- short.
```

---
## \#6 Posted by: MysticalDork Posted at: 2020-02-01T03:29:10.542Z Reads: 51

```
I've got nothing.

If it's a vesc issue, you should be able to get a fault reading out of it using the console.

If it's a BMS issue, then bypassing should have fixed it.

If it's a wiring or connector or battery issue, it should present as voltage sag, not an abrupt cutoff.
```

---
## \#7 Posted by: RedLiquid Posted at: 2020-02-01T03:47:26.005Z Reads: 42

```
The only thing I can think of is a bad motor?  I dropped the motor from about 4ft onto the ground before these problems started happening, although I did not see any obvious damage.

My theory is that under high RPM & current, something from the motor causes my VESC to freak out and reboot, but I want to confirm if that is even a possibility before I spend any money on a replacement motor.
```

---
## \#8 Posted by: MysticalDork Posted at: 2020-02-01T03:54:46.098Z Reads: 41

```
Even if it is damaged and causes vesc faults, it should still result in a fault code that you can read in the terminal.
```

---
## \#9 Posted by: RedLiquid Posted at: 2020-02-01T03:58:32.100Z Reads: 41

```
I see.  I'll try to reproduce the shutdown again this weekend and double check the fault logs.
```

---
## \#10 Posted by: mynamesmatt Posted at: 2020-02-01T09:46:05.941Z Reads: 37

```
maybe just try updating firmware and redoing your motor detection? that may help?
```

---
## \#11 Posted by: beckw Posted at: 2020-02-02T01:07:49.312Z Reads: 32

```
Hi RedLiquid,

I had the same on my Mountainboard. I've setup my battery, motor and VESC that it can deliver over 60 Amps by 42V. After a while on high load my motors stopped. I know it can't be the motor because both of them cut off so I measured the voltage during under load and I measured a significant voltage drop. Unfortunately the Vesc has quite a high voltage cut off default setting but during your configuration you can switch this feature off or set the cutoff voltage lower. In my case I've disabled this feature because my BMS is doing this already. Since then my Mountainboard drives very nice.
Hope that helps
```

---
## \#12 Posted by: RedLiquid Posted at: 2020-02-02T04:02:53.888Z Reads: 28

```
Hey guys I tried a few of your suggestions, but I've had no luck.

[quote="MysticalDork, post:8, topic:105717, full:true"]
Even if it is damaged and causes vesc faults, it should still result in a fault code that you can read in the terminal.
[/quote]

I tried reproducing the shutdown earlier today to check for fault codes, but there were no codes registered "since startup".  I believe the entire VESC powers down/reboots when I lose power, so every time the error occurs, any fault codes are erased from memory.  I verified this by using the "Print Threads" command in vesc tool; it tells me that the vesc has only been awake for the duration after the shutoff.  Right now it seems like a game of Schrodinger's cat, because I don't have any way to view the codes. : (

[quote="mynamesmatt, post:10, topic:105717, full:true"]
maybe just try updating firmware and redoing your motor detection? that may help?
[/quote]

I tried this multiple times, but it doesn't appear to change the odd behavior of the vesc.

[quote="beckw, post:11, topic:105717"]
the Vesc has quite a high voltage cut off default setting but during your configuration you can switch this feature off or set the cutoff voltage lower. In my case I’ve disabled this feature because my BMS is doing this already
[/quote]

I just checked, and I have my voltage cutoff set to 3.0v per cell, which seems to be the lowest value that anybody recommends.  I have not tried to disable the cutoff feature entirely yet, but I believe if this was the issue, my fault log would show it?
```

---
## \#13 Posted by: MysticalDork Posted at: 2020-02-02T10:27:01.738Z Reads: 22

```
[quote="RedLiquid, post:12, topic:105717"]
I have not tried to disable the cutoff feature entirely yet, but I believe if this was the issue, my fault log would show it?
[/quote]
Even if the low voltage cutoff is set too high and causing faults, the vesc hardware itself can operate down to like 12 volts, so unless you're somehow dragging your battery voltage all the way down to <12v, the vesc should still remain powered. That's what's confusing me.
```

---
## \#14 Posted by: professor_shartsis Posted at: 2020-02-02T12:25:48.256Z Reads: 20

```
make sure your absolute max current setting is a lot higher than the motor and battery current setting limits and the low volt cutoff is properly set if that doesnt work try lowering the motor current limit setting and adjusting the temp cutoff settings
```

---
## \#15 Posted by: RedLiquid Posted at: 2020-02-03T02:03:55.242Z Reads: 20

```
I was finally able to read some fault codes today, after testing the motor with no load.  It says I have ABS_OVER_CURRENT, but I'm not sure which setting I need to change.  I attached my fault code and vesc settings below.

**Battery: 12s5p li-ion**

**Motor: Maytech 6374 190kv, 60A cont, 3550W max**

**VESC: Flipsky fsesc 6.6**


![Capture|399x500](upload://bzb7rsdPhSSY0IX5wg3ONdHjilJ.jpeg) 
![CAP2|690x193](upload://vQ0dGu4BJeBS5I7rLy2A0xHg8VE.jpeg) 

![CAP3|690x158](upload://iWv7wVDMEzIvSIRoNkXXZ4d8iqY.jpeg)
```

---
## \#16 Posted by: RedLiquid Posted at: 2020-02-03T02:37:44.769Z Reads: 19

```
Just got another fault code, this time showing a current spike of 217A (wtf!).  Not sure what is causing the current to jump like that.

![CAP4|482x265](upload://7MUBiTn5dUAhOH5DkDnlMm1kGUY.jpeg)
```

---
## \#17 Posted by: MysticalDork Posted at: 2020-02-03T02:53:44.275Z Reads: 21

```
Well, that's something at least. I would suggest trying to shorten your battery and motor wires as much as possible, as inductive current/voltage spikes can cause issues like this.

You might also try limiting your ERPM to ~60,000, and see if that affects things.
```

---
## \#18 Posted by: RedLiquid Posted at: 2020-02-03T03:49:25.333Z Reads: 18

```
**Update: got a new fault code.**  I repeated the same test, but this time I used my bike brake to simulate a heavy load.  The vesc rebooted itself and this code popped up:


Also, I had my ERPM limited to 48000 already. (my motor emits a high pitched noise at >50000erpm)
![cap5|645x340](upload://tSqV9DtdyTDDNCkppBbcVS054Sw.jpeg)

edit: Did some research on this code and it looks like it doesn't really tell us anything other than the fact that the vesc has, in fact,  rebooted. x_x
```

---
## \#19 Posted by: professor_shartsis Posted at: 2020-02-03T12:11:33.161Z Reads: 15

```
try lowering your motor current limit setting

ps whats the bat voltage, kv and # of magnets in your motor. i don’t think you want the erpm limit set below what the motor will naturally do
```

---
## \#20 Posted by: RedLiquid Posted at: 2020-02-03T16:23:19.660Z Reads: 14

```
Will try that later today.  Also really? I never knew the erpm shouldn't be set too low.  My battery is 12s, so 43.2v nominally.  The motor is 190kv & 14 magnets.  It naturally reaches 52000erpm but I had it limited to 48000.
```

---
## \#21 Posted by: professor_shartsis Posted at: 2020-02-03T20:33:09.620Z Reads: 14

```
i’d limit it 70000 erpm or above and lower the motor current limit, lemme know if that works
```

---
## \#22 Posted by: RedLiquid Posted at: 2020-02-05T03:46:52.044Z Reads: 13

```
Changed erpm limit to 70,000 and reduced motor current limit to 40A.  Vesc is still crashing due to massive current spikes (fault log showed 300A spike).

I'm highly suspicious that the motor might be faulty; I ordered a replacement motor and will test everything again later this week.
```

---
## \#23 Posted by: RedLiquid Posted at: 2020-02-07T21:01:50.097Z Reads: 9

```
I finally figured it out!  Changing the motor did not solve the problem, so I decided to take a look at all my wiring.  Turns out there was a cold solder on my loop-key, and it got worse over time because I was pulling it after every ride.  This caused the vesc to lose power whenever I drew too much current.  I repaired the bad solder and everything seems to be running smoothly now.
```

---
