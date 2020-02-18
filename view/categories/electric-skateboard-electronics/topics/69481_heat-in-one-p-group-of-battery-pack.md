# Heat in one P Group of battery pack

### Replies: 13 Views: 317

## \#1 Posted by: Mikenopolis Posted at: 2018-09-28T17:57:41.247Z Reads: 152

```
Looking to pick your brains on this while waiting for Dave's recommendation.

The 12s3p battery pack in question is from @oriol360 / MiamiElectric. Because I usually ride/test in 10 mile increments, I know this build has under 100 miles on it. Recently I had some issues with the battery turning off under harder acceleration or on a small incline, same route I always take from the home to office. The board would just not accelerate anymore, the LCD would be off, power button still in on position. A restart and the board would work again until I go a bit faster.

I swapped out the antispark switch, that didn't resolve it. @psychotiller took a look at the battery and didn't really see any physical problems, but he helped change the BMS to charge only. Today I finally had time to test it out after that change. Took it slow because I really didn't wanna street my face before work.

Average Speed 10mph
Max Speed 25.1mph
Distance 6.3 miles
Starting Battery: 98%
Ending Battery: 46%

After the ride, I discovered a hot spot in the battery pack with my thermal camera, looks to be a P group that's hotter than the rest of the pack. Motor temp seems to be fine

![flir_20180928T095937|640x480](upload://jYACBHsFlXdbSt4HXFoeV5zenrF.jpeg) ![flir_20180928T095803|640x480](upload://hQ0cY7DbGJWxiyZ6DusP93Pp7Rr.jpeg) 

After getting back into the office I checked again, and the battery is cooling down, but now I'm not sure I should plug it in
![flir_20180928T102010|375x500](upload://uh7xJndBWTWZYZs4p18zJ9qq7T1.jpeg)
```

---
## \#2 Posted by: Eretron Posted at: 2018-09-28T18:04:06.955Z Reads: 139

```
I guess one of the cells in that p groub is faulty.
```

---
## \#3 Posted by: DavidBanner Posted at: 2018-09-28T18:05:13.427Z Reads: 140

```
that shit is soooo cool - finally we are living in the age of "Predator" and so far no one has had their head ripped off - good times!

Where is the positive lead from the pack coming from, the top or the bottom of the pack?

any chance of some FLIR photos with the enclosure removed?
```

---
## \#4 Posted by: thisguyhere Posted at: 2018-09-28T18:10:59.878Z Reads: 135

```
![image|375x500](upload://wmP7pP5W95vd71eaYlczupYZ2xU.jpeg) 

is there anything else aside from the battery in this part inside the enclosure?

could be

* bad cell in that P group
* cell connection bad / coming loose / slow short
* balance lead going bad

good catch, 90f isn't too bad though but the fact that there's such a variance in the pack is concerning.

according to mooch max operating temp for the 30q is 75c / 170f.

you may want to check on voltage drift, i bet that P group will be lower.
```

---
## \#5 Posted by: psychotiller Posted at: 2018-09-28T20:20:25.656Z Reads: 117

```
I love your camera...I think that you should pay me with that camera to work for me for free. These "are" the droids you're looking for.


we probably need to take that p group out and maybe replace a cell or 3
```

---
## \#7 Posted by: pat.speed Posted at: 2018-09-28T21:10:11.748Z Reads: 112

```
At least now you have a spare bms and as switch 🤷‍♂️

Honestly though I would most likely say that the cells are a lower voltage and because of that they are generating more heat while trying to keep up with the others
```

---
## \#8 Posted by: Mikenopolis Posted at: 2018-09-28T22:47:22.336Z Reads: 104

