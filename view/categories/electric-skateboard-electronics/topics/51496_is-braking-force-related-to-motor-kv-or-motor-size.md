# Is braking force related to motor KV or motor size?

### Replies: 44 Views: 1690

## \#1 Posted by: Eboosted Posted at: 2018-04-07T17:05:27.106Z Reads: 256

```
I got two 6384s 200KV from APS for my Trampa build, I love how the board rides and accelerates but the braking force is somewhat weak, I've increased the battery min from -12A up to -20A per VESC but it's still pretty poor. I'm running a 12S4P of 30Qs. I wonder if I should lower the motor KV down to 170to increase braking.

Motor pullies are 62T and motor pullies 14T, the issues might also been related with too high speed 75.59kph unweighted and 64.25km/hr weigthed.
```

---
## \#2 Posted by: Deckoz Posted at: 2018-04-07T17:11:48.566Z Reads: 250

```
You running stock vesc to firmware on the  escapes or ackmaniacs..as stock vesc toool braking is balls..
```

---
## \#3 Posted by: Ishayc Posted at: 2018-04-07T17:12:21.980Z Reads: 245

```
If you increase the ratio between the wheels and motor the braking will get stronger.
```

---
## \#4 Posted by: Deckoz Posted at: 2018-04-07T17:13:47.411Z Reads: 240

```
I can almost guarantee it is the VESC tool version he is running. It's a known issue....

If your on 3.xx, the only firmware I would run is the 3.100 ackmaniac. Because the braking algorithms bvedder changed it to make no sense. Ack put it back to work like 2.18 & 2.54.
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-04-07T17:20:43.471Z Reads: 233

```
Breaking force is both related size of stator and kv 20 amp for 2 should be enough. but I also think it's a problem with VESC tool.
```

---
## \#6 Posted by: Deckoz Posted at: 2018-04-07T17:21:29.207Z Reads: 224

```
https://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268/308?u=deckoz

Here is one of the references. As well Ack mentions it in his Ack ESC tool thread.

[quote="Ackmaniac, post:1, topic:35116"]
Brakes can be stronger than acceleration. This way a weak acceleration but strong brakes can be defined which should be safe for kids
[/quote]
```

---
## \#7 Posted by: Eboosted Posted at: 2018-04-07T17:58:32.566Z Reads: 200

```
[quote="Deckoz, post:6, topic:51496"]
well Ack mention
[/quote]

I'm running 3.100 from @Ackmaniac, so it's not a firmware issue, I'm exchanging the pullies frm 62t to 72t and will see how it works.
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-04-07T18:14:18.028Z Reads: 185

```
I am running 6384 170kv from APS and brakes are freaking huge like if I brake bit too hard I can fly off the board... But stading brakes are shit like if I stand on hill with fully braked board goes backwards...
```

---
## \#9 Posted by: Eboosted Posted at: 2018-04-07T18:18:33.894Z Reads: 179

```
What are your VESC settings?

What's your pulley ratio? (pulley teeth count)
```

---
## \#10 Posted by: E1Allen Posted at: 2018-04-07T18:22:50.419Z Reads: 175

```
What's motor min?
```

---
## \#11 Posted by: Eboosted Posted at: 2018-04-07T18:30:30.698Z Reads: 172

```
These are my settings:

Motor max 100A
Motor min - 65A
Batery max 40A
Battery min - 20A
```

---
## \#12 Posted by: E1Allen Posted at: 2018-04-07T18:36:31.122Z Reads: 169

```
Could increase motor min to -100, are your ppm settings giving you a full 100% positive and negative on your throttle?
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-04-07T18:43:31.218Z Reads: 167

```
I am running at the moment default settings 60A
```

---
## \#14 Posted by: Bjork3n Posted at: 2018-04-07T18:46:54.902Z Reads: 163

```
Is it really safe to run -20 on each vesc on batterymin when using a 12s4p 30q?
The max amp charge is 16A? So -16 should be the limit?
I run -8 on each vesc on my build with a gearing 16/36 with 83mm wheels. The brakes are weak at highspeed but ok from medium to slow speed.
```

---
## \#15 Posted by: E1Allen Posted at: 2018-04-07T18:58:47.771Z Reads: 154

```
[quote="Bjork3n, post:14, topic:51496"]
e max amp charge is 16A? So -16 should be the limit?
[/quote]

