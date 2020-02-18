# Vesc Leds explained - SOLVED

### Replies: 31 Views: 6248

## \#1 Posted by: ikjahaa Posted at: 2016-08-13T19:33:30.172Z Reads: 612

```
Currently I have some problems with my vesc, It wont rotate my motor.
I saw that there are some leds on the vesc so i thought perhaps they mean something ?
my blue and green led are constatly on and the red led is blinking. does someone know what this means ?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-08-13T19:35:57.196Z Reads: 609

```
The Bleu is for the power, the green is for the command, the red is for the drv failure (and it is normal the see the red led blinking in the vesc boot cycle)
```

---
## \#3 Posted by: ikjahaa Posted at: 2016-08-13T19:36:50.766Z Reads: 596

```
but i guess its not normal that it keeps blinking ?
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-08-13T19:39:25.105Z Reads: 571

```
No, it should just blink like tree time, if it keep blinking, it is most likely to be a drv fault... and of course a broken vesc.... but before going to this conclusion, can you post some picture, maybe we can find something else.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-08-13T19:45:33.127Z Reads: 536

```
You say the green light is for command. 
Does that mean receiver connection?
```

---
## \#6 Posted by: sl33py Posted at: 2016-08-13T19:52:33.535Z Reads: 515

```
The best way to troubleshoot is to connect it to the BLDC tool and look at the error codes if any are generated.

Did you do a motor detection and everything *was* working - or has it never worked?
```

---
## \#7 Posted by: Namasaki Posted at: 2016-08-13T19:54:14.249Z Reads: 491

```
When your out riding, does the Vesc save data that you can check later on the bldc tool ?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2016-08-13T19:54:54.768Z Reads: 474

```
Not really, I think it use to see when a command is pass from the micro-controller to DRV, but I maybe wrong, I didn't take the time to read how micro-controller is program.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-08-13T19:57:05.457Z Reads: 450

```
No, to see the data, you must leave the power on the vesc and then plug it on your computer.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-08-13T19:57:27.510Z Reads: 439

```
[quote="JohnnyMeduse, post:2, topic:7605"]
the red is for the drv failure
[/quote]


Not true, the red blinking means there's a fault code. Which could be a drv related fault code, it could mean your powering with a voltage outside of the range you set in the vesc (ie, you configured it for 38-42 volts (10s), but you are powering them with an 8s), it could be another issue. 

Red blinking after the initial 3 means there's a fault code. Hook it up to the bldc tool, connect via usb, go to live data tab, click activate sampling, and the line labeled fault code will tell you your problem (along with the other data you see there).
```

---
## \#11 Posted by: sl33py Posted at: 2016-08-13T19:58:39.074Z Reads: 419

```
agree - why it's important to connect and get the actual error code.  I had the 3 blinks (temp loss of connection/power) - from 2 different errors - Overvoltage and ABS.  Adjusted settings and worked fine afterwards.
```

---
## \#12 Posted by: ikjahaa Posted at: 2016-08-13T20:03:55.263Z Reads: 404

```
Everything was working in the past.


----------

here are some photo's of the vesc....

<img src="/uploads/db1493/original/2X/4/4b9bfd5a4768d1063ce63010e41cbce605c287e1.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/e/e3ad3592d56cffa99e530ffdc56c0c5248249488.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/a/a3f256b2c469f61c3ef256c0d5817863a0ff4418.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/7/741cc062773257b347234c604c98c3e37e9c8b99.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/4/4bd277de4eb007098b26793d07264e4a10d92a3b.jpg" width="375" height="500">
```

---
## \#13 Posted by: ikjahaa Posted at: 2016-08-13T20:07:07.901Z Reads: 346

```
Over voltage, big thanks to you man !
```

---
## \#14 Posted by: evoheyax Posted at: 2016-08-13T20:07:09.680Z Reads: 344

```
If it was working and not now, and your sure our battery is in the right voltage range (you didn't over charge or over discharge), the only way to figure anything out is to hook it up and read out the fault code. It's likely an expensive paper weight now, like my only 2 enertion vescs did the the second day I used them.
```

---
## \#15 Posted by: ikjahaa Posted at: 2016-08-13T20:07:58.889Z Reads: 340

```
Since i have 6S setup, shouldn't my max voltage be 25.2V ?
that's what i had though... was an overvoltage
```

---
## \#16 Posted by: ikjahaa Posted at: 2016-08-13T20:10:05.460Z Reads: 336

```
lipo's are 4.2V @ max and 3.3V @ min right ?
```

---
## \#17 Posted by: evoheyax Posted at: 2016-08-13T20:10:18.915Z Reads: 340

