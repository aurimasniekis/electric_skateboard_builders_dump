# Problems with batteries

### Replies: 88 Views: 1438

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:34:52.255Z Reads: 173

```
About a year ago I built my esk8 and it was great, I went for a pretty cheap first build with options to upgrade. But there's one problem I can't seem to solve ever since the start:
When the board was running, for some reason, only one cell from one battery emptied (got to 1.7v once) and the board became too slow to ride after that. I contacted Hobbyking and they sent another battery, and when I sautered and connected the new one, a different problem appeared - power is only withdrawn from one battery until each cell is around 2.7V and the board gets too slow to ride.
The batteries I'm using are two of these:
https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html
They're connected in series using this connector:
https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-series.html?___store=en_us
The connections I'm using are XT90's which I soldered to the batteries and the esc.
Also using an anti-spark XT90 loop key:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204
So my question is what is causing this? can I fix it or do I need to get another battery? I don't think its likely that I would get 2 faulty batteries in a row.
I can post pictures and a more detailed explanation of the parts and how they are connected if it's needed.
Thanks
```

---
## \#2 Posted by: Ishayc Posted at: 2018-04-09T10:39:41.493Z Reads: 140

```
Are you charging/discharging through a BMS?
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:43:22.496Z Reads: 139

```
No, through a normal IMAX charger:
https://hobbyking.com/en_us/imax-b6-dc-charger-5a-50w-copy.html
Using the cable that came with the charger, and soldered the XT90 connector to the other side, thing is, the cable is pretty thin, can that be a problem?
```

---
## \#4 Posted by: Ishayc Posted at: 2018-04-09T10:46:13.597Z Reads: 130

```
It happens during discharge, not charge so the charging cable is not the problem.
What esc are you using?
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:48:09.497Z Reads: 126

```
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html?___store=en_us
if getting a VESC will solve it, ill buy one right away, i was thinking of getting one for a while now
```

---
## \#6 Posted by: Ishayc Posted at: 2018-04-09T10:49:57.109Z Reads: 113

```
You are connecting two 5 cells batteries in series which is 10 cells to a 6 cells esc?
Connect them in parallel


Edit: though it was 5 cells.
```

---
## \#8 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:51:51.925Z Reads: 109

```
Any other ideas?
```

---
## \#9 Posted by: telnoi Posted at: 2018-04-09T10:52:23.115Z Reads: 103

```
Got the same lipos and connector (though I am using 4). No issues. 

I would measure the output voltage to see if it is 6S if the lipos are fully charged. Keep measuring the output voltage when you apply throttle. Does it drop suddenly? What happens? What if you move the cables?
```

---
## \#10 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:53:28.793Z Reads: 102

```
how do i check the voltage? usually to check the cells i use my charger, do i need something else for that?
```

---
## \#11 Posted by: Ishayc Posted at: 2018-04-09T10:54:27.996Z Reads: 101

```
Take a voltmeter and see that the series cable is ok first.
Are you sure you are getting the power of 6s and not only 3s? you can say by the speed.
```

---
## \#12 Posted by: telnoi Posted at: 2018-04-09T10:54:48.229Z Reads: 96

```
volt meter or multi meter. With a multimeter, you can also measure the resistance of the cables, thus check if they are ok.
```

---
## \#13 Posted by: Acidfie Posted at: 2018-04-09T10:54:53.147Z Reads: 94

```
this is a **physical problem**. if both batteries are connected there is **NO** way they are not discharged both
```

---
## \#14 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:56:17.782Z Reads: 91

```
I weigh about 80kg and i get at least 20kph so Im pretty sure its all 6 cells
```

---
## \#15 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:56:57.701Z Reads: 90

```
Alright, so what do you suggest i do? resolder everything?
```

---
## \#16 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:57:22.382Z Reads: 92

```
dont really have one lying around lol 
ill just get one on ebay
```

---
## \#17 Posted by: Ishayc Posted at: 2018-04-09T10:58:25.074Z Reads: 87

```
Checking the resistance is a good idea as @telnoi suggested.
You can upload a photo of the soldering job you did, we might spot something.
```

