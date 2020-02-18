# How do I get more distance? (or am I dumb?)

### Replies: 119 Views: 4008

## \#1 Posted by: denton Posted at: 2017-04-08T04:04:35.880Z Reads: 302

```
Hey everyone!
I need some help here maybe just explaining some things to me, so I am looking to the Hive Mind for filling in some gaps of my elementary understanding of electric vehicals.

**First** 
I cannot get my battery to charge past the 39.8v 
Is this the upper limit or is there something wrong with the balancing or are the individual cells unbalanced? I read all of them with a multimeter before I welded it all up and they were the same voltage at assembly.
Or is this just normal operation?



<img src="/uploads/db1493/original/3X/d/1/d1aea366740791bfba9bb158be4773e2ae5b9627.JPG" width="375" height="500">

**My second question:** is there any way I can increase my range? 

Now I have ridden the board a few times and she works GREAT! I love it! So much response and power and it just accelerates like crazy, but it cuts out right at 9.5 kilometers.
Here is my latest test ride. I stayed close because I ended up pushing the last kilometer. 
(also I stopped and grabbed a drink at Quick Trip on KM 4 and 5 to explain the time change)
<img src="/uploads/db1493/original/3X/f/9/f96bb3f2b9a52eeddf9d4ff5d890117521fc97a5.PNG" width="281" height="500">
<img src="/uploads/db1493/original/3X/5/f/5fbe5a03e395a58ff34fb67584072e613a693755.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/e/5/e52c71970509278a7ba0d91f8b0d59f18025f458.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/9/c/9c25338af304796a48ea42a9808ada151b94eb3a.PNG" width="281" height="500">

and here is the voltage at then end
**No Throttle** 
<img src="/uploads/db1493/original/3X/7/7/774e8147ca1760e80eefb346ccd0d86abbe18984.JPG" width="666" height="500">

**When I hit the throttle**
<img src="/uploads/db1493/original/3X/8/f/8f4be3811a411dc4ec0084f2e051025cb146a70e.JPG" width="666" height="500">

**My batteries are Samsung 18650s 25R**

<img src="/uploads/db1493/original/3X/2/2/22b05d6142267ef3f88626ca1b93bc7ac1f5b592.png" width="690" height="118">

**My BMS is this one that @Namasaki sold me. (THANK YOU IT'S WORKING AMAZING!)**
 
<img src="/uploads/db1493/original/3X/3/2/321a064b238697194bfa4df9fc0a5b4286a0579b.png" width="388" height="500">

Thanks to anyone who offers me some insight and maybe explains some things I don't quite understand about current draw to me because I just made things without fully understanding what I'm doing.

Also as a thanks. Here is my "Boosted Clone" we are talking about.
<img src="/uploads/db1493/original/3X/f/e/fe244bec947121edaf4845561f9fffb03363227f.JPG" width="666" height="500">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-08T04:28:57.894Z Reads: 277

```
If it not charging to full, it's because the cells are too far out of balance. 
They have to be balanced before you assemble the pack.
```

---
## \#3 Posted by: PXSS Posted at: 2017-04-08T04:29:12.104Z Reads: 279

```
What is your battery configuration?
10S4P? 9S4P?

Can you post your esc settings too?

E: If its a 10S3P, then they are out of balance. 
Are you discharging through your BMS or bypassing it? If you're bypassing it, then you've most likely damaged your pack already
```

---
## \#4 Posted by: Namasaki Posted at: 2017-04-08T04:31:18.568Z Reads: 272

```
Judging from the voltage sag I'm guessing 10s2p
```

---
## \#5 Posted by: denton Posted at: 2017-04-08T04:31:32.263Z Reads: 269

```
I measured them out before I assembled it, and everything read at 4.2v each. I was wondering if I should take it all the way apart and rebalance every cell.... That would suck but I guess it might be an option.

Sorry I didn't put that in, it is in a 10S3P configuration, and I have 2 of the Enertion VESC 4.12
```

---
## \#6 Posted by: PXSS Posted at: 2017-04-08T04:31:45.659Z Reads: 262

```
Judging by the screenshot He bought 30 cells so I think 10S3P
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-08T04:32:24.620Z Reads: 256

```
Maybe some bad cells?
```

---
## \#8 Posted by: denton Posted at: 2017-04-08T04:32:27.138Z Reads: 252

```
lol, see that is what makes me thing something is up with my battery pack.
because it's a 10S3P
```

---
## \#9 Posted by: PXSS Posted at: 2017-04-08T04:33:00.791Z Reads: 244

```
Are you bypassing bms to discharge?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-04-08T04:33:08.310Z Reads: 242

```
Even at 3p it's only 60a max
But something else is wrong not charging past 39v
```

---
## \#11 Posted by: denton Posted at: 2017-04-08T04:34:46.542Z Reads: 238

```
I have it wired up through the BMS like the diagram above in the specs page shows.
I don't know as much about what I am doing so I just followed the instructions.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-08T04:35:56.686Z Reads: 223

```
Maybe some bad connections in the battery pack
```

---
## \#13 Posted by: denton Posted at: 2017-04-08T04:36:16.932Z Reads: 217

```
And that's what I was thinking, I have charged it for hours and then discharged it, (rode around) and charged again for all day thinking the BMS would just take time to balance it or something, but nothing.
```

---
## \#14 Posted by: Blasto Posted at: 2017-04-08T04:36:36.017Z Reads: 213

