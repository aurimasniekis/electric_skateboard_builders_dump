# Vesc Cuts Out During Too Fast Acceleration?

### Replies: 5 Views: 701

## \#1 Posted by: chewydinosaurs Posted at: 2017-01-18T00:44:13.414Z Reads: 102

```
So I made my first diy board, still working out issues as my gear isn't exactly centered with my wheel. SO what that all means is that the tension on my belt is changing; every half rotation it's loose the other half rotation it's tight. On top of that issue (I'm just going to get a new gear), my vesc cuts out throttle if I accelerate too quickly. And I mean I'm barely putting anything on the trigger before it cuts out and flashes a red LED 6 times. I'm running 2x3s lipos into a 6s series on 70mm wheels (I'm going to order 80mm) with an SK3 280 kv motor connected to a vesc. Transmitter is an HKG2B. Any help on the vesc cutting out would be very helpful. Ive ordered larger 83 mm wheels and a new 36 pin gear and hopefully by centering it on the new wheels it will solve the problem?
```

---
## \#2 Posted by: evoheyax Posted at: 2017-01-18T01:11:00.089Z Reads: 99

```
Well the red light flashing is a sign that your getting an fault code. Fault codes are somethings a physical hardware problem, somethings a setting problem (the later seems ore likely for your symptoms). Is it possible to recreate the problem while its connected to your computer and on the bench? Under the real time data tab, there's a line that says Fault Code. If we know what that is, we can help you solve your problem pretty quickly.

My guess would be you need to adjust your low voltage cutoff. But it could be a couple other things.
```

---
## \#3 Posted by: chewydinosaurs Posted at: 2017-01-18T01:37:56.814Z Reads: 87

```
For some reason in BLDC the fault code line in the real time data tab is cutoff so I cannot see it not matter how many times I reformat the window size. I assume it's a voltage error but I cant see what error it is...<img src="/uploads/db1493/original/3X/1/6/16ca8361423752d2861316ea1bdec23bf07b7632.png" width="690" height="388">
```

---
## \#4 Posted by: Conor Posted at: 2017-08-27T01:13:10.848Z Reads: 45

```
Same thing happened to me have figured out how to see the fault code?
```

---
## \#5 Posted by: Bloop Posted at: 2017-08-27T01:52:04.494Z Reads: 40

```
If you are getting an error dont turn off the vesc. 
Go to terminal and write faults and you should see the error
```

---