---
## \#18 Posted by: ShakeNBake7000 Posted at: 2018-04-09T10:58:37.550Z Reads: 90

```
I can post pictures of the connections if needed, not at home right now though
edit: i will in a few hours
```

---
## \#19 Posted by: Acidfie Posted at: 2018-04-09T10:58:47.875Z Reads: 90

```
too high resistance anywhere from the battery that is not getting discharged.

please provide gearing ratio, wheel size for calculating maximum speed so we can see if your value is correct
```

---
## \#20 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:00:11.574Z Reads: 89

```
wheels are 90mm, need to check about the gears
```

---
## \#21 Posted by: ARetardedPillow Posted at: 2018-04-09T11:02:44.538Z Reads: 78

```
You should never discharge lipo under 3.2 volts
```

---
## \#22 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:06:11.490Z Reads: 72

```
total or per cell?
```

---
## \#23 Posted by: Acidfie Posted at: 2018-04-09T11:06:34.111Z Reads: 70

```
per cell

10char
```

---
## \#24 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:06:51.380Z Reads: 76

```
Here are the details:
Specification:
Name: Skateboard component
Model: 512181
Color: Black and silver
Material: Surface oxidation+stainless steel
Gear of wheel: 36 tooth
Gear of motor: 12 tooth
Bore of wheel: 21mm
Bore of motor: 8mm
Round hole diameter of motor mount: 19mm
Motor mount width: 15mm
Motor mount length: 131mm
Belt width: 11mm
Belt length: 270mm



hope it helps
```

---
## \#25 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:07:52.656Z Reads: 75

```
but the max per cell when i charge is around 4 so its not even a quarter of the actual battery capacity.
when i ride it around, it usually goes a few kilometers and then stops, one battery is full (3.7, 3.7, 3.7) and the other is (2.7, 2.7, 2.7) considering what youre saying that is really bad
```

---
## \#26 Posted by: Rinzler Posted at: 2018-04-09T11:09:54.073Z Reads: 69

```
The series cells in the indivdual battery have different resistance and they are all different. Cells with low resistance get drained faster and sag a lot more, also age faster so the problem is in the cheap zippy packs.
```

---
## \#27 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:11:01.614Z Reads: 67

```
wow, when i first picked the items people here suggested those exact batteries
rip
```

---
## \#28 Posted by: telnoi Posted at: 2018-04-09T11:12:19.244Z Reads: 71

```
ehmm, no...
Cell drift of 0.3v MAX on 4 different zippies at 50A VESC bat draw...
They can't be that bad, across 3 cells no less.
```

---
## \#29 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:13:23.036Z Reads: 68

```
Sorry, im kind of new to this, didnt really understand what you meant
and im not using a vesc, im using a remote car ESC
```

---
## \#30 Posted by: ARetardedPillow Posted at: 2018-04-09T11:16:30.754Z Reads: 68

```
Your max for each cell is supposed to be 4.2 volts -+0.01volts, and your minimum should really be around 3.3-3.4, 3.2 volts is borderline, any more and you're damaging your batteries
```

---
## \#31 Posted by: telnoi Posted at: 2018-04-09T11:16:34.404Z Reads: 68

```
When fully charged, your lipos should be 4.2V (min 4.18/19 with bad balancing). If they are not on both lipos, your charger settings or charger is messed up. 

A cell drift of 1V after riding is absolutely ridiculous. I have never seen that happen with my 4 zippies (they are 5s). The maximum cell drift I ever got at 70% discharge was 0.3V. That's with 4 different lipos, 20 different cells.
```

---
## \#32 Posted by: ARetardedPillow Posted at: 2018-04-09T11:17:39.239Z Reads: 63

```
What amp do you charge them at and what voltage? And what in mode do you charge them?
```

---
## \#33 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:18:16.287Z Reads: 63

```
wow, so its really busted then? when i charge at 5 amps in the charger it only goes to about 3.8-4V and then stays there
```

---
## \#34 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:19:28.602Z Reads: 60

```
I charge at 5 amps which is the max of the charger and in the balance/normal charge mode
not sure at what voltage, where does it show the voltage?
```

---
## \#35 Posted by: telnoi Posted at: 2018-04-09T11:19:48.459Z Reads: 56

