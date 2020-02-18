# Remote issues/vesc random braking. Who else had this problem?

### Replies: 10 Views: 787

## \#1 Posted by: MysticalDork Posted at: 2017-11-29T17:06:13.220Z Reads: 95

```
So, I've got my build pretty much finished. I'm using a GT2B remote with a 3d printed enclosure, with dual vesc6 from trampa. 

I've had the board do random hard braking, as well as sluggish throttle response/latency. I've checked, and I have no faults registered on either vesc, and the problem is not readily reproducible. It just randomly happens, and I tend to eat pavement as a result.

Have any of you folks had similar issues and fixed them? If so, how?!

I'm considering getting a nano-X remote or similar, and I'd like your opinions on which has the most reliable connection. I'm hoping for something with a second/third channel accessible through a button, for controlling my headlights, and hopefully with PWM or PPM output, since that's what my vescs/headlights/taillights are set up for.
```

---
## \#2 Posted by: MrHappy Posted at: 2017-11-29T17:44:58.441Z Reads: 90

```
This remote works great, https://www.ebay.com/itm/2-4GHz-Radio-Binding-Plug-Remote-Controller-Receiver-For-Electric-Skateboard/192223853151?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649
```

---
## \#3 Posted by: Exiledd_Top Posted at: 2017-11-29T18:04:44.148Z Reads: 85

```
I've had this problem long long ago If u look at my account u can find that post had the same problem with gt2b control all u have to do is discount the receiver and rebind the receiver never had any problems every again
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-11-29T19:59:58.567Z Reads: 78

```
Thanks, I'll try that when I get home.
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-12-10T04:29:21.960Z Reads: 61

```
Well, I thought I had it fixed, but it just threw me off again today. Getting really sick of this crap. Considering selling/parting out the board and using the funds/parts to build an ebike.
```

---
## \#6 Posted by: Clonkex Posted at: 2017-12-10T22:21:50.067Z Reads: 49

```
What have you tried to debug it so far? Things I would try:

- Different receiver/remote set
- Either find a way to log battery voltage over time and check what it's doing at the moment of faceplant, or set the voltage cutoff very low or off in the VESCs
- If you have the VESCs connected with canbus, check/disable your traction control settings and/or remove the canbus and connect the receiver to both VESCs
- Do the motors make any odd noises when the braking happens?
- Try just one VESC/motor at a time and see if the issue is specific to one VESC
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-12-10T22:28:11.338Z Reads: 47

```
There are no noises when braking.

I haven't got a second rx/tx but I can order one. What do you recommend?

I'm fairly confident that it wasn't a battery voltage thing. Two times ago, the battery was nearly full (4.1/cell) and the most recent time it was 3.85/cell. I have my cutoffs set to 3.2 and 3.0, so I shouldn't be anywhere near those.

I do have canbus/traction control, I guess I can swap to a Y splitter. I was under the impression that that was potentially more harmful for the vesc6 though, so I'm a little reluctant.
```

---
## \#8 Posted by: scepterr Posted at: 2017-12-10T23:01:30.201Z Reads: 42

```
Could traction control do that?
Are you running sensored?
I'll have a bunch of nanox Tuesday if you want one
```

---
## \#9 Posted by: Clonkex Posted at: 2017-12-10T23:27:31.256Z Reads: 42

```
@MysticalDork I don't know what controllers are available and good, but I was hoping you might have had a second one laying around that you could test with. Hmm... well probably the controller/receiver is fine and you should start with other steps.

I also was fairly confident about battery voltages with my X-Car ESC (as was @TeslaAlex in [this thread](http://www.electric-skateboard.builders/t/motor-esc-brakes-under-hard-acceleration/39222/38?u=clonkex)), but it turned out the that voltage cutoff was causing sudden braking under hard acceleration even with the cutoff on its lowest setting. It might be worth testing this theory even if it seems very unlikely.

I don't know much about the VESC6. Do you have any source for a splitter being harmful? I'd be interested to hear more about that.

@scepterr I have no idea if traction control could do that, but the goal is to simplify the setup as much as is humanly possible, then if the problem doesn't come back, progressively reintroduce the extra features until one of them causes the problem to reappear. It's more difficult if the problem is one that tries to kill you at random of course, but you gotta start somewhere :P
```

---
## \#10 Posted by: MysticalDork Posted at: 2017-12-11T00:05:41.627Z Reads: 39

```
The strangest thing is that it always seems to occur at periods of non-peak load. Either gentle throttle for cruising, or gentle braking for maintaining a sane speed downhill. It never seems to happen under hard acceleration (I sat on the board and did full throttle/full brake slams from 0-15mph and back like a dozen times with zero trouble. )

I seem to remember seeing somewhere that the pins dedicated to canbus have better protection/are more robust against higher voltages than the PPM pins. I'll look around and see if I can find the source.

One interesting thing about traction control is that if I hold one wheel and give the board some throttle, the other wheel spins slowly (as it should, according to the maximum ERPM difference setting) and the wheel that is held gives a constant torque, trying to accelerate to match the other wheel. 
If I hold the other wheel, however, the torque given by the held wheel isn't constant. It fluctuates as the other wheel spins.
```

---
