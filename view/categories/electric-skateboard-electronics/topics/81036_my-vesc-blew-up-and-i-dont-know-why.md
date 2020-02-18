# My VESC blew up and i dont know why

### Replies: 30 Views: 428

## \#1 Posted by: AdamE3399 Posted at: 2019-01-16T10:14:52.358Z Reads: 127

```
So I was just taking my board out for a casual ride like I have for a while, the board in question was nine months old and never had any major problems and I constantly check and maintained the board appropriately, then after a drv failure on my vesc I bought a new one a replaced it with a new one and after only a few rides I felt the motor fail so Iooked down and noticed fire coming from the back of the board where the phase wires come out and as you could imagine I was quite concerned, got home opened it up to find a fried vesc though thankfully the battery was fine and all voltages were even and high at 4.09 volts per cell, I am assuming this is because I have a BMS protecting through discharge, anyway here are the pics:

![20190116_174912|281x500](upload://srpabGcrKKMh1sTxfj1JoWqQQuY.jpeg) ![20190116_174930|690x388](upload://jyQuHLbqWWvJUg0yEafLPwsbZYC.jpeg) ![20190116_174926|690x388](upload://6Qebyxjpayjwx4GBVQDfJWdDPSK.jpeg) ![20190116_174917|690x388](upload://eefAPuK3k7N7Rqu7jVj6B6KfpoO.jpeg) 


Any ideas @JohnnyMeduse ?
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-16T10:20:08.056Z Reads: 118

```
which vesc you had before, which is the burned one?
to what you set your vesc max min values ?
```

---
## \#3 Posted by: AdamE3399 Posted at: 2019-01-16T10:31:39.121Z Reads: 117

```
Ive been using turnigy VESC, and the burned one is also a turnigy, the settings were max bat 30 min bat -20 max motor 60 min motor -40, I don't think it was my vesc settings because I have been using them for nearly 9 months with no issue.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-01-16T10:34:20.477Z Reads: 115

```
jap looks good, but nothing we can know without that you tell us.
how was it mount? was there an opportunity that water could come there somehow? or other things that could cause a short?
maybe other cables close to it etc.
```

---
## \#5 Posted by: b264 Posted at: 2019-01-16T10:34:38.003Z Reads: 114

```
That VESC is done and cannot be repaired
```

---
## \#6 Posted by: Andy87 Posted at: 2019-01-16T10:35:54.227Z Reads: 111

```
are you sure? :thinking: :mage: :thinking:
```

---
## \#7 Posted by: AdamE3399 Posted at: 2019-01-16T10:46:50.326Z Reads: 110

```
All my cables were moved out the way and all connections were heat shrinked, as far as water, I never leave the boards near water and I live in Townsville Aus so I don't even know the concept of rain, so I was thinking maybe it was a manufacturing issue?
```

---
## \#8 Posted by: Blitz Posted at: 2019-01-16T11:03:35.858Z Reads: 107

```
I'd like to  contradict you and say that "all things are possible" but 
that vesc  really looks like someone set it on fire with lighter fluid then striked the vesc with a hammer and then teared the vesc with 2 pliers in a failed atempt to rip it in half.
```

---
## \#9 Posted by: b264 Posted at: 2019-01-16T11:07:16.001Z Reads: 105

```
"Beyond Economical Repair" would be the category
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2019-01-16T20:19:50.055Z Reads: 86

```
@AdamE3399

I’m really sorry but I do not have any Idea at all on what happen. I just suppose it could be one of the power cap that blew up short and the heatshrink cut fire 🔥
```

---
## \#11 Posted by: Turboboard Posted at: 2019-01-17T00:28:20.255Z Reads: 72

```
Maybe with that heat shrink you used didn't allow any/very little heat dissipation and it overheated
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-01-17T00:33:25.907Z Reads: 70

```
vesc are supposed to shutdown if their thermal limit is reached, the vesc is smart enough not to kill itself. and heat shrink should be rated up to 100c without combustion
```

---
## \#13 Posted by: lrdesigns Posted at: 2019-01-17T00:41:24.337Z Reads: 66

