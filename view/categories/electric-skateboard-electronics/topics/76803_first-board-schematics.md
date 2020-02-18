# First board schematics

### Replies: 23 Views: 677

## \#1 Posted by: Wisp Posted at: 2018-12-02T16:00:36.063Z Reads: 174

```
Hi,

I'm currently making a build for my first board and I would like to know if my schematics are correct. There are a couple of things that I couldn't find on this forum so I could use the confirmation :sweat_smile:

Main components:
* Battery: 30Q 10S3P
* ESC: FOCBOX
* Motor: SK3 6374 190kv
* BMS: Charge only

I want to build my battery pack with double balance wires. (simplified in the schematic).
1 set for the BMS (11 pin) and 1 set split into 2 (2x 6 pin) for my voltage buzzers. Since there are no voltages buzzers for 10S I split them to check half and half.
Sadly this means that I cannot (to switch it off when not using) put the negative balance wire into the buzzer from after the loop key, at least not for both buzzers.
I solved this with a 2 pole switch to turn them off separately (not ideal...)

The rest of the build is rather generic and should be OK I think.

PS: Thick wires are 12AWG, the thin wires are 20AWG (could be 22 but I have 20 laying around). Is 20AWG OK for 5A charging?
![54|690x387](upload://yJ7zqDCGXbxgbvCVe2gMt4dxCLQ.jpeg) 

Thanks for any help!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-12-02T18:34:26.503Z Reads: 146

```
with the balance leads and voltage buzzers, this works great I've got it on my build with this cable i made
![20180622_140311|375x500](upload://iFSUxrje46YbDeJKL2zeD2d8CQV.jpeg)
```

---
## \#3 Posted by: Wisp Posted at: 2018-12-02T18:53:26.891Z Reads: 127

```
The big connector goes into your BMS and the smaller ones one in the battery one in the buzzer?
```

---
## \#4 Posted by: pat.speed Posted at: 2018-12-02T20:17:59.191Z Reads: 121

```
Yeah, the male to his battery and female to the checkers. I wouldn’t leave the checkers plugged in even when disconnecting the negative wire as it can still draw power from the other cells.
```

---
## \#5 Posted by: ventisca1011 Posted at: 2018-12-03T17:24:30.361Z Reads: 98

```
i need some help from expert ,, this is my schematics for my first build!:smiley:![BMS|375x500](upload://mINCseLEBzIiXu3gDW0BWp0siTa.jpeg)
```

---
## \#6 Posted by: Alex753 Posted at: 2018-12-03T17:32:25.925Z Reads: 83

```
Hey ! 

Everything sounds pretty good to me, what did you whrote between the anti spark and the Watt metter ?
```

---
## \#7 Posted by: ventisca1011 Posted at: 2018-12-03T17:35:14.264Z Reads: 82

```
thx man,, in red line i wrote fuse , im still thinking if i need those or not ,,
```

---
## \#8 Posted by: Alex753 Posted at: 2018-12-03T17:38:34.890Z Reads: 78

```
Oh ok, i don’t use one but maybe it can prevent from over tension while using regenerative brake at full battery ?
```

---
## \#9 Posted by: Wisp Posted at: 2018-12-03T21:19:39.015Z Reads: 72

```
12S9P? What a beast :smiley: 

Your BMS is charge and discharge? Often then there is a direct connection to the BMS for the negative of the charger, but maybe yours doesn't have it.
Else everything looks fine
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-12-03T21:41:02.589Z Reads: 69

```
why do you have buzzers?

voltage cutoff can be set in software...
```

---
## \#11 Posted by: Wisp Posted at: 2018-12-03T21:42:59.497Z Reads: 65

```
I want to see if one of my groups is drifting. If one of them has failure, voltage cutoff of the hole pack won't happen or will happen to late
```

---
## \#12 Posted by: thisguyhere Posted at: 2018-12-03T21:43:43.181Z Reads: 62

```
oh i see, got it.

looks like a lot of splicing but cool if you can get it work.
```

---
## \#13 Posted by: b264 Posted at: 2018-12-03T21:45:05.190Z Reads: 69

```
You should wire the battery P-packs so they connect together in the middle instead of connecting to their neighbor and needing to be insulated from the cells across from them.  It's a far, far higher risk the way you drew it.

![connections|610x460](upload://abaq8WOXm5Cc1sQiBRd5nC6sJoz.png)
```

---
## \#14 Posted by: Wisp Posted at: 2018-12-03T22:17:21.242Z Reads: 64

```
I get what your are saying but don't see an increased risk. Insulation of the cells across them is rather easy and since I want to spot weld to a nickel plate and then connect the series with braided wire and solder it is harder to do if I need to connect in the middle. Any sugesstions?
```

---
## \#15 Posted by: b264 Posted at: 2018-12-04T02:31:34.917Z Reads: 62

```
I'm not sure the best way, but this is a way I've done it

![20180924_001917_HDR|690x345](upload://llAAbGcprXCEwPwOFfcRNQoR3EU.jpeg) 

![20180923_235853|249x499](upload://3rIEehMcTAYEXIUJs7nhbScTQrj.jpeg) 

![20180924_001139_Burst01|690x345](upload://f5p5sJg3gQJnAnDElod63vWe8Hw.jpeg)

and then of course lots of fishpaper and stuff to deal with vibrations
```

---
## \#16 Posted by: swimmydude Posted at: 2018-12-04T03:19:14.648Z Reads: 58

```
I know I could probably look it up but I'm honestly exhausted jumping down this battery rabbit hole. Is there a difference between regular braided copper wire and tinned braided copper wire, at least for the application of a battery pack? Afaik, tin isn't all that conductive. Is it just a protective barrier?
```

---
## \#17 Posted by: b264 Posted at: 2018-12-04T03:20:58.591Z Reads: 58

```
It means the solder sticks to the tin very well, unlike copper.  Copper you have to tin yourself first.  Plus, tinned copper won't corrode.  "Tin" here is a verb and not a noun.  It means "to apply the thinnest coating of solder (tin & lead) so that the next solder operation works better."

You want tinned 0.25" braided copper which is good for 40A continuous.  2 of them for 80A continuous.
```

---
## \#18 Posted by: swimmydude Posted at: 2018-12-04T03:29:08.078Z Reads: 57

```
oh wow, derp. I'm familiar with soldering and while I'm not an expert, I consider myself somewhat proficient with it. So when looking at the term tinned copper, it completely flew over my head it was referring to tinning the copper and not just copper with another element coating it. Thanks.
```

---
## \#19 Posted by: Wisp Posted at: 2018-12-04T14:09:51.712Z Reads: 48

```
Thanks! But I still don’t see what the increased risk is, care to elaborate?

Ps: I don’t have the rights to see the topic in your previous post
```

---
## \#20 Posted by: b264 Posted at: 2018-12-04T16:57:33.284Z Reads: 42

```
When you have the ends of cells butting up against each other with an insulator between them, then you subject it to violent and heavy vibrations (aka: riding the board) then the sharp metal can wear through the insulator and touch the neighboring cells, causing a short and fire.  Unless those two cells are already connected together anyway.... then there is no short.

You're increasing fivefold the amount of risk for no gain
```

---
## \#21 Posted by: Wisp Posted at: 2018-12-05T22:10:58.901Z Reads: 36

```
Ok, got it. Thanks!
```

---
## \#22 Posted by: Wisp Posted at: 2018-12-28T18:27:47.546Z Reads: 33

```
Hey, what do you think of this way instead of braided wire? He connects them with nickle tabs and then bends it over. Any remarks concerning amps, vibrations, etc?
https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102/162?u=wisp
```

---
## \#23 Posted by: bigben Posted at: 2018-12-28T18:34:59.597Z Reads: 32

```
Thanks for linking this! I do like the way @b264 does this. The way I've done is is quite possibly inferior but well recognised way to do it by a lot of commercial pack manufacturers.. I will now very likely build a pack this way. My only comment would be that with the 5 strips of nickel, the current will flow in 5 places rather than 2. Although in practice with the pack compressed that probably won't be the case. If you follow?
```

---
