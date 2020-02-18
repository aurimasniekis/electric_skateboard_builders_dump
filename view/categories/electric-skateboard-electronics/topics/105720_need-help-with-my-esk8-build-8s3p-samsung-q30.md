# Need help with my Esk8 build &#124; 8S3P &#124; Samsung Q30

### Replies: 5 Views: 81

## \#1 Posted by: Gvido Posted at: 2020-02-01T10:26:17.797Z Reads: 26

```
Hello,

I decided to build an electric longboard about a year ago, but I never finished it, and I'd like to do it now but I have a few problems.

I bought a hub motor kit with 600W each motor, the battery is 8S3P made out of Samsung 18650 Q30 batteries, and I got 2 40A 2S - 8S ESCs.

These are the links to my parts:

Motors: shorturl.at/fEJLU

2xESC: shorturl.at/KQUW3

Controller: shorturl.at/gqtAB

Battery: 8S3P - 264Wh (9Ah) with max. Constant Current 45A (I don't have a link because it is homemade)

The problem is that when I try to set it up, first it beeps for programming the ESC, and when I finish the programming it should work, but the motors spin for less than half a circle and stop, and then start beeping again for no reason.

I have tried the motors with another ESC and battery and they worked, but the ESC also worked with a smaller battery and smaller motors, so I thought they just weren't compatible (I don't know if this is possible but I heard it is). But, I found a review on the 80A version of these ESCs which are also 2S - 8S that they worked up to 6S, at 7S a bit worse, and at 8S not worked at all, but it was in French so after translating it, it said that he fixed it by extending the receiver wire by 25cm (about 10 inches) but I don't know how this would help, and what wire he meant by that.

I would really like to solve the problem if possible, or if not, what ESC, or VESC should I buy that is not too expensive that would work?

Here's what the review said if anyone understands French:

Regler bis 6S keine Probleme.
Regler bei 7S leichte Aussetzer.
Regler bei 8S nicht möglich !!!!!!
Den Fehler habe ich bei mir so behoben, indem ich das
Empfänger-Kabel um 25cm verlängert habe.

Thanks in advance.
```

---
## \#2 Posted by: anorak234 Posted at: 2020-02-01T12:40:15.127Z Reads: 21

```
[quote="Gvido, post:1, topic:105720"]
Regler bis 6S keine Probleme. Regler bei 7S leichte Aussetzer. Regler bei 8S nicht möglich !!! Den Fehler habe ich bei mir so behoben, indem ich das Empfänger-Kabel um 25cm verlängert habe.
[/quote]


This is German, not French. I believe that by Receiver wire the review would be referencing the cable that you attach the receiver to for whatever remote you are using to control speed. This sounds like a bit much in my opinion, but you could always make plug-in extensions for every part of it to test what the dude meant.
```

---
## \#3 Posted by: Gvido Posted at: 2020-02-01T16:05:21.117Z Reads: 20

```
Yes, German, my bad.

I tried to make the receiver wire longer although I don't know how that would help. Everything is the same, no difference. 

I thought it may be because my BEC powers 7.4V, maybe it's too much for the receiver but I'm not sure.
```

---
## \#4 Posted by: anorak234 Posted at: 2020-02-01T22:04:17.727Z Reads: 17

```
That could be an issue. Step down converters off eBay are nice and cheap.
```

---
## \#5 Posted by: Gvido Posted at: 2020-02-02T13:52:32.174Z Reads: 10

```
No, that's not the issue either. I just tried it with 2 AA batteries and no BEC how the receiver specifications say, but there's no difference.
```

---
