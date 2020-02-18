# Fried 6355 motor? Fried 6S ESC? Help me diagnose please!

### Replies: 20 Views: 1933

## \#1 Posted by: popopopop Posted at: 2016-08-12T21:55:57.208Z Reads: 137

```
I have a 6S setup with TB's 6355 motor and TB's sensored 6S ESC. I plugged my motor into the hall sensor port for the first time and might have messed up. It worked great for a few seconds and I definitely noticed the smoother startup. However, the motor was spinning in the wrong direction so I switched two of the motor wires around. I'm going to guess it's super finnicky about the ordering because I turned it back on, motor clicks, and noticed visible smoke from the ESC. 

Now I can't get my motor to spin and the ESC's beeping noises are audibly quieter than before. The light on it is green, fan kicks in, and I can still program it. My motor only clicks now : (. Can someone help me diagnose?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-08-12T22:00:15.037Z Reads: 136

```
And if you use it with the motor sensor not attached...what happens?

Video please
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-08-12T22:01:32.784Z Reads: 134

```
And..just noticed the word "smoke"....

That's the soul of the ESC going to ESC heaven (maybe)
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-08-12T22:02:42.024Z Reads: 130

```
Need to have @torqueboards chime in
```

---
## \#5 Posted by: popopopop Posted at: 2016-08-12T22:04:06.976Z Reads: 123

```
Lol, that's what I figured about the ESC, but hate thinking that when everything on it looks back to normal besides the quieter noise. TB says he'll be free in 2 hours.

The light on my ESC is yellow/green, then turns red when I throttle when the motor sensor is attached.
The light on my ESC is green, then turns off when I throttle when the motor sensor is NOT attached. The motor clicks on when it's like this. It doesn't click when the motor sensor is attach.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-08-12T22:06:58.977Z Reads: 119

```
It's funny...I got an esc doing that clicking thing too...but the sensored wires weren't even attached ...but the clicking on mine seems to be coming from the esc ...never got smoke tho ...

Keep us updated on what u may find out
```

---
## \#7 Posted by: mccloed Posted at: 2016-08-12T22:14:23.275Z Reads: 114

```
Yup. Your ESC is fried. The phase wires can only be connected one way on a sensored motor. If you run them different you need to reverse the motor in the ESC settings. Or mess with the sensor wires(not recommended)
```

---
## \#8 Posted by: popopopop Posted at: 2016-08-12T22:17:57.351Z Reads: 105

```
Ahh, that's what I figured. I remember reading ONE thread about this, but didn't know better. I wish it came with a diagram, because sensored felt so buttery with the throttling. Thanks for your input guys!
```

---
## \#9 Posted by: torqueboards Posted at: 2016-08-12T22:26:26.007Z Reads: 100

```
Yeah, @mccloed is correct. Sensored setup needs to be correct as far as phase wires. You had it correct the first time. To reverse it, you'd have to change "reverse" on the ESC Card settings.

If it's not correct, you'll fry it after you ride it.
```

---
## \#10 Posted by: popopopop Posted at: 2016-08-12T23:16:54.444Z Reads: 94

```
It's there a way to know the color order? I'm about to try this again once I order a new one.
```

---
## \#11 Posted by: torqueboards Posted at: 2016-08-13T01:01:58.846Z Reads: 86

```
When looking at the motor phase wires it's A B C. Shoot me an email or PM. I'll discount you a bit on your ESC if you want to purchase it again.
```

---
## \#12 Posted by: Cptanpanic Posted at: 2016-08-13T10:43:31.874Z Reads: 70

```
@torqueboards So I have one of your 5055 motors.  So looking down at face of motor.  The colors are black, blue, yellow.  They are A, B, C respectively?
```

---
## \#13 Posted by: torqueboards Posted at: 2016-08-13T15:57:58.741Z Reads: 67

```
@Cptanpanic
Blue   = A
Black  = B
Yellow = C
```

---
## \#14 Posted by: mccloed Posted at: 2016-08-13T19:40:18.652Z Reads: 68

```
If the motors are being used on a different ESC other than @torqueboards, the phase wires might be different. I have found that the HK 150a has the phase wires reversed from the FVT.
```

---
## \#15 Posted by: popopopop Posted at: 2016-08-15T16:13:15.192Z Reads: 64

```
Since I don't want to repeat this, can you double check on the wiring again? My phase wires goes blue, yellow, and black like this crude diagram I drew. Does it connect like this to the ESC like how it's drawn? Or should it connect in descending order of A,B,C from the ESC side too, meaning I have to cross the the B and C wires?
http://i63.tinypic.com/35ksj7b.png

Btw, somehow my parts shipped Saturday and getting here today, Monday. That's some fast shipping!
```

---
## \#16 Posted by: torqueboards Posted at: 2016-08-16T20:53:10.284Z Reads: 59

```
You want to make sure that you know the A B C orientation for both the ESC and the motor. As many people have already mentioned they do vary depending on what/who the ESC is and/or if someone customizes the motor wires.

Technically, it doesn't matter which way they connect and they might not be a straight through connection as your showing. You'll need to just connect A to A, B to B, C to C, etc.

Always run it on the bench for testing first and check to see how smooth the motors start-up. If it's a smooth start-up, then you should be ok. Run it at really slow speeds first to confirm.
```

---
## \#17 Posted by: OskarCastrone Posted at: 2016-08-16T21:32:29.416Z Reads: 60

```
I actually had a similar problem recently with two FVT ESCs. I was not paying attention to the orientation of wires since I wasn't using the sensors... After only a two test runs the fist ESC fried. The weird thing is, that it worked fine the first two times, and then during startup (!) it started smoking a bit. I then tried with another one I've got which fried a couple of seconds after I turned the board on....
It is still a mystery to me.
```

---
## \#18 Posted by: Bender Posted at: 2016-10-07T02:26:37.845Z Reads: 43

```
@torqueboards Can you let us know how the VESC is layed out in terms of A, B, C
thanks
```

---
## \#19 Posted by: maxz Posted at: 2016-10-07T03:43:37.253Z Reads: 41

```
Yes i need to know this to haha
```

---
## \#20 Posted by: Bender Posted at: 2016-10-08T13:57:59.342Z Reads: 30

```
Well I tried a bunch of combinations and this is what worked best for me <img src="/uploads/db1493/original/3X/0/d/0d49f4425580525e3568235ba36b9fa8a59bcb88.jpeg" width="666" height="500">
```

---
