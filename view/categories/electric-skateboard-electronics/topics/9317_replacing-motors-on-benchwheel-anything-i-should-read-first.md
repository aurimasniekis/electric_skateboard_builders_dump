# Replacing motors on benchwheel - Anything i should read first?

### Replies: 25 Views: 2909

## \#1 Posted by: philippeb Posted at: 2016-09-10T07:57:38.728Z Reads: 147

```
i where a little confused if i should post this on prebuilt sub or this one, but since it is going to become a custom build i thought this where the right place to ask.

Anyways, my benchwheel broke after only 5 days of use, so i decided to take it apart and replace the broken motor.

i was thinking that my battery, esc and rest of current setup should be able to support a new engine around 1800-2000w 200kv (Less than 50mm).
But i actually never have done anything like this before so i was hoping to get some headsup before i mess up.

I am only going to replace the right engine at first, see how well it goes, and if evrything goes fine i will do a remake later.

Please give me any headsup i should take note of before i get going :slight_smile:
Thanks
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-10T09:01:06.189Z Reads: 138

```
the motors are 280kv 5065 motors. Just make sure you get a motor with the correct hole pattern
```

---
## \#3 Posted by: philippeb Posted at: 2016-09-10T09:50:47.293Z Reads: 137

```
Wow. Thanks.
How do i know about the holes ?
I mean, 5065 means 50mm in diameter and 65mm length right ? 
And how did you know about the kv ?

I assume holes follow a standard pattern depending  on diameter and mabey length ?
```

---
## \#4 Posted by: Jinra Posted at: 2016-09-10T10:37:05.321Z Reads: 129

```
Yea different motors may have different distances for their mounting holes, just make sure the replacement is the same. I know about the kv from benchwheel themselves.
```

---
## \#5 Posted by: philippeb Posted at: 2016-09-10T15:42:48.597Z Reads: 125

```
cool.thanks. a lot
```

---
## \#6 Posted by: leven Posted at: 2016-09-11T18:50:04.258Z Reads: 106

```
Benchwheel actually says 270Kv for motors for the dual.
Look at motorsection here:

https://wholesaler.alibaba.com/product-detail/Custom-high-speed-3600W-boosted-board_60521938664.html?spm=a2700.7724838.0.0.1pooNa
```

---
## \#7 Posted by: philippeb Posted at: 2016-09-29T12:35:34.834Z Reads: 92

```
Okay thanks.
Update on the Benchwheel.
The 1 motor is causing so much trouble now.
Damn, i strongly advice NOBODY to spend 600-700 USD on this piece of shit.

I havent even had it for 1 month.

Anyways.

Replacing the engine/motor should hust be a plug and play kinda thing ?
I dont need to setup the voltage or anything in the esc right ?
```

---
## \#8 Posted by: philippeb Posted at: 2016-09-29T12:55:15.853Z Reads: 82

```
Besides.
There is somthing i dont quite get.

How come i see serval single motor setup going 20mph with somthing like
1600W / 270 KV motors

While this board with 2x 1800 270 kv engines barely go 15MPH ?

Should i assume the promised engine spec's are fakes ?

I was considering going with this engine

http://www.hobbyking.com/hobbyking/store/__18175__turnigy_aerodrive_sk3_5055_280kv_brushless_outrunner_motor.html

Since i cant find anything "Stronger", but it seems to be weaker on the paper than my current one.
But if anyone in here got some inputs feel free to share :)
```

---
## \#9 Posted by: petivel Posted at: 2016-10-16T11:48:06.549Z Reads: 73

```
[quote="philippeb, post:8, topic:9317"]
e got some inputs feel free to share
[/quote]

same motorfault issue here, keep me posted.
```

---
## \#10 Posted by: leven Posted at: 2016-10-16T22:07:26.839Z Reads: 70

```
It has to do with several things.

A 270kv motor is not that strong, a 200kv motor is a lot stronger.
But a 270kv motor spins faster at the same voltage, but with less force, so to get the board to go uphill etc, they designed it to be less fast.

1, It has a 6s battery, faster boards usually have 10 or 12s, a lot more voltage to the motors.
2, 16>46 gears, most diy-boards have 15/16>36teeth on the gears, aka faster.
3, not verified not i think its electronally limited, i remeber reading something about max 17Mph is the law in china for these.

So try to find a motor that is around 270 like the original.
```

---
## \#11 Posted by: petivel Posted at: 2016-10-17T05:32:53.941Z Reads: 69

```
http://www.hobbyking.com/hobbyking/store/__35387__Turnigy_Aerodrive_SK3_5065_320kv_Brushless_Outrunner_Motor_EU_Warehouse_.html
I am thinking buying 320kv turnigy, is that compatible? wont be burned of the heavy load? 8kg+80kg

(this would be 2nd motor on it, next to the original275kv)
```

---
## \#12 Posted by: irexjr Posted at: 2016-10-17T07:25:29.617Z Reads: 69

```
Be careful you don't strip the grub screws. They're thread locked. I broke two allen keys trying to unmount one of the motor mounts. Now it's stripped and I can't get my second motor off.

