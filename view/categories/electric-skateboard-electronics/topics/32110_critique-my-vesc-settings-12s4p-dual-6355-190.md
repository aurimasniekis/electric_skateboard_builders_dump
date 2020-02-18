# Critique my VESC settings 12s4p dual 6355/190

### Replies: 10 Views: 1521

## \#1 Posted by: irishthriller Posted at: 2017-09-02T19:37:15.526Z Reads: 226

```
12s4p dual mechanical 6355/190; 16:36T; 90mm wheels

I have very little background knowledge on these things and I was hoping the kit I bought from DIY would be more 'plug and play'. I think these are these only three screens screens I altered settings on. Please provide feedback on my settings before my FIRST RIDE! Thanks!

<img src="/uploads/db1493/original/3X/a/3/a394c1c1d3209daf19f8dd07d71a0aefaf87b777.png" width="690" height="429"><img src="/uploads/db1493/original/3X/8/f/8f8dc90c02a92500f4cce38bc301148af328c99d.png" width="690" height="420"><img src="/uploads/db1493/original/3X/1/d/1d058d99bfd927006b2f8c0bc56c00811ef6ad38.png" width="690" height="422">
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-09-02T20:38:03.699Z Reads: 209

```
Well for one, you need to make sure you set the BEMF coupling and integrator limit to the values provided by your motor detection.  It looks like you ran motor detection but didn't put the values in the fields.  

Once you use the values provided by motor detection, make sure you hit write configuration. 

It also looks like your battery cutoff is not right, it should be up in the 40's for 12s, (3.5x12 for cutoff end and 3.6x12 for the cutoff start. Again, once you change the cutoff, hit write configuration. :)
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-09-02T21:13:02.389Z Reads: 203

```
For a 12S4P which is obviously a LiIon Battery i recommend a cutoff start at 3.0V a cell and a cutoff end at 2.8V a cell. So in your case 36V for start and 33.6V for end. 
@ShutterShock your recommended settings would fit for a LiPo Battery.

And if you have a dual drive you can raise your batter min to -8V and if you have a ingle drive you can go up till -16V because each cell can handle 4V. If you ask me you can even go a little higher to -10 or -20 in case of a single drive because those currents will only be for a few seconds.
```

---
## \#4 Posted by: irishthriller Posted at: 2017-09-03T01:33:59.620Z Reads: 192

```
Thanks. How's this? Anything else? <img src="/uploads/db1493/original/3X/1/e/1eac41f3424b8e150ffb1f955a44dcbf939d0149.png" width="690" height="424"><img src="/uploads/db1493/original/3X/c/9/c9c0c03b94a6dc8df349c2081c7b727014a702aa.png" width="690" height="423"><img src="/uploads/db1493/original/3X/c/5/c55bec81a99df06b7acd742b37b0f23ec6cc11f5.png" width="690" height="416">
```

---
## \#5 Posted by: ShutterShock Posted at: 2017-09-03T02:55:00.446Z Reads: 174

```
Ohh my bad I didn't realize it was liion, my bad. @Ackmaniac
```

---
## \#6 Posted by: pennyboard Posted at: 2017-09-03T13:57:06.926Z Reads: 162

```
Why do you recommend such high cutoffs for a lipo? Is it not fine for a lipo to go down to 3.1 volts per cell or so? I've been doing that for about 9 months with mine and they're still in good, working condition.
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2017-09-03T16:29:40.881Z Reads: 151

```
I'm not entirely sure if it is correct, but you should probably have a smaller difference between bat min and motor min. As you have a delta of 62A between those, only 8 amps would go back to the battery while the rest will be turned into heat in the motor and the vesc. -70A per Motor would be very strong, i'm running bat -10 and motor -40 on my single 6374.
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-09-03T16:56:41.376Z Reads: 146

```
That's simply not the case. The VESC or the motor doesn't burn that into heat. They would melt in a couple of seconds.
It all has to do with the duty cycle. But that is a long topic.
```

---
## \#9 Posted by: Der6FingerJo Posted at: 2017-09-03T17:38:33.551Z Reads: 144

```
Alright thank you, i wasn't too sure either but someone mentioned that it might be a problem especially in FOC. I guess that's not the case then.
```

---
## \#10 Posted by: Ixf Posted at: 2017-12-18T01:46:57.669Z Reads: 112

```
Quick note, are you using the 12s4p form torqueboards?   I believe their BMS will cut off above 80 A discharge.  If you are running dual might want to limit battery max to 40A so the board doesn't cut off on you on hard acceleration.
```

---
