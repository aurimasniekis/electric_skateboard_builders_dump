# Will voltage sag cause intermittent power loss?

### Replies: 6 Views: 620

## \#1 Posted by: chewydinosaurs Posted at: 2017-08-20T21:11:49.583Z Reads: 97

```
I used my board at campus today with some steeper hills. I'm running a 6s with 280kv so it could certainly use more power which I'm debating on using an 8s lipo. I only have the issue when going up or down hills (braking constantly) and it would intermittently cut out and almost feel like it was braking. The failsafe is set and I don't have the setting set to brake when it loses connection either in the bldc tool. It's almost rhythmic being every 2 seconds and it cuts out at a higher rate the faster I go. I'm wondering if a voltage sag would cause this when going up or downhill, but I also just started using the mini remote which could be the issue.

Edit: I notice my mini 2.4ghz (same as torque boards remote) flashes red when it cutsout. Im not sure of this is a battery issue in the remote or if it's losing connection
```

---
## \#2 Posted by: Hardwiring Posted at: 2017-08-20T21:17:49.066Z Reads: 90

```
I had a very similar problem that was the remote battery
```

---
## \#3 Posted by: evoheyax Posted at: 2017-08-20T22:15:33.411Z Reads: 73

```
The flashing red indicates it's looking for the receiver. Either your remote is cutting out (you need good fresh batteries) or you have an issue that causes the receiver to lose power.
```

---
## \#4 Posted by: Kaden56 Posted at: 2017-08-20T22:22:24.854Z Reads: 67

```
The same thing happened to me with the the mini enertion remote and almost caused me to wreck hard. I went back to the gt2b
```

---
## \#5 Posted by: torqueboards Posted at: 2017-08-20T22:35:27.311Z Reads: 61

```
Check batteries and/or make sure your antenna is sticking out a bit. The mini has been pretty much 100% reliable only issue I had was when batteries died out.
```

---
## \#6 Posted by: Deckoz Posted at: 2017-08-21T13:57:13.315Z Reads: 42

```
Hey man use this for setting up the bind and failsafe and ppm endpoints so that you coast when failsafe or cutouts

http://www.electric-skateboard.builders/t/torqueboards-nano-remote-throttle-fix/30895/24

But yes if you are sagging going up hill or regenerating higher then your max input the vesc will cut off. For min and max input try to set the settings about 1 cell voltage below your min charge. And your max 2 cell voltages.(obviously set your cut offs for actual values)

Ie I run 10s liion. My cut off start is 35.5, and my cut off is 33.5. 

I have my min input as 30volts to account for rolling sag at the bottom of the charge

My max is set to 48volts for regen. I hardly ever brake especially when I start riding as the first mile is typically just cruising getting my ankles and feet feeling the board. So over regen isn't an issue as typically regen braking will spike volts but the current isn't that high for long periods.

Anyway set wider min and maxes and you should see less cut outs. Of course this is dependent if you have a BMS limiting discharge current and Voltage as well..
```

---
