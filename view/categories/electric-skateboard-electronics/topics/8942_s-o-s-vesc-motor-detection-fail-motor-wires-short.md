# S.O.S. Vesc motor detection fail: motor wires short

### Replies: 13 Views: 1507

## \#1 Posted by: kyo Posted at: 2016-09-05T03:17:49.466Z Reads: 208

```
First, some info : last week i did motor detection with vesc, using laptoplike charger 19v 3,42a. It SPINED, but detection failed, thought there was not enough juice. More details in my build thread.

http://www.electric-skateboard.builders/t/air-blade-enertion-r-spec-6372-10s5p-tb-single-motor-kit-never-summer-el-jefe-board/6203/37?u=kyo 

Last night, i did the detection with 18650  10s5p, connect everything: motor, vesc, computer, bat. The bldc tool connected

Then i clicked dectect button, instantly a little short sound popped up, and i disconnected the bat in panic and found out this:

<img src="/uploads/db1493/original/2X/c/c4c7893b2a12c29a7a37d034e7c250edc5195630.jpeg" width="500" height="500">(re-stage)

Two of the motor wires were touching each other. Damn i forgot to put the heat shrink tube in like i did last week, the eager to make it quick to show off (my brother and father were there) get me off guard. I am usually carefull, double check everyting with a list. 

Back to the story, there is no spark, no smoke, no smell( yes i smelled everything repeatedly motor, vesc, bat) no burn that can be seen, i checked the resistor of the motor using voltmeter, it was very low (around 0.05ohm) i think it is fine.

Then i setup everything again(with 10s5p), connected successful, read, write still good. The nunchuck worked fine( green bar went right, left accordingly to the joystick) 

is my vesc still good? Or dvr chip is a goner? @chaka @onloop @lowGuido @JLabs @Michaelinvegas     

I did detection again. NO spin, vesc flash red 3 times i think then "bad motor detection" :scream:

I dont know what to do. Where can i get my vesc fixed? :sob:

Here are some pics i took with my phone.
<img src="/uploads/db1493/original/2X/3/381410096a640bf24aa0b1dd6b6972f3fc7d5748.jpeg" width="500" height="500"><img src="/uploads/db1493/original/2X/3/31d830d07d013aedba5e5b065bea338c94b29990.jpeg" width="500" height="500"><img src="/uploads/db1493/original/2X/a/a3fa199bfd4d2beb2473fbe491979bfe4b48c5df.jpeg" width="500" height="500">
```

---
## \#2 Posted by: JLabs Posted at: 2016-09-05T03:42:23.934Z Reads: 197

```
Hmm dosnt sound like a DRV failure. Sounds like something else is blown. But I am not a master of the vesc like @chaka
```

---
## \#3 Posted by: kyo Posted at: 2016-09-05T04:14:31.881Z Reads: 194

```
Thanks @JLabs

@torqueboards can you take a look at this? Please
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-05T04:21:16.214Z Reads: 191

```
check your faults in terminal. type "faults"after the bad detection
```

---
## \#5 Posted by: torqueboards Posted at: 2016-09-05T04:24:09.128Z Reads: 193

```
Yeah, check your faults. If so, replace that DRV and/or purchase another one :confused:
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-09-05T06:29:26.461Z Reads: 176

```
That's a hard lesson to learn about covering your bullet connectors
```

---
## \#7 Posted by: kyo Posted at: 2016-09-05T06:30:49.522Z Reads: 170

```
Thank for the input, 

So if it say drv fault, then the drv chip is dead , have to replace it. Is there any way to know for sure that the drv is dead and a replacement will do the trick. @torqueboards @Jinra
```

---
## \#8 Posted by: kyo Posted at: 2016-09-05T06:34:17.413Z Reads: 165

```
I know,  ahhhh , I am feeling really bad now. Hope replacing the drv will fix it

Btw even when drv is dead, connection, read, write ,nunchuck connection still work ???
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-09-05T06:58:45.182Z Reads: 163

```
That will have to go to a pro...

Couldn't say
```

---
## \#10 Posted by: kyo Posted at: 2016-09-07T04:41:22.253Z Reads: 142

```
@chaka hi chaka, can you shed some light on this please? Look into my case please

It is possible that even when drv chip is dead, the read, write, nunchuck connecttion still work?
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2016-09-07T04:51:19.151Z Reads: 137

```
Yes, these option are not control by the drv but the mcu...
```

---
## \#12 Posted by: chaka Posted at: 2016-09-07T14:17:57.622Z Reads: 127

```
Looks like a dead drv chip.
```

---
## \#13 Posted by: kyo Posted at: 2016-09-08T01:33:03.044Z Reads: 120

```
Thanks guys @chaka @JohnnyMeduse  i will buy a drv , have old one replaced
```

---
