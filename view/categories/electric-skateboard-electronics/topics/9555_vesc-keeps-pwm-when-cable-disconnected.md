# VESC keeps PWM when cable disconnected

### Replies: 16 Views: 1128

## \#1 Posted by: chinzw Posted at: 2016-09-13T21:26:05.075Z Reads: 81

```
Im not sure if anyone had this problem or even tryied it out, but yesterday i was failsafe testing and realized that if i unplug the receiver cable while holding the throttle, the VESC will keep spinning at that speed until i reconnect the cable! Am i missing some setting or what? This is extremely dangerous.
```

---
## \#2 Posted by: DougM Posted at: 2016-09-13T22:51:28.450Z Reads: 75

```
It's been discussed [here](http://www.electric-skateboard.builders/t/hidden-dangers-of-esk8ing-causes-effects/8255/6)
```

---
## \#3 Posted by: chinzw Posted at: 2016-09-13T23:11:41.470Z Reads: 72

```
Im wondering if there's any solution. I can see a "timeout" setting in the VESC, but it does nothing. When there's no PWM signal the board should do nothing, not keep the last value. I've set my remote failsafe, and that works fine if my remote disconnects or i turn it off.
```

---
## \#4 Posted by: DougM Posted at: 2016-09-14T14:44:50.201Z Reads: 54

```
There is a solution, but not on our end - you'd have to get either Vedder himself or a good C++ programmer to go into the VESC source and locate.

Now that Chinzw has found what looks like an easy repro scenario it shouldn't be that difficult to fix.  However, I'm not certain that there is just one bug here, there might be several.

Seems as though the best way to do it would be for those who send him checks every month to put a note in that politely asks him to look at the issue...
```

---
## \#5 Posted by: chinzw Posted at: 2016-09-14T16:32:25.450Z Reads: 48

```
I'll start going through the code once i get some free time. It seems that the timeout isn't working as it should.
```

---
## \#6 Posted by: DougM Posted at: 2016-09-21T21:48:19.490Z Reads: 36

```
The same problem exists in the serial interface - if you can look at that as well you might save my life :slight_smile:
```

---
## \#7 Posted by: chinzw Posted at: 2016-09-21T22:25:56.064Z Reads: 33

```
Forgot to update this thread, as Benjamin explained in his forum BLDC Tool sends packets to the VESC to keep it awake, so the disconnect failsafe wont work while plugged in to the USB port. I haven't had the time to try this out, but im pretty sure it will work like that.
```

---
## \#8 Posted by: DougM Posted at: 2016-09-21T23:14:14.057Z Reads: 32

```
That will likely clear up your repro scenario, but my failure was on the road.
```

---
## \#9 Posted by: chinzw Posted at: 2016-09-21T23:25:39.953Z Reads: 29

```
What's your exact problem?
```

---
## \#10 Posted by: DougM Posted at: 2016-09-21T23:48:57.770Z Reads: 29

```
I have a control board upstream that takes the input from the handheld controller (XBee) and converts it to commands the VESC understands and sends them via serial.  The control board is powered by VESC.  While riding on a trail the control board (I suspect) got hit by a static discharge that killed the processor (a Teensy 3.2) and shorted the power to the board to ground.  (as soon as I removed the Teensy the power came back) So the control board is completely dead.

VESC did not timeout correctly and continued to execute the last command sent, which unfortunately was an accelerate command (it's actually the VescUartSetCurrent(); command in RollingGecko's arduino [library](https://github.com/RollingGecko/VescUartControl).

Thanks,
```

---
## \#11 Posted by: chinzw Posted at: 2016-09-21T23:58:56.228Z Reads: 28

```
Hmm,thats odd, since i can see in the code there's a timeout implemented:

case COMM_SET_CURRENT:
    ind = 0;
    mc_interface_set_current((float)buffer_get_int32(data, &ind) / 1000.0);
    timeout_reset();
    break;
```

---
## \#12 Posted by: DougM Posted at: 2016-09-22T01:16:12.977Z Reads: 27

```
I think the problem is in the code that receives the serial command.

My best guess is that there's a buffer that the serial data goes into and that buffer does not get cleared between serial receive calls, so that when the call fails the buffer does not get updated and the same value gets passe down the line.
```

---
## \#13 Posted by: chinzw Posted at: 2016-09-22T02:46:00.530Z Reads: 26

```
that code i pasted in my previous message is the one that handles the serial commands
```

---
## \#14 Posted by: DougM Posted at: 2016-09-22T03:03:18.447Z Reads: 25

```
[quote="chinzw, post:11, topic:9555"]
mc_interface_set_current
[/quote]

what happens if mc_interface_set_current doesn't return?
```

---
## \#15 Posted by: chinzw Posted at: 2016-09-22T03:21:44.649Z Reads: 23

```
That's part of the VESC so having your Rx or UART disconnect will not stop the function from returning.
```

---
## \#16 Posted by: DougM Posted at: 2016-09-22T15:30:46.693Z Reads: 20

```
I'm coming at this from an end-user standpoint, not a code standpoint, so maybe I'll stop guessing what's wrong :-)  

The bottom line is that somehow VESC does not time out in the instance where the serial stream is interrupted in an unknown fashion.  My best guess is that holding both TX and RX low will cause this.  

The other anomaly was that the power on the controller board was shorted to ground, but that was on the other side of a 3.3v regulator, so that wouldn't pull the VESC 5v output directly to ground, but would put a significant load on it.

In any event, thank you for looking into it.  I will try to create a repro scenario and will post here if I can do it.
```

---
