# Dead wiiceiver from Austin David. HELP! (Fixed Kind Of)

### Replies: 35 Views: 2498

## \#1 Posted by: JLabs Posted at: 2016-05-09T23:37:36.224Z Reads: 99

```
I have about 30 miles on my board and my wiiceover will no longer turn on. I changed nothing and don't know what it wrong! I know it is the wiiceiver because I can connect the esc programming card with no problems and when I change a setting the motor beeps.. Can anyone help?! Thanks!!!
<img src="/uploads/db1493/original/2X/1/1ce343601980287b4f880efce6420ef5e9063b75.jpg" width="689" height="390">
```

---
## \#2 Posted by: claudiofiore88 Posted at: 2016-05-09T23:50:28.198Z Reads: 91

```
What are the 2 leds doing? Are they on?  Are they flashing?
```

---
## \#4 Posted by: JLabs Posted at: 2016-05-09T23:59:39.031Z Reads: 87

```
No, the leds are not on, neither is the red light on the actual receiver for the wii remote. 
@claudiofiore88
Thanks for the help!
```

---
## \#5 Posted by: barajabali Posted at: 2016-05-10T00:29:07.896Z Reads: 83

```
why dont you swap out the remote for a wired one to see if its the receiver or the remote and the block
```

---
## \#6 Posted by: JLabs Posted at: 2016-05-10T00:31:02.717Z Reads: 79

```
There is no power to the board but I will give it a try, thanks
```

---
## \#7 Posted by: claudiofiore88 Posted at: 2016-05-10T00:38:56.053Z Reads: 76

```
I ran into a different problem than this one when I received my first wiiceiever from @torqueboards.  Mine was powering on, but it didn't accept the input from the nunchuck.  I just ended getting a replacement.  If you just bought it, it's probably still under warranty assuming you didn't fry it from water damage or something.
```

---
## \#8 Posted by: lilracerboi Posted at: 2016-05-10T00:49:26.176Z Reads: 74

```
Might try looking into another ATMega328. You can pull one out of an Arduino Uno after writing the Wiiceiver software to it. I wouldn't advise getting another one off the internet as it won't have a bootloader on it yet, unless you got the tools.
```

---
## \#9 Posted by: JLabs Posted at: 2016-05-10T01:05:00.639Z Reads: 71

```
That worked!!! :) Thank you!! I stole the chip out of the arduino!!! Do you know why the problem occurred so it dosnt happen again?
```

---
## \#10 Posted by: JLabs Posted at: 2016-05-10T01:30:11.728Z Reads: 70

```
Now the nunchuck will not connect? Not sure why.. A wired nunchuck works just fine, any tips?
```

---
## \#11 Posted by: torqueboards Posted at: 2016-05-10T02:40:09.273Z Reads: 66

```
@JLabs - You'll need to program the Atmega. You can check on Austin's site and see how to load the bootloader onto the Atmega. You can flash with Arduino.
```

---
## \#12 Posted by: lilracerboi Posted at: 2016-05-10T03:49:35.603Z Reads: 64

```
To be honest, I'm not sure.
It could possibly be the wiring inside the Nunchucks receiver.

These exact issues happened to me as well, before switching to @torqueboards mini remote.

(EXCELLENT by the way)
```

---
## \#13 Posted by: lowGuido Posted at: 2016-05-10T04:33:51.537Z Reads: 62

```
Just so you know. Don't ride it like that. make sure you crack open the dongle and solder it first or else you may street your face.

http://www.electric-skateboard.builders/t/opening-up-the-nyko-kama-dongle/1477
```

---
## \#14 Posted by: makepeace Posted at: 2016-05-10T08:47:13.685Z Reads: 54

```
@JLabs, you will probably find there was a power spike to the micro-controller, due to something or other. Because if lights aren't on, the chip is dead. It may have something to do with Austin's peripheral circuit. I just used an Arduino Pro Mini for my wiiceiver. Was like $8, and I got my nunchuck for $15 and everything's still holding strong as after about 3 months of use.

Re. what @torqueboards said, it seems like your software is fine, seeing as you say the wired remote is working. 

What is happening in terms of the LEDs on the dongle and the nunchuck? Are they talking/synced? If they are, then the problem is likely to be the connections between the dongle and the wiiceiver circuit. If they're not, then it's likely you have a syncing issue. 

Does your dongle/nunchuck have a sync button? What I usually do when my dongle and nunchuck aren't talking is turn everything off, turn on the wiiceiver, wait a couple of seconds for the wiiceiver to boot up, turn on the nunchuck. If it's not synced, I'll then press the sync button on the nunchuck. If it's still not synced, I'll press the button on the dongle. And if still not, I'll press the button on the nunchuck again. A combination of those things usually works for me. :blush: 

I completely agree with @lowGuido, solder those dongle connections.
```

---
## \#15 Posted by: JLabs Posted at: 2016-05-10T22:04:29.800Z Reads: 43

```
The leds are solid and wont connect, dongle light is on and the light is blinking on the nunchuck. I plugged it into a normal wii remote and it wont connect, any suggestions?
@makepeace
@lowGuido
@lilracerboi
@torqueboards
@claudiofiore88
@barajabali
```

---
## \#16 Posted by: lilracerboi Posted at: 2016-05-10T22:19:28.017Z Reads: 43

```
The Nunchuck receiver might be dead. This happened to me as well, completely out of nowhere, it just stopped working. Wiiceiver worked fine though, since a wired nunchuck worked with it, but I don't know what caused the issue.
```

---
## \#17 Posted by: JLabs Posted at: 2016-05-10T22:22:34.474Z Reads: 38

