# Optimal Gearing ratio for 6 inch wheels?

### Replies: 15 Views: 1148

## \#1 Posted by: nikoli280 Posted at: 2018-02-28T22:36:09.710Z Reads: 178

```
Hi i am trying to find the optimal gearing ration for 6 inch wheels?

my old setup used 15/36 for 80mm wheels 

I have looked at  15/68 or 10/48 

What is the optimal ration for speed to Thrust?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-28T22:37:05.921Z Reads: 175

```
i’m sorry but i have to ask, why do you create so many threads?
```

---
## \#3 Posted by: nikoli280 Posted at: 2018-02-28T22:39:16.170Z Reads: 174

```
I have many questions that i am unsure about, and i think i create threads that are diverse enough to count as separate threads and not be bound into one. I also think that someone can find thees threads and find them useful
```

---
## \#4 Posted by: DavidBanner Posted at: 2018-02-28T22:53:40.732Z Reads: 165

```
gearing ratio can be quite subjective, some folks want top speed, others are happy to sacrifice top speed for more torque. Some people live in Holland where it is flat, others in San Francisco.

I am experimenting with 6 inch pneumatics at the moment myself, I am starting with a 15:60 ratio and will try other size wheel pulleys to get a feel for what is the sweet spot for my skill level, riding style, mission profile, battery and motor config.
```

---
## \#5 Posted by: mmaner Posted at: 2018-02-28T23:01:17.821Z Reads: 181

```
most people use 15/60 or 15/72.
```

---
## \#6 Posted by: b264 Posted at: 2018-02-28T23:07:33.545Z Reads: 179

```
Doing a quick search comes up with a few relevant things

https://www.electric-skateboard.builders/t/esk8-calculator/6693

https://www.electric-skateboard.builders/t/one-calculator-to-rule-them-all/23937

https://www.electric-skateboard.builders/t/esk8-spec-calculator/13024

https://www.electric-skateboard.builders/t/torque-calculations/6855

https://www.electric-skateboard.builders/t/whats-the-formula-to-calculate-top-speed-of-a-e-board/14352

https://www.electric-skateboard.builders/t/are-esk8-calculators-wrong/32626

https://www.electric-skateboard.builders/t/how-to-calculate-speed-for-hub-motor-skateboards/34858
```

---
## \#7 Posted by: nikoli280 Posted at: 2018-02-28T23:11:01.447Z Reads: 136

```
You don't understand my question all of these results are not relevant. I'm not asking for a calculator since I have used that. I asking about experience and feel.
```

---
## \#8 Posted by: nikoli280 Posted at: 2018-02-28T23:11:36.796Z Reads: 137

```
Great can you keep me updated I live in Denmark which is completely flat like Holland
```

---
## \#9 Posted by: b264 Posted at: 2018-02-28T23:13:03.485Z Reads: 134

```
Pick a top speed at which you don't feel safe over, then use the calculator to find the gearing ratio that hits that loaded top speed which maximises motor kv while keeping erpm under 50k

The more greedy you are with your top speed, the less torque you will have, so pick a real-world top speed like 25mph to 30mph
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-03-01T16:09:49.743Z Reads: 110

```
@marcmt88 is making 58T POM pulleys, I think they would be a good match for a 15T motor pulley and a 10s/SK3 190kv(real kv = 170kv iirc) setup, 38kph. Add another 2s and that figure increases to 46mph

there are also options in europe from @Idea - @fottaz  

and probably a lot of other places too
```

---
## \#11 Posted by: mmaner Posted at: 2018-03-01T16:18:37.510Z Reads: 106

```
This is a spreadsheet I put together to calculate data.  If anyone is interested I'm happy to share.

![image|690x438](upload://vAOReglYE7FOiHOzeteSKOBqeUo.png)
```

---
## \#12 Posted by: nikoli280 Posted at: 2018-03-01T17:34:25.308Z Reads: 96

```
Yes please share
```

---
## \#13 Posted by: mmaner Posted at: 2018-03-01T17:47:05.514Z Reads: 96

```
Here ya go...

https://www.dropbox.com/s/5lv681kviqlrann/MASTER%20esk8%20data.xlsx?dl=0
```

---
## \#14 Posted by: janpom Posted at: 2019-03-08T11:51:24.815Z Reads: 59

```
[quote="b264, post:9, topic:47792"]
loaded top speed which maximises motor kv while keeping erpm under 50k
[/quote]

Sorry to revive an old thread, but this is very interesting. If I understand correctly, you're saying that more kv is better (everything else being the same) as long as you don't exceed the erpm limit, right?

For example, say I have 10S battery and 170 kv motor. That should max out at 50k erpm. Now, if instead I used a 85 kv motor and doubled the gearing, how would that compare to the original? What would be the downside? I believe the max speed an the torque would remain the same. Is it just that the motor price would probably be higher?
```

---
## \#15 Posted by: b264 Posted at: 2019-03-08T20:00:07.610Z Reads: 47

```
Typically the motors do run more efficiently at higher speeds / kv for the same loaded ground speed.  However sometimes the gear/pulley ratios you need aren't readily obtainable (for example, 15/36 pulleys are very easy to find but 15/48 pulleys are unobtainium) or are too physically unwieldy (for example, not enough space for a 5:1 gear ratio)

Also, the higher kv motors draw more current for the same voltage, so you need to make sure your ESC can handle it.
```

---
