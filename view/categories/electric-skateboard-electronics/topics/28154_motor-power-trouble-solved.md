# Motor power trouble (SOLVED)

### Replies: 28 Views: 698

## \#1 Posted by: DaffieT Posted at: 2017-07-20T22:39:17.477Z Reads: 68

```
I am having an issue where my motor just doesn't spin fast enough, I have tried many different settings on the vesc to try and help it but it just isn't going that fast. I am wondering if my power supply (3 5000mah batteries) isn't enough to power the motor efficiently but that doesn't seem like that would be the case. The motor spins decently fast with no load but when I connect the wheel it just doesn't spin fast (2-5mph) (3-8kph). Help is appreciated thanks.
My set up
Torqueboards vesc
3 5000 mah batteries in parallel
6374 190 kv torqueboards motor
80mm wheels with 20 tooth motor pulley and 74(counting may be off a little bit) tooth wheel pulley.
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-20T22:45:00.356Z Reads: 65

```
What voltage are you batteries not clear from the description also include screenshots of your VESC configuration, could be low voltage cut off or some other limits.
```

---
## \#3 Posted by: DaffieT Posted at: 2017-07-20T22:49:21.563Z Reads: 61

```
3 11.1v batteries so 33.3v
<img src="/uploads/db1493/original/3X/a/2/a266b4ab8eea5b7025991ead0a10bf27ce737d4b.png" width="690" height="345">
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-20T22:50:40.868Z Reads: 53

```
So 3 3S LiPo batteries in series (you said parallel but think you mean in series if you're adding the voltages)
```

---
## \#5 Posted by: DaffieT Posted at: 2017-07-20T22:51:42.982Z Reads: 50

```
Yes series my bad
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2017-07-20T22:52:07.086Z Reads: 51

```
[quote="DaffieT, post:1, topic:28154"]
3 5000 mah batteries in parallel
[/quote]

3s batteries in parallel should give you 11.1V not 33V to get 33V they need to be in series.
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-20T22:52:13.742Z Reads: 49

```
If they're in parallel you're not getting 33.3v
```

---
## \#8 Posted by: wafflejock Posted at: 2017-07-20T22:58:37.848Z Reads: 48

```
If it is 3 3S LiPo in series it's effectively 9S you should be able to check the voltage with a voltmeter on the leads going into the VESC.  Battery cut offs look okay though...

Your battery max seems really low why 25A ?  If they are say 20C batteries you can pull 20*5Ah = 100A from them "safely".  VESC can't handle that continuously but should protect itself in terms of thermal cut off if things are getting too toasty.

---

Edit this is a bad idea.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-07-20T23:07:00.002Z Reads: 46

```
[quote="wafflejock, post:8, topic:28154"]
Your battery max seems really low why 25A ?  If they are say 20C batteries you can pull 20*5Ah = 100A from them "safely".  VESC can't handle that continuously but should protect itself in terms of thermal cut off if things are getting too toasty.
[/quote]

**Please Don't it's playing with fire...** 25A to 40A is more than enough, best thing to do is starting at 25A and then if you don't feel like having enough torque, then ramp up the current little by little..
```

---
## \#10 Posted by: wafflejock Posted at: 2017-07-20T23:09:16.260Z Reads: 43

```
Hmm yeah fair didn't meant to imply setting it up to 100A right away but saw a few other threads that it helped to bump that up for better performance.  If it's only going 5mph though sounds like something else is wrong at 9S with 25A you'd be pushing 825W through the system so you should be moving faster than 5mph.
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-07-20T23:12:45.387Z Reads: 41

```
[quote="wafflejock, post:10, topic:28154"]
like something else is wrong
[/quote]

Yeah... and that why we might need more screen shot and picture @DaffieT

Also @DaffieT connect the vesc to the bldc tool and go on the tab "Realtime Data" and then check the box in the right corner "activate sampling" then take a screen shoot.
```

---
## \#12 Posted by: DaffieT Posted at: 2017-07-21T01:26:27.042Z Reads: 33