Probably so. And split between both vesc
```

---
## \#16 Posted by: Eboosted Posted at: 2018-04-07T18:59:57.782Z Reads: 147

```
I have the same settings on my Darth Maul but instead of 200kv I have 190kv motor 15/40T gearing instead of 14/62Ts and 107mm wheels instead of 200mm and it brakes perfectly
```

---
## \#17 Posted by: Acido Posted at: 2018-04-07T19:07:44.286Z Reads: 144

```
30q are max 5 a per cell(if i remember well) charging thats 20a in your 4p pack so i would put max 12a per vesc
```

---
## \#18 Posted by: Bjork3n Posted at: 2018-04-07T19:08:55.954Z Reads: 143

```
dont you mean -10 per vesc then?
```

---
## \#19 Posted by: Acido Posted at: 2018-04-07T19:10:19.002Z Reads: 143

```
Its okay to put it a little bit higher because you will never be breaking at 20a for more than just a second or two so you can put it a little bit higher
```

---
## \#20 Posted by: Acidfie Posted at: 2018-04-07T19:18:03.447Z Reads: 141

```
Braking force is **NOT** related to kV.

i already had a discussion about torque from kv differences, see kv has nothing to do with torque. 

the **higher** the kv, the **more amps** the ESC has to supply to generate the same amount of torque compared to a lower kv motor.

