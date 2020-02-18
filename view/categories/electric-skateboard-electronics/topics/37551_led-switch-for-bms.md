# Led Switch for BMS

### Replies: 33 Views: 1791

## \#1 Posted by: Migro Posted at: 2017-11-06T20:12:14.262Z Reads: 248

```
Hi. I searched the forum and did not quite find what i was looking for, or else i did not understand it the right way. So now im seeking your advice and knowledge. 
As the title say i want led switch so i know when the board is powered on. 

I have a 12s Bms from bestech with e-switch output. But is it possible to somehow hook up a switch with led. Where can i get some power from for the switch. 
I found these two switches. one with power symbol and the other ones without. 
The first one here has 5 pins and seems pretty long:
https://www.ebay.com/itm/Red-Power-Indicator-LED-19mm-ON-OFF-Black-Metal-Shell-Push-Button-Toggle-Switch/201600351994?epid=3006426466&hash=item2ef0513efa:g:q78AAOSwXYtYspd1&vxp=mtr
And the other one has 4 pins and is a bit shorter:
https://www.ebay.com/itm/12mm-12V-Latching-Push-Button-Power-Switch-Black-Metal-LED-Waterproof-Ramdom-1PC/263207812957?hash=item3d48687f5d:g:EVMAAOSwvppZuyvh

Unfortunately i do not know if the first one is waterproof.
But the switches is not the important part. The question is how i would manage to do so. 

Thanks in advance
```

---
## \#3 Posted by: Acido Posted at: 2017-11-06T21:08:52.068Z Reads: 209

```
That is a really useful post I was just wondering how to wire the switch but didn't remember too do some research, damn this skateboard never stops taking my money!
```

---
## \#4 Posted by: mmaner Posted at: 2017-11-06T21:14:08.274Z Reads: 212

```
I didn't actually use it on my board, Those damned SPDT latching switches are waaaayyyy to long to fit in an enclosure comfortably.  I did it on my kids board and was using the Step Down Module anyways to power to some RGB Addressable LED's...o it just made sense.

I made sure to get advice before I pulled the trigger, but its still working over a month later.  Here's the original thread.
http://www.electric-skateboard.builders/t/bms-e-switch-step-down-convertor-led-power-switch/31889/11
```

---
## \#5 Posted by: Migro Posted at: 2017-11-06T21:21:18.975Z Reads: 192

```
@mmaner okay i do think i saw your post while searching. Does it really work with only one of the e-switch wires?
Thats probaly what confused me. 

I think i read someone talking about a 3.3v output on the vesc or something is this something you or anybody else knows anything about?
```

---
## \#6 Posted by: mmaner Posted at: 2017-11-06T21:23:49.461Z Reads: 181

```
Yeah, if you connect both switch legs it stays off, no idea why.  I just heat shrinked and secured the other leg so it didn't short.

There is either a 3.3v or 5v circuit on the VESC but I don't want to use it, don't like messing with the VESC hardware more than I have too, worried about burning them up.
```

---
## \#7 Posted by: Migro Posted at: 2017-11-06T21:29:06.849Z Reads: 171

```
If it works it aint stupid. And thanks. 
I may see if i can find something with the 3.3v or 5v
But yeah definitely not the only one afraid of burning it up :smiley:
```

---
## \#8 Posted by: Migro Posted at: 2017-11-06T22:55:28.127Z Reads: 167

```
So it is possible to use the 5V from the BEC connector. (reciever + and -) But it is rated for 5v at 1.5A. 
So as long as the button is using around 1A or so it should be fine. (Could be wrong) 
Someone mentioned som extra heat that could be building up, but i cant imagine with a small led that this would be a problem. 
And the buttons i linked is also 12v so running on 5v would mean that the light should be dimmed quite much(i haven't teste could be wrong) 

Okay i kinda answered my own topic here with some guidens. :smiley:
```

---
## \#9 Posted by: Namasaki Posted at: 2017-11-06T23:20:42.463Z Reads: 157

```
@Migro 
I'm using the same type of switch but wired this way:
This way turns the bms on and lights the led.
The voltage for the led is isolated from the bms e-switch
I'm taking 5v pos/neg from empty channel on the receiver.
basically, the buck converter on the vesc is powering the light through the cable to the receiver.
It's not a problem for the buck converter since the led is low drain.
I've built 3 boards with this setup so far. The oldest one over a year ago. It has not caused any issues for the receiver or the Vescs. I used Ollin vescs on 2 of the builds and Focboxes on the 3rd.
<img src="/uploads/db1493/original/3X/7/1/71c1deb6358de4d9133c9b0bde19ac980e9d9ad1.png" width="690" height="338">
```

---
## \#10 Posted by: mmaner Posted at: 2017-11-07T00:19:29.955Z Reads: 146

```
Good to know.  thanks
```

---
## \#11 Posted by: Migro Posted at: 2017-11-07T06:31:57.968Z Reads: 136

```
Thanks. That actually makes perfekt sense.

And thanks @mmaner your suggestion may be used in the future if more than 5v is needed.
```

---
## \#13 Posted by: TowerCrisis Posted at: 2019-01-01T18:42:38.929Z Reads: 69

```
Sorry for reviving a dead thread, BUT it appears that this diagram for the switch is incorrect and a new user just fried his BMS wiring it up like this.

You should never supply additional voltage or run current through a BMS eswitch, it is probably not made to drive a high power LED and even if it doesn't blow it could still affect it's functionality.

@Namasaki has the correct diagram, and it can also be used with a stepdown converter.
```

