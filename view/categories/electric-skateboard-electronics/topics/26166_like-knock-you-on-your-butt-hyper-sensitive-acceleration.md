# Like knock you on your butt hyper sensitive acceleration

### Replies: 16 Views: 1071

## \#1 Posted by: Bluecro Posted at: 2017-06-25T22:59:45.784Z Reads: 216

```
Battery: Two 5000 mah, 6S, 20C in series. I carry two sets while riding.
Theoretical top speed is 32 Km, my first run I had it up to 26 Km, but i wasnt pushing it.
Two Motors 6374 190KV 3150 W
Two TORQUE ESC VESC Electronic Speed Controller enclosed in a vented Pelican box.
Trampa trucks.
TorqueBoards 2.4ghz Nano Remote Controller.

Board rides good but I have a couple of issues. The breaking is too strong so i decreased the amount of motor min amps. 
The other issue im having is the throttle, its too sensitive, like really sensitive, like knock you on your ass sensitive. Do you guys of any suggestions on programming or adjusting for smooth acceleration? Any thoughts would be much appreciated.
```

---
## \#2 Posted by: Eboosted Posted at: 2017-06-25T23:04:14.954Z Reads: 206

```
What remote are you using?
```

---
## \#3 Posted by: gee Posted at: 2017-06-25T23:10:01.479Z Reads: 199

```
configure your vesc maybe?
```

---
## \#4 Posted by: wafflejock Posted at: 2017-06-25T23:14:11.154Z Reads: 197

```
What control mode are you using in the VESC configuration?  Also check the remote input display to make sure the min and max ms values are set correctly for the top and bottom end and that the deadband is big enough in the middle to avoid easily creeping into the acceleration zone.
```

---
## \#5 Posted by: Jinra Posted at: 2017-06-25T23:16:20.887Z Reads: 187

```
If you're using the Nano v2 remote, see here for exactly why this is happening

http://www.electric-skateboard.builders/t/correct-foc-settings-controller-bugging-out/26156/8?u=jinra
```

---
## \#6 Posted by: Bluecro Posted at: 2017-06-25T23:33:56.187Z Reads: 181

```
TorqueBoards 2.4ghz Nano Remote Controller.
```

---
## \#7 Posted by: Bluecro Posted at: 2017-06-25T23:55:06.006Z Reads: 173

```
Set for current no reverse with brake. I checked the ms. on the main vesc its was good, on # 2 vesc was not set properly, Set to #1 specs.
Deadband is set to 0.15. Is that ok?

I decreased the motor max amps by 10 amps. havnt tested yet.
```

---
## \#8 Posted by: wafflejock Posted at: 2017-06-26T00:21:29.700Z Reads: 160

```
Yeah mode is good then I only have 1 VESC so can't speak to the two VESC setup or config at all really.  Regarding the deadband you just want to shake your remote around a bit and see how much the percentage drifts from center, if you have it set at .15 that's basically 15% from what I gather so 7% above the 50 and 7% below it will ignore and starts using values between the 57-100 range or 43-0 range for acceleration or deceleration.  That should be fine but you can either make it smaller to make it more responsive or larger to make it not respond to the small squeezes or pushes.
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-06-27T09:38:56.942Z Reads: 129

```
The Nano remote is not safe to use, there are lot´s of issues with it.
Get a proper Mini or a GT2B modded.
```

---
## \#10 Posted by: Bluecro Posted at: 2017-06-28T06:47:10.663Z Reads: 103

```
Thank you for the info waffejock, appreciate it.
```

---
## \#11 Posted by: Bluecro Posted at: 2017-06-28T06:48:55.295Z Reads: 102

```
Vesc set to BLDC mode.
```

---
## \#12 Posted by: Jinra Posted at: 2017-06-28T06:49:42.299Z Reads: 104

```
Did you mean to reply to me?
```

---
## \#13 Posted by: Bluecro Posted at: 2017-07-09T06:43:43.356Z Reads: 79

```
yes thanks for your help
```

---
## \#14 Posted by: almogu Posted at: 2017-09-05T19:46:47.313Z Reads: 69

```

Hi, it's the same thing to me, when I accelerate a little, it's like I'm doing the full tour, but the same thing happens to me with the nano remote, as with an RC station. I do not know what the solution is, I've looked at parameters but I do not know what it can be. by the way, what is the switch that leads to the middle of the command ???
```

---
## \#15 Posted by: Bluecro Posted at: 2017-09-06T06:03:30.434Z Reads: 57

```
You have to calibrate the remote every ride. Look at Jinra's comment. Not sure what your referring to ???
```

---
## \#16 Posted by: almogu Posted at: 2017-09-07T19:24:04.269Z Reads: 38

```
the route does it well, because in the bldc tool's display, you see the center point that is 50% and the maximum and minimum values ​​are set with ppm max and min values. I read the comment, probe has done it and nothing. I read in another section the same thing that happens to me. if I accelerate a 1/3 of the command is 100%
```

---
