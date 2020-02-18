# Did i wire my BMS up right?

### Replies: 50 Views: 818

## \#1 Posted by: Lumaci Posted at: 2018-04-24T16:23:15.050Z Reads: 83

```
Never wired a bms up before wired it up once and fried the BMS took a new one out of the box and tried again.

Before when i wired it up every second wire was negative = No power out of the wire.

Now theres a group of two wires getting the same amount of power, is that wired up right?

![image|666x500](upload://oTSP4Bd51e9aqju4Zzmc7irQUkY.jpg)![30930334_1627156090714245_1784427139_o|666x500](upload://lULKJkEFi7qInkJsPpNmkXiqdfd.jpg)
```

---
## \#2 Posted by: b264 Posted at: 2018-04-24T16:26:58.483Z Reads: 76

```
[quote="Lumaci, post:1, topic:53354"]
Now theres a group of two wires getting the same amount of power, is that wired uo right?
[/quote]

No, it is not correct.  Do not plug that into the BMS.

 Take a closer photo of the top of your cells.
```

---
## \#3 Posted by: Lumaci Posted at: 2018-04-24T16:28:42.483Z Reads: 73

```
![30825369_1627161740713680_471452245_o|375x500](upload://2U9LqoPfgg9Mm7Lsbqf3joFJ4lt.jpg)![30776334_1627161767380344_1276797671_n|375x500](upload://gcZERxzyaJ4HPRU1o7YsxuuzOtq.jpg)![30831798_1627161780713676_1286555768_n|375x500](upload://j6z9l2fKGWYNnLvMR11r2pENo14.jpg)![30430001_1627161814047006_59069732_n|375x500](upload://grh6Sw480MxuDEOEIRPBMgU0FFt.jpg)
```

---
## \#4 Posted by: b264 Posted at: 2018-04-24T16:55:59.465Z Reads: 64

```
I'm confused how the small black balance lead can be at 3.7V.  You're measuring them all relative to the big black battery negative wire, right?
```

---
## \#5 Posted by: dg798 Posted at: 2018-04-24T16:57:31.162Z Reads: 68

```
What cell battery is this? And is this for charge only or discharge as well
```

---
## \#6 Posted by: Lumaci Posted at: 2018-04-24T16:58:28.126Z Reads: 66

```
Old Evolve Bamboo GT Battery pack some prismatic 18650 cells.
```

---
## \#7 Posted by: Lumaci Posted at: 2018-04-24T16:59:00.499Z Reads: 68

```
 measuring them all from the - and + side. i can show you how two sec.
```

---
## \#8 Posted by: Lumaci Posted at: 2018-04-24T17:02:31.007Z Reads: 65

```
Did this on each point, the entire side where theres no balance wires is a negative side the entire side with the balance wires is a positive afaik

![30998378_1627184024044785_934347780_o|375x500](upload://kfJMZzzkBPTEyoP3FAX3G6u63G2.jpg)
```

---
## \#9 Posted by: b264 Posted at: 2018-04-24T17:04:19.828Z Reads: 58

```
No, the entire side with no balance wires is why it's not working for you but I can't suggest how to fix it because the little black wire shouldn't be at 3.7V and I don't know why it's measuring that way
```

---
## \#10 Posted by: dg798 Posted at: 2018-04-24T17:05:10.958Z Reads: 56

```
The black wire should be ground and no voltage and the yellow and white wire that were the same should be different leaving the black as 0
```

---
## \#11 Posted by: b264 Posted at: 2018-04-24T17:05:35.230Z Reads: 52

```
@dg798 Don't confuse him more.  There are two black wires.
```

---
## \#12 Posted by: b264 Posted at: 2018-04-24T17:05:42.731Z Reads: 54

```
You’re measuring them all relative to the big black battery negative wire, right?
```

---
## \#13 Posted by: Lumaci Posted at: 2018-04-24T17:05:51.483Z Reads: 50

```
When i did it so the black wire and other wires were ground the bms instant fried.

Its been plugged in now for like 4 min no smoke.
```

---
## \#14 Posted by: dg798 Posted at: 2018-04-24T17:06:34.627Z Reads: 46

```
Should’ve been a little more specific the black wire on the end of the connector
```

---
## \#15 Posted by: Lumaci Posted at: 2018-04-24T17:06:35.120Z Reads: 45

```
Should i do that? If i do that the voltage is really weird.

Getting 16V on the second last wire.
```

---
## \#16 Posted by: dg798 Posted at: 2018-04-24T17:07:36.350Z Reads: 45

