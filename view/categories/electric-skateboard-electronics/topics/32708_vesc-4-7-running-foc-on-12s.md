# VESC 4.7 running FOC on 12s

### Replies: 5 Views: 547

## \#1 Posted by: The_Dude Posted at: 2017-09-09T13:43:12.650Z Reads: 124

```
Hi VESCperts,
currently I'm running my dual quality (self soldered 😉) VESCs V4.7 in BLDC Mode with 12s Lipos on my eMTB. 
I'm tempted to go to FOC with the new FW 3.28 ... what HW measures do you suggest, that I don't fry them at the first go?
```

---
## \#2 Posted by: trampa Posted at: 2017-09-11T19:04:25.838Z Reads: 79

```
Hi Dude, I had no issues so far, but we used our Low KV motors (118 and 136), which don't swallow lots of amps and the lower ERPM makes it easy to track the rotor position. I would just start with lower Amp settings. Should work just fine. 

Frank
```

---
## \#3 Posted by: stormboard Posted at: 2017-09-12T02:53:18.026Z Reads: 66

```
also thinking using focbox with a 12s setup im starting this week..can the focbox handle a single 190/170kv motor with say a 12s 20wh setup
```

---
## \#4 Posted by: The_Dude Posted at: 2017-09-12T12:35:00.451Z Reads: 52

```
Thanks Frank! 
Currently I'm using 80A motor and battery max, Motor is about 200 kV. What are your settings?

No bigger C21, cooling of MOSFET or anything else? I have to admit, I just lost track of all the measures described somewhere in the forum and especially which measure really helps ...
```

---
## \#5 Posted by: trampa Posted at: 2017-09-12T14:07:40.482Z Reads: 43

```
We use 45A for Motor and Battery. The low KV helps to put out the torque at low Amps. 118KV on the 4.7....

Frank
```

---