```
<img src="/uploads/db1493/original/3X/e/8/e8839e2a8bd758c62f3f9f2eecbb5a11f2ff9875.png" width="690" height="368">

Sorry for replying so late. had a dinner
```

---
## \#13 Posted by: DaffieT Posted at: 2017-07-21T01:26:57.021Z Reads: 29

```
also i amped it up to 40a
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-07-21T01:37:49.018Z Reads: 29

```

OK... so your batteries are in parallel... so you are running at 12V instead of 33V... you have to pu your batteries in series to gain some speed

<img src="/uploads/db1493/original/3X/8/d/8d3e0be3861b39278a06ce84b2345b00743bf88a.png" width="690" height="368">
```

---
## \#15 Posted by: DaffieT Posted at: 2017-07-21T01:40:20.770Z Reads: 29

```
Hmmm, I guess I mad a big mistake, ill draw my setup one sec.
```

---
## \#16 Posted by: DaffieT Posted at: 2017-07-21T01:47:03.342Z Reads: 30

```
<img src="/uploads/db1493/original/3X/2/8/28a616d2032af98125a2b34966d854b6d7c03f32.JPG" width="666" height="500">
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2017-07-21T01:51:46.092Z Reads: 29

```
Your Drawing look good, can you poste some picture of your connection ?
```

---
## \#18 Posted by: wafflejock Posted at: 2017-07-21T01:54:29.396Z Reads: 30

```
Looks like you made a series circuit then added it to another series circuit which should be fine but there's sort of an extra connector in there it could also just be one negative lead from first battery then positive to negative from one battery to the next until you get to the last battery and you have the positive from that one to connect to the VESC.

---

Need pictures of the real thing like @JohnnyMeduse said shouldn't be showing 12V in the realtime data
```

---
## \#19 Posted by: DaffieT Posted at: 2017-07-21T01:56:58.644Z Reads: 30

```
<img src="/uploads/db1493/original/3X/4/b/4b808a33cedf74dd1d453512ac34ec33892aeea1.JPG" width="375" height="500">
```

---
## \#20 Posted by: DaffieT Posted at: 2017-07-21T01:57:11.441Z Reads: 28

```
can you give me a visual?
```

---
## \#21 Posted by: benwong Posted at: 2017-07-21T02:01:38.814Z Reads: 30

```
better cover up all the wire connection point with heat shrink to prevent any short.
```

---
## \#22 Posted by: DaffieT Posted at: 2017-07-21T02:07:32.373Z Reads: 29

```
Done, any idea why I'm only getting 12v?
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2017-07-21T02:23:23.832Z Reads: 28

```
check your connections, my best guess is that one of your batteries in the wrong polarity.

+12V +12V -12V = 12V
```

---
## \#24 Posted by: wafflejock Posted at: 2017-07-21T02:23:36.750Z Reads: 27

```
Basically can do it like shown in the picture here:

http://www.streetmusician.co.uk/batteryconnections/

Ignore the stuff on the page about amperage really if you are multiply the Ah by the Voltage you get Wh not Watts, Watts is if you multiply actual Amps drawn by voltage, amp hour is capacity not flow.

---

Helps to keep all the negative wires black just to keep your orientation all correct too.  If you don't have black wire can just wrap those in electric tape to mark them.
```

---
## \#25 Posted by: DaffieT Posted at: 2017-07-21T02:25:33.126Z Reads: 28

```
Yup that's what it was dang boneheaded mistake
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-07-21T02:28:42.018Z Reads: 28

```
[quote="DaffieT, post:25, topic:28154, full:true"]
Yup that's what it was dang boneheaded mistake
[/quote]

could have been worst, could have been -12V... then you would have had some serious problems. the magic smoke would have escaped (mark the thread as solved)
```

---
## \#27 Posted by: DaffieT Posted at: 2017-07-21T02:39:36.020Z Reads: 26

```
Can't thank you enough for your help👍

How do I mark as solved?
```

---
## \#28 Posted by: Michaelinvegas Posted at: 2017-07-21T05:11:52.294Z Reads: 20

```

```

---
