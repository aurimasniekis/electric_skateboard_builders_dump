# FOCBOX flashing fault repreatly

### Replies: 47 Views: 2188

## \#1 Posted by: trancejunkiexxl Posted at: 2017-08-18T01:39:30.610Z Reads: 169

```
getting this flashing redlight, can still connect but no power to wheels.. I think I broke it...
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-08-18T01:40:56.659Z Reads: 169

```
Oh boy.... I'm getting less and less happy about buying two of them for this build.
```

---
## \#3 Posted by: JLabs Posted at: 2017-08-18T01:42:34.806Z Reads: 170

```
Type “fault” in the faults tab to see what comes up.
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-08-18T01:43:28.679Z Reads: 159

```
And post screenshots of your settings.
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2017-08-18T02:16:44.802Z Reads: 152

```
FAULT_CODE_DRV8302 is the error
```

---
## \#6 Posted by: scepterr Posted at: 2017-08-18T02:18:16.387Z Reads: 152

```
Failbox is a more appropriate name than focbox
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-08-18T02:20:20.448Z Reads: 150

```
is there nothing I can do other than buy a new unit.. this one only had 10miles on it
```

---
## \#8 Posted by: scepterr Posted at: 2017-08-18T02:21:32.945Z Reads: 151

```
Yeah mine had about the same mileage before crapping out, you can get the DRV replaced.
```

---
## \#9 Posted by: evoheyax Posted at: 2017-08-18T02:40:59.625Z Reads: 151

```
So enertion still has DRV issues?


Chaka 4.12 is still the most reliable IMO. Never fails, and if you make a big enough heat sink, you can do the same as the FOCBOX in performance.
```

---
## \#10 Posted by: flywithgriff Posted at: 2017-08-18T02:44:32.654Z Reads: 145

```
Three weeks ago.. FOCBOX is the best... I bought two!

Now.. FOCBOX are dying in foc... I cry myself to sleep!
```

---
## \#11 Posted by: scepterr Posted at: 2017-08-18T02:47:29.299Z Reads: 141

