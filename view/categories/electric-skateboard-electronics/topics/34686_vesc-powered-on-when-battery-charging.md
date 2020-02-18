# VESC powered on when battery charging?

### Replies: 13 Views: 779

## \#1 Posted by: cwazy1 Posted at: 2017-10-03T17:44:12.526Z Reads: 129

```
Just noticed that there was a blue light on in my enclosure when my battery was plugged in charging. I have to assume it was the VESCs, as there is nothing else with a blue light in the enclosure.. is that normal behavior? 

The battery switch itself was off.

My power pack is from TB. Its basically a space cell 4. 12s4p with the integrated anti spark switch, charging port, LED % indicator and 2 USB ports in the packaged battery.
```

---
## \#2 Posted by: Silverline Posted at: 2017-10-03T17:45:17.187Z Reads: 126

```
Using the bestech BMS ??
```

---
## \#3 Posted by: cwazy1 Posted at: 2017-10-03T17:45:54.071Z Reads: 127

```
Just edited my OP. 

I'm using whatever is in the TB power pack.
```

---
## \#4 Posted by: Colson003 Posted at: 2017-10-04T00:30:16.821Z Reads: 110

```
@cwazy1 My 6S4P from them does the same thing. I found that out by playing with the remote while the board was charging and the motor started spinning.
```

---
## \#5 Posted by: JdogAwesome Posted at: 2017-10-04T04:47:43.017Z Reads: 102

```
I would assume that means that the switch inside the battery or whatever has failed and is now always on. I'd recommend physically disconnecting your battery from the rest of the board or else it's gonna over time drain the bat really low, until the BMS cuts it.
```

---
## \#6 Posted by: Colson003 Posted at: 2017-10-05T03:07:18.646Z Reads: 91

```
@JdogAwesome I can still turn it off using the switch, but when plugged in to charge it powers everything on. Why would that cause the battery to drain really low when it's charging?
```

---
## \#7 Posted by: JdogAwesome Posted at: 2017-10-05T21:10:40.427Z Reads: 83

```
Oh I didn't realize that's what was happening, no if it's charging and it turns it on then it's not going to discharge, it's just going to be on so yeah. Though that sounds weird and I doubt it's normal you might want to check out your wiring or maybe get a different BMS.
```

---
## \#8 Posted by: Colson003 Posted at: 2017-10-06T16:13:20.614Z Reads: 70

```
@JdogAwesome since both our packs (@cwazy1 and mine) do this and they're both from TB I'm assuming this is just what their BMS does.
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-10-06T17:25:39.251Z Reads: 63

```
No that doesn't sound right, have you tried contacting torque boards about it cause it's not normal.
```

---
## \#10 Posted by: cwazy1 Posted at: 2017-10-06T18:31:15.391Z Reads: 61

```
hmm @torqueboards ?
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-10-06T18:40:20.502Z Reads: 60

```
My pack from torqueboards does the exact same thing. I don’t think it’s anything out of the ordinary
```

---
## \#12 Posted by: cwazy1 Posted at: 2017-10-06T18:42:08.903Z Reads: 59

```
It sounds like thats just the way that the TB power packs function, but the real question is... does it do any harm to components downstream of the battery, ie your VESCs by having them on all the time while charging.
```

---
## \#13 Posted by: mmaner Posted at: 2018-09-09T17:06:57.336Z Reads: 37

```
Most BMSs have to be powered on to charge and balance, it's normal.
```

---
