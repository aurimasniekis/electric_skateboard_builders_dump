# Power cutoff almost immediatly when riding (even with no load)

### Replies: 12 Views: 342

## \#1 Posted by: Mazer Posted at: 2019-06-23T17:38:45.107Z Reads: 102

```
Hello eSk8 builders

Recently I built my first electric longboard. It is a single belt driven longboard. I watched a lot of YouTube tutorials online before I made my own. So close to all parts that I used came from Mboards and hobbyking. Once my package arived I started mounting everything together and everything worked fine for about 40 mins (two rides of 20 minutes each in two days). Since then my board will automatically cut off power almost immediatly once I try to ride it (also cuts off when I let it free spin, so no load). Also, it beeps really loud from time to time (while it's in error). The connection between my ESC and remote is working fine and not getting interupted becasue when I use my break, the led lights up. I can turn on and off the ESC with the on/ off push button, but that only seems te reset it with the same outcome as already descriped.

My guess is that there is an error with the ESC. But i'm not sure.

I made some pictures of my board, aswell as a wiring diagram.
(wiring isn't as clean anymore because I already took of the tape to check my connections to try and find the error).

![ESC|690x459](upload://5nCT50Tkz6Gd4McfnxirUZZx8Qi.jpeg) ![remote|333x500](upload://q0h5ug8R94hAp6gG77gJ6IKdcdm.jpeg) ![total|690x459](upload://wXIPsg9LAfZQGOCsgxtIMCNBHO5.jpeg) ![wiring|690x459](upload://t6hzM35LGZoSrGE6s8Sl9sNEEMv.jpeg) 

*Specs:*

* MBoards 6355 180KV Motor

* Single Belt Driven Motor ESC (Orderen for 10S battery)

* 2x Turnigy 5000 mAh 5.0 20-30C discharge (wired in series to make it 10s)

* Kegel 80mm

* Caliber II trucks



I hope someone knows the solution because I really want to start riding again!

Kind regards,
Mazer741
```

---
## \#2 Posted by: Szosiem Posted at: 2019-06-23T19:15:38.441Z Reads: 85

```
For me looks like your ESC died (maybe overheated or something). 

Check the ESC board closely. Is there any noticeable damage on ESC? Smell of electronic?
Is there any possibility to check error codes of that ESC? 

If I where you I would buy the VESC or FOCBOX. It costs more, but there are a lot of posts from this community connected with those devices and their problems. It worth that price. Also good idea is to connect a fuse since I don't see any BMS in your config. 

Hope it helps a bit ;)
```

---
## \#3 Posted by: Mazer Posted at: 2019-06-23T19:51:49.060Z Reads: 81

```
Thank you for responding

If it died, would it still be able to turn on and accelerate for a few seconds (brakes also still work)?

I can't see any damage or smell of burned electronics Yeah if my ESC would be unrepareable i'll defenitely go for a VESC. But ofcourse I hope someone knows a solution :slight_smile:


Also what fuse should I integrate? How do i calculate the max amps that can go trough?
```

---
## \#4 Posted by: Szosiem Posted at: 2019-06-23T20:26:56.129Z Reads: 76

```
[quote="Mazer, post:3, topic:97171"]
If it died, would it still be able to turn on and accelerate for a few seconds (brakes also still work)?
[/quote]

Well, it depends how deep a damage of ESC is.

For example I had an motherboard in my PC that I shorted by mistake with faulty USB drive. Motherboard still worked, but after a few months it started to shut down under load.

Maybe someone have an experience with this ESC and can share any experience. If you are not familiar with electronics it's going to be hard with diagnostic. You would need some equipment like oscilloscope to check ESC output to know what exactly is happening. (Someone correct me if I'm wrong)

[quote="Mazer, post:3, topic:97171"]
Also what fuse should I integrate? How do i calculate the max amps that can go trough?
[/quote]

Personally I'm using fuse that is close to constant value of VESC can handle (in my case 50Amps). It's a car audio fuse in cute water resistant case like this :smiley: :

![](https://images.yaoota.com/yPmhjXa9itIUcBamF-Wz5-eRljQ=/trim/yaootaweb-production-ng/media/crawledproductimages/ce80f4e8a7d18d0e2d3032bff2917494bc48abdb.jpg)

In your case look's like the same thing (if it's your device - [link](https://www.mboards.co/products/single-belt-driven-motor-esc) ). Fuse is relatively cheap comparing to other devices on skateboard and it's easy to change.
```

---
## \#5 Posted by: Mazer Posted at: 2019-06-23T22:55:43.990Z Reads: 59

```
Yeah i'm not able to do such a diagnostic.
And yep that's the ESC I'm using, I'll make sure i use a fuse in my circuit next time.

But if possible I'd still want to fix the issue i'm still having. Maybe someone else has any experience with such ESC's? I' really appreciate it!
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-06-23T23:36:51.132Z Reads: 58

```
[quote="Mazer, post:3, topic:97171"]
If it died, would it still be able to turn on and accelerate for a few seconds (brakes also still work)?
[/quote]

It's dead, on one of my dual ESC's both motors would work in slow mode but if I went into high mode it would work for the first few seconds but afterwards one motor cut out

^^meaning one motor would only cut out durning high erpm
```

---
## \#7 Posted by: banjaxxed Posted at: 2019-06-24T01:36:40.336Z Reads: 52

```
Try these
https://www.electric-skateboard.builders/t/dual-hub-motor-esc-first-build-doesnt-work/96707?u=banjaxxed
```

---
## \#8 Posted by: Mazer Posted at: 2019-06-24T12:34:27.179Z Reads: 36

```
Well thanks for the help everyone!
Sadly enough I think this ESC is unrepareable so I'll order a new one. This time I'll go for VESC since they seem a lot more dureable and reliable.
```

---
## \#9 Posted by: Halbj613 Posted at: 2019-06-24T21:54:09.214Z Reads: 24

```
According to the battery meter on your remote it is out of charge

Also certain esc work with lipo and some with lion you probably bought the wrong one 

That is pre programmed as these are not programmable
```

---
## \#10 Posted by: Schulerbible Posted at: 2019-06-24T22:32:25.943Z Reads: 19

```
Get the Hobbyking vesc
```

---
## \#11 Posted by: Mazer Posted at: 2019-06-25T10:01:00.292Z Reads: 17

```
It has worked so I'm sure i bought the right one. And the batteries still measure at about 15V per batterie.
```

---
## \#12 Posted by: Mazer Posted at: 2019-06-25T22:35:09.481Z Reads: 13

```
I fixed it! Thanks everyone for helping me think. It gave me the inspiration to solve the issue.
```

---
