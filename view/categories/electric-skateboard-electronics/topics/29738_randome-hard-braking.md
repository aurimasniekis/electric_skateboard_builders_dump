# Randome hard braking

### Replies: 17 Views: 912

## \#1 Posted by: filipandre95 Posted at: 2017-08-04T22:23:35.549Z Reads: 114

```
After trying to climb a steep hill with my e-board and power just cut off, my board very often randomly breaks a very short moment. I thought it was the phase wiers so I solderd new bullet connectors between the motor and the VESC. This didnt help. I can also feel a loss in power wich I dont understand...
My setup:
VESC 4.12
Motor: 1x Alienpower 63mm 3,3KW
Battery: Alienpower 18650 pack, 12s3p
Remote/reciever: Alienpower
Enertion trucks.

I can also tell that I had no problems with the board before this.
```

---
## \#2 Posted by: saul Posted at: 2017-08-04T22:29:04.002Z Reads: 113

```
redo motor detection. I've had vesc reset to default. they still work but no real power.

check your rx wires, could be coming loose.
```

---
## \#3 Posted by: Jinra Posted at: 2017-08-04T22:33:11.461Z Reads: 106

```
what's your minimum voltage and battery cutoffs on the vesc?
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-08-04T22:33:24.664Z Reads: 105

```
You best bet is a connection loss of your remote. So maybe Check if it helps to Position the receiver somewhere else abd Check the wires.
```

---
## \#5 Posted by: filipandre95 Posted at: 2017-08-05T20:19:24.288Z Reads: 77

```
@Jinra  Minimum input voltage: 8V
Battery cutoff start 10V, End 8V
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-05T20:29:34.687Z Reads: 71

```
Could you post the rest of your vesc settings preferably in the form of a screenshot. make sure to include all tabs
```

---
## \#7 Posted by: filipandre95 Posted at: 2017-08-05T20:29:51.622Z Reads: 71

```
@saul Did it and it had not changed
```

---
## \#8 Posted by: filipandre95 Posted at: 2017-08-05T20:33:43.821Z Reads: 68

```
[https://gyazo.com/d40ed63bb98d72e514e67458cb1a0cea](https://gyazo.com/d40ed63bb98d72e514e67458cb1a0cea)
[https://gyazo.com/83f1a6fd45afe583857d9ff769b05b52](https://gyazo.com/83f1a6fd45afe583857d9ff769b05b52)
[https://gyazo.com/5d86a10010d3ff3e66ddcb192bbabb8f](https://gyazo.com/5d86a10010d3ff3e66ddcb192bbabb8f)
[https://gyazo.com/63fedfe8245fe8071e7c6997182bb526](https://gyazo.com/63fedfe8245fe8071e7c6997182bb526)
[https://gyazo.com/4ec13d714a3d75a567d282a28c5382cf](https://gyazo.com/4ec13d714a3d75a567d282a28c5382cf)
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-05T20:40:47.776Z Reads: 63

```
I don't see any settings that are that off. However, your max current ramp step in the advanced tab is 10x higher than it is by default. You may have a buggy 2.18 firmware which you may want to re-flash with a fixed one. 

See here

http://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262?u=jinra
```

---
## \#10 Posted by: filipandre95 Posted at: 2017-08-05T20:50:54.994Z Reads: 61

```
Is there a link to the latest 2,18 version FW?
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-05T20:55:13.763Z Reads: 59

```
http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/
```

---
## \#12 Posted by: JTAG Posted at: 2017-08-05T21:35:44.819Z Reads: 52

```
This happens when ESC power is lost OR when one phase wire had an intermittent connection.

Can you share a picture of your setup / soldering?
```

---
## \#13 Posted by: filipandre95 Posted at: 2017-08-05T22:05:22.554Z Reads: 48

```
@Jinra Thats the one I have  :confused:
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-08-05T22:08:29.457Z Reads: 47

```
Your problem comes from the remote. It losses connection for a short while. Or the signal from the Potentiometer jitters. Just switch everything on and give a little throttle on the bench. Then shake the remote and squeeze it a little. If you have losses it is clear where your issue is coming from. These are the short hickups you experience.
```

---
## \#15 Posted by: filipandre95 Posted at: 2017-08-05T22:13:21.936Z Reads: 43

```
@Ackmaniac
 I will try and use my other RC remote and see if it works better, if It does then I change it :)
Thanks!
```

---
## \#16 Posted by: Silverline Posted at: 2017-08-06T10:10:56.457Z Reads: 37

```
Had the same sort of problems. Sometimes i lost power for a second going op a hill, and two times when braking, the board suddenly stops braking for a moment. Changing my remote, to a GT2B,  seems to have fixed my problems (knocking on woods) so far.
```

---
## \#17 Posted by: filipandre95 Posted at: 2017-08-06T14:00:53.050Z Reads: 31

```
Thats the exact remote im using now and it solved my problem. Im greatful it was as simple as that :)
```

---
