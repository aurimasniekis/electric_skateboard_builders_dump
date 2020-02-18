# 10s8p - what should I set as discharge rate?

### Replies: 22 Views: 406

## \#1 Posted by: Skatejitsu Posted at: 2019-03-29T21:44:54.036Z Reads: 159

```
First time unity setup... I have a 10s8p pack made with sony VTC6 cells.  Racestar 200kv motors.  What should I set as my max discharge rate, or how do I calculate it?
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-03-29T21:48:50.058Z Reads: 158

```
Hi, \
So I don't want to sound toxic but you made a bunch of threads asking a lot of noob questions. There's an own thread for these. OR just use the search function :slight_smile: \
But to answer your question: theoretically, they could supply 120A but also depends on your bms.
```

---
## \#3 Posted by: wafflejock Posted at: 2019-03-29T21:48:50.308Z Reads: 153

```
Take Max discharge of a single cell and multiply by number in parallel, pick something lower than that.  Honestly I end up with motor amps limited because otherwise torque is overkill but still good to set reasonable limits.
```

---
## \#4 Posted by: Skatejitsu Posted at: 2019-03-29T21:54:47.823Z Reads: 146

```
Sorry!  I thought it made more sense to start threads since the questions are all unrelated.  I will keep them in here. 

I have a charge only BMS, so no amps would be pulled through that, but the specs on the motors show this:

**Tested with 36V voltage:**
No load current: 0.9A
No load speed: 7220rpm
Max current: 46A
Max power: 1650W

Does that mean I should set max discharge to 92 (46 x 2) to be safe?
```

---
## \#5 Posted by: Mich21050 Posted at: 2019-03-29T21:56:51.490Z Reads: 138

```
So most vesc's would blow at 50A current. So I would set the battery current to between 45A-50A per vesc and your motor current to somewhere around 40A-45A.
```

---
## \#6 Posted by: Skatejitsu Posted at: 2019-03-29T22:00:52.556Z Reads: 132

```
![unity%20slider|604x290](upload://ep3hXnM11VkblKrcgNXSdOIvqN8.jpeg)  I'm just doing the simple walkthrough on unity setup and it defaults at 60 A on this slider... Their website specs say 80A motor throughput and 160A system. 

So when you say 40-45 per VESC that would be if I had 2 individual VSC's, correct? Since unity is essentially 2 controllers in one I'm assuming on this slider that means I can safely go to 80-90?
```

---
## \#7 Posted by: Mich21050 Posted at: 2019-03-29T22:03:08.328Z Reads: 126

```
That's a question for somebody with a unity. But I'm going to assume that that's the max discharge for the whole unity so I would set it to around 100A (please somebody with a unity double check that) :slight_smile:
```

---
## \#8 Posted by: Skatejitsu Posted at: 2019-03-29T22:35:51.504Z Reads: 116

```
So I've completed the initial setup other than being able to pair the remote.  Here's a super noob question... I have a mini remote.  Do I use the little 2.4ghz receiver module that came with that, or is there already a receiver in the unity?

The setup just says to pull the trigger to calibrate, but there's nowhere in the configuration tools I see to actually pair the remote, which is making me think this receive is supposed to be connected  somehow.
```

---
## \#9 Posted by: Mich21050 Posted at: 2019-03-29T22:38:17.375Z Reads: 109

```
You need to connect your mini remote receiver to your unity.
```

---
## \#10 Posted by: dareno Posted at: 2019-03-29T22:44:57.663Z Reads: 106

```
Do we have pictures of any of this build?  10s8p?  I need pictures and I need them now!
```

---
## \#11 Posted by: pjotr47 Posted at: 2019-03-29T22:54:25.351Z Reads: 105

```
Unity is rated to 140A battery. 

10s8p Sony vtc6 can easy do 160A. 

So the most important thing would be the bms you are using.
```

---
## \#12 Posted by: Skatejitsu Posted at: 2019-03-29T23:29:39.682Z Reads: 97

```
So I'm up and running, with one final issue it seems.  These motors are "clunking", or stuttering almost.  Could this be related to the wrong current settings in my config?
```

---
## \#13 Posted by: Mich21050 Posted at: 2019-03-29T23:33:22.583Z Reads: 97

```
We need a bit more information. Sensored? Bldc of FOC and so on. Also, it would help if you could post some pictures of your settings. :slight_smile:
```

---
## \#14 Posted by: Skatejitsu Posted at: 2019-03-29T23:51:52.541Z Reads: 91

```
![foc%20data|301x500](upload://AjqIadHnecRbZZj0NTiIp5lVFvz.jpeg) 
and these are the motors I have - 
https://www.banggood.com/Racerstar-5065-BRH5065-200KV-6-12S-Brushless-Motor-With-Gear-For-Balancing-Scooter-p-1117658.html?rmmds=myorder&amp;cur_warehouse=CN
```

---
## \#15 Posted by: Skatejitsu Posted at: 2019-03-30T00:13:17.412Z Reads: 84

```
I just realized it's not detecting linkage in the test where you spin the motors by hand. Maybe I need to double check my connections on those sensor wires.
```

---
## \#16 Posted by: Skatejitsu Posted at: 2019-03-30T00:30:13.438Z Reads: 78

```
Got it working!  I didn't actually have wheels connected to my motors yet and just had to spin the motors harder to get the detection to work.  Running smooth now. Thanks for the help everyone.
```

---
## \#17 Posted by: Skatejitsu Posted at: 2019-03-30T00:47:33.711Z Reads: 74

```
I unfortunately don't have any shots of my battery before it was shrink wrapped.  It took a hell of an enclosure to fit everything though and it sucked carrying it last week when my original Evolve ESC fried on me, lol.  I can post pics of the board itself but I'm assuming you're more interested in just the battery.
```

---
## \#18 Posted by: dareno Posted at: 2019-03-30T00:55:54.921Z Reads: 74

```
Interested to see the build in general my friend.  Good to share pics for you and anyone else that wishes to do something similar.
```

---
## \#19 Posted by: Eboosted Posted at: 2019-03-30T02:40:32.940Z Reads: 65

```
Why did you choose a 10s8p battery is a massive battery that would make your esk8 and enclosure look chunky, the weight will crack your back if you need to carry it sometime, completely unnecessary IMHO unless you use it every day to commute 80kms which comming from an Evolve won't be used often
```

---
## \#20 Posted by: Skatejitsu Posted at: 2019-03-30T13:56:12.743Z Reads: 49

```
Yeah it's pretty overboard.  I wanted to be able to go longer distances without ever having to even think about battery being an issue.  Really the only downside so far has been exactly what you said, breaking down in the woods and having to carry it a couple miles.  I will start keeping a shoulder strap of some sort in my backpack.
```

---
## \#21 Posted by: Eboosted Posted at: 2019-03-30T15:17:08.322Z Reads: 41

```
Get a smaller battery, not worth the weight
```

---
## \#22 Posted by: Eboosted Posted at: 2019-03-30T15:22:55.103Z Reads: 37

```
See what battery percentage you have when you get home if it's more than 60% then make a smaller battery and cooler looking board
```

---
