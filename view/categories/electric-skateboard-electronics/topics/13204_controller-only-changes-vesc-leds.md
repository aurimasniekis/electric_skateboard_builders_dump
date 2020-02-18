# Controller only changes VESC LEDs

### Replies: 15 Views: 1087

## \#1 Posted by: meercat Posted at: 2016-11-17T00:45:58.986Z Reads: 62

```
This is stumping me, even after doing a lot of searches. Brand new build. It's a dual-motor board, but I'm just working with one VESC/motor to start my testing.

I have the battery, VESC, and motor connected. The BLDC tool seems to test the configuration just fine, and spins the motor. However, when I connect the controller (torqueboards nano), it syncs just fine, but won't drive the motor. The blue LED is always lit. When I pull the throttle *down* and hold it for a second and release, the green LED lights and stays on. It goes out if I push the throttle *up* and hold it for second, then release.

What am I doing wrong here? It's driving me crazy.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-11-17T00:50:28.437Z Reads: 59

```
Please send a screenshot of your BLDC tool config.
```

---
## \#3 Posted by: meercat Posted at: 2016-11-17T00:53:24.283Z Reads: 61

```
This screen? <img src="/uploads/db1493/original/3X/a/4/a47e6f265016cea9990da0b370be4be96b6fa415.png" width="690" height="358">
```

---
## \#4 Posted by: tim_felbinger Posted at: 2016-11-17T00:58:47.739Z Reads: 57

```
Go to the app configuration tab.

Under General make sure it is set to PPM

Then go to the PPM tab.

Under this tab you will want to check the box that says display. That will show you the input signal you are getting from the controller.

Setup the max and min values appropriately. See this: http://vesc.net.au/

Then set the mode control mode to whatever you like. 

Most people seem to prefer 'current no reverse with brake' or 'current' (which has reverse)
```

---
## \#5 Posted by: meercat Posted at: 2016-11-17T01:03:27.855Z Reads: 49

```
Thanks @tim_felbinger. It was set to PPM. On the display signal area, it shows full reverse throttle at 12% and full forward throttle at 81%. Still, I don't get any motor action with the remote. Just the LED action described earlier.
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-17T01:04:29.973Z Reads: 44

```
You need to select a mode, its probably set to "Disabled". The most common mode is "Current no reverse with brake"
```

---
## \#7 Posted by: meercat Posted at: 2016-11-17T01:07:22.059Z Reads: 48

```
<img src="/uploads/db1493/original/3X/9/b/9bcb1705a9e97df850f5fcc4e1bcb49da1eca613.png" width="690" height="356">
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-17T04:24:12.754Z Reads: 38

```
You're running sensored mode, but your hall sensor detection is failing, which usually means you don't have sensors plugged in. If you're not using sensors make sure to change the motor mode to unsensored.
```

---
## \#9 Posted by: meercat Posted at: 2016-11-17T04:29:35.975Z Reads: 39

```
I am just leaving the sensors disconnected while I'm connected to the BLDC tool because plugging them in disconnects it from the BLDC tool for whatever reason. I've tried them in both sensors and uncensored mode. 

This is weird though. Pulling the remote backwards definitely applies the brakes. So it's just having a problem supplying power forward. It freewheels fine, just doesn't spin the motors.
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-17T04:32:56.607Z Reads: 38

```
plugging them in should **not** affect bldc tool. Are you sure the wires in the right place? Maybe you're shorting something out when plugging it in... If you do leave them out and have it in sensored mode, it definitely wont run.

You should probably also post a pic of your motor tab as well
```

---
## \#11 Posted by: meercat Posted at: 2016-11-17T04:47:02.892Z Reads: 39

```
I agree. There has to be something weird going on. I was able to get it to connect to BLDC for a short while even with the sensor wire plugged in, but when I tried clicking "start detection" the motor gave a little lurch and stopped and the VESC disconnected and now it won't reconnect unless I disconnect the sensor wire. Here's my motor tab. <img src="/uploads/db1493/original/3X/b/6/b65393cf9dd8892f426cacc2285d418543a74036.png" width="690" height="356">

And here's all the physical connections themselves.
<img src="/uploads/db1493/original/3X/f/4/f48966538d0fcc2cc84f0eb884115a7d3cf346a2.jpg" width="690" height="388">
```

---
## \#12 Posted by: Jinra Posted at: 2016-11-17T04:53:47.131Z Reads: 34

```
Your sensors are plugged into the program/debug port.. the hall sensor port is under the red/black power cables in your picture. You'll want to make sure each pin is also in the right spot as they're not usually in the right spot from the factory.

I mean the motor tab not the BLDC tab. Also your motor wires should be facing the opposite direction and 'U-turning' back into the enclosure if you want them to last.
```

---
## \#13 Posted by: meercat Posted at: 2016-11-17T04:58:51.303Z Reads: 33

```
MANY thanks! I didn't even notice the port under the power cables. I was planning to turn the motors so the wires face the other direction, but was trying to figure out how to get the parts all working first. I'm guessing this will do it. I'll try and report back. Thanks again.
```

---
## \#14 Posted by: Jinra Posted at: 2016-11-17T05:00:46.116Z Reads: 31

```
no problem, just make sure you plug in the vcc,gnd,temp, and sensor wires in the right order. The three sensor wire order doesn't matter but the vcc,gnd, and temp do.
```

---
## \#15 Posted by: meercat Posted at: 2016-11-17T05:38:55.757Z Reads: 25

```
Thank you! Looks like things are working now as expected. I had to play around with the BLDC settings a bit, but things look good. Thanks again so much.
```

---
