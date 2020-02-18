# Extreme bad luck with this project

### Replies: 33 Views: 2967

## \#1 Posted by: pengy Posted at: 2016-12-26T13:09:25.830Z Reads: 281

```
Hey.. After a long wait for parts to show up to help me connect everything together better.. I connected everything as I should and my vesc started to smoke.. I checked and there was no short circuit anywhere..
The smoke came out of the chip marked in the picture, was connected to a 4s battery..

I guess there is no warranty for this things but wanted to know if maybe it's possible to replace the chip only or I should buy a new one..

<img src="/uploads/db1493/original/3X/f/9/f9761ce4dad2ac30cdb5501db87b57bc98ab7c17.jpg" width="370" height="500">
```

---
## \#2 Posted by: wmj259 Posted at: 2016-12-26T13:58:40.058Z Reads: 270

```
Where did  you buy that from?
```

---
## \#3 Posted by: goldenHusky Posted at: 2016-12-26T14:02:52.908Z Reads: 268

```
Your TVS diode is blown. 
The TVS is intended to suppress sudden and very narrow high voltage spikes, however if the high voltage lasts longer than some seconds, the diode will burn down. It looks like the linear regulator outputs a higher voltage than 5V, that would be clearly a production/ component failure and not your fault.
Your VESC might be ok (ST32 and DRV chip), however I would contact the manufacturer. 
Replacing the diode wouldn't make that much sense, since the failure will occur again.
```

---
## \#4 Posted by: pengy Posted at: 2016-12-26T14:24:05.759Z Reads: 255

```
diyelectricskateboard. Thank you I will pass them this information and hopefully they would take care of it somehow, a 100$ is allot of money for something I didn't even had the chance to use yet..
```

---
## \#5 Posted by: Blasto Posted at: 2016-12-26T14:28:29.997Z Reads: 254

```
Sounds like a manufacturing fault, 2 reasons the tvs could blow.

-bad gnd on the drv chip, made the output unstable >5V
-tvs could have been installed in the wrong side, hard to tell from the pic
```

---
## \#6 Posted by: goldenHusky Posted at: 2016-12-26T14:29:30.282Z Reads: 250

```
[quote="pengy, post:4, topic:15220"]
Thank you I will pass them this information
[/quote]

No problem, however please note that this is just my personal "diagnosis" which could be wrong.
Let us know what they replied. :wink:
```

---
## \#7 Posted by: PXSS Posted at: 2016-12-26T14:41:17.582Z Reads: 235

```
@torqueboards
```

---
## \#8 Posted by: pengy Posted at: 2016-12-26T15:23:25.858Z Reads: 230

```
Definitely, it makes sense, probably one of the spikes after few connection attempts got the chip blown and it seems not to handle the voltage well..
```

---
## \#9 Posted by: goldenHusky Posted at: 2016-12-26T15:36:45.053Z Reads: 225

```
[quote="pengy, post:8, topic:15220, full:true"]
Definitely, it makes sense, probably one of the spikes after few connection attempts got the chip blown and it seems not to handle the voltage well..
[/quote]

Maybe you should consider purchasing an anti spark switch or you could precharge the VESCs capacitors with an additional e.g. 500 ohms resistor moments before you connect your battery and the VESC (sparks are beautiful.. just not in electronics :wink:)
```

---
## \#10 Posted by: pengy Posted at: 2016-12-26T15:43:01.986Z Reads: 217

```
It was connected through a double XT60 or 90.. Adding a resistor is a great idea, essentially I would like to connect a 12S battery so even better.. So that means I should get a 1500 ohms resistor? 500X3. And how do I do this in an elegant way?
The idea is to elevate the voltage gradually to the VESC?

What if I integrate it with some kind of switch/button?
```

---
## \#11 Posted by: Blasto Posted at: 2016-12-26T15:51:04.990Z Reads: 211

```
If your gnd pad under the drv chip was badly soldered, it will cause the 5V output to go over 5V
```

---
## \#12 Posted by: goldenHusky Posted at: 2016-12-26T15:57:10.260Z Reads: 213

