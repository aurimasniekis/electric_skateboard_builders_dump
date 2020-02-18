# Board stopped braking this morning

### Replies: 53 Views: 1055

## \#1 Posted by: rey8801 Posted at: 2018-06-12T12:53:18.028Z Reads: 257

```
Hi!
I have read about ti but I would like to know a final answer to what happened. Basically I just left my home, 10s board charge to 41.2V (I do not charge it to 100%). After 200 meters I had to brake hard due to a truck leaving a parking spot and basically the board braked at first, then it suddently stopped for 1 second before brake again. I lost the balance and fell. Now I know that when the battery is fully charge this is a mechanism to protect the VESC and battery, but I thought that charge it to 41.2V nad set the overvoltage detection to 57V would prevent it. There is something else I could do it to avoid it for next time?
Settings:
10s3p 30Q battery pack
BMS 60A charge/discharge
Diyeboard 90mm hub motors
Motor max 50  / min -55 (now lowered to -50)
Battery max 30 / min -6
Dual vescs.

Thanks!
```

---
## \#2 Posted by: Acido Posted at: 2018-06-12T13:29:51.580Z Reads: 239

```
probably your bms did not balance the cells because you dont charge ti fully, and when the charging current came in the bms cut of the power
```

---
## \#3 Posted by: Deckoz Posted at: 2018-06-12T13:47:26.053Z Reads: 219

```
Are you using the BMS to discharge? Or is discharge. Bypassed from the BMS?

If you are discharging through the bms... It is the bms fault trying to prevent over charge.
```

---
## \#4 Posted by: rey8801 Posted at: 2018-06-12T13:56:23.095Z Reads: 204

```
@Acido @Deckoz Thank guys for the reply. Yes my bms is also discharge. I used for the past 2 months without problem but I have to say that this morning was just after have left my apartment and I braked quite hard. I also thought is the bms that prevent the overcharge. I was hoping that by charging the battery to 41.2V instead of 42 would avoid this problem. Apparently it helps normally but if I brake too hard from the beginning than I run it the problem. At least this morning :confounded:
```

---
## \#5 Posted by: Acido Posted at: 2018-06-12T14:03:26.531Z Reads: 191

```
you need to accumulate 8wh to make your battery go from 4.12 to 4.2v per cell
and that's a lot because you brake for like 3-4 seconds
```

---
## \#6 Posted by: rey8801 Posted at: 2018-06-12T14:08:31.448Z Reads: 182

```
exactly, that's why I use to charge to 41.2V. The brake stopped working after half second, so could be the first strong peak the cause. The thing is that it's scary.
```

---
## \#7 Posted by: Deckoz Posted at: 2018-06-12T14:12:29.336Z Reads: 179

```
While yes he needs 8wh to charge the battery to rest at 4.2/cell. Voltage spikes from braking can easily over volt even at 41.2 with heavy braking.

I would switch to bypass discharging for safety (your own not the boards).
```

---
## \#8 Posted by: mmaner Posted at: 2018-06-12T14:18:35.545Z Reads: 175

```
[quote="Deckoz, post:7, topic:58644"]
(your own not the boards).
[/quote]

Thats funny.  I almost dove in front of a car the other day when my dog (6 month old german shepherd) slipped her collar.  I swear I'd take a bullet for that dog, but when she tried to bite my bludgeon last night I almost put a straight up a WWE smack down on her :slight_smile:. 

Not that I value my board over my dog, but you know...
```

---
## \#9 Posted by: skatardude10 Posted at: 2018-06-12T14:21:19.055Z Reads: 170

```
I'm not well versed in BMSs and stuff, but I charge my battery to 100% at least once a week until the BMS cuts off power. The display remains at 100% for a while, presumably while balancing cells.

So tell me if I am flawed in my thinking here: if @rey8801 never charges to 100%, could the P groups potentially be out of balance, one near to 100%, and when a strong charge current comes back to the BMS, it doesn't accept the strong current because it detects an out of balance P group? 

Just a thought... I guess all BMSs are different, not sure what bara ships his batteries with but even at 100% 41.9/42.0 volts I've never had a problem braking when starting out my ride.
```

---
## \#10 Posted by: SORRENTINO Posted at: 2018-06-12T14:36:14.913Z Reads: 156

```
The only thing a discharge BMS does is add another failure point to the equation imo. The only time I would use a bms for discharge is if the BMS had a built in antispark :slight_smile:
```

---
## \#11 Posted by: rey8801 Posted at: 2018-06-12T14:41:10.185Z Reads: 146

```
Well... My P groups should also be balanced during the discharge phase.
```

---
## \#12 Posted by: rey8801 Posted at: 2018-06-12T14:51:43.378Z Reads: 141

