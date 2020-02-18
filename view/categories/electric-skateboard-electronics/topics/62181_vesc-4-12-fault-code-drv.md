# Vesc 4.12 fault_code_drv

### Replies: 22 Views: 769

## \#1 Posted by: xilw3r Posted at: 2018-07-18T07:54:35.239Z Reads: 121

```
Topic name change edit: I guess I burned my DRV chip, question is why. I was doing some testing (probably dumb), I was slowly rolling backwards on my board and I was pushing the throttle and brakes to see what will happen, first few times it just seemed to help roll backwards faster when i pressed throttle and brakes worked fine. Then boom and no more response from remote. After a restart it tried to move a bit and then again nothing.
In vesc tool I get the FAULT_CODE_DRV, when I try pressing the throttle.  But I get no red flashing led on the vesc or anything, it lights up blue as per usual, just no bright green led when I press on the throttle.


By the way, the original issue was simply me not having enough motor amps to push my fat ass any faster than walking speed. Even with 1:5 gearing 30 motor amps werebasically nothing...damn some one needs to go on a diet.

-------------------------------------------------------------------

Hello people

First tests of my "board" on the way, and a weird issue presents it self.

When I am off my board and give it some throttle, it does a burnout. All good there.

When I get on the board and push off for a rolling start and give it throttle it has absolutely no power, throttle at full, rolling at slightly above walking pace, motor running pretty damn loud and vibrating. Then if I get to accelerate a bit more somehow, the sound changes becomes smoother, sounds like when the board is going on its own. And the throttle appears. I did not push it above this "crossover" point much because I am a noob rider and it feels like it can rip the board from beneath my feet if I give it full power.


As I understand, the vesc is running at a duty cycle mode at low rpms and then switches to bldc. My question is, why the hell is it so severely underpowered at low rpm that it barely accelerates? Anyone know which setting governs this? Perhaps the minimum ERPM limit (one of the three detection settings)

Stats, sry I do not have how to log my data currently.:

Voltage during testing ~40V, vesc cut off start at 33 end at 30
Motor amps 60, Motor breaking amps -40
Battery amps 45, braking battery amps -20

edit: I increased motor amps and battery amps significantly before this test since I thought it was the reason for no power.. I was wrong.

I can post full settings later when I am home

edit2:   I have another weird issue, when vesc is connected through USB I can not move the motor with the arrow keys anymore. It worked before, then after latest motor detection It does not respond anymore, it just clicks in place, no current goes through, even if the settings allow for a lot.

edit3: I get a lot of abs overcurrent faults when using my remote to give throttle.. read that this might mean a bad DRV chip? But how come it"kind of" works then
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-07-18T08:05:05.291Z Reads: 103

```
Try recalibrating your remote
```

---
## \#3 Posted by: xilw3r Posted at: 2018-07-18T08:19:31.561Z Reads: 102

```
The remote does not seem to have issues with the ppm signal. All looks fine there.. no erratic response, etc
```

---
## \#4 Posted by: Andy87 Posted at: 2018-07-18T12:40:42.879Z Reads: 95

```
check all your connections.
ABS over current can come from a bad solder join.
I had some the same issue once my xt90 anti spark was plugged in only by the half.
I can imagine it could be something the same if the motor cables not right soldered or not fully plugged inside each other.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-07-18T12:56:25.286Z Reads: 87

```
Does a motion detection work flawlessly without errors?
```

---
## \#6 Posted by: xilw3r Posted at: 2018-07-18T13:00:59.805Z Reads: 86

```
@TarzanHBK Yes it does. But only when I set the current to 10A. On low current it just clicks in place or does not speed up properly.

@Andy87 I checked all connections, everything is solid. Unless it really is a badly soldered pin on one of the smd components on the vesc, I did not check those... only what I did my self
```

---
## \#7 Posted by: TarzanHBK Posted at: 2018-07-18T13:06:31.010Z Reads: 82

```
hook the vesc on the tool, start the board and look at the realtime tab.
Does it come with strange spikes or is everything normal.
Check realtime data from your remote if you find some faulty data there.
```

---
## \#8 Posted by: pennyboard Posted at: 2018-07-18T14:10:37.284Z Reads: 77

```
Are you sure its not a mechanical problem? You said the motor vibrates and makes noise, could the belt be slipping at low speed?
```

---
## \#9 Posted by: xilw3r Posted at: 2018-07-18T14:28:09.383Z Reads: 76

```
Its definitely the motor, belt is not loose (or over tightened). Its just a cogging sound, I would not pay much attention to it, but I really expected to have (at least some) power available at really low speeds. I will try making minimum ERPM for which to use integrated bldc much lower and see if it has effect when i get back home
```

---
## \#10 Posted by: xilw3r Posted at: 2018-07-19T07:30:32.181Z Reads: 65

