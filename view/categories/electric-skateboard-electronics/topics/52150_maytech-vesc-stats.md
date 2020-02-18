# Maytech vesc stats

### Replies: 21 Views: 1098

## \#1 Posted by: Alex.Scheff Posted at: 2018-04-13T10:24:13.726Z Reads: 162

```
Hello

I have two maytech vesc's and wonder how my bldc settings should look like. Can anyone show his settings to me?
```

---
## \#2 Posted by: Acidfie Posted at: 2018-04-13T10:26:12.817Z Reads: 164

```
depends of your motor and battery.

when using maytech firmware, check for the **current ramp step bug**
```

---
## \#3 Posted by: Alex.Scheff Posted at: 2018-04-13T10:30:21.324Z Reads: 157

```
Motor kv 170
Battery 12s6p lg hg2 (20A discharge per cell)
```

---
## \#4 Posted by: Acidfie Posted at: 2018-04-13T11:19:29.429Z Reads: 142

```
need to know **which motor** aka, specification. not only the kv number, thats only the tip of the iceberg.

as long for the battery:

battery max: 100A should do fine
battery min (regen): approx. 20 amps (overall)

1 or 2 or 3 or 4 vescs?

dude with this information no one can help you right now.
```

---
## \#5 Posted by: Blitz Posted at: 2018-04-13T11:47:12.646Z Reads: 120

```
First video Uses new program second one Is the old classic BLDC tool
It Is hard to explain how to set It up if you don't understand the words etc I highly recommend you watch one of the videos linked.
https://www.youtube.com/watch?v=v1glLDO-EjA

https://www.youtube.com/watch?v=_mNnHp7sOBE
```

---
## \#6 Posted by: Bjork3n Posted at: 2018-04-13T13:27:07.891Z Reads: 95

```
From my experience maytech vesc is only suitable for max 30A battery max on each vesc. 
When I went above 30A battery max I got random drv faults on heavy accelerations.
Same issue with 3 maytech vescs
```

---
## \#7 Posted by: Acido Posted at: 2018-04-13T13:29:34.886Z Reads: 88

```
100a on maytech vesc?
```

---
## \#8 Posted by: Bjork3n Posted at: 2018-04-13T13:36:19.262Z Reads: 87

```
"Poof" 😂   ......
```

---
## \#9 Posted by: Acido Posted at: 2018-04-13T13:37:22.306Z Reads: 86

```
more like ![track|660x440](upload://2pUuGglGkeo6KQv5XuSNZvDQ8hs.jpg)
```

---
## \#10 Posted by: Alex.Scheff Posted at: 2018-04-13T14:29:33.451Z Reads: 78

```
I'm sorry I was in school :sweat_smile:
```

---
## \#11 Posted by: Alex.Scheff Posted at: 2018-04-13T14:32:58.830Z Reads: 74

```
 [This](http://www.electric-skateboard.builders/t/new-6374-with-hall-sensors-and-reinforced-mounting-side-tell-me-what-you-want/48635) motors

Two vesc's
```

---
## \#12 Posted by: Alex.Scheff Posted at: 2018-04-13T14:37:18.310Z Reads: 73

```
Do you still use the maytech vesc?
```

---
## \#13 Posted by: Bjork3n Posted at: 2018-04-13T14:46:17.269Z Reads: 67

```
yes i do. 
But as i said i only use batterymax 30A on each vesc.
So total 60A battery max on my dual setup. (Same as raptor 2 setting).
Had not had any issues when i lowered the batterymax to 30A. 

I have orderd x2 Focboxes i will use once the maytech fails....if they fail.
```

---
## \#14 Posted by: Acidfie Posted at: 2018-04-13T15:06:27.787Z Reads: 65

```
Afaik the vesc regulate the current by it self, I was using 60 amps on a maytech VESC and it worked without any issues
```

---
## \#15 Posted by: Bjork3n Posted at: 2018-04-13T15:13:00.457Z Reads: 61

```
Battery max 60A or Motor max? With hard accelerations?
```

---
## \#16 Posted by: Acidfie Posted at: 2018-04-13T15:15:38.727Z Reads: 56

```
Battery max
```

---
## \#17 Posted by: Bjork3n Posted at: 2018-04-13T15:25:15.275Z Reads: 51

```
Lucky you. 

3 vesc from maytech all the same issue. Bad luck for me.
```

---
## \#18 Posted by: banjaxxed Posted at: 2018-04-13T15:34:04.521Z Reads: 53

```
The fancy new ones or the older version? I've read good threads regarding doc and 12d from the newer batch with the label on the caps_emphasized text_
```

---
## \#19 Posted by: Acido Posted at: 2018-04-13T15:56:49.509Z Reads: 46

```
you said 100a
```

---
## \#20 Posted by: JdogAwesome Posted at: 2018-04-13T19:25:08.610Z Reads: 41

```
Like @Acidfie said I have my Maytech VESC limited to 60A Battery current and it's worked great for me. I was also running my hubs at to high a voltage so they where drawing like 40A each at full throttle and it worked fine, with some added small heatsinks to the MOSFET's.
```

---
## \#21 Posted by: Acidfie Posted at: 2018-04-13T19:28:43.064Z Reads: 39

```
I said 100A overall meaning 2 VESCs so 50 per VESC
```

---