---
## \#14 Posted by: Z4MSupreme Posted at: 2019-01-01T19:18:44.923Z Reads: 63

```
That was me! 😭🙈. @mmaner you should really delete that post. For some reason, I was stupid and did realise that it would connect the power to the BMS. Ffs
```

---
## \#15 Posted by: Z4MSupreme Posted at: 2019-01-01T19:48:09.199Z Reads: 55

```
I am surprised that nobody else has had the same problem.
```

---
## \#16 Posted by: Migro Posted at: 2019-01-01T19:49:49.803Z Reads: 55

```
I just went with the simple solution
```

---
## \#17 Posted by: Z4MSupreme Posted at: 2019-01-01T19:50:32.510Z Reads: 57

```
An xt90 loop?
```

---
## \#18 Posted by: Migro Posted at: 2019-01-01T19:51:38.982Z Reads: 60

```
no the namasaki diagram. And just got 5v from my vesc
```

---
## \#19 Posted by: Migro Posted at: 2019-01-01T19:52:14.463Z Reads: 61

```
![image|690x338](upload://u5ZrExVId41b5qofmcPl0dwuFR2.jpeg)
```

---
## \#20 Posted by: mmaner Posted at: 2019-01-01T19:53:01.467Z Reads: 60

```
I disagree. If you use the switch that is linked the switch and the led are 2 separate circuits. So either the new user wire the switch incorrectly or used a different kind of seitch.
```

---
## \#21 Posted by: mmaner Posted at: 2019-01-01T19:53:42.909Z Reads: 56

```
It does NOT connect power to the BMS. If you used the correct switch the switch and led are separate circuits.
```

---
## \#22 Posted by: Z4MSupreme Posted at: 2019-01-01T19:56:32.375Z Reads: 54

```
It was the same switch as the diagram you used. And @TowerCrisis must be right because when I wired up the switch your way if fried the fuse in the BMS.
```

---
## \#23 Posted by: Z4MSupreme Posted at: 2019-01-01T19:57:24.232Z Reads: 54

```
Have you wired up the switch the same way you posted because you will have encountered the same problem as me
```

---
## \#24 Posted by: mmaner Posted at: 2019-01-01T20:00:24.199Z Reads: 54

```
I have, on 2 different decks well iver a year ago and I've had no problems. I think something must be different, post pics so we can see.
```

---
## \#25 Posted by: mmaner Posted at: 2019-01-01T20:02:01.044Z Reads: 56

```
What step down module did you use?
```

---
## \#26 Posted by: Z4MSupreme Posted at: 2019-01-01T20:06:33.833Z Reads: 56

```
https://www.ebay.co.uk/itm/DC-DC-Buck-Converter-Step-down-Module-Power-Supply-15V-58V-to-12V-3A-36W-MA1045-/163248608601
```

---
## \#27 Posted by: TowerCrisis Posted at: 2019-01-01T20:09:31.792Z Reads: 54

```
I disagree, because by bridging the + and NO you connect all three pins (NO, +, and C) when the button is pressed.
```

---
## \#28 Posted by: mmaner Posted at: 2019-01-01T23:43:15.946Z Reads: 53

```
I deleted the post, buy know that Bestech TS is the in that told me to do it this way. I have emailed them to ask for specifics, but my understanding is the when bridging the + & NO you do NOT bridc the Common. I'll post when I get more.
```

---
## \#29 Posted by: TowerCrisis Posted at: 2019-01-01T23:56:25.599Z Reads: 51

```
It does become bridged though, only when you press the button and it latches on

I'm quite surprised they suggested you do that... It just seems like an odd way to connect it
```

---
## \#30 Posted by: mmaner Posted at: 2019-01-02T00:33:53.123Z Reads: 50

```
They didn't suggest it, just approved it when I sent it to them.  I sent it because I couldn't get it to work any other way. Inuse loop keys or AS switches now, discharge only BMSs, so it doesn't matter anymore but I want to know for the sake of possible use in the future.
```

---
## \#31 Posted by: TowerCrisis Posted at: 2019-01-02T00:56:57.296Z Reads: 48

```
I'm really curious since you got it to work. What voltage did you run your buck converter at?
```

---
## \#32 Posted by: mmaner Posted at: 2019-01-02T02:53:59.518Z Reads: 47

```
12v, that's what the step-doen convertor outputs. It's not adjustable as far as I know.
```

---
## \#33 Posted by: J_Dizzle Posted at: 2019-01-13T17:57:05.878Z Reads: 43

```
For the 5v neg and pos am I taking from ch1 or the right 3 pins?

![image|375x500](upload://jttCOHmzGL3xK5Ao9YwjdAMa8Yg.jpeg)
```

---
## \#34 Posted by: Migro Posted at: 2019-01-14T16:15:51.707Z Reads: 42

```
I believe you could do that, im taking mine from the uart port on the vesc. Dont know if anything is better than the other.
```

---
## \#35 Posted by: TowerCrisis Posted at: 2019-01-14T17:42:57.858Z Reads: 41

```
![76307789|379x500](upload://13IaCLu5hEMClby2563eT1aeIhu.jpeg) 

Just to clarify, these are the pins. The channels run up and down, and the kind of pins (pos, neg, sit) run vertically.

Each channel for PWM needs one of each pin.
```

---
