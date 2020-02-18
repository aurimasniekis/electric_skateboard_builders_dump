# Stuttering at higher speeds

### Replies: 12 Views: 968

## \#1 Posted by: brandon Posted at: 2016-11-16T18:22:11.481Z Reads: 107

```
I am experiencing some brief stutters when I get my board up to higher speeds, and it persists on and off after the initial occurrence at lower speeds as well. The stutters almost feel like brake is being applied (stutters are on the order or miliseconds repeating every second or two erratically) rather than the throttle just being cut off due to signal loss, but I could be wrong there.

My setup is as follows:

turnigy sk3 249kv, enertion vesc, series 2x3S zippy 5000mAh, arduino bluetooth ppm controller

I have the vesc setup to cut throttle, not brake on signal loss, but it should always have a signal as my receiver sends a neutral throttle signal upon losing connection to the controller. The only way for vesc to lose signal is power issue with my receiver (I would definitely notice this, takes 4-5 seconds to turn back on) or issue with the signal wire, but again it really feels like brake is being applied for a split second which the vesc is not configured to do.

Any thoughts? What other vesc settings would be useful to check here?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-11-16T19:03:48.170Z Reads: 94

```
Check your phase wires .. make sure the bullet connectors are all in correctly simple things first
```

---
## \#3 Posted by: yaca Posted at: 2016-11-16T19:10:22.653Z Reads: 89

```
What is your max ERPM set? What remote do use?
```

---
## \#4 Posted by: brandon Posted at: 2016-11-16T19:17:39.986Z Reads: 85

```
They look good to me, solder connections solid as well. It's a non sensored motor so it doesn't matter how they are connect right? I did recently reverse a pair so I could have my motor in the front of my board while riding, but I don't think that would make a difference.
```

---
## \#5 Posted by: brandon Posted at: 2016-11-16T19:20:28.349Z Reads: 73

```
I use a phone app paired with an hc06 bluetooth module. It just feeds a PPM signal to the VESC.
```

---
## \#6 Posted by: yaca Posted at: 2016-11-16T19:23:33.256Z Reads: 68

```
Post screenshots of your motor settings, so people can help you easier.
```

---
## \#7 Posted by: brandon Posted at: 2016-11-16T19:39:50.419Z Reads: 64

```
I am not able to access my motor at the moment, but I will as soon as I am able. ERPM should be whatever the default is set to. I only modified a few settings as dictated in the new users guides.
```

---
## \#8 Posted by: brandon Posted at: 2016-11-16T20:44:37.532Z Reads: 57

```
<img src="/uploads/db1493/original/3X/a/a/aa71c0071fdc01e0b5bb9e363119466423d7137f.png" width="690" height="388">
```

---
## \#9 Posted by: yaca Posted at: 2016-11-16T21:37:41.883Z Reads: 53

```
Can not see a problem here. Just for safety set your Max ERPM to 60000. But this will not be the problem. Show also your advanced motor config. You did motor detection?
```

---
## \#10 Posted by: brandon Posted at: 2016-11-17T15:05:11.502Z Reads: 42

```
I did motor detection. The only setting I changed under advanced was to increase the startup boost to .04 from .03 (I think I have the power of 10 correct here) but I will get a screenshot as soon as I am able.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-11-17T17:28:22.405Z Reads: 40

```
Loosing power at high speed can feel like the brakes coming on. 
I would recomend checking your motor phase wire connectors by pulling on them and twisting them to see if the come loose. Sometimes visual inspection isn't enough. I'd also recommend trying a different controller. 
Bluetooth controllers are known to be unreliable. 
2.4ghz is the way to go.
```

---
## \#12 Posted by: yaca Posted at: 2016-11-17T20:49:05.583Z Reads: 32

```
You can type faults in the terminal of BLDC tool right after the stuttering happens (without disconnecting the power since that will reset the fault codes)? That will print all faults that occurred. I'm not sure if dropouts from the receiver/controller are shown as a fault. Maybe someone reads this and can give an answer.
```

---