```
I think it would be helpful to take a video of how u are measuring each cell so it’s easier for us to see what’s going on
```

---
## \#17 Posted by: b264 Posted at: 2018-04-24T17:07:57.243Z Reads: 48

```
[quote="Lumaci, post:15, topic:53354"]
Should i do that?
[/quote]

Yes, you have to do it that way and it's why it didn't work the first time
```

---
## \#18 Posted by: Lumaci Posted at: 2018-04-24T17:08:15.161Z Reads: 45

```
Already did hahaha, on its way.
```

---
## \#19 Posted by: Lumaci Posted at: 2018-04-24T17:11:33.156Z Reads: 46

```
https://www.youtube.com/watch?v=1afGmsJUDSU
```

---
## \#20 Posted by: b264 Posted at: 2018-04-24T17:13:05.635Z Reads: 43

```
The problem is that when you check the voltages, you need to keep the black multimeter probe on the fat black battery minus wire and just move the red multimeter probe.  Those wires on the other side are not all negative, those are series connections just like the ones on the opposite side
```

---
## \#21 Posted by: Lumaci Posted at: 2018-04-24T17:16:55.977Z Reads: 40

```
But im getting no readings from the other side and when i do its like 0.8V or 4V or something really low? Hmm.
```

---
## \#22 Posted by: b264 Posted at: 2018-04-24T17:20:14.781Z Reads: 37

```
If you move the black multimeter probe off the fat black battery negative wire, the reading you get will be incorrect
```

---
## \#23 Posted by: Lumaci Posted at: 2018-04-24T17:21:20.310Z Reads: 38

```
That is the reading i get whenever the black wire is on the main black wire on the battery.
I just tested the entire pack getting 40V then 10V 10V 8V 8V 4V 4V on the other side but 16V 24.2V and 36V and 4V on the red side of the pack.
```

---
## \#24 Posted by: b264 Posted at: 2018-04-24T17:22:50.124Z Reads: 37

```
That sounds more correct and shows the little black balance wire is not actually at 3.7V
```

---
## \#25 Posted by: Lumaci Posted at: 2018-04-24T17:23:51.370Z Reads: 39

```
Ive got a video on the way
```

---
## \#26 Posted by: oyta Posted at: 2018-04-24T17:24:53.741Z Reads: 42

```
![IMG_2237|309x500](upload://dAcAja5EXjZIKSqKQo3J00LkjKs.jpg)

There seems to be some wrong wiring here. Why do you have two wires on the same place? Have you drawn a schematic of how you think it should be wired? Is this 10s (seems so according to the voltage)?

![IMG_2239|690x328](upload://zFPVB0O3LOrb65VRkWiulbMLcRN.jpg)

This is an example of how to wire a BMS. Note - it is not certain that this is the same for your BMS.
```

---
## \#27 Posted by: b264 Posted at: 2018-04-24T17:26:16.967Z Reads: 39

```
His cells aren't oriented in the snake pattern but more in the U pattern
```

---
## \#28 Posted by: Lumaci Posted at: 2018-04-24T17:26:45.425Z Reads: 40

```
Yeah i used a guide like that, thats how the first BMS went up in smoke.

I also tried to follow the original wires and when i did that it also wasnt correct, the cloest ive been so far has been this but still dosnt seem correct.
```

---
## \#29 Posted by: Lumaci Posted at: 2018-04-24T17:27:52.268Z Reads: 41

```
https://www.youtube.com/watch?v=a0ZDaeOwB3w
```

---
## \#30 Posted by: b264 Posted at: 2018-04-24T17:27:57.401Z Reads: 39

```
It's not correct, but you need to understand why before fixing it, and it was because you were referencing the voltage measurements to the wrong places.  Always measure the voltage against battery minus
```

---
## \#31 Posted by: b264 Posted at: 2018-04-24T17:29:39.755Z Reads: 41

```
Those measurements are correct, so your first balance lead (small black wire) goes to the 4V measurement, the second balance lead (small light-orange wire) goes to the 8V measurement and so on.  Down one side from B- and then back on the opposite side
```

---
## \#32 Posted by: Lumaci Posted at: 2018-04-24T17:37:16.538Z Reads: 39

```
Okay thanks i just wired it up, one video on its way to make sure its right.
```

---
## \#33 Posted by: Lumaci Posted at: 2018-04-24T17:41:04.646Z Reads: 38

```
https://www.youtube.com/watch?v=fn3hjbkdRhQ
```

