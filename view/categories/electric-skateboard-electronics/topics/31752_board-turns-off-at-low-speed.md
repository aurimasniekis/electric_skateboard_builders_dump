# Board turns off at low speed

### Replies: 18 Views: 644

## \#1 Posted by: Pickwick Posted at: 2017-08-29T16:11:17.547Z Reads: 74

```
Hello. 

I have some problems with my board. 
When I drive at low speeds (5mph) the board drives nice, but when I give it a little more it dies.. 
I have a 10S BMS mounted which I don't think is the problem, I think it has something to do with the VESC. 

Can someone see my mistake?<img src="/uploads/db1493/original/3X/f/6/f6b90ae43c6c1b531b3d90036e95cf03cb60a3be.PNG" width="690" height="407"><img src="/uploads/db1493/original/3X/e/d/ed55d20dae072a34b043567980bcf959414c8de0.PNG" width="690" height="406"><img src="/uploads/db1493/original/3X/d/d/dd269b0cb1275dc2e31fe18ed6d9f99605d35d6a.PNG" width="690" height="408">
```

---
## \#2 Posted by: Alanhunt123 Posted at: 2017-08-29T16:17:23.117Z Reads: 63

```
Go out and make the problem happen once more. Then, without disconnecting power, connect your VESC to the computer and go to the "Terminal" Tab. Then type in "faults" in the terminal, and report back if you find any faults.

Good luck!
```

---
## \#3 Posted by: Pickwick Posted at: 2017-08-29T17:21:07.594Z Reads: 52

```

I have just tried, but the power is being shut down when it happens, so the VESC gets shut down aswell. 
I really have no idea of why it suddenly just turn off the power.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-08-29T17:26:28.441Z Reads: 48

```
I would circumvent the BMS and go direct connection from the battery discharge to the VESC so you can take that out of the equation, don't see anything obviously wrong standing out in your settings from here.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-08-29T18:02:28.256Z Reads: 44

```
What the Brand of your vesc ? And in the tab "advance" the "Max Ramp Current at 1Khz" is way to high... maybe you should reflash your firmware with a genuine one.
```

---
## \#6 Posted by: Pickwick Posted at: 2017-08-29T19:36:52.074Z Reads: 36

```
It's a maytech VESC. Do you think it could help if I lowered it?
```

---
## \#7 Posted by: Pickwick Posted at: 2017-08-29T19:37:42.576Z Reads: 36

```
Well that sucks..
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-08-29T19:38:30.573Z Reads: 37

```
It should be at 0.04 If I remember.
```

---
## \#9 Posted by: wafflejock Posted at: 2017-08-29T19:42:06.306Z Reads: 37

```
Yeah I read on a thread somewhere that there was a bad firmware at some point where if you saved on that config page it would change the value in the box and if you saved again you would end up with it getting multplied by 10 each time or something like that.  Pretty sure it was a bug in the firmware.
```

---
## \#10 Posted by: Pickwick Posted at: 2017-08-29T19:44:00.373Z Reads: 35

```
And mine is 50... Wtf
```

---
## \#11 Posted by: Pickwick Posted at: 2017-08-29T19:44:37.692Z Reads: 35

```
I hope that's not the case..
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-08-31T11:01:53.466Z Reads: 31

```
Also what BMS are you using? Do you have a link?
```

---
## \#13 Posted by: Pickwick Posted at: 2017-08-31T12:16:54.670Z Reads: 26

```
I have fixed the problem now. It was a minor mistake. 

The BMS I'm using is this: http://bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-31T12:24:54.586Z Reads: 25

```
You definitely have the ramp step bug. 
Good catch @JohnnyMeduse
Still it sounds like your bms is entering protection mode for some reason.
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-08-31T13:41:39.110Z Reads: 18

```
Thats an 8s BMS - not good if you try to use it with 10S :fire:
```

---
## \#16 Posted by: Pickwick Posted at: 2017-08-31T13:42:44.874Z Reads: 17

```
Whups.. I send the wrong one. It's the same though, just with 10S ;)
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-08-31T13:45:18.729Z Reads: 16

```
good :smiley:
So you fixed the issue? What was it?
```

---
## \#18 Posted by: Pickwick Posted at: 2017-08-31T13:49:46.332Z Reads: 18

```
I think it was because I only had 30% left on the battery.. Cause when I charged it up, the problem went away  :p
```

---
