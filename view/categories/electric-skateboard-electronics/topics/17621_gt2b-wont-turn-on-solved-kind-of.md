# GT2B won&rsquo;t turn on. Solved kind of

### Replies: 21 Views: 1701

## \#1 Posted by: Kaden56 Posted at: 2017-02-13T00:08:28.918Z Reads: 102

```
I did a basic gt2b mod a while back and the remote has been working great until now. The timeline goes as follows.

-**About 2 months ago** I hooked up my receiver and remote and it worked great. 

-**Couple weeks later** the red light started flashing whenever the remote was on but it still kept working great.

-**The other day** I rode it on campus and it worked perfectly for half the day, then I went to turn it on and no lights or anything. Almost like a totally dead battery. I plugged it in to charge for about an hour during which time the green light was on so I assumed it was charging. Then an hour later I unplugged it from the charger and tried turning it on. Nothing. Later that night I flipped it on and it turned on! Light still flashing but it was on! Then within 15 seconds of riding my board it felt like it was throwing out a sketchy signal (board was jumpy) and then the lights went off and it was dead. 

**What have I done so far?** 
I took it apart and checked for any shorts or opens and there was nothing. I looked over the circuit board and nothing looked burned out or disconnected. I tried another 3.7V battery and it didn't turn on at all. I also checked the switch by shorting it to see if it would turn on and it did not. 

I would like to ride my board this weekend when I go to visit family so I'm really trying to figure out my remote situation ASAP! Thank you for any help!
```

---
## \#2 Posted by: jmasta Posted at: 2017-02-13T05:07:57.185Z Reads: 87

```
Any luck on your problem?

My GT2B is completely dead now.  Plugging into USB does nothing and no LEDs turn on anymore :frowning:
```

---
## \#3 Posted by: Kaden56 Posted at: 2017-02-13T06:28:08.847Z Reads: 82

```
na man I wish some people would chime in but maybe no one has any idea what's going on. I just really need to get it fixed before this weekend!
```

---
## \#4 Posted by: jmasta Posted at: 2017-02-13T06:36:59.218Z Reads: 80

```
Well this was my solution.  Haha

<img src="/uploads/db1493/original/3X/7/b/7b8b49aebd782d113c07663bd2f690b58cfb29c7.png" width="690" height="323">
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-02-13T14:29:20.330Z Reads: 74

```
Maybe the battery died or something got damaged through an impact, like a broken solder spot.
Screw it open and look over everything. If you find something broken, solder it. Measure your battery if its ok.
If everything looks good, battery still ok but it simply won´t work properly, just get a new one :+1:
```

---
## \#6 Posted by: jmasta Posted at: 2017-02-13T16:05:54.265Z Reads: 67

```
Mine is still stock, so I can't speak for Kaden, but it has the same exact symptoms he is describing.  My GT2B's lipo is currently at 2.90V, so I think a low voltage cutoff must be active.  I question whether my remote's charging circuit ever even worked correctly

@Kaden56 was your red or green light flashing? My red LED was solid, and the green was flashing. Charging LED would not light up, even when plugged into USB.   But now no LEDs light up

Maybe I can figure out a way to hook that little 1S lipo up to my balance charger...
```

---
## \#7 Posted by: Kaden56 Posted at: 2017-02-13T21:57:05.268Z Reads: 61

```
Mine had a solid red and blinking green while
It was on. I tried it with another 1s battery and still nothing.
```

---
## \#8 Posted by: jmasta Posted at: 2017-02-13T22:14:15.386Z Reads: 61

```
Well I "fixed" my dead GT2B by rigging up a balance charger directly to the 1S lipo.  Attached wires with Kapton tape and charged at 0.8A (1C)

<img src="/uploads/db1493/original/3X/3/e/3e12ad76eb3b02a39ff051e34db4edbc9b2d1163.JPG" width="666" height="500">

The remote works again. Solid red power LED and solid green status LED.  But plugging a USB charger into the remote does not indicate it's charging at all.  Shouldn't the charge LED blink red?  I am wondering if the FS-GT2B has a problem with the internal charge circuit...
```

---
## \#9 Posted by: AndyPG Posted at: 2017-02-14T18:49:39.064Z Reads: 58

```
[quote="jmasta, post:6, topic:17621"]
My GT2B's lipo is currently at 2.90V,
[/quote]

As soon as the low battery light starts blinking, you need to be charging up.
2.9v is well into permanent battery damage territory.
There are a few recovery methods which should be done very carefully and visually monitored 100%.[quote="jmasta, post:8, topic:17621"]
Well I "fixed" my dead GT2B by rigging up a balance charger directly to the 1S lipo
[/quote]

Note that the little GT2B battery is a Li-ion not a LiPo.
```

---
## \#10 Posted by: Kaden56 Posted at: 2017-02-14T19:24:19.165Z Reads: 56

```
Turns out that was the problem with mine too! The battery just wasn't actually charging when I would plug it in via usb. The battery finally just completely died. I got an old spare 3.7v lion battery from an old camera and tested it to see if it was the battery and I thought I could rule out the battery being the issue cause it still didn't work. Turns out that battery was just completely dead too! I charged it up in the camera and then took it out and put it into my remote and it worked! So until I get my nano x receiver fixed and back from enertion I'll be taking the battery out of the enclosure and charging it in my camera and then putting it back into the remote. 