```
When fully charged, read the voltage through the bldc tool or with a meter... could be your lcd that is wonky
```

---
## \#15 Posted by: Namasaki Posted at: 2017-04-08T04:37:31.270Z Reads: 209

```
Good point @Blasto check it with a good multimeter.
```

---
## \#16 Posted by: denton Posted at: 2017-04-08T04:37:50.490Z Reads: 209

```
Yeah, Ill try that one out too. I can measure out both to see if there is anything dropping between the battery before the BMS, After the BMS and at the ESC.

Ill try that in the morning when I get it charged.
```

---
## \#17 Posted by: PXSS Posted at: 2017-04-08T04:38:17.886Z Reads: 207

```
Weird. Your battery should have never dropped beneath 25V. The BMS should prevent it. You need to adjust your VESC settings too to decrease the potential of damage. 

Do you have a voltmeter??
I was about to suggest the same thing about measuring voltages.

E2: @denton
Measure the voltage across each cell on the BMS if you can before charging so we know if you've damaged the cells
```

---
## \#18 Posted by: Namasaki Posted at: 2017-04-08T04:41:19.607Z Reads: 207

```
Patrick has a good point, the BMS should shut down if any cell group drops hits 3v
Are you sure the balance leads are properly connected and are you turning the power switch on to charge?
```

---
## \#19 Posted by: denton Posted at: 2017-04-08T04:42:55.490Z Reads: 210

```
I do, and I will bust it out in the morning.
It drops like that and then the VESC shuts it off. 
It just shows 36 and sits there, then when you hit the gas it will shut it off because it drops down to like 22.
Is that normal or is that part of my issue here that it fluctuates that far?
```

---
## \#20 Posted by: JLabs Posted at: 2017-04-08T04:43:02.059Z Reads: 202

```
Do you only have a 39.8v charger? You need a 42v charger for full charge. Only other thing I can think of is that the cells are imbalanced, or the LCD is off.
```

---
## \#21 Posted by: Blasto Posted at: 2017-04-08T04:44:13.491Z Reads: 184

```
[quote="denton, post:19, topic:20586"]
It just shows 36 and sits there, then when you hit the gas it will shut it off because it drops down to like 22.
[/quote]

Errrr... that sounds like a dead parallel pack
```

---
## \#22 Posted by: denton Posted at: 2017-04-08T04:45:54.164Z Reads: 189

```
When I assembled it I measured across each balance lead and it all added up as I went as it should have. I wrote it all down on my dry erase board at one point.

I think you may have been right about how it might have been a cell that may be disconnected somewhere. 

I am about to measure them here before I try charging it again and I'll report back.
Thanks again guys for the help here.
```

---
## \#23 Posted by: denton Posted at: 2017-04-08T04:48:25.831Z Reads: 190

```
Here is my charger.... It's a 48v charger. Which now that I think of it may be too much.
<img src="/uploads/db1493/original/3X/3/8/38fbd55b21772dbb9f1970a7ff0be7b544493fa2.JPG" width="375" height="500">
```

---
## \#24 Posted by: JLabs Posted at: 2017-04-08T04:52:14.158Z Reads: 181

```
That's no bueno unless the BMS shut off the voltage after it reached 42v
```

---
## \#25 Posted by: Blasto Posted at: 2017-04-08T04:52:18.254Z Reads: 181

```
Well shit... that sucks... a 15$ charged fucked 200$ of batteries...
```

---
## \#26 Posted by: Namasaki Posted at: 2017-04-08T04:52:18.661Z Reads: 176

```
That is way too much. You need a 42v charger
```

---
## \#27 Posted by: JLabs Posted at: 2017-04-08T04:54:04.950Z Reads: 177

```
A couple of charges with that and she's dead.
```

---
## \#28 Posted by: Namasaki Posted at: 2017-04-08T04:55:22.272Z Reads: 175

```
I hope that didn't damage the bms as well.
```

---
## \#29 Posted by: denton Posted at: 2017-04-08T04:57:56.594Z Reads: 175

```
Well damnit.....


Into the trash it goes.
Ill pick up a 42v charger, I just pulled the enclosure off and I am going to measure out everything.
I think the BMS should be what cuts it down, and if there is an issue it would be what I might need to replace if the charger damaged it... 

I knew it might be because I am dumb....
```

---
## \#30 Posted by: Namasaki Posted at: 2017-04-08T05:10:14.943Z Reads: 173

```
Well hopefully the bms is not damaged. It still turns on right? and there was no smoke right?
These are good signs.
```

---
## \#31 Posted by: denton Posted at: 2017-04-08T05:11:28.085Z Reads: 175

```
So I measured everything out across the balance leads.
This is still after riding and is not charged yet.

1- 3.7v          (3.7v)
2- 7.3v          (3.6v)
3- 11v           (3.7v)
4- 14.1v        (3.1v) Bad one I guess.
5- 17.7v        (3.6v)
6- 21.4v        (3.7v)
7- 25.1v        (3.7v)
8- 28.8v        (3.7v)
9- 32.5v        (3.7v)
10- 36.2v      (3.7v)

The battery at the connection with it on is reading 36.2 as well as the 10 lead so the BMS isn't dropping anything.
```

---
## \#32 Posted by: denton Posted at: 2017-04-08T05:14:40.224Z Reads: 173

