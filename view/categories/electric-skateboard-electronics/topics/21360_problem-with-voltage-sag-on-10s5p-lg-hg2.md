# Problem with voltage sag on 10S5P (LG HG2)

### Replies: 9 Views: 716

## \#1 Posted by: pyttroll Posted at: 2017-04-19T11:44:51.908Z Reads: 113

```
Hi guys,

After running into over voltage faults last week I decided to rewire my BMS to only use it for charging.
Since then I've noticed some unusual voltage sagging.
Could my rewiring of the BMS have caused this? Do you guys have any idea on how I should proceed to diagnose the issue?

Here is the same ride, before and after my changes:

https://metr.at/r/ik0qw

It gets really bad towards the end...

https://metr.at/r/b2Rt2

Thanks,

Pyt
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2017-04-19T11:53:50.988Z Reads: 105

```
Can you post pics of your current BMS wiring and maybe draw a diagram how it was wired earlier?
```

---
## \#3 Posted by: Nordle Posted at: 2017-04-19T11:59:21.163Z Reads: 99

```
Goes down from 40v to 33v with 2 times over voltage (from hard braking i assume)? Can't see the "sag" in your charts.
```

---
## \#4 Posted by: pyttroll Posted at: 2017-04-19T12:03:34.546Z Reads: 97

```
Maybe I'm confused about voltage sagging, I'm concerned about the voltage jumping a lot between 34V and 40V, it does not look as stable as it used to. On the first ride, voltage was super steady, on the second ride it's all over the place...
```

---
## \#5 Posted by: Nordle Posted at: 2017-04-19T12:06:54.002Z Reads: 97

```
Ok now i see, thats the opposite of voltage sag^^ could be from hard breaking too. Lowering max regen brake current could help but would result in weaker brakes.
```

---
## \#6 Posted by: Blasto Posted at: 2017-04-19T12:08:00.638Z Reads: 94

```
Towards the end, there's little spikes because you are braking, look at youbcurrent, it will be negative
```

---
## \#7 Posted by: pyttroll Posted at: 2017-04-19T12:10:24.151Z Reads: 92

```
Ok that makes sense, I guess the BMS was preventing these spikes before... Is this going to be a problem for the battery?
```

---
## \#8 Posted by: Nordle Posted at: 2017-04-19T12:21:29.708Z Reads: 90

```
Don't think so, hg2 is rated for 4A max charging current. So for 4P that would be 16A (4*4). Can't see that much in your chart. Anyways you should set max charge current @16A or maybe bit lower for longer battery life.
Edit: 4P is mine^^ 5P is 20A of course :P
```

---
## \#9 Posted by: pyttroll Posted at: 2017-04-19T12:29:28.379Z Reads: 85

```
Thanks, I'll do that.
```

---