So this brings up something interesting though. Why are mine and some others gt2b's batteries not charging via the usb port after modding them? I did a very simple mod too. No relocation of the usb port or anything. Just cut off the excess part of the CB on the side and then soldered the pos and neg wires to the battery. Any ideas?
```

---
## \#11 Posted by: PXSS Posted at: 2017-02-14T19:34:29.943Z Reads: 54

```
Its a LiPo. It says so right on the battery
```

---
## \#12 Posted by: PXSS Posted at: 2017-02-14T19:36:41.354Z Reads: 53

```
You could have stressed the board and created microfractures, try reflowing the components, maybe a via is damaged too, you can grab a multimeter and check for continuity. throughout
```

---
## \#13 Posted by: jmasta Posted at: 2017-02-14T20:45:38.009Z Reads: 52

```
[quote="AndyPG, post:9, topic:17621, full:true"]
[quote="jmasta, post:6, topic:17621"]
My GT2B's lipo is currently at 2.90V,
[/quote]

As soon as the low battery light starts blinking, you need to be charging up.
[/quote]

My GT2B will not charge.  Plugging in a USB power source does nothing.  And my remote is still 100% stock. No drops or damages. No mods.

Same problem as @Kaden56 it seems. But it helps narrow down the problem to the actual FS-GT2B, and not a case mod or USB relocation issue
```

---
## \#14 Posted by: AndyPG Posted at: 2017-02-14T21:04:55.059Z Reads: 47

```
[quote="PXSS, post:11, topic:17621, full:true"]
Its a LiPo. It says so right on the battery
[/quote]

Are we looking at the same picture?
It clearly says Li-ion.
```

---
## \#15 Posted by: jmasta Posted at: 2017-02-14T21:05:34.905Z Reads: 44

```
Li-ion Polymer... aka LiPo  :)



Side note:  To what voltage does the GT2B charge it's battery at full capacity?  It seems like charging to 4.20 or even 4.15V might not be ideal since it takes so long to discharge the battery.  I stopped mine at 3.85V.  **Would one of you mind measuring a fully charged battery?**  Thanks!
```

---
## \#16 Posted by: AndyPG Posted at: 2017-02-14T21:07:15.826Z Reads: 41

```
[quote="jmasta, post:15, topic:17621"]
Li-ion Polymer... aka LiPo  :slight_smile:
[/quote]

[quote="PXSS, post:11, topic:17621, full:true"]
Its a LiPo. It says so right on the battery
[/quote]

Sorry guys, you're both mistaken.
Google it...:slight_smile:
Li-ion is not Li-Po...
```

---
## \#17 Posted by: jmasta Posted at: 2017-02-14T21:09:39.364Z Reads: 41

```
https://en.wikipedia.org/wiki/Lithium_polymer_battery

> A lithium polymer battery, or more correctly **lithium-ion polymer battery** (abbreviated variously as **LiPo**, LIP, Li-poly and others), is a rechargeable battery of lithium-ion technology in a pouch format. Unlike cylindrical and prismatic cells, LiPos come in a soft package or pouch, which makes them lighter but also less rigid.
```

---
## \#18 Posted by: AndyPG Posted at: 2017-02-14T21:14:16.392Z Reads: 39

```
Guys, Please do some Googling.
You are confusing Li-Po's with Li-Ion.
They are different batteries.
Probably better to let the thread get back on track.
```

---
## \#19 Posted by: jmasta Posted at: 2017-02-14T22:04:51.707Z Reads: 39

```
Maybe we are using a different google machine.  LiPo's are a form of lithium-ion batteries.  Most cell phones today use LiPo's, despite them generally being referred to as simply "lithium ion".  LiPo's are li-ion; squares are rectangles.  Li-ion is not necessarily LiPo, just as a rectangle doesn't have to be a square

Anyway, we are tying to figure out why our GT2B's are not charging....
```

---
## \#20 Posted by: PXSS Posted at: 2017-02-14T22:10:50.735Z Reads: 37

```
Not confused. Knowing battery technology is my job.
Yes, Lithium-Polymer batteries and Lithium-Ion batteries are not the same.
Lithium-Polymer batteries DO NOT exist in the consumer world, you rarely see them in the industrial world and are more often seen in academia. The reason the technology has not developed is because it performs poorly at room temperatures.

What most people refer to LiPos in the consumer world are ***Lithium-Ion Polymer*** cells.
All RC batteries in the consumer market are Lithium-Ion Polymer batteries.
The difference in what we call Li-ion and Li-Po is the packaging and slight chemical changes.
The cell in the picture by those standards is a Li-Po.

You can read more at:
http://batteryuniversity.com/learn/article/the_li_polymer_battery_substance_or_hype
Don't tell people they are mistaken without backing up your statement with some actual data or citations.
Makes you seem like an ass no offense...
```

---
## \#21 Posted by: PXSS Posted at: 2017-02-14T22:15:44.258Z Reads: 35

```
Can you take a couple of pictures?
Could anything on the board be burned?
Try measuring things with a voltmeter, maybe you can pinpoint it to a component.
```

---
