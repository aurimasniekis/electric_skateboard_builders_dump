# Remote MTSKR1512 Maytech

### Replies: 13 Views: 1455

## \#1 Posted by: Luuke Posted at: 2017-11-18T15:12:49.957Z Reads: 229

```
Hi,
I think some of you here are using MTSKR1512 already?!
@longhairedboy
Can you tell me how to connect the reciever to the VESC?
<img src="/uploads/db1493/original/3X/d/c/dcd0f263f28c8decfcd5f527d1c2c3099fe8c756.jpg" width="666" height="500">

Can you tell me what this button at the inside is for?
<img src="/uploads/db1493/original/3X/7/3/735aa629f6c636559e21568cf268f11e48f8ef42.jpg" width="666" height="500">
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-11-18T20:53:18.817Z Reads: 200

```
I don't know anything about this remote but if I had to guess that is probably the bind button
```

---
## \#3 Posted by: rich Posted at: 2017-11-18T22:14:51.682Z Reads: 190

```
Easy! :grin:

Connect it as shown on picture, the receiver has 1 channel but 2 parallel connectors.

<img src="/uploads/db1493/original/3X/4/4/4419a0eb3935ba091a2f8a7d8148b177143e3b38.jpg" width="690" height="388">


If you PM me your e-mail I can send you the manual.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-11-18T22:32:28.177Z Reads: 175

```
yeah that’s it. channel 1 on the receiver goes to the vesc. easy peasy. 

just sold the last of my steezes, moving to the new ones. they have two different throttle curves. on my boards that lets you choose between “ok i got this” and “holy fucking christ” modes. also they don’t seem to break. we’ve been throwing them in the street at speed as a sort of drop test.
```

---
## \#5 Posted by: Sebike Posted at: 2017-11-18T22:37:56.617Z Reads: 167

```
Pics, video and audio or it didn't happen!
```

---
## \#6 Posted by: Luuke Posted at: 2017-11-18T23:15:30.861Z Reads: 169

```
[quote="ShutterShock, post:2, topic:38692"]
bind button
[/quote]
What means bind button??

@rich:
Thank you! That's easy.
What are the solder pads for?

And how can i use cruise control? And what are both buttons on front side for?

PS: got the manual https://shop.elektro-skateboard.de/media/pdf/ea/12/8f/MTSKR1512_manual.pdf
Or is there a other / better one available?
```

---
## \#7 Posted by: rich Posted at: 2017-11-18T23:38:13.466Z Reads: 160

```
[quote="Luuke, post:6, topic:38692"]
What are the solder pads for?
[/quote]

I have no idea, you don't need them. The manual is the correct one. 
I bought 2 and I had to bind (pair) 1 of them, and changed the channel as well.
When you use cruise control you press the speed joystick at desired speed. But to stop cruise control you have to move the throttle twice and when you fall, your board could say good bye, I don't like it.
Just to make it easy:

<img src="/uploads/db1493/original/3X/b/c/bcaeed18d2ea391e73972262297c94c0e61b65ff.PNG" width="690" height="467">

<img src="/uploads/db1493/original/3X/8/3/83ad48f57a03d5f2074b2365ada6ed00fdc07d85.PNG" width="659" height="500">


## Pairing Process:

**1,** Turn off the Remote and Receiver.
**2,** Turn on the remote with A Button.
**3,** Press down and release C button. The A Light will blink green.
**4.** Press the B button 10 times in less than 10 seconds. All lights on your controller should turn off.
**5.** Turn on the receiver. E Light has some combination of flashing lights. The pairing begins.
**6.** The two lights (A & C) together tell you what frequency it is. The A Light is in terms of tens, and the C Light is the single digits. Simple add the two numbers together to determine which frequency you are on. 
Example: The default frequency for this remote is 2. A Light flashes 2 times. If the frequency is 15, A Light flashed 1 time and C Light flashes 5 times. To change the frequency, simply slide the joystick (Do not press the C button) up or down to increase and decrease the frequency.
**7.** Press C Button to save the frequency. All lights turn off.
**8.** Press and hold the A button to turn off the remote. Turn on both your remote and electric skateboard. The receiver should blink red and become solid red if pairing was successful.
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-11-19T00:17:17.411Z Reads: 129

```
Do you understand what you need to do from what these guys are saying?  I was just speculating.

Usually the bind button is what you use to pair a remote with a receiver, and I guessed that it may be that.
```

---
## \#9 Posted by: Luuke Posted at: 2018-01-09T21:16:26.760Z Reads: 108

```
[quote="longhairedboy, post:4, topic:38692"]
they have two different throttle curves. on my boards that lets you choose between “ok i got this” and “holy fucking christ” modes.
[/quote]

How can you switch between those two modes?
Couldn't find anything in the manual about that...
```

---
## \#10 Posted by: longhairedboy Posted at: 2018-01-10T02:00:03.580Z Reads: 101

```
click the power button once to switch modes. Its perfectly safe to switch modes while coasting, but i may not want to do it while throttling. I change modes all the time while coasting.
```

---
## \#11 Posted by: Luuke Posted at: 2018-04-09T20:27:35.851Z Reads: 79

```
Hey, just tried my board, but I am not able to change the mode.
There ist absolutely no different after pushing the power button.
Besides that: the ppm throttle response is quite strange and unresponsive. The gradient is really limited.
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-04-10T00:04:39.303Z Reads: 75

```
if you're using a VESC, you need to load vesc tool or bldc tool or whatever you're using and set it up for your remote. You have to do this any time you change remotes if you want to get what you expect out of it.
```

---
## \#14 Posted by: composites_r_awesome Posted at: 2018-07-27T11:11:17.685Z Reads: 34

```
Hi

I have this very same remote, but if was left uncharged for a year and now the binding doesn't work. In the manual they warned about letting it discharge too much as it will delete the 'data' on the remote, Could this be fixed somehow?
```

---
