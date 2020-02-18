# Are anti spark switches necessary?

### Replies: 13 Views: 3222

## \#1 Posted by: Entonic Posted at: 2017-07-29T18:08:15.536Z Reads: 461

```
So I know that there is a lot of forums about this topic, but are they really necessary? I am using a toggle switch with a rating of 15A and 250V and I have it directly connected to my battery and my VESC-X. I'm using 2 3s 20c zippy's in series. I've been riding this for probably 30 miles so far, and I have had zero problems turning it off and on. No visual sparks, or anything like that. Am I really dumb for having this set and using it for so long? I want to get an antispark switch, but I don't want to spend $50+ on just a switch. Heres a picture of what I have: <img src="/uploads/db1493/original/3X/f/6/f69a6a9d74e1cb301bd6ab2eaa56e5ad759928af.jpg" width="375" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-29T18:09:58.709Z Reads: 441

```
Your 15A switch is essentially acting as a fuse, I would advise against using it as the current limit is way too low. You can instead build a loop key if you want something on the cheap.
```

---
## \#3 Posted by: Entonic Posted at: 2017-07-29T18:12:16.287Z Reads: 431

```
Alright, thanks Jinra. I'll do that.
One other question: Do you need to use XT90's for the loop key or can you get by with XT60's?
```

---
## \#4 Posted by: evoheyax Posted at: 2017-07-29T18:13:03.403Z Reads: 424

```
I personally just just my negative connected and use a 5.5mm bullet connector that sticks out of my board for the positive. You get a big spark, and it eats away at your connectors, but it won't damage your focbox.

The xt90 loop key is the best solution though for cheap.
```

---
## \#5 Posted by: Entonic Posted at: 2017-07-29T18:13:54.114Z Reads: 412

```
Does it have to be a XT90 not a XT60?
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-29T18:15:42.518Z Reads: 396

```
You can use XT60's, but there's an antispark XT-90s you can readily buy

https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
```

---
## \#7 Posted by: Entonic Posted at: 2017-07-29T18:16:46.054Z Reads: 374

```
Alright thanks for the help. I found some on amazon that I'll probably get.
```

---
## \#8 Posted by: Kempo1 Posted at: 2018-10-27T17:09:47.078Z Reads: 202

```
Jinra i just purchased a focbox and don’t want to short it out and I am new to electric builds. Can you upload a picture of how your wire setup is?
```

---
## \#9 Posted by: SeanHacker Posted at: 2018-10-27T17:14:50.060Z Reads: 198

```
This is how I do loop keys (for dual vesc builds) @Kempo1. 

![IMG_20180813_144439|690x388](upload://xImxXtrtr6SLpeFJrqQUuIdiN7E.jpg)
```

---
## \#10 Posted by: Kempo1 Posted at: 2018-10-28T17:33:32.268Z Reads: 175

```
thank you. I have a single motor so i will give it a go today. i fried out 2 xt60 connectors already this week because i didnt have an anti spark connector in my board thats only 5 months old. Any reason on why it would do this? i understand the that both sides must have equal resistance correct?
```

---
## \#11 Posted by: Livid Posted at: 2018-10-29T13:01:46.249Z Reads: 160

```
I just connect and disconnect my main pack to power on and off my board, there's a pretty big spark but nothing i'm not used to with other HV stuff i do, i just use a toothpick to spread out the xt60 pins every so often and it's not a problem
```

---
## \#12 Posted by: threebysix Posted at: 2018-10-29T14:30:37.894Z Reads: 152

```
All those big sparks would make your connectors wear out faster though which is fine, just need to replace it more often.
```

---
## \#13 Posted by: Livid Posted at: 2018-10-29T14:37:12.435Z Reads: 147

```
If you plug the connector in slightly skewed so as to bias the side that sparks it'll last basically forever
```

---
