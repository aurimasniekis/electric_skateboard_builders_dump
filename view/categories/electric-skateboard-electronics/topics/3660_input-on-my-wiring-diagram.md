# Input on my wiring diagram

### Replies: 22 Views: 4970

## \#1 Posted by: Johan Posted at: 2016-05-22T21:49:21.480Z Reads: 258

```
Hi, im going to build my first electric longboard and I am a little bit unsure if this wiring would actually work.

I would like to have the battery on one end and the other electronics by the motors, and have flat braided cables under the grip tape to connect it. Is it possible to have the battery connected to the ecs's constantly and switch the board on/off with the ecs switches?

If you see something crazy please let me know. Also, I would like to remove the two switches that come with the esc's and instead wire a normal 12v switch instead that turn both esc's on. I drew all the switches just so you guys can see what I mean.

<img src="/uploads/db1493/original/2X/3/38621d66a5d4790dfcf4ba15bcdef5cef0bec72a.jpg" width="690" height="274">
```

---
## \#2 Posted by: treeme Posted at: 2016-05-22T21:56:58.341Z Reads: 248

```
Hey man, pretty sure the main switch doesn't turn the board off. as long as either the main switch or one of the side switches is on, the esc will get power. instead, you need to wire the main switch so that for for both switches, the main switch is is series.
```

---
## \#3 Posted by: Johan Posted at: 2016-05-22T22:12:58.922Z Reads: 224

```
Do you mean like this? @treeme
<img src="/uploads/db1493/original/2X/6/6594c72df110d2afbb299ca676a4b1126bd5206e.jpg" width="690" height="274">
```

---
## \#4 Posted by: Maxid Posted at: 2016-05-22T22:13:49.852Z Reads: 208

```
Your battery indicator will be turned on the entire time and drain your battery. Better to connect its ground to the switch as well. Also it will simply not work like this and I am pretty sure you meant to connect the voltmeter ground to the actual battery ground in your drawing.
```

---
## \#5 Posted by: Johan Posted at: 2016-05-22T22:16:34.623Z Reads: 208

```
Yeah i got that wrong. Is this the way you mean? @Maxid
<img src="/uploads/db1493/original/2X/a/a5adf7f866ba7cbcee35a46f7c46003127e1463e.jpg" width="690" height="274">
```

---
## \#6 Posted by: treeme Posted at: 2016-05-22T22:31:59.177Z Reads: 197

```
<img src="/uploads/db1493/original/2X/7/7a14652bdab92db86e9dff8d8c0bac1aa565c4a9.png" width="690" height="378">  Like this (excuse my poor laptop drawing skills). The idea here is that when the main switch is off, the wiring is disconnected fully. @Maxid, as lon as there's no conection from the positive end to the negative end when the switch is off, the battery indicator won't be powered.
```

---
## \#7 Posted by: treeme Posted at: 2016-05-22T22:33:44.430Z Reads: 185

```
Also, another thing which we didn't mention was that you had both positive and negatives going to the switch the wrong way. thay would always have the circuit complete which would explode your battery.
```

---
## \#8 Posted by: Johan Posted at: 2016-05-22T22:47:05.042Z Reads: 176

```
Ok, but with the way you have drawn it is not possible to use a standard 12v switch or am I wrong? @treeme
```

---
## \#9 Posted by: treeme Posted at: 2016-05-22T22:52:38.363Z Reads: 175

```
Sorry, didn't see that part. With the stuff you have listed, it would be impossible no matter which way you wire it. You would need to use something called a relay to have a lower voltage switch control a higher voltage. The relay itself would need power and is honestly not worth it here.  

Why not just repurpose the esc switch as the main switch?
```

---
## \#10 Posted by: Johan Posted at: 2016-05-22T22:55:21.575Z Reads: 158

```
Yeah I just want to turn in both esc with one switch, is that possible? @treeme
```

---
## \#11 Posted by: Johan Posted at: 2016-05-22T22:56:37.374Z Reads: 141

```
Also switches aside, is it safe to have the battery plugged in when the esc's are turned off? Also is it ok to charge when it's connected? @treeme
```

---
## \#12 Posted by: treeme Posted at: 2016-05-22T22:59:18.725Z Reads: 135

```
yes, As long as you wire a switch that can handle the voltage going through it, then the diagram I drew would suit your needs.
```

---
## \#13 Posted by: treeme Posted at: 2016-05-22T23:03:08.510Z Reads: 130

```
If the main switch is off, there's nothing wrong with leaving it connected. there's nothing wrong with leaving it charging while connected; since I don't know what kind of battery it is, I can't confirm it's okay to have the system on while charging, but you can do a poor man's test by checking to make sure the battery doesn't get too hot.
```

---
## \#14 Posted by: Johan Posted at: 2016-05-22T23:05:29.786Z Reads: 127

```
I found a switch that is rated at 230V 10A do you think it would work?

Sorry for all the questions but i'm not good at this
```

---
## \#15 Posted by: treeme Posted at: 2016-05-22T23:12:24.827Z Reads: 123

```
@Johan, don't take this personally, but a question like that is something that you can just google without asking others since the question is just factual/technical. [Here's](http://www.tpub.com/neets/book3/9f.htm) a link to a website that answers your question.
```

---
## \#16 Posted by: Johan Posted at: 2016-05-22T23:15:58.440Z Reads: 125

```
Yeah better if I do some more research, I might learn something😏. Thanks for the help man! @treeme
```

---
## \#17 Posted by: Maxid Posted at: 2016-05-22T23:19:45.249Z Reads: 120

```
No - it needs to be in parallel not in series. 

Also why are you going for a complicated high current switch when the esc ones can easily be switched with a low current one. I will try to draw something tomorrow.
```

---
## \#18 Posted by: Maxid Posted at: 2016-05-22T23:32:03.768Z Reads: 121

```
Dude please stop giving electrical advice if you do not know what you are talking about - this can be really dangerous.
It is not just the voltage but also the current that is the problem. Voltage does not go "through" anything - current does.
```

---
## \#19 Posted by: Namasaki Posted at: 2016-05-23T01:18:51.935Z Reads: 127

```
what brand and model of Esc's are you planning to use. Some cannot be connected to one switch but must have their own separate switches. And you should put the main switch at the battery to switch it off and on. Anyway, not all RC car Esc's are good for this application.
Also, if your planning to run dual motors, then you should consider running higher voltage system.
```

---
## \#20 Posted by: treeme Posted at: 2016-05-23T04:31:32.202Z Reads: 123

```
Here's a better diagram of an appropriate way of doing what you want.
the circled "A" is an ammeter, the circled "V" is your battery gauge, the disconnec partt being the switch, the box a fuse, the battery the double horrizontal bars, and the esc pretty self explanatory, 

<img src="/uploads/db1493/original/2X/f/f728f52baa0214b383e1b6b6009a3fea9902578e.png" width="642" height="500">
```

---
## \#21 Posted by: seanpain4 Posted at: 2016-05-23T22:51:16.076Z Reads: 103

```
You could also use a DPST switch which will allow you to turn both on at once without interfering with each  other. You just chop the switches off the ESC's and wire both to the on. These are switches on the ESC they are low current so you can use pretty much any DPST switch.
```

---
## \#22 Posted by: Johan Posted at: 2016-05-24T06:21:03.482Z Reads: 96

```
Thank you! Haven't seen those before.👍🏻
```

---
