# Help, my motor is intermittent!(Solved)

### Replies: 17 Views: 859

## \#1 Posted by: Hardwiring Posted at: 2017-04-23T13:23:04.261Z Reads: 120

```
Hi folk
 Thanks for any pointers offered before time.....
so under throttle AND breaking my motor runs on, then off, blipping for maybe quarter of a second then the torque returns for a second, then repeat. Same under breaking, resistance for about a second then no resistance for a quarter of second (approx) then repeat. This problem appeared to start after i had used my board a dozen times.
my settings
<img src="/uploads/db1493/original/3X/e/e/ee01ae247b1bc975d5c6c64fda3ecad5a44d2cf7.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/1/4/1459e8b2a882c9821f147e43fecc3ad60699f04a.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/e/b/eba0e5c5247e9375c0ca30f666ea2b97d6268fd2.jpg" width="690" height="388">
My stuff
DIY electric skateboard VESC
10s (2x5s) 8000mah lipo
SK3-6374-168 motor
GT2B in baby buffalo form
vedder switch
Thanks for any advice
```

---
## \#2 Posted by: Hardwiring Posted at: 2017-04-23T16:11:18.823Z Reads: 87

```
I've tried a visual inspection of everything from belt to batteries no damage visible on vesc and motor turns freely. Really confused, can't seem to duplicate problem on unladen board. Are my amp limits correct?
```

---
## \#3 Posted by: LaCha Posted at: 2017-04-23T16:45:52.727Z Reads: 84

```
I once had an issue like that with a build I recently finished. It turned out the problem for me was that the heat shrink for the motor wires wasn't reaching all the way in, and the motors were shorting a little on and off.
```

---
## \#4 Posted by: Hardwiring Posted at: 2017-04-23T20:56:55.074Z Reads: 74

```

[quote="LaCha, post:3, topic:21609, full:true"]
I once had an issue like that with a build I recently finished. It turned out the problem for me was that the heat shrink for the motor wires wasn't reaching all the way in, and the motors were shorting a little on and off.
[/quote]
Like this??
<img src="/uploads/db1493/original/3X/b/a/bac5447c9074129084a22118d656f5bdda514920.jpg" width="281" height="500">
```

---
## \#5 Posted by: Jebe Posted at: 2017-04-23T21:05:59.827Z Reads: 71

```
could also be a dry solder
I had a similar problem with an enertion r-spec. solder between the motor windings and silicon cable - very little contact area here anyway, touched it up with some solder and it seemed to be fine.
<img src="/uploads/db1493/original/3X/d/9/d97e875bc88cc3cef19c33042b4391ad849157fd.JPG" width="690" height="388">
```

---
## \#6 Posted by: Titoxd10001 Posted at: 2017-04-23T21:14:39.372Z Reads: 70

```
This is probably not the cause, but you should change your max input voltage to 57v. Also you change the trim on your control to read at exactly 50% when in nuetral, then set your failsafe (button on receiver) and to check it's working properly you want to turn off your control and it should stay at 50%
```

---
## \#7 Posted by: Jebe Posted at: 2017-04-23T21:17:34.821Z Reads: 69

```
already at 48volts - assuming this is a 10s build? 48 should be plenty.
```

---
## \#8 Posted by: Titoxd10001 Posted at: 2017-04-23T21:29:17.306Z Reads: 67

```
I realize that having it at 48v might not be the cause of his issue, but there is no reason to lower it from the standard 57v
```

---
## \#9 Posted by: Hardwiring Posted at: 2017-04-23T21:32:21.138Z Reads: 64

```
Yes 10s I had the no brakes issue and raised it to 48v.
  It could well be after the vesc. Will tape connection  and report back... thanks all
```

---
## \#10 Posted by: Hardwiring Posted at: 2017-04-23T21:35:04.438Z Reads: 62

```
I reset mine and it set to 40v and I raised it (I think) but I am working on more than 1 board atm and get confused as to what I've changed and where
```

---
## \#11 Posted by: Jebe Posted at: 2017-04-23T21:42:03.510Z Reads: 57

```
set them all to 57 as Tito said. it's there to protect the cells from overcharging but in reality who immediately bombs mount everest with a full battery from their front door?
```

---
## \#12 Posted by: Hardwiring Posted at: 2017-04-23T22:44:31.617Z Reads: 55

```
No still bad, gonna get back into the vesc, restore all settings and will up that voltage
Then open my motor if necessary, hayho
```

---
## \#13 Posted by: potatowarrior13 Posted at: 2017-04-24T00:33:25.835Z Reads: 51

```
A problem I have had before is the motor screws reaching two far into the motor housing and shorting the coils, you might check that?
```

---
## \#14 Posted by: LaCha Posted at: 2017-04-24T03:34:24.482Z Reads: 48

```
No, on the other end, the motor end. Like what the other guys are posting.
```

---
## \#15 Posted by: Hardwiring Posted at: 2017-04-24T10:53:47.387Z Reads: 46

```
Now I'm struggling to remove the gear off the motor shaft, time for a bit of heat, then I can get inside and see whats what

thanks
```

---
## \#16 Posted by: Hardwiring Posted at: 2017-05-12T20:53:06.186Z Reads: 28

```
Right, solved,couple of weeks ago forgot to say

The cause? :blush: (mumble mumble mumble...............
```

---
## \#17 Posted by: Customesk8 Posted at: 2019-12-24T12:49:32.149Z Reads: 13

```
.......... what was the cause dude?
```

---
