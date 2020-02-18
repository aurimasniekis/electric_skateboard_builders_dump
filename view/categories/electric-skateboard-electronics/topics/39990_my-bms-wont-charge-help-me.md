# My bms wont charge help me

### Replies: 22 Views: 1399

## \#1 Posted by: onepunchboard Posted at: 2017-12-03T05:14:41.992Z Reads: 116

```
here is drawing of what i did.<img src="/uploads/db1493/original/3X/8/4/84e8ad748b8813f4da0a183d487da321cb13fe17.jpg" width="281" height="500">

it just simply wont turn on. i checked every wire. Vesc works fine.
i pluged charger, stays green.
could be faulty bms but i wonder if I switched polarity of charging port if I followed my drawings.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-03T05:41:19.372Z Reads: 112

```
Need info:
Battery type and specs.
bms type and specs.
charger type and specs.
and test the polarity of your charge plug from the charger with a multi meter and make sure it matches the charger port on your board.
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-12-03T05:48:41.160Z Reads: 109

```
battery lipo 5s5a x4 = 10s10a. getting 40.5v
bms https://m.ebay.com/itm/Max-40A-Balance-Battery-Protection-Board-BMS-PCB-For-36V-10S-10Packs-Li-ion-Cell/311862435323
charger: 42v 2amp, getting 44v with multimeter.

i check balance lead which is correct order.

i soldered bms with batt- and charger- left p- empty. 
maybe i should connect p- to something to work?
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-12-03T05:53:24.905Z Reads: 109

```
im thinking i should connect batt plus to p-?<img src="/uploads/db1493/original/3X/1/6/16c441f2ed03346af0df621d6f084fa592c05f20.jpg" width="632" height="500">
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-03T06:34:50.583Z Reads: 94

```
[quote="onepunchboard, post:4, topic:39990"]
im thinking i should connect batt plus to p-?
[/quote]


Please don't do that. Connecting the battery's positive to P- will short the battery.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-12-03T06:38:25.802Z Reads: 97

```
Your charger should only be outputting 42v
44v is too high and it sounds like you have a defective charger.

Another reason for your battery not charging completely is if the cells are too far out of balance.
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-12-03T06:43:08.968Z Reads: 95

```
i charged the batt before put them to gether they are with in .1 to .15 differences. may be the charger problem :(. i hav besttech bms on the way but cant figure what the problem is
```

---
## \#8 Posted by: sterlinggray4 Posted at: 2018-04-25T15:14:48.692Z Reads: 72

```
Was this ever solved? I seem to be having the same issue. @Namasaki or @onepunchboard any thoughts? 

In my case I can get my VESC powered and my motor running when it is on the charger but nothing works when I unplug. I am using a Bestech BMS with E switch and a 10s5p Li-ion config. My cells are all balanced and if I unplug/plug the balance cables from the BMS the charger begins charging for ten second before stopping.
```

---
## \#9 Posted by: onepunchboard Posted at: 2018-04-25T15:28:08.342Z Reads: 68

```
frankly i gave up using bms for that. besttech bms shouldn't be the problem but not sure why such problem occur.
```

---
## \#10 Posted by: sterlinggray4 Posted at: 2018-04-25T15:48:45.318Z Reads: 68

```
So what'd you do? I am at a loss as my board is basically complete but I cant take it off the charger!
```

---
## \#11 Posted by: Namasaki Posted at: 2018-04-25T17:29:42.051Z Reads: 66

```
If you unplug the balance connector while the bms is on, it will go into protection mode and you’ll have to cycle it off and on to reset. 

Try this sequence 

1:Turn the bms off. 
2:Connect the balance connector to the bms.
3: plug your charger into the charge port
4: turn the charger on and then immediately turn the bms on.
5: when charging is complete, turn the charger off then turn the bms off and wait for the system to drain off residual voltage and then unplug the charger from the charge port.
```

---
## \#12 Posted by: sterlinggray4 Posted at: 2018-04-25T18:45:56.524Z Reads: 61

```
That didn't seem to do anything...
```

---
## \#13 Posted by: Namasaki Posted at: 2018-04-25T19:08:42.274Z Reads: 61

```
Double check your wiring then. Especially the balance wires.
```

---
## \#14 Posted by: sterlinggray4 Posted at: 2018-04-25T19:41:29.660Z Reads: 60

```
All balance cables are showing correct voltages, the charger is correctly showing 42.5V. I believe all my solder joints are correct? But I could be wrong, Ill post a picture and the wiring diagram I used
```

---
## \#15 Posted by: sterlinggray4 Posted at: 2018-04-25T20:25:31.628Z Reads: 58

```
![IMG_1705|690x459](upload://dLCSm8jaHOUk6Icw2Y37ovSCwSS.JPG)![IMG_1703|690x459](upload://uzAWlxN4hymLQgwth30YmGQ5DXQ.JPG)![IMG_1706|690x459](upload://8V53xpVGNGb1NaLfBinBLCB9gsB.JPG)

Here's some pictures of my Wiring and then here are my BMS specifications

![D528V1LI10S80A-02  BesTech Power datasheet|353x500](upload://25kTecmLCdGXSKuhSAjEx7GEJsw.png)![D528V1LI10S80A-02  BesTech Power datasheet 1|353x500](upload://jJY5rt6BtUVi8uln1fzJvRVM8SH.png)

And the wiring diagram I followed

![esk8 drawing-3|666x500](upload://xuSHw4Gh4Qx5VsXIxARnDwPvd8H.png)
```

---
## \#16 Posted by: sterlinggray4 Posted at: 2018-04-26T01:07:48.192Z Reads: 50

```
@RedEagle @Fissh02 Would love some advice here!
```

---
## \#17 Posted by: Lambjr088 Posted at: 2018-04-26T02:59:38.569Z Reads: 47

```
I'm wondering if this will work for my bms the wiring is correct as I followed the diagram from bestech and now the bms wont turn on. I used my voltmeter to check and it runs 8.7 volts in its current condition but the e-switch wont do anything the battery by itself measures at 37.5 volts 10s5p. Seems the bms is my problem but dont know any fix for it I have emailed Lucy to see if they can replace it as I haven't soldered anything to it just testing it
```

---
## \#18 Posted by: sterlinggray4 Posted at: 2018-04-26T12:24:37.618Z Reads: 44

```
What model do you have? I am using the HCX-D52.
```

---
## \#19 Posted by: RedEagle Posted at: 2018-04-26T12:31:41.723Z Reads: 47

```
My guess is that you've got a faulty bms. Your wiring seems fine. What wire gauge are you using?
Check for cold solder joints and the bms for shorts.
```

---
## \#20 Posted by: sterlinggray4 Posted at: 2018-04-26T12:54:26.291Z Reads: 46

```
I thought so too but i just switched to the second BMS I got from Bestech and I'm still having the same issues. I am using 10 gauge pretty much everywhere.
```

---
## \#21 Posted by: RedEagle Posted at: 2018-04-26T13:52:51.938Z Reads: 45

```
Could be a bad batch. Did you check for shorts? 
Is the e switch working?
```

---
## \#22 Posted by: Lambjr088 Posted at: 2018-04-26T22:49:11.416Z Reads: 44

```
I use the D596B. It's 80A I have the li-ion 10s version its the only one out of 3 that I ordered that doesn't work when I test it. But its the eswotch that won't turn it on. Still I see the 8.7volt current running thru it when I connect the leads.
```

---
