# Abs over current from dead stop

### Replies: 26 Views: 1382

## \#1 Posted by: Eboosted Posted at: 2017-04-10T06:16:24.145Z Reads: 145

```
I'm getting this error more often now, it only happens if I accelerate from a dead stop at 20% of throttle, VESC reboots itself and I don't have any control from the remote. If I accelerate very smoothly it accelerated with no error. 

Can I fix this issue by upgrading the C18 and C26?
```

---
## \#2 Posted by: sl33py Posted at: 2017-04-10T06:26:51.028Z Reads: 145

```
I've had this and it was a simple adjustment of settings to fix...  What voltage and your setup info?

What is your configuration and settings specifically?  Screenshots of the BLDC tool will help.

GL!
```

---
## \#3 Posted by: Eboosted Posted at: 2017-04-10T06:36:06.119Z Reads: 140

```
Motor max: 80A
Battery max: 40A
Motor min: - 60A
Battery min: - 10A

Start up boost: 0.020

Cutoff start: 30V
Cutoff end: 28V

Runing 10S4P on dual belt with VESC
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-04-10T06:40:45.943Z Reads: 129

```
And what is your absolute max and your drive mode? FOC or BLDC?
```

---
## \#5 Posted by: Eboosted Posted at: 2017-04-10T06:42:09.807Z Reads: 127

```
Absolute max: 130A 

I'm runing BLDC
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-04-10T06:49:15.291Z Reads: 124

```
post screenshots with your other settings, there might be something else. Nothing wrong with the things you posted. Also did you check your wiring? Might be a small short somewhere.
```

---
## \#7 Posted by: kptheinventor Posted at: 2017-04-11T22:54:16.159Z Reads: 107

```
I believe I am also having this issue with my vesc. Does your vesc occasionally do this when trying to brake? And you loose your brakes for a second?
```

---
## \#8 Posted by: sl33py Posted at: 2017-04-11T23:17:06.391Z Reads: 104

```
@kptheinventor - this is what i experienced on my test bench.  After sharing my configuration settings, i adjusted the voltages slightly and the abs overcurrent error was resolved.  It was something simple like adjusting the voltage up a few volts to not error.  When it errored it would lose communication for a second or two and give me 3 red blinks (iirc).  After adjustment - no more problem.

Not like the OP who has this when starting from a dead stop - that's different and more concerning...
```

---
## \#9 Posted by: kptheinventor Posted at: 2017-04-11T23:18:46.326Z Reads: 104

```
I can never get my back to do this error when it's plugged into my computer. It only happens when I'm physically out riding it. Do you know what settings you adjusted?
```

---
## \#10 Posted by: Eboosted Posted at: 2017-04-12T05:32:11.042Z Reads: 103

```
Well I'm still having the issue, so no setting has been useful yet. Hope someone could give me some suggestions
```

---
## \#11 Posted by: PXSS Posted at: 2017-04-13T11:38:05.176Z Reads: 98

```
Have you checked your battery? A bad weld could mean spikes in current maybe. 

Otherwise its a bad vesc
```

---
## \#12 Posted by: Eboosted Posted at: 2017-04-13T14:10:50.024Z Reads: 92

```
I have an exact same setup on a different board but the issue does not happen there, the only difference is on the issue-board I have a 15/36T on 97mm wheels and on the non-issue-board 16/40T on 100mm wheels. 

I uploaded the latest @ackmaniac firmware v2.54 yesterday, I'll test it today and report back.
```

---
## \#13 Posted by: Eboosted Posted at: 2017-04-13T14:15:40.215Z Reads: 90

```
[quote="PXSS, post:11, topic:20705"]
Have you checked your battery? A bad weld could mean spikes in current maybe
[/quote]

Thanks for the suggestion, I'll take a look at the battery today
```

---
## \#14 Posted by: Eboosted Posted at: 2017-04-14T04:57:37.134Z Reads: 90

```
I think you were correct, my battery is sagging too much, even on the bench with no load. 

I'll take off the enclosure tomorrow
```

---
## \#15 Posted by: kptheinventor Posted at: 2017-04-21T02:21:24.469Z Reads: 82

```
Are you still having this problem?
```

---
## \#16 Posted by: Eboosted Posted at: 2017-04-21T04:27:15.923Z Reads: 80

```
Hey man! yes, I'm still having the issue, but it only happens when I press the throttle on a hill from a dead stop or on launches very harsh terrains
```

---
## \#17 Posted by: kptheinventor Posted at: 2017-04-21T04:46:55.708Z Reads: 78

```
Did the voltage sag have any effect on anything?
```

---
## \#18 Posted by: Eboosted Posted at: 2017-04-21T04:52:39.002Z Reads: 76

```
I don't think this has anything to do with voltage sag at all. In fact my sag was perfectly normal, my capacity tester has a very high sample rate so that's why I incorrecrlyt though I was having sag
```

---
## \#19 Posted by: kptheinventor Posted at: 2017-04-21T05:05:48.344Z Reads: 77

```
Ah alright
```

---
## \#20 Posted by: Eboosted Posted at: 2017-04-21T05:09:15.314Z Reads: 78

```
I'd suggest to use hybrid mode, just a JST connector and solder it to the sensor wires on the motors, you won't have this issue as manu times as today and a much smoother launch from a dead stop.

It's only 3 bucks

http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Connector-with-Wire-X-10-Sets-TW-/141757606740?hash=item2101696b54:g:W9EAAOSwgQ9V3m4W
```

---
## \#21 Posted by: kptheinventor Posted at: 2017-04-21T05:22:15.469Z Reads: 77

```
Do I have to have a sensored motor? I have a sensorless. And is that cable just a replacement cable for the jst?
```

---
## \#22 Posted by: Eboosted Posted at: 2017-04-21T05:22:42.497Z Reads: 76

```
[quote="kptheinventor, post:21, topic:20705"]
ave a sensorl
[/quote]

Yes, sorry you need a sensored motor
```

---
## \#23 Posted by: ninja Posted at: 2017-09-28T08:25:54.005Z Reads: 51

```
@Eboosted did you solved your error issue ?
```

---
## \#24 Posted by: darkkevind Posted at: 2017-09-28T10:08:53.800Z Reads: 49

```
Interested too...
```

---
## \#25 Posted by: Michaelj1 Posted at: 2018-05-16T16:38:35.743Z Reads: 30

```
I think I’m having this issue too. I have dual sensored motors, I’m running in FOC mode with traction control. VESC firmware 3.38. I assumed it was just traction control but it seems to happen over rough terrain when accelerating hard or giving it a lot of throttle on hills. It doesn’t happen a lot, it’s only happened to me like 2 times, but my friend was going up a hill and he said it went full brake on him(might be an unrelated issue)
```

---
## \#26 Posted by: Michaelj1 Posted at: 2018-05-16T16:39:42.058Z Reads: 30

```
I think my friend just hit a rock tho because I’ve never had the board go full brake on me(yet)
```

---
