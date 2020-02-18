# How to get top speed Vesc 6.6plus

### Replies: 9 Views: 195

## \#1 Posted by: Woeggi Posted at: 2019-11-20T19:00:43.920Z Reads: 72

```
Build thread: https://www.electric-skateboard.builders/t/landyachtz-falcon-36-tourque-boards-direct-drive-10s5p-carbon-fibre-enclosure-building-something-dangerous/103988?u=woeggi

GPS measured top speed was 47km/h. This is already bonkers fast, but according to my math the wheels should spin with around (90kV Motor, 37V, 110mm Wheels) 80km/h (no load). Not to be greedy but i thought it would do over 50 at least. I guess this has something to do with the VESC. The realtime data shows something between 110 and 120km/h without load. (which cant be right). The obvious settings like wheel diameter, direct drive and so on are ok. I suspect the motor poles not being the assumed 14. Does someone know more than me here? How do i get the most speed out of my vesc? If its not easy please point me in the right direction to read up on it.
```

---
## \#2 Posted by: murdomeek Posted at: 2019-11-20T19:28:29.802Z Reads: 67

```
use a 12s battery
```

---
## \#3 Posted by: Woeggi Posted at: 2019-11-20T19:35:57.848Z Reads: 63

```
Well... obvoiusly ;)
The question should be: Are 47km/h expected on this kind of hardware or too low/high. 
Secondly how do i correct the ridiculus real time data from the vesc?
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-11-20T20:55:19.540Z Reads: 56

```
Just because a motor is "90kv" doesn't actually mean it is that high, I have "190kv" motors that measure 151kv...so between that and resistive loss you'll loose speed.  I think BLDC has a higher top speed than FOC, and it'll only go full speed at full battery (but you'll get a few bolts of sag at full throttle).  Also the max duty cycle is only 95% for VESCs by default

Hope that helps
```

---
## \#5 Posted by: BluPenguin Posted at: 2019-11-20T21:57:59.850Z Reads: 54

```
What is your amp draw at top speed? Do you have a wiring bottleneck or wrong limits set on vesc? 47km/h should pull roughly 20-30 battery amps on flat ground with that setup.
```

---
## \#6 Posted by: Woeggi Posted at: 2019-11-21T13:13:24.097Z Reads: 42

```
@ZachTetra I did not know motors are rated in a guesstimated way and show sort of wrong values. Thx for info!  I read up a little on FOC vs BLDC and will give BLDC a try (just for achievable topspeed as it is less efficient). What max duty cyle really is still kinda eludes me. At the moment  I think 100% duty cycle would mean you are pumping power through the fets 100% of the time (or at least keep them open)? Lots of heat if not destruction could be the cause( is it safe if the fets reached max temp around 40° ish at the moment). What do you mean by bolts of sag? (sorry no english native) Is it that the battery will pretty soon come down to its nominal voltage (like 37V ish) after a recharge.

@BluPenguin The set battery limit is 75A at the moment. Motor limit is around 60 per motor (from the wizard) Series wiring is in 10AWG if that was the suggestion? Still need to watch the amp draw at max speed under load. (scaaaary) 

Do you have a suggestion how to correct the realtime speedreading of the vesc? Only solution i would have is measure the tyrespeed manually with a high speed camera, do some math and play with the motor pole number until it overlaps.
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-11-21T13:27:30.230Z Reads: 37

```
Duty cycle reduces the voltage going to the motors, 70% duty cycle will send a voltage to the motors that is only 70% of the battery voltage

I meant voltage sag, if you pull a lot of amps for a long time the battery voltage will read a little low

With a full battery you will lose 2v to 95% max duty cycle and possibly another 2v to sag, plus the first 2 volts are drained very fast anyways so for speed calculations you just want to use the nominal voltage for the most part
```

---
## \#8 Posted by: BluPenguin Posted at: 2019-11-21T21:00:44.643Z Reads: 31

```
FOC vs BLDC should not have a drastic increase in top speed, maybe a few km/h. Check your speed/RPM in the vesc tool with no load on the board. You should be getting over 3000 RPMs on the motors while it's on the bench free spinning. 36v * 90kV should give you 3240 RPMs. If you're not getting full speed rpms while freespinning, either your kV rating is way off, or there is an erpm limit in the vesc that you don't know about. If you are getting full spin speed without weight on the board, then you'll need to log your power draw as you're riding it to figure out where the power constraint is.
```

---
## \#9 Posted by: Woeggi Posted at: 2019-11-26T19:23:34.746Z Reads: 16

```
Sooo.. back after a few days and some testing.
At 39,8V and no load i get 42000ERPM. As i don't know the exact pole number i will keep it at erpm(but i suspect 28. At around 40V that would mean 3000RPM with my 90kv motor 3600 would be the calculated result )
With load at top speed i got 34000ERPM. I got about 50km/h out of it. (14polepairs check out with this)

A couple things that stood out: The measured max current is around 60 amps (during acceleration), but my settings say 75A Battery current.
Also: directly after the max speed runs acceleration was like in low voltage mode.

Motors are set at 60ish amps each. Can it be that the battery setting is only for the one vesc that i am reading out? 

That would mean i am drawing 120A total out of the battery. It would also explain a quite big voltage drop from 39V to just around my set limit of 34V and therefore the "low" top speed. 

If i get around it i will test again tomorrow with lower set maximum current and maybe disassemble the motor to get clearance about the polenumbers.
```

---
