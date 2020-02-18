# X car beast120a esc

### Replies: 20 Views: 1116

## \#1 Posted by: charliek Posted at: 2017-02-23T02:34:13.361Z Reads: 144

```
So I've been using x car beast 120a esc with 280kv motor. Out of sudden, esc is not able to detect the motor (red and blue light flashing). I thought that cold soldering joints might have caused the problem so I soldered the wires directly. Esc still can't detect the motor. what else could I try?
```

---
## \#2 Posted by: lowGuido Posted at: 2017-02-23T03:06:51.964Z Reads: 135

```
check your connection to the receiver isn't broken.
once you have fixed that re calibrate the ESC.
```

---
## \#3 Posted by: charliek Posted at: 2017-02-24T01:01:09.075Z Reads: 114

```
It's really weird. It connected once after all but it stopped working again.
```

---
## \#4 Posted by: lowGuido Posted at: 2017-02-24T03:41:21.233Z Reads: 103

```
Did you make sure your PWM wires are good? Have you tried a different one?
```

---
## \#5 Posted by: charliek Posted at: 2017-02-24T03:57:45.938Z Reads: 95

```
sorry but what are pwm wires?
```

---
## \#6 Posted by: goldenHusky Posted at: 2017-02-24T12:42:09.235Z Reads: 90

```
@charliek he probably means the wires from the receiver to the esc, I think they are ppm, but anyway :yum: :joy:
```

---
## \#7 Posted by: Vieo Posted at: 2017-02-24T15:31:13.527Z Reads: 81

```
What remote are you using? I had purple light for a while and that was due to the RC remote
```

---
## \#8 Posted by: lowGuido Posted at: 2017-02-24T15:44:07.419Z Reads: 80

```
PWM = Pulse Width Modulation
PPM = Pulse Position Modulation 

our RC transmitters use Pulse Width Modulation to control throttle. typically a width of 1ms to 2ms. 
but yeah I mean the white wire.
```

---
## \#9 Posted by: FinnishSnowmobiler Posted at: 2017-02-24T19:08:25.100Z Reads: 73

```
I had the same ESC. Have you tried to recalibrate the motor with the receiver?  

I've already ordered the VESC since the X-CAR 120A ESC makes so horrible noise when braking and can't withstand full throttle without cogging...
```

---
## \#10 Posted by: Montiey Posted at: 2017-02-24T19:19:14.877Z Reads: 73

```
PWM is the single-channel, 1000-2000 microsecond protocol. PPM (sometimes called CPPM) is multiple channels mashed together, using the same 1-2 millisecond protocol for each. As far as I know, the VESC only handles one channel over the servo connector, so I _guess_ we'd call it PWM, no? In BLDC Tool it says PPM, anyways.

You might want to recalibrate the signal range from the receiver, so raise the throttle to MAX, then plug in the battery to the ESC. You should get some noise, so then lower the throttle to MIN.

If there really is a problem between the ESC and the motor, this won't help, but it's a common problem so i'd try it first.
```

---
## \#11 Posted by: charliek Posted at: 2017-02-25T13:19:00.582Z Reads: 63

```
I'm using torquebaords remote
```

---
## \#12 Posted by: charliek Posted at: 2017-02-28T05:50:08.315Z Reads: 59

```
Does vesc not make any noise when it brakes?
```

---
## \#13 Posted by: charliek Posted at: 2017-02-28T05:50:30.000Z Reads: 58

```
Problem solved! thank you!
```

---
## \#14 Posted by: FinnishSnowmobiler Posted at: 2017-02-28T07:06:34.592Z Reads: 55

```
That's what I've understood. I guess it can't be completely silent but X-CAR's noise is a programmed feature which I hate...
```

---
## \#15 Posted by: lowGuido Posted at: 2017-02-28T08:59:10.112Z Reads: 49

```
The VESC is completely silent under brakes.
```

---
## \#16 Posted by: evilboarder Posted at: 2017-02-28T09:53:36.422Z Reads: 44

```
how did you solve your problem? i have the same esc and having similar problems with it
```

---
## \#17 Posted by: charliek Posted at: 2017-02-28T11:34:20.197Z Reads: 44

```
I did what @Montiey suggested. I recalibrated throttle range.
```

---
## \#18 Posted by: charliek Posted at: 2017-02-28T11:44:05.554Z Reads: 42

```
Interesting. Do you know why they deliberately programme car escs to make noise?
```

---
## \#19 Posted by: lowGuido Posted at: 2017-02-28T11:48:38.196Z Reads: 43

```
I can only assume it is because they wanted a screech for rc cars to sound more realistic. 
Only an assumption.  I don't really know.
```

---
## \#20 Posted by: FinnishSnowmobiler Posted at: 2017-02-28T12:08:51.709Z Reads: 41

```
You can't disable the noise by programming. Maybe it could be done by removing the origin of sound but that would require some research.
```

---