```
Never done it with a resistor tbh, but some XT60/XT90 connectors are already built spark proof, they usually have green marks on the yellow plastic. google "xt60 anti spark" and you'll find them.

Well you can use nearly any resistor value, depends on the charging time you want to achieve. e.g. it takes 0.25 seconds to charge the VESCs capacitors (3x680uF) to 12s voltage with a 25 ohm resistor.
I always used Vedders anti spark switches, soldered a couple of them yesterday.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2016-12-26T16:04:02.087Z Reads: 202

```
C'MON GUY.... it is a drv problem.... Bad soldering of the ground pads.
```

---
## \#14 Posted by: goldenHusky Posted at: 2016-12-26T16:31:16.121Z Reads: 203

```
yea, most likely, but what's the problem taking another step and talking about spark protection lol ? He'll send it to the manufacturer anyway.
```

---
## \#15 Posted by: Iceni Posted at: 2016-12-26T16:38:14.060Z Reads: 202

```
The spark that comes off when connecting the battery won't do any damage to the electronics, only thing that will take damage over time is the connectors themselves.
The batteries and caps can handle the momentary inrush current.

But still, on 12s antispark is usually a good idea.
```

---
## \#16 Posted by: Eboosted Posted at: 2016-12-28T07:11:41.300Z Reads: 168

```
So what exactly was the problem here? Bad VESC soldering from the manufacturer?
```

---
## \#17 Posted by: saul Posted at: 2016-12-28T07:36:20.498Z Reads: 163

```
its probably just a bad one. cut off the heat shrink and get some close ups of the pins.

i didn't notice there was no warranty now. i wonder what "tests" are actually being done if this can slip by....
```

---
## \#18 Posted by: pengy Posted at: 2016-12-28T11:44:44.873Z Reads: 162

```
It's a good question, it has worked for like a month until it didn't, I did nothing different. My guess is that there might have been a weak soldering point that may have gotten loose on the ground connection.. Assessing that according to what I've gathered do far with the help of guys on this forum.

I haven't heard anything from the manufacturer so far.
Wondering if I could diy it to replace the faulty chip..

Or to buy a cheap or used one..
```

---
## \#19 Posted by: goldenHusky Posted at: 2016-12-29T12:42:08.965Z Reads: 148

```
for diy replacement you will need a hot air soldering station (50$ on amazon) and some solder paste, I got best results with Sn63Pb37 pastes
I would ask someone in the forum to replace your DRV, some friendly guys only charge shipping and material costs
```

---
## \#20 Posted by: PXSS Posted at: 2016-12-29T13:19:27.376Z Reads: 146

```
Have you tried pming @torqueboards? He's been pretty good at replying pms through here with me.
```

---
## \#21 Posted by: pengy Posted at: 2016-12-30T10:13:16.533Z Reads: 135

```
Sounds great, and I am willing to pay for the work as long as it's worth it and to save some money.
Or buy a used one..
```

---
## \#22 Posted by: pengy Posted at: 2017-01-16T17:54:41.611Z Reads: 125

```
Hey guys, just an update regarding the VESC.. Fixing it through the company + shipping cost will cost me almost like a new one. So I was thinking about trying my luck and see if anyone here has a used one for sale or can fix my VESC's fried chip with pay of course.

Thanks
```

---
## \#23 Posted by: pengy Posted at: 2017-01-16T17:56:16.621Z Reads: 124

```
BTW got a brand new drop down deck today.. But until I have a working vesc I guess I'll have to push
```

---
## \#24 Posted by: Eboostin Posted at: 2017-01-17T21:52:52.236Z Reads: 117

```
Wow, they really didn't take care of it for you?
```

---
## \#25 Posted by: pengy Posted at: 2017-01-17T22:41:07.885Z Reads: 116

```
They offered to, but the cost makes it not worth it.. I understand the shipping cost but to activate the warranty alone is 60$ So it adds up to almost a the price of a brand new vesc. At this point my valid options are, if it's not to much to dill with to send it to someone who can fix it or just buy a used one.. and let the 120$ go to waste.. Didn't even had a chance to ride before it went faulty..Any offers will be welcomed
```

---
## \#26 Posted by: michaelcpg Posted at: 2017-01-17T23:01:15.521Z Reads: 106

```
Surely if the product was sent to you faulty then they should cover any costs with getting it repaired regardless of the warranty on it? 
Not sure what the laws are like in the US but here in NZ the seller would be required by law to do this.