```
No problems and it reads great across it, still works great.

The Connections at the VESCs also reads at 36.2v as well, I need to hook up my computer to see what the BLDC tool says the voltage is, but Im not expecting it to differ much.
```

---
## \#33 Posted by: denton Posted at: 2017-04-08T05:19:37.510Z Reads: 174

```
Is this a better charger?
<img src="/uploads/db1493/original/3X/3/3/33302ae9afc0b07372e886af5763690c142d2f1d.png" width="690" height="263">
```

---
## \#34 Posted by: Namasaki Posted at: 2017-04-08T05:23:09.598Z Reads: 171

```
my 26650 Basen Li-ions would sag from 70% charge to 30% or 40% when going up a 10% grade!
The 25R's Iv'e heard are known for their sag as well.
It could be the sag is due to the type of cells and because a 3p is only 60a. If your running duals at say 30a each.
You could be maxing out the battery which will cause sag especially when the pack is already down to 36v.
At lower voltage, your gonna draw more amps and thats gonna cause more sag.
```

---
## \#35 Posted by: Namasaki Posted at: 2017-04-08T05:23:47.245Z Reads: 173

```
Ya but you can get a better deal on eBay
```

---
## \#36 Posted by: denton Posted at: 2017-04-08T05:27:00.093Z Reads: 174

```
And I know I have the dual motor setup and it is a bit aggressive on my BLDC settings, so I know I am pulling some juice. I guess I could adjust it so that it's not as mean on the acceleration. 

Should I look at taking my pack apart for that #4 cell?
```

---
## \#37 Posted by: Namasaki Posted at: 2017-04-08T05:27:56.158Z Reads: 175

```
http://www.ebay.com/itm/Universal-Charger-42V-2A-Adapter-For-Hoverboard-Smart-Balance-Scooter-Wheel-US-/332136054967?hash=item4d54da00b7:g:NhgAAOSwfVpYroIn

**Free Shipping**
```

---
## \#38 Posted by: denton Posted at: 2017-04-08T05:33:22.278Z Reads: 173

```
I was just looking at that.
```

---
## \#39 Posted by: Namasaki Posted at: 2017-04-08T05:39:10.087Z Reads: 174

```
[quote="denton, post:36, topic:20586"]
Should I look at taking my pack apart for that #4 cell?
[/quote]

Not sure, need to know what the voltage was when it was discharged. 
If you had a hobby charger or a power supply, you could isolate and charge that pack without taking it out.
```

---
## \#40 Posted by: Namasaki Posted at: 2017-04-08T05:41:07.930Z Reads: 167

```
there are some other chargers on eBay that already have the same connector as your board.
```

---
## \#41 Posted by: PXSS Posted at: 2017-04-08T11:46:03.506Z Reads: 159

```
Dont take your pack apart. No need. As others said that charger is probably what did the damage, glad you had a BMS.

It still doesn't explain why your BMS isn't cutting off above 25V. Try hitting the throttle so that your pack sags just below 30V, if it doesnt turn off do it again with it sagging to 28v, if it doesn't shut off do it again to 26V. If it doesn't shut off, there is something wrong with your BMS.

Also please post your VESC settings so we can aid you with that. What worries me is that your battery should never ever be at 22V and both the ESC and BMS should cutoff before then.
```

---
## \#42 Posted by: JLabs Posted at: 2017-04-08T15:55:21.427Z Reads: 152

```
Nope, you need a 42v 2a charger exactly. I may have a good one laying around. I'll let u know when I get home in a few days if your interested.
```

---
## \#43 Posted by: Namasaki Posted at: 2017-04-08T16:06:27.110Z Reads: 153

```
I just realized that you where monitoring your voltage while bench testing which means no real load on the motors.
So if your battery is sagging that much with no substantial load, then your battery is surely done.
```

---
## \#44 Posted by: PXSS Posted at: 2017-04-08T16:55:36.155Z Reads: 144

```
Not necessarily. If his throttle mode is current control. 50% throttle will always result in same amount of power out, regardless of load.
```

---
## \#45 Posted by: denton Posted at: 2017-04-08T18:28:06.469Z Reads: 144

```
I ordered a 42V 2A charger and I will just change out my plug to the 3prong one to accept it so I don't have to frankenstine together a charger cable. It should be here Monday.
Thank you though!
```

---
## \#46 Posted by: denton Posted at: 2017-04-08T18:31:46.325Z Reads: 151

```
Here are my screenshots of my BLDC setup at this point. Again, I have no idea what I am doing with it, I just set it up like the videos said to.

I still have not charged it yet, I am going to wait for my new charger to get here on Monday to replace it and charge it.

I know it's not under load and is not an accurate test of it, but it shouldn't sag like that when I hit the throttle. 
Ill take a video soon of me hitting the throttle and the measurements of it as I do it if that helps. 

<img src="/uploads/db1493/original/3X/d/3/d39cb51c1a8b6de138f2f291f107c9e8c50142eb.png" width="690" height="437"><img src="/uploads/db1493/original/3X/e/d/edd3f3d2b8bfa6cc003cf482c91b96e4d0042ec5.png" width="690" height="437"><img src="/uploads/db1493/original/3X/4/d/4d46e9d3ba5c87c3449acef28b7da37b66825222.png" width="690" height="437"><img src="/uploads/db1493/original/3X/7/d/7d7eafc0134b9a08bd90c9901382a54dfa73be30.png" width="690" height="437">
```