still, there will be a limit for braking, but i think were talking about forces we will not reach while driving and braking, beforehand your wheels will lock up.
```

---
## \#21 Posted by: E1Allen Posted at: 2018-04-07T19:55:27.249Z Reads: 132

```
![IMG_4742|281x500](upload://wQi0zVjEsy1jkliq3uRcjPgJxkJ.PNG)

Max 4a each
```

---
## \#22 Posted by: Eboosted Posted at: 2018-04-07T19:55:31.507Z Reads: 127

```
Then the answer is that I'm running an incorrect reduction ratio, I'll confirm it in 1 hour as soon as I replace the 62Y with 72T pullies
```

---
## \#23 Posted by: E1Allen Posted at: 2018-04-07T19:59:08.192Z Reads: 126

```
Just looked at your post about your calculated top speeds.  That seems pretty high and would account for slower acceleration and braking.  It doesn't seem like you're reaching those speeds on your setup
```

---
## \#24 Posted by: Acidfie Posted at: 2018-04-07T19:59:31.098Z Reads: 122

```
as long your belt isnt skipping you can heighten up that brake current.. i think maxing out will not destroy your motor since its no constant amperage generating while braking.
```

---
## \#25 Posted by: E1Allen Posted at: 2018-04-07T20:00:50.682Z Reads: 115

```
But 64km/hr on Trampa... U reach those speeds @Eboosted ?
```

---
## \#26 Posted by: Eboosted Posted at: 2018-04-07T20:04:54.961Z Reads: 116

```
I didn't have the correct pulley set at the time, I just got the 72T pulleys so I'm testing.

I'll report back in a moment
```

---
## \#27 Posted by: Pedrodemio Posted at: 2018-04-07T20:15:27.679Z Reads: 116

```
The main problem is that we don't know the max charge current the cells can take. Yes, they are list at 4A at the data sheet, but that number is for a full charge cycle, from 0% to 100% in one go, in our case the brake peak break current happens for what? 10 seconds max? the cells won't explode if you put higher than the data sheet says, within reason

Personally I prefer to have a battery that last a little less (number of cycles) and can brake me when I need than be conservative with it and one day go flying over a car because my board couldn't brake in enough time.

In my case the max charge current of NCR GA is 1.65A, if i set to that it's the same as having no brakes, so i run each at 5A and I can stop wherever i like, saved me from a few scratches a few times
```

---
## \#28 Posted by: Ackmaniac Posted at: 2018-04-07T20:23:31.498Z Reads: 115

```
Just measure your motors kv. You can do so in the terminal tab of the ESC-Tool. For example all 6374 190 kv motors that i have seen so far are 170kv motors. Maybe with your 200kv motors it is the opposite. Possible they are even 213 or 230. 

And just simply raise your motor min value. if the ratio has a 30% higher gearing than your other setup then it also needs 30% more amps to reach the same torgue.
```

---
## \#29 Posted by: Battosaii Posted at: 2018-04-07T20:23:50.532Z Reads: 117

```
Brakes on my 16/33 107mm top speed set up had ok brakes but I have to anticipate braking at high speeds cause it's take a bit to stop. My 16/36 107mm daily set up had decent brakes but if I lean correctly I can fully brake so I may change it from -60 motor to -80
```

---
## \#30 Posted by: Sebike Posted at: 2018-04-07T20:48:25.027Z Reads: 112

```
I tried to address this before, but got no response. In the esc tool (ackmaniac) it won't give any reads when typing kv, just sais calculated kv is 0 erpm while giving full throttle
```

---
## \#31 Posted by: Eboosted Posted at: 2018-04-07T20:49:28.589Z Reads: 114

```
[quote="Sebike, post:30, topic:51496, full:true"]
I tried to address this before, but got no response. In the esc tool (ackmaniac) it won’t give any reads when typing kv, just sais calculated kv is 0 erpm while giving full throttle
[/quote]

I think we have to run a little bit and then write KV on terminal
```

---
## \#32 Posted by: Sebike Posted at: 2018-04-07T20:51:02.530Z Reads: 105

```
I've tried multiple times and always got no read. How long would you say is needed approximately until it can get a proper read?

Edit: Let it run for about 1 minute but still saying 0.

Don't want to hjack this thread, but just saying that this method might not work for all and I haven't seen a solution for it yet. 

If anyone knows how to fix this issue, best place to do so would be in the ackmaniac esc tool thread. Thanks :hugs:
```

---
## \#33 Posted by: E1Allen Posted at: 2018-04-07T21:35:50.955Z Reads: 102

```
I had to run the motor using the arrow key and type kv then enter while the motor was running
```

---
## \#34 Posted by: Eboosted Posted at: 2018-04-08T01:06:21.322Z Reads: 92

```
Ok, I was able to test the board with 72T pullies and it has more torque and more braking force, board feels way more fun, but I still need more braking force.

I'm going to increase motor min from -65a to -80A and reduce battery min from -20A to to -16A

Let see what happens
```

---
## \#35 Posted by: Pedrodemio Posted at: 2018-04-08T02:00:21.082Z Reads: 90

```
When the brake is weak? At top speed or close to zero? If it’s weak at top speed but good at low you need more battery current, it it’s weak across all speeds you need more motor current, and possibly battery also
```

---
## \#36 Posted by: Eboosted Posted at: 2018-04-08T02:41:50.181Z Reads: 88

```
It's weak on all speeds. However I had the same setup before and the brakes were pretty good the only difference was a lower kv motor and 1 teeth less on motor pulley (13T instead if 14T), hence the reason I posted this thread
```

---
## \#37 Posted by: Pedrodemio Posted at: 2018-04-08T03:20:53.820Z Reads: 84

```
You said you have a Bluetooth module right? Try recording the ride and doing a full brake from top speed to zero, then we can see what’s happening
```

---
## \#38 Posted by: Eboosted Posted at: 2018-04-11T04:32:54.074Z Reads: 69

```
Time to update this thread.

My old setup was this:

14/62T pullies
Motor max 100A
Motor min -65A
Battery max 40A
Battery min - 20A

My new setup is:

14/72T pullies
Motor max 100A
Motor min -80A
Battery max 40A
Battery min -16A

The board brakes like a dream now, acceleration is unreal, top speed is adecuate and I can't reach it because of speed woobles on a Trampa board, but it's stable until 40km/hr

I don't want to ride anything at all besides this board now. 

I even increased throttle 10% polynomimal and I LOVE IT!
```

---
## \#39 Posted by: lrdesigns Posted at: 2018-04-11T05:06:52.976Z Reads: 64

```
[quote="Eboosted, post:38, topic:51496"]
My new setup is:

14/62T pullies
[/quote]

Typo? Seems like you put on a bigger wheel pulley?
```

---
## \#40 Posted by: Eboosted Posted at: 2018-04-11T06:14:56.845Z Reads: 59

```
Ups, correct. I'm fixing it right now.

Thanks!
```

---
## \#41 Posted by: L3chef Posted at: 2018-04-11T06:46:05.111Z Reads: 55

```
What size tyres you have?
```

---
## \#42 Posted by: E1Allen Posted at: 2018-04-11T06:50:00.531Z Reads: 56

```
Sweet. Glad the board runs good now
```

---
## \#43 Posted by: Eboosted Posted at: 2018-04-11T06:50:31.052Z Reads: 57

```
200mm Primo Alpha 8"

![20180408_224216|666x500](upload://cv784Ohh7EWS54n0tFCUHk9LIc4.jpg)
```

---
## \#44 Posted by: L3chef Posted at: 2018-04-11T06:59:03.455Z Reads: 55

```
Nice! I've 8" trampa tyres aswell with 16-72 pulley. 10s4p..
Love the acceleration and brakes on it
```

---