```
Ok good to know that even an increase in voltage for a half second can do that. So the BMS I used is has charge and discharge at the same port.

![aliexpresshd|281x500](upload://jGV3VxRka8CjnC78wwIkGNcxBzr.jpg)![aliexpresshd|281x500](upload://xL1kJTxNXz8o4YPBhB5zYQHIaLc.png)

To use it only for charging I would need to remove the B- and the the load negative I guess. Which is the safe way to do it? Can I just go backwards in the step. So first the load negative and then the B- (thicker wire)? Thx a lot
```

---
## \#13 Posted by: Deckoz Posted at: 2018-06-12T14:56:43.826Z Reads: 127

```
So basically you would take the -c for the load line, and connect directly to the battery negative terminal

Yellow is remove, blue is the new line
![received_10160408786830521|280x500](upload://Vkpsl72bApRUysf6z8Z666OEZd.jpeg)

Leave the line for the charger(I know the edge of the yellow is slightly touching it because fat finger drawing)
```

---
## \#14 Posted by: rey8801 Posted at: 2018-06-12T14:59:06.087Z Reads: 119

```
OK so I leave the big B- I only remove the load Negative from the BMS and connect the load - to battery negative. Right? It's so stupid that I put such huge BMS for nothing...I guess is a learning curve
```

---
## \#15 Posted by: Deckoz Posted at: 2018-06-12T15:01:18.218Z Reads: 120

```
Yes that is correct. Remove the load- from the -c connection and connect directly to battery negative.

Do you already have an Antispark in your circuit?
```

---
## \#16 Posted by: rey8801 Posted at: 2018-06-12T15:01:58.963Z Reads: 123

```
yes I have both a antspark switch and a loop key. Thanks for the help
```

---
## \#17 Posted by: Deckoz Posted at: 2018-06-12T15:04:24.145Z Reads: 123

```
Ok cool, wasn't sure if you were using a switch on the bms. But since you already have them in place, just changing the load negative to be connected to battery negative will make your setup bypass discharge
```

---
## \#18 Posted by: rey8801 Posted at: 2018-06-12T15:05:40.903Z Reads: 117

```
Thanks. Yes my anti sparks are place befoer the VESCs so no problem for that.
Thanks man! Appreciate...
```

---
## \#19 Posted by: Acido Posted at: 2018-06-12T15:19:34.428Z Reads: 116

```
I always fully charge my board and at the end of my street theres a long hill and I usually brake on it, no problems ever

You just need to set your bms settings correctly
```

---
## \#20 Posted by: Deckoz Posted at: 2018-06-12T15:21:04.626Z Reads: 114

```
Non configurable BMS? How do you set BMS settings with no interface???
```

---
## \#21 Posted by: rey8801 Posted at: 2018-06-12T16:40:48.295Z Reads: 103

```
I was wondering. If I bypass discharge than would I need to charge the battery up to 42V in oder to allow the BMS to balance the cells? Do you charge the cells to max their max Voltage every time?
```

---
## \#22 Posted by: Deckoz Posted at: 2018-06-12T17:11:51.260Z Reads: 105

```
Yea you can charge to max voltage every time. The cells should balance down to about 4.18/cell. Typically even within a mile of riding you use alot more energy than regenerated during braking. So the chance of truely "over charging" the pack is slim.
```

---
## \#23 Posted by: rey8801 Posted at: 2018-06-12T17:23:46.747Z Reads: 104

```
Ok I will use one charger at 41.2V for daily charging and another one time to time to balance the cell at 42V. Thx thx
```

---
## \#24 Posted by: Acido Posted at: 2018-06-12T18:08:14.920Z Reads: 98

```
In case of bestech you can order the settings when you order the bms, or you can get a programming card to do it yourself 

i do not know about other bmss since i never used them
```

---
## \#25 Posted by: BoostedBuilder Posted at: 2018-06-12T18:45:51.863Z Reads: 88

```
Do you have their software to program it?
```

---
## \#26 Posted by: Acido Posted at: 2018-06-12T18:47:44.051Z Reads: 90

```
When you order a bms you can buy the programming card from them ( some Texas instruments model) and it comes with an usb with the software

if you already have the card you could ask them for the software only
```

---
## \#27 Posted by: BoostedBuilder Posted at: 2018-06-12T18:49:52.241Z Reads: 87

```
Interesting, thanks!
```

---
## \#28 Posted by: rey8801 Posted at: 2018-06-12T21:20:49.766Z Reads: 88

```
That's interesting. I knew it that with bestech you can choose the setting before the order. I didn't know you could have the programming card. Nice to know
```

---
## \#29 Posted by: rey8801 Posted at: 2018-06-13T08:34:27.426Z Reads: 83