---
## \#47 Posted by: PXSS Posted at: 2017-04-08T18:53:29.358Z Reads: 131

```
Dont worry about it. We're here to help. 

E1: You have a dual setup correct? And the settings are identical in both ESCs?
```

---
## \#48 Posted by: denton Posted at: 2017-04-08T18:55:36.788Z Reads: 129

```
Yes, it is a dual motor setup and both VESCs are identical
```

---
## \#49 Posted by: PXSS Posted at: 2017-04-08T19:11:03.284Z Reads: 130

```
Your settings are actually almost perfect. 
You should change your RPM limits to 60000 in each direction so you dont burn up the ESC. 
Voltage cutoff start and end are a little high but that should only mean it's safer. 

Have you run the board while BLDC is connected?
Run it again with the realtime terminal open and see how much it sags there. Also check the faults after it quits.
```

---
## \#50 Posted by: Ackmaniac Posted at: 2017-04-08T20:01:45.387Z Reads: 134

```
[quote="PXSS, post:44, topic:20586, full:true"]
Not necessarily. If his throttle mode is current control. 50% throttle will always result in same amount of power out, regardless of load.
[/quote]

Well that's not true. If you have setup motor max to 80 amps and give 50% throttle then you won't reach 40 amps in the bench. And even if then only for a fraction of a second. Afterwards the motor spins at maximum speed and can't consume more amps anymore. So to let the battery sag you really need to stand on the board. Otherwise the free spinning wheels have not enough resistance. And the power is also not there instantly. There is a small ramping in the code of the Vesc.
```

---
## \#51 Posted by: Namasaki Posted at: 2017-04-08T21:41:32.073Z Reads: 132

```
[quote="PXSS, post:44, topic:20586, full:true"]
Not necessarily. If his throttle mode is current control. 50% throttle will always result in same amount of power out, regardless of load.
[/quote]
I think you are incorrect on this point Patrick. 
I believe the current control mode on the Vesc is basically a current limiiter. 
As you increase throttle, it allows more current but the current needed is still determined by load.
```

---
## \#52 Posted by: PXSS Posted at: 2017-04-08T21:56:21.502Z Reads: 125

```
Yep yep. You are correct
```

---
## \#53 Posted by: Okami Posted at: 2017-04-08T23:05:56.074Z Reads: 126

```
Im still an observer .. but i think he will either need to individually balance that one cell out.. if it is really out of balance that much (3.1 vs 3.5v)..

or worst case, replace it..

--

Though Im still not sure either how you @denton could get 22v readout.. that is 2.2v per cell, at not very big load.. so Something is probably not super right in the readings either..
```

---
## \#54 Posted by: IsTalo Posted at: 2017-04-08T23:27:01.243Z Reads: 117

```
What is wrong with bypassing a Bms?
```

---
## \#55 Posted by: Namasaki Posted at: 2017-04-08T23:55:17.121Z Reads: 109

```
It is possible that all the cells are damaged from charging with too high voltage.
```

---
## \#56 Posted by: Okami Posted at: 2017-04-08T23:58:02.788Z Reads: 110

```
@Namasaki  ut what did bms do in this situation? IT somehow still allowed the cells to be charger.. this is the part about which im not very clear about - how it did even work without burning up something..

Did the bms just ''allow'' the current / voltage to flow, without limiting it in any way?
```

---
## \#57 Posted by: Namasaki Posted at: 2017-04-09T00:07:01.422Z Reads: 112

```
Charging with 48v might have caused some damage to the bms but I'm not sure. Not connecting the balance wires correctly will certainly damage it so possibly too much charge voltage could as well.
I have used several of these bms's and currently have them on 2 builds and have had no issues with them functioning as they are suppose to including shutting down when the battery reached low voltage trigger.
```

---
## \#58 Posted by: denton Posted at: 2017-04-09T00:20:13.447Z Reads: 120

```
Here is the BLDC reading when hitting the throttle.
It shuts down when it drops under the voltage limit.
So I feel that is a good sign. I made the video first, then ran it on BLDC. It shut off and that is the reading it gave me.
<img src="/uploads/db1493/original/3X/3/8/3852a37630d7bcedae7ab753e78850066ffdba3b.png" width="690" height="437">
https://youtu.be/JU-JhzsNXQs
```

---
## \#59 Posted by: Namasaki Posted at: 2017-04-09T00:52:38.244Z Reads: 112

```
Can you take a pic of your wiring and post it?
```

---
## \#60 Posted by: Ackmaniac Posted at: 2017-04-09T00:57:09.356Z Reads: 110

```
Bypass the BMS (connect battery and vesc directly). If it acts the same then you know the battery is gone. If not you know the BMS is gone.

But I guess the battery is dead from overcharging.
```

---
## \#61 Posted by: denton Posted at: 2017-04-09T01:03:57.012Z Reads: 114

```
<img src="/uploads/db1493/original/3X/0/a/0a613430589a82b3c58cbe067ae455601b2c5eea.JPG" width="375" height="500">
```

---
## \#62 Posted by: PXSS Posted at: 2017-04-09T01:05:59.056Z Reads: 113

