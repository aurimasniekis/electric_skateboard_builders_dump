# Throttle range/travel too short on 2.4 Ghz mini remote

### Replies: 21 Views: 959

## \#1 Posted by: kustihusti Posted at: 2018-05-05T08:56:52.533Z Reads: 164

```
Hey Guys

I got a problem with the throttle-range on my 2.4 Ghz mini remote. The problem is, that I already reach full speed at 25% of throttle travel. This also happens if I’m on the board (75kg load).  I’ve tried almost everything what was discussed in the forums. I’ve even bought a new remote (2.4 Ghz) changing from the nano remote to the mini remote. My setup is current control no reverse with break in PPM mode. Anyone has an idea to solve this problem within the BLDC tool form Benjamin Vedder? I’m using the latest version of the BLDC tool and a VESC from  . Or is there calibration of the remote needed? Any advice to my specific problem would be highly appreciated.😊

Greeting from Switzerland Jan
```

---
## \#2 Posted by: PartyPoison Posted at: 2018-05-05T09:39:15.061Z Reads: 156

```
If you're using nano v2 read this
https://www.electric-skateboard.builders/t/nano-v2-full-review/25159
```

---
## \#3 Posted by: b264 Posted at: 2018-05-05T09:42:59.834Z Reads: 147

```
The mini remote for sure will work.  You need to adjust the throttle curves and the PPM settings in the VESC Tool.
```

---
## \#4 Posted by: kustihusti Posted at: 2018-05-05T10:12:37.562Z Reads: 135

```
Is there really an option to ajust them in the tool? Or do I have to download this expansion from Ackmaniac? Would be really cool if you could send me a screenshot...
Greetings Jan
```

---
## \#5 Posted by: kustihusti Posted at: 2018-05-05T10:15:16.828Z Reads: 129

```
I actually bought a 2.4 gHz mini remote from alieexpress. I though that would fix my problem because everybody was talking really good about it....
```

---
## \#6 Posted by: kustihusti Posted at: 2018-05-05T11:20:06.440Z Reads: 123

```
Is there really an option to ajust them in the tool? Or do I have to download this expansion from Ackmaniac? Would be really cool if you could send me a screenshot…

Greetings Jan
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-05-05T14:08:55.903Z Reads: 110

```
under  PPM tab ++> mapping ==> input deadband  

this wording is using vesc tool, but should be same for ackmaniac


ackmaniac =
App config ==> PPM ==> "pulsewidth" at bottom


if can adjust on remote would be easier i guess, its been awhile since i had to mess with that setting (in firmware) so memory foggy
```

---
## \#8 Posted by: clistpdx Posted at: 2018-05-05T14:39:35.201Z Reads: 102

```
Have you tried turning on remote first, then toggling the thumb control all the way up then all the way down, then turn on board?
```

---
## \#9 Posted by: kustihusti Posted at: 2018-05-05T14:47:18.134Z Reads: 101

```
Nop I'm going to try it will be back in a minute...
```

---
## \#10 Posted by: kustihusti Posted at: 2018-05-05T15:29:25.318Z Reads: 104

```
I'm actually using the BLDC tool. 
These are my settings, I really can't see my mistake....![Unbenannt|690x386](upload://xDStxtoeTi3MqfxNll9fSqucZ75.PNG)
```

---
## \#11 Posted by: kustihusti Posted at: 2018-05-05T15:31:35.983Z Reads: 96

```
I tried it unfortunately it didn't work :disappointed_relieved:
```

---
## \#12 Posted by: Scoo_B_SK8 Posted at: 2018-05-05T16:28:20.661Z Reads: 86

```
change value in "max pulsewidth" or "min pulsewidth" or both... id start with max setting

Edit: might even want to adjust "deadband" as far as tweaking what feels comfortable for your riding
```

---
## \#13 Posted by: b264 Posted at: 2018-05-05T17:21:48.135Z Reads: 83

```
When you pull the trigger all the way, what is the maximum pulsewidth?  Then type that number into the box and it will make "100%" become that point
```

---
## \#14 Posted by: Ackmaniac Posted at: 2018-05-05T18:52:57.316Z Reads: 82

```
Just use one of the newer firmwares where you have throttle curve and also not the old current control. Can use my bldc-tool mod 2.54 or my latest 3.101 or latest original from Vedder which is 3.38 if I am not wrong. All of them have a better control algorithm.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-05-05T19:07:14.191Z Reads: 83

```
I’m using 2.18 fw and BLDC tool with mini 2.4 remote. 
Throttle response and range are good. 
If you don’t want to change firmware and software, try following this tutorial to setup your remote with BLDC tool. 
https://youtu.be/OtuofrQr3F8
```

---
## \#16 Posted by: Eboosted Posted at: 2018-05-06T06:01:07.849Z Reads: 68

```
I can also reach full speed at 25% throttle but the acceleration is slower, the speed control of a VESC is different than an ESC like the Evolve one, where you can set the speed by the throttle percentage.
```

---
## \#17 Posted by: kustihusti Posted at: 2018-05-06T15:23:37.120Z Reads: 62

```
That‘s exactly what I did. I tried it multiple times but in the end I always reached full speed at around 50% throttle range. What actually is the deadband setting for? I didn‘t change it, always left it on 0.25 ms...
```

---
## \#18 Posted by: kustihusti Posted at: 2018-05-06T15:28:18.973Z Reads: 60

```
Thats what I did all the time... I detected min/max pulsewith and tiped it into the boxes... still didn‘t work. Also the braking function is working in a really harsh way... way to strong to break safe (imagine me flipping of the board at 40 kmh😂). Any other ideas to fix the problem? In the end I‘m going to download Ackmaniacs firmware, as he suggested.
```

---
## \#19 Posted by: Scoo_B_SK8 Posted at: 2018-05-06T15:30:34.677Z Reads: 56

```
"deadband" is the position at witch throttle starts to kick in.  (the grey area where nothing happens)

example:   if .25 is 12 o clock and you increase to .50 would be 1 o clock
```

---
## \#20 Posted by: kustihusti Posted at: 2018-05-06T15:40:23.933Z Reads: 54

```
I‘m going to try to fix my problem with the modified tool from ackmaniac. If there‘s a new remote needed I‘ll get back to you👍
Ty very much
```

---
## \#21 Posted by: kustihusti Posted at: 2018-05-06T15:42:05.164Z Reads: 49

```
Alright I‘m going to try it with your tool, seems like a very cool and handy thing. I‘ll try it the following week I‘ll get back to you to tell if it worked.
Thank you very much👍
```

---
