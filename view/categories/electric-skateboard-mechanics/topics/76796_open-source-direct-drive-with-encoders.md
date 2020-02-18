# Open Source DIRECT DRIVE &#124;&#124;&#124; with encoders

### Replies: 27 Views: 1285

## \#1 Posted by: fedestanco Posted at: 2018-12-02T14:01:13.051Z Reads: 368

```
No one ever reads the written intro when there are pics below, so I'll try to be concise:

Objectives: 
a) Fewest possible amounts of parts; the reason is to contain costs in small batches production; for example the 2 motor walls are a single design; [no custom part](https://item.taobao.com/item.htm?spm=a230r.1.14.13.786b455cFW7Zsi&id=527678369898&ns=1&abbucket=13#detail) required to hold on the stator.

b) Maximizing stator dimensions given a 300mm (circa) axle length; the motor tube will only have to contain the stator and about 4 extra mm for copper windings (may vary according to wire gauge); all the extra wiring job ang soldering can be done in the black plastic part (optional) above the hanger.
---I am aiming at 52.8mm(standard available diameter) by 60mm (length)----  

c)CNC friendly: minimum dimension endmill required is 4mm. Chamfers are used in convex curves and fillets in concave grooves.

d)Custom encoder pcb (optional) instead of the 3hall standard sensors; this bumps the angular precision to 2^14 digits (maybe a bit less since a couple bits are used for other purposes). The "observer" (software) knows perfectly where the magnets are and can apply torque without playing the guessing game.

e)To prevent having the project ending on the back burner, I will be releasing it on github under GPL v3 license (**modify, share every modification, sell, give attribution**)

TODO list:
a)simulate stress on chromoly hollow axles (12mm stepped down to 10mm. Inner 4mm through axle hole)
b)make ISO drawings for non-CNC parts (motor tube and walls)
c)make notes about ISO interference fit on constrained parts
e)make a scaled down version with half the stator size

Github repo: TODO ([Thingverse repo is ready](https://www.thingiverse.com/thing:3256883))
![front%20view%20total%20assembly|690x351](upload://tn8eA0cr8oTGymgcKRk1nyrPE5O.png) ![half%20section%20view|690x447](upload://gaVacnaZXrvjYy8jlipSQztoOJa.png) ![front%20view%20half%20assembly|690x442](upload://yhxhIL9yVj4OTNpCla1s5Q1C8Wz.png) ![rear%20view%20total%20assembly|690x340](upload://2ySaKP0JjtYVtnJlp3qrl1J9mNE.png) ![pcb%20pic|572x500](upload://25NOS3rJgV6a2vyLNXQgKuit9u9.png) ![encoder%20view|675x500](upload://34PBVfRl0OqK4Sl6FvLBsJputic.png)
```

---
## \#2 Posted by: torqueboards Posted at: 2018-12-02T16:36:45.851Z Reads: 317

```
Looks great :slight_smile:
```

---
## \#3 Posted by: banjaxxed Posted at: 2018-12-02T20:24:09.137Z Reads: 285

```
MIC drop
Pin drop
```

---
## \#4 Posted by: Blasto Posted at: 2018-12-02T21:09:48.794Z Reads: 272

```
The encoder placement is a bit weird to say the least
```

---
## \#5 Posted by: fedestanco Posted at: 2018-12-02T21:12:49.323Z Reads: 270

```
Still very experimental. If I am not wrong 107mm wheels are wide enough to completely enclose the encoder assembly within the urethane, making it safe from impacts.
```

---
## \#6 Posted by: Klaerke91 Posted at: 2018-12-02T21:29:34.722Z Reads: 253

```
Nice that you have made it opensource. Looking forward to the github repo being released :-)
```

---
## \#7 Posted by: fedestanco Posted at: 2018-12-03T18:50:09.464Z Reads: 224

```
I temporarely uploaded the STLs on Thingiverse since the licensing process is more straightforward. Since I am a new user, 24h have to pass before they can be available to the public. The link will be published _[here](https://www.thingiverse.com/thing:3256883)_.

I want to follow @Blasto suggestion and make the encoder assembly a bit neater; thus the relative files will be published after remodeling.

A note on STL format: it sucks. Unfortunately thingiverse doesn't accept IPT format; I will have to look into another platform in the next days.
```

---
## \#8 Posted by: Fiori Posted at: 2018-12-03T18:53:18.286Z Reads: 214

```
Maybe GrabCad?
```

---
## \#9 Posted by: fedestanco Posted at: 2018-12-03T18:55:40.313Z Reads: 203

```
GrabCad is great and also supports formats conversion but I read users cannot use the files for commercial projects and must ask the author for permission each time they want to...
```

---
## \#10 Posted by: Mich21050 Posted at: 2018-12-03T19:02:09.368Z Reads: 199

```
First of all: Great project and really nice idea to make it open source... Maybe once you finsih everything you could write a step per step guide? 
Keep us updated :smile:
```

---
## \#11 Posted by: moon Posted at: 2018-12-03T19:10:17.895Z Reads: 197

```
Why not use .step file format
```

---
## \#12 Posted by: fedestanco Posted at: 2018-12-03T19:13:56.430Z Reads: 190

```
I think you are referring to the encoders wiring; if so I printed on the PCB the same infos (and in the same order I believe) that are printed on vesc6 derivatives. So the wiring shoud be pretty simple. 

@moon I can do it if it's supported; even though ipt source files are preferred I believe.
```

---
## \#13 Posted by: Mich21050 Posted at: 2018-12-03T19:15:22.015Z Reads: 188