```
YHe was charging through the BMS. The battery is not necessarily damaged, and neither is his BMS. His charger has a max current output, if that isn't enough to bring the cells to 4.2V then the BMS will allow charging until the cells reach 4.2V at which point the BMS will cutoff the current.

What will happen is that his BMS will never balance cells

@denton
Can you shoot another video, this time focusing on BLDC screen. I'm mostly interested in the bottom right corner where the battery voltage is displayed.
If you have a voltmeter maybe even try to get that in the video too so we have several sources to confirm voltage. (I for one, dont trust those screens fully)
```

---
## \#63 Posted by: Okami Posted at: 2017-04-09T01:11:24.485Z Reads: 108

```
I would also 'guess' / suggest to bypass the Bms to see how it looks then.

Maybe it is messed up and starts to cut down on power..

Is the indicator (voltage / battery display) conneted directly to the battery or the bms?

If it is directly connected to battery.. then okay it might be battery's fault afterall.. otherwise, ..bms

--
@denton  aternatively - just hook up multimeter to the battery connections directly, then do the ''throttle test'' again to see what voltage is showed there.. then I think it would be the best way to check whenever bms looses power / voltage or is it the battery itself..
```

---
## \#64 Posted by: PXSS Posted at: 2017-04-09T01:21:01.918Z Reads: 109

```
@okami @Namasaki @Ackmaniac
If @denton does the same test and measures the voltage across battery terminals, before BMS and the battery never drops below 25V then the BMS and/or ESC is functioning properly. 

The next test would be to measure voltage across cell 4 while performing the throttle test to ensure that the cell is not dropping below 2.5V. If it does then the BMS is probably damaged, if it doesn't then the BMS is working properly. 

Do you guys agree??
```

---
## \#65 Posted by: Okami Posted at: 2017-04-09T01:25:42.962Z Reads: 105

```
@PXSS sounds good to me, since all we know right now is what happens after BMS.. and that last part of video looked a bit strange on how exactly it got cut off.
```

---
## \#66 Posted by: denton Posted at: 2017-04-09T01:33:02.478Z Reads: 106

```
https://youtu.be/bmFoKBX8Ewo
```

---
## \#67 Posted by: Namasaki Posted at: 2017-04-09T01:55:40.744Z Reads: 102

```
I think you have a loose connection or a cold solder joint somewhere
```

---
## \#68 Posted by: PXSS Posted at: 2017-04-09T01:57:27.268Z Reads: 105

```
@denton
I cant zoom in enough on the screen, can you walk me through it, what was the lowest voltage recorded and what is the fault?

The good news is that your battery didn't sag beneath 30V for this test. 

I think your BMS is working just fine! The reason your ESC kept cutting off is because the one cell most likely hit 2.5V and the BMS cuts power, once it recovers, you're able to reconnect and try again and it trips over and over. 

So good news is your pack is most likely fine!!
Just out of balance

E: @denton to confirm, measure the voltage across 4 and do the test again. If the ESC cuts off as soon as that cell sags then the BMS is working and all you need is to get yourself a 42V charger so your BMS can actually balance
```

---
## \#69 Posted by: denton Posted at: 2017-04-09T01:59:59.368Z Reads: 99

```
I have spent the last 30 min opening up the battery to look at that #4 cell.
And it has some bad welds. It looks like they came apart.
```

---
## \#70 Posted by: Namasaki Posted at: 2017-04-09T02:01:20.911Z Reads: 98

```
When this bms trips and shuts off, it doesn't just turn back on by itself. you have to reset it with the power button
```

---
## \#71 Posted by: PXSS Posted at: 2017-04-09T02:01:21.752Z Reads: 93

```
Sorry to hear. Can we get pics?
```

---
## \#72 Posted by: PXSS Posted at: 2017-04-09T02:01:57.651Z Reads: 96

```
Ahhhh. Mine trips and resets after x seconds.
```

---
## \#73 Posted by: denton Posted at: 2017-04-09T02:06:39.100Z Reads: 97

```
It is resetting on its own. 
I am currently working on getting this opened up to where I can weld it back. See if I can balance it back.
```

---
## \#74 Posted by: Namasaki Posted at: 2017-04-09T02:15:01.687Z Reads: 97

```
What welder are you using?
```

---
## \#75 Posted by: PXSS Posted at: 2017-04-09T02:41:45.302Z Reads: 96

```
Do you own an RC charger to balance the cells individually? If not @jmasta has a pretty clever solution to do it by using a power resistor and a voltmeter
```

---
## \#76 Posted by: denton Posted at: 2017-04-09T03:23:29.987Z Reads: 98

```
This is the one I am using.
It is terrible. 
I have more issues with broken welds on this then anything else. 
<img src="/uploads/db1493/original/3X/1/b/1b4c1aadaff98c8273ae229cfea3132a2c6ed3b3.png" width="690" height="325">

And @PXSS I have no Idea how I am going to balance it, I will have to look that up.

Also sorry for the longer response time. I am working on the battery now.
```

---
## \#77 Posted by: Okami Posted at: 2017-04-09T03:55:52.684Z Reads: 96

```
if it really is just one cell (cell group) in your place I might as well would look up how to individually charge it up..

What @jmasta mentioned in the other topic does not sound bad but i see it as more practical if more groups are way higher than needed, than when just one group is below every other group..

If you got access to electronic shop / distributor, maybe look up some of these **TP4056 modules**

https://dlnmh9ip6v2uc.cloudfront.net/datasheets/Prototyping/TP4056.pdf

 they are for 1cell and max 1amp, you would still need to check the voltage and dont let it go over the voltage of other cells..

--

Though, firstly, probably try to figure out where the problem is.. and then it can be decided what action should be taken
```

