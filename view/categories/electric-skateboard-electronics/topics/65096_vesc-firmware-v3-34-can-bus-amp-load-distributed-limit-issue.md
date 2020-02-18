# VESC Firmware V3.34 CAN Bus Amp Load Distributed Limit Issue

### Replies: 1 Views: 138

## \#1 Posted by: ZFreaky Posted at: 2018-08-16T17:57:01.266Z Reads: 38

```
I had to replace my hand made VESCs with a pair of torqueboards VESCs and I set the current limit on both to 10 amps to draw 20 from the battery, however, what's actually happening is the telemetry on my remote is saying it's limiting to 5 amps, which leads me to believe that it's saying the one master VESC it's connected to limiting to 5 amps, because it knows there's a second VESC to command the other 5 amps. So I'm confused. Imma try changine the VESC settings to 20 amps each and see if that fixes it, anyone with experience with this? Is it just the master I need to set?
```

---
