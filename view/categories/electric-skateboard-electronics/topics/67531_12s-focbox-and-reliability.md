# 12s focbox and reliability

### Replies: 20 Views: 1251

## \#1 Posted by: BooYA Posted at: 2018-09-09T19:30:04.151Z Reads: 258

```
Hi guys just a quick question about reliability. 12s4p 30Q, dual focbox with 5065 140kv motors running FOC sensored at 40amps 60k erpm .
Worked for about 50 kilometers and then DRV error occurred... No idea why. 
Is 12S safe on Focboxes? Also a have quite long battery wires, should I add more caps?
Is it possible that I blew my drv because of the inductance being too important?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-09T19:33:03.778Z Reads: 254

```
Can be a reason yes. How long your battery wires?
```

---
## \#3 Posted by: linsus Posted at: 2018-09-09T19:36:32.667Z Reads: 252

```
could be a number of things. I personally never run anything above 10s on any 4.x hardware. (dont own F-boxes)
```

---
## \#4 Posted by: pixelsilva Posted at: 2018-09-09T20:50:37.859Z Reads: 240

```
[quote="BooYA, post:1, topic:67531"]
12s4p 30Q, dual focbox with 5065 140kv motors running FOC sensored at 40amps 60k erpm .
[/quote]



Think the 60.000 erpm is top limit for the Focbox. 12s will go way over that. You need to maintain things below 60k at around 53.000 erpms to play on the safe side. That in turn allows you to use only 8s or perhaps 9s before traspassing the 60K threshold.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-09-09T21:00:18.784Z Reads: 216

```
He run 140kV motors...you will not reach the 60k max erpm with it. Not with 12s.
From 190kV you could get troubles.
But there also only if you pull your trigger fully on fully charged batteries and without load.
As soon as you stay on your board you will lower the max erpm.
```

---
## \#6 Posted by: Sourcecode Posted at: 2018-09-09T21:23:31.488Z Reads: 210

```
Been running 2 focbox for over a year now, in foc, 500mm 8agw batt wires, 12s and 200kv motors (although limited to 60000 in the settings) 65 motor max and 60 battmax. Haven't had any problems so far
```

---
## \#7 Posted by: E1Allen Posted at: 2018-09-10T02:07:57.142Z Reads: 189

```
He was running FOC, so no erpm limit. Also no one runs 8/9s with focbox. 10-12s is more normal and plenty do it without fail.  You shouldn't run into any issues with focbox properly setup.
```

---
## \#8 Posted by: dareno Posted at: 2018-09-10T06:16:41.479Z Reads: 172

```
There are so many factors here that can cause failure in a vesc.  At those settings you should have been safe although at 40 amps per controller you are at the limit with that battery.  12s is usually safe on focboxes over any other vesc4 derivative but so many other things can weigh in.  Are you unduly stressing the board out with steep hills in your area?  Are your belts like guitar strings? Are the vescs secured in the enclosure safe from vibration? Are they cooled sufficiently? These are all things that have tripped me up.  Without knowing the exact set up you have its almost impossible to provide an answer to the question posed.
Oh and sometimes if you look at esk8 electronics with one eye half shut and the other open they will fail.
every time.
```

---
## \#9 Posted by: BooYA Posted at: 2018-09-10T21:49:12.281Z Reads: 155

```
Thanks guys for your inputs, I will try to add caps and report here. Also I'm really lightweight, I almost never go full power on my board, never had overtemp issues and my Focboxes are mounted using extra thick double sided foam tape... I'm the '' careful '' type of builder.
Just wondering if 12s is usually safe on Focboxes
```

---
## \#10 Posted by: Jasonkimberson Posted at: 2018-09-11T14:13:20.288Z Reads: 143

```
How many other people do not have the esc right next to the battery and added caps?
```

---
## \#11 Posted by: Deckoz Posted at: 2018-09-11T15:38:01.473Z Reads: 145

```
[quote="Deckoz, post:33, topic:65801, full:true"]
Look here is the truth. It doesn’t matter the series count. Over 13s you will kill escs no matter what

I think the real problem is people’s builds

* vibration dampening
* good soldering
* good covered connections
* good dust proofing
* not taping or hot gluing pinned connections in place
* using antispark switches with the wrong type of fets so when it fails it doesn’t backflow to battery and the ESC blows
* having a shitty power connection or your board is off, remote is on and you are rolling fast enough to generate bemf to power on the controller, it brakes and there’s no where for the current to go and it pops.

I think most Focbox failures are related to all the above which is basically user error.

Basically the margin for user error is high on any voltage… lol
[/quote]

That's all I'm saying... Lol
```

---
## \#12 Posted by: Battosaii Posted at: 2018-09-11T15:55:43.307Z Reads: 130

```
Oh and 60k Erpm limit does not apply to the Focbox it's been tested way above 100k Erpm
```

---
## \#13 Posted by: 12meterkuk Posted at: 2018-09-11T16:43:14.275Z Reads: 125

```
What do you mean by no erpm limit in foc? Does that mean It can run at any erpm even over 100k?
```

---
## \#14 Posted by: telnoi Posted at: 2018-09-11T17:11:15.635Z Reads: 122

```
No Xtra caps, about 40cm of wire in between focboxes and lipos, 12s, 50A battery amps, 80 motor, dual 6374. Total weight 120 kg and I bomb up hills off-road.

I'm using true copper 10awg silicone wire though. Noticed that most cables don't actually seem to have copper strands.
```

---
## \#16 Posted by: Schulerbible Posted at: 2019-01-14T08:39:03.183Z Reads: 94

```
I would add static electricity also to the list. I've seen a lot of ppl touching their ESCs with bare hand w/o any sort of anti statics protection.
```

---
## \#17 Posted by: Pantata Posted at: 2019-01-27T23:15:06.996Z Reads: 75

```
Yes, the myth about 60k erpm on focbox is a myth. Tested upto 100k or maybe even more. Posted by enertion.
```

---
## \#18 Posted by: Arek Posted at: 2019-01-27T23:38:48.636Z Reads: 75

```
You can have plated copper strands.
```

---
## \#19 Posted by: telnoi Posted at: 2019-01-28T11:01:16.649Z Reads: 65

```
Not sure. The typical stuff you buy from say Hobbyking is silver colored rather than copper. What I have now is much darker and towards brown/red/orange.
```

---
## \#20 Posted by: Battosaii Posted at: 2019-01-28T11:08:39.841Z Reads: 65

```
Mine is def plated or coated cause when you cut it you can see copper in the ends.
```

---
## \#21 Posted by: AlexBE Posted at: 2019-01-29T03:21:39.023Z Reads: 46

```
The best way to tell is simply to weigh the cable. Copper is 3 x heavier than Aluminium. In weight sensitive applications like quadcopters, you actually want Aluminium cable for higher conductivity to weight ratio.
```

---
