# Having issues with an Enertion Focbox, not sure how to proceed

### Replies: 8 Views: 723

## \#1 Posted by: Vivalize Posted at: 2017-10-24T04:35:56.845Z Reads: 171

```
Hi there,

In my effort to dive into the VSEC world, I picked up a Focbox and tried connecting it to my hardware (10s battery, 260kv motor (links at the bottom)). When configuring the Focbox through the provided BLDC_Tool, I would get "Bad Detection Result Received" whenever trying to "Start Detection" in the BLDC side tab. I contacted Enertion support, had one of their guys remotely connect into my computer to try the same detection (at one of his later attempts, the focbox sparked up when he tried it). He then told me that the Focbox should still work (because he was still able to connect to it), but that I needed a new motor because 260kV was too high. I picked up a 190kv motor ( collections/electric-skateboard-motors/products/electric-skateboard-motor-6374-190kv-3150w ) and I am now trying the same detection process, though getting the same bad detection results. I contacted Enertion again, but this time they don't want to help, referring me to here.

So basically my question is, what should I do? I'm getting a bad feeling that the Focbox fried when the Enertion support guy tried the detection earlier. I should also mention that the Focbox gets really hot when idle, even though I've never even run a motor though it. I don't remember whether this occurred before it sparked. Enertion isn't giving replies to any of these issues, so any help would really be appreciated.

(In case it's relevant, the battery I'm using is two of these in series: https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html and the OLD motor I had (that was connected when the support guy ran the detections is: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html )
```

---
## \#2 Posted by: scepterr Posted at: 2017-10-24T04:38:40.850Z Reads: 155

```
Type faults in terminal tab after trying detection,
If its getting hot while idle there's likely damage
```

---
## \#3 Posted by: Vivalize Posted at: 2017-10-24T04:49:50.759Z Reads: 149

```
Typing "faults" into terminal after a failed detection just gives
> No faults registered since startup
```

---
## \#4 Posted by: scepterr Posted at: 2017-10-24T04:54:57.411Z Reads: 148

```
Do detection and watch real-time tab, see what happens there
```

---
## \#5 Posted by: Vivalize Posted at: 2017-10-24T05:03:10.497Z Reads: 142

```
It doesn't seem to be changing anything at all. Current stays at 0, Current In hangs around -0.06, Duty Cycle about the same. Temperatures still staying high at around 50C, and RPM also stays at 0 throughout. In the stats below, these stay pretty much the same throughout the detection as well.
Power: 0.0W
Duty Cycle: ~0.3%
Electrical Speed 0.0rpm
Battery current: ~0.06 A
MOSFET temp: ~50C
Fault Code: DRV8302
...
Drawn cap/Charged cap/Drawn energy/Charged energy: All zero
Tacho & Tacho ABS: 5 counts
Battery Voltage: ~38V
```

---
## \#6 Posted by: scepterr Posted at: 2017-10-24T05:03:59.545Z Reads: 131

```
There yah go
[quote="Vivalize, post:5, topic:36322"]
MOSFET temp: ~50C
Fault Code: DRV8302
[/quote]
```

---
## \#7 Posted by: Vivalize Posted at: 2017-10-24T05:16:59.350Z Reads: 123

```
Alright, I'm assuming that fault code is usually a sure sign that it's fried? Thanks for the help though!
```

---
## \#8 Posted by: barajabali Posted at: 2017-10-24T13:37:31.555Z Reads: 105

```
I'll look into your case for you pm me your info :)
```

---
