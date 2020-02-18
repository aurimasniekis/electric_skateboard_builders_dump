# Setup two vanda vesc&rsquo;s

### Replies: 11 Views: 327

## \#1 Posted by: chickengun Posted at: 2019-04-20T14:45:28.786Z Reads: 66

```
I am trying to setup my two vanda vesc's HW 4.12 for my first build.
Using the newest vesc tool (version 1.08) I flashed the newest firmware 3.54 on both of the vesc's.
Since I want to setup a dual hub motor in BLDC mode I had to go to "Wizards -> Setup Other Motors". I set the Amp limit to 15 A / -7.5 A. The motor was recognized and also spinning. I applied the changes and did the same for the other motor. So far so good.

I have both motors connected over CANH/CANL and when I go to "Setup Input" the following message pops up:

![image|517x254](upload://5Mu8UzwjdNVq75Zo8GZ2RXMyyKg.png) 

I don't understand this, both are at Firmware 3.52...

As a workaround: I noticed that I don't get this message when I disconnect the receiver (Firefly receiver) shortly from the board. This way the setup continues:

![image|519x324](upload://fkkZI3qusFhewRAbjcavrh4xxYP.png) 

I calibrated the firefly remote and pressed Finish.

The problem now is that I can only spin one motor. When I swich master/slave the other motor spins only. By the way the receiver is connected over PPM.

Next I used the vesc tool v0.95 and flashed firmware 3.40 on both vesc's. After the motor/input setup I was able to spin both motors but in the opposite direction. After switching two phase wires on one of the motors I was only able to spin one of them. Strange.

Does anyone have an idea what I can do to make the motors work? Any help is appreciated.
```

---
## \#2 Posted by: Grozniy Posted at: 2019-04-20T14:57:45.647Z Reads: 59

```
https://www.electric-skateboard.builders/t/wiki-a-beginner-guide-to-diy-an-esk8/46844/16?u=grozniy
Maybe this helps
```

---
## \#3 Posted by: chickengun Posted at: 2019-04-20T14:59:29.979Z Reads: 53

```
I saw that video. There is a more recent version of the vesc tool (1.08) but it's similar and not describing my problem.
```

---
## \#4 Posted by: Andy87 Posted at: 2019-04-20T15:16:02.248Z Reads: 45

```
[quote="chickengun, post:1, topic:91234"]
After switching two phase wires on one of the motors I was only able to spin one of them.
[/quote]

You need to do motor detection again after swapping phase wires. Instead of phase wire swapping you could only apply invert motor direction in the vesc settings. This wouldn’t need a new motor detection.
```

---
## \#5 Posted by: chickengun Posted at: 2019-04-20T15:25:14.500Z Reads: 39

```
Thanks a lot, I forgot that. When I use Firmware 3.40 it works now. But it still doesn't work with 3.54. Is that normal?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-04-20T15:29:09.543Z Reads: 37

```
I have no experience with the new FW, can’t tell you.
```

---
## \#7 Posted by: Kingdom421 Posted at: 2019-04-20T15:40:15.417Z Reads: 36

```
I have the same setup but I have not experienced this with my vanda's but I also set each vesc separate set one as slave and connected by self made canbus. Maybe this week I can reconnect and see if I can simulate the same problem you are having. Why is the amp limited so low
```

---
## \#8 Posted by: chickengun Posted at: 2019-04-20T15:42:51.252Z Reads: 33

```
it was just a first quick test. I am using a 10s4p battery pack over a HCX-D223V1 bestech bms. I thought 15 A per motor should be ok to not let it run too hot. What are your Amp settings?
```

---
## \#9 Posted by: Kingdom421 Posted at: 2019-04-20T15:48:31.012Z Reads: 29

```
30 and -10 but I'm not home till Monday though to double check. I'm also running a 10s4p. 4 separate BMS
```

---
## \#10 Posted by: chickengun Posted at: 2019-04-20T16:16:11.924Z Reads: 28

```
Do you have the newest firmware 3.54 running?
```

---
## \#11 Posted by: Kingdom421 Posted at: 2019-04-20T16:18:55.673Z Reads: 27

```
Yes it was the first thing I did
```

---
