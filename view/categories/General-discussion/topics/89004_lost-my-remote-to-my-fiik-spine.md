# Lost my remote to my fiik spine

### Replies: 15 Views: 579

## \#1 Posted by: Socalway Posted at: 2019-04-01T16:54:11.296Z Reads: 145

```
Maybe someone can help me get my board back on the road. My back pack was stolen with my remote in it. I have tried everything to get another replacement remote from Fiik and even tried contacting next drive which is the manufacturer of the board in China with no luck. On the site it claims to be Wireless and proximity activated with Stepless Digital Throttle. Does anyone know how I can connect another remote to this esc? I would like to keep the original esc in order to maintain the looks of the board and continue to use the original housings. I will attach pics of the esc and receiver. Please help... ! Can I connect a different remote and receiver to this ESC? If so which one, and how???  I haven't ridden my board in months...Thanks![15541379221303243862105376718594|375x500](upload://tj6DB4rrdjkMdiQSVwo6QhtqPDR.jpeg) ![15541379725403850920529137492828|375x500](upload://379zwcF1IcxhK14k0UEXekieYkl.jpeg) ![20190305_110902|374x500](upload://wSAzBtBQSq6QnbE4Qi7BaX3nZKn.jpeg) ![15541380714391432124361525288760|375x500](upload://7wxz9Fx8FFyQhzEJzZKGTsIlbpw.jpeg)
```

---
## \#2 Posted by: KaramQ Posted at: 2019-04-01T23:07:59.294Z Reads: 105

```
That board is sick, never knew fiik made a board like that, do you have any pictures on how the remote looks?
```

---
## \#3 Posted by: KaramQ Posted at: 2019-04-01T23:11:27.412Z Reads: 101

```
But it seems if you rewire the servo cable, you can run a regular mini remote on it
```

---
## \#4 Posted by: wafflejock Posted at: 2019-04-01T23:48:02.262Z Reads: 100

```
Hrm yah not sure from look of receiver board it has TX/RX pins so some sort of serial communication which makes it difficult because you'd need to know what kind of serial communication, baud rate, etc. and then would need to know what actual control signals are being sent through.  If it were just a PPM or PWM signal then it would just have GND 5V and signal wire typically.

---

Guess is they have TX/RX so can get data from the ESC to send to the remote as well... the "Stepless Digital Throttle" idea has me baffled too though if it's digital it isn't continuous/analog so it has to have "steps" if they are small enough you won't notice them but they are there if using something digital.
![40%20PM|690x334](upload://24NEmdkEJitbl4CEN5VYt2p5Igc.png)
```

---
## \#5 Posted by: M.Hboards Posted at: 2019-04-01T23:50:53.567Z Reads: 89

```
Do you have a picture of what the remote looks like i may know where to get a replacement.
```

---
## \#6 Posted by: Jebe Posted at: 2019-04-02T03:53:59.339Z Reads: 81

```
they don't, you can find it on alibaba and get any badge put on it.
```

---
## \#7 Posted by: Socalway Posted at: 2019-04-02T07:03:00.006Z Reads: 76

```
Here's the remote..
![Screenshot_20190401-200021_Chrome|268x500](upload://71FXKbEbey9r3DHZTZdEZW3VTNI.jpeg)
```

---
## \#9 Posted by: Tangent Posted at: 2019-04-02T07:37:56.120Z Reads: 68

```
If you can't find a compatible remote, you always have the option of changing the ESCs getting a ppm remote and reuse everything else on the board. All the info needed on doing the transplant can be found here on the forum..
```

---
## \#10 Posted by: marsrover001 Posted at: 2019-04-02T15:52:49.265Z Reads: 52

```
I'd try putting a regular PPM remote on 5v, gnd, tx.

It could be serial, but it could also be ppm. Since it's a digital signal either way you won't break anything.

Otherwise, time to upgrade to a unity.
```

---
## \#11 Posted by: banjaxxed Posted at: 2019-04-02T16:34:02.427Z Reads: 51

```
_* **Pistol Grip Controller:**  Wireless and proximity activated with Stepless Digital Throttle_

I'm guessing you'd have a better chance of replacing the esc for a small dual like the unity ^

Their ESC looks pretty tiny but the Unity is pretty small, * Outer Case Footprint: 117mm x 64mm
* Outer Case Height: 19mm

![image|474x288](upload://mVI3LgE2Jl1HTDOaRMW2j3yvJEt.png)
```

---
## \#13 Posted by: Socalway Posted at: 2019-04-05T02:17:44.635Z Reads: 25

```
[quote="M.Hboards, post:5, topic:89004"]
wheat
[/quote]



Here is a pic of the remote. That would be awesome if you know where I can get one . Thanks either way
```

---
## \#14 Posted by: Socalway Posted at: 2019-04-05T02:20:17.327Z Reads: 24

```
How do I do that?
```

---
## \#15 Posted by: M.Hboards Posted at: 2019-04-05T02:34:05.396Z Reads: 24

```
Sorry spell correct changed it to wheat it was supposed to day what! There is a brand on Alibaba called iwonder that appears to manufacture the board you have and they sell replacement remotes however yours looks different than the one they sell and I'm not sure if they're cross-compatible.
```

---
## \#16 Posted by: KaramQ Posted at: 2019-04-05T02:44:00.784Z Reads: 22

```
It wouldn’t work, to be honest, I would just switch the esc to a focbox unity
```

---
## \#17 Posted by: wafflejock Posted at: 2019-04-05T03:27:28.868Z Reads: 18

```
Yup just took a look at some of their remotes on the site and new one has a display it looks like and old one had speed control so was sending signals from the remote to the receiver to update the ESC values so will be hard to work out all the details of the serial bus connection and protocol used for sending throttle (especially without having a working transmitter/receiver, could at least reverse engineer it with an oscilloscope if you had both sides... and an oscilloscope capable of capturing the serial communication or some other serial sniffer device).

Long story short agree with others your best bet to get back up and running is a new ESC, Unity is a good but not cheap option for dual drive and allows many kinds of remote input from different kinds of receivers.
```

---
