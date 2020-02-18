# Need HELP, motor will not run

### Replies: 19 Views: 166

## \#1 Posted by: BrokenGloves Posted at: 2019-04-28T21:31:42.406Z Reads: 60

```
Can anyone please help me, I've had a day of reading manuals, checking connections and scrolling topics on here but I cannot figure out why my motor still won't run. I'm running a Turnigy 6364 190kv motor with a x-car 150a ESC from hobby king and 2 zippy 3ah 5c in series.![IMG_20190428_202704%20(1)|666x500](upload://vVzMG2k1bPBWcXFSIsa26id2NJu.jpeg) ![IMG_20190428_202720|666x500](upload://oodvBmlBTGv4qog8zjkWKoG7jE9.jpeg) ![IMG_20190428_202740|666x500](upload://8bUVsnaJAofztZhp1Z70zx0zOu1.jpeg)
```

---
## \#2 Posted by: linsus Posted at: 2019-04-28T21:32:38.568Z Reads: 57

```
Get a vesc 👍
```

---
## \#3 Posted by: BrokenGloves Posted at: 2019-04-28T21:34:14.570Z Reads: 57

```
any ideas for what I've already got? have i missed something simple with numbers here?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-04-28T22:04:05.838Z Reads: 53

```
photos help champ
```

---
## \#6 Posted by: murloc992 Posted at: 2019-04-29T10:34:10.817Z Reads: 28

```
Did you calibrate the throttle by holding the set butting while turning it on? I had this ESC and it is very picky with neutral PPM signal which is required to hear the beeps of initialization. After the beeps the motor will work. You should get 5 short and 1 long beep when it is on. If you are not getting them, the calibration is incorrect.

I think the first one is brakes, you get a long beep, then acceleration, you get two beeps, the final one is neutral, you get three beeps. Restart the ESC and it will be calibrated.

The manual will help more.

Wait a fucking minute. 10S?

~~It's dead. If you turned the ESC on, it's dead as fuck. 6S max.~~

![image|422x175](upload://bZNx6Z6EcISCj0M7E2wMdj4PFHG.png) 

Get a VESC for 10S.
```

---
## \#7 Posted by: BrokenGloves Posted at: 2019-04-29T11:30:40.803Z Reads: 17

```
Fuck, I thought 2 ~ 6s meant 2 x 6s 
I did initially try it with one battery and got a light but no beeps
```

---
## \#8 Posted by: murloc992 Posted at: 2019-04-29T11:31:11.476Z Reads: 16

```
It's 2 TO 6S. Try to connect to the single 5S. Does it still have fanspin and LEDs? If it is still alive, you will need to use the 5S in parallel to get a 5S 40C 6Ah battery. :slight_smile:
```

---
## \#9 Posted by: BrokenGloves Posted at: 2019-04-29T11:31:53.683Z Reads: 14

```
yeah, fan and led still come on
```

---
## \#10 Posted by: murloc992 Posted at: 2019-04-29T11:32:23.237Z Reads: 15

```
It's still alive. Connect it to a single 5S, connect your receiver, calibrate the throttle and pray. :slight_smile:

I used it with 6S (two 3S 5Ah 20C zippies) and it was quite nice with a single 6365(6364?) at 245kV.
```

---
## \#11 Posted by: BrokenGloves Posted at: 2019-04-29T11:35:28.589Z Reads: 12

```
nothing, it all seems to go well but absolutely nothing from the motor
```

---
## \#12 Posted by: murloc992 Posted at: 2019-04-29T11:35:52.971Z Reads: 11

```
Does it beep 5 times when you turn it on? Did you calibrate the throttle response?
```

---
## \#13 Posted by: BrokenGloves Posted at: 2019-04-29T11:36:49.307Z Reads: 11

```
no beeps at all, and I've binded the controller again but still nothing
```

---
## \#14 Posted by: murloc992 Posted at: 2019-04-29T11:38:43.215Z Reads: 12

```
Not binding, throttle calibration. You hold the set button, you turn it on while holding the button. It will enter calibration mode. Make sure your remote is on. When it is on, start holding brakes until you hear one beep. Then you will see the LED change color, start holding max acceleration, it will beep twice. After that release the throttle to neutral and wait for it to beep three times. Turn off the ESC and turn it back on. Hear 5 beeps (4 short and 1 long) and if it is still alive, it should spin.
```

---
## \#15 Posted by: murloc992 Posted at: 2019-04-29T11:41:20.771Z Reads: 12

```
It's in the manual:
![image|690x215](upload://pQBBmaPCkz9I3cwduxL3J2knk8J.png)

No need to set to REV. Just do brakes where it is throttle and throttle where there are brakes. My post above is how I did it.
```

---
## \#16 Posted by: BrokenGloves Posted at: 2019-04-29T11:48:30.854Z Reads: 11

```
thank you it is working and spinning, just need to get it calibrated correctly now
```

---
## \#17 Posted by: BrokenGloves Posted at: 2019-04-29T11:48:45.752Z Reads: 12

```
thanks a lot buddy
```

---
## \#18 Posted by: murloc992 Posted at: 2019-04-29T11:49:22.338Z Reads: 12

```
Glad to help. :slight_smile:

Please do not attempt 10S now. :slight_smile: Ofc you can, for science, but last time I checked it is not really rated for it on the inside.
```

---
## \#19 Posted by: BrokenGloves Posted at: 2019-04-29T11:50:01.863Z Reads: 13

```
yeah ill try to avoid that thanks for your help
```

---
## \#20 Posted by: murloc992 Posted at: 2019-04-29T11:51:01.626Z Reads: 13

```
Either use the 5S batteries, or grab like, 4 of 3S 5Ah zippy lipos. Make a 6S2P pack and you will be happy. At least I was. My first build was pretty much what you have. :smiley:
```

---
