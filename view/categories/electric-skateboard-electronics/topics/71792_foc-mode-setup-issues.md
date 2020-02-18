# FOC mode setup issues

### Replies: 10 Views: 549

## \#1 Posted by: chrismccabe Posted at: 2018-10-20T10:10:04.299Z Reads: 135

```
Hi guys!

I've been playing around with setting op FOC mode this morning but for some reason I can't get it to run smoothly. Having issues with startup cogging of the motor.
I've done all that jazz measuring the resistance, inductance and flux linkage in VESC tool. Also played with the settings for Openloop mode, but can't get it to start properly.

https://www.youtube.com/watch?v=lq5gCN9n_wc

Setup is:
Aerodrive 6374 192kv motor (Sensorless)
Maytech 50A VESC (FW:3.38 HW: 410)
10S3P li-ion pack

Any ideas on how to fix this? The reason why I want to use FOC mode is that it would make the board a bit more silent.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-20T11:13:34.454Z Reads: 119

```
ok so foc is great for if you're running sensored motors on either a vesc 6 or focbox. running a vesc 4.2 on foc unsensored will most definitely blow up your speed controller. it's just too hard on the components. use bldc and don't set battery amps over 40a. motor amps you can push to 70a i think
```

---
## \#3 Posted by: Michael319 Posted at: 2018-10-20T16:27:46.901Z Reads: 105

```
Cogging is normal for unsensored. Change to sensored to get rid of the Cogging. Or push to start.
```

---
## \#4 Posted by: brenternet Posted at: 2018-10-20T18:38:19.169Z Reads: 93

```
[quote="mynamesmatt, post:2, topic:71792"]
running a vesc 4.2 on foc unsensored will most definitely blow up your speed controller
[/quote]

This is a pretty broad statement. There are loads of people running 4.12's on foc without issue.
```

---
## \#5 Posted by: bigben Posted at: 2018-10-20T18:58:32.928Z Reads: 88

```
Did you do motor detection without the belt on?
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-10-20T21:32:32.310Z Reads: 76

```
[quote="brenternet, post:4, topic:71792"]
loads of people running 4.12’s on foc without issue.
[/quote]
when i say this i mean stock where there is no cooling and no heat sink
```

---
## \#7 Posted by: Fiori Posted at: 2018-10-20T21:36:45.452Z Reads: 74

```
It's actually pretty well known that 4.12 without direct FET's will blow on FOC. 

Cogging will occur in both BLDC and FOC settings modes if you are running and sensorless motor.
```

---
## \#8 Posted by: dareno Posted at: 2018-10-21T02:26:42.270Z Reads: 71

```
Not a great idea foc with normal vesc 4.12  and maytech definitely don't like it.  

[quote="chrismccabe, post:1, topic:71792"]
I want to use FOC mode is that it would make the board a bit more silent.
[/quote]
The scream of a sk3 motor is a beautiful noise
[quote="mynamesmatt, post:2, topic:71792"]
don’t set battery amps over 40a.
[/quote]
I would be checking the type of battery before telling someone to set the max battery amps.  ie; if thats a 10s3p from diye or a chinese prebuilt then the bms will go poof at 40 amps.
```

---
## \#9 Posted by: mynamesmatt Posted at: 2018-10-21T03:32:06.560Z Reads: 66

```
@dareno (i assumed he'd know the Max draw of the pack)
```

---
## \#10 Posted by: chrismccabe Posted at: 2018-10-21T08:29:07.784Z Reads: 60

```
Built the pack myself, VTC6 cells and a 60A Battery Supports BMS. Should be fine. Have been running it at 50A battery settings.
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

What is exactly the issue then? Why does it blow up the FET's?
Also I did think the cogging should be solved with running it open loop to start with (weird name, as the FOC should also run open loop seeing as I'm not using a hall sensor, encoder. Or is the current and voltage measurement of the stator done properly enough with some added observer to derive RPM from that data?)

Didn't do the detection without the belt. It would be slightly of but not significantly it seems. Even saw Benjamin do these measurements with the belt still attached.

And yes the sound of the SK3 really does sound futuristic. I also like it. But want to be a bit more stealthy. :slight_smile:
```

---