```
lipo should be min of 21 (6 x 3.5), max of 25.2 (6 x 4.2).
liion should be min of 21.6 (6 x 3.6), max of 25.2 (6 x 4.2).

anything past 3.5 and the voltage drops off. With sag, you will likely shorten the life of your battery. It should never get to less than 3.2 ever. Setting it to 3.3 might be ok, but you would need to determine your sag, and make sure your not sagging under 3.2.
```

---
## \#18 Posted by: ikjahaa Posted at: 2016-08-13T20:14:13.827Z Reads: 330

```
This is what i got now, any tips ?
changes max input voltage from 25.2 to 25.3 to cope with that error....
<img src="/uploads/db1493/original/2X/9/97b67df140490d9a02143f827110d45645bbcf77.PNG" width="534" height="148">
```

---
## \#19 Posted by: Namasaki Posted at: 2016-08-13T20:15:02.987Z Reads: 318

```
I thought Li-ion cells could safely go lower than Lipos.  3.0 volts or even 2.8v
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2016-08-13T20:17:14.044Z Reads: 313

```
Do you have something else plus over the 5V ?
```

---
## \#21 Posted by: ikjahaa Posted at: 2016-08-13T20:18:33.217Z Reads: 292

```
As you can seen on the photos, i have my receiver getting power off the 5V and gnd from the vesc
```

---
## \#22 Posted by: evoheyax Posted at: 2016-08-13T20:25:03.329Z Reads: 288

```
Not from my understanding. Everything I've read says you should go from 3.6 to 4.2.

You can probably pull it down lower than a lipo with less risk, but I still wouldn't recommend it.

Remember though, Sag needs to be accounted for.

On my space cell, at 4.2, I sag down to 4 at full throttle on flat.
At 3.6, I sag to 3.2 at full throttle on flat.
At 3.5, I sag to 3 at full throttle on flat.

But it depends on your cells max amps. Generally, as you get closer to their limits, they drop off quickly. Using a 20 amp cell, generally, you can do 15 amps with little sag, at 20, you will have a good sized sag. Just be aware of this, as I have messed up several lipos like this.

If your using more than one lipo in series, you could also over discharge one of them, because one might have a higher voltage than the other. Unless your run it through a bms that is.

These two cases are why you should...

A) get a battery with higher amps ratings then you will ever need
B) get a battery with more range than you will ever need
C) never discharge all the way down to the batteries limit
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-08-13T20:33:11.800Z Reads: 258

```
What kind of receiver are you using ?

Edit: I ask this simple question, because I see two 5v wire going to your receiver, and this look uncommon, also the 5v is provide by the DRV, witch may explain the fault.
```

---
## \#24 Posted by: ikjahaa Posted at: 2016-08-13T21:05:56.761Z Reads: 248

```
It came with my nitro rc car.

https://kyosho.com/eng/products/rc/detail.html?product_id=100269

It needs 5v as power supply....
```

---
## \#25 Posted by: Namasaki Posted at: 2016-08-13T21:09:14.283Z Reads: 246

```
Voltage sag is one of the reasons I like to discharge through a BMS
The low voltage protection on my BMS is set at 2.8v
When I was testing my new pack for max range, I ran until the BMS shut me down. (27 miles total)
When I turned the board back on, the bat meter was showing over 20% remaining at rest.
I,m happy to say that running it down to 2.8 did not damage any cells. I know this would not be the case with Lipos. In the future I will not running my pack bellow about 50% since 10-12 miles is about all I ever do in a single session.
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2016-08-13T21:13:33.606Z Reads: 235

```
have you try to power it up, without connecting the receiver ?
```

---
## \#27 Posted by: ikjahaa Posted at: 2016-08-13T21:20:57.664Z Reads: 231

```
Yea . it worked perfect before.
All is well now, it was a voltage overcharge error.
```

---
## \#28 Posted by: JohnnyMeduse Posted at: 2016-08-13T21:25:07.402Z Reads: 228

```
OK nice... (maybe just put solved on your topic)
```

---
## \#29 Posted by: evoheyax Posted at: 2016-08-14T00:05:48.948Z Reads: 216

```
I updated the title so the community knows this problem was solved.

:wink:
```

---
## \#30 Posted by: Airwolf Posted at: 2019-11-04T04:37:52.882Z Reads: 28

```
Hey Evoheyax,

I see that You have had some issues with Focbox Unity's not lasting.
 
I too have a small pile of dead Focbox Unity's and am wondering if You know of any VESC or other ESC that you consider more reliable and less likely to break soon after installation.

In other words, do You know of any other ESC's that seem to last longer than Enertion's Vescs??? I would really appreciate knowing if You are aware of another ESC that lasts longer.

Thanks in advance.
```

---
## \#31 Posted by: evoheyax Posted at: 2019-11-12T19:54:38.459Z Reads: 22

```
For me, the official trampa vesc 6 has been the most solid vesc I’ve used beside chakas but idk if he’s still making vescs or what.
```

---
