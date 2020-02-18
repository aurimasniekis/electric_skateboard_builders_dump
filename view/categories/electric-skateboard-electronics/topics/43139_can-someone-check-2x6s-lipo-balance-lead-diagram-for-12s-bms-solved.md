# Can someone check 2x6s lipo balance lead diagram for 12s BMS (solved)

### Replies: 31 Views: 2328

## \#1 Posted by: dg798 Posted at: 2018-01-08T01:39:04.744Z Reads: 158

```
cant seem to find anything on the forum in regards to a schematic of wiring the balance leads of 2 6s lipos in series.
```

---
## \#2 Posted by: jmasta Posted at: 2018-01-08T01:53:30.794Z Reads: 156

```
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/7/8/782ff289069542c5a6c42c33f1c25047664e83c2_1_512x500.jpg
```

---
## \#3 Posted by: dg798 Posted at: 2018-01-08T01:57:47.146Z Reads: 148

```
I have 2 6s that I need to wire in series
```

---
## \#4 Posted by: jmasta Posted at: 2018-01-08T01:59:44.526Z Reads: 143

```
It's the same concept, dude.
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-01-08T02:27:17.076Z Reads: 133

```
i’m really not trying to be mean, but you may wanna stay away from wiring things yourself and pay someone to make one for you
```

---
## \#6 Posted by: dg798 Posted at: 2018-01-08T02:28:28.656Z Reads: 128

```
I know how to wire things I just don’t want to do anything before I get a schematic that I understand fully, that’s all.
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-01-08T02:30:46.904Z Reads: 126

```
i mean, after the battery incident.  I think you soldering potentially high voltage connections isn’t a good idea.

again, not trying to be mean. just trying to save you from a  potential fire
```

---
## \#8 Posted by: dg798 Posted at: 2018-01-08T02:46:53.921Z Reads: 122

```
I don’t mind trying, I’ve been practicing since then.
I just need to understand how to wire the balance leads in series
```

---
## \#9 Posted by: jmasta Posted at: 2018-01-08T02:57:58.012Z Reads: 124

```
http://www.electric-skateboard.builders/t/10s-balance-connector-series-harness/33051
```

---
## \#10 Posted by: thisguyhere Posted at: 2018-01-08T03:04:15.905Z Reads: 125

```
no man, u don't do anything with the balance leads. I meant u series your two 6s packs. 

the balance leads get directly connected to the bms. 

please, go look at the diagrams post, there's some good examples there.
```

---
## \#11 Posted by: dg798 Posted at: 2018-01-08T03:06:07.530Z Reads: 118

```
oh, I already have my packs wired in series
```

---
## \#12 Posted by: dg798 Posted at: 2018-01-08T03:07:11.581Z Reads: 118

```
how do I know which balance lead is 1,2,3,4-12. How would I go about marking them? Which lead do I start with??
```

---
## \#13 Posted by: Namasaki Posted at: 2018-01-09T01:59:50.512Z Reads: 112

```
The battery pack that supplies negative to the system is battery number 1
The battery pack that supplies positive to the system is the last battery in sequence.

With two 6s batteries in series.
Battery 1 supplies cells 1-6
Battery 2 supplies cells 7-12

<img src="/uploads/db1493/original/3X/2/c/2c137280e677f9767b1ecb1361b21813169ceab7.png" width="149" height="278">
```

---
## \#14 Posted by: dg798 Posted at: 2018-01-09T02:36:05.341Z Reads: 107

```
does this diagram look right?
<img src="/uploads/db1493/original/3X/e/9/e94c5e9c2ecc63845b50fcbbfb31f3d1b0f5fd8f.png" width="505" height="500">
```

---
## \#15 Posted by: dg798 Posted at: 2018-01-09T02:38:13.915Z Reads: 107

```
also my packs balance leads are all black except for the positive of course. How do I know which one is ground if they are all black??
```

---
## \#16 Posted by: craj1031tx Posted at: 2018-01-09T05:49:51.510Z Reads: 102

```
This thread raises an interesting question... I have been using 2 6s Lipos and charging them independently (each one on a 6s external balance charger), but running them in a 12s configuration when they're inside of my board.

This theoretically could mean that while all 6 cells within a single pack are at the same voltage, each group of 6 across the two packs could be at two different voltages (even though the charging 'ends' at ~25.2 volts for both packs, independently, according to the charger, an IMAX B6 clone.)

Will connecting the two packs that were not balance charged with each other lead to issues down the line?
```

---
## \#17 Posted by: Ishayc Posted at: 2018-01-09T06:12:48.850Z Reads: 100

```
@craj1031tx 
No problem, the voltages are just being added.
The other parameters of the two packs must be the same though(Ah, C rating)
```

---
## \#18 Posted by: Namasaki Posted at: 2018-01-09T07:32:07.605Z Reads: 101

