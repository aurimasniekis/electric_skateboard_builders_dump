# Possible overload on the BMS?

### Replies: 11 Views: 682

## \#1 Posted by: Aggdaddy Posted at: 2017-07-07T15:29:41.072Z Reads: 75

```
I have a 10s lipo battery (MTB configuration) created by a vendor.  It works good, but I am trying to figure out what is happening when I hit the trigger too hard from a stand still.  I have two 6355 190kv motors  on 7" pneumatics wheels  and 2 TB 12s ESC's connected to the 10s lipo battery.  

Sometimes when I do an aggressive trigger pull, the battery monitor just goes dead and everything turns off.  Once I disconnect the loop key and plug it back in.  The esc's, receiver and voltmeter comes back up.

Is this normal? Is it the BMS just shutting down from a high current draw or something?

Ive been able to ride it pretty hard, its only when I have a fresh battery and I hit the trigger really hard, even when I am not standing on the board.  I just have the wheels up testing for friction.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-07-07T15:33:45.025Z Reads: 72

```
It's quite possible. Depends on your BMS; can you post a link to it? I couldn't find your buid thread.
```

---
## \#3 Posted by: Aggdaddy Posted at: 2017-07-07T18:21:41.728Z Reads: 67

```
not much details to provide.  Scramboards made the battery.  Its only listed as a 10s lipo.  Id have to remove the shrink wrap to know more.
```

---
## \#4 Posted by: rpn314 Posted at: 2017-07-07T23:14:37.676Z Reads: 57

```
Oh, okay. I don't know what to tell you then. I personally have not been impressed in general by his offerings (the "VESCs" at least, as they're just rebranded Maytechs....). Is this the one you bought?
https://www.scramboards.com/parts/pcb.html
```

---
## \#5 Posted by: Aggdaddy Posted at: 2017-07-08T02:05:00.977Z Reads: 45

```
Unfortunately, I bought a complete mtb, that didn't work from the start and it was before they changed to the dual box configuration (battery box and esc box)   .  I was just wondering if anyone else has encountered this issue with TB 12s esc's.   Never did this with a vesc config, only with the TB 12s esc's.   

Probably not an esc problem, since they can't make the battery monitor turn off.  I think the burst that the TB 12S escs are capable of is what's causing it.  So I am wondering if it will get worse, the bms that is.
```

---
## \#6 Posted by: psychotiller Posted at: 2017-07-08T02:16:12.334Z Reads: 43

```
[quote="Aggdaddy, post:1, topic:26988"]
Is it the BMS just shutting down from a high current draw or something?
[/quote]

Is it a charge/discharge bms? Bestechs will do this with precision.
```

---
## \#7 Posted by: Aggdaddy Posted at: 2017-07-08T05:18:18.194Z Reads: 36

```
Not sure.  I haven't removed the shrink wrap from the battery.  I am not familiar with BMS;s, I haven't build a battery yet, but maybe after this battery fails to charge or something.
```

---
## \#8 Posted by: psychotiller Posted at: 2017-07-08T05:34:53.405Z Reads: 32

```
Sounds like its the bms to me. Why else would both escs shut off at the same time? Unless you are hitting a low voltage cutoff. But I still doubt that.
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-07-08T06:05:53.647Z Reads: 32

```
Yeah sounds like the BMS is most likely just tripping the over current protection and shutting off. Would recommend either bypassing the over current protection and just using an inline fuse, or buying a higher current BMS.
```

---
## \#10 Posted by: Aggdaddy Posted at: 2017-07-08T15:01:48.158Z Reads: 24

```
Thanks, that's what I was looking for.  What size fuse would you recommend?
```

---
## \#11 Posted by: JdogAwesome Posted at: 2017-07-08T15:03:38.430Z Reads: 23

```
Id say 60A is fine, though if you want to have a little bigger margin 70A or 80A.
```

---
