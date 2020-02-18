# Motors are &ldquo;choking&rdquo; when I input the throttle to go/accelerate

### Replies: 13 Views: 301

## \#1 Posted by: kchxaz Posted at: 2019-07-25T16:29:41.752Z Reads: 98

```
Sorry if this has been addressed before, I wasn't getting any related results from my keywords, "choking" probably isn't the best descriptor one could use...

Anyways, I went from using a Vanpro mini-remote to the new flipsky vx1 remote. I set it up PPM style as I couldn't get UART to work no matter how many times I tried.

Problem is that from a stopped condition or, and this is the one that worries me, from a partially going speed (like 5-10 mph) there are times, way more often than I would like, where one of the motors does not turn properly, it just stays in an at rest condition, obviously when you are already moving this is an issue as it drags one side of the board to a stop, or tires to. I don't particularly want to go head over heels because of this one day either.

I have never experienced it with manufactured e-boards so that's why I am guessing it's something to do with programming the VESC. When I give it instantaneous full throttle (I hate doing this for wear and tear on the belts and stuff) it doesn't seem to occur, only when giving it slow gradual throttle and it almost always does it when I accelerate this way...

Does anyone know if there is something in the VESC setup that controls this, IDK, "phenomenon", for lack of better term?
```

---
## \#2 Posted by: briman05 Posted at: 2019-07-25T16:39:49.423Z Reads: 93

```
Did you do the motor detection? And are your belts too tight/too loose? Also did you set the max and the min for the controller?
```

---
## \#3 Posted by: kchxaz Posted at: 2019-07-25T19:27:13.970Z Reads: 82

```
Yes, I ran through the motor detection part of the motor setup and also the min/max detection of the remote during the app setup...It seems to happen most when there is no load against the motors, such as when I flip the board upside down, it will always do the motor "choke" at this time, sometimes even both motors simultaneously...
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-07-25T19:54:08.645Z Reads: 75

```
Are you running sensors or sensorless? BLDC or FOC? Sensors help a lot with rough starting like this, as does FOC (But only if your ESC can handle it)
```

---
## \#5 Posted by: kchxaz Posted at: 2019-07-25T23:34:34.754Z Reads: 56

```
Using FOC, It's what the VESC tool starts when you use the wizard to setup motors. Motors do not have sensors on them. Belt drive non-sensored.
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-07-25T23:53:34.368Z Reads: 52

```
Strange. Maybe try redoing the motor detection? Or switch to BLDC, do that detection (It's different) and then switch back?
```

---
## \#7 Posted by: kchxaz Posted at: 2019-07-26T00:32:18.098Z Reads: 44

```
Yeah, sure, what could it hurt to try BLDC? If It works then might even stay on it, right? Unless there is a something negatively adverse such as possibly extra battery drainage difference, for example. I'm not sure I even know what the differences are supposed to be between BLDC and FOC really...lol
```

---
## \#8 Posted by: Hummie Posted at: 2019-07-26T01:25:17.701Z Reads: 39

```
See if the electrical resistance numbers are similar between the motors on the bldc tool.

Are the motors the same temp?
```

---
## \#9 Posted by: Santino Posted at: 2019-07-26T06:50:56.232Z Reads: 34

```
I wil try this:
Run the latest Vesc tool firmware on both Vescs
Detect can bus
Run motor detection with can bus (both motors should doit at the same time)
Set PPM and UART
Go to PPM and  do de mapping process (you need to get full percentage to both sides)
Set positive ramping at 0.10
Set max amps cutoff at 10amps 
Then set throthle curve natural (linear)
Go for a ride...If you do not like it, go to Throttle curve and move to exponential, and ad at firs 5 % positive value (do not mes with break, just acceleration), you might need more juice at the beginning...
Keep in mind that BDLC it is not as soft as FOC, of course I would run parameters on BDLC if a have no sensors...
I would also activate the can bus to check that the other Vesc is at the same settings as the masters vesc...
Hope it helps...remember to NOT mess with the breaks, that it is dangerous...
```

---
## \#10 Posted by: kchxaz Posted at: 2019-07-27T01:19:48.647Z Reads: 22

```
I like where your thinking is going with this. I thought something similar the way it happens under certain current loads...I just didn't know with what to start looking at to change the proper setting. Amps makes total sense with the way the motor chokes at certain loads...Thanks I'll let you know how it goes...One last quick question: I should do this in FOC or BLDC? Why?
```

---
## \#11 Posted by: Santino Posted at: 2019-07-27T02:24:10.246Z Reads: 19

```
BLDC, detect parameters....Because you are running sensorless.... But here you have more info:
https://www.electric-skateboard.builders/t/the-difference-between-motors-commutation-bldc-vs-foc-trapeziodal-sinosuidal/3002
```

---
## \#12 Posted by: Hummie Posted at: 2019-07-27T02:46:03.741Z Reads: 18

```
I think amp will only help the motor from chocking from a standstill, in that if it doesn't have enough amps it will cog.  if youre getting weird or no responses while moving the settings aren't going to fix it.  did you try the tests on the bldc tool to see if it passes or shows strange numbers?
```

---
## \#13 Posted by: banjaxxed Posted at: 2019-07-27T11:06:22.000Z Reads: 16

```
Can you log it on the desktop with the vesc tool?
```

---
