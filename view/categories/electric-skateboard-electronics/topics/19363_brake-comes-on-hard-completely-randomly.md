# Brake comes on hard completely randomly

### Replies: 15 Views: 1354

## \#1 Posted by: yakerman Posted at: 2017-03-20T18:34:52.193Z Reads: 172

```
So I finished my 1st build about a week ago and have spent the time fine tuning it and getting used to riding. I've had one big issue the whole time which I cant seem to figure out.

At what seems to be completely random times whilst riding the brake will just engage on full power stopping the board dead. Its been at relatively low speeds  and I thought It had gone but today It happened again and I went flying. Not ideal. I'm fine but its a bit disconcerting and I want to get it fixed before I take it out again. 

Its happened maybe 4 or 5 times. Does anyone know what might be causing something like this? I think it could be a loose connection but they all seem good so I'm a bit stumped. 

Its a single motor 8s VESC setup.
```

---
## \#2 Posted by: treenutter Posted at: 2017-03-20T18:41:45.798Z Reads: 164

```
@yakerman pls post screenshots of your BLDC Tool settings (and maybe photos of your build). I'm guessing that you need to check the voltage cutoff limits. It sounds you're triggering a reboot because of voltage sag while you accelerate. 

It could also be an adjustment you need to make to your PPM settings... maybe the trigger is not calibrated and it is randomly engaging the brakes.
```

---
## \#3 Posted by: yakerman Posted at: 2017-03-20T18:57:01.235Z Reads: 160

```
<img src="/uploads/db1493/original/3X/1/e/1e6b949580d86d172c078b42c21d02c41a948cbc.png" width="690" height="393">

<img src="/uploads/db1493/original/3X/c/1/c16aacda9bba760276b2c92e7c5953bb71a737c3.png" width="690" height="389">

<img src="/uploads/db1493/original/3X/0/8/0851b469ec3f4d514e6d1805b7d8057aa6551fc6.png" width="690" height="395">

<img src="/uploads/db1493/original/3X/7/c/7c1354df82dab68f0405b82585b2dbf0014a8d1b.png" width="690" height="387">
```

---
## \#4 Posted by: Stefan Posted at: 2017-03-20T19:16:01.449Z Reads: 139

```
What remote do you use? Maybe you are losing connection sometimes and the vesc engages the failsafe function
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-03-20T19:17:20.284Z Reads: 140

```
First of all you have the max current ramp step bug. So you should upgrade your firmware. 
Secondly please connect the vesc to your PC and have a look at the ppm tab. As in your Screenshots I can  see that the ppm signal is good. But what happens when you switch off your remote. Does it stay at 1.55 pulse width or does it go much lower. If that is the case then you have remote connection dropouts and then the vesc thinks you brake. Because when the receiver doesn't find the remote it goes back to the default pulse width.
```

---
## \#6 Posted by: yakerman Posted at: 2017-03-20T19:26:52.011Z Reads: 134

```
Okay, I just turned off the remote whist connected and it stayed at 1.55. I'm using the mini remote btw. I'll upgrade the firmware too.
```

---
## \#7 Posted by: jm.riviere Posted at: 2017-04-22T07:03:18.045Z Reads: 107

```
I have the exact same problem, any news? Did updating the firmware change anything, or did you change something else? 
Thank you very much in advance
```

---
## \#8 Posted by: yakerman Posted at: 2017-04-22T09:20:44.932Z Reads: 99

```
I do seem to have fixed it but I made a few changes and I'm not sure exactly what the cause was or which change was the solution but this is what I did. I think it Treenutters theory about voltage sag was the most likely.
- Updated to Ackmaniac's firmware (which is awesome) 
- Switched to FOC (just because I fancied it, I'm not sure this will help)
- Changed the Batt Max to 40. I think this is what stopped the problem but I did notice a reduction in power. I have since changed up back up to 50 and its been fine. 
- Increased the Motor max to 70 because I read this would help with startup torque. I noticed a slight increase.

Let me know how you get on I'm interested to know what you do to solve this.
```

---
## \#9 Posted by: yakerman Posted at: 2017-04-22T09:22:23.826Z Reads: 97

```
Oh yeah I'm also running in Watt mode now
```

---
## \#10 Posted by: jm.riviere Posted at: 2017-04-22T21:37:56.002Z Reads: 85

```
Ok cool I'll try all of this and will keep you updated! 
I read about Ackmaniac's Watt Mode, but didn't dare to upgrade my Vesc firmware because of all the warnings. Worth the shot in your opinion?
```

---
## \#11 Posted by: yakerman Posted at: 2017-04-22T22:05:51.507Z Reads: 78

```
I would definitely recommend Ackmaniac's firmware and Watt mode. Super easy to upgrade to. As for FOC I didn't have any issues myself but obviously lots of people have. It is good though! 

One other thing I would check are your motor phase wires. I think if there is a loose connection with those then it will cause a similar problem.
```

---
## \#12 Posted by: Michaelj1 Posted at: 2017-07-17T17:16:23.892Z Reads: 71

```
I'm having a very similar issue. My board will randomly slam the brakes on while I'm riding it. I'm running a 6s (2x 3s 5000mah 40c batteries in series) setup, with dual 270kv motors and dual VESCs. Any chance anyone could help me out?
```

---
## \#13 Posted by: Michaelj1 Posted at: 2017-07-18T13:07:14.569Z Reads: 61

```
Since it appears that both motors slam on the brakes, I've narrowed it down to either the parameters for the remote not being set up correctly, the remote itself, or the VESCs not getting enough voltage so they reboot
```

---
## \#14 Posted by: Michaelj1 Posted at: 2017-07-20T02:01:52.883Z Reads: 48

```
Yeah so it turns out one of the motors had a bad solder connection and was locking up randomly... the system figured out one motor wasn't spinning and siezed up I think. I just hope getting a replacement motor fixes the problem. Will keep you guys posted
```

---
## \#15 Posted by: jm.riviere Posted at: 2017-07-31T17:43:34.419Z Reads: 35

```
Sorry for the late reply! In my case, it was very obvious, I super stupidly connected the 4mm motor wires to the 5.5mm from the VESC (good intuition, @yakerman) . Soldered the bigger connectors and it has been running without a hiccup since then! 
Will try installing WATT mode in the next few days :slight_smile:
```

---
