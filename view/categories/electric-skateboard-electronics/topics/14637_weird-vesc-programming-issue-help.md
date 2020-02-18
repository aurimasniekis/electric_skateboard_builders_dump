# Weird VESC programming issue. Help?

### Replies: 19 Views: 730

## \#1 Posted by: mmaner Posted at: 2016-12-14T03:33:55.060Z Reads: 63

```
I bought a VESC from DIY, connected it just the like the YouTube tutorial but I never get a usable port.  Any ideas?
```

---
## \#2 Posted by: mmaner Posted at: 2016-12-14T03:54:52.267Z Reads: 64

```
Btw, I've tried it in 2 PC's with 2 different USB cables.  Alli get is a blue light with a rapid blink, not the multi-color lights I expected. Any help would be greatly appreciated. Thanks
```

---
## \#3 Posted by: Esrapp21 Posted at: 2016-12-14T03:57:20.104Z Reads: 64

```
Is everything connected, the motor and battery? Also, if everything is connected, try a different cord. I have had unusable USB cords before, maybe that's the issue...
```

---
## \#4 Posted by: mmaner Posted at: 2016-12-14T03:59:18.367Z Reads: 63

```
Yep, motor and battery pack are connected. I tried a different cable as well.  It's a 6s battery pack, could that be the issue?
```

---
## \#5 Posted by: rpn314 Posted at: 2016-12-14T04:03:41.056Z Reads: 54

```
If you've had the issues across known working USB cables my guess is the bootloader. Issues like this seem to always lead back to a missing/bad bootloader. Which tutorial are you following exactly?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-12-14T04:04:13.229Z Reads: 56

```
[quote="mmaner, post:2, topic:14637"]
Alli get is a blue light with a rapid blink
[/quote]

WEIRD, the blue light is suppose to be the Power... except if they change the placement do you have any video of the booting (what the led does when you plug the power)
```

---
## \#7 Posted by: mmaner Posted at: 2016-12-14T04:10:19.552Z Reads: 51

```
I'm.using the DIY tutorial here...
https://www.youtube.com/watch?v=dxDXUrk-7ek

But I've done tons of reading g and watching, trying g to get familiar as this is my 1st VESC.
```

---
## \#8 Posted by: mmaner Posted at: 2016-12-14T04:11:19.440Z Reads: 51

```
I don't, and I left it at work so I can't get it right now...but I will post some 1st thing in the morning. But for real, it's just a rapid blue light.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-12-14T04:13:55.276Z Reads: 49

```
If the blue light it at the same place as the other one (the one in your video), and is blinking you might have a hardware issue with you VESC
```

---
## \#10 Posted by: caustin Posted at: 2016-12-14T05:31:23.002Z Reads: 42

```
I had that issue, spent a lot of time on boot loader etc. Then tried another USB cable and it worked, USB with power and data.
```

---
## \#11 Posted by: Eboosted Posted at: 2016-12-14T05:43:27.735Z Reads: 44

```
Have you got the latest VESC version from DIY? 4.12? 

Hope you find the fix, please keep us posted as I got the same vesc yesterday and would like to know if I'll have the same issues
```

---
## \#12 Posted by: mmaner Posted at: 2016-12-14T18:41:22.507Z Reads: 31

```
I think Ive isolated this down to a battery issue.  frikkin zippy's are gonna drive me to drinking.  Ill update when I get a new pack in.
```

---
## \#13 Posted by: rpn314 Posted at: 2016-12-14T19:23:02.288Z Reads: 32

```
Batteries shouldn't have any effect on connecting via USB as long as they're at some minimal voltage (5-6V I think). You could literally power the VESC enough to connect to USB with a couple AA batties (try 5 in series?)
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-12-14T19:29:54.200Z Reads: 28

```
If the power fluctuate, the vesc might not be able to boot properly
```

---
## \#15 Posted by: rpn314 Posted at: 2016-12-14T19:31:41.344Z Reads: 26

```
True.

@mmaner what did you do to determine that it was the zippy's? Have you tried watching the battery voltage with a multi-meter when you attempt to turn on the vesc and connect to it?
```

---
## \#16 Posted by: mmaner Posted at: 2016-12-14T19:54:10.063Z Reads: 21

```
Ive got 1 cell that will not balance in a series pack.  Its below the minimum so I think the VESC is defaulting to auto-cutoff.
```

---
## \#17 Posted by: rpn314 Posted at: 2016-12-14T20:02:17.143Z Reads: 22

```
Unless it's really low, the vesc won't cutoff for USB connections. The low voltage cutoff is to cutoff the motors.

However if you've got a LiPo pack that isn't balancing correctly I would definitely replace it.
```

---
## \#18 Posted by: mmaner Posted at: 2016-12-14T20:03:28.748Z Reads: 19

```
I'm trying to find a decent battery now, but the only ones available immediately are pretty pricey.  I might end up getting a couple of new Zippy's to get through to the new year.
```

---
## \#19 Posted by: mmaner Posted at: 2016-12-14T22:06:04.446Z Reads: 19

```
yep, it was the battery pack.  I found  a good 5k mAh 3s lipo and it kicks right off.  frikkin zippys...
```

---
