# Why is my motor screeching at high speed

### Replies: 12 Views: 985

## \#1 Posted by: gmcgaffey Posted at: 2016-08-17T02:14:39.007Z Reads: 135

```
when riding around getting up to speed the motor starts to screech. this only happens when using 12s I have a 10s battery and it sounds fine. is this because the motor can't Handel. my setup is a 12s battery with enertion vesc and enertion motor the big one 63 74
```

---
## \#2 Posted by: VladPomogaev Posted at: 2016-08-17T05:25:45.378Z Reads: 118

```
Screeching in the motor is an indicator that the signal to the motor is being pulsed using PWM. You might be hitting a current limit, or the RPM limit on the VESC.
```

---
## \#3 Posted by: gmcgaffey Posted at: 2016-08-17T05:33:38.471Z Reads: 114

```
@VladPomogaev can I turn turn down the power or something. I want to keep using 12s.
```

---
## \#4 Posted by: VladPomogaev Posted at: 2016-08-17T05:34:08.408Z Reads: 111

```
I'm not sure. Play around with it. I don't own a vesc yet :P
```

---
## \#5 Posted by: gmcgaffey Posted at: 2016-08-17T05:34:34.835Z Reads: 109

```
ok thankyou
```

---
## \#6 Posted by: saul Posted at: 2016-08-17T20:05:27.746Z Reads: 84

```
what kind of screech is it? you could configure your pwm so it only goes to 90%ish but thats no fun
```

---
## \#7 Posted by: gmcgaffey Posted at: 2016-08-18T05:07:23.790Z Reads: 74

```
it starts around 75% throttle then fades out.
```

---
## \#8 Posted by: saul Posted at: 2016-08-18T20:17:46.203Z Reads: 66

```
mm whats your gearing? could be working too hard

i'm using a 6374 sk3 12s 14/36 on 97mm clones.... no noise other then the usual bldc hummm.....

did you detect the motor correctly or just use the preprogrammed setting from enertion?
```

---
## \#9 Posted by: gmcgaffey Posted at: 2016-08-18T21:29:22.733Z Reads: 59

```
my gearing is 15 tooth motor gear and 36 tooth wheel. it's an enertion motor 6374
```

---
## \#10 Posted by: saul Posted at: 2016-08-18T22:02:46.220Z Reads: 57

```
mmm hard to say without more detail.. maybe just a bad motor...
```

---
## \#11 Posted by: gmcgaffey Posted at: 2016-08-18T22:30:31.105Z Reads: 59

```
I think it's fine if rode 20 miles and it kind of makes the noise then dies out
```

---
## \#12 Posted by: Tijmen Posted at: 2016-11-10T15:15:00.767Z Reads: 36

```
Any update on this? I have the same issue of it screeching at about 70% throttle but being fine below and above that.
Here's a video of my issue:
https://www.youtube.com/watch?v=3enCgApUqK0
```

---
