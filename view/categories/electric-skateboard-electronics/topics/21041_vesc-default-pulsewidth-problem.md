# VESC Default Pulsewidth Problem

### Replies: 9 Views: 637

## \#1 Posted by: RunPlayBack Posted at: 2017-04-14T23:50:43.623Z Reads: 76

```
Has anyone ever encountered this before? A default pulsewidth of 1.1 with the controller off? Basically my brakes stay on unless I turn on the receiver. A safety hazard if I get a dropout or if I accidentally turn off the controller while riding.

<img src="/uploads/db1493/original/3X/5/3/53408d30c08ab908914fe5e3b08e35ecfa10ebbd.png" width="690" height="340">
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2017-04-14T23:58:32.528Z Reads: 73

```
What controller do you have? Have you adjusted your failsafe. On the gt2b there's a button on the receiver that you need to set so the pulsewidth goes to 50% neutral when there's no connection
```

---
## \#3 Posted by: RunPlayBack Posted at: 2017-04-14T23:59:47.204Z Reads: 74

```
I have a Nano controller..oh yes that's right. Let me try rebinding and see if that fixes it.
```

---
## \#4 Posted by: Titoxd10001 Posted at: 2017-04-15T00:09:35.995Z Reads: 68

```
Not sure how you adjust failsafe on that remote, maybe check manual. On gt2b there is a physical button on the receiver

Also have you given @Ackmaniac bldc firmware a try it's pretty good
```

---
## \#5 Posted by: RunPlayBack Posted at: 2017-04-15T00:15:19.663Z Reads: 70

```
Yup that did the trick thanks! I had to switch receivers during a ride and didn't bind the Nano remote correctly - basically didn't remove the bind plug before powering off. If you don't do that it doesn't set neutral correctly. It's a Winning Nano remote issue that's been documented before I just totally overlooked it. Thanks again for the help, much appreciated :)
```

---
## \#6 Posted by: Titoxd10001 Posted at: 2017-04-15T00:17:43.499Z Reads: 67

```
No problem
```

---
## \#7 Posted by: Guacamoleface Posted at: 2017-04-15T00:17:48.026Z Reads: 61

```
Yeah its just the rebinding :) I had that problem aswell and it threw me off real hard(while I cruised by a bunch of people feeling really awesome on my newely built board :joy: ).

This was followed by another issue I had with the remote(winning), random cutoffs, Not sure how often. I feel like alot of them I dont notice due to them being really quick on connecting again.
```

---
## \#8 Posted by: RunPlayBack Posted at: 2017-04-15T00:23:57.085Z Reads: 56

```
Yeah once is too many times for me, I think I may get another Mini Remote, no problems with that one.
```

---
## \#9 Posted by: Eboosted Posted at: 2017-04-15T01:15:20.276Z Reads: 54

```
This is how you fix it:


1. Turn your remote on
2. On BLDC tool go to the ppm tab
3. Select control mode as disabled and save settings (in order to avoid wheel spin during remote calibration) 
4. Adjust you calibration ppm signal, max, min pulsewight and dead band
5. Turn turn off the remote and write down how many points the dead band moves up or down from 50%
6. Turn on the remote and adjust the offset on the calibration wheel on the remote itself by the points written in the previous step until you get 50% dead band
7. Adjust the dead band again on the ppm tab on BLDC tool
8. Select current/Watt mode and save the settings
```

---