---
## \#34 Posted by: b264 Posted at: 2018-04-24T17:43:07.577Z Reads: 36

```
https://www.youtube.com/watch?v=Bt9zSfinwFA
```

---
## \#35 Posted by: Lumaci Posted at: 2018-04-24T17:43:43.013Z Reads: 33

```
hahaha, trust me i tried to record it the right way.

But my phone for some reason prefers to record it vertical.
```

---
## \#36 Posted by: b264 Posted at: 2018-04-24T17:44:29.422Z Reads: 33

```
Yes, that is how they need to be wired.  :slight_smile:
```

---
## \#37 Posted by: Lumaci Posted at: 2018-04-24T17:51:08.966Z Reads: 34

```
Awesome, so it was really just each had to go up by 4? So its 4 8 12 16 20 24 28 32 36 and 40.

Easssy damn.
```

---
## \#38 Posted by: oyta Posted at: 2018-04-24T17:53:43.711Z Reads: 34

```
You also need to wire them the correct way on the connector from B-  towards B+. Not the other way around. It should be stated in the BMS schematics how it should be connected.
```

---
## \#39 Posted by: Lumaci Posted at: 2018-04-24T17:57:20.729Z Reads: 35

```
They are all B+![image|632x500](upload://7Koai0iZldxguIzXPPAziMCt6JP.jpg)


But i did B10 is 40V B9 is 36V B8 is 32V and so on.
```

---
## \#40 Posted by: oyta Posted at: 2018-04-24T17:58:45.709Z Reads: 32

```
That is correct.
```

---
## \#41 Posted by: Lumaci Posted at: 2018-04-24T18:00:29.863Z Reads: 29

```
Hmm something is wrong some where, just plugged it in to charge.

Says its already fully charge when its not.
```

---
## \#42 Posted by: b264 Posted at: 2018-04-24T18:06:37.253Z Reads: 27

```
What voltage is your charger?
```

---
## \#43 Posted by: Lumaci Posted at: 2018-04-24T18:07:39.395Z Reads: 24

```
Its a 42V (10S) 1.5 Amp charger
```

---
## \#44 Posted by: Lumaci Posted at: 2018-04-24T18:11:33.050Z Reads: 23

```
Looks like its charging my bet is its saying its fully charged since the first balance lead is overcharged my guess would be that i need to cycle it a few times before it stops doing it.
```

---
## \#45 Posted by: b264 Posted at: 2018-04-24T18:11:42.740Z Reads: 26

```
[quote="Lumaci, post:39, topic:53354"]
But i did B10 is 40V B9 is 36V B8 is 32V and so on.
[/quote]

this is correct
```

---
## \#46 Posted by: b264 Posted at: 2018-04-24T18:13:55.812Z Reads: 23

```
The first time you charge it it may take a ridiculously long time if it's unbalanced.  Leave it on the charger and keep checking to see if the voltage is climbing.  Like leave it there for 3 hours and see if the voltage went up at all.  Then try 12 hours.  If it's climbing but very very slowly, then it's just balance-charging and that should only happen the first time until the pack gets balanced
```

---
## \#47 Posted by: Lumaci Posted at: 2018-04-24T18:14:50.511Z Reads: 25

```
Yeah exactly what i was thinking, letting it sit for 30 min to check if the voltages has changed.

The main + wire said 42V when i plugged the charger in so it looks like it is charging since its only 40V when i take it out.
```

---
## \#48 Posted by: Lumaci Posted at: 2018-04-24T18:16:47.716Z Reads: 27

```
Yep works thanks, went from 40V to 40.4V now and the rest of the cells thats already at the norm voltage isnt charging.
```

---
## \#49 Posted by: b264 Posted at: 2018-04-24T18:19:24.339Z Reads: 27

```
When the red light turns green, it DOES NOT mean it's done charging.  It means the charger switched from constant current to constant voltage mode.  Typically, for a balanced pack, that means it's ALMOST done charging.  If your pack is way off balance, especially if you just manufactured it, it may need to sit on green for a long time.  The cells are being balanced by the BMS so they are all the same voltage exactly.
```

---
## \#50 Posted by: Lumaci Posted at: 2018-04-24T18:25:27.282Z Reads: 28

```
Exactly, ill keep and eye on the pack for the rest of the day and tomorrow ill give an update to see how well it went.

Just saved 300 bucks and almost able to have a fully working diy board now thanks.

Just one problem, my charging port is a bit to big so need to take it out to fit the pack but worth it.
```

---