```
does it ever say that the charge cycle is completed? Depending on the charger, balancing the packs and going to full 4.2V can take a long time. My old charger needed about 30 minutes to balance all cells.
```

---
## \#36 Posted by: ARetardedPillow Posted at: 2018-04-09T11:20:38.549Z Reads: 58

```
You really shouldn't charge them at 5 amps if you're trying to use your batteries for more than a month, if your voltage only goes up to 3.8-4.0, I would say something is wrong, get new batteries, if the same thing happens again, toss your charger
```

---
## \#37 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:20:52.894Z Reads: 56

```
it takes it 5 mins to charge up to 3.8-4 and then stays there, i left it on balance for 2 hours and nothing
```

---
## \#38 Posted by: ARetardedPillow Posted at: 2018-04-09T11:21:32.662Z Reads: 56

```
Okay it should really take a lot more than 5 minutes to charge your batteries, this is ridiculous

From what I'm seeing, you're treating your batteries like shit
```

---
## \#39 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:21:49.465Z Reads: 51

```
Damn, alright ill try to look at some different batteries, anything you know is reliable?
```

---
## \#40 Posted by: telnoi Posted at: 2018-04-09T11:22:15.578Z Reads: 54

```
ok..first guess is charger issues (see if you can check another lipo/different charger), second cable/soldering/resistance issues. Third, defective lipo.

Charge your stuff at the recommended C rate.
8000 mah lipo can be charged at 8A, which is 1C. Well within the limits.
```

---
## \#41 Posted by: ARetardedPillow Posted at: 2018-04-09T11:23:19.327Z Reads: 52

```
I used to use zippy and turnigys without a problem before I switched to liion and they were pretty damn reliable, there's definitely something wrong with your setup, send pics
```

---
## \#42 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:23:44.904Z Reads: 50

```
A lot of people are telling me a lot of different stuff right now, is it the resistance or the charger or the soldering or are the batteries just busted, im new to this and its confusing
```

---
## \#43 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:24:41.774Z Reads: 48

```
yeah i used 5 amps because i asked on some other post and thats what they recommended
```

---
## \#44 Posted by: telnoi Posted at: 2018-04-09T11:24:59.076Z Reads: 48

```
Yup, 5A is completely fine..
```

---
## \#45 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:25:16.735Z Reads: 49

```
in about an hour i will send pictures of everything, i really want to fix it
```

---
## \#46 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:26:05.332Z Reads: 45

```
thanks for all the replies guys, not sure how to fix it yet but when i send pictures mabye it will become easier to pinpoint the problem
```

---
## \#47 Posted by: Tuomalar Posted at: 2018-04-09T11:28:53.178Z Reads: 49

```
This conversation is a little messy right now but lets clear some things. 

1. Your batteries are wasted and i recommend to buy new ones. Zippys are great and your zippys probably broke due to user error.

2. Your charger is broken or your settings are wrong. Check settings and show them to us, if those are okay buy a new charger.
```

---
## \#48 Posted by: ARetardedPillow Posted at: 2018-04-09T11:31:13.527Z Reads: 47

```
And don't take the battery resistance info for now, theres absolutely no way brand new batteries can be THAT BAD unless they're screwed up in some way. Worry about the 2 things above
```

---
## \#49 Posted by: ShakeNBake7000 Posted at: 2018-04-09T11:34:34.397Z Reads: 49

```
alright ill check some stuff when i get home, thanks
Edit: just wondering, how could i have avoided "destroying" the batteries? they were like this from the start, so im not sure what i could have done
```

---
## \#50 Posted by: Tuomalar Posted at: 2018-04-09T12:01:13.510Z Reads: 50

```
For example wrong values in charger or broken charger can do that.
```

---
## \#51 Posted by: ShakeNBake7000 Posted at: 2018-04-09T14:47:57.257Z Reads: 51

