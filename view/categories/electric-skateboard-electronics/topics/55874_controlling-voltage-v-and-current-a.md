# Controlling voltage (V) and current (A)

### Replies: 6 Views: 361

## \#1 Posted by: pedro Posted at: 2018-05-18T09:25:30.163Z Reads: 85

```
Hello, i saw the normal voltage is 36V, but the current?
I'm thinking use a LiFePo4 but already not found a good and cheap.
My motor can support 37V and 60 A, and have 1510W, if i use 30A and 36V, so i think i dont need a good motor P=36*30=1080W, and save some money
```

---
## \#2 Posted by: linsus Posted at: 2018-05-18T10:38:46.409Z Reads: 77

```
Getting tired of these threads without the bother to construct a comprehensive problem or a question.

What voltage is it that you have seen? What color was it? Why was it normal? Was it a he or a she?...
```

---
## \#3 Posted by: pedro Posted at: 2018-05-18T10:56:39.265Z Reads: 70

```
ok, i will ask another one more acceptable. :thinking:
If i define 36V and 45 A in my VESC for output, it will be always at this values? for example if i ' m in climbing a hill :sunrise_over_mountains: or just flat street :motorway: this values will be the same, and if i press hard :muscle: or soft :leaves: the control remote will change the voltage or current :zap::zap:? without considering the lost of batteries capacity.
This question is more  acceptable?
```

---
## \#4 Posted by: linsus Posted at: 2018-05-18T11:14:35.060Z Reads: 58

```
If you're intrested in how an electric motor works in relation to power voltage and current, I think you have some reading to do. If you dont like educational literature i sudgest using the search function on this forum.

To try answer your question in a short manner. No. The amps and voltage will differ depending on load. Only way to reach high power output is generally to constantly climb a hill. You will not get the kW you're talking about just by surfing the pavement. Power is a meassurement of energy, just cause you have a high power motor, doesnt specify where this power is actually fully used. Typically you'd use more power when accelerating and alot less when just maintaining speed. 

This is basic physics, internet is your friend. Use it. 

Regarding the choice of batteries, thats Another question entirly, a subject you can find truckloads of on the forum as well.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2018-05-20T02:21:12.457Z Reads: 32

```
Like what @linsus is saying, do some reading and please do not try to make an electric skateboard if you have little to no knowledge about basic electronics
Don't dive into the deep end for these things. You will hurt yourself
```

---
## \#6 Posted by: Hummie Posted at: 2018-05-20T04:16:40.686Z Reads: 25

```
the current you can control with the esc limits and the throttle and the current out will depend on the load.  the voltage just varies a bit to the motor as current is needed.  If you search pulse width modulation it will tell what voltage and current is going to the motor from the battery.
.   theres some cheaper lifepo4 around on ebay I just saw and posted about in the thread here on lifepo4

the limits you post for the motor are not true.  you could put a lot more amps into the motor than its rated for for a short time and the voltage isn't really an issue and you could use a much higher voltage battery.
```

---
