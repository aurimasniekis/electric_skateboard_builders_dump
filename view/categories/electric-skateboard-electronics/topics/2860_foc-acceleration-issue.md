# FOC acceleration issue

### Replies: 13 Views: 1920

## \#1 Posted by: BoardAdmin Posted at: 2016-05-03T17:02:24.264Z Reads: 146

```
Hey guys,

i tried the FOC modus a little bit today. It works fine if i ride smooth and dont pull the trigger too hard. But as soon as i go full throttle the vesc stops( red light blinking) for about three or four seconds and then the controller (gt2b) can be used again. 
Sometimes this also happens if braking too strong. 
Is there a way to fix this through settings?

Thanks in advance
Badmin
```

---
## \#2 Posted by: Hummie Posted at: 2016-05-03T17:08:03.766Z Reads: 147

```
I've had similar things happen.  If the vesc is going completely off, which it sounds like, maybe your battery connection isn't good. I had to open and resolder a battery lead.  I think the high amps going through the lead burns the connection. Maybe giggle it wires and see if u can get a spark
```

---
## \#3 Posted by: BoardAdmin Posted at: 2016-05-03T17:09:25.734Z Reads: 143

```
Because of my not existing soldering skills this could be it. I´ll try it later. Thanks!
```

---
## \#4 Posted by: treenutter Posted at: 2016-05-03T18:35:46.825Z Reads: 129

```
@BoardAdmin it sounds like you're exceeding VESC's thresholds for voltage. Have you adjusted those setting in BLDC tool to match your battery setup?

I wouldn't poke around looking for a spark; if you think there is a bad solder join I would disconnect the battery pack and visually inspect it. 

... but that you're experiencing the problem at specific times (as opposed to randomly) suggests that there's something going on w voltage sag.
```

---
## \#5 Posted by: sl33py Posted at: 2016-05-03T18:52:53.667Z Reads: 123

```
agree with @treenutter - this sounds like configuration and settings issue.  I had almost identical flash (edit: LED blinking is better than flash as no sparks) and non-responsiveness for 2-3 seconds.  Vedder helped me adjust my voltage settings to fix for me.  I would connect up the VESC and do live-logging and see if you can duplicate.  It will give you specific voltage or amperage error that will help you figure out what you need to adjust in the settings.

Warning - be gentle and don't hammer it stop/go repeatedly - i fried one DRV chip doing this.   

GL!
```

---
## \#6 Posted by: Hummie Posted at: 2016-05-03T20:56:14.159Z Reads: 115

```
For me 3 red blinks is when it goes on. There's a blue light as well behind it always. And white when I throttle

My board would shut down or not come on and rustling the battery wires showed where a spark was under the shrink wrap on my nanotech a-spec rediculously expensive batteries.  It sparked a lot and now I have a dud cell
```

---
## \#7 Posted by: Bobfandango Posted at: 2016-05-03T23:42:01.563Z Reads: 101

```
3 red blinks on startup is normal I believe...
```

---
## \#8 Posted by: BoardAdmin Posted at: 2016-05-04T16:17:20.012Z Reads: 90

```
So i resoldered everything but the issue was still there. I changed the maximum input voltage from 33.6 to the default 57 and now it works fine.
Is this possible ?
```

---
## \#9 Posted by: sl33py Posted at: 2016-05-04T16:37:38.768Z Reads: 90

```
that's exactly what we were telling you.  

when you say you changed it from 33.6v to "default" 57v - what batteries (series or voltage) were you running?

If you looked at your live logging i'd bet a shiny nickel you got an overvoltage error.  Here was one of mine:
[img]/uploads/db1493/original/2X/5/55818b125bfe335f0b54232ecb3364a9155aebb3.jpg[/img]
I had this and an ABS over current error (when braking iirc).  Adjusting the settings eliminated the issue.  I would get this error - got those flashes/blinking LEDs and the ESC would be non-responsive for a couple seconds.  Adjusted and BOOM - in business again!
```

---
## \#10 Posted by: BoardAdmin Posted at: 2016-05-04T16:40:21.523Z Reads: 88

```
Yeah it just feels awesome to ride again.
```

---
## \#11 Posted by: Hummie Posted at: 2016-05-04T17:22:43.706Z Reads: 88

```


Do u know of a resource where u can learn how to use all the vescs tools?  

U can record and then play back what's happened later right?  I've heard of people riding around holding a laptop though 

I'd like to do a video recording and overlay it with all the vesc's info
```

---
## \#12 Posted by: sl33py Posted at: 2016-05-05T22:29:28.279Z Reads: 68

```
Vedder has a support forum now i believe.

As for learning the BLDC tool - i'd start w/ the basic discovery and settings unless you are getting an error.  Then only adjust if you find an issue.  Some of it is mostly common sense - setting RPM limits, etc.  Other areas are voodoo i don't understand at all.

Vedder did some great videos w/ overlay - i think he commented how he did this (it was a wired laptop i believe).  Hopefully some new ways to do this.  BT and tablet would be awesome!

GL!
```

---
## \#13 Posted by: trancejunkiexxl Posted at: 2017-08-09T05:31:17.233Z Reads: 30

```
i have also experienced this, are you sensored or unsensored.. also some controllers i have if you give throttle outside of 
 ppm range the motor will cogg and eject you.. i hope you are able to figure it out!
```

---