http://www.electric-skateboard.builders/t/completed-benchwheel-rebuild-hobbyking-150a-fs-gt2b-6s-lipo-cut-deck/10465/1
```

---
## \#13 Posted by: irexjr Posted at: 2016-10-17T07:29:20.629Z Reads: 63

```
The motors are 270kv. But it seems slower because the gear ratio of the pulleys are built for torque, I think it's 12 to 46 or something when I counted. Most builds are like 10-15 to 30-35 on this forum.
```

---
## \#15 Posted by: petivel Posted at: 2016-10-27T05:05:56.312Z Reads: 57

```
I counted 16x48 holes
```

---
## \#16 Posted by: philippeb Posted at: 2017-05-18T15:59:46.284Z Reads: 43

```
So, things took a step back due to work and such.
But i have allmost collected all the stuff i need for this replacement.

Only thing i need to know.

When i look at the motor i found, it has a 8mm shaft.
Is that equivalent to the pulley with "8mm bore" ?
```

---
## \#17 Posted by: Jinra Posted at: 2017-05-18T16:00:27.642Z Reads: 42

```
yep
10 chars
```

---
## \#18 Posted by: thisguyhere Posted at: 2017-05-18T16:36:07.622Z Reads: 43

```
just letting you know, you're in the EXACT same boat as i was.  got a benchwheel, thought i was hot stuff, then it broke after about a month.  had the grand plan to selectively replace parts to save money.

what wound up happening is i just build a brand new board from scratch after trying for a while.

for one, the battery pack on the benchwheel is 6s4p.  you're going to want more power very quickly.

the esc and bms are kind of part of the same pcb.  found out on my the esc was malfunctioning, in addition to the motor burning out, but couldn't do anything about it since everything's bespoke and integrated.

anyway, wish you best of luck on repairing, i'm curious to see how it goes.
```

---
## \#19 Posted by: philippeb Posted at: 2017-05-18T16:44:39.746Z Reads: 42

```
woa.
Thanks for letting me know.
I kinda think i need to replace it all in time.
But atm i have my car and i use it for my daily travel, the board is only for 1 year ahead when i need to go back to uni and study, but for now i think i will start with a motor and see whats the next thing.

How did you figure out the esc was malfunctioning ?
```

---
## \#20 Posted by: thisguyhere Posted at: 2017-05-18T16:52:01.776Z Reads: 41

```
Connected another, good motor to it and one side wasnt working.
```

---
## \#21 Posted by: philippeb Posted at: 2017-05-18T17:02:28.159Z Reads: 40

```
that could actually maybe explain why the one motor faulted ?
I mean, its kinda stuck.
as if the motor messed up in the magnetic field.

It dosent feel like somthing is stuck inside the motor, more like it has jammed by itself.

could be i should look into creating my own setup.
```

---
## \#22 Posted by: thisguyhere Posted at: 2017-05-18T17:14:58.120Z Reads: 41

```
like you said, you'll probably end up replacing everything on this board.  even if that happens, what will you be left with?

i think the sunk cost fallacy is in full effect here.  i know it's hard to say good bye to $650, but let's say you spend another...$300 to replace the broken bits.  you're now $900 in.  once fixed, how long until something else stops working?  are you going to replace the whole pcb if either the esc, remote controller, or bms blows out?  how much is that going to be?

the only bad thing is, it's going to be somewhat difficult to reuse the parts off the benchwheel if you do a new build.

the aluminum enclosure on the benchwheel, while it's nice, is not practical for a larger battery.  you may be able to reuse the truck / mount / pulley / wheels combination.

anyway, i'm on the side of ditching the whole thing and going diy 100%.
```

---
## \#23 Posted by: philippeb Posted at: 2017-05-18T17:24:12.361Z Reads: 41

```
[quote="thisguyhere, post:22, topic:9317"]
only bad thing is, it's going to be somewhat difficult to reuse the parts off the benchwheel if you do a new build.
[/quote]

im gonna be a total dick-ahole combination on you.
I filled a claim against the seller on paypal and got all my money back while keeping the board because seller dident follow the rules of returns.
So i am actually just playing around with this thing, its 100% free for me to break or fuck up.

But yes, i totally get you, actually am i right now looking at some mount kits and so on, guess i will be needing a new setup and just ride this garbage with the one motor left until it faults too :P
```

---
## \#24 Posted by: thisguyhere Posted at: 2017-05-18T17:31:13.659Z Reads: 39

```
Aww fregging sweet, good on you. 

Yea then no emotional attachment, definitely go for a new build. 

To start, hit up @yummyblobs for focbox (vesc-x) and motors, @Shogu12 for mounts, @Titoxd10001 for pulleys if he's still got some. Theyve got great prices
```

---
## \#25 Posted by: yummyblobs Posted at: 2017-05-18T18:02:41.233Z Reads: 40

```
I had a benchwheel too, only thing salvageable is the drive unit. I built a 8s4p dual build with the old benchwheel stuff and it worked out pretty good, it would be my prefered board if it wasnt so slow at 22mph top speed. At 8s you need to limit the erpm but the dual drive unit has surprising torque!

Those Samsung betteries are also pretty much junk, not worth it to to use for esk8, you can use it for other projects though. I recommend Sammy 30q's.
```

---
## \#26 Posted by: mikel Posted at: 2018-05-30T05:44:17.839Z Reads: 18

```
newbie here... my benchwheel motor gets stuck and once you touch it-- it zoooms. is it the electricals or jst the motor

video here at 7:25

https://youtu.be/9KtVQe3nzoA?t=7m26s
```

---
