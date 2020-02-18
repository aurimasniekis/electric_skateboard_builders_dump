# Help me understand BMS balance wiring options. Positive, Negative or Middle?

### Replies: 18 Views: 610

## \#1 Posted by: lrdesigns Posted at: 2018-10-23T03:23:16.999Z Reads: 101

```
Hi guys, I am really confused about the different way people wire up the balance wires on a BMS. I have seen people wire them to the negative of the p-group, the positive of the p-group and between p-groups. It leaves me with so many questions. 

1. In my logic there would be only one way to wire a BMS, can any BMS be really wired in one of these 3 ways? 
2. Is one method better than another from a cell life point of view or a safety point of view?
3. I did three (4S-4P) example layouts below, is that the correct wiring for each method? Charge only layout.

I came to e-sk8 from RC hobby and have only used balance chargers so far. 

![image|690x245](upload://rbXQujWXRlvwnTwHYWonLDA91Pt.png) 

![image|690x255](upload://aOAPcytcvt9HfdfyhgPEUIl5vOu.png) 

![image|690x247](upload://kb1ahHtBlqvf06pUNFF0QklXNM6.png)
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-10-23T03:27:32.086Z Reads: 96

```
Ya lots of ways to wire depending on bms. I've always just copied other people's projects and followed them as closely as possible. Downside is image are misleading sometimes and can look backwards. It makes sense to me that you can use a multimeter and add your voltsges up of balance wires. But ya other aspects I completely don't understand 🤣 Iove these posts though! Do you @b264? 😃
```

---
## \#3 Posted by: jmasta Posted at: 2018-10-23T03:29:50.667Z Reads: 91

```
Depends on the BMS.... but those all look wrong to me
```

---
## \#4 Posted by: b264 Posted at: 2018-10-23T03:39:46.509Z Reads: 88

```
A, B, and C all look wrong; the way to wire them would depend on the specific BMS, and A might be correct for some BMS but probably not for a majority of them.
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2018-10-23T03:41:48.126Z Reads: 83

```
If you were given a bms with no diagram could it be possible to work it out using common sense? Or is this just a horrible question 🤣🤣
```

---
## \#6 Posted by: b264 Posted at: 2018-10-23T03:47:54.337Z Reads: 81

```
It's likely to be possible but not guaranteed
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2018-10-23T03:51:45.616Z Reads: 85

```
Ok. This is a relief I feel like I've seen only 2 styles so far. I took bout 50 pictures 🤓 would be cool to identify them all without major thread digging. Hopefully that doesn't sound 2 lazy 😃
```

---
## \#8 Posted by: TowerCrisis Posted at: 2018-10-23T03:56:52.565Z Reads: 83

```
General rule of thumb, they connect to the positive terminals of the cells. Typically start from the main battery + and work your way down.

If a 12S BMS has 13 pins, then they connect to all the positive terminals plus the initial negative.

If a 12S BMS has 12 pins, then it only connects to the positive terminals.

Milage may vary, reference the provided disgram with the BMS.
```

---
## \#9 Posted by: dareno Posted at: 2018-10-24T04:15:45.792Z Reads: 62

```
@TinnieSinker
Mate can you have a look at this and give your opinion please because the replies have me a little messed up.  Thanks pal.
```

---
## \#10 Posted by: lrdesigns Posted at: 2018-10-24T04:35:02.482Z Reads: 60

```
To the comments that all the diagrams are wrong. The **Ref**erence wire I have obviously goes where your BMS tells you to put it as this can be routed different depending on the particular BMS.

![image|175x133](upload://ziO1Xwi1Dr569u8NOjkClgwI6RD.png) 

The point was about which is the **best** way to hook up the balance wires.  If the answer is just follow your BMS diagram, well ok but thats is so dull.
```

---
## \#11 Posted by: TinnieSinker Posted at: 2018-10-24T06:53:23.086Z Reads: 56

```
yea all 3 are incorrect. 

ref is most likely the same as main negative wire, which could be called 0. balance wire 1 is the first positive after 0, so the last/ highest number is the same as the main positive wire.

so ref is correct in C 
balance wires are correct in B

generally there's only two ways to wire. charge only and both charge and discharge. varying slightly with brands.

for charge only setup, you want a small(20awg) black wire to go to the b- on the bms and then from the c- (or p- if there is no c-) to the charge plug. 
this is separate to the main black wire, but connected to the same spot on the battery.

hopefully that makes sense, i'll try find some pics
```

---
## \#12 Posted by: TinnieSinker Posted at: 2018-10-24T07:19:25.684Z Reads: 51

```
i haven't taken any good pics so i re did your diagram. it may or may not make sense

![4bcdd7af55e00ae176a24c351b545877670f215e|690x255](upload://gRA5o6PTzhIy9nlISqNSw3A3kmj.jpeg)
```

---
## \#13 Posted by: lrdesigns Posted at: 2018-10-24T07:21:18.714Z Reads: 52

```
[quote="TinnieSinker, post:11, topic:72041"]
so ref is correct in C
balance wires are correct in B
[/quote]

@TinnieSinker ok thanks. So this (dia D) should be right then?

![image|690x264](upload://bXYgm3CaPMMMPTgANeDh2rCB9s5.png) 

What's the difference or advantage of going to the middle of the p-group? (dia E)

![image|690x245](upload://7vKYOvCHpYEF0U0hHY6muAzSr4Z.png)
```

---
## \#14 Posted by: Andy87 Posted at: 2018-10-24T07:22:21.853Z Reads: 50

```
like my bestech d140. 
13pins on the pcb but on the diagram they sent with the bms only 12 used.
the first balance b- is need to be left out.
```

---
## \#15 Posted by: TinnieSinker Posted at: 2018-10-24T07:26:06.016Z Reads: 50

```
[quote="lrdesigns, post:13, topic:72041"]
advantage of going to the middle of the p-group
[/quote]

it makes no difference. just comes down to convenience of where you want the wire placed
```

---
## \#16 Posted by: Andy87 Posted at: 2018-10-24T07:27:40.839Z Reads: 49

```
nothing, the potential is the same. you could also solder it on the - terminal of that serial connection. which would be even more save as you don´t need to add solder on the positve cell terminal with the opening holes.
```

---
## \#17 Posted by: dareno Posted at: 2018-10-24T09:14:28.776Z Reads: 46

```
Sorry to tag you mate if you're busy but batteries are kind of important.  You my friend know your shit.
```

---
## \#18 Posted by: TinnieSinker Posted at: 2018-10-24T11:22:26.047Z Reads: 42

```
all g, there's always time for ridgy didge diagrams haha
```

---
