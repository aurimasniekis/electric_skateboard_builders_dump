# Blown anti-spark on off switch

### Replies: 22 Views: 1198

## \#1 Posted by: Danny414 Posted at: 2018-06-16T04:43:55.226Z Reads: 204

```
![image|375x500](upload://p5N7UOW3gwPaTFNe5SYE0pqeTaV.jpg)I have a 12s5p and my anti-spark on off switch just blew for the first time.. did a little reading and see this is common with the mosfets.. a few questions.. can any direct me to how to figure out which one is bad and how to fix it.. also does using xt90 anti-spark connectors help this from ever happening again? What’s the best way to prevent this from happening?

Thanks!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-16T04:46:43.295Z Reads: 192

```
I would say add a xt90s loop key to your board, everyone says they aren’t pretty but they won’t ever fail. There actually are some nice looking ways to mount them with 3D printed parts. 

What sort of switch is it? Tb?
```

---
## \#3 Posted by: Danny414 Posted at: 2018-06-16T04:51:50.323Z Reads: 186

```
I really like the On off button and would rather figure out how to make it work.. I purchased it from someone on here.. I think he got it from anti spark heaven.. the thread I was reading was from a couple years ago.. figured/hoping that issue has been solved??
```

---
## \#4 Posted by: pat.speed Posted at: 2018-06-16T04:56:07.283Z Reads: 182

```
Well from the picture it doesn’t look like anything is burnt, could I see the other side please? If there is any components on the other side
```

---
## \#5 Posted by: pat.speed Posted at: 2018-06-16T04:58:56.065Z Reads: 170

```
And a close up of the smaller mosfet, please?
```

---
## \#6 Posted by: Danny414 Posted at: 2018-06-16T05:43:09.908Z Reads: 164

```
I have a multimeter.. can that be used to diagnose?

![image|374x500](upload://9OojZUG839VCXAC5yd5cU8s6m2Q.jpeg)![image|374x500](upload://n2vLJpE4lsNk0S79MZHKPVYDCxO.jpeg)
```

---
## \#7 Posted by: pat.speed Posted at: 2018-06-16T05:56:21.590Z Reads: 156

```
I can’t really see any visible damage, how did it actually blow up? Did it just stop working
```

---
## \#8 Posted by: Danny414 Posted at: 2018-06-16T06:08:40.649Z Reads: 159

```
I had the enclosure off and was messing around trying to organize the wiring.. the power button was not inserted into the plastic housing and I just touched the anti spark switch with my finger and it turned the board on.. and when I plug the On off button into the housing it will not power off
```

---
## \#9 Posted by: pat.speed Posted at: 2018-06-16T06:11:45.502Z Reads: 157

```
I don’t quite understand, so you turned it on accidentally and now it won’t turn off? Did it spark or anything like that?
```

---
## \#10 Posted by: Danny414 Posted at: 2018-06-16T06:19:03.222Z Reads: 156

```
It turned on by itself when I touched the actual anti-spark switch/board itself.. the power button wasn’t even connected.. super weird.. when I plugged the button back on it would not power off.. when I connect the xt90 now it sparks louder then usual
```

---
## \#11 Posted by: koralle Posted at: 2018-06-16T06:20:37.359Z Reads: 148

```
Meh always disconnect power before you disconnect the button.
```

---
## \#12 Posted by: Danny414 Posted at: 2018-06-16T06:25:07.596Z Reads: 146

```
Good to know. Did not know that
```

---
## \#13 Posted by: pat.speed Posted at: 2018-06-16T06:28:53.283Z Reads: 141

```
Maybe @JohnnyMeduse might know what happened. Sounds like static shock to me. Where you on carpet by any chance? With socks on
```

---
## \#14 Posted by: Danny414 Posted at: 2018-06-16T06:30:03.277Z Reads: 139

```
Yeah, but no socks.. crap didn’t think about that either
```

---
## \#15 Posted by: BoostedBuilder Posted at: 2018-06-16T06:33:20.183Z Reads: 141

```
[quote="Danny414, post:8, topic:59074"]
and I just touched the anti spark switch with my finger and it turned the board on…
[/quote]

Damn man, you a magician?
```

---
## \#16 Posted by: koralle Posted at: 2018-06-16T06:34:29.117Z Reads: 143

```
![Screenshot_20180616-083030|281x500](upload://9qGqrUxa5CxvIhiMUGecmi6Wqz2.jpg)

Now what's interesting is that @longhairedboy adds a detachable switch to his battery pack but no way to disconnect the anti Spark from power. Is there a way to solve this on the pcb?

![Screenshot_20180615-145939|281x500](upload://upFwOrnGfXc8g22jvLf63rvYNAE.jpg)
```

---
## \#17 Posted by: Danny414 Posted at: 2018-06-16T06:34:51.346Z Reads: 142

```
Ha! It seems I sparked my anti spark
```

---
## \#18 Posted by: banjaxxed Posted at: 2018-06-17T15:16:14.515Z Reads: 128

```
https://www.electric-skateboard.builders/t/antispark-switch-mosfet-stops-working/28978
```

---
## \#19 Posted by: Eboosted Posted at: 2018-06-17T15:37:12.390Z Reads: 124

```
I can help you. If you can't turn it off then you just shorted the mosfets, they are very prone to be sticked in the close position if there is any short  even with your fingers. Do not ever touch the mosfets when they have power, do not connect the antispark without the on/of button plugged in, do not leave the antispark circuit without heat wrap or some kind of insulation. 

Here is the procedure.

1. Check with a multimeter if the negative in and negative out have continuity, if so the mosfets are stucked close. 

2. You can't test the mosfets in the board, as they are in parallel and when you check one the other will fool you.

3. Buy 10 mosfets from Mouser.Com, part number IRFS7530-7PPBF, it's gonna be roughly USD 45
Believe me you will use them. It's way better than buying a new antispark switch. 

4. Remove both mosfets using a hot air gun at 400C, try to do it quick as posible, if you don't have a hot air use chip quick from Amazon and a soldering iron

4. Clean the mosfet and with a multimeter check is its shorted or good using this procedure:

https://youtu.be/IF740E5bm84

5. Change only the bad one

6. Ride your skate again and feel proud to have it repaired yourself with help of your brothers from the forum :smile:
```

---
## \#20 Posted by: Jammeslu Posted at: 2018-06-17T22:11:55.954Z Reads: 103

```
@goldenHusky he is the head in this subject
```

---
## \#21 Posted by: longhairedboy Posted at: 2018-06-19T19:15:41.053Z Reads: 87

```
@koralle
 
I use a connector loop i made to keep the switch off when the packs are in storage or being installed with the switch unplugged. You can make one by taking a servo cable and cutting one side off then shorting the center wire to one of the outer wires. Plug it in one way and the pack is on, take it out and plug it in the other way, and the pack turns off. 

Also, it takes time for the switch to fail on. It doesn't happen right away. You have a minute to get it unpluggled and plugged back in. Often they take longer than overnight to fail into the on position. I've never had one fail on while actually working with it, but i have had them sit for a while and be stuck on when i came back. Eventually they will fail into the on position, how long it takes seems to be randomly longer than a few hours at least in my experience.
```

---
## \#22 Posted by: Wankerman Posted at: 2019-08-01T06:15:08.917Z Reads: 26

```
I just blew up my switch too. I can confirm that connecting the switch to the battery without the button plugged in damages the switch 100%.
```

---