```
Ok, so there are no really weird spikes, except short ones at the very start and end of the motor movement.
A more interesting thing, when I had the board connected to usb and was just trying to press full throttle while holding it from movement, it either stutters in place, which is fine, but I had two weird shut downs while doing this, the whole system shut down and I needed to reboot through the e-switch, looks like the BMS might be at fault here. The data screen on the vesc tool indicated a "low voltage" error.

Oh and i did some acrobatics while holding my laptop in hand connected to vesc via usb and me riding it full throttle. Which is less scary than it sounds because my current never breaks something like 6A in the data. I am pretty sure the BMS I have is messing stuff up.. somehow
```

---
## \#11 Posted by: pat.speed Posted at: 2018-07-19T07:52:31.128Z Reads: 59

```
Is it sensorless or does it have sensors? If it does try unplugging them and see if it works
```

---
## \#12 Posted by: xilw3r Posted at: 2018-07-19T08:04:37.172Z Reads: 55

```
Running sensorless.

What a "small detail" I forgot to mention :) I will probably try bypassing the BMS to see if my assumption is correct. Though now I need to make a new power cable..
```

---
## \#13 Posted by: pat.speed Posted at: 2018-07-19T10:36:09.735Z Reads: 50

```
I doubt it would be the bms. Did you say you are running hybrid mode? Something about it switching when picking up speed?
```

---
## \#14 Posted by: xilw3r Posted at: 2018-07-19T11:03:23.764Z Reads: 43

```
Nevermind that, I suppose the "speed up" happened when I was on a very slight downward slope. I could not reproduce any "speed up" today and the current to the vesc tops out at 5-7 A range. How can this be caused by the vesc if it is not the bms ? 

I will know for sure if its the bms later today I hope
```

---
## \#15 Posted by: pat.speed Posted at: 2018-07-19T11:23:14.268Z Reads: 41

```
[quote="xilw3r, post:1, topic:62181"]
the vesc is running at a duty cycle mode at low rpms and then switches to bldc
[/quote]

This is what I was meaning. Are you referring to having it in hybrid mode? It should be set to sensorless in the Vesc setting
```

---
## \#16 Posted by: xilw3r Posted at: 2018-07-19T11:38:56.081Z Reads: 45

```
My motor is set up as sensorless. I do not really understand what hybrid mode you are talking about.

As I understand the VESC always runs on delay commutation (i thought its called duty cycle mode), when it is at low ERPM (below the minimum you define in the settings), because the back emf is not high enough to do the integration for bldc sensorless mode.

I really don't understand how a stupid BMS can be limiting the current it sends out so severely, I thought they do not even have such possibility, only hard shut down when the current is above the critical value.

But on the other hand, how the hell can VESC decide to take in such a low ammount of current when it is programmed for much much more.
```

---
## \#17 Posted by: pat.speed Posted at: 2018-07-19T11:40:44.335Z Reads: 43

```
Yeah I’m not sure how it could be the bms, but it’s work a check just in case
```

---
## \#18 Posted by: ElskerShadow Posted at: 2018-07-19T12:03:55.171Z Reads: 45

```
I had exactly the same problem a few months back, I even had underpower fault in the vesc.
I couldn't find the issue but it was the bms, I replaced it and the issue was gone.it was a bestech 12s 80a bms
```

---
## \#19 Posted by: xilw3r Posted at: 2018-07-20T13:34:52.247Z Reads: 43

```
I had hopes after reading your reply, but alas, it is not the bms

Gotta be the vesc that is busted... well, shit.
```

---
## \#20 Posted by: xilw3r Posted at: 2018-08-01T19:28:40.146Z Reads: 35

```
Vesc wasnt busted, motor amps were too low. By the way, in real time data plot, the motor current is an average or something I suppose? Because it never gets to the limit of what is set in the settings. 30 motor amps in the settings show up as~15 -20 amps of motor current in the real time plot.


fault code drv is the new kid on the block now... and vesc is busted for sure :(
```

---
## \#21 Posted by: xilw3r Posted at: 2018-08-02T13:14:11.427Z Reads: 26

```
Weirdness continues.

a colleague looked at the drv, it seemed that one leg might have come loose from a cold solder, so he soldered it,  I connected to test, at start no issues, no red lights, no errors. Give it throttle with the arrow keys, movement is happening, the green signal led shines full bright as normal. Press the arro key again, green led starts flashing rapidly, no movement, terminal throws up a bunch of drv errors.... But I HAD MOVEMENT. After a few tries it starts to try and move again, the same rapid green led blinking happens and more drv faults.

I suppose the drv can still be busted... just in some weird way perhaps?

I could really use some input here.. thanks
```

---
## \#22 Posted by: ThermalM16 Posted at: 2018-08-05T04:01:17.455Z Reads: 21

```
Hi @xilw3r yes, that can happen. I've run into quite a number of very weird issues during all of the repairs I've completed on VESCs. There are a few things you'll want to check, namely the resistors on your FETs and your FETs themselves in your case. But the DRV will likely need to be replaced if it's throwing errors.
```

---
