# Vesc 6 Problem. Plese Help

### Replies: 6 Views: 183

## \#1 Posted by: vitaswww Posted at: 2019-08-22T12:29:12.644Z Reads: 72

```
Hello. Sorry for my English)
I have a problem with a couple of my Vesc6. When I go 10-15 km / h without acceleration and press on the accelerator, my Vescs first give a sharp braking impulse and only then accelerate. At speeds above 15km \ h this is not. It knocks me down sometimes, I don’t know how to fix it. 2x Vesc 6 With Can connection. 10s7pBat
60 BatA
75 MotorA
190kv motors
Ppm flipsky controller
```

---
## \#2 Posted by: vitaswww Posted at: 2019-09-11T15:57:41.029Z Reads: 42

```
Anybody can help me?
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-09-11T17:47:56.441Z Reads: 35

```
It sounds like you just need to do ppm calibration?

Try that, and send us pictures of the best tool. Show stuff like your battery and motor Max and min
```

---
## \#4 Posted by: Darkie02 Posted at: 2019-09-11T17:53:23.727Z Reads: 34

```
Try recalibration your motors sensors if you useing them. by default thay work at slow rpm not high rpm. Could be a cause of them been out slightly
```

---
## \#5 Posted by: trampa Posted at: 2019-09-11T17:56:59.283Z Reads: 33

```
Clone ESC or VESC SIX?
```

---
## \#6 Posted by: Stupidspencer Posted at: 2019-09-14T17:08:11.120Z Reads: 23

```
I have experienced this, and found a way to eliminate it.  Just to be sure its the same symptoms, I will describe the problem from my experience. You are riding at some fraction of full speed, and release the throttle. Then you give it just a tiny little bit of throttle as you are coasting down. At the moment you move your throttle control (in the acceleration direction), a quick, hard braking action is experienced.
I only use the Android version of VESC tool with the bluetooth link, so my descriptions of where the following settings are located is for the Android version. But I think you will find them in the Windows version easily regardless.
There are several settings in VESC tool that can help eliminate this. First setting to check is "input deadband" which will be in app config --> PPM --> Mapping.  The default value is 15% which means that the first 15% of throttle trigger movement is ignored. Increased value means you will need to move your throttle farther from center before the VESC reacts. If the problem is due to a noisy PPM signal or a less-than-perfect throttle potentiometer in your transmitter, increasing this setting is likely to solve the problem. In my case, I turned this setting down to 5% and began experiencing the problem you describe. So I turned it up to 12% and this eliminated the problem for me.
The other setting to try is the "median filter" found in app config --> PPM --> general. This setting will establish a buffer of throttle commands, and ignore commands that are well outside of the median value of the data in the buffer. This setting is enabled by default, and will also introduce a slight delay to the throttle response (about 200ms roughly). Personally, I hate the delay, so I have it turned off. But I also shielded my PPM cable and isolated the RC receiver from EMF interference by putting it in its own grounded metal box so that I could safely disable that function.
BTW @trampa, I can't speak for the OP, but I am using 2 CANbus connected original VESC6+s that I bought from... You! And I'm using VESC tool v1.19 (Android) and firmware 3.61

Edit: May also be helpful to know that my radio system is a Turnigy GTX3
```

---