```
Alright, I took some pictures of the charger settings and how i charged it, i hope it helps.
settings (those are the defult settings):
![53 PM|375x500](upload://vLXeyWXFdPFGxFUBDPeirqy3uLj.jpeg)
![53 PM (2)|375x500](upload://98M8p4fiTimc4pc84CP2JyNkMYQ.jpeg)
![53 PM (1)|375x500](upload://1BHzuhu0NUOMJnkWV8OpVf8lOhG.jpeg)
![53 PM (4)|375x500](upload://6ATfjKCriSg381TQgkTO8V4WwGk.jpeg)
![53 PM (3)|375x500](upload://6aCY80a8VkYp98UbZfZskN57yz6.jpeg)
![53 PM (5)|375x500](upload://q4yLDzT8oG9QHs6TTCU7efVNtBM.jpeg)
 And how i charge it:
![53 PM (6)|666x500](upload://eQlH8zB8BoH3X9FnAJMIGK4SyIN.jpeg)
![53 PM (7)|666x500](upload://6M0uM0BZcbvr95gVXeFylB8IMPJ.jpeg)
On the last pic i just hold start and the charging starts
If this is not enough i would be more than happy to send more, just need to know what you need.
Thanks
Edit: sorry some of the pictures are not stright, i didnt realise it when i was taking them
```

---
## \#52 Posted by: Acido Posted at: 2018-04-09T14:59:10.832Z Reads: 43

```
Get a bms or a voltage alarm for the next batteries if you can not "fix" these
```

---
## \#53 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:06:55.415Z Reads: 41

```
I was thinking of getting a bms, which one do you recommend?
```

---
## \#54 Posted by: Tuomalar Posted at: 2018-04-09T15:09:50.522Z Reads: 41

```
If I'm correct that 22.2V should be 25.2V? (4.2x6) do you use balance leads? In the picture, I can see only 3s balance cable.
```

---
## \#55 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:10:47.475Z Reads: 43

```
im using a balance adapter from two 3s's to one six. in the picture i was just testing one battery so it wasnt connected
looks like this:
https://hobbyking.com/en_us/2-x-3s-gt-6s-splitter-jst-xh-5pcs-bag.html?___store=en_us
```

---
## \#56 Posted by: Acido Posted at: 2018-04-09T15:11:53.497Z Reads: 43

```
bestech is IMO the most used here
```

---
## \#57 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:13:28.645Z Reads: 44

```
There are so many models, is a PCM the same as BMS or is it something completely different?
i found the 6s section, but cant really make out any differences between them
http://bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/
```

---
## \#58 Posted by: Acido Posted at: 2018-04-09T15:21:57.639Z Reads: 42

```
see the discharge rating, dimenisons, communications...
yes the pcm is a bms
```

---
## \#59 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:25:06.507Z Reads: 41

```
the continues current is how fast it charges?
```

---
## \#60 Posted by: Acido Posted at: 2018-04-09T15:27:27.983Z Reads: 43

```
BMSs have charging and discharging rates

Charging thru it is one lets say 15a maximum
Discharging is lets say 80A

So you can charge the batteries with a max 15A charger and discharge the batteries maximum 80a thru it
```

---
## \#61 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:32:04.917Z Reads: 41

```
oh alright, but the batteries have a "max" amps they can be charged and discharged at too, right?
```

---
## \#62 Posted by: Acido Posted at: 2018-04-09T15:35:27.669Z Reads: 37

```
Yes, its declared in their specs ;)
```

---
## \#63 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:39:43.406Z Reads: 37

```
Alright, thanks ill look around some more and check my battery's max
```

---
## \#64 Posted by: wafflejock Posted at: 2018-04-09T15:46:51.197Z Reads: 39

```
Pretty sure my charger uses the same software, when actually charging try hitting the arrow key to see the individual cell charges.  You never want to charge a LiPo at more than 1C or 1 times its capacity in Ah, so if you have a 3Ah battery 3A should be the maximum charge current set on the charger (for the safety of the battery and anything around it).  The charger should end with showing 'full' and the mAh put into the battery at the end of the charge cycle.

As to the original issue as others have said there is likely some sort of connection issue if you aren't seeing power pulled from cells then they aren't connected to the circuit show us pics of the wiring between the batteries and the ESC (actual pics not product pics)
```

---
## \#65 Posted by: ShakeNBake7000 Posted at: 2018-04-09T15:52:29.485Z Reads: 38

