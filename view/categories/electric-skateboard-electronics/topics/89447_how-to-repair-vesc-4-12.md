# How to repair VESC 4.12

### Replies: 18 Views: 297

## \#1 Posted by: spork Posted at: 2019-04-05T06:05:55.245Z Reads: 80

```
I've got a VESC 4.12 that's failed.  I've replaced it, but would like to learn how to repair it myself.  I have hobbyist level electronics skills, reasonable soldering equipment, a reasonable oscilliscope, and can more or less make my way around a schematic.  What I'm hoping for is to learn any tips on what items commonly fail on the VESC 4.12 and whether there are any tips on how to diagnose (either functionally or with my scope).

On this particular unit there's no obvious damage to the board or components.  I get a blue light when it's powered up and a flashing red light when I give it throttle.  I can read it's configuration with the BLDC tool, and it's producing 5V at the PPM connector to power the receiver.  But the motor is no-go.  I tried plugging in the other motor, but also no-go. 

It would be great if we could start a thread on how to diagnose and repair the most common failures on these things.

Any tips would be greatly appreciated.  Thanks.
```

---
## \#2 Posted by: Jinra Posted at: 2019-04-05T06:08:13.873Z Reads: 77

```
get the red light again and open up bldc/vesc tool and go to terminal and type "faults" see what is failing. If it's the common DRV error, hope your SMD soldering skills are up to snuff.
```

---
## \#3 Posted by: Gamer43 Posted at: 2019-04-05T06:09:26.114Z Reads: 77

```
iT's tImE tO bREaK oUt tHE hEAt gUn.

Ok in all seriousness, most VESCs fail because the DRV8302 dies due to transients or something else.
Most repairs involve replacing the DRV8302, which is more of a pain in the ass than it should be because it needs to be reflowed with hot air.
```

---
## \#4 Posted by: spork Posted at: 2019-04-05T06:25:31.204Z Reads: 70

```
Wow - that was some quick response and some great advice - thanks!  I suspected the DRV8302, but was hoping for some tips to diagnose it prior to trying to replace it (since it does look like a PITA).  Here's the result...

    The following faults were registered since start:

    Fault            : FAULT_CODE_DRV8302
    Current          : -0.2
    Current filtered : 0.9
    Voltage          : 24.60
    Duty             : 0.46
    RPM              : -0.0
    Tacho            : 0
    Cycles running   : 6
    TIM duty         : 3858
    TIM val samp     : 1932
    TIM current samp : 6136
    TIM top          : 8407
    Comm step        : 5
    Temperature      : 26.79

    Fault            : FAULT_CODE_DRV8302
    Current          : -0.7
    Current filtered : -0.2
    Voltage          : 24.60
    Duty             : 0.49
    RPM              : -0.0
    Tacho            : 0
    Cycles running   : 21
    TIM duty         : 3899
    TIM val samp     : 1956
    TIM current samp : 5908
    TIM top          : 7904
    Comm step        : 5
    Temperature      : 26.79

I'm not entirely sure what to make of this message other than that it seems to be the DRV8302.
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-04-05T07:04:53.221Z Reads: 56

```
I'll say it again :P.
[quote="Gamer43, post:3, topic:89447"]
iT’s tImE tO bREaK oUt tHE hEAt gUn.
[/quote]
```

---
## \#6 Posted by: spork Posted at: 2019-04-05T07:17:01.385Z Reads: 55

```
Indeed.  I've done some SMD drag soldering, but not yet done it with a heat gun.  Fortunately we have a good reflow solder station and an expert at the office. :smile:   Been watching videos on the technique.

Should be fun to give it a try.  And fortunately the VESC is already broke. :smile:
```

---
## \#7 Posted by: xilw3r Posted at: 2019-04-05T07:31:07.678Z Reads: 53

```
pfffff reflow station.. too easy, go hard core with manual hot air :D 

I joke, my vesc had the same fault, a colleague helped replace the damned DRV, hardest part was to get the chip, they are often out of stock, go order now.
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-04-05T07:32:42.945Z Reads: 51

```
https://www.arrow.com/en/products/drv8302dca/texas-instruments

142 in stock, free shipping, gogogogo
```

---
## \#9 Posted by: robthebuilder Posted at: 2019-04-05T07:56:13.027Z Reads: 50

```
I tried replacing mine on my first VESC with manual hot air but I failed. I just bought another VESC and tried to stay happy about it :joy: I still have the old VESC and a spare DRV-chip so I will try it again soon but with more time and patience! I thinks it should be possible even without the right tools.
```

---
## \#10 Posted by: spork Posted at: 2019-04-05T07:57:15.768Z Reads: 49

```
Just placed the order.  Thanks!
```

---
## \#11 Posted by: spork Posted at: 2019-04-08T06:22:27.424Z Reads: 31

```
Question...

My DRV8302 is supposed to arrive tomorrow, so I hope to try and swap it out then.  But it occurs to me that I don't know how to make sure and flow the solder on the pad beneath the chip with a hot-air rework station.  Is there any secret?  

And if I get things too hot are the components going to fall off the other side of the board?
```

---
## \#12 Posted by: Jinra Posted at: 2019-04-08T06:43:06.750Z Reads: 28

```
Just look at SMD soldering videos. Use lots of flux...
```

---
## \#13 Posted by: spork Posted at: 2019-04-08T07:18:13.720Z Reads: 27

```
I have checked out SMD soldering videos.  Haven't found one that addressed the pad under the chip.  Perhaps I just need to keep looking.
```

---
## \#14 Posted by: Jinra Posted at: 2019-04-08T07:22:03.317Z Reads: 26

```
https://www.youtube.com/watch?v=c_Qt5CtUlqY
```

---
## \#15 Posted by: spork Posted at: 2019-04-08T07:30:37.756Z Reads: 23

```
Great reference.  Thanks!
```

---
## \#16 Posted by: Gamer43 Posted at: 2019-04-08T07:42:26.891Z Reads: 23

```
When I did it, I had to eyeball it, I held the the heat gun to the chip til I saw the majority of the pins/ pads reflow. Held the chip in place using pliers. Held the heat gun directly over the board, perpendicular. I aligned and tacked on all the pins before reflowing.

My issue was not the parts on the opposite side, but the parts right next the drv8302 getting blown away by the hot air. Surface tension should hold the parts on the opposite side on as long as you apply heat for the shortest amount of time as you can.
```

---
## \#17 Posted by: spork Posted at: 2019-04-08T08:21:51.831Z Reads: 20

```
[quote="Gamer43, post:16, topic:89447"]
My issue was not the parts on the opposite side, but the parts right next the drv8302 getting blown away by the hot air.
[/quote]

Does that mean you should have used less airflow, or does that cause other problems?
```

---
## \#18 Posted by: Gamer43 Posted at: 2019-04-08T08:23:53.488Z Reads: 18

```
Holding the heat gun perfectly perpendicular didnt cause a problem, it wasn't until I angled it did it start blowing things away. If I could I wouldve used less airflow.
```

---
