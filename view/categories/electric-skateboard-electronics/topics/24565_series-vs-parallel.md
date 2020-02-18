# Series vs parallel!

### Replies: 18 Views: 2091

## \#1 Posted by: NewbieBoardBuilder Posted at: 2017-06-04T20:11:03.624Z Reads: 206

```
I know there are many threads already out there, but I just want to clarify the differences... Can someone explain the wiring differences between the two, and how they effect range and speed...thank you so much!
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-04T20:22:47.992Z Reads: 203

```
When batteries are in series you double the voltage but range stays the same. When you put them in parallel you double the mAh/range but the voltage stays the same.
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2017-06-04T20:24:47.180Z Reads: 199

```
What is more common and why?
```

---
## \#4 Posted by: Smorto Posted at: 2017-06-04T20:29:16.811Z Reads: 193

```
There really isn't a set one about which is better. If you give us some specs about which batteries you are using we can help you decide. To put it simply, parallel will increase range but not speed, and series will increase speed but not range. To get more specific like what @JLabs was saying, when you put two batteries in series, the voltage doubles, but the Mah stays the same. When you put two batters in parallel, the Mah and C rating of the pack double but the voltage stays the same. Which one you should use depends on you batteries, your ESC, and what you want out of the board.
```

---
## \#5 Posted by: NickTheDude Posted at: 2017-06-04T20:37:58.935Z Reads: 178

```
Thats not true. When you wire in series range is doubled as well.

You have 4 things to be concerned with:

Capacity (Ah amp hours)
Discharge (A amps)
Voltage (V volts)
Range (Wh watt hours)

Voltage is doubled when wired in series, and discharge and capacity are double when wired in parallel.

Wh = V * Ah

Therefor range will double regardless of how you wire your batteries. Lets say you have 2 batteries that were 10V, 10A and 10Ah.

Wired in series the battery would have 20V, 10A and 10Ah, wired in parallel the battery would have 10V, 20A and 20Ah.

20V * 10Ah = 200Wh
10V * 20Ah = 200Wh

Either way the watt hours are equivalent.
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2017-06-04T23:29:39.179Z Reads: 158

```
@NickTheDude has the right answer here.  neither magically doubles your range.  However, generally people on this forum prefer to use series (higher voltage) because (i think?) it's more efficient for most of the hardware we use.
```

---
## \#7 Posted by: pennyboard Posted at: 2017-06-04T23:39:20.538Z Reads: 152

```
Yes, I am under the impression that the reason it is more efficient has to do with top speed. 

Take this example scenario: 
I like to run my board at 20mph. If I use 6s batteries, I have to use a small gear reduction in order to achieve that top speed than if I used 12s batteries. This smaller gear reduction means less torque, so to achieve the same acceleration, I have to pull more amps to the motor, draining the battery faster. 

Thus if I was to ride exactly the same with 6s and 12s, 12s would, in general, get me more range because I would have the advantage of more low end torque, while still maintaining my desired top end speed courtesy of the higher voltage.
```

---
## \#8 Posted by: MoeStooge Posted at: 2017-06-04T23:58:14.480Z Reads: 142

```
General rule is, 200lb man take 2.1hp to travel 22mph. 2.1 HP =1564watt. 1564watt=106A@14.8v. double the volts 29.6  200lb man still take 2.1hp to travel 22mph 2.1hp=1564watt. now check this out 1564watt= 53amp@29.6v  hey now chucky can run smaller gage wire, doesn't need a 120a esc, or high discharge rate batteries,  exct.  Increase volts lowers amps at same performance.
```

---
## \#9 Posted by: NewbieBoardBuilder Posted at: 2017-07-01T21:37:15.769Z Reads: 114

```
[quote="Smorto, post:4, topic:24565"]
If you give us some specs about which batteries you are using we can help you decide.
[/quote]

This is really what I need help deciding..
```

---
## \#10 Posted by: NewbieBoardBuilder Posted at: 2017-07-01T21:38:23.102Z Reads: 110

```
I'm super lost on what to buy...I think I'm doing 12 cells, 190kv mono motor at 13:36 gearing
```

---
## \#11 Posted by: Smorto Posted at: 2017-07-02T03:08:36.682Z Reads: 107

```
I would recommend a 15/36 or 16/36 gearing so your belt doesn't slip. It will also give you more speed.
```

---
## \#12 Posted by: NewbieBoardBuilder Posted at: 2017-07-03T13:56:27.337Z Reads: 94

```
What if I'm running 12S battery with a 190kv motor, won't that already have enough speed?
```

---
## \#13 Posted by: Smorto Posted at: 2017-07-04T00:14:59.426Z Reads: 86

```
Yes but a 13 tooth motor pulley will most likely slip so I recommend a higher tooth motor pulley.
```

---
## \#14 Posted by: Idle Posted at: 2017-11-19T20:29:23.601Z Reads: 68

```
[quote="JLabs, post:2, topic:24565"]
When batteries are in series you double the voltage but range stays the same.
[/quote]


This, for a guy like me was hard to understand. 
I just didn't get it. 
Everywhere I'd looked or read said this same exact thing.


That capacity, ie: range doesn't increase when connecting cells in series, only in parallel.

Was it poor reading comprehension or am I just dumb? idk...

Either way, I feel a little smarter now knowing that 2+2 is indeed 4 as I suspected all along👻! 

Thanks @NickTheDude for breaking it down.
```

---
## \#15 Posted by: Greenie Posted at: 2017-11-19T21:38:10.230Z Reads: 51

```
What about batteries that are classified as 2s2p for example. If I get 3 of them, I get 6s6p? What would that mean?
```

---
## \#16 Posted by: pat.speed Posted at: 2017-11-19T21:42:22.386Z Reads: 48

```
Yes, technically but if you have a 5000mah 2s2p the two cells in parallel will only have 2500mah each so then when you put it together you will get 15000mah. Simply you can just times the total mah of the battery by three because there is three batteries. So 5000mah x 3 equals 1500mah
```

---
## \#17 Posted by: Greenie Posted at: 2017-11-19T22:08:39.483Z Reads: 47

```
Is it a good configuration to make? I want this range. So I understand the whole series vs parallel thing but didn't understand what it means when the battery says both. I was looking to get 3 6000 mah 2s2p
```

---
## \#18 Posted by: pat.speed Posted at: 2017-11-19T22:12:49.300Z Reads: 45

```
It just means there are two batteries in series so 7.4v and 2 3000mah batteries in parallel so 6000mah. Yes it is perfectly fine and you will get plenty of range.
```

---