```
With this much damage you will probably never know, a good effort though almost burned it right in half. You should get an award :trophy: for most radical vesc meltdown. 

![image|690x472](upload://1eNkv3sEoF6oRT6uiKqduiO1ecJ.jpeg) 

As others said if all is going to plan the software will prevent it from damaging itself, so something physically caused a short, a component came loose or road debris etc etc. Then BOOM! :boom:
```

---
## \#14 Posted by: AdamE3399 Posted at: 2019-01-17T00:44:33.636Z Reads: 63

```
Yeah i was pretty surprised myself as i have had drv errors before but this definitely took the cake.
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-01-17T00:55:35.249Z Reads: 61

```
Ive gotten water on my vesc and all i got were fault codes, and once dried out it worked fine but this is just insane.
```

---
## \#16 Posted by: lrdesigns Posted at: 2019-01-17T00:56:39.296Z Reads: 61

```
I got one wet too and it blew the DRV, no other damage.
```

---
## \#17 Posted by: AlanZhou Posted at: 2019-01-17T00:57:43.215Z Reads: 62

```
mine didn't blow im lucky all i got were drv fault codes and it somewhat worked like sometimes it had power but than no power, i could literally see moisture on the vesc heat shrink because it was clear after i got home

usually esc of any kind dont work when its wet but once dried out it should be all fine.
```

---
## \#18 Posted by: J0ker3366 Posted at: 2019-01-17T01:06:20.870Z Reads: 64

```
It was something in this area
![Screenshot_2019-01-16-18-02-28|281x500](upload://tY0Mzbl6OH8AmsBHR5mhtQPaUv7.png) 
being that was the source of ignition. I'm willing to bet something came loose in that area and crossed with something. Can't say if that's normal wear or factory fault. 

Glad youre good though. So did you get the whole ghost rider feeling with flames coming out the back?
```

---
## \#19 Posted by: TowerCrisis Posted at: 2019-01-17T01:36:37.921Z Reads: 61

```
Coming up next "WTS: lightly used VESC, blown DRV but hardly used, great deal! $100USD"
```

---
## \#20 Posted by: Goonman Posted at: 2019-01-17T01:57:00.780Z Reads: 59

```
In the second image, the drv fet at the top of the image has circular mark on it. For my experience of screwing things up. That FET looks like it shit itself. maybe the phase output shorted somewhere, maybe on the PCB where they are soldered hence the small localised crispy area. were you running fuses or just the BMS?
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-01-17T02:00:16.707Z Reads: 52

```
Wait holdup what brand is the vesc? @AdamE3399
```

---
## \#22 Posted by: AdamE3399 Posted at: 2019-01-17T02:19:15.076Z Reads: 51

```
It was a turnigy
```

---
## \#23 Posted by: AdamE3399 Posted at: 2019-01-17T02:19:45.700Z Reads: 52

```
And though the flames were cool for a second, it sucked when i opened and saw the charred pcb that was left
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-01-17T02:20:42.152Z Reads: 53

```
4.10 or 4.12?
```

---
## \#25 Posted by: AdamE3399 Posted at: 2019-01-17T02:21:39.315Z Reads: 51

```
4.12 
10 char
```

---
## \#26 Posted by: AlanZhou Posted at: 2019-01-17T02:23:21.850Z Reads: 50

```
not the most reliable things from what ive heard, my advice get a tb vesc their only 85$ right now.
```

---
## \#27 Posted by: AdamE3399 Posted at: 2019-01-17T02:24:38.791Z Reads: 49

```
I would but im in Australia and its like 70 bucks shipping so its not really worth it, also i have been running flipsky 4.12s in dual for a while and have been working really well so i might get one of those to run in single as their only 80 bucks
```

---
## \#28 Posted by: banjaxxed Posted at: 2019-01-17T23:47:27.253Z Reads: 35

```
wanna make it a dual? I’m 
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5342?u=banjaxxed
```

---
## \#29 Posted by: b264 Posted at: 2019-01-17T23:49:25.896Z Reads: 34

```
If they only have 80 bucks they probably don't have a lot of things in stock.  I'd venture to say Flipsky has more than 80 bucks.
```

---
## \#30 Posted by: AdamE3399 Posted at: 2019-01-18T00:23:52.960Z Reads: 32

```
Mine has a gaping whole in it, i think i win :slight_smile:
```

---
