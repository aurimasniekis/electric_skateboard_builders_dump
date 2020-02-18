# Heat sinking Focboxes

### Replies: 25 Views: 422

## \#1 Posted by: Andy87 Posted at: 2018-11-27T18:51:31.791Z Reads: 134

```
I have this heat sink laying around 
![image|375x500](upload://jtOYPBH657ikSd75c2qzMo2RfRe.jpeg) 
and thought maybe I can use it to mount my focboxes on to get a better cooling.
My question is now, could I just screw the focboxes with there stock heat sink on my heat sink like this
![image|375x500](upload://d5vh4dqxpVMyhQM0VW1zGXD4dSJ.jpeg) 
and wouldn’t it support the cooling?
Or do I need to dismount the pcbs and mount them directly on my heatsink with a thermal pad inbetween?
I know @Kug3lis is a heatsink expert 😉 maybe you can give me some advice.
```

---
## \#2 Posted by: mmaner Posted at: 2018-11-27T18:53:50.272Z Reads: 128

```
I would get some heat transfer paste/tape and mount them as is directly to the heat sink.  Then cut as small a hole as you can in your enclosure and bolt it to the enclosure, with the fins down.  Once you have the fit perfec, remove it from the enclosure, add some 3m silicone (or other sealant) and re-mount it.

Any idea where you got that heat sink?  Looks nice.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-11-27T19:16:37.138Z Reads: 115

```
I got the sink in our local electronic store for about 5$ 😅
I‘ll mount the heat sink on top of my battery on top of my deck into a custom made 3D case.
So that shouldn’t be an issue.
Just on the focbox I have this terminal on the place of the fets
![image|375x500](upload://pfShjwqou4xeBMtNf2vJrhqp5I9.jpeg) 
As my heat sink is flat, I would need to creat some kind of spacer plus use bigger thermal tape. If no, I think I would short the other contacts from the pcb.
That’s why I came to the idea if it’s possible to use the heat sink of the focbox as it’s already everything cut out right for the pcb and just add some more heat sink on top of it.
```

---
## \#4 Posted by: J0ker3366 Posted at: 2018-11-27T19:25:21.347Z Reads: 103

```
You could buy some plastic stand offs and then you could mount straight to the big heatsink. Unless you're just want to slap it together as is. Either way will work. I would say though, mounting the pcb to the bigger one would be better though.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-27T19:29:28.391Z Reads: 102

```
But for this i would need a 5mm thermal pad
![image|375x500](upload://xQSmuuKk8yEYuAJN4bqMBt74r8V.jpeg) 

Not sure where I can get something like that
```

---
## \#6 Posted by: dareno Posted at: 2018-11-27T19:30:49.032Z Reads: 97

```
More heat sink the better surely.  Do like mike.  Get the fins in the airflow.
```

---
## \#7 Posted by: Sn4pz Posted at: 2018-11-27T19:31:21.405Z Reads: 99

```
I dont know if that pad will be thin enough to do its job well? :thinking:

The regular pad is thin as heck
```

---
## \#8 Posted by: J0ker3366 Posted at: 2018-11-27T19:33:49.750Z Reads: 99

```
Yeah my bad forgot what it actually looked like. So what about cutting the heat sink out of the focbox bottom and then attaching? Same concept as you were thinking. I figure with it just being the heatsink part instead of the whole bottom, your causing a more direct path to the bigger one. I hope you followed that lol. Cloud 9 as usual here lol
```

---
## \#9 Posted by: J0ker3366 Posted at: 2018-11-27T19:36:17.349Z Reads: 90

```
I don't think it will crest enough heat to worry about that. Unless he just ovst amps it down/up hill
```

---
## \#10 Posted by: Sn4pz Posted at: 2018-11-27T19:36:59.547Z Reads: 89

```
I assumed that it would be a high amperage pneumie build, it is @Andy87 :rofl:
```

---
## \#11 Posted by: longhairedboy Posted at: 2018-11-27T19:37:39.400Z Reads: 88

```
put the stock sink back on the focboxes and bolt the big sink directly to the stock sinks. You can do this because there are threaded screw holes ready to be used on the focbox sinks. I'd get some Arctic Silver or other CPU thermal past to smear on the surfaces before bolting together just to make sure they are thermally coupled.
```

---
## \#12 Posted by: akhlut Posted at: 2018-11-27T19:39:04.645Z Reads: 87

```
That's all I did.  made a plate and mounted the focboxes to it with some thermal paste.  Then mounted the plate to the deck.  Does the trick.  Nothing fancy.

![20181122_215707|666x500](upload://clapapslbcn4OwNbjIHrUi2ixR4.jpeg)
```

---
## \#13 Posted by: Andy87 Posted at: 2018-11-27T19:43:04.592Z Reads: 81

```
@akhlut and @longhairedboy thx for confirmation. That was the intial plan. Just add some thermal paste between the sinks and than bolt it together through the holes which already in the stock sink. 
Just wanted to get it confirmed that it will work like this.
```

---
## \#14 Posted by: BigBrit Posted at: 2018-11-27T19:44:30.399Z Reads: 74

```
is heat sinking them necessary? I have been running 45A per VESC in my eboosted enclosure without it for a while.  I do live in the UK mind, we are not famous for our hot weather :joy:
```

---
## \#15 Posted by: Andy87 Posted at: 2018-11-27T19:45:24.897Z Reads: 75

```
Nu i need a bit more than 45a for my 8085 motors 😉
```

---
## \#17 Posted by: BigBrit Posted at: 2018-11-27T19:46:35.697Z Reads: 72

```
700 miles and counting bro... 

@Andy87 I thought Focbox could only handle 50A max
```

---
## \#18 Posted by: dareno Posted at: 2018-11-27T19:47:10.121Z Reads: 71

```
Same and I'm in qld where winter only gets down to a chilly 25 degreesC  Not a heat issue with standard sinks running 40amp per
```

---
## \#19 Posted by: Andy87 Posted at: 2018-11-27T19:47:24.272Z Reads: 71

```
No, 45a should work with the stock sink too.
With the boosted sink it will work even better I think.
```

---
## \#21 Posted by: Andy87 Posted at: 2018-11-27T19:49:02.741Z Reads: 66

```
Ask @Kug3lis how much amps he pull through his focboxes 😉 
It’s a bit more than 50.
Everything just depends how good you can get rid of the heat.
```

---
## \#22 Posted by: BigBrit Posted at: 2018-11-27T19:50:25.407Z Reads: 67

```
fair enough mate, good to know... I am just about to start a Trampa build with a pair of focbox so handy to know this
```

---
## \#23 Posted by: Kug3lis Posted at: 2018-11-27T20:03:28.818Z Reads: 62

```
The best thing when it was 2ºC outside max temp of mosfets were 38ºC at 130A :thinking:  So at winter I can probably amp up some more current

Everything depends on airflow and how fast you can cool it down... If it was water cooling with decent radiator I could guarantee 200a would be flawless :D 

Regarding heatsink I suggest to sand off the surfaces to remove anything what could increase thermal resistance, and mount focbox on it or there is another way. cut out small rectangular piece of aluminium like a in original case to lift up because 5mm thermalpad will like air cooling...

P.S. Don't forget this mosfet package can't run without heatsink as it doesn't have any thermal mass
```

---
## \#24 Posted by: Blitz Posted at: 2018-11-27T20:12:10.008Z Reads: 58

```
Try get some thermal paste that's non conductive.

And shh man drill the holes and sell these babys for 50 bucks a pop ;)
```

---
## \#25 Posted by: Andy87 Posted at: 2018-11-27T20:14:02.175Z Reads: 55

```
It doesn’t matter if the thermal paste is conductive or not if I apply that just between the stock sink and my sink 😉
```

---
## \#26 Posted by: Blitz Posted at: 2018-11-27T20:15:09.704Z Reads: 56

```
Mistakes can happen I've heard of people by mistake sploshing thermal paste all over there motherboards.

It just gives me some peace at mind for me.
```

---
## \#27 Posted by: dareno Posted at: 2018-11-27T20:17:03.863Z Reads: 55

```
[quote="Blitz, post:24, topic:76259"]
And shh man drill the holes and sell these babys for 50 bucks a pop
[/quote]

Once again you have me baffled.
```

---
