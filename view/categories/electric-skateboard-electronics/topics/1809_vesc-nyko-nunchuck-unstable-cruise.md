# VESC + Nyko Nunchuck, unstable cruise !?

### Replies: 17 Views: 2353

## \#1 Posted by: EvanAndDadProd Posted at: 2016-03-14T22:52:55.183Z Reads: 159

```
Hi there,

I've just tried the VESC with firmware 4.15 with a Nyko Nunchuck on config below and we're having a strange behaviour when using the cruise button. It accelerates then slows down then accelerates again, etc. It's not so brutal that you can't stay on the board, but it's far from ideal either.

Has anyone got any view on what the problem might be?

**Motor: 3.2kW 63mm motor**
> KV: 170
> MAX POWER: 3200W
> WIRE WINDS: 10
> MAX AMP: 80A
> MAX VOLT: 10S
> RESISTANCE: .56
> NO LOAD CURRENT: 1,4

**Battery pack**
> 2x 5s in series
> 8000 mAh
> 30C discharge
> 5C max charge rate

<img src="/uploads/db1493/original/2X/d/dbfda117f4f85ee0ca63e010d782135f43a65861.png" width="690" height="431">

<img src="/uploads/db1493/original/2X/f/f7d51dbc94a5fc7b52bbbd65a3df71b6d137df06.png" width="690" height="431">
```

---
## \#2 Posted by: lowGuido Posted at: 2016-03-14T23:40:56.344Z Reads: 151

```
are you going up a hill when this occurs? 
or how is the drag on the board when it freewheels?

the cruise control on the VESC, how do I explain it? it checks the speed that you are doing and dials that as the speed you want to do, then it checks the speed again at certain interval and adjusts acceleration to suit. 
I am not sure what the interval is, but of you are going up a hill I have noticed a sort of surging sensation as it corrects the speed. I am sure that the code could be changed to have a smaller interval, or perhaps bearings cleaned and belt tension checked so that you don't have as much drag and the board doesn't slow as rapidly?
```

---
## \#3 Posted by: EvanAndDadProd Posted at: 2016-03-15T08:05:24.281Z Reads: 141

```
Come to think of it, there might indeed be something to do with load. I am 70kg and have this issue whether going up or down. My son, who's 20kg less than me doesn't systematically have it. It seems that the faster he cruises the less likely he is to have the speed oscillating that way. 

I should add that the problem happens only when using the cruise control mode, not when controlling the speed with the nunchuck joystick.
```

---
## \#4 Posted by: lowGuido Posted at: 2016-04-18T03:47:43.991Z Reads: 127

```
hey @EvanAndDadProd
last night I upgraded my VESC firmware to the latest version (2.16) and today when I went for a test rid it was doing the surging thing REAL bad! its HORRIBLE.
way worse that I had mentioned previously in this thread!
im gonna check the settings and see if I cant make it right.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-04-18T04:50:51.894Z Reads: 126

```
well i just re flashed my firmware back to 1.14 and she's all sweet again.
dunno whats up with that? all the settings programmed in were the same.
```

---
## \#6 Posted by: Bobfandango Posted at: 2016-05-05T16:07:10.283Z Reads: 149

```
@lowGuido, re: the surging, are you using FOC?  If so, you may need to tweak the PID parameters.  See the related post at: http://vedder.se/forums/viewtopic.php?t=98
```

---
## \#7 Posted by: lowGuido Posted at: 2016-05-05T21:18:06.968Z Reads: 147

```
Not using FOC. Just standard
```

---
## \#8 Posted by: massy Posted at: 2016-05-05T23:28:05.919Z Reads: 152

```
Same here (@lowGuido ) I THINK. Not using FOC and have only used this firmware so cannot compare. When holding cruise it feels like throttle, release, throttle, release, smooth, throttle, release and so on, I don't dare use it at high speeds. 

Also the latest problem I mentioned in this thread with random cutouts and surprise things from the remote was definitely motor wires screwing up the receiver. When the receiver was close to the wires it cut out as soon as applying throttle at the bench. Getting longer wires and moving it 10 cm from wires and no more problems whatsoever. I think I finally sorted the remote stuff out.
```

---
## \#9 Posted by: Bobfandango Posted at: 2016-05-06T21:53:40.819Z Reads: 138

```
Hey, I figured out that FOC *NOT* a requirement to experience this problem.  See this: http://vedder.se/forums/viewtopic.php?f=6&t=74&p=586&hilit=cruise+control#p586

There are PID parameters for speed control in the Advanced tab of Motor Configuration (they are labeled KP, KI and KD).  From the thread, Vedder and Whitepony get best results with KP=KI (and KD zero I think).  Whitepony used .002 for both KP and KI...  ymmv
```

---
## \#10 Posted by: Bender Posted at: 2016-05-10T04:29:30.994Z Reads: 119

```
@Bobfandango thanks for that link
I'm having the problem in both FOC and BLDC
I'll try those setting for FOC tomorrow
```

---
## \#11 Posted by: Hawkmoon269 Posted at: 2016-05-10T05:17:31.082Z Reads: 118

```
There's a setting in the nunchuck block of the bldc tool that controls the refresh speed of the cruise control. I found that lowering the number reduced the changes because the board doesn't have that much time to decelerate in the small amount of time you can set it too. I'm not an expert but you could try that
```

---
## \#12 Posted by: EvanAndDadProd Posted at: 2016-05-10T06:29:05.598Z Reads: 116

```
Thanks a lot everyone. It looks like between the PID parameters and the refresh rate we have a bunch of things to explore.
```

---
## \#13 Posted by: Maxid Posted at: 2016-10-06T23:07:22.618Z Reads: 78

```
how did it turn out? I am experiencing the oscillation as well on my new VESCs
```

---
## \#14 Posted by: Bender Posted at: 2016-10-07T01:27:51.455Z Reads: 79

```
That Fixed the cruise control!
```

---
## \#15 Posted by: Goombaacez84 Posted at: 2016-10-07T04:14:58.558Z Reads: 75

```
Was it only the phase wires causing issues? Or do you know if the battery leads (if nearby) was causing issues as well?
```

---
## \#16 Posted by: massy Posted at: 2016-10-07T10:47:15.994Z Reads: 72

```
If i remember correctly the effect was more prominent around the phase wires. In the end on my build though I replaced the Nyko Kama with the Enertion/Steez remote as I never got it to work perfectly with the signal. I did not feel I could trust the Nyko Kama going around at 30 km/h.
```

---
## \#17 Posted by: Goombaacez84 Posted at: 2016-10-07T13:46:34.191Z Reads: 69

```
I've added a ferrite and moved it away from the phase wires a bit but they're still pretty close because I've also been trying to keep it away from the battery leads as well. This made it difficult since... well, VESCs are designed to have the battery leads on one side and the phase wires on the other side, so that doesn't leave me much room to go to :sweat_smile:

I'm going to be changing out the remote with something a little more reliable (2.4ghz mini or benchwheel remote) but am trying to make this work to the best it can while it's what I'm stuck with. Winter is coming where I live and I'm just trying to enjoy what's left of the warm-ish weather!
```

---
