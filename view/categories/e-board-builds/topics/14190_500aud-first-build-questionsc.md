# $500AUD First Build Questionsc

### Replies: 15 Views: 1180

## \#1 Posted by: Koto Posted at: 2016-12-05T03:02:52.270Z Reads: 86

```
Hi,
I'm trying to make my first board and i have a bit of uncertainty about some things. first, here are my parts

83mm enertion power wheels

Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor

Turnigy 5000mAh 3S 25C Lipo Pack

265-5M-09 Synchronous Timing Belt

15 Teeth X 9mm Belt Width, 5M HTD Type Heavy Duty Timing Pulleys - 9-15-5M-F

36t 9mm enertion drive hub

HobbyKing® ™HK-GT2B 3CH 2.4GHz Transmitter and Receiver w/Rechargable Li-ion Battery

TorqueBoards 120A 6S ESC

TorqueBoards ESC Programming Card

single motor mount

Hobbyking Parallel charging Board for 6 packs 2~6S (HXT4mm)

Nylon XT90 Connectors Male/Female (5 pairs)
 

HobbyKing B6 AC/DC Compact LiPO/NiMh 50W Charger (EU Plug)

TorqueBoards v2 Pro Trucks



I am trying to have tops $500 AUD build.
I am having trouble finding an answer to a few questions:

- if my motor says 10S, and my batteries are 6S, will their be any problems?
- what recommendations do you have for battery & motor?
- do i have any overkill or underkill parts?
- what parallel charging board would fit my connectors
- how do i calculate my battery life?
- how do i calculate top speed?


thank you so much


Oscar
_xxXX KOTO XXxx_
```

---
## \#2 Posted by: saul Posted at: 2016-12-05T03:17:33.308Z Reads: 68

```
use search more. and study build threads there are tons.
http://calc.esk8.it/

your budget will be tight if possible at all especially since shipping to aus is crazy high.
but at least use diy pulley 12mm kit because enertion's requires truck mod.

running your motor at lower voltage is fine. it will just be slower.

if you can I would say up the budget to get a vesc and 9-12s battery because it is worlds better than the 6s esc.
```

---
## \#3 Posted by: Koto Posted at: 2016-12-05T03:18:25.560Z Reads: 65

```
shipping not included when i said 500
```

---
## \#4 Posted by: Koto Posted at: 2016-12-05T03:20:07.009Z Reads: 62

```
thanks Soo much BTW. i am getting way too stressed and someone answering my question is really apreciated
```

---
## \#5 Posted by: saul Posted at: 2016-12-05T03:26:24.249Z Reads: 56

```
no problem. I think the build looks fine. but like I said a vesc and higher voltage make a huge difference in feel and reliability. 

my ride is
vesc
8s 10ah lipo
single 6354 190kv
mini rc remote
jet spud 29"
14/36 gearing
97mm flywheel clones

I get 22mph top speed and about 10-14 miles. But i can go up almost any hill.
re-gearing to 16/36 will get me 26+.
```

---
## \#6 Posted by: Koto Posted at: 2016-12-05T03:39:30.075Z Reads: 56

```
Strange- calculator says 55km/h when weighted at 80% efficientcy,. btw, made  a new thread with a whole lot more newb questions. no pressure, u have allready done a lot for me 
thanks
```

---
## \#7 Posted by: Koto Posted at: 2016-12-05T04:04:54.408Z Reads: 49

```
[quote="saul, post:5, topic:14190"]
re-gearing to 16/36
[/quote]

that is because it creates a higher reduction ratio right?
```

---
## \#8 Posted by: saul Posted at: 2016-12-05T04:08:55.484Z Reads: 48

```
no problem. i'm working on a wiki to help avoid these types of questions so its good to see what people are confused on...
for the calc i think you left the battery at 10s?

16/36 is actually a lower gearing ratio.

1:  36/16 = 2.25
2:  36/14 = 2.57
i guess writing them backwards doesn't help lol.

so 1 would have higher top speed. 2 would have more torque(acceleration).
```

---
## \#9 Posted by: Koto Posted at: 2016-12-05T04:12:36.048Z Reads: 45

```
[quote="saul, post:8, topic:14190"]
1 would have higher top speed. 2 would have more torque(acceleration).
[/quote]

which one means longer battery time
```

---
## \#10 Posted by: Koto Posted at: 2016-12-05T04:15:03.019Z Reads: 41

```
oh, and what is efficiency and erpm
```

---
## \#11 Posted by: saul Posted at: 2016-12-05T04:24:37.636Z Reads: 46

```
range depends on many factors. gearing will only change this by a bit.
it really comes down to how/where you ride. the faster you go the less range. the more hills less range. heavy rider less range. opposites of these give more range.

[quote="Koto, post:10, topic:14190"]
what is efficiency and erpm
[/quote]

efficiency - the ratio of the useful work performed by a machine or in a process to the total energy expended or heat taken in.
in english, something like mpg for a car. more efficiency means more range with the same amount of energy.

erpm is the rate the esc is switching the motor phases.
similar to kv of motor. where kv = rpm per volt. but since bldc motors that we use have 14 poles in pairs we multiply kv by 7.

so erpm = kv * 7 * voltage
voltage = 4.2(full charge li ion/lipo) * 6(s in your case).

erpm is really only important with vesc because there is a 60,000 erpm limit. above this causes problems.
**this is why as voltage goes up we use lower kv motors.**
```

---
## \#12 Posted by: Koto Posted at: 2016-12-05T04:27:44.155Z Reads: 41

```
btw i am now probs changing to 5S and maybe vesc
```

---
## \#13 Posted by: Koto Posted at: 2016-12-05T04:28:33.488Z Reads: 43

```
http://www.electric-skateboard.builders/t/wiring-charging-and-a-whole-lot-of-newb-questions/14194
```

---
## \#14 Posted by: Koto Posted at: 2016-12-05T21:24:34.680Z Reads: 33

```
[quote="saul, post:11, topic:14190"]
this is why as voltage goes up we use lower kv motors.
[/quote]

May be a problem- says 63455 erpm, what do i do/?
```

---
## \#15 Posted by: Koto Posted at: 2016-12-06T02:02:56.172Z Reads: 29

```
[quote="saul, post:11, topic:14190"]
60,000 erpm limit
[/quote]

so less kv motors
```

---