```
Here's the thing though, it could be some kind of defect/manufacturing fault that's making recent focboxs fail but since the only "warranty" option is to buy another for $80. We'll never know unless enertion discovers something and admits it.
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-08-18T02:49:41.075Z Reads: 142

```
They can't even fix a sticker issue!!!
```

---
## \#13 Posted by: scepterr Posted at: 2017-08-18T03:02:35.320Z Reads: 142

```
I hope we didn't get this batch, I rebuilt mine just to be sure :neutral_face: https://www.electric-skateboard.builders/t/raptor-2-most-powerful-direct-drive-electric-skateboard-kickstarter/12694/1954<img src="/uploads/db1493/original/3X/e/6/e62fa1138a1a1cd2a1ecbc1c25029bdaea226809.jpg" width="281" height="500">
```

---
## \#14 Posted by: trancejunkiexxl Posted at: 2017-08-18T03:03:34.700Z Reads: 138

```
ya im super bummed, I really liked mine =(
```

---
## \#15 Posted by: scepterr Posted at: 2017-08-18T03:17:44.711Z Reads: 140

```
The focbox and esk8.de ESC are nearly identical physically and identical in performance. EXCEPT esk8.de lists all upgraded components and advises AGAINST FOC even so far as saying using FOC will void your warranty. Now knowing all that I would of course not buy it for the purposes of using FOC at least not in the warranty period since they were nice enough to say it will likely break the esc. Expectations set and met, that's how you run a business. 
https://store7570530.ecwid.com/#!/Original-ESK8-controller-1-1-mit-direct-Fet´s-Made-in-Germany/p/88140891/category=15255004
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2017-08-18T03:22:49.060Z Reads: 134

```
Nha this batch as never see the light of days...
```

---
## \#17 Posted by: scepterr Posted at: 2017-08-18T03:25:32.436Z Reads: 137

```
Then it just leaves FOC as the silent killer :smirk:
```

---
## \#18 Posted by: trancejunkiexxl Posted at: 2017-08-18T03:32:26.175Z Reads: 134

```
I was running bldc mode
uncensored
```

---
## \#19 Posted by: scepterr Posted at: 2017-08-18T03:33:24.455Z Reads: 133

```
Hmm curious
Is it a sensored motor/were sensor wires plugged in?
```

---
## \#20 Posted by: JLabs Posted at: 2017-08-18T03:39:49.532Z Reads: 132

```
Post some screnshots.. maybe you had the old buggy firmware?
```

---
## \#21 Posted by: Namasaki Posted at: 2017-08-18T05:13:46.181Z Reads: 120

```
Please post more info about your setup. It will be very helpful to others.
voltage
motor KV
bldc settings
```

---
## \#22 Posted by: trancejunkiexxl Posted at: 2017-08-18T05:16:06.846Z Reads: 121

```
will do, it was my first run at a dual setup, so all values were halved.. had to call it a night but will follow up.. I ended up pulling the unit out also, batt max was at like 20 and motor max was something like 32.. still using 12s2p battery on TB6355's still sheding tears gotta mail it 2 Johnny..  =/
```

---
## \#23 Posted by: Namasaki Posted at: 2017-08-18T05:29:37.966Z Reads: 120

```
Some causes of blown drv's

motor Kv too high for voltage
Ramp step bug ( this issue was addressed long ago)
Shorting of motor phase wires, either external or inside the motor.
```

---
## \#24 Posted by: karma Posted at: 2017-08-18T11:26:41.998Z Reads: 118

```
Seems like FOCBOXes are blowing up everywhere. I just recieved 2x, I read about the risks with CAN. Any other hard to think about misstakes to avoid?
```

---
## \#25 Posted by: trancejunkiexxl Posted at: 2017-08-18T11:27:06.324Z Reads: 122

```
I was using split ppm safer imo
```

---
## \#26 Posted by: Namasaki Posted at: 2017-08-18T17:03:39.625Z Reads: 110

```
I prefer split PPM over canbus 
I think it's more reliable and no risk as long as you clip one of the 5v wires. 
We are currently testing the dual receiver with single controller concept which affords highest redundancy with no risk to Vesc.
```

---
## \#27 Posted by: Jinra Posted at: 2017-08-18T17:05:44.364Z Reads: 106

```
I wonder how this will affect Raptor 2 owners in the near future..

@Namasaki according to trampa, the world may end if you use split Y on the VESC
```

---
## \#28 Posted by: trancejunkiexxl Posted at: 2017-08-18T17:15:22.940Z Reads: 105

```
if it hadn't had been for the fact i was running dual motors, i would have ate it big, i was going down hill max speed when i felt the focbox die.. there was a huge jerk, and then i coasted and realized it was burnt toast
```

---
## \#29 Posted by: deucesdown Posted at: 2017-08-18T17:18:38.623Z Reads: 104

```
Is it just the China batch that's dying? Are the earlier US ones holding up better?
```

---
## \#30 Posted by: JLabs Posted at: 2017-08-18T17:26:12.844Z Reads: 104

```
I would assume so as the recent batch was the only ones from China.. (China dosnt mean bad quality tho). With the new MFG they may not have got some really small detail wrong and now there are problems..

I have ridden 2 focbox in FOC (new batch) for a while now with no problems.. so it could be settings, who knows
```

---
## \#31 Posted by: trancejunkiexxl Posted at: 2017-08-18T17:32:44.776Z Reads: 102

```
ya my other unit is holding up just fine.. gotta refine and build it again..
just one hell of an expensive lesson
```

---
## \#32 Posted by: Namasaki Posted at: 2017-08-18T18:16:08.310Z Reads: 102

```
[quote="Jinra, post:27, topic:30938"]
@Namasaki according to trampa, the world may end if you use split Y on the VESC
[/quote]

I think that only applies to Vesc 6
I can't imagine why though
```

---
## \#33 Posted by: trancejunkiexxl Posted at: 2017-08-18T18:25:39.787Z Reads: 101

```
i can only think of like rca, where if you split signal you need a booster or maybe ferrite ring.. i dono
```

---
## \#34 Posted by: Namasaki Posted at: 2017-08-18T18:30:40.870Z Reads: 100

```
I've been running split ppm for over a year with no issues and no ferrite rings or boosters. 
Just gotta remember to only supply 5v from one source
```

---
## \#35 Posted by: Namasaki Posted at: 2017-08-18T18:36:05.906Z Reads: 100

```
[quote="deucesdown, post:29, topic:30938, full:true"]
Is it just the China batch that's dying? Are the earlier US ones holding up better?
[/quote]

There have been recent cases of the old version failing.
```

---
## \#36 Posted by: bigben Posted at: 2017-08-18T18:54:50.433Z Reads: 99

```
Have the failures all been on 12s?
```

---
## \#37 Posted by: scepterr Posted at: 2017-08-18T18:57:03.353Z Reads: 97

```
Mine was 7S batt max 28A
```

---
## \#38 Posted by: trancejunkiexxl Posted at: 2017-08-18T18:57:30.227Z Reads: 101

```
12s2p battmax ~20-22

*mute the audio
https://drive.google.com/file/d/0B1KhCcXEs2BbUEctTC1aY0J0bjg/view
this is the other working unit.. runs pretty good

just bought a new one from @yummyblobs
going to send the old unit to the wizard..
```

---
## \#39 Posted by: kuphjr Posted at: 2018-07-15T02:34:05.528Z Reads: 61

```
TBH I don't even understand why people use FOC.  I mean, all it seems to do is blow out speed controllers.  From what I hear, the only real benefit is quiet motors, which doesn't really seem to be that big of a deal.  I have heard the efficiency gains from FOC are minimal at best.
```

---
## \#40 Posted by: Namasaki Posted at: 2018-07-15T05:35:19.548Z Reads: 62

```
I'm with you on this.
I have never used FOC and I have never had a Vesc fail.
```

---
## \#41 Posted by: kuphjr Posted at: 2018-07-15T16:22:00.239Z Reads: 60

```
I’ve blown a DRV on the 4.12 VESC with BLDC, but I’m pretty sure that’s my own fault because I like to tow my other friends uphill on regular longboards. I’m sure I was pulling 60A.

I also just blew a focbox because of water damage. I was taking a test ride and all the sudden hit a patch of really wet leaves.![image|375x500](upload://8fDEMEezRIUmrt4MOKlNLjXRxxA.jpeg)
```

---
## \#42 Posted by: Eboosted Posted at: 2018-07-28T00:03:03.526Z Reads: 57

```
I burnt my third FocBox today, weird stuff it just stopped working.

Red light flashing repeatedly 4 times.
```

---
## \#43 Posted by: Namasaki Posted at: 2018-07-28T04:23:21.102Z Reads: 56

```
FOC + 12s ?
```

---
## \#44 Posted by: Eboosted Posted at: 2018-07-28T05:50:36.061Z Reads: 53

```
10s3p runing 30A. The 12s is runing strong on the Trampa daily commuter at really high discharge.
```

---
## \#45 Posted by: SBMTB Posted at: 2018-09-14T10:50:21.827Z Reads: 41

```
I blown one of my both vesc 12s FOC yesterday. I got fooled by the name.  Wish i saw the post earlier... ;( Motor 6374 TB (wanted 6380 but it was BO at the moment...) Running 60a (Can Bus)
Year before, killed 2 vesc 6 again 12s FOC. Motor Trmp 136kv running 50a (CHCHING $$!)  So aint gonna foc around again! Thanks for all this info!
```

---
## \#46 Posted by: sam121 Posted at: 2019-04-12T06:29:57.206Z Reads: 23

```
How are drv's blown?
```

---
## \#47 Posted by: Andy87 Posted at: 2019-04-12T06:46:40.664Z Reads: 21

```
voltage spikes, current spikes, to high erpm, over temp, mechanical impact... pretty much all you can imagine.
```

---
