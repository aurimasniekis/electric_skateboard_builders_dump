# \[New Builder\] Battery capacity tester

### Replies: 10 Views: 1338

## \#1 Posted by: Mox Posted at: 2016-10-21T09:13:05.145Z Reads: 155

```
I want to permanently mount a capacity tester on top of my board so that I know how much juice I have got left while riding.
I came across this unit which is supposed to be water resistant. 
https://de.aliexpress.com/item/Batteriekapazit-t-Tester-Anzeige-12-V-24-v-48-v-auto-blei-s-ure-batterien-lithium/32580155072.html?btsid=9ae9ad6e-d04a-4314-8dd3-790be26f373c&ws_ab_test=searchweb0_0%2Csearchweb201602_3_10065_10068_10069_10084_10083_10017_10080_10082_10081_10060_10061_10062_10056_10055_10054_10059_10078_10079_10073_10070_421_420_10052_10053_10050_10051%2Csearchweb201603_4&spm=2114.010208.3.1.0qdUng

Im running a 12s battery (4x 3s in series) and a vedder Anti spark switch. 
The question is where do you hook the voltage tester up and how? I am a newbie when it comes to electronics.
Also, will I be able to monitor the capacity of the 4 batteries in series as if they were one? Or do I need 4 Testers.

Thanks in advance!
```

---
## \#2 Posted by: jmasta Posted at: 2016-10-21T16:39:58.579Z Reads: 131

```
Wire the red wire to the positive (+) lead of the anti-spark switch output / VESC input.  Wire the black wire to the negative (-).  Red to red; black to black.

Please don't take this the wrong way, but it slightly worries me that you are building a high power electric vehicle and don't know how to wire a voltmeter...  I trust you can do it with enough research.  Just don't burn down your house :wink:
```

---
## \#3 Posted by: Mox Posted at: 2016-10-21T17:06:06.018Z Reads: 125

```
Will try. :dizzy_face:
Thanks man!
```

---
## \#4 Posted by: Aborn Posted at: 2016-10-22T23:41:05.704Z Reads: 106

```
Please enlighten me. What is a antispark and what is its purpose?. my board will have a permanently mounted battery my plan is to just have a switch to turn it on and off.
```

---
## \#5 Posted by: sl33py Posted at: 2016-10-22T23:56:30.626Z Reads: 101

```
[quote="Aborn, post:4, topic:11615, full:true"]
Please enlighten me. What is a antispark and what is its purpose?. my board will have a permanently mounted battery my plan is to just have a switch to turn it on and off.
[/quote]


the higher the voltage - the more of a spark you will get when connecting the battery each time.  Or turning it on.  Usually i'd suggest if you are 8s-12s range to use anti-spark switch or anti-spark loop key.  You could also use it for 6s, but i don't feel it's quite as needed.  Each time it "sparks" it wears away some of the metal, so over time your switch and battery contacts will wear/erode away eventually.

Simplest solution - an XT-90s anti-spark loop key.  Stupid simple and a fun quick project if you have a decent soldering iron, some basic solder skills, and a few minutes of time to spare:
http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

A push button anti-spark switch is also nice.  There are a few from Enertion, DIYes, Ollin BC, MEB, esk8.de that vary in price.  Personally i really like the v1.3 and newer v1.4 Vedder/Fechter anti-spark switches.  Myself and @DeathCookies have a few "kits" left (you assemble yourself from components), or you can buy one from the above.  

Ultimately it boils down to a $5-10 loop key, or electronic switch for a bit more.

GL!
```

---
## \#6 Posted by: Aborn Posted at: 2016-10-23T00:17:30.747Z Reads: 86

```
Thanks!

But wouldnt that be the same as having a power switch connected to the positive lead?

Can you link me one of those kits that you have?
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-10-23T16:42:07.925Z Reads: 76

```
[quote="Aborn, post:6, topic:11615"]
But wouldnt that be the same as having a power switch connected to the positive lead?
[/quote]

No. a normal switch would let flow ALL current the battery can deliver and the VESC capacitors need through the switch in milliseconds. Thus you would get a spark again.

The switches offered by Enertion, DIYes, Ollin BC, MEB, esk8.de or by our kit would let the current flow slowly into the capacitor of the VESC and that way there will be no spark.
[quote="Aborn, post:6, topic:11615"]
Can you link me one of those kits that you have?
[/quote]

Please use the search function:

Vedder anti spark kit. Then you will find the thread of @sleepy and me.
```

---
## \#8 Posted by: Aborn Posted at: 2016-10-23T16:43:21.167Z Reads: 72

```
Thanks a lot! :slight_smile:

I will deffinitely get one of those
```

---
## \#9 Posted by: Shunbear Posted at: 2016-10-25T02:44:52.417Z Reads: 59

```
What's the difference between the v1.3 and v1.4 vedder anti spark switches?
```

---
## \#10 Posted by: mmaner Posted at: 2016-10-25T02:55:25.990Z Reads: 57

```
This is how I wired my volt meter (Drok DC8).  

<img src="/uploads/db1493/original/3X/3/d/3d5a35ee25a88e4712e3bf9e0b0c68ec5cb6b348.jpg" width="690" height="435">

Both use 5.5 mm connectors.  With the on in the left I used solod core copper, bent it to a 90 and pushed it through the holes in both of the connectors and filled up the barrels with solder.  With the one on the right I did what my dad calls a "slip splice".  I stripped about 1/4 of the jacket and wrapped an inch of the 18 gauge wire around it, solderd it and made sure I got a good flow through the center wire.  I've tested both, they are identical in performance.  

Also, there the added benefit that I can take them.out and solder another lead on pretty easily if I wanted to connect something else, without having to touch the system wires (battery's, ESC, motor phase wires, etc).
```

---
