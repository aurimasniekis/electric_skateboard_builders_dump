# VESC &#124; First time VESC configuring some questions

### Replies: 6 Views: 753

## \#1 Posted by: thylen11 Posted at: 2017-03-11T18:27:02.649Z Reads: 139

```
Hey all,

I bought myself a VESC and hooked it up to my PC and configuered it as best as I could. However I'm scared to death I made a mistake and end up blowing my precious student money so therefore I'd like to ask some of the Vescterans (pun intended) to maybe look at it and tell me if I did something wrong.

My battery: 6s2p https://hobbyking.com/en_us/turnigy-5000mah-1s-20c-lipoly-single-cell.html
My motor: SK3 320KV https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-320kv-brushless-outrunner-motor.html

My configuration: 
<img src="/uploads/db1493/original/3X/d/6/d6fce77e90f23d7d415ecc23a350fb387cfdffa7.jpg" width="690" height="366">

Im stoked to get my first ride in with the VESC! Thanks in advance :D
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-03-11T18:45:19.156Z Reads: 125

```
Your battery max should be lower or at least equal to your motor max. Try 50 battery max and 60 motor max.
Your maximum input voltage should be 57V.
Set your battery cutoff start to 21.6 and your battery cutoff end to 20.4
And show Screenshots of the bldc, advanced and the controller settings tabs.
```

---
## \#3 Posted by: thylen11 Posted at: 2017-03-11T18:53:54.851Z Reads: 125

```
Thanks you good sir! I changed the things you said. Here is the advanced tap:
<img src="/uploads/db1493/original/3X/4/5/45b8d91e885a0420bcd5e057e24ec8ddaaef56b9.jpg" width="690" height="318">
I didn't dare to change any since the YT tutorials from torque said not to bother if you're a noob like me.
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-03-11T19:05:34.333Z Reads: 111

```
You need to upgrade your firmware because you have the bug where max current ramp step parameter gets multiplied each time you write the settings. Search in the forum for that parameter name, then you will find more information how to upgrade the firmware.
```

---
## \#5 Posted by: thylen11 Posted at: 2017-03-11T19:20:52.330Z Reads: 108

```
Will do thank you so much!
```

---
## \#6 Posted by: Namasaki Posted at: 2017-03-11T22:56:27.057Z Reads: 96

```
The max current ramp step should be 0.04
```

---
