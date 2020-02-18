# Is my setting OK

### Replies: 10 Views: 213

## \#1 Posted by: AutoCar Posted at: 2019-09-18T06:22:24.376Z Reads: 62

```
I am using Focbox on an RC car and then drive it with a computer. You can find some pictures here. https://twitter.com/SmallpixelCar/status/1162240910928650242  The computer continuously sends speed and steering command to the VESC to navigate. If the computer stops sending the messages, the car would stop. I found if the car ran above 15 mph however, it could not stop immediately even  the computer halt sending messages. The car would still run but at a slower and slower speed. I tried two Focbox, they both had the same issue. I checked my computer software but did not find any issue. So I am guess my Focbox setting was not correct. I also noticed that when I ran "Detect motor", it failed. My BLDC tool is 4.12 and firmware is 2.18. Below are pictures of my VESC settings. Could anyone help what is wrong?

![p1|690x418](upload://y7Ld9QUaT6zgm1Kl06fBRa7ghJc.png) ![p2|690x423](upload://tebTrERAtYkf1uNn5T3nh8zO2D2.png) ![p3|690x429](upload://rJbtmJMM5NWFvGRgsObnFKksaNB.png)
```

---
## \#2 Posted by: olestra Posted at: 2019-09-18T15:02:11.135Z Reads: 48

```
[quote="AutoCar, post:1, topic:101930"]
it could not stop immediately even the computer halt sending messages
[/quote]

okay -- this is unclear. computer sending a 'halt' or computer no longer sending any? two very different scenarios

If a halt message was sent, then look at your ramp settings. 
If no messages sent, then look at the 'app settings' tab for timeout and timeout brake current.
```

---
## \#3 Posted by: AutoCar Posted at: 2019-09-19T03:54:16.754Z Reads: 39

```
[quote="olestra, post:2, topic:101930"]
computer no longer sending any
[/quote]

I meant to say "computer no longer sending any". 

What should I look for in the "App settings" tab?
```

---
## \#4 Posted by: olestra Posted at: 2019-09-19T14:50:52.550Z Reads: 33

```

timeout and timeout brake current.
 timeout is how long it waits before it decides it has lost signal, and timeout brake current is how hard it puts on the brakes once signal is lost.
```

---
## \#5 Posted by: AutoCar Posted at: 2019-09-19T16:47:45.270Z Reads: 28

```
@olestra Thank you very much for the information. "Lost signal" means "No control signal from user" so the VESC need to decides what to do, correct? 

In my software, I always send signal to VESC. If I want it to stop, I just send speed=0. Is this considered "Signal"?
```

---
## \#6 Posted by: olestra Posted at: 2019-09-20T17:42:30.114Z Reads: 19

```
speed = 0 would be a continuous signal if using pwm controls, if using uart, or can-bus, I'm not sure -- you'll need to dig into your control library to see if what it's actually sending.

with pwm, a speed=0  would be no forward motion, but also no brakes. depending on how you have the esc setup to respond.

in the app tab, look at what control type you are using. if you are using PWM, and have no need of reverse, map your speed range (0-100?) to the full range of normal pwm signal. and set the pwm settings to something like 'current, no reverse' that would set 0 to be full brakes, 50 to be coasting, and 100 to be full forward.

If  you are using pwm and need reverse, you'll need to set negative speed until your device comes to a halt. once it's halted, then speed=0. if you do reverse+brakes on the app settings, pwm controls... you just made programming a bit more complicated. you would need to set speed to be something negative, then 0 then negative again to go from moving forward to moving in reverse.
```

---
## \#7 Posted by: AutoCar Posted at: 2019-09-20T23:03:13.579Z Reads: 13

```
I am using "No App". I actually do not know what that means
```

---
## \#8 Posted by: AutoCar Posted at: 2019-09-20T23:04:34.482Z Reads: 14

```
My currently setting is like this. Not sure if this is OK
![motor|690x421](upload://nUhbbu7bKGGmBwwcQBQrm7iipCM.png)
```

---
## \#9 Posted by: AutoCar Posted at: 2019-09-20T23:12:22.523Z Reads: 17

```
@olestra
Please ignore my previous post. I am accutually using "PPM and UART"
![App|690x428](upload://t8EGtpkEce8nkln3vt4jgBm4cCE.png)
```

---
## \#10 Posted by: olestra Posted at: 2019-09-23T14:57:47.045Z Reads: 7

```
okay -- Is your controller sending via uart or ppm? (ppm is the same as pwm for this discussion)

I suspect it is, and that you are receiving telemetry back via uart. If this is the case, then you need to look at the ppm tab under app settings. So that you can figure out what you need to send to apply brakes.

if your controller is using uart, then you'll need to look at the library you are using to find out hoe to do that.

Basically I think the issue is that you aren't hitting the brakes, you are taking you foot off the gas, to use a car analogy
```

---
