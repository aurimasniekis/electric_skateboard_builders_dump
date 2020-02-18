# Mounting 3D printed pulleys to the motor drive shaft?

### Replies: 24 Views: 1846

## \#1 Posted by: TheFluffiest Posted at: 2018-02-14T18:28:29.049Z Reads: 168

```
Hi there, I am having problems with mounting a 3d printed HTD5m 15mm width pulley to my sk3 5055 motor shaft. Currently, I have a set screw going through the printed teeth into the drive shaft, which I have dremeled flat. I know 3D printing isn't ideal for the motor pulley, but I don't have the money to but them right now. I am printing with Nylon, as it's the strongest I have. The problem I am running in to is after about 10 feet, the pulley starts slipping on the drive shaft. I used to have the problem of the pulley falling off the shaft, but I seem to have fixed that. 

Anyone have any ideas? How did you solve this problem?
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-02-14T18:36:54.082Z Reads: 164

```
I wound’t recomend 3D printing for the motor pulleys, since there are fewer teeth’s in mesh the stress in much greater than the wheel pulley

I tried it one time, it lasted approximately 100m before half of the teeth were destroyed
```

---
## \#3 Posted by: HighMasterGogo Posted at: 2018-02-14T18:47:29.325Z Reads: 153

```
This^ 10chars
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-02-14T19:05:38.074Z Reads: 147

```
Even with nylon? Isn't this kind of thing what nylon is made for? Like I said, it's only temporary for about a week or two. Currently it's at 16 teeth, but I can adjust it to around 20 so there's more contact.
```

---
## \#5 Posted by: Achmed20 Posted at: 2018-02-14T19:08:47.210Z Reads: 138

```
screwing them down didnt work for me. 
i filed my motorsdhaft into a D shape and just glued it on. which worked for last ~100km so far.
```

---
## \#6 Posted by: TheFluffiest Posted at: 2018-02-14T19:11:29.974Z Reads: 135

```
I've tried glueing it using JBWeld, but it came off as soon as I tried it. It might be a matter of needing to file it down more so it can have a rougher surface to grab on to. What kind of glue did you use, what motor do you have, how many teeth on the motor pulley, and what material did you use to print?
```

---
## \#7 Posted by: Achmed20 Posted at: 2018-02-14T19:16:01.778Z Reads: 133

```
Turnergy 6374 190kv, 15 or 16 teeth and loctite 648.
but to be fair, the glue had about 2 weeks to settle and also, im not realy sure if i just got lucky since the glue is actualy metal glue and should not realy work to well with nylon
```

---
## \#9 Posted by: TheFluffiest Posted at: 2018-02-14T19:31:40.553Z Reads: 129

```
Good to know. Is there any way I could see the original CAD file, or at least the STL? Thanks for your help!
```

---
## \#10 Posted by: Achmed20 Posted at: 2018-02-14T19:44:18.154Z Reads: 130

```
this is what i used. you can just generate about every gear u need with this (using scad)

https://www.thingiverse.com/thing:16627

here is my edited version with the added D shape
https://www.thingiverse.com/thing:2794331
```

---
## \#11 Posted by: TheFluffiest Posted at: 2018-02-14T22:35:42.876Z Reads: 111

```
Have you had to replace your 3d printed pulleys at all? If so, what happened?
```

---
## \#12 Posted by: Achmed20 Posted at: 2018-02-15T02:15:48.186Z Reads: 101

```
the large one (wheel) including the motor pulley, 1 time . 
it failed because the smaller one failed (petg) and that one failed because i had belt skipping before. so i completly overtightend which led to way to much friction resulting into heat which just melted both pulleys. lesson learned, sticked with skipping belts while braking and so far the parge one survived.

the small one i replaced (while experimenting) a few times.
- no 1, PETG,  failed because i didnt use  enough wall thickness (2 layers). broke at the screw holder
- no2, PETG, failed because i overtightend the screw which cracked the pulley allready
- no 3, PETG, worked flawlessly, but i had to remove it because i got a new mount
- no 4. PETG, wasnt put on properly (had a slight angle) and wobbled. because my new PETG i had back then overextruded liek alot and i couldnt fit it on propberly and had to use some brute force.
- no 5, nylon, failed because the d-shape on my motor shaft had to sharp edges which basicly cut through the nylon when accelerating hard. could have also been not enough infill. no screw this time
- no 6., nylon, was glued on, no screws and i removed the shard edges. infill was grid at 50%. so far, so good ^^
```

---
## \#13 Posted by: Scoo_B_SK8 Posted at: 2018-02-15T02:15:52.668Z Reads: 99

