# Question about battery capacity

### Replies: 18 Views: 272

## \#1 Posted by: Winfly Posted at: 2018-07-12T22:28:54.491Z Reads: 107

```
So I'm mildly confused about how everyone calcuate their battery capacity. Saw someone said that they have a 30q 10s6p or something and they have 18Ah. 

Let's bring it back to the basics. Ampere measures how much electrical charge move through a surface thus it is collums/seconds. And battery are rated in [mAh] = [collums]. 

Let say we only use 30q. 
If u have 1s1p (only 1 cell) you have 3000mAh = 3Ah.
If u have 10s1p ==> 30 Ah.
If u have 10s4p ==> 120Ah.
Am I wrong or are ppl miss labelling their battery.?
```

---
## \#2 Posted by: chuttney1 Posted at: 2018-07-12T22:37:10.627Z Reads: 99

```
[quote="Winfly, post:1, topic:61702"]
Let say we only use 30q.
If u have 1s1p (only 1 cell) you have 3000mAh = 3Ah.
If u have 10s1p ==&gt; 30 Ah.
If u have 10s4p ==&gt; 120Ah.
Am I wrong or are ppl miss labelling their battery.?
[/quote]

Sorry. This is incorrect. In terms of the 30Q, 1P for  is only 3Ah and not 30Ah. 4P is 12Ah, not 120Ah.
```

---
## \#3 Posted by: Blix Posted at: 2018-07-12T22:37:37.570Z Reads: 92

```
A 30q has 3 Ah/3000mAh
3*6 = 18 :P
```

---
## \#4 Posted by: chuttney1 Posted at: 2018-07-12T22:38:30.165Z Reads: 90

```
[quote="Blix, post:3, topic:61702"]
3*6
[/quote]

Half-life 3, part 6 confirmed.
```

---
## \#5 Posted by: RedEagle Posted at: 2018-07-12T22:42:13.649Z Reads: 89

```
[quote="Winfly, post:1, topic:61702"]
miss labelling
[/quote]


*COUGH * airport customs *COUGH *
```

---
## \#6 Posted by: strattos Posted at: 2018-07-12T22:53:17.700Z Reads: 85

```
Voltage has nothing to do when measuring capacity. You only gain extra amp hours for cells in parallel. A 100s1p 30Q battery is still only 3Ah.
```

---
## \#7 Posted by: Sebike Posted at: 2018-07-12T22:57:05.598Z Reads: 82

```
what about a 1000000000s1p battery then???
```

---
## \#8 Posted by: Winfly Posted at: 2018-07-12T23:45:01.843Z Reads: 79

```
Ok it sounds very unintuitive for me. Can someone explain it in college lv physics?
```

---
## \#9 Posted by: rey8801 Posted at: 2018-07-12T23:47:49.417Z Reads: 76

```
parallel adds capacity, series adds Voltage. 30Q battery 3.7V 3000mAh, 2 cells in parallel 3,7V 6000mAh cap. 2 cells in series 7.4V 3000mAh. :wink:
```

---
## \#10 Posted by: Winfly Posted at: 2018-07-13T00:17:04.380Z Reads: 76

```
I mean you just told me how it works. Not why it works this way.
```

---
## \#11 Posted by: deltazeta Posted at: 2018-07-13T00:35:25.587Z Reads: 72

```
Sounds like the confusion is AmpHour(Ah) is not a valid measurement of energy, since it depends on voltage. The closest unit of energy you can convert to from Ah is WattHour(Wh), which you get by multiplying the voltage with the Ah. So when you get series connections, you increase Voltage, which increases Wh, but not Ah. While adding parallel connections you increase Ah but not Voltage. In both cases you do increase overall energy, but only adding parallel connections gets you that conventional Ah number
```

---
## \#12 Posted by: rey8801 Posted at: 2018-07-13T00:36:44.892Z Reads: 70

```
here the physic behind. you only need to see the formulas to understand it. https://en.wikipedia.org/wiki/Series_and_parallel_circuits. There are plenty of explanation online from simple to more complex
```

---
## \#13 Posted by: strattos Posted at: 2018-07-13T01:13:42.651Z Reads: 60

```
Build it and you can tell me :stuck_out_tongue:
```

---
## \#14 Posted by: strattos Posted at: 2018-07-13T01:18:38.744Z Reads: 58

```
In a series circuit, the current through each of the components is the same, and the voltage across the circuit is the sum of the voltages across each component.[1] In a parallel circuit, the voltage across each of the components is the same, and the total current is the sum of the currents through each component.[1]

Your understanding of electricity is a little off. Most of this stuff would be considered college level physics. Though if you want to know the why behind why it functions this way, well that's a whole nother level, and my question for you is why do you need to understand it to that level of detail.
```

---
## \#15 Posted by: Sebike Posted at: 2018-07-13T07:12:41.545Z Reads: 39

```
With two rows of batteries it will be 5,6k miles long though. Have to find a matching longboard.
```

---
## \#16 Posted by: Winfly Posted at: 2018-07-13T07:41:48.313Z Reads: 36

```
Thanks I just got my units wrong.
```

---
## \#17 Posted by: Acido Posted at: 2018-07-13T08:12:41.875Z Reads: 35

```
series connections add voltage not capacity

paralel connections add capacity but not voltage
```

---
## \#18 Posted by: dareno Posted at: 2018-07-13T08:29:24.522Z Reads: 31

```
I thought 30q refers to continuous current discharge rate?  I could be wrong.  Its been known.
```

---
