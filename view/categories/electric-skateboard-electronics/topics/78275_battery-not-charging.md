# Battery not charging

### Replies: 38 Views: 851

## \#1 Posted by: Kempo1 Posted at: 2018-12-17T16:50:36.527Z Reads: 121

```
Can anyone help me in figuring out my battery issue? My charger and all battery connections have polarity and read correct voltage. i charged it fine a few days ago. Now the green light on charging box  stays green, and my battery voltage is reading 33 volts but beeps saying its dead. Is this my BMS? ive spent the last two months building my board rode it a few times now having this issue. Please any help would be greatly appreciated.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-17T17:33:46.855Z Reads: 112

```
Which battery you have? 6s, 10s,12s or something else?
Did you measure the voltage of each individual pack? They all have the same voltage?
```

---
## \#3 Posted by: Kempo1 Posted at: 2018-12-17T19:51:57.758Z Reads: 90

```
Mines a 10 s and haven’t checked individual.
```

---
## \#4 Posted by: rsalmon Posted at: 2018-12-17T20:08:04.395Z Reads: 83

```
Sounds like a dead BMS. I had similar symptoms recently and swapping the BMS solved it. Do you have someone you could borrow one to check?
```

---
## \#5 Posted by: Kempo1 Posted at: 2018-12-17T20:28:48.746Z Reads: 80

```
No unfortunately not but I was thinking it was the bms.
```

---
## \#6 Posted by: Kempo1 Posted at: 2018-12-18T04:54:46.340Z Reads: 68

```
Can you by pass the bms
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-18T05:32:39.959Z Reads: 62

```
yes you can bypass the bms, but it´s highly recommended to first check the individual pack voltages to make sure no any of your packs got out of blance.
```

---
## \#8 Posted by: Kempo1 Posted at: 2018-12-18T05:55:58.821Z Reads: 59

```
Ok thanks I’m new to electrical and just been learning and teaching myself. So any knowledge I can pick up is good and appreciate all the help.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-12-18T06:15:24.448Z Reads: 59

```
there could be different reasons why your charger not charging.
your charger is broke, your bms is broke, or something wrong with some cells in your pack.
if something wrong with your cells, than the bms stop charging them up.
if the bms is faulty then your charger also can´t charge the cells up and if the charger is broke...than nu... than your charger is broke :sweat_smile:
i would start meassure each of the 10 packs.
if one is out of the row than you need to change this pack most likely.
if all packs have the same voltage (by +-0.1V) than you can bypass your bms to check if the charger start charging your pack up. 
if that´s the case than it´s definitly your bms and you need to swap the bms out.
```

---
## \#10 Posted by: J0ker3366 Posted at: 2018-12-18T06:18:06.117Z Reads: 54

```
Is your charger plugged into the wall?
```

---
## \#11 Posted by: b264 Posted at: 2018-12-18T07:12:45.513Z Reads: 51

```
You joke about this, but I have a charger that is broken -- it won't charge -- unless you plug it into the skateboard first, then plug the charger into the wall.
```

---
## \#12 Posted by: Sebike Posted at: 2018-12-18T07:26:30.075Z Reads: 50

```
Before swapping bms and cells and whatnot, are you sure you get a good connection between charger and charge plug when plugging in the charger to your board?

Sometimes it's the simplest things...
```

---
## \#13 Posted by: Andy87 Posted at: 2018-12-18T07:32:55.638Z Reads: 49

```
that´s definitly a good point to check first!
we just had one guy here on the weekend where the charging port was boken and that was the reason why the charger didn´t charged anymore.
```

---
## \#14 Posted by: Sebike Posted at: 2018-12-18T07:38:42.005Z Reads: 47

```
Happened to me as I got a new charger that wouldn't turn red. Standard 2.1/5.5, but still had to push it in with some force to get it to start charging.
```

---
## \#15 Posted by: Kempo1 Posted at: 2018-12-18T15:00:29.280Z Reads: 44

```
I’ve checked all connnections and they’re all good and tried plugging it into the board first then the wall that didn’t work. Tried almost everything but checking the individual packs.
```

---
## \#16 Posted by: Kempo1 Posted at: 2018-12-18T17:39:53.997Z Reads: 39

```
It looks like it wants to turn red when I plug it in for a split second but then just stays green.
```

---
## \#17 Posted by: Kempo1 Posted at: 2018-12-18T17:43:39.353Z Reads: 40

```
And do I need to take the entire battery apart to know what type of bms? I know either way I’ll have to to put in the new one but don’t want to do extra work if not needed.
```

---
## \#18 Posted by: Andy87 Posted at: 2018-12-18T19:57:57.043Z Reads: 38

```
plug in the charger (wall and charging port)
Than measure the voltage on the back site of the charging port. Do you measure some voltage there?
```

---
## \#19 Posted by: Kempo1 Posted at: 2018-12-18T20:41:01.270Z Reads: 39

```
i dont have my multi meter with me and hoping to grab it later in the day. I will let you know my outcome appreciate the support and hospitality.
```

---
## \#20 Posted by: Andy87 Posted at: 2018-12-18T20:47:59.291Z Reads: 39

```
It’s time for me to go to bed 😅
Post your results non the less. If nobody will answer you i‘ll have a look in the morning 😉
```

---
## \#21 Posted by: Kempo1 Posted at: 2018-12-19T19:30:09.805Z Reads: 33

```
charging cable does not give any reading from the wall to the box. Can i rule out thagt my problem is the cord?
```

---
## \#22 Posted by: Andy87 Posted at: 2018-12-19T20:17:38.549Z Reads: 33

```
How your charger get green light if you can’t measure any voltage?
Did you change to AC on your multimeter?
```

---
## \#23 Posted by: Sebike Posted at: 2018-12-19T22:48:50.329Z Reads: 34

```
from where to where exactly? 