```
[quote="dg798, post:14, topic:43139, full:true"]
does this diagram look right?
[/quote]

Your diagram looks  wrong to me.
```

---
## \#19 Posted by: Winfly Posted at: 2018-01-09T10:15:01.913Z Reads: 94

```
This might help you.
<img src="/uploads/db1493/original/3X/3/4/34c3dad50e500d13615210795b8c5e6717fb365e.png" width="540" height="500">
```

---
## \#20 Posted by: SimosMCmuffin Posted at: 2018-01-09T10:24:58.790Z Reads: 91

```
I have not used this BMS, so I'm asking for OP's sake.

Is the "B-" bottom balance tab on the balance connector connected to the main battery lead "B-" tab?
```

---
## \#21 Posted by: dg798 Posted at: 2018-01-09T12:28:04.350Z Reads: 87

```
How do I know which is ground if they are all black?
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2018-01-09T12:31:17.883Z Reads: 87

```
Do you have a multi-meter? You can figure out the way they are wired by measuring the voltages from the balance lead.
```

---
## \#23 Posted by: dg798 Posted at: 2018-01-09T12:40:48.481Z Reads: 85

```
How would I do that
```

---
## \#24 Posted by: krloz Posted at: 2018-01-09T12:51:17.281Z Reads: 85

```
[quote="dg798, post:6, topic:43139"]
I know how to wire things
[/quote]

90% of the messages you write in This post include the words "how do i". I'm not sure you really know what you are doing.  And that diagram is really bad and will destroy the bms.
I'm sure the diagram you need is already on the forum but your best bet is the one posted by jmasta from the beginning.  Only your batteries have each another single wire in between the rest
```

---
## \#25 Posted by: pat.speed Posted at: 2018-01-09T12:58:16.515Z Reads: 82

```
Dude the diagram you posted looks mostly right but why the hell did you swap the order of the red wire and the two black ones after it?

Edit: I looked at it again and that is not right at all if you haven't figured it out by tomorrow I'll draw you a new diagram of how to wire the cells into 12s and you can workout how they connect to the bms. Deal?
```

---
## \#26 Posted by: dg798 Posted at: 2018-01-09T13:49:09.419Z Reads: 86

```
@krloz I have looked all over the forum for a diagram but couldn’t really find one.
@pat.speed I think I understand how to do it now. Will post another diagram later today to make sure I did it right.
```

---
## \#27 Posted by: dg798 Posted at: 2018-01-09T17:49:12.969Z Reads: 85

```
Ok here’s the new diagram. Let me know if it’s better or worse.<img src="/uploads/db1493/original/3X/f/2/f204363183f368d1fcfcb58102c2c7ca31a9fba9.jpeg" width="375" height="500">
```

---
## \#28 Posted by: dg798 Posted at: 2018-01-09T19:53:05.888Z Reads: 84

```
It’s just the balance lead wiring as I want to make sure that’s good.
```

---
## \#29 Posted by: pat.speed Posted at: 2018-01-09T20:38:13.249Z Reads: 83

```
Now you are missing one wire. In the middle middle where the series connection is there should be one wire coming off. Always remember this. However many batteries are in series add 1 and that's how many balance leads there are. So in your case there should be 13 which when you add the one onto the middle cell there will be. 

Now on a bms USUALLY there is only room for 12 wires. That is because it will USUALLY have b- which acts like one balance lead. So USUALLY you leave out the first wire because that is already connected to to the main negative lead which goes to b-. 


That was kinda comfusing to explain. Just check the wiring diagram for that specific bms too just to be sure that's how it connects
```

---
## \#30 Posted by: Winfly Posted at: 2018-01-10T04:21:43.244Z Reads: 83

```

http://www.electric-skateboard.builders/t/solved-wiring-bms-bypass-discharge-10s-anti-spark-help-please/27876

Please reference this post. You are basically doing the same thing but with 2x6S lipo. Your diagram is wrong because the red lead is always the positive end of the battery, which is cell 6 and 12 for you. The remaining black wires should come arranged in order. If you are not confident you should use a multimeter. Since yours came in 1 red wire and 6 blacks. You should measure the voltage across from the negative lead of the battery to the wires. There should be 1 that reads 0V, which you will not need to connect to the bms because that is directly connected to B-. #1 cell should read 3.7V-4.2V (voltage of 1s), #2 read double of that (2s). etc... your red wire should read 6s voltage.

I recommend looking up how to use a multimeter if you don't already know.
![image|412x500](upload://5GetGomHyOMkl9Sl93dUnA7NTCY.png)
![Untitled|659x499](upload://iQp0goiibgSl3WEeJW7aGp7o7XB.jpg)![IdentifyBalanceLead|659x499](upload://i8BBrzuaiSe4y5GKloQtpmfFb20.png)
```

---
## \#31 Posted by: dg798 Posted at: 2018-01-10T05:33:37.115Z Reads: 73

```
Got it thanks
```

---
