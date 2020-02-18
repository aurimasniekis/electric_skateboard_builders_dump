# Battery noob, need help filling out a sheet

### Replies: 23 Views: 1245

## \#1 Posted by: Airmacx Posted at: 2016-09-17T16:18:51.105Z Reads: 144

```
Since I can't build a pack myself, no tools and lack of knowledge, and trust in myself, I decided to get it done professionally. I have 40 Samsung 25R 18650 batteries, and plan on configuring it to 10s4p. The guys building it require me to fill out a sheet with some info (which I will attach). Problem is, because I'm totally clueless about the whole battery thing, I need help filling out the stuff like the voltage stuff, discharge, min and max temperature etc. Obviously, it'll be li-ion so I got that, but the rest is what I don't really know.I guess charging time doesn't really matter but ideally, something under 2 or 3 hours. I'm not sure if it's possible but 1hr would be a dream. Anyways, I hope you guys can help me out! Please let me know if there's any important info that I need to tell the guys about this pack, so that it works fine with my board. Will be powering an R-SPEC 6373 motor, and of course I'll be using a VESC (Enertion). 


**THE FORM THAT NEEDS FILLING**

<img src="/uploads/db1493/original/3X/2/b/2b5d90570c2960fa65a3c904e2a0c88ccf922549.png" width="690" height="232">

Edit: as for size, I think I can probably answer that myself, as I have a Mastercho enclosure, which according to the esk8 market site, is 23 “x 8.5” x 1.1 “in size.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-09-17T16:56:08.367Z Reads: 135

```
<img src="/uploads/db1493/original/3X/e/f/efe471dfe4883dd747fcb180979ec90b79ede297.png" width="690" height="232">

Raw version, i think the values are correct, maybe someone else can review them

V2:
<img src="/uploads/db1493/original/3X/9/0/90f84186c1885c96cffbe8f2829ac07c13c831f5.png" width="690" height="232">
```

---
## \#3 Posted by: Airmacx Posted at: 2016-09-17T16:58:09.728Z Reads: 129

```
Thank you my friend. I will wait for a few more responses just to double check, but thanks so much!
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-09-17T17:24:21.945Z Reads: 123

```
I agree with @flatsp0t except for the connector, I would just go with regular XT90, since I have experience with the anti-spark blowing up... If you want to use anti-spark I would get a separate anti-spark, or make a loop key, since those are much easier to replace if they break.
```

---
## \#5 Posted by: flatsp0t Posted at: 2016-09-17T17:35:49.558Z Reads: 118

```
the only context i ever heard of them breaking was in loop key applications, so i thought it would be ok, but maybe you are right.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-09-17T17:37:22.987Z Reads: 115

```
The continuous amperage is too low. 
25/80
Those batteries in a 4p configuration should in theory handle 100a continuous 
If you tell them 25, you will get a 25a BMS. 
Tell them just 80a continuous and forget the peak 
Then they should do an 80a BMS
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-09-17T17:41:20.984Z Reads: 107

```
Well, i did not think about them selecting the BMS, but seems pretty obvious now :slight_smile:

I edited my post
```

---
## \#8 Posted by: michaeld33 Posted at: 2016-09-17T17:42:48.424Z Reads: 105

```
IDK, I'd rather have a broken loop key than a broken battery connector, I can make another loop key easy, taking the board apart, cutting the wires, re soldering the connector... harder
```

---
## \#9 Posted by: Namasaki Posted at: 2016-09-17T21:41:33.588Z Reads: 85

```
I think a Loop Key is a great idea for an inexpensive anti-spark solution that can be accessed from outside the enclosure.
```

---
## \#10 Posted by: Jinra Posted at: 2016-09-18T03:01:37.697Z Reads: 79

```
25r's actually so 20 continuous, but yea 80a continuous is what they can technically handle. However you want to be away from 80a continuous due to the heat it can produce on your batteries.
```

---
## \#11 Posted by: Pantologist Posted at: 2016-09-18T04:45:45.122Z Reads: 67

```
Just curious where you are getting this done? Also what price are they charging you?

The specs are right as far as I can tell for flat's V2 version.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-09-18T04:59:19.445Z Reads: 63

```
My mistake, I thought they where rated for 25a
```

---
## \#13 Posted by: Airmacx Posted at: 2016-09-19T23:31:31.999Z Reads: 60

```
I just got a reply and he had concerns about the BMS. 


>The issue comes with the need to find an 80A BMS, we don’t stock one. We have a 10S 20A continuous with 90A±10A trip in our range. 

>I can enquire about a 25A and 100A one of our suppliers has. I can’t see you using more than 20A continuous though, most legal electric bikes only draw about 7A continuous. I had an electric cargo bike that I set up for 15A continuous output, that bike alone was often over 50kg with gear on it, add a rider and you are around 125kg. A board and rider would not get anywhere near this weight or wind drag when moving.
 

What do you guys think? Should I settle for 20A? If not where's best place to get an 80A BMS?

But as I recall, @Namasaki said even 25A is too low.

Edit: looking at other builds with 10s4p, such as @longhairedboy they don't always have 80A, a bit smaller though like 60A. Not sure if it's as viable but I'm open to different options. I live E I'm Australia by the way, so if anyone finds one,  it needs to be shipped here.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-09-19T23:44:52.314Z Reads: 55

```
20a is too low. 60a would work.
```

---
## \#15 Posted by: barajabali Posted at: 2016-09-19T23:52:44.147Z Reads: 53

```
@Airmacx

I can handle this for you if you need? Us only
```

---
## \#16 Posted by: Airmacx Posted at: 2016-09-19T23:58:41.177Z Reads: 53

```
Yeah, that would be a dream, but I live in Australia. I have found this though. 

http://www.batterysupports.com/36v-37v-42v-10s-80a-10x-36v-lithium-ion-lipolymer-battery-bms-p-389.html

Is this a good fit for my pack?  I'm going for 10s4p as you recommend.


The guy I'm in talks with just got back, he can get 100A, but I'm not sure if it's overkill and too much. Thoughts?
```

---
## \#17 Posted by: barajabali Posted at: 2016-09-20T00:57:17.043Z Reads: 47

```
Yes! That's a fine bms. You can get away with 60amp too
```

---
## \#18 Posted by: Jinra Posted at: 2016-09-20T01:01:00.163Z Reads: 48

```
You can also tell them to bypass bms and add a fuse
```

---
## \#19 Posted by: Airmacx Posted at: 2016-09-20T01:05:11.200Z Reads: 49

```
What about 100A?
```

---
## \#20 Posted by: barajabali Posted at: 2016-09-20T01:31:48.393Z Reads: 52

```
100 is fine too but you'll never pull that many.
```

---
## \#21 Posted by: Airmacx Posted at: 2016-09-20T01:33:31.805Z Reads: 46

```
Okay. He says 100 is overkill, but so is 80A. What is the reason for 80 or 60,or even anything above 20 for that matter?  @Jinra you mentioned that I should stay away from 80A even though it can handle it, what would you say then 60?
```

---
## \#22 Posted by: Jinra Posted at: 2016-09-20T02:12:05.058Z Reads: 41

```
80a burst is fine, you should probably aim for a 60a bms
```

---
## \#23 Posted by: longhairedboy Posted at: 2016-09-20T16:40:02.517Z Reads: 37

```
yup. 60amp is plenty.
```

---