Obviously if you sent it back at it turned out to be a result of user error etc then obviously it's a different story.
```

---
## \#27 Posted by: pengy Posted at: 2017-01-18T08:38:02.581Z Reads: 99

```
I agree, I rather not deal with legal issues since in this case it is not worth it.
Unfortunately a gray area has been opened here which is based on the fact that I can't actually prove that the VESC came faulty, therefore most likely I would be charged for the warranty if I were to send it to the manufacturer.
I clearly don't have the upper hand here.

Ideally.. I think that if I were the manufacturer, making these VESCs and having these chips lying around anyways, the tools and handy enough to do a simple soldering and replacing that chip within a few minutes, which also means preserving a happy costumer, all considering the circumstances of course.. Then I would take it all to consideration, but who 's asked me..
```

---
## \#28 Posted by: pengy Posted at: 2017-01-18T08:39:50.190Z Reads: 99

```
In this situation if anyone can help me figure out how to buy that chip and maybe go to a professional to replace it I'll be more than happy.
```

---
## \#29 Posted by: Blasto Posted at: 2017-01-18T16:05:57.670Z Reads: 95

```
http://www.electric-skateboard.builders/t/johnny-vesc-repair-services/11267?u=blasto
```

---
## \#30 Posted by: pengy Posted at: 2017-03-01T07:57:22.801Z Reads: 85

```
Hey everyone, I received my VESC two days ago from Johnny, after he had successfully fixed the problem!
So glad to have found this resource since sending it back to the manufacturer and activating the warranty would have cost me almost the full price of the vesc, which made me feel helpless. So glad Johnny offered his service and my vesc didn't go to waste.

The fried chip scenario has made me uncomfortable dealing with the vesc by myself, so looking for someone to help me through (with pay) the connections and finally connecting it to an Arduino.

Thanks.
```

---
## \#31 Posted by: Blasto Posted at: 2017-03-01T16:53:05.859Z Reads: 79

```
I've done a few arduino projects with the VESC, you have a few options when it comes to controlling the vesc. I like to directly use the PPM input, because i'm lazy and i find it quite handy to only use the myservo.writeMicroseconds( command to control the vesc.


I use a galvanic isolation for the arduino and vesc (3 pin ppm header on the vesc). 

<img src="/uploads/db1493/original/3X/7/3/731d6828b2755496cfb88800092c1cac13d34674.png" width="635" height="348">
<img src="/uploads/db1493/original/3X/8/0/808bd0c4375142795e2a7d97acb7d38686162206.png" width="571" height="224">


but you can also control it by UART-SPI even USB
```

---
## \#32 Posted by: pengy Posted at: 2017-03-12T09:10:19.072Z Reads: 59

```
[quote="Blasto, post:31, topic:15220"]
PPM in
[/quote]

Looks great, so just to be sure.

http://vedder.se/wp-content/uploads/2015/01/PCB_Front.png

To the PPM middle pin I connect the Arduino, Ground goes back to the ground of the arduino, and the third one is for
supplying the current to the VESC so 5V is enough, right?

Pretty much like this?
https://forum.openrov.com/uploads/openrov/1722/c4729a84546e64b2.png
```

---
## \#33 Posted by: pengy Posted at: 2017-03-12T09:49:51.231Z Reads: 53

```
This is what I did:

https://ykedwa.dm2302.livefilestore.com/y3p6M-FIVt_dQJs7l1OzNhmnRG4fwPl4OMEX9dq5FWNO5Jdv5lWEQhj34uD77m58frrVilwLbcjFvbzfc1y-NCajwmiU__5buFzSsUQDHbbMzVyuJt16prBIwOI61GVUoo1tiERteg6WTBvkiPjljdUGjmTEhW0CFjXmc6K1o9N1zQ/P70312-114226.jpg?psid=1

Orange from pin 9~ to VESC middle pin
White to GROUND
And Red to First pin
```

---
