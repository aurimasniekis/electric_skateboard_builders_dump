# Serious disturbance in the signal

### Replies: 2 Views: 604

## \#1 Posted by: yaniv Posted at: 2015-12-28T14:01:14.889Z Reads: 58

```
Greetings
I purchased 4 Vesc from Enertion boards.
November edition.
After learning a little , I was able to update the Firmware.
To HW 410 HW411 default.
I'm using Arduino and bluetooth, to control VESC.
In Arduino I use 4 digital outputs, one for each controller.
On PC, I see the signal received by Arduino, clean and fast.
Another computer, I see the signal received by VESC.
When connected only one VESC , no problem all looks good.
When I connect more than one, it seems that there is a serious disturbance in the signal.
One affects the other, I see it in BLDS TOOL, ppm display.
The signals in Arduino look fine.
What do you think could be the problem?
Thank you
yanv
```

---
## \#2 Posted by: Blasto Posted at: 2015-12-28T21:39:14.623Z Reads: 49

```
I had a similar problem using a tensy to control 2 vesc by ppm.

Turns out the ppm signal was to slow for the speed of the tensy (ppm is 50 to 200hz). Added a nasty 5ms delay in the control loop to correct this. Also you can turn on the means filter to get a cleaner signal.

I would higly recommend controlling the vesc by uart instead of ppm, it's faster and you could get all vesc' telemetry.
```

---
