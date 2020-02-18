# Enertion Steez Remote&hellip;connected but runs motor on its own

### Replies: 11 Views: 1428

## \#1 Posted by: CRABOLSKY Posted at: 2016-08-17T11:03:22.826Z Reads: 88

```
 Hey guys I am finally taking a moment after recovering from the thumb injury to get back on the horse and continue with the build. 

 Learning from my mistakes on Monday you'll note I have the truck bolted to the board while doing this test 😛  

 I've gone through the connection process couple times now and I seem to be getting the same result. When I power on the remote and board,  I seem to be getting an unexpected results with the signal.  Essentially the motor starts running without any input from me,  but the motor will stop running when I go full reverse on the remote? 

Check out the video (notice the thumb😎) and let me know if anyone's come across this before or how I might troubleshoot the solution? 

http://www.youtube.com/watch?v=zC7W1r3hA_0

Might it be to do with my VESC settings? I ran monitor detection and applied the settings. 

<img src="/uploads/db1493/original/2X/5/536719a5adc65bfcdcc44dc612654fff8e632cf2.png" width="690" height="405">
```

---
## \#2 Posted by: lox897 Posted at: 2016-08-17T11:44:28.294Z Reads: 75

```
Have you checked your throttle trim and vesc transmitter settings?
```

---
## \#3 Posted by: CRABOLSKY Posted at: 2016-08-17T11:48:26.776Z Reads: 72

```
Shit no I haven't. I am looking at it now... Is the Steez UART?
```

---
## \#4 Posted by: Skitzor Posted at: 2016-08-17T11:56:57.714Z Reads: 72

```
disable your current control and look in the PPM tab. checkmark the display above the slider and you should see your steez values. Then above it you have to put the min and max you get in the min and max values. Now when the remote is enabled, it will be right in the middle and your motor should be quiet.

link: http://www.electric-skateboard.builders/t/vesc-ppm-settings/526/7?u=skitzor
```

---
## \#5 Posted by: CRABOLSKY Posted at: 2016-08-17T12:32:50.198Z Reads: 69

```
Fantastic @Skitzor that was the missing link... I apologise if that what obvious. I was using the Jacob tutorials which didn't go as in-depth with the programming of the remote. 

I've got the trim set not be running on its own. I am running a mac and the readouts aren't quite as friendly when you are pushing full throttle or break. No percentage readout to be able to gauge its midpoint. They glitch around (for want of a better word) and shuffle the numbers after the decimal point. I have to use screen capture to catch the readings. 
<img src="/uploads/db1493/original/2X/f/fe835f4fed7643abe4ec3169d14a57b8f2f9b603.png" width="134" height="112"><img src="/uploads/db1493/original/2X/8/86eaca50533f9dc7afb80adcba7ba4b4b0e2c6c6.png" width="175" height="170">

Although not under load or attached to a belt the motor has only distinct acceleration points. I seem to remember this being an issue for some initial Raptor customers. Even light throttle is running at 40%. I'll have to re-read their solutions. 

Is there is anything obvious in my settings please let me know... Thanks again... feeling much better.
<img src="/uploads/db1493/original/2X/0/036504d134bbda0fae73de016f6a2c6924c17f3e.png" width="690" height="405">
```

---
## \#6 Posted by: Skitzor Posted at: 2016-08-17T13:19:15.023Z Reads: 51

```
Better something obvious that you overlooked and we can solve, than being the odd one with a problem that's unfixable. 

My steez is middle at 45% though it works like it should.
Not clear if it solved your issue though?
```

---
## \#7 Posted by: CRABOLSKY Posted at: 2016-08-17T13:54:46.892Z Reads: 47

```

Yes thank you... solved the running-while-neutral issue. I'll need to look deeper into the settings to determine why it doesn't slowly/incrementally accelerate. It behaves like its more all on or off.
http://www.youtube.com/watch?v=DBQTw0nWUjw
```

---
## \#8 Posted by: ikjahaa Posted at: 2016-08-17T14:11:23.347Z Reads: 46

```
You are controlling the amp draw with your remote, not the rpm of your motor. So there is a big difference when testing without load to testing with load.

Take a look here, @onloop explains it pretty good. 
http://www.electric-skateboard.builders/t/vesc-faq-duty-cycle-vs-current-control-ppm-settings/1218?u=ikjahaa
```

---
## \#9 Posted by: Skitzor Posted at: 2016-08-17T14:52:39.174Z Reads: 40

```
Exactly what @ikjahaa said. So you're all set. Just stand on your board and you'll see it will accellerate slowly (like your finger)
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-17T14:57:50.181Z Reads: 38

```
current control gives current to overcome any load and once it does it goes full throttle since the voltage is unchanging. Duty cycle would give you throttle based speed, but will leave you with the inability to coast.
```

---
## \#11 Posted by: CRABOLSKY Posted at: 2016-08-17T22:55:05.078Z Reads: 30

```
 Thanks guys this is very helpful. I can't wait to test this out under load. I think my current settings will probably work best for my riding style.
```

---
