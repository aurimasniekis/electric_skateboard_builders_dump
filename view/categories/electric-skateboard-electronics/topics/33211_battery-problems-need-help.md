# Battery Problems. Need help!

### Replies: 14 Views: 679

## \#1 Posted by: Emerson Posted at: 2017-09-15T18:18:06.423Z Reads: 115

```
I've got a 10S3P made of 25Rs from the last big group buy via @JLabs .  The pack is charged up and multi-meter readings show the voltage go from around 7V to 42V when I turn it on and off via the e-switch.  Buuuuut that's only when its not plugged into anything else.  When I have the pack connected to my vescs or even just one the voltage will ramp up to about 36V upon turning it on then quickly drops off to about 3.7V.  

What I've tested:
- Replaced the battery with a different 10S4P pack and everything seems to function as intended.  This would include all connections, cabling, vescx + focbox, and motors.  
- Taken multi-meter readings straight off the xt60 connector from the battery (on/off)
- Taken multi-meter readings when connected to two vescs (Voltage drop off)
- Taken multi-meter readings when connected to one vesc (Voltage drop off)

   Any clue why this would happen?  Has the BMS somehow fried?
```

---
## \#2 Posted by: barajabali Posted at: 2017-09-15T18:21:58.534Z Reads: 109

```
It's likely broken spot welds

Does voltage flex when you do not touch it? Or when you move it around.
```

---
## \#3 Posted by: Emerson Posted at: 2017-09-15T18:36:25.248Z Reads: 101

```
Voltage is consistent (~42V when on) when not touching it.  I'll do a multi-meter flex test this evening.
```

---
## \#4 Posted by: JdogAwesome Posted at: 2017-09-15T18:55:44.204Z Reads: 93

```
Could we possibly get some pics? I think @barajabali definitely has a good point it could be the welds, though is the BMS and switch integrated into the pack if so it could be that as well.
```

---
## \#5 Posted by: mmaner Posted at: 2017-09-15T18:56:28.404Z Reads: 86

```
Im guessing, but it might be the BMS.  There have been other issues with the BMS in those packs.  Its pretty simple to replace if you have the soldering skills.
```

---
## \#6 Posted by: Emerson Posted at: 2017-09-15T19:41:47.444Z Reads: 85

```
Yeah, I'm heavily leaning towards it being a BMS issue.  I'm fairly confident in my soldering at this point though...between esk8, drones, and batteries I've gained a bit of experience (not necessarily good, but I have experience). 

 Assuming all other items are ruled out, is there a BMS with an integrated e-switch that you guys would suggest?  

Right now the pack has shrink wrap on it that I'll have to remove but I'll get some pics up this evening.
```

---
## \#7 Posted by: sl33py Posted at: 2017-09-15T19:45:21.437Z Reads: 81

```
Especially if it's suspect - i would re-wire and bypass/remove the BMS - then see if the battery gives consistent/correct voltages.  Just process of elimination - if that doesn't address/fix - dig deeper into pack.

If you want a replacement BMS, do you want a full size (and power through) BMS, or a small one just to charge and bypass for discharge?
```

---
## \#8 Posted by: Emerson Posted at: 2017-09-15T19:56:15.401Z Reads: 83

```
I would probably want to go with a full size one just for piece of mind but I'm open to discussion.  I like the idea of not worrying as much when braking down hills while on a fully charged pack (with a discharge only bms I think) but who knows.
```

---
## \#9 Posted by: mmaner Posted at: 2017-09-16T00:07:48.966Z Reads: 63

```
<img src="/uploads/db1493/original/3X/9/7/976b5f7e88c372bb516e7b32645b5f4960b97e4f.JPG" width="354" height="500">
```

---
## \#10 Posted by: Emerson Posted at: 2017-09-20T11:35:31.009Z Reads: 41

```
I was finally able to run a few tests this weekend and figured I'd post the results for those curious.  I bypassed the BMS (discharge) and was able to run the dual vescs as intended.  I even got to ride for a few miles with no issues.  As such I'll be replacing the BMS, hopefully with the BesTech listed above.  @mmaner Don't those in particular have a MOQ of 2?  Might anyone have a spare I could purchase?
```

---
## \#11 Posted by: mmaner Posted at: 2017-09-20T11:59:37.380Z Reads: 39

```
They do, shouldn't be a problem to sell the 2nd one though, they are popular.
```

---
## \#12 Posted by: Just_esk8in Posted at: 2017-09-20T12:11:14.774Z Reads: 41

```
If you do end up buying one from bestech, might I ask for the second one.
```

---
## \#13 Posted by: Emerson Posted at: 2017-09-20T19:49:13.916Z Reads: 31

```
I forgot to reply to your comment...I didn't notice any broken spot welds when inspecting the pack.  Voltage doesn't change when sitting idly or if moved around.
```

---
## \#14 Posted by: Emerson Posted at: 2017-09-20T19:49:28.179Z Reads: 31

```
Sure thing.
```

---
