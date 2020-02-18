# Problem with vesc (spark)

### Replies: 40 Views: 2517

## \#1 Posted by: Nooby Posted at: 2016-11-02T20:36:20.999Z Reads: 162

```
Soooooo
I connected my vesc to my lipo...
Without antispark...
There was a spark...
Now it is dead

Are there any parts of the vesc which typiccaly break if there was a spark? Anything that could ne broken that i can replace?
```

---
## \#2 Posted by: rtasca Posted at: 2016-11-02T20:45:00.775Z Reads: 159

```
Sparks are not a problem to the vesc unless you wired it wrong polarity.
```

---
## \#3 Posted by: Nooby Posted at: 2016-11-02T20:48:54.356Z Reads: 155

```
Idk i just wired it right (as long as i know )connected it but noled light and no led on the reciever and no working Motor
```

---
## \#4 Posted by: rtasca Posted at: 2016-11-02T20:52:30.338Z Reads: 151

```
I mean, a spark at the plug when it gets connected, If you saw a spark inside the VESC its no good news. I read some units had problems with the pin connectors punching through the main wires insulation. Does anything look cooked on the board? Maybe some pics will help
```

---
## \#5 Posted by: Nooby Posted at: 2016-11-02T20:53:32.321Z Reads: 146

```
Ill get pics tomorrow and ill try to connect another time...
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-11-02T20:55:03.671Z Reads: 142

```
Can you post some picture ?
```

---
## \#7 Posted by: Nooby Posted at: 2016-11-02T20:55:42.580Z Reads: 140

```
Tomorrow i will
```

---
## \#8 Posted by: elkick Posted at: 2016-11-02T21:51:45.824Z Reads: 137

```
Are you still using the same battery setup?http://www.electric-skateboard.builders/t/did-i-do-sth-wrong/8812

Since it produced already a spark in your old configuration it might be still causing problems.
```

---
## \#9 Posted by: Nooby Posted at: 2016-11-03T06:47:08.686Z Reads: 115

```
Normally yes bit i forgot connecting
```

---
## \#10 Posted by: Nooby Posted at: 2016-11-03T07:15:19.822Z Reads: 114

```
<img src="/uploads/db1493/original/3X/2/2/227af8bce431925b0bd39acbdf3e0e7914b9d2cd.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/7/b/7badc5945a6d4204baf0b6205459c00a42638e67.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/9/f/9fb967efa4db231b03814f374e7c036fcfece029.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/3/a39c55ce1ea1c8f9246256012f25f4d4fdd84d0d.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/6/568f39f64404cf98b83b62c76c17cf27da5875d1.jpg" width="666" height="500">
Tell me which other pics you need
```

---
## \#11 Posted by: Nooby Posted at: 2016-11-03T07:22:58.235Z Reads: 110

```
<img src="/uploads/db1493/original/3X/8/9/892d1f5c95ed00203842be2fffa31d7df60ed5cf.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/c/dcbb5783cb5d3b1bd477f3060edf7d42e9f588c3.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/a/4a3a32b69609bdcb936c93503e6004156a5b9f3b.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/0/00473dddf73a10b2307a5806d55c13fb073659b0.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/6/f/6f9eea30b7fbc38a5fc15553f5ace497a15e0bba.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/a/2afc50005194514ed213763b205a64f6e0022b57.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/3/8/38175c8c199f1070c13ad772eb8255386a4371a6.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/d/cdc95604ff57b48bc9bceab6c1d1687d28692008.jpg" width="375" height="500">
I noticed that there is like a bubble on a mosfet
```

---
## \#12 Posted by: Nooby Posted at: 2016-11-03T07:28:59.412Z Reads: 104

```
Wrong alarm was only sticky crap
```

---
## \#13 Posted by: Nooby Posted at: 2016-11-03T07:31:40.691Z Reads: 104

```
I cleaned it and there is nothing wrong with it.....
```

---
## \#14 Posted by: Nooby Posted at: 2016-11-03T07:39:53.510Z Reads: 103

```
Is there a test if it is still alive without lipo?
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-11-03T07:56:34.517Z Reads: 102

```
You could use a 12V power supply.
```

---
## \#16 Posted by: smudgeUK Posted at: 2016-11-03T08:03:44.534Z Reads: 100

```
I'd recommend d re-soldering your red cable to your vesc's main board, that join is really bad!
3rd to last picture
```

---
## \#17 Posted by: SORRENTINO Posted at: 2016-11-03T13:49:37.833Z Reads: 85

```
Post a pick of the connectors so we can see if the are reversed
```

---
## \#18 Posted by: rtasca Posted at: 2016-11-03T15:37:56.907Z Reads: 78

```
Man, this looks really bad.... you should try to stick with black for negative and red for positive... I can't even tell IF you have something reversed on that harness because of the color mess. 

http://www.electric-skateboard.builders/t/did-i-do-sth-wrong/8812
```

---
## \#19 Posted by: evoheyax Posted at: 2016-11-03T16:43:05.649Z Reads: 74