sounds like you are measuring the cable coming from the wall to your charger only which is probably not the case..
```

---
## \#24 Posted by: Sebike Posted at: 2018-12-19T22:57:37.041Z Reads: 31

```
I'd measure directly on the connector coming from the charger first. Don't cause a short though  lol

If that's fine, next step is to plug it in to your board and as @Andy87 said, measure off the connectors on your charging port (inside of you enclosure) with your battery unplugged. 

Then, I'd replug the battery, unplug your charger, and CAREFULLY measure voltage on you charging port, but I'd do it with one probe on the charging port - and the other directly on your battery +, and then switch to one probe on batt - and other on your charging port +, to minimize the risk of shorting the battery having both probes around the charging port...
```

---
## \#25 Posted by: Kempo1 Posted at: 2018-12-19T23:29:33.526Z Reads: 30

```
i can try doin that sounds a little sketchy for someone whos never done it but as long as probes dont come into contact i should be ok  right? And i was measurung dc volts thank you for the correction.
```

---
## \#26 Posted by: b264 Posted at: 2018-12-19T23:41:28.050Z Reads: 30

```
[quote="Sebike, post:24, topic:78275"]
and CAREFULLY measure voltage on you charging port
[/quote]

Don't do that, you ***will*** short your battery.  Cut a connector and plug it in, then measure on the wires.
```

---
## \#27 Posted by: Sebike Posted at: 2018-12-19T23:42:36.300Z Reads: 27

```
no. even one probe can short your battery if you put it into your charging port. only measure off your port (backside) if you know what you are doing.
```

---
## \#28 Posted by: Sebike Posted at: 2018-12-19T23:45:44.761Z Reads: 26

```
I said - I would.... - I don't recommend that unless he knows how to do it and what he's doing. 

I've measured off the charging port without a problem, but only with one probe
```

---
## \#29 Posted by: Kempo1 Posted at: 2018-12-19T23:50:01.411Z Reads: 26

```
ya if i dont have bad luck i have no luck at all so might have to ask a buddy who does electric to guide me or i dont feel comfortable enough and not enough knowledge without messing something up
```

---
## \#30 Posted by: Kempo1 Posted at: 2018-12-19T23:51:20.069Z Reads: 25

```
one of the solder connections is wore away will that have any effect?
```

---
## \#31 Posted by: Sebike Posted at: 2018-12-19T23:51:59.083Z Reads: 25

```
what solder connection? picture!
```

---
## \#32 Posted by: Kempo1 Posted at: 2018-12-20T00:41:09.216Z Reads: 25

```
![image|375x500](upload://bUMc6lTimJTfMKz6ASVS0XNtuu2.jpeg)
```

---
## \#33 Posted by: Kempo1 Posted at: 2018-12-20T00:42:09.736Z Reads: 25

```
The c - solder spot
```

---
## \#34 Posted by: Sebike Posted at: 2018-12-20T00:47:40.987Z Reads: 25

```
That's where your charger connection would go, so if the wire is no longer connected, you won't be able to charge through your port :grin:

Solder it back (probably a loose black wire coming from the charging port) and give me a "solution" lol
```

---
## \#35 Posted by: Kempo1 Posted at: 2018-12-21T03:56:07.538Z Reads: 23

```
ok i will try that tonight. whats the reading from the end of the charging cable from box to the board connection its reading .02?
```

---
## \#36 Posted by: b264 Posted at: 2018-12-21T04:11:58.572Z Reads: 23

```
Those C- and P- are cold solder joints.  It either wasn't hot enough or no resin was used, or both
```

---
## \#37 Posted by: Kempo1 Posted at: 2018-12-21T05:00:34.323Z Reads: 23

```
ok thanks it was from the factory is it possibal to resolder it and try it?
```

---
## \#38 Posted by: b264 Posted at: 2018-12-21T05:00:51.929Z Reads: 23

```
I would resolder it, definitely
```

---