```
Sorry to resume this thread, but this morning I tried to replicate the problem and indeed when I tried to break hard once left my apartment the board stopped breaking again. This time I was monitoring the ride and I am not sure was the bms the problem.
![chrome|281x500](upload://6aGlFuT840l5KwdDA8MAV0z7mWD.png)![vescmonitor|281x500](upload://y8xZ6XFtiJnMFywRLEwSK5H87um.png)![vescmonitor|281x500](upload://B0y4jCiPofZgn9ZkiOeC2nORaY.png)

As you can see the VESC went in overcharge protection. It recorded 58V spike. When I tired to break hard few kms later it was fine. So I am wondering whether it's only the VESC the cause of it and not the bms because if I reach 58V with a spike probably when the voltage is a bit lower I do not reach the 57V threshold set in the VESC tool but for sure still higher than 42.25V overcharge protection of the BMS. Maybe the BMS has to read this overcharge for few second before cut the current while the VESC does it immidiately. Do you think can I increase the threshold to 70V on the VESC tool just to be safe? Thx


Edit: I was looking around for a solution and could be the same problem @Eboosted described to @Ackmaniac once http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286/702?u=rey8801
Where basically the bms stops to send current to the battery and for that reason the VESC reads higher Voltage and shows the overvoltage fault.
```

---
## \#30 Posted by: Deckoz Posted at: 2018-06-13T11:45:16.834Z Reads: 76

```
Okie doke if you have bypassed the bms and that is happening one of your series connections is broke Inspect the pack @rey8801
```

---
## \#31 Posted by: rey8801 Posted at: 2018-06-13T12:43:10.983Z Reads: 77

```
No this morning the bms was still with the discharge connected. I just wanted to say that I could repeat the issue and present the data too. Now I am changing the bms configuration to charging only and once I charge the board I will try again to brake hard.
```

---
## \#32 Posted by: Deckoz Posted at: 2018-06-13T12:52:54.368Z Reads: 77

```
Ah ok. Yea if the bms was still on discharge. The voltage spikes is from the BMS cutting current.

If this happens with bypassed, it is likely what I said in my last post, and a thorough inspection of the pack is necessary.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2018-06-13T16:25:41.107Z Reads: 77

```
Correct, the BMS is the party crasher here. Kick it out of the discharge cycle and only use it for charging.
```

---
## \#34 Posted by: rey8801 Posted at: 2018-06-13T17:19:24.022Z Reads: 81

```
Thx did it this afternoon. I will report back tomorrow when I charge the board and try again to brake.