```
i use all 3d printed parts; PLA, HTCFPLA, PETG, ABS, TPE.

never used metal parts yet...on the way though so i have comparison.  

biggest thing that helped me out attatching motor pulley was this...
https://www.amazon.com/flite-Prop-Adapter-8mm-Shaft/dp/B001J8R8ES
```

---
## \#14 Posted by: Scoo_B_SK8 Posted at: 2018-02-15T02:18:42.468Z Reads: 94

```
also added guide walls to both motor and wheel pulleys to prevent belt slipping off
```

---
## \#15 Posted by: pixelsilva Posted at: 2018-02-15T05:33:18.048Z Reads: 91

```
How this helped you out? Don't get it?
```

---
## \#16 Posted by: pixelsilva Posted at: 2018-02-15T05:33:33.333Z Reads: 86

```
Say again??
```

---
## \#17 Posted by: TheFluffiest Posted at: 2018-02-15T07:58:58.985Z Reads: 80

```
Can you post a picture of your setup so I can see what you mean?
```

---
## \#18 Posted by: TheFluffiest Posted at: 2018-02-15T08:04:48.461Z Reads: 81

```
I currently have nylon on hand, so I will continue testing. I made my own pulley with the D thing, so I will see how it works. I have been doing between 6-8 walls on my prints with 40% grid infill, and haven't had any problems with it breaking, I just can't get the grub screw to bite into the nylon enough :laughing: I will keep the sharp edges thing in mind. Is there any other suggestions you might have? Sorry about all the questions, I just want to make sure I get it right this time! Thanks!
```

---
## \#19 Posted by: TheFluffiest Posted at: 2018-02-15T08:07:15.826Z Reads: 83

```
What material and settings in terms of wall thickness and infill did you use for the motor pulley? What motor did you use? Out of curiosity, what did you use for a motor mount? Mine is 3d printed with steel rods through it, prototyping with PLA and finished product with Nylon and eventually carbon fiber filled.
```

---
## \#20 Posted by: Scoo_B_SK8 Posted at: 2018-02-15T12:02:36.179Z Reads: 71

```
i know on 3D printed rod couplings for nema steppers, some make use of a Nut that slides into a void on coupling similar to this...
https://cdn.thingiverse.com/renders/25/e3/48/31/ac/Z_couple_Parametric_42_2_0.75_preview_featured.jpg

although i would recommend doing 2... as to balance it out.
```

---
## \#21 Posted by: Achmed20 Posted at: 2018-02-15T12:45:01.439Z Reads: 65

```
my linked pulley has this, but those are pretty unreliable with the amount of torque the motors spits out.
its to punctual
```

---
## \#22 Posted by: Scoo_B_SK8 Posted at: 2018-02-15T13:08:17.443Z Reads: 66

```
@TheFluffiest 
motor mount i did exactly the way you said, bolts run through entire mount.  used "High Temp Carbon Fiber PLA" @100% infill.

i should have paused a bit longer before the reply to motor shaft as my build is a bit unconventional.  

i can send or post my build with pics/vids .scad files or .stl files. (when i find 'em all & present properly)

have a video on youtube can try and view setup (video was when i was testing 3D printed belts, which i still use).
https://www.youtube.com/watch?v=Efco5Im3YsU


@Achmed20 just took a quick view earlier just now saw the nut void when looked again in thingview.  not surprised about slippage with amount of torque coming from experience in 3D printer couplings with same issue.  is why i went with the prop adapter(<=== ZERO slippage).
```

---
## \#23 Posted by: TheFluffiest Posted at: 2018-02-15T17:28:35.638Z Reads: 62

```
That does look quite unconventional, I'm very intrigued as to what is going on! If you are willing, please post it! I'm sure it can help someone in the future too. I tried the nut-in-void (TWSS) thing but same problem; too much torque.
```

---
## \#24 Posted by: xilw3r Posted at: 2018-02-16T15:33:09.369Z Reads: 55

```
3D printed belts? Still using?

Must see. more details pls !
```

---
## \#25 Posted by: MD84 Posted at: 2018-10-23T03:26:14.428Z Reads: 36

```
I haven't tried machining on the shaft yet. I am waiting on my motor but I will need to do some work on it. I assume they are hard steel. I would maybe suggest filing down a very nice full flat maybe a third way down the diameter of the shaft. The flat would need to be as far down the length of the shaft that your pulley rides. Then print your pulley with a flat on it. Try not to have any void between the pulley and the shaft, it should be a perfect match.

Maybe another idea would be to drill all the way through the shaft and allow the set screw to act as a pin. Perhaps you could tap the shaft to match your set screw.

edit: somehow I missed many of the replies above....same answers
```

---