```
I was actaully talking about the whole dd.. :smile:
```

---
## \#14 Posted by: fedestanco Posted at: 2018-12-03T19:19:55.166Z Reads: 185

```
In that case the best I can do is an exploded view with some notes attached. A video would be better but , you know, this thing is not cheap to prototype and already have [some other project](https://www.electric-skateboard.builders/t/the-sparkling-switch/58033/26?u=fedestanco) in the waiting list :slight_smile:
```

---
## \#15 Posted by: Mich21050 Posted at: 2018-12-03T19:20:42.917Z Reads: 175

```
That would be great :slight_smile:
```

---
## \#16 Posted by: pat.speed Posted at: 2018-12-03T19:54:29.959Z Reads: 167

```
Why are you going for a hollow axle? A solid axle would be stronger no?
```

---
## \#17 Posted by: fedestanco Posted at: 2018-12-03T20:01:36.265Z Reads: 172

```
Yes it would. The hole is meant for the encoder wires; if you dont need sensors you can have it made solid. 
One interesting thing though is that heat treatments work better on hollow axles: the thermal shock is felt both in the inner and the outer axle body so the overall hardened metal is more if you have an hollow axle.
```

---
## \#18 Posted by: pat.speed Posted at: 2018-12-03T20:04:06.557Z Reads: 169

```
That is true I have never thought of that. I am building a dd too and am stuck with what material to use for my axle. I can easily source 12mm 304SS but I’m not sure if it’s strong enough, what do you think?
```

---
## \#19 Posted by: fedestanco Posted at: 2018-12-03T20:22:11.789Z Reads: 175

```
I wouldn't feel safe on a 304steel axle I you ask me. Probably 12mm would do but you still have to step it down to 10 if you use standard wheels. If I were you I'd go Gcr15 (bearing steel) as minimum; [these guys](https://item.taobao.com/item.htm?spm=a1z10.1-c.w4004-16225904547.46.7ccd4770v6l4NJ&id=576004220599) work with that steel. Obviously the best available steel is chromoly (41xx) if you can find a good supplier.
```

---
## \#20 Posted by: pat.speed Posted at: 2018-12-03T21:25:38.003Z Reads: 173

```
Thanks man, you are my saviour. I did find some gcr15 for 3D printer rails but I couldn’t find much info on its strength and hardness so assumed it wasn’t worth it.

Looking back this is exactly what I need, and it’s a good price too. Thank you a lot, just to check does this look right to you?

 ![image|281x500](upload://9ukCPwkAiiNJpZ9WSyK7wPwU4Ri.png)
```

---
## \#21 Posted by: fedestanco Posted at: 2018-12-03T23:15:31.908Z Reads: 153

```
Yep the name checks out. It is also equivalent to SUJx in the Japanese nomenclature.
Bear in mind that to get the advertised hardness you will need to temperature treat axle.

If you want to see how good/bad this alloy is maybe take a look at this chart: the red circles are from top to bottom: Chromoly, Gcr15, 304ss

![Screenshot_2018-12-04-00-14-37|281x500](upload://AiEiCTNJqxzpiNDrfCBkK5Zer6d.png)
```

---
## \#22 Posted by: harrypzee Posted at: 2018-12-04T00:26:51.055Z Reads: 142

```
Sick! Check out my post about my own open source hub motors/trucks (still very very work in progress!): https://www.electric-skateboard.builders/t/open-source-precision-trucks-and-hub-motors-project/61480 (mine is a bit different bcuz its in wheel hubs)
```

---
## \#23 Posted by: pat.speed Posted at: 2018-12-04T00:36:15.259Z Reads: 142

```
Do you know how come there is no ratings for tensile strength or yield point with the Gcr15, could it be due to it being used for bearings that it doesn’t have a normal rating
```

---
## \#24 Posted by: mikenyc Posted at: 2018-12-04T01:22:12.701Z Reads: 142

```
How is your project going?
```

---
## \#25 Posted by: pat.speed Posted at: 2018-12-04T10:04:14.897Z Reads: 127

```
oooooooh I searched google and found some cromoly for super cheap in the right size. 12mm - $15/m I just need to pester the crap out of the seller to ship it to a different state now :sweat_smile:

 ![39%20PM|690x361](upload://31quQiQRM27OhZzn8BzfGXfCa2H.png)

![51%20PM|526x132](upload://sxPTDcjIdzSyBeI6vw3OzdtDOqm.png)
```

---
## \#26 Posted by: Vanarian Posted at: 2018-12-04T11:07:47.231Z Reads: 123

```
Now that's **innovation** right? :stuck_out_tongue_winking_eye:

@fedestanco more seriously that's super  nice of you to make these **open source** and available **freely**. Keep the good work up, that's how one drives a DIY community forward.

https://media.giphy.com/media/11uArCoB4fkRcQ/giphy.gif
```

---
## \#27 Posted by: moon Posted at: 2019-01-08T12:27:01.252Z Reads: 82

```
[quote="fedestanco, post:1, topic:76796"]
d)Custom encoder pcb (optional) instead of the 3hall standard sensors; this bumps the angular precision to 2^14 digits (maybe a bit less since a couple bits are used for other purposes). The “observer” (software) knows perfectly where the magnets are and can apply torque without playing the guessing game.
[/quote]

Could this custom encoder pcb be used on bldc outrunners? - not dd

I'm guessing it will work 

![pcb%20pic|572x500](upload://25NOS3rJgV6a2vyLNXQgKuit9u9.png)
```

---