---
## \#78 Posted by: denton Posted at: 2017-04-09T04:32:19.254Z Reads: 100

```
I went through and re-welded the connections on the #4 cell and doubled checked the rest of the battery and it all looks good.

When I got it all back together I checked my balance leads and this is how they read

1- 3.7v (3.7v)
2- 7.3v (3.6v)
3- 11v (3.7v)
4- 14.6v (3.6v) 
5- 18.3v (3.7v)
6- 22v    (3.7v)
7- 25.7v (3.7v)
8- 29.4v (3.7v)
9- 33.1v (3.7v)
10- 36.8v (3.7v)

Now It reads like this on the board.
<img src="/uploads/db1493/original/3X/1/c/1c4b08c9619f6fcbf38d69ed64d1edc54c79aede.JPG" width="375" height="500">

And with the "throttle test" it sits steady at 36.3
<img src="/uploads/db1493/original/3X/d/a/daac1fab601bc1d4243b1c4b8123fe1f42a9de8d.JPG" width="375" height="500">

My volt meter on my board is always about .1 off from my multimeter. But now it doesn't fluctuate and cutoff like it did.
```

---
## \#79 Posted by: Namasaki Posted at: 2017-04-09T04:38:23.658Z Reads: 95

```
I'm afraid those 30a welders don't really have enough power.
I was using a 60a welder and I had to turn it all the way up and use 8 pulses to get a strong weld
I'm afraid your whole pack could be in question as far as the strip connections.
Since you got the welder from Amazon, you might be able to return it and get a 60a welder.
```

---
## \#80 Posted by: denton Posted at: 2017-04-09T04:41:03.153Z Reads: 98

```
It really is the worst. This is the second time I have gone back in and rewelded my pack. I think I am going to just throw it out of my window on the highway.

I wrapped every weld with tape and wrapped it all the way around, as tight as I could get it. So we will see if that helps.
```

---
## \#81 Posted by: Namasaki Posted at: 2017-04-09T04:44:31.493Z Reads: 100

```
Looks like you found the problem. 
Did you test each welded connection by pulling on it with needle pliers ?
If the welds are good, you won't be able to pull the strips from the battery cells without destroying them.
```

---
## \#82 Posted by: Namasaki Posted at: 2017-04-09T04:48:28.355Z Reads: 100

```
[quote="denton, post:80, topic:20586"]
This is the second time I have gone back in and rewelded my pack. I think I am going to just throw it out of my window on the highway.
[/quote]


Like I said already, the problem your having is because of the welding machine is too low power.
And vibration will work a cold weld joint loose over and over again.
You need at least 60a welder. that's the minimum.
This is like the one that I had. It did the job but only on full power using the fixed electrodes. The handheld electrodes reduce power too much for my liking.
http://www.ebay.com/itm/2in1-Pulse-Spot-Welder-709A-Battery-Welding-Soldering-Machine-1-9kw-60A-US-Stock-/282184419748?hash=item41b38089a4:g:W1UAAOSw44BYYyuy
```

---
## \#83 Posted by: denton Posted at: 2017-04-09T04:52:45.896Z Reads: 103

```
I picked at them with my multimeter leads. And they were good but you're right. The vibrations will end up cold working it and breaking more in the future. I will be shopping for a new welder soon. It will give me a chance to take the whole battery apart and balance out each battery or something. We will see.
```

---
## \#84 Posted by: jmasta Posted at: 2017-04-09T04:58:36.788Z Reads: 102

```
[quote="Okami, post:77, topic:20586, full:true"]
if it really is just one cell (cell group) in your place I might as well would look up how to individually charge it up..

What @jmasta mentioned in the other topic does not sound bad but i see it as more practical if more groups are way higher than needed, than when just one group is below every other group..[/quote]

Something like this CV/CC voltage regulator could be used to charge an individual cell:

* Input voltage: 4-38V 
* Output power: 75W(Max) 
* Transfer efficiency: 96%(Max) 
* Output current: adjustable;5A(Max) 
* **Output voltage: 1.25-36V constantly adjustable** 
* Short-circuit protection: YES(limited current of 8A) 
* Over-temperature protection: YES(item will stop output atomatically) 

https://www.amazon.com/Step-down-Constant-Converter-Regulator-Electromobile/dp/B00VUHVX6W/

There are some with LCD screens for voltage/current, but they don't seem to be CC/CV. I'm not sure if this would work

https://www.amazon.com/DROK-Adjustable-Converter-Stabilizer-Regulator/dp/B01GM91FP6
```

---
## \#85 Posted by: denton Posted at: 2017-04-09T05:01:01.686Z Reads: 97

```
Funny I actually just picked up a couple of these the other day. Ill use it if my new charger and BMS doesn't balance it out.

Thank you!!!
```

---
## \#86 Posted by: Namasaki Posted at: 2017-04-09T05:01:03.619Z Reads: 96

```
Grab the nickel strips in between the cells with needle pliers and tweak them in a rocker motion back and forth slightly.
If they break loose, they are no good. It is important to resolve this issue because a poor connection like this can also cause heat between the strip and cells.
```

---
## \#87 Posted by: Namasaki Posted at: 2017-04-09T05:04:07.087Z Reads: 94

```
Those converters won't work because his charger is over 38v output.
```

