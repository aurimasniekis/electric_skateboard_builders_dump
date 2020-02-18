# Cheap anti spark kill switch idea. will it work?

### Replies: 29 Views: 2508

## \#1 Posted by: nimbuskate Posted at: 2017-05-26T09:32:28.995Z Reads: 271

```
i thought of using one of the car audio circut breaker 100amp with a anti spark system with momentary button.. total cost should be about $20 which is a cheap option
can anyone tell if this going to work out?

<img src="/uploads/db1493/original/3X/0/c/0c2cb6814c83ec4f1f317ea47583094f90573772.jpg" width="500" height="500">
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-05-26T09:42:28.760Z Reads: 258

```
Sure it will work, but why so complicated?
Get an antispark loop key. Cheaper and smaller :slight_smile:
```

---
## \#3 Posted by: nimbuskate Posted at: 2017-05-26T09:46:20.841Z Reads: 252

```
dosnt looks too complicated.. i thought it would be nice to turn on the board with a flick of the switch and pushing a small button at the same time instead of pluging and pulling the darn xt90.. those things are super tight!
```

---
## \#4 Posted by: nimbuskate Posted at: 2017-05-26T09:47:19.341Z Reads: 244

```
plus! no loop key to loose!
```

---
## \#5 Posted by: TarzanHBK Posted at: 2017-05-26T10:04:01.495Z Reads: 232

```
hmm sounds more complicated for me :smiley:

Cheapest solution is always the loop key. If you don´t like it, or like a more simple solution, go for a vedder antispark. which is not much more expensive than your solution. And you can get a much cooler LED button :slight_smile:
```

---
## \#6 Posted by: krloz Posted at: 2017-05-26T11:01:39.923Z Reads: 217

```
Not "at the same time though". First press the button and then Flick that switch/fuse. Otherwise you could still get a spark inside the switch
```

---
## \#7 Posted by: Tuomalar Posted at: 2017-05-26T11:08:25.465Z Reads: 202

```
So you just want more parts which can break.
```

---
## \#8 Posted by: KTMinni Posted at: 2017-05-27T00:16:21.549Z Reads: 181

```
Why are you guys ripping on him for thinking outside the box?  I think it's an interesting idea, don't crap on creativity.
```

---
## \#9 Posted by: saul Posted at: 2017-05-27T00:53:57.378Z Reads: 184

```
out of the box thinking is great, but in this case there are some oversights.

for one, car audio is only 12v! so thats a big one.
next up I don't think something like this would survive the vibration of esk8.
and finally aniti spark switches have already dropped below $30.

and of course you can just tether your key loop to the board for the $5 winner.


https://www.amazon.com/STEREO-AUDIO-CIRCUIT-BREAKER-INLINE/dp/B00DD9EKTM
```

---
## \#10 Posted by: KTMinni Posted at: 2017-05-27T01:31:32.697Z Reads: 164

```
To be honest I hate the idea of a loop key just because of how "janky" it looks
```

---
## \#11 Posted by: Smorto Posted at: 2017-05-27T02:02:18.255Z Reads: 161

```
IMO there are many ways to mount it so it looks clean and professional but again, that is just by opinion.
```

---
## \#12 Posted by: Namasaki Posted at: 2017-05-27T02:15:45.499Z Reads: 162

```
I tried using a similar auto breaker switch when I did my first build.
They work but not for long. Because there are points inside that come together to make the connection and they get arcing everytime you turn it on.  On mine the spring bar that holds the points together got weak from heat and I started loosing connection while riding.
These type of switches are not meant to be turned on and off repeatedly. 
They're meant to stay on all the time as an overload breaker.
If you want cheap, an anti-spark loop key is really the only option.<img src="/uploads/db1493/original/3X/8/3/83fc18fc8e7e3ad71c028da7b7e6dd4030a3ab5c.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/b/8/b8efc3cc84430dc672528b7720ccd8a542696be7.JPG" width="375" height="500">
```

---
## \#13 Posted by: nimbuskate Posted at: 2017-05-27T22:26:47.333Z Reads: 146

```
So i ended up going with the xt90 anti spark.. yes much simpler to setup . Soldered bullet connectors on the xt90 for easy unplugingfor charging <img src="/uploads/db1493/original/3X/2/8/28b458600a3a609cac31bed329efaf0dd3295dbc.jpg" width="666" height="500">and figured out how to unplug and plug easier for charging
```

---
## \#14 Posted by: nimbuskate Posted at: 2017-05-27T22:38:12.326Z Reads: 143

```
This is my build btw a mini electric skateboard<img src="/uploads/db1493/original/3X/1/2/12b00fb3b2ad43e2f9a1fa20273fb78c9982ef04.jpg" width="375" height="500">
```

---
## \#15 Posted by: Namasaki Posted at: 2017-05-27T23:24:33.191Z Reads: 136

```
Good choice for an inexpensive but dependable solution.
```

---
## \#16 Posted by: lowGuido Posted at: 2017-05-27T23:59:55.961Z Reads: 135

```
https://www.instagram.com/p/BP6RyQgh318/
```

---
## \#17 Posted by: Namasaki Posted at: 2017-05-28T00:21:21.238Z Reads: 132

```
Every time you push that button and those contact points snap together, there is electrical arcing between them.
It won't be as damaging at 6s but at 12s it wears them out real fast.
```

---
## \#18 Posted by: lowGuido Posted at: 2017-05-28T00:23:51.014Z Reads: 132

```
been running it for 3 years daily mate. no issues.

