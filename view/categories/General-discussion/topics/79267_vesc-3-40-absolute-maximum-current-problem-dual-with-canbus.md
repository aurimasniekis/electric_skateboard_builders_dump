# Vesc 3.40 absolute maximum current problem dual with canbus

### Replies: 18 Views: 306

## \#1 Posted by: sayekim Posted at: 2018-12-28T22:00:35.340Z Reads: 93

```
I think I found a bug in fw 3.40 which is pretty dangerous and I need someone else to confirm this or disprove it. 

I was running a dual escape with default firmware 3.40 with canbus connection and every time it throws an over current fault when the combined value of my motor amps reads over 160amps which is the maximum absolute maximum current value that can be set per esc. 

This should not happen. 

It should only give this fault when one esc reads 160amps and not the combined value of both esc. 

This problem has now thrown me off of my board once almost twice. 

I just downgraded the firmware to 3.38 and now it no longer gives me this fault all though I have only tested on a very short distance and not gone over the 160amps combined motor amps value for a longer time due to living room testing. 

Either way here are some data from metr. 

FW 3.40 with fault. 

https://metr.at/r/t2xxi

FW 3.38 no fault

https://metr.at/r/255aM

If you got data with dual esc, fw3.40, and canbus that shows combined value of motor amps above 160 without an over current fault that would be great. 

Or even better perhaps someone can just look at the source code and spot the error in fw3.40 that would create this behavior?

Somewhere that shows shut off when sum motor amps esc 1+2 >= max current esc 1 = true or some shit like that. 
Not really a coder evidently.
```

---
## \#2 Posted by: sayekim Posted at: 2018-12-30T22:36:21.173Z Reads: 74

```
Okay I can confirm now that the over current fault is definitely gone with firmware 3.38 and even running 100 amps per motor. 

https://metr.at/r/vJ5Qc

Still no one with fw 3.40 running 80 or 80+ amps getting over current failt with full acceleration?
```

---
## \#3 Posted by: taz Posted at: 2019-01-14T13:51:11.000Z Reads: 59

```
I got an ABS OVER CURRENT fault yesterday.
Motor amps were set at 70 each
VESC6 escs.
I may try fw 3.38 to see if this cures it.
Does anyone have the android version of the previous vesc tool? I have opened and closed my battery box so many times the last week :roll_eyes:
```

---
## \#4 Posted by: sayekim Posted at: 2019-01-14T14:00:27.081Z Reads: 59

```
I guess your abs max current was still set on the default 130amps too?
```

---
## \#5 Posted by: taz Posted at: 2019-01-14T14:15:09.547Z Reads: 59

```
No, the standard value for the VESC6 is 150A.
```

---
## \#6 Posted by: sayekim Posted at: 2019-01-14T14:32:44.944Z Reads: 54

```
Firmware 3.40 no matter which hardware you use will have abs max current default value of 130 A. 

Hardware doesn’t determine the default value.
```

---
## \#7 Posted by: linsus Posted at: 2019-01-14T14:48:43.062Z Reads: 48

```
Even if you set current draw for each individual? As in 70A on one and 70A on one? (=140A). 

Never happened for me
```

---
## \#8 Posted by: Friskies Posted at: 2019-01-14T14:51:03.208Z Reads: 45

```
Change your firmware to no_hw_limits and adjust the max current value as you see fit?
```

---
## \#9 Posted by: sayekim Posted at: 2019-01-14T15:13:48.863Z Reads: 41

```
What are you implying?

Can you be more specific?

I suppose you mean if I write the value individually? and via vesc tool on a desktop?

I did write them individually on the desktop vesc tool but don’t remember for sure if I used the same value for testing to trigger it. I think I did too. 

I think it’s irrelevant since the mode writing with the metr app works fine for 3.38 and I can do 100 amps per vesc without triggering the over current faults but with 3.40 not.
```

---
## \#10 Posted by: linsus Posted at: 2019-01-14T15:19:10.491Z Reads: 36

```
Yes thats what I mean, configuring all thresholds per individual. Given the escs will never draw the exact same current, can you tell which one produces the error?

The problem is usually the other way around, you have a battery that can tolerate 60A draw so you set 60A as setting on both escs(120A :D ) i did that a few times but quickly realised it was wrong. 

Currently I run Innovas on a gear setup with pretty low thresh, never had the over current trigger. Dont have that many hills to climb here however. I had to occacional passanger on it tho...
```

---
## \#11 Posted by: taz Posted at: 2019-01-14T16:28:51.836Z Reads: 35

```
It seems we may be both correct (or wrong, depending how you look at it).
First of all it turns out my absolute max current value was set at 130A.
However I was certain it was 150A.
The reason is that the pc version of the VESC tool I used to setup the vescs the last time has 130A as a default value.
The android version however I had used previously has 150A as a default value.
Here is a short clip showing my programmed values and then the default values when using the android version.

https://youtu.be/M4CNfAyFnAc
```

---
## \#12 Posted by: sayekim Posted at: 2019-01-14T16:38:58.138Z Reads: 30

```
I’m not sure. Good question. I imagined with a canbus connections that the master esc is the one that will report the fault but how to know if the fault didn’t come from the slave. 

Don’t know enough to say how this works. I suppose it would be best if each esc saves its own faults of course but since in this case the fault is caused by the combined value it raises questions.
 
Neither esc here should report a fault since neither one reaches 160 amps or more.
```

---
## \#13 Posted by: linsus Posted at: 2019-01-14T16:42:55.351Z Reads: 29

```
Do you run NRF-remote by any chance? Could remove CAN all together and run them from same remote to see which one triggers.
```

---
## \#14 Posted by: sayekim Posted at: 2019-01-14T17:14:00.778Z Reads: 29

```
That would defeat the whole problem I think since I believe it only happens with a canbus connection. 
The data shows almost 160 amps and then the fault triggers. That data is from metr pro where it adds the amps values of both esc. 

Without the canbus connection it would only register the amps of one motor and so it would not be triggered since it will hit the amp limit of 80amps while abs max current is set to 160.
```

---
## \#15 Posted by: linsus Posted at: 2019-01-14T17:27:23.367Z Reads: 31

```
You'd still get fault code on one of the esc with proportional threash values. I don't think this is a CAN issue.
Just tossing balls here to help you debugg
```

---
## \#16 Posted by: sayekim Posted at: 2019-01-14T18:17:12.571Z Reads: 27

```
I don’t get it. What and how do you think I should test?

Give me an example with values.
```

---
## \#17 Posted by: Santino Posted at: 2019-01-15T05:29:58.977Z Reads: 24

```
Check all of the motor wires that are connected to the Vesc, if one is a little loose, you will probably get ABS Over Current Fault...I use shrink tube on each wire to avoid that... Hope is just that...
```

---
## \#18 Posted by: Gerrycorrado Posted at: 2019-05-27T18:54:42.576Z Reads: 14

```
@Deodand i was pointed to this topic. Might help you too?
```

---