---
## \#88 Posted by: Namasaki Posted at: 2017-04-09T05:09:14.457Z Reads: 90

```
A lab power supply is a good investment. You can get a 0-30v for fairly cheap on Amazon.
With it you can charge single cells and cell groups. And do other stuff like programing Vescs etc.
```

---
## \#89 Posted by: jmasta Posted at: 2017-04-09T05:10:15.762Z Reads: 96

```
You'd use it with any standard DC power supply. 5V, 12V, 24V, etc. Almost any power supply would work, expect for our high voltage 10S+ chargers
```

---
## \#90 Posted by: Eboosted Posted at: 2017-04-09T06:18:24.967Z Reads: 102

```
I had the same issue as you, but two cells of one of my packs were 0V and the others 3.7v.

I tried many different things to be able to balance the cells with a standard 2A 42V brick charger, but it never balanced at all. I'm buying a lab power supply and hope I could use it to balance my pack while charging.

I'm not sure if the BMS I currently have will be able to balance the packs, I got this message from. Battery Supports:

Dear Alan,

the BMS is more like a monitor, it cant balance battery cells, obviously, one of group has shorter capacity than others, thats why it cant be balanced, BMS cant change battery capacity, it is just find this out but cant cure it.

It is not safe to mix battery cells having different capacity in use. We advise you to use a new good battery packs. But if  this is too costly, you may separately charge this shorter group, not re-charge by BMS. But still, this shorter battery will drain other batteries in use. We advise that this battery pack needs replacement. 

Should you have any in doubt, please feel free to contact us. 

Regards,
```

---
## \#91 Posted by: PXSS Posted at: 2017-04-09T12:44:51.619Z Reads: 97

```
Your problem is different though because you were bypassing the BMS. @denton was not, his cells definitely got saved by it.

What I think was happening is that whenever he applied the throttle and cell 4 reached his BMS LVC, the BMS cut power. This is suppported by his test 2 video where BLDC shows his battery voltage dip all the way down to 5V while his battery voltage before the BMS stays above 30V.

The cause of his problem was bad weld joints and it could be the same for you. The BMS thought should be able to handle the balancing with the right power supply.
```

---
## \#92 Posted by: jmasta Posted at: 2017-04-09T17:13:56.599Z Reads: 94

```
[quote="Eboosted, post:90, topic:20586"]
the BMS is more like a monitor, it cant balance battery cells, obviously
[/quote]


I'm confused by this.... Is that not one of the primary functions of a BMS?

I've had a hard time getting clear answers when emailing Battery Supports, probably due to the language barrier
```

---
## \#93 Posted by: Eboosted Posted at: 2017-04-09T17:38:58.282Z Reads: 93

```
Well was never able to balance my packs with a BMS at all. @PXSS diagnosed it as a bad brick charger-BMS combo, as soon as I receive my lab power supply I'll do the testing and keep everyone informed
```

---
## \#94 Posted by: Namasaki Posted at: 2017-04-09T17:41:22.633Z Reads: 96

```
There is sometimes miscommunication because of the language barrier. 
And @Eboosted may have received some incorrect information from a rep at Battery Supports.
However, if this is true then the battery supports BMS is useless.
```

---
## \#95 Posted by: jmasta Posted at: 2017-04-09T17:53:19.677Z Reads: 97

```
Good luck! Hope you figure it out.  I think the key takeaway here is to balance all cells before assembly.  One website I was reading said that if the cells are very out of balance, it could take _weeks_ for a BMS to fully balance them.  

[quote="Namasaki, post:94, topic:20586, full:true"]
There is sometimes miscommunication because of the language barrier. And @Eboosted may have received some incorrect information from a rep at Battery Supports.However, if this is true then the battery supports BMS is useless.
[/quote]

My 12S 60A BMS from Battery Supports balances my 4x 3S Lipo battery pack. Lillian from Battery Supports said it starts balancing at 4.15V.   Yet some places list it starting at 3.9V... (like on their website!).  I have yet to confirm whether mine starts at 4.15 or 3.9V, but it does indeed balance them
```

---
## \#96 Posted by: denton Posted at: 2017-04-14T04:05:33.986Z Reads: 89

```
Hey guys, thank you soooooo much for the help over this past week! 
What a great community, you guys are awesome.

So I replaced my charging jack to a 3 pin, and bought a new charger. 
The first one came in and sparked and let the smoke out as I plugged it into the wall. Didn't even plug it into the board and it caught fire..... Returned it and got a better one.


That one came in today and I charged it for 2 hours and the voltage actually dropped over those 2 hours.
So I think the BMS charging circuit might be fried out.... I can't see anything in the BMS that is burned or let the smoke out.

<img src="/uploads/db1493/original/3X/2/9/295ed8d753b5894d48a0818ad9ebe65e7c41712b.JPG" width="375" height="500">
```

---
## \#97 Posted by: Namasaki Posted at: 2017-04-14T05:30:23.423Z Reads: 82

```
It might not be the bms, it might be the battery cells are damaged
Or maybe you still have some cold weld joints
```

---
## \#98 Posted by: Namasaki Posted at: 2017-04-14T05:33:50.854Z Reads: 81

```
What do you think about picking up a couple inexpensive 5s Lipos to connect to the bms and charge to see if it works with another battery.
```

---
## \#99 Posted by: PXSS Posted at: 2017-04-14T05:37:01.695Z Reads: 79

