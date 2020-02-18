# Problems with build, some turnigy esc expert here?

### Replies: 9 Views: 454

## \#1 Posted by: michondr Posted at: 2017-05-04T15:11:01.621Z Reads: 66

```
hello all!
Recently, I've built my longboard using these components:
sk3 6374 168kv motor
Turnigy 150A ESC
rocksta transmitter/receiver
6s6p battery from salvaged laptop batteries
diy deck in a shape of vanguard, caliber 2 trucks, ogangatang kegel wheels
16:36 pulleys on 15mm belt

this setup is quite good at higher speeds (top +-22kph), but when I need to go slower, sometimes the motor just freaks up - lots of weird sounds come out. At the same time, I have to push once to get it moving, I can't accelerate from zero.
I can't find out whether this is a problem of esc setting, motor kV, gearing ratio, or too shitty batteries.
here are setting of ESC: http://imgur.com/a/QlUaI (to be honest, I understand nothing here)

I think this is not a problem of battery, because the same happened with 12v lead acid, maybe just more aggressively due to low voltage. Also probably not a problem of gearing ratio, because if I changed it for more torque, I'll go slower. I don't want that to happen.

at low speeds, it just feels like the ESC changes polarity in motor too quickly, which means it is unable to rotate enough to be "caught" by next winding.

any opinions?
```

---
## \#2 Posted by: bartroosen12 Posted at: 2017-05-04T15:34:58.477Z Reads: 55

```
Can you describe better when this happens?
I had a 120A boat esc and the breaks were very random, somethimes just like it should be 20% braking but the other time it was braking at full power which is't very easy to predict :smile:
The other problem the esc had was when I was riding and took my finger of the trigger (So just rolling but no power to the motor) At this moment when I want to speed up the board randomly brakes and in both situations it sounds horrible.
```

---
## \#3 Posted by: michondr Posted at: 2017-05-04T17:21:52.880Z Reads: 41

```
to describe my problem more, I'd like to point out that I have no problems with braking.
What bothers me is the way the ESC utilising its power in low RPMs. The ESC can't speed up from stationary position with me standing on the board.
I know speeding form 0 is most power hungry process, but the setup acts as there is a problem in ESC setting.
This problem also sometimes happens when I want to speed up more aggressively - again, the ESC is unable to handle it
```

---
## \#4 Posted by: JohnA Posted at: 2017-05-04T19:58:59.380Z Reads: 32

```
I used two of those track star 150 amps on my last build. The cogging of the motor was normal.. I think it was partially caused by not enough amps available to the ESC, but also the fact it's not made for pushing a person. With motor sensors it might be better though, but a bolt on hall sensor kit didn't help my start up at all. I think if you want an esc that can start you from stop without hall sensors you have to use the VESC. Also though if you get a second ESC and motor, it will help with the startup. Still won't start from stop but after a kick it will have some power
```

---
## \#5 Posted by: michondr Posted at: 2017-05-05T14:36:23.146Z Reads: 25

```
thanks for the response! I'm planning to use vesc for my second build (copy of whiteponnys vanguard).
But for now, I have to stick with this ESC which is just crap to work with :smiley:. 
Have you played with the settings of this turnigy esc? Could you give me please a comprehensive description of all the fields in those pictures I've posted?
```

---
## \#6 Posted by: JohnA Posted at: 2017-05-05T16:10:57.776Z Reads: 22

```
 I just used the programming card and never plugged it into the computer. But my last settings I used were 
;
Forward/brake 
Reverse speed 25%
Punch rate switch 50%
First stage punch 5
Second stage punch 5
Throttle input curve yes
Throttle dead band 43us
Drag brake 10%
Brake strength 75%
Initial brake drag brake
Brake rate switch 50%
Turbo timing 0deg
Turbo full throttle delay 0.10 sec
Turbo engage slope 15deg


I remember messing with the settings a lot but nothing really helped... the only thing that did was a second motor and ESC.
```

---
## \#7 Posted by: michondr Posted at: 2017-05-05T16:23:06.609Z Reads: 20

```
do you remember what turbo timing does? I read somewhere that people max it out (I believe max is 15 degreees), you have it on zero
```

---
## \#8 Posted by: JohnA Posted at: 2017-05-05T17:51:00.590Z Reads: 13

```
If I remember correctly with turbo timing turned up the ESC cycles before motor is to that position, so it helps it have better startup and acceleration. But it also makes more heat, so it is a balance of how much heat you want and startup power. But for me it didn't really seem to make a difference.
```

---
## \#9 Posted by: michondr Posted at: 2017-05-05T17:54:51.805Z Reads: 13

```
ok, I'll try tinker some more with the system.
btw, from your perspective, would you recommend this turnigy esc? because from my point of view, everything on the market except vesc is just inconvenient to use.
```

---
