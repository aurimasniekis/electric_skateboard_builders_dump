# Charging two 4s batteries with one charger

### Replies: 18 Views: 3185

## \#1 Posted by: wieg16 Posted at: 2016-04-19T23:48:34.336Z Reads: 182

```
hey guys, I've been building my first electric skateboard and I have ran into a small hiccup... so i purchased everything for a 8s board, my low voltage alarm is 8s, my charger is a 8s balance charger. since it is impossible to find a 2x4s connector to 8s balancing lead, i decided that i would try and make one. Is it possible to take the two 4s connectors and cut them off, then solder that into a 8s connector so that the two batteries essentially become one?
```

---
## \#2 Posted by: laurnts Posted at: 2016-04-20T00:40:21.830Z Reads: 180

```
Very much possible. It needs to be carefully done. It's also recommended to use multimeter to get the voltage channel within the balance plug properly. I did this to combine 2 3S into 6S.
```

---
## \#3 Posted by: cmatson Posted at: 2016-04-20T00:43:09.165Z Reads: 176

```
You can also charge batteries in parallel just fine if you want to still keep them separate.
```

---
## \#4 Posted by: wieg16 Posted at: 2016-04-20T02:52:29.798Z Reads: 164

```
can someone link a picture of how i will need to plug the 4s wires into the new 8s connector
```

---
## \#5 Posted by: trbt555 Posted at: 2016-04-20T09:35:27.606Z Reads: 153

```
You can buy 4S parallel balancing lead at [Hobbyking](http://www.hobbyking.com/hobbyking/store/__27078__JST_XH_Parallel_Balance_Lead_4S_250mm_2xJST_XH_.html) and you'll probably also find a parallel charge lead there too.
These will allow you to charge your lipo's in parallel and avoid needing to build your own series charging harness and all potential fireworks that go with it.

The only drawback is you'll be balancing parallel sets of two cells but if you balance your lipo's individually from time to time, you'll be fine.
```

---
## \#6 Posted by: treenutter Posted at: 2016-04-20T19:07:38.997Z Reads: 142

```
@trbt555 when you charge two batteries in parallel I think that we:

* Use a parallel connector to attach both batteries to the charger

* Use a parallel balance lead like the one in your link

* Set your charger to the voltage of a single battery (or do you set it to charge to their total?) I.e. charger set to 4s or 8s?
```

---
## \#7 Posted by: trbt555 Posted at: 2016-04-20T19:45:15.541Z Reads: 137

```
You need to set it to 4s.
Look at it this way: in a parallel setup each individual pack is connected directly to the charge leads so the voltage should only be that of the packs.
```

---
## \#8 Posted by: mohammedex Posted at: 2016-04-20T22:10:34.360Z Reads: 131

```
There you go. Now that you already have an 8s charger I think you should make the 4s to 8s connector it is really simple and you won't have to worry about balancing them individually once in a while.

<img src="/uploads/db1493/original/2X/6/6b26a12c3db8322ecec971791ed676b47bdd8e87.png" width="690" height="388">
```

---
## \#9 Posted by: wieg16 Posted at: 2016-04-20T22:53:42.220Z Reads: 128

```
Thanks so much guys!! I think I'm going to make that and try it out in series
```

---
## \#10 Posted by: trbt555 Posted at: 2016-04-21T04:49:44.541Z Reads: 125

```
Be very careful with the order n which you connect the packs to your series charging harness. Number the connections and the plugs so you always connect in the same order.
Otherwise you'll see the infamous magic smoke & light show.
```

---
## \#11 Posted by: wieg16 Posted at: 2016-04-30T20:35:07.007Z Reads: 115

```
i tried soldering them together today to make this 4s-8s conversion and whenever i connected the positive to the negative to hook the batteries up in series the plugs sparked and i fried the connectors. does anyone know why this is happening, all the balancing leads are hooked up in the same way as the diagram. im sure it has to do with the batteries having the positive and negative balancing leads hooked up and having the batteries positive and negative leads connected, causing the battery to think you are plugging it into itself.
```

---
## \#12 Posted by: mohammedex Posted at: 2016-04-30T20:40:34.209Z Reads: 111

```
Damn, can you post a pic of the wiring?
```

---
## \#13 Posted by: wieg16 Posted at: 2016-04-30T20:41:02.174Z Reads: 111

```
<img src="/uploads/db1493/original/2X/8/8617984290816840c6281c8d91670e58abd2aa09.jpg" width="375" height="500">
```

---
## \#14 Posted by: wieg16 Posted at: 2016-04-30T20:41:32.150Z Reads: 107

```
I have them pulled out but they were soldered and pushed all the way in
```

---
## \#15 Posted by: trbt555 Posted at: 2016-04-30T20:51:21.262Z Reads: 108

```
You need to make sure you get the order of your batteries in series right.
It needs to correspond to the order in which you've rigged the balance connections.
Here's my schematic for 2x3S but the principle will be the same, just add a cell to each pack:
<img src="/uploads/db1493/original/2X/a/af6930ce81da30351fadee13e22a8cbd8ae0428f.png" width="382" height="500">
```

---
## \#16 Posted by: wieg16 Posted at: 2016-04-30T21:00:05.094Z Reads: 105

```
i believe that is how i have it set up, would you be able to skype so i could work out the problem live?
```

---
## \#17 Posted by: trbt555 Posted at: 2016-04-30T21:04:59.807Z Reads: 100

```
Lay out your wiring clearly and show us a picture.
```

---
## \#18 Posted by: wieg16 Posted at: 2016-04-30T21:07:49.976Z Reads: 101

```
I think I figured it out, if I try usin the opposite wires to connect in series, it doesn't spark. I'm guessing my problem was that the wires were not wired in series right corresponding with the balance plugs like you said
```

---