```
Yes, exactly.. The light on the dongle is on tho... @lilracerboi
```

---
## \#18 Posted by: lilracerboi Posted at: 2016-05-10T22:39:28.212Z Reads: 33

```
Oh whoops, nevermind. I read your comment wrong.
When I was using the Wiiceiver it would do kind of the same thing. Both lights blinking, but not connecting. I would just remove the battery from the nunchuck and put it back in to reset it, then wait for the led to shut off. It would connect after that, but I don't know if your situation is the same.
```

---
## \#19 Posted by: Michaelinvegas Posted at: 2016-05-10T23:20:20.771Z Reads: 35

```
Dude lose the wiiceiver just get a 
👇🏻
http://s.aliexpress.com/IZjmm2uM

It's just as small...it has a trigger for better throttle control ...
And easy to replace
```

---
## \#20 Posted by: JLabs Posted at: 2016-05-10T23:39:19.457Z Reads: 35

```
Yes but there is Bo cruise control and throttle smoothing with the thy 120a 6s esc
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-05-11T00:04:06.267Z Reads: 37

```
Cruise control really ?

To each their own
```

---
## \#22 Posted by: lilracerboi Posted at: 2016-05-11T01:12:04.075Z Reads: 35

```
I'll have to agree with @Michaelinvegas. I was put off by the lack of cruise control, but after a couple falls caused directly by the Wiiceiever, I switched to this remote.

Best decision ever. Way more control over the motor. Don't even need a cruise control feature.
The throttle smoothing was actually more of a headache than anticipated.
```

---
## \#23 Posted by: lowGuido Posted at: 2016-05-11T01:16:24.241Z Reads: 34

```
Nah man dont listen to them. Keep it nyko kama all the way.
Triggers suck.

Maybe make a video of what ots doing. Or take loads of pictures.
```

---
## \#24 Posted by: lilracerboi Posted at: 2016-05-11T01:25:41.022Z Reads: 33

```
By the way, I'm not trying to persuade you to get the trigger remote, though it does sound like it. I've just had some bad experiences with the Wiiceiver, to the point where I either have anxiety just riding my board or don't ride at all.

DIY is about preference/customization and it will always be that way.
```

---
## \#25 Posted by: Michaelinvegas Posted at: 2016-05-11T01:29:06.155Z Reads: 30

```
@lowGuido reserves his trigger finger for 👃🏻
Lol
```

---
## \#26 Posted by: JLabs Posted at: 2016-05-11T01:34:43.536Z Reads: 30

```
I will tomorrow have u ever had the problem?
```

---
## \#27 Posted by: lowGuido Posted at: 2016-05-11T02:38:09.763Z Reads: 34

```
It actually sounds like a problem with the kama itself. Try the place you got it from
```

---
## \#28 Posted by: lowGuido Posted at: 2016-05-11T02:40:43.768Z Reads: 34

```
@Michaelinvegas I reserve my trigger finger for
https://youtu.be/iH2vJCtrL48
```

---
## \#29 Posted by: lowGuido Posted at: 2016-05-11T03:00:21.420Z Reads: 34

```
one way of checking it is getting someone close by who also has a kama and seeing if it will connect, then you can tell if its a problem with the reciever or the chuck. i have had about 5 or 6 kama's and they all connect to any of the recievers.
```

---
## \#30 Posted by: makepeace Posted at: 2016-05-11T05:36:14.933Z Reads: 35

```
I rate you may have fried something on the dongle. It makes sense that if the micro blew, and was fixed by replacing, that some peripheral components might be gonners too, and there is lots that can go wrong on that dongle. Have you soldered the dongle directly to the wiiceiver board yet? Either that or +1 to @lowGuido's suggestion. 

Also, wiiceiver and nunchucks all the way. They are great. I have had 1 fall from it, but once you figure it out and nail down the way YOU built your board and have done the wiring etc, it's smooth sailing. Also, I'm slowly modding the wiiceiver firmware to my safety standards and tastes. It's not all that hard.
```

---
## \#31 Posted by: JLabs Posted at: 2016-05-12T20:00:17.400Z Reads: 35

```
Do any of you have a spare nunchuck? I bought a yobo on amazon for $10 and it dosnt work.. I will give $15 to $20 for one.. Thanks

@makepeace @lowGuido @Michaelinvegas @lilracerboi @torqueboards @claudiofiore88

I think that when the AtMega shorted, it also shorted the Nyko nunchuck dongle
```

---
## \#32 Posted by: lowGuido Posted at: 2016-05-12T20:01:24.435Z Reads: 34

```
Where are you located?
```

---
## \#34 Posted by: Michaelinvegas Posted at: 2016-05-12T20:07:59.827Z Reads: 35

```
I have two used ones
```

---
## \#35 Posted by: JLabs Posted at: 2016-05-12T20:08:47.248Z Reads: 35

```
Yes please!! I will PM you @Michaelinvegas
```

---
## \#36 Posted by: claudiofiore88 Posted at: 2016-05-12T21:26:50.145Z Reads: 33

```
[quote="JLabs, post:31, topic:3047"]
Do any of you have a spare nunchuck? I bought a yobo on amazon for $10 and it dosnt work.. I will give $15 to $20 for one.. Thanks
[/quote]

I still have mine. I'd probably sell it with the wiiceiver as a combo maybe.
```

---
## \#37 Posted by: raven Posted at: 2017-10-12T07:47:23.482Z Reads: 13

```
I have a receiver from Austin and water sipped in. Got a new one works great. And a nyko Kama from eBay
```

---