![IMG_20180613_154049|690x388](upload://xKGHrf9hJrOa0FcJaf9unbcOVq7.jpg)

Let's see it :grin:
```

---
## \#35 Posted by: Eboosted Posted at: 2018-06-14T00:12:28.776Z Reads: 75

```
Hello @rey8801, I know this problem like the back of my hand.

You are charging your battery at 100% 42V or close to that, when you brake the regen current raises the voltage until the point the BMS shuts the current down to the motors, at this point the current has no where to go because the line to the battery is cutted, so voltage raises until VESC shuts itself down causing a fault.

This fault does not mean the spike it's the culprit of the issue, it's just a consecuence of the BMS shutting power down and leaving the current flowing no where
```

---
## \#36 Posted by: rey8801 Posted at: 2018-06-14T04:48:28.985Z Reads: 69

```
Yes thank you very much. I change the BMS as charge only and I am going to test it today if it is gone. Scary stuff when happens!
```

---
## \#37 Posted by: Eboosted Posted at: 2018-06-14T05:10:56.955Z Reads: 69

```
What bms are you runing?

The best way to fix this issue is charging only to 41.80V, get an adjustable EOC charger
```

---
## \#38 Posted by: Hariboisawesome Posted at: 2018-06-14T05:32:55.206Z Reads: 68

```
Dude I’m cracking up picturing you delivering the stone cold stunner to the pooch!! 😂😂💀
```

---
## \#39 Posted by: rey8801 Posted at: 2018-06-14T06:40:47.504Z Reads: 68

```
I am using this one 10S 40A/60A bms Li-ion large high current BMS PCM with SAME discharge port for electric bike electric car 60a bms
 http://s.aliexpress.com/ZzUZRVvE?fromSns=Copy to Clipboard. I do charge the board to 41.2V but the BMS still cut the current if I brake hard in the first km. Then no problem whatsoever. That's why I didn't have the issue before it's really in the first km that can happen the the voltage goes down.
```

---
## \#40 Posted by: rey8801 Posted at: 2018-06-14T07:47:29.608Z Reads: 66

```
@Deckoz @Acido @Ackmaniac @mmaner Thx guys for the help! Now BMS is only for charging and I tested the board fully charge and I can brake hard without any issue now. Thx Thx Thx!
```

---
## \#41 Posted by: lrdesigns Posted at: 2018-06-14T08:00:15.208Z Reads: 63

```
Forum win!! Congrats on the fix. 

Makes sense why many choose not to have a BMS for discharge. High amp BMS's for discharge are also huge.
```

---
## \#42 Posted by: rey8801 Posted at: 2018-06-14T08:09:09.120Z Reads: 58

```
Yeh, community power! This aspect should be highlighted somewhere. At the time I was seeking for information was clear the part that BMS has a constant discharge current, if it is used for discharging, whihc will limit the drained current during hard accelleration if you choose the wrong one. Although was not really clear to me the fact that can also cut the current during brakesm whihc makes a lot of sense now but I discovered it in the wrong way...:sweat_smile:
```

---
## \#43 Posted by: JonathanLau1983 Posted at: 2018-06-14T08:56:08.297Z Reads: 58

```
Now you're bypassing for discharge doesn't that mean if you heavy brake it will overcharge the battery? Anyone know how much overcharging 18650s can typically take?
I know lots of Lipos can go HV 4.35V, although not advertised for safety. Not sure about Li-ion.
```

---
## \#44 Posted by: rey8801 Posted at: 2018-06-14T08:57:57.228Z Reads: 57

```
Yes you will overcharge the battery but only for 1 sec and moreover just the first kms. Better to give a bit of stress to the battery than don't have the brakes, belive me, I know it! :confounded:
```

---
## \#45 Posted by: JonathanLau1983 Posted at: 2018-06-14T09:00:51.074Z Reads: 56

```
That's true
```

---
## \#46 Posted by: Silverline Posted at: 2018-06-14T18:49:16.606Z Reads: 53

```
I'm using the bestech 80a bms because of the 80a discharge rate. If i should buy a quality bms only for charge (im from EU) what should i buy then ?
```

---
## \#47 Posted by: rey8801 Posted at: 2018-06-14T18:55:50.374Z Reads: 52

```
I think only for charge you can go with cheap one from ebay or Amazon. Something like 10s 15A constant discharge current. You can by them also from bestech if you trust them more. If you can wait Ali is the way. Otherwise some Esk8 store. If you need names just ask. The high discharge BMS takes a lot of space. Now I have a big BMS only for charging. I do not like.
```

---
## \#48 Posted by: Silverline Posted at: 2018-06-14T21:20:41.403Z Reads: 46

```
Yeah... But one of the main selling points for the bestech 80a bms, is that it has a in built "anti spark switch" with a bypassd bms, i would need to have a separate anti spark , if i dont want to use a simple loop key etc. And this will also take Up space, and given the fact, that many antisparks is known to fail at some points , i think that there is more in to it. 
From my home, i always need to brake down a hill the first 500 meters, and with a fully charge batteri, and bestech bms for discharge, i have never experience my brakes to fail. This compo is a year old now.
```

---
## \#49 Posted by: rey8801 Posted at: 2018-06-14T21:23:48.096Z Reads: 49

```
Than perfect like that. I che k my bms cut the current once reach 4.25V so even if I charged to 41.2V for the first km or so if I hard brake it will do it. Probably yoyr bestech has higher threshold (since you can decide it when you buy it) or the overcharge has to last for few second preventing the issue with only spikes.

Edit: anyhow my BMS is way bigger than my antispark. True the second part that they tend to fail.
Questin with the antispark on the BMS your board has to stay on during charging?
```

---
## \#50 Posted by: Silverline Posted at: 2018-06-14T21:27:44.961Z Reads: 49

```
Yes it does. Thats why i have a loopkeey , so my focboxes dont have to stay on, when charging.
![IMG_20180614_233005_HHT|690x388](upload://uwBPk5ffTwL9lJflmFf9u1SWmkl.jpg)
```

---
## \#51 Posted by: rey8801 Posted at: 2018-06-14T21:44:29.139Z Reads: 49

```
Than If you change the BMS the only difference is that you need to unplug the loop key often than now, but the space taken is the same. Anyhow if you don't have problem why change it. I also didn't have problem the first two month than when I need to brake hard immidiately due to a truck going backwards it failed and I tasted the concrete...:tired_face:
```

---
## \#52 Posted by: Wraith Posted at: 2018-08-10T11:19:28.099Z Reads: 42

```
I'm curious what happens in the situation when you don't have a BMS on Li-ion pack(because I plan on balance charging it with a Li-po balance charger) and you break hard on 4.12v as well or on full charge?

Does the same happen wherein the Vesc will shut itself off to prevent over voltage because the power being generated from the motors braking has nowhere to go?

If that was the case what would be a safe solution for that besides always leaving some allowance like say 90% charge before riding?
```

---
## \#53 Posted by: Eboosted Posted at: 2018-08-10T18:54:00.013Z Reads: 34

```
If you don't have a BMS on discharge then nothing will happen, the VESC won't shot down you will have to be riding downhill non stop with a battery charged at 100% before the VESC triggers the maximum cutoff voltage.
```

---
