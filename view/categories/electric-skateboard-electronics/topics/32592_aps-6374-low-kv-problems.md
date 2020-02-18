# APS 6374 low KV problems

### Replies: 17 Views: 785

## \#1 Posted by: Takis Posted at: 2017-09-08T05:20:13.662Z Reads: 125

```
Hello everyone , I have a Alien Power Systems 6374 60KV motor and I use Maytech VESC with 12s , do you have any idea how to tune the the vesc because I have tons of cogging the motor does not even start some times 😢does anyone have the same problem or can help ? Thanks 😁
```

---
## \#2 Posted by: Bloop Posted at: 2017-09-08T06:15:26.661Z Reads: 115

```
Do you mean when you start from stand still ? 

I mean if you give it a little push does it work ? 

also from a fast look on Alien's page they say : MAX VOLT: 10S. Idk tho should be fine with 12 probably :-??

Also post some screenshots from the bldc tool with motor config
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-09-08T06:37:30.410Z Reads: 107

```
60kV is extremely low, even for a hub motor. What kind of gearing are you using?
```

---
## \#4 Posted by: Takis Posted at: 2017-09-08T07:18:08.347Z Reads: 95

```
It's ok with 12s I pedal push first but still no luck 😢
```

---
## \#5 Posted by: Takis Posted at: 2017-09-08T07:22:18.227Z Reads: 94

```
I currently have the system on a ebike with 9t on the motor , it's cogging even if I pedal with the motor , I have a problem that the vesc disconnects from PC when the motor is working and I can't do a proper motor detection ,(I want to make it sensored so it can work perfect without cogging or any other issues but APS 63mm hall sensors are out of stock 😕😕
```

---
## \#6 Posted by: Nordle Posted at: 2017-09-08T07:29:35.108Z Reads: 85

```
Maytech maybe
```

---
## \#7 Posted by: Takis Posted at: 2017-09-08T07:41:45.052Z Reads: 84

```
Hopefully not Maytech cause I don't have money for a new one I already killed one 😉😢
```

---
## \#8 Posted by: TarzanHBK Posted at: 2017-09-08T07:48:26.488Z Reads: 81

```
post screenshots of your vesc settings. Then people are able to help you out
```

---
## \#9 Posted by: Takis Posted at: 2017-09-08T07:59:26.042Z Reads: 76

```
As soon as I get home I will
```

---
## \#10 Posted by: Bloop Posted at: 2017-09-08T08:02:15.084Z Reads: 73

```
if you disconnect the pulleys the motor is working ok or still not working ?
```

---
## \#11 Posted by: Namasaki Posted at: 2017-09-08T15:26:42.491Z Reads: 56

```
You have to get through the motor detection. 
It is not optional. 
Check your phase wires. You may have a bad connection. A cold solder joint is all it takes.
```

---
## \#12 Posted by: Jinra Posted at: 2017-09-08T15:31:05.535Z Reads: 53

```
[quote="Takis, post:4, topic:32592"]
It's ok with 12s I pedal push first
[/quote]

I'm surprised no one mentioned sensors. This sounds like normal behavior for a sensorless setup. You just gotta kick push when you start up.
```

---
## \#13 Posted by: Takis Posted at: 2017-09-08T16:39:48.075Z Reads: 43

```
still not working ! motor barely moves at all :/
```

---
## \#14 Posted by: Takis Posted at: 2017-09-08T16:40:40.111Z Reads: 43

```
i always pedal first it does not have the power to move me otherwise :P
```

---
## \#15 Posted by: Jinra Posted at: 2017-09-08T16:42:13.963Z Reads: 40

```
It does have the power to move you, it just can't negotiate the rotor position since you're not running sensors.
```

---
## \#16 Posted by: jmasta Posted at: 2017-09-08T16:43:29.014Z Reads: 40

```
Post up more of your board specs 

Without knowing them, I blindly suggest you bump up your motor current settings.  90A motor max will give you much better startup torque
```

---
## \#17 Posted by: Takis Posted at: 2017-09-08T17:20:11.291Z Reads: 35

```
 The problem must be in the motor connection , it diassembly the ebike kit and hold the motor with the vesc connected ( mounted not with bare hand) the motor worked for a few minutes ive done the motor detection and i was using the keys *D ,I ,RPM* just to see if it works , i stop and after i went to press the RPM button again and i saw a spark i diassebly the motor but i didnt manage to find any burn , and now its back to the same it makes a tiny sound and still does not move . :/ im tired of that :/  <img src="/uploads/db1493/original/3X/3/8/38c8eee4a22924fa858202ba3d4ed727d28b7b19.png" width="690" height="387"><img src="/uploads/db1493/original/3X/6/e/6e7a8d508881f88fd6e1948c85e187002be5eb4b.png" width="690" height="387">
```

---
