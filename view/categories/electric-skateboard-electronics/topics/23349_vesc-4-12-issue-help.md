# VESC 4.12 issue, help!

### Replies: 8 Views: 635

## \#1 Posted by: MysticalDork Posted at: 2017-05-18T02:33:20.938Z Reads: 72

```
Hi folks! Long time lurker here, finally made an account to reach out to the community for a little bit of help. I'm nearly done with my second build, a dual rear with pneumatic tires (build thread to come once finished) and I'm having strange issues with the two DIYElectricSkateboard 4.12 VESCs I'm using in it. I've successfully set parameters and even done a small shakedown run with them, but now that I'm tweaking for final assembly, I'm getting weirdness.

When I plug in the loop key, everything powers up, all seems well. I squeeze the GT2B trigger, the wheels spin. If I keep the motors spinning for ~30 seconds, both stop, and will not start again. Motor detection also only works once or twice, then refuses to work again. If I unplug the loop key and let everything sit for 20 minutes, I can get the same response again. It almost behaves like the VESCs are overheating, but everything is stone cold.

I'm running 10s with 6354 motors. I have the current limits, voltage limits, ERPM limits etc set correctly, the damn thing just seems to go on strike after 30 seconds. Has anyone experienced this? Does anyone know how to fix this?

I'm definitely upgrading to a VESC 6 ASAP, just for peace of mind, but in the meantime, it would be really nice to ride the board I just built.

Thanks in advance!
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-18T02:43:23.394Z Reads: 68

```
I'm sure it's a setting in the VESC or maybe a loose solder joint. Polar some screen shots of your settings and of your setup. This helps us help you.
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-05-18T02:55:51.793Z Reads: 66

```
I'll go grab a couple photos of the current setup. I had to re-heatshrink the VESCs, so the boards aren't visible.
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-05-18T03:04:12.813Z Reads: 63

```
@JLabs  Here you go. Everything is kludged together and messy right now, need to spend some time making it nice once it works.<img src="/uploads/db1493/original/3X/e/c/ec7017105198de5a0a9db3b150e0724215b95e61.jpg" width="689" height="388"><img src="/uploads/db1493/original/3X/a/d/adfc689a808b9ff44ac9930fec4463bf0bae8ded.jpg" width="690" height="388">
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-05-19T02:04:34.040Z Reads: 49

```
@JLabs   OK, new information: I went into the terminal of BLDC tool and searched for faults, it appears I'm getting an overtemp error, even when everything is cold. Could I have a miscalibrated temperature sensor? Under realtime data, the MOSFET temperature is reading over 100 degree, but that's obviously wrong because I can't feel any heat from them at all.
```

---
## \#6 Posted by: Michael319 Posted at: 2017-05-19T03:20:27.135Z Reads: 44

```
It must be the temp sensors. Did you make the Vesc yourself?
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-05-19T04:13:48.819Z Reads: 41

```
No, I bought them from  back in March. I just ran across a thread with several people who had identical issues to mine from the same batch. Since I want to have it working and not sent back, I currently have just raised the thermal limits to compensate for the offset. I will be ordering replacement sensors and soldering them myself later, but for now, I'm just happy to have a working board.

Unrelated: First time with hall sensors and FOC. Unbelievably smooth, it's almost unreal.
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-05-23T05:39:25.338Z Reads: 32

```
ANNNDDDDDD.... I've killed both DRV chips. Damn you FOC, so smooth, so dangerous. While doing a shakedown ride, both speed controllers locked up mid-acceleration and went to full brake, throwing me smack in the middle of crossing the street.

 Just ordered two VESC 6.0s, I'm a little too wary to ride something that can kill the DRV chips that easily.
```

---