```
What charger did you get? Can you post pictures. 
My gut tells me you got the wrong charger. 

There is no charging circuit in the BMS. All it is, is a few FETs that switch off when you hit a certain voltage + the balancing part. 

If your voltage is dropping when you plugged the charger in, then the charger is outputting less voltage than your pack. So in reality you are discharging your pack to your charger, which is scary to even think of...

Check the voltage coming out of your charger. Make sure it's 42V
```

---
## \#100 Posted by: denton Posted at: 2017-04-15T04:12:39.433Z Reads: 81

```
This is what I have. 
<img src="/uploads/db1493/original/3X/4/b/4b3726f65597c3933e67aa11a0e816113ee406e2.JPG" width="375" height="500">
```

---
## \#101 Posted by: denton Posted at: 2017-04-15T16:54:59.548Z Reads: 77

```
@PXSS I went and measured out my charger with my multimeter and it fluctuates from 30v to 50v and it would never stop on a number. It wouldn't give a consistent reading.
```

---
## \#102 Posted by: denton Posted at: 2017-04-15T16:55:40.111Z Reads: 77

```
I was thinking of doing this anyway for my other skateboard to get it working.
```

---
## \#103 Posted by: Namasaki Posted at: 2017-04-15T16:58:50.109Z Reads: 75

```
Sounds like a flaky charger
```

---
## \#104 Posted by: Eboosted Posted at: 2017-04-15T17:02:26.002Z Reads: 77

```
It shouldn't fluctuate between 30v and 50v, I'm guessing your charger is not good again, you might want to ask for your money back at this point and get a new charger somewhere else. 

You can read the voltage from the charger plug easily but never measure the voltage from the charging port on the board, you will have a big short if the voltmeter terminal touches positive and negative, very dangerous.
```

---
## \#105 Posted by: denton Posted at: 2017-04-15T17:19:35.369Z Reads: 76

```
I measured it off the plug. I didn't measure the charging port on the board. I'll get another charger.
```

---
## \#106 Posted by: denton Posted at: 2017-04-15T17:24:18.666Z Reads: 75

```
Also. Sorry for the late replies lately. I work at a church and Easter is like the church Super Bowl. So I'm a bit busy.
```

---
## \#107 Posted by: Eboosted Posted at: 2017-04-15T22:44:39.036Z Reads: 73

```
Yes, I know you didn't, just giving you a heads up before you commit a mistake
```

---
## \#108 Posted by: denton Posted at: 2017-04-15T22:55:46.650Z Reads: 71

```
Thanks! I do appreciate it!
```

---
## \#109 Posted by: Namasaki Posted at: 2017-04-16T00:17:42.207Z Reads: 72

```
You are certainly having your share of bad luck with this build but hang in there. 
You will get it sorted out.
```

---
## \#110 Posted by: PXSS Posted at: 2017-04-16T00:31:16.444Z Reads: 71

```
I may have a spare charger that I could sell you.
I haven't opened it up yet so I need to check that it's in working condition.
```

---
## \#111 Posted by: denton Posted at: 2017-04-16T01:01:05.319Z Reads: 70

```
I just picked this up on Amazon earlier today... Hopefully 3rd time is the charm lol

<img src="/uploads/db1493/original/3X/d/0/d0fae9b898ab5b8e0ff0d4497c8bee79fe46e295.png" width="690" height="223">
```

---
## \#112 Posted by: denton Posted at: 2017-04-21T15:03:05.767Z Reads: 71

```
So yesterday I put this charger on and it started to charge right away. I guess I just got some bad chargers. 

<img src="/uploads/db1493/original/3X/e/7/e71895481009cf17af2ad414e1e14cee566ddf54.JPG" width="375" height="500">

This was right before I went to bed. 
Also my onboard voltage meter has always been .1 below the actual voltage reading so I'm happy with that! 

But now the motors won't turn so I think it may be a voltage setting on my VESCs.
```

---
## \#113 Posted by: Namasaki Posted at: 2017-04-21T15:20:41.086Z Reads: 69

```
Glad you got it sorted out and there appears to be no damage to your battery or electronics.
```

---
## \#114 Posted by: denton Posted at: 2017-04-21T15:22:10.377Z Reads: 68

```
Yeah! Me too! Hahaha thanks again for all the help!
```

---
## \#115 Posted by: Namasaki Posted at: 2017-04-21T15:36:12.706Z Reads: 66

```
Btw, even when I charge with a power supply filling my battery completely to 42v.  After I stop charging, the BMS eventually trims the battery down to 41.9
```

---
## \#116 Posted by: Eboosted Posted at: 2017-04-22T05:35:32.478Z Reads: 61

```
What are your current VESC settings, battery cut off start and end?
```

---
## \#117 Posted by: Namasaki Posted at: 2017-04-22T06:14:28.219Z Reads: 64

```
<img src="/uploads/db1493/original/3X/6/8/68a8556693f9fd15d4d913b925707bdacd5c4a37.png" width="690" height="362">
```

---
## \#118 Posted by: denton Posted at: 2017-04-22T18:34:27.107Z Reads: 57

```
Yeah I just changed my voltage limit on my VESCs from 42 up to 48 and it works fine. 

Today is the first day it's not raining here so I am going to go for another test ride.
```

---
## \#119 Posted by: Namasaki Posted at: 2017-04-22T21:19:40.921Z Reads: 57

```
the Max input voltage should stay at 57v.
```

---