```
alright, taking pictures
```

---
## \#66 Posted by: ShakeNBake7000 Posted at: 2018-04-09T16:27:35.127Z Reads: 42

```
Sorry it took a while, phone ran out of battery, here is the actual wiring of the board:
![36 PM|463x500](upload://jDE2qfKfUSzqgSVVIO6VgIEssbV.jpeg)
![36 PM (2)|375x500](upload://oCFAJnLkgivPduUyYiQys09BnaD.jpeg)
![36 PM (3)|375x500](upload://9VDIhPw10mUBJ6xJ2myHYgIXEuU.jpeg)
![36 PM (4)|375x500](upload://s3Vlsv9iMNG22Q4zKqLiasBD6Z3.jpeg)
![36 PM (5)|375x500](upload://j2iVGlQbQK3qQ5ysT7GKWXV3GI.jpeg)
```

---
## \#67 Posted by: wafflejock Posted at: 2018-04-09T17:15:46.635Z Reads: 38

```
Okay nothing obvious in the pics wrong (possibly issues in the connections themselves/soldering the wire to the xt-90s but seems pretty unlikely).  Are you able to see the individual cell voltages when you hook the batteries up choose charge then hit the arrow key? would be nice to see pics of those per cell voltages on each battery just to see where things stand right now.  When manufacturers make the battery packs they match the internal resistance across groups of cells so each cell in a given pack will have roughly the same internal resistance, in theory all the 30C or whatever C rating cells have the same internal resistance but the IR will increase over time as the cells are used so older cell may end up with higher IR than newer ones.  IR is just the same as any other resistance except it's the resistance in the battery itself, if you have higher resistance it will resist the flow of current and produce heat as a result (higher resistance or higher current equals more loss).

The only way it can be really pulling only charge from one battery in your case is if the resistance is so high between one of the batteries and the rest of the circuit that no charge is pulled through/from the battery but since they are connected in series that can't possibly be true (kirchoffs law basically states same current going in one side comes out the other).

Anyhow long story short I'm still confused as to what's going on, but would help if we can all see the individual voltage on the cells to maybe.
```

---
## \#68 Posted by: ShakeNBake7000 Posted at: 2018-04-09T17:32:51.731Z Reads: 39

```
[quote="wafflejock, post:67, topic:51678"]
ps of cells so each cell in a given pack will have roughly the same internal resistance, in theory all the 30C or whatever C rating cells have the same internal resistance but the IR will increase over time as the cells are used so older cell may end up with higher IR than newer ones.  IR is just the same as any other resistance except it’s the resistance in the battery itself, if you have higher resistance it will resist the flow of current and produce heat as a result (higher resistance or higher current equals more loss).

The only way it can be really pulling only charge from one battery in your case is if the resistance is so high between one of the batteries and the rest of the circuit that no charge is pulled through/from the battery but since they are connected in series that can’t possibly be true (kirchoffs law basically states same current going in one side comes out the other).

Anyhow long story short I’m still confused as to what’s going on, but would help if we can all see the individual voltage on the cells to maybe.
[/quote]

Alright, so right now i just charged both batteries in series on balance mode for about an hour, and this is the cell situation:
![32 PM|666x500](upload://cbK7cqu5eakwmzEZ0bGEGMOBHLX.jpeg)
![32 PM (1)|666x500](upload://9s1vHMHJOLn6TTpXFBvRiePciXg.jpeg)

At this state it takes ages for it to go up 0.05v so this is basically the max I can charge for this setup and current batteries.
If you want, I can connect the packs to the board and just run the motor on idle to discharge the batteries and see what cells/battery gets drained
you can still see that the battery that was drained first has a little less voltage in it, mabye it can tell you something about the problem?
Thanks
```

---
## \#69 Posted by: telnoi Posted at: 2018-04-09T17:48:07.888Z Reads: 34

```
It all looks a bit botched together. Uncertain if you hooked up your balance leads correctly to the charger. Does a single 3s charge correctly using an original balance cable?
```

---
## \#70 Posted by: wafflejock Posted at: 2018-04-09T17:55:43.468Z Reads: 33