```
Who produced this VESC? No offense, but those joints are all really bad looking IMO... High heat, thick lead solder, and less than 2 seconds to touch and you should have beautiful joint. This looks like the soldering I did when I didn't know how to solder correctly.
```

---
## \#20 Posted by: SORRENTINO Posted at: 2016-11-03T17:13:20.632Z Reads: 68

```
You can clearly see that the wire wasn't even tinned lol
```

---
## \#21 Posted by: elkick Posted at: 2016-11-03T17:38:31.807Z Reads: 60

```
That's the first time I see such a solder joint on one of our VESCs. 

Strange thing, but please PM me and we get that joint right and check, if it was causing that spark, which I doubt, since the battery looks a little bit strange too.
```

---
## \#22 Posted by: Nooby Posted at: 2016-11-03T18:45:08.169Z Reads: 58

```
it isnt from you @elkick sorry for the missunderstanding...
I just thought you would know the problem....
Idk where i bought it from im gonna research it.
```

---
## \#23 Posted by: Nooby Posted at: 2016-11-03T19:23:19.594Z Reads: 53

```
connected to the powersuply with 12 volts didnt pull any amps ....
maybe the capacitors are dead but i got nothin to measure.
```

---
## \#24 Posted by: Nooby Posted at: 2016-11-03T19:25:21.354Z Reads: 53

```
I think I am not going to resolder the joints myself but maybe ask somebody with more expreience to do it for me since I dont want to mess it up.
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2016-11-03T19:40:12.777Z Reads: 52

```
If you have a multimeter you can also check the can traceiver 
http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse

Or if your looking for repair maybe I can help you
```

---
## \#26 Posted by: Nooby Posted at: 2016-11-03T19:41:56.274Z Reads: 53

```
problem is that i cant find my multimeter :frowning:
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2016-11-03T19:43:07.096Z Reads: 53

```
Well, that kind of an important device 😜
```

---
## \#28 Posted by: Nooby Posted at: 2016-11-03T19:45:56.479Z Reads: 50

```
i guess im just gonna buy a new one.... never gonna find you again my friend
RIP MULTIMETER 1900-2016 :smile:
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2016-11-03T19:51:48.268Z Reads: 49

```
That a long life 1900.... more than time to change it.
```

---
## \#30 Posted by: Nooby Posted at: 2016-11-03T20:03:31.905Z Reads: 49

```
XD true story
```

---
## \#31 Posted by: Nooby Posted at: 2016-11-04T11:58:25.576Z Reads: 42

```
I found it!!!!!
```

---
## \#32 Posted by: Nooby Posted at: 2016-11-04T11:58:44.943Z Reads: 40

```
Soooo im gonna start messuring
```

---
## \#33 Posted by: Nooby Posted at: 2016-11-04T12:06:51.097Z Reads: 38

```
There is no power comong to my vesc and in the diode check mode it onlly beeped for the black cable  entering and exitong the capacitor pcb
```

---
## \#34 Posted by: Nooby Posted at: 2016-11-04T12:25:45.669Z Reads: 39

```
So after some more checking i reslized that the pcb connection between the positive and the capacitors is broken so i am going to solder some bridges in place later
```

---
## \#35 Posted by: TarzanHBK Posted at: 2016-11-04T12:50:59.246Z Reads: 38

```
[quote="Nooby, post:22, topic:12334, full:true"]
it isnt from you @elkick sorry for the missunderstanding...I just thought you would know the problem....Idk where i bought it from im gonna research it.
[/quote]

dude you just caused a german blackout! Now @elkick started an investigation who of his fellow german workers solders like that. Now everybody has to fill out a form where you have to put down exactly your workflow and after that a 23 hour speak about how someone dares to solder like that.

Don´t mess with us Germans about our quality!
:monkey:
```

---
## \#36 Posted by: Nooby Posted at: 2016-11-04T13:00:58.573Z Reads: 36

```
Sorry i didnt want to i never said that it was from him i just asked him if he knew the fault and thats it.
I hoped he knew it because he is also producing vescs
```

---
## \#37 Posted by: TarzanHBK Posted at: 2016-11-04T13:05:23.526Z Reads: 37

```
It´s alright dude, was just a joke :D

<img src="/uploads/db1493/original/3X/1/0/107a74ab1d4c1aaca79a47f5d9a395f61635118b.gif" width="640" height="360">
```

---
## \#38 Posted by: Nooby Posted at: 2016-11-04T13:06:13.801Z Reads: 40

```
Ooooh man 
i hate you for that joke
```

---
## \#39 Posted by: Nooby Posted at: 2016-11-04T16:33:54.740Z Reads: 35

```
Soooooo my vesc is fixed!<img src="/uploads/db1493/original/3X/8/0/8094cb51e4d6fd098b2079f1c3ca6efd085793a8.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/3/9/399af5b7b28302c5840c9b55514eda9525f1ee7a.jpg" width="375" height="500">
buuut now the remote wont connect
```

---
## \#40 Posted by: rtasca Posted at: 2016-11-05T00:23:16.749Z Reads: 33

```
I just sprayed beer all over my keyboard ROFLOL
```

---