(given it is only rated to 24V I probably wouldnt recomend it for 12S)
```

---
## \#19 Posted by: Namasaki Posted at: 2017-05-28T00:28:30.244Z Reads: 131

```
Ok, I never tried them on low voltage. Only on 12s which when it sparks it goes bang!
when I took it apart to see, the points where fried.
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-05-29T11:08:13.784Z Reads: 121

```
I think what you did does not prevent the spark.
Your xt90s is plugged in already, so the small resistor won´t protect the connection!

The way the xt90s works is:
If you plug it in, the first contact is through a resistor, which only allows a small current to close the circuit and prevent a spark that way, which is normally caused by higher voltage.
That all happens fast and you should not leave a xt90s this way for too long, because it will melt down due to the current trying to keep going through the small resistor.
And finally you reach the end position while plugging in, so the resistor is bridged and the current can flow.

So use the connector itself to close the circuit!
```

---
## \#21 Posted by: lowGuido Posted at: 2017-05-29T11:18:32.498Z Reads: 113

```
nah it will work.
so what he does is hold down the button with the resistor that connects the circuit preventing any spark when he switches the breaker on. that way the points on the breaker dont wear out.
@nimbuskate 's solution will work perfectly.
oh wait.. did he not end up doing that?? how did he go from a really elegant solution to cutting an XT90 in half?
```

---
## \#22 Posted by: TarzanHBK Posted at: 2017-05-29T12:44:14.391Z Reads: 107

```
Only works if he cuts the connector with the resistor on one side and the matching socket on the other side i think.
Otherwise you´ll have a constant flow and no spark will be surpressed
```

---
## \#23 Posted by: lowGuido Posted at: 2017-05-29T12:48:28.829Z Reads: 107

```
I liked the breaker, resistor and push button from the OP, that would work well for higher than 6S. hell for 6S you wouldnt even need the resistor.

and I dont see any reason for cutting the connector in half.
```

---
## \#24 Posted by: TarzanHBK Posted at: 2017-05-29T12:58:29.722Z Reads: 108

```
On my 6s with the Xcar i´m not using an antispark neither.
I think most Car Esc won´t have any problem with a little 6s spark. Same thing for the connectors - I´m using 5,5mm bullets and they are totaly fine after lot´s of sparky zipps :slight_smile:
I´d be much more carefull with higher voltage and vesc though!
```

---
## \#25 Posted by: nimbuskate Posted at: 2017-05-30T03:26:58.474Z Reads: 103

```
I cut the xt90 in half so it didnt take more force to plug it in.. lol
```

---
## \#26 Posted by: nimbuskate Posted at: 2017-05-30T03:34:58.015Z Reads: 100

```
i cut the xt90 in half so only the negative is connected only.. the positive side is still unpluged.
```

---
## \#27 Posted by: TarzanHBK Posted at: 2017-05-30T06:43:07.939Z Reads: 96

```
sound like you have to to some workout mate :grin:
Think about if it´s too lose it will come of with a few vibrations.
Better to have it sit tight
```

---
## \#28 Posted by: Smorto Posted at: 2017-05-30T10:21:49.823Z Reads: 88

```
I didn't find the XT90-S hard to plug in myself... I do agree with @TarzanHBK that it should be tight though, you don't want tit coming unplugged mid-ride.
```

---
## \#29 Posted by: mattdig Posted at: 2019-06-04T18:02:31.864Z Reads: 25

```
If anyone else is looking at this, I've had a 100A fuse exactly like nimbuskate for 2 years, at 8s, no anti-spark, and it's totally great (and cheap!).
BUT: that red switch fell off the little nub it's attached to. It's only held on with friction. If you buy a similar unit, pull the switch off (not the button), add glue, put it back. You also need to spray the mechanism with air regularly or it won't spring back to the off position without some coaxing. It's cheap for a reason.
```

---