```
Would go with what @telnoi said as well just hook up directly with the original balance cable each battery individually and try to charge that way.  If the cells are too out of whack voltage wise and you try to do the 'balance charge' I'm pretty sure it will attempt to drain charge out of whatever cells are too high, perhaps it is stuck attempting to drain charge from the higher cells/battery and attempting to push power into the entire battery is resulting in the ones with lower IR to get pumped up more and therefore out of balance again.  I'd charge both batteries individually up to 4.2V if possible then try hooking them up and do a discharge test on the board (run it for a few minutes) then check the voltage on all the cells again to see how far they've drifted from each other and how much they've dropped from 4.2V (typically most of the mAh [juice] is in the 3.6-3.8 range so will generally drop in voltage pretty quickly from 4.2 to near 3.8 and most of the 'life' of the battery will be in that range of 3.6-3.8V)
```

---
## \#72 Posted by: ShakeNBake7000 Posted at: 2018-04-09T17:59:35.942Z Reads: 32

```
Alright, ill try that, and telnoi, im sure i connected it correctly because i made a post about it asking how to do it and they said its good, ill try to charge them alone now, what mode should i use? normal charge? fast charge? or balance?
```

---
## \#73 Posted by: wafflejock Posted at: 2018-04-09T18:00:02.120Z Reads: 33

```
Do balance charge but yeah just 1 of the 3S at a time.
```

---
## \#74 Posted by: ShakeNBake7000 Posted at: 2018-04-09T18:05:12.590Z Reads: 32

```
ok, charging now at 5 amps
(shows 4.2A actual charge)
```

---
## \#75 Posted by: wafflejock Posted at: 2018-04-09T18:05:58.158Z Reads: 33

```
Yeah the 5A you set is a maximum it will typically show less amps drawn as it gets closer to actually fully charged so nothing to worry about there.
```

---
## \#76 Posted by: ShakeNBake7000 Posted at: 2018-04-09T18:16:32.264Z Reads: 33

```
its been 10 mins and it went from
3.84 3.84 3.83
to
3.95 3.97 3.95

pretty slow but going up
```

---
## \#77 Posted by: wafflejock Posted at: 2018-04-09T18:22:12.846Z Reads: 33

```
Yeah for 8Ah capacity charging at 5A it will take 8/5 = 1.6hrs (96 minutes) to charge from empty (around 3.5-3.6V) when putting them in series you are charging up at a higher voltage but the amperage and time should stay the same so long as you aren't changing the capacity (Ah) or the charge rate (A).  I'd guess you have about 20-30 minutes left to get it fully charged (tends be slower at the end since the current is going lower as the voltages get closer to each other... that is what the charger is putting out and what the battery is currently at, the voltage difference between the two is ultimately what determines the amperage).
```

---
## \#78 Posted by: ShakeNBake7000 Posted at: 2018-04-09T18:28:51.462Z Reads: 34

```
ok that makes sense, thanks for explaning, makes me feel a little better knowing the long wait time is normal and that thats not another problem i have to deal with
```

---
## \#79 Posted by: riva_00 Posted at: 2018-04-09T18:59:56.743Z Reads: 33

```
@ShakeNBake7000
Just skimmed through this thread and looks like you're getting lots of help here, no need for me to add anything technical, however can i check that at this point you're charging in LiPo safe bags with possibly a fire extinguisher nearby.

I don't expect you'll need them, but i have that stuff even with batteries that i consider to be in top-notch condition, and these look like they've been through a bit. Not many people have the fire extinguisher, but a LiPo safe bag at this point is a must. Use it when charging please.
```

---
## \#80 Posted by: ShakeNBake7000 Posted at: 2018-04-09T19:07:57.643Z Reads: 31

```
Well, i dont have a safe bag, you mind linking me one? ill buy it right now if its not expensive, and either way i never charge without me being there to watch it if something happens
```

---
## \#81 Posted by: ShakeNBake7000 Posted at: 2018-04-09T19:14:07.528Z Reads: 32

```
battery seems to be stuck at 
4.18 4.20 4.17
0.2A
ill just start charging the other one
```