```
Just took a bit of the shrink wrap off, visibly looks fine, I plug it into the charger and checked the thermal camera and can see the on or two cells that are hotter than the other, I think it's just one cell from the second P group that shows 80.3F. 

EDIT: I just noticed the charger light turned green, and now the thermal camera shows an even temperature throughout the pack.

@psychotiller how hard of a repair would this be given the way this pack is built? any chance of getting it done before CicLAvia on Sunday? Not like it's an issue since both the DIYs are 3Ps anyway. Gonna need that 10s5p for Vegas I think. 

For those wondering. The camera I use is actually my second phone (work vs personal) It's a [CAT S60](https://www.amazon.com/CAT-S60-Thermal-Waterproof-Smartphone/dp/B06Y662YC3). pretty weak GSM Android phone with a built in FLIR camera. 

 ![flir_20180928T152619|640x480](upload://sfwzhrMOZxrr9CJVlI80VfAmlAP.jpeg) ![flir_20180928T152737|640x480](upload://npK8InHDtVv7rNfykyeGYRodNxJ.jpeg)
```

---
## \#9 Posted by: oriol360 Posted at: 2018-09-28T23:47:45.554Z Reads: 95

```
Hey @Mikenopolis

Your first issues with the having to restart the board, it sounds like you were hitting one of the BMS cutoffs, whether it's the 50A max or Voltage cutoff.
I ran into this problem when I would use settings higher than the follow:
The included BMS was 50amps
So each VESC should be set to 25A Battery Max
As for Motor Max should also have been set around 60A each

Moddifing to charge only, will bypass the discharge limits of the BMS, but will introduce new issues like what you are seeing.

I believe, like others have pointed out this issue is due to voltage drift.
Looking at your ride stats 6miles should note have taken you down to 46% unless one of the cells is significantly low. 
I do not believe the cells are the issue here. Although they may have sustained some damage, your testing seems pretty mild unless you are trying to discharge at 100A or have discharge below 2.8v.

Your issue may be with the BMS. First, check that the connection to that P group is solid and not wiggling around. 
After which take a look at the BMS make sure there is no bad electrical smell and all the components look good.

Lastly, you can spot charge that P group to match the voltage of the other cells on the pack, then monitor the drift of the group with your test rides, both before and after charging. 
You can see if it's drifting during discharge(Usually means faulty cells) or drifting when charging(Usually means faulty BMS) and change our accordingly. 

Hope that helps a bit. Also good thing you got @psychotiller there check it out!
```

---
## \#10 Posted by: Mikenopolis Posted at: 2018-09-28T23:56:34.919Z Reads: 91

```
[quote="oriol360, post:9, topic:69481"]
VESC should be set to 25A Battery Max
Motor Max should also have been set around 60A each
[/quote]

Not 100% sure, but I think my BATT MAX is 30A and MOTOR is 60A (maybe changed to 80A this last repair)

the battery was running like a champ for the first five 10 mile test runs, had a motor issue first run, fixed it, then the next thing was mount angle not staying. finally fixed that and then I got the battery shut off issue, thought I got it fixed and now I get this issue......maybe I should just get a Meepo :roll_eyes:

Thanks for your insights @oriol360
```

---
## \#11 Posted by: Eboosted Posted at: 2018-09-29T03:58:46.475Z Reads: 79

```
Mike, may I suggest you check the connections between p-groups, it seems one connection is poor that's why you get more temperature on that spot
```

---
## \#12 Posted by: Lambjr088 Posted at: 2018-09-29T14:30:38.082Z Reads: 60

```
It looks like the hot spots were arpund the areas u stand on that extra pressure on the batteries can b a factor
```

---
## \#13 Posted by: Acido Posted at: 2018-09-29T14:53:55.290Z Reads: 60

```
If its a bestech bms it could be shutting off from over temp/amp or
```

---
## \#14 Posted by: psychotiller Posted at: 2018-09-29T15:20:43.398Z Reads: 56

```
I checked out the pack and it was put together really well. The welds were solid and the everything was laid out clean. I'm charging a few new cells right now and the plan is to switch that group out this afternoon. 

We'll inspect the whole pack again and take some photos to add to this thread for science.
```

---
