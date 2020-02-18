# Remote question

### Replies: 15 Views: 929

## \#1 Posted by: Mattmccrary8 Posted at: 2017-11-15T15:54:24.379Z Reads: 169

```
I’m currently using a Winning V2 remote that works great but i Want a remote with 2 speed modes. Since my 12s dual 6374 190kv motor is way to much torque for most. I’d like to have two speed modes on it. Will the benchwheel remote provide that? Or can I do that with my remote now ?
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-11-15T16:00:58.889Z Reads: 164

```
i just bought 20 of the new maytech remotes and i'm about to list them tonight. They have two speed modes and a much smaller receiver, a much much more ergonomic feel, and i'm basically in love with them. Cruise control is gone, but so is the awkward size. IT fits in a pocket and even tells you if the board is powered on (with a seperate indicator light instead of just saying its paired)

Also the cable is a usb micro instead of mini and its a normal cable that can also be used to connect your FocBox to your bldc tool. Its not that stupid long special cable from the Steeze.
```

---
## \#3 Posted by: Mattmccrary8 Posted at: 2017-11-15T16:11:04.566Z Reads: 153

```
Texting you now
```

---
## \#4 Posted by: oriol360 Posted at: 2017-11-15T18:09:44.069Z Reads: 137

```
Hey,

I carry both remotes with two speed modes.
I made a quick video to show off some key differences but they are both great remotes.

https://youtu.be/6PF8t7TN3Rc
```

---
## \#5 Posted by: mmaner Posted at: 2017-11-15T21:01:01.057Z Reads: 105

```
If you don't want to buy a new remote, and I'm not saying you shouldn't, you could install a Bluetooth HM-10 and use the @Ackmaniac firmware to setup modes.
```

---
## \#6 Posted by: Jinra Posted at: 2017-11-15T21:05:29.149Z Reads: 102

```
just fyi the winning v2 DOES have two "speed" modes
```

---
## \#7 Posted by: Battosaii Posted at: 2017-11-15T21:12:30.518Z Reads: 104

```
Really? Cause mine doesn't change speed it just turns on and off channel 2, I'd like speed modes on my Raptor cause it's a bit too much for people that have never ridden esk8
```

---
## \#8 Posted by: Jinra Posted at: 2017-11-15T21:17:04.523Z Reads: 102

```
Yes, but it doesnt the same thing as with any PPM remote with multiple modes, in which it limits the pulse width. For the v2 it limits it to about 70/-70%. And just so we're on the same page this is the remote I'm referring to. For this reason it doesn't limit speed so much as it limits current, which in turn will limit speed in conditions where supplied current doesn't overcome load.

https://www.ebay.com/itm/Mini-Remote-Controller-w-Receiver-Electric-Skateboard-Longboard-2-4GHz-US-Seller/172832554248?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m1438.l2649

The Enertion nano-x is the same as the remote above.
```

---
## \#9 Posted by: Battosaii Posted at: 2017-11-15T21:20:04.721Z Reads: 100

```
I have that same remote I'll have to test it tonight to see if there is any difference in acceleration, I know on my V1 for sure it has only 1 speed mode mode. Im at work but I have my board in the car I will try it out in the parking lot later
```

---
## \#10 Posted by: Jinra Posted at: 2017-11-15T21:26:33.921Z Reads: 97

```
yea v1 only has 1 mode, v2 has 2 modes. Full throttle is down position on the switch below the throttle, and 70% throttle is up position.
```

---
## \#11 Posted by: Battosaii Posted at: 2017-11-15T22:10:22.491Z Reads: 81

```
I'd be interested to see if I've been riding in slow mode all this time.... I did try the switch during testing on a bench with no load but saw no difference
```

---
## \#12 Posted by: Jinra Posted at: 2017-11-15T22:11:45.844Z Reads: 77

```
because the raptor and raptor 2 don't use duty cycle control, it's all current control. On the bench it'll look the same in almost any throttle position since you only need a couple amps to ramp to full speed.
```

---
## \#13 Posted by: Battosaii Posted at: 2017-11-15T22:30:33.049Z Reads: 66

```
It's on my mono diy board but it's all Raptor parts anyway lol ah I want to try it now
```

---
## \#14 Posted by: Jinra Posted at: 2017-11-15T22:33:41.282Z Reads: 67

```
If you set PPM values on the VESC in slow mode you'll still have 100% throttle range. The 2 modes only have effect if you set PPM values based off "fast" mode on the remote.
```

---
## \#15 Posted by: Battosaii Posted at: 2017-11-15T22:36:05.576Z Reads: 67

```
Thanks for the valuable info!
```

---