---
## \#82 Posted by: riva_00 Posted at: 2018-04-09T19:22:43.822Z Reads: 30

```
that's the charger balancing the voltages, let it finish. It's at 0.2A as it's fine-tuning the voltages, most of the work is done at the end of a charge cycle when balancing.

£3 for a bag that'll prevent a LiPo fire, jumbo version, this shouldn't be a secondary concern.
https://hobbyking.com/en_us/lithium-polymer-charge-pack-25x33cm-jumbo-sack.html

*get 2
```

---
## \#83 Posted by: Acido Posted at: 2018-04-09T19:41:16.348Z Reads: 29

```
nah just put it in front of your house
if it blows up nothing happens, just some black concrete lol
```

---
## \#84 Posted by: wafflejock Posted at: 2018-04-09T20:28:18.955Z Reads: 31

```
yeah if they don't ever all get to 4.20 it may get stuck so long as they are within a few hundredths of a volt of each other it should be okay.  The problem is basically say for argument sake one cell is at 3.8V while another is at 4.0V if both are otherwise equivalent and we discharge from both at the same time and at the same rate (current) then the one with 3.8V will get below the safe low voltage on a LiPo (typically around 3.4-3.3V) before the one that was charged to 4.0V.  Once the low cells get past the 'voltage cliff' they typically can't be charged again or if they can be revived it's temporary and with overall increased resistance and shorter total cell life.

Scan through for the images here to see what I mean about the 'voltage cliff' (drawing doesn't show it but continues down to 0V very steep drop off there below 3V)

https://endless-sphere.com/forums/viewtopic.php?t=52240
```

---
## \#85 Posted by: wafflejock Posted at: 2018-04-09T20:29:28.270Z Reads: 31

```
Regarding safe charging I typically go with a "lipo safe" bag too might end up getting one of these boxes too though seems nice/convenient and purpose made (if a bit pricey) https://hobbyking.com/en_us/bat-safe-lipo-battery-charging-safe-box.html
```

---
## \#86 Posted by: ShakeNBake7000 Posted at: 2018-04-09T20:58:03.037Z Reads: 33

```
Wow, so I just charged them both back up to 4.20 except a few cells (4.17,4.15), then I held down the controller for around five mins and all of them dropped together, not one cell or one battery, all of them! I'm not sure it will stay that way but for now its good, thank you for all the help, it's really appreciated, I would be lost without everyone's help.
I'll get two of the safe bags to be safe and mabye get a bms soon, still not sure which one to get.
So again, thank you so much I will test it better tomorrow and see if everything is good because at one point I had a cell at 1.4V (lol) hope that didn't damage the battery permanently. 
Thank you.
```

---
## \#87 Posted by: ShakeNBake7000 Posted at: 2018-04-11T10:18:03.870Z Reads: 25

```
Finally got to ride around the city and its great, I rode for around 2-3 km just to check if everything is fine and it dropped from 4.20 per cell to 4.05 
I was wondering what is the lowest I can go before its bad for the battery?
trying to calculate my max km with full battery
```

---
## \#88 Posted by: FredrikHems Posted at: 2018-04-11T13:22:09.453Z Reads: 23

```
You will damage the battery permanently if you go lower than 3.2-3v per cell, but it you want to have your batteries for as long as possible don't go lower than 3.6v per cell.
```

---
## \#89 Posted by: jmapark91 Posted at: 2018-04-11T14:23:13.757Z Reads: 25

```
Hi,

I also own an Imax B6AC charger, and yesterday I was charging my 6S battery.
It was working all fine for 2 hours or so and the batteries reached its max voltage (25.2V), then suddenly white smoke started coming out of a small gap between the LCD and the charger casing, so I immediately unplugged everything. My first cell in the series is now completely dead.

The charger.. how do I tell if it's fried? The LCD works, all the buttons work, and now if I connect my batteries it says low cell voltage (since 1 cell is dead). Would you guys say the charger is probably still okay to use or don't risk anything and get a new charger?

Any help is appreciated..
```

---
## \#90 Posted by: FredrikHems Posted at: 2018-04-11T14:31:54.475Z Reads: 25

```
I would suggest you to start your own topic. You will get more help then.
```

---
