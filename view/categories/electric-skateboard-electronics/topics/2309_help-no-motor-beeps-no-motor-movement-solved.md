# Help! No Motor Beeps, No Motor Movement (solved)

### Replies: 12 Views: 1557

## \#1 Posted by: DjPaco397 Posted at: 2016-04-12T11:23:54.516Z Reads: 59

```
First off here is my setup.

-Dual diagonal exertion r-spec motors 
- 2 turnigy trackstar 120a esc'so
- 2 3s 8000mah lipos in series on each motor
- spektrum 2.4ghz tx/rx

Main problem seems to be no input between the esc's and motors. When turning the system on my motors are quiet and do not twitch the slightest. 

So far my transmitter is binded, the throttle calibration worked as per instructions that came with the esc. 

Troubleshooting: I've checked the motors for any visual sign of a short. Used my multimeter to check for continuity between the 3 motor wires which I have. All of my solders appear to be solid, and my BEC harness is plugged into the throttle slot on my reciever. 

At this point I'm kinda out of ideas guys! Hoping a few fresh minds can help me out, will upload pics underneath. Cheers!

<img src="/uploads/db1493/original/2X/8/85e08ffec1068709fb3f19bf3b12ab8ed85c1745.jpg" width="374" height="500">
```

---
## \#2 Posted by: laurnts Posted at: 2016-04-12T11:31:38.396Z Reads: 53

```
Try to control 1 ESC only (remove the RX harness). It could be that you power / damage the receiver because each esc produce power for the receiver. If it gets both power, it could damage the RX module. Try to see if theres light blinking in your RX module, otherwise test with servo tester.
```

---
## \#3 Posted by: lox897 Posted at: 2016-04-12T11:33:56.349Z Reads: 54

```
Please categorise this post. It could go under eboard electronics.
```

---
## \#4 Posted by: DjPaco397 Posted at: 2016-04-12T11:48:46.547Z Reads: 52

```
I've tried running both systems by themselves with no luck either, when I have them both hooked into the rx only one escape supplies power, I removed the 2nd esc's BEC power wire.
```

---
## \#5 Posted by: DjPaco397 Posted at: 2016-04-12T12:33:42.612Z Reads: 49

```
I did have the motors both working previously when my quanum pistol TX lost connection to my previous rx and then would never bind again. Ever since then I can't get the motors to do anything.
```

---
## \#6 Posted by: laurnts Posted at: 2016-04-12T13:12:52.208Z Reads: 42

```
Is there any lights / blink from rx module? try to detatch the rx module from the esc and power the esc. The motor / esc should beep because of on signal input. or might be you have the positive and negative wrong.

You could also try to power single esc with the battery without any connection to rx and motor just to check if your esc is turning on.
```

---
## \#7 Posted by: DjPaco397 Posted at: 2016-04-12T13:30:00.737Z Reads: 43

```
Fairly sure I've tried all of that, but I'll give all of your suggestions another shot when I get home in an hour! I was looking into the esc specs and for battery it reads 2-4 cells lipo. Since I have 2 3s in series (6 cells) could that cause the esc/motor not to recognize the system?
```

---
## \#8 Posted by: laurnts Posted at: 2016-04-12T14:09:20.778Z Reads: 37

```
Ahh yea that it the problem I think. Over voltage cutoff.
```

---
## \#9 Posted by: DjPaco397 Posted at: 2016-04-12T15:06:40.123Z Reads: 35

```
Thanks for helping me think it through man, now I have to decide is 3s will give me enough power and torque or if I should just go ahead and order 2 6s esc's
```

---
## \#10 Posted by: laurnts Posted at: 2016-04-12T15:14:11.107Z Reads: 36

```
Well you will have to test ride 3s first. Actually I like cruising low speed so higher s rating is not something I am looking for besides marketing / once a while thrill factor. I have to say 4s is quite ideal for most care and simpler to construct.
```

---
## \#11 Posted by: DjPaco397 Posted at: 2016-04-12T15:34:51.707Z Reads: 36

```
Only reason I was leaning towards 6s is because I'll be using it in the Virginia islands and their "hills" there are no joke
```

---
## \#12 Posted by: laurnts Posted at: 2016-04-12T16:01:58.912Z Reads: 32

```
It's not really voltage that is required the most for hill climbing, it's more the amps (current) and discharge capability. This also affect the esc that you are using if they are able to handle it. I suggest migrating to VESC as they are more capable handling this type of condition. My motor gets super hot when using this RC grade car esc when hill climbing and not happening with higher spec ESC.
```

---
