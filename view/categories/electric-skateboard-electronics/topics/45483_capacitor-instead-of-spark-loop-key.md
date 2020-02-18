# Capacitor instead of spark loop key?

### Replies: 47 Views: 1641

## \#1 Posted by: RosyRoseman Posted at: 2018-02-03T19:55:26.499Z Reads: 269

```
I don't have much experience with reading schematics, but would a system [as outlined here](https://www.illinoiscapacitor.com/pdf/Papers/spark_suppression.pdf) be sufficient to stop sparking? Or why not? I'm not a huge fan of having a vital removable piece that can get lost... Thank you!
```

---
## \#2 Posted by: chomp Posted at: 2018-02-03T20:04:19.573Z Reads: 269

```
As far as I’m aware an anti-spark key is just a resistor.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-02-03T20:04:39.398Z Reads: 269

```
This would work, but you have to calculate the resistor value to keep the VESC on all the time or it would not work, and by that you would constantly drain the battery 

Basically to not have a spark the potential of both sides of the plug must be almost the same

Another way would be to have a momentary push button that engages the spark suppression a few seconds before you turn of the main switch, you don’t even need the capacitor

But you still would need a XT60 or something like that to serve as primary current path

Basically this design complicates things compared with a XT60 antispark or an electronic anti spark
```

---
## \#4 Posted by: RosyRoseman Posted at: 2018-02-03T20:09:57.272Z Reads: 254

```
So what would a pushbutton system look like? And would it be damaged if you turned the system on without pushing the button? Also, what is the order of operations of the spark key, what I mean is, when do you put it in/take it out? And thank you!
```

---
## \#5 Posted by: Namasaki Posted at: 2018-02-03T20:38:08.999Z Reads: 230

```
The problem I found when trying to create a simple anti spark system using a resistor on a 12s system is that if the resistor was completing the circuit for more than a second, it started overheating.
```

---
## \#6 Posted by: Sebike Posted at: 2018-02-03T21:35:03.450Z Reads: 205

```
Like this you mean? ![DSC_1382-01|690x388](upload://UUv3r34x3rfzyZunpYqD2un0ck.jpeg)
A two switch switch 😋
```

---
## \#7 Posted by: Achmed20 Posted at: 2018-02-03T21:54:55.907Z Reads: 188

```
im not realy experienced  with electronics either but i think
the problem is not realy the spark, but rather the high current. the resistor would help preventing the spark, but the switch would just melt in the process.
```

---
## \#8 Posted by: krloz Posted at: 2018-02-03T21:56:53.033Z Reads: 186

```
Exactly.  You will still need a switch rated for tens of amps. Preferably also up to 56V. That sounds big
```

---
## \#9 Posted by: Sebike Posted at: 2018-02-03T22:14:18.955Z Reads: 181

```
This is what I use. Don't know amp rating, but no problems yet.

https://laughingsquid.com/wp-content/uploads/ESCIFstreetart.jpeg
```

---
## \#10 Posted by: krloz Posted at: 2018-02-03T22:15:57.042Z Reads: 175

```
 That thing won't do.
It doesn't have a nice led
```

---
## \#11 Posted by: Sebike Posted at: 2018-02-03T22:18:47.093Z Reads: 167

```
No, but it has a built in movie theater and a bar.
```

---
## \#12 Posted by: krloz Posted at: 2018-02-03T22:25:03.759Z Reads: 163

```
[quote="Sebike, post:11, topic:45483"]
bar
[/quote]

Yeah you got me there. 

I'm pretty sure that switch could fit a couple of trucks motors vesc.... and make it rideable
```

---
## \#13 Posted by: Sebike Posted at: 2018-02-03T22:28:43.446Z Reads: 155

```
yeah. That's not an esk8, that's a motorized switch.
```

---
## \#14 Posted by: krloz Posted at: 2018-02-03T22:30:57.011Z Reads: 162

```
Anything flat with trucks and motors is an esk8
```

---
## \#15 Posted by: krloz Posted at: 2018-02-03T22:33:31.979Z Reads: 161

```
![Sandwich-Skateboard|640x319](upload://vugqTl7potqVh75ge5M7mZzCzf6.jpg)
```

---
## \#16 Posted by: Sebike Posted at: 2018-02-03T22:43:12.453Z Reads: 157

```
2 flat boxes with /monster/ trucks and motors. Esk8s?

https://i.ebayimg.com/images/g/U1cAAOSwdnZaNBNu/s-l500.jpg
```

---
## \#17 Posted by: chomp Posted at: 2018-02-03T23:06:27.336Z Reads: 146

```
Not sure about the pushbutton part of your question but the easiest way I use the loop key is to use an xt-90 like: https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html 

I place one of these on the positive cable between the battery and esc. I put it in before I ride and remove after. Bonus points if it's attached to one of these: https://www.amazon.com/Rotary13B1-Insert-Before-Flight-Keychain/dp/B007UL4JKE

Regardless, if you're still into the switch idea, check out this thread: http://www.electric-skateboard.builders/t/vedder-anti-spark-switches-for-sale-from-18/31847 Sounds kind of like what you're looking for.
```

---
## \#18 Posted by: krloz Posted at: 2018-02-03T23:44:01.950Z Reads: 131

```
I would certainly ride that... up for sale?
```

---
## \#19 Posted by: Pedrodemio Posted at: 2018-02-04T02:27:37.359Z Reads: 123

```
Depends, most people say they never damaged an ESC/VESC by spark, you see people running airplanes at 14S without anti spark, but you do erode the connector overtime

The best approach is or use an electronic anti spark ou a XT90S that has the anti spark resistor built in. I prefer the electronic one since it looks more clean and professional
```

---
## \#20 Posted by: RosyRoseman Posted at: 2018-02-04T19:29:27.145Z Reads: 103

```
What kind of specs should I use for this resistor? Would I also use a resistor in a loop-key setup, and would it be the same size as this one?
```

---
## \#21 Posted by: Sebike Posted at: 2018-02-04T20:11:34.791Z Reads: 91

```
The resistor size was actually discussed in the loop key thread you were referring to earlier. XT90s uses a 5.6 ohm resistor, but you're not bound to use that value to make it work. 

The "momentary push button then switch on" schematic I drew is probably possible, but not the easiest solution.. Remember that all your current will go through that push button when riding your board, which means it needs to be amp-rated accordingly. It also needs to be vibration proof, so it doesn't give continuous cut-outs and sparks..... No good.. 

If you use the XT90S you don't need to worry about the resistor as it's included in the plug.
```

---
## \#22 Posted by: laurnts Posted at: 2018-02-04T20:30:55.330Z Reads: 82

```
Here is the thing about antispark, its easy to build. I've did manual switch antispark system with double switch.

What cause the spark is the capacitor draining so much current directly from the battery. What does antispark does is limit the amount of current the capacitor takes with a resistor. You only need a resistor of 10ohm to do it.

So how does double switch mechanism work? the first switch is momentary switch with 100 ohm resistor, you trigger that (since there is a resistor), it doesn't spark at all. It will take about 0.5 sec to fill the capacitor. After the capacitor is filled, you can trigger the primary switch (theres no spark), because the capacitor is already filled in and so there won't be inrush current that will be pulled from the battery. This is the basic mechanism of an antispark system.
```

---
## \#23 Posted by: krloz Posted at: 2018-02-04T20:52:16.676Z Reads: 79

```
I've thought a lot about That idea.  To turn on less power hungry equipment like buck converters that would drain max 5A but still have an input cap. The thing is I have only found double switches that have each On position on either side of the Off. Ie. On-Off-On.  Wich woulda be ok as long as you don't get the sides mixed. Ideal would be an Off-On-On switch with the resistor on the centre On. That way flipping the switch from one side to the other would turn on whatsoever going first through the spark resistor. 
The thing is in not sure that kind of switch exists
```

---
## \#24 Posted by: ZackoryCramer Posted at: 2018-02-04T21:07:54.178Z Reads: 77

```
Same. I used the anti-spark on a 13s battery and it instantly blew.
```

---
## \#25 Posted by: laurnts Posted at: 2018-02-04T21:13:58.765Z Reads: 82

```
No this never be the case. It only blew if you turn the antispark switch system without connection the primary switch. So basically drawing so much amp through the resistor, ofc it blew. But if you use the antispark system just to fill in the capacitor charge and then switch on the primary switch, its no problem. Thats why its best to use momentary switch on the antispark switch so it will never blow.
```

---
## \#26 Posted by: Sebike Posted at: 2018-02-04T21:34:38.208Z Reads: 79

```
Just realized how the double switch schematic should be done. duh...

![DSC_1384-01|690x388](upload://g8lTaLHwAQGG4gix8uVBss2T1i1.jpeg)
```

---
## \#27 Posted by: Achmed20 Posted at: 2018-02-04T22:01:27.708Z Reads: 77

```
your problem would be the switch.
just try to look up switches which can handle 50A+ and see how large they are
```

---
## \#28 Posted by: Sebike Posted at: 2018-02-04T22:04:22.830Z Reads: 77

```
Well that's about exactly what I said, and that's why I suggest using a simple xt90s loop key.

@laurnts did use this on a previous build though and could probably share more about how his switch held up.
```

---
## \#29 Posted by: Achmed20 Posted at: 2018-02-04T22:23:44.867Z Reads: 74

```
beside the switch issue, im pretty sure your last drawing wont work.

**edit: attention > bullshit answer from me ahead ;)**
_you just created a paralel circuit and this way.  you'd still get the spark in the main switch._
_your first drawing was actualy right (besides missing a capacitor to bridge the powerless once the tactile button is released)_
```

---
## \#30 Posted by: faithfulpuppy Posted at: 2018-02-04T22:38:20.163Z Reads: 72

```
no that schematic looks like it would work. Close the top one, then the bottom one. It's exactly the same way that the xt-90s loopkey works
```

---
## \#31 Posted by: Achmed20 Posted at: 2018-02-04T22:43:40.865Z Reads: 72

```
ups, you are right. i kinda forgot that the spark is only created because there is no flow at all.
also, i was still thinking about the "melting switch" problem ^^
```

---
## \#32 Posted by: Sebike Posted at: 2018-02-04T22:49:51.587Z Reads: 73

```
while I was thinking about the melting witch problem

http://www.urbanbaby.com.au/WebRoot/Store/Shops/UrbanBaby/5255/FCE4/A4C2/645E/04DB/C0A8/DA0B/0725/BSWitchDetail.jpg
```

---
## \#33 Posted by: RosyRoseman Posted at: 2018-02-04T22:59:11.803Z Reads: 69

```
This may be a dumb question, but the spark look key completely replaces an on/off switch, right?
```

---
## \#34 Posted by: Sebike Posted at: 2018-02-04T23:00:18.365Z Reads: 68

```
yes 100000chars
```

---
## \#35 Posted by: laurnts Posted at: 2018-02-05T13:37:26.484Z Reads: 60

```
The diagram is correct. I use the exact same diagram. Please note that what causes the spark is the instant draw of high amp by the capacitors. If the capacitors is fully charged (with an antispark), it won't make the spark. The same exact reason if you plug the main (no antispark here), it will create huge spark. But if you unplug it for approx 0.5second and plug it back in, there won't be a spark.

I agree that there is no small switch that can handle 50A, however I use DPST switch and make them work in parallel. Single line can handle 15A - 20A, so when it's double it will hold 40A++. AGAIN, please don't make such statement if you don't know what are you dealing with especially about amp draws. I agree that there will be a moment that the switch needs to handle 40A up to 100A, but this draw only last not more than couple of seconds. So this switches will do just fine without melting down. I've ridden many times, uses the switches many times over the course of 2 years without any issues. Anyway if you're so keen enough to look how much constant amp draw from the motor (use amp meter or vesc log), they only draw 1 - 3Amp constant and not 50A / 100A.

And let me tell you why there is no constant 50A draw like all member here are saying. Imagine you have 10s4p (36v 10Ah) in which the standard of batteries used by alot of members here. Say your motor draw 50A constant. Now convert that 10Ah (10 Amp Hours) into Amp seconds. 10 * 3600 = 36 000As. Now 3600 As / 50As =  720. You have 720 seconds = 12 minutes. Now question your self, does anyone here ride for about 12 minutes of rides with single or dual setup on full battery? I guess not...... don't be fooled by amps.
```

---
## \#36 Posted by: PXSS Posted at: 2018-02-05T15:32:37.783Z Reads: 55

```
Your math is correct but it is extremely hard to read and your units are out of whack. 

Hope you don't mind me fixing it. 

10Ah Battery (Amp*hour)
50A constant discharge (Amps) 

10Ah/50A = 0.2h (Amp * hour / amp = hour)
0.2h * 60 = 12mins (hour to minutes conversion)
```

---
## \#37 Posted by: laurnts Posted at: 2018-02-05T15:41:19.530Z Reads: 51

```
Yea I was doing it real quick, made some mistakes. But well this was explained alot multiple times, but i guess some newer member might have missed it.
```

---
## \#38 Posted by: PXSS Posted at: 2018-02-05T15:44:39.715Z Reads: 55

```
Yep yep. I fully agree with you.
I think it's dumb for people to be building batteries that can do >100A continuous :)
```

---
## \#39 Posted by: Achmed20 Posted at: 2018-02-05T17:13:31.172Z Reads: 54

```
people living int the alps or san francisco might disagree here ;)
```

---
## \#40 Posted by: RosyRoseman Posted at: 2018-02-05T17:18:15.375Z Reads: 51

```
Sorry for the small questions, I'm trying to understand the discourse. The "instant draw of high amp by the capacitors" is referring to the V/ESC caps, right? Not some extra anti-spark control capacitor? If this is the case, would a sliding potentiometer that goes from a high resistance to zero resistance (assuming it could handle the amps I suppose) work? 

Could you elaborate on your DPST switch? Do you use an arming button with it?
```

---
## \#41 Posted by: RosyRoseman Posted at: 2018-02-05T17:46:30.185Z Reads: 45

```
Ooh! Or Maybe [This Switch?](https://www.mouser.com/ProductDetail/CW-Industries/G-1328S-0031?qs=sGAEpiMZZMtHXLepoqNyVabJQRveLwH14IFeviemHg4%3d) With it running in parallel as you said and a resistor in the middle position?
```

---
## \#42 Posted by: Vanarian Posted at: 2018-02-05T18:27:15.928Z Reads: 44

```
May I ask why you don't go for a proven reliable layout if the double switch / resistor idea is not an improvement? To me it looks like a complication and potential failure point.

Why not simply do one of these solutions : 
- put loop key inside a protected cavity within your enclosure / add a cover where it may plug
- get an anti-spark module with a classic switch from @GoldenHusky (he has DirectFET versions if you really feel the need)
```

---
## \#43 Posted by: RosyRoseman Posted at: 2018-02-05T19:49:57.845Z Reads: 40

```
Because I am making these plans to run at a Makerspace. We will be offering classes for all ages and walks of life, and the simpler I can make it (fewest removable parts, least number of steps to turn on and off) the better. And while I understand that an e-switch with mosfets is the easiest to operate, we are also trying to keep costs down and affordable, and every e-switch I've seen is ~$50. If it was just for me, I wouldn't have a problem with the loop key, or two-button setup, but for the lowest common denominator...
```

---
## \#44 Posted by: Vanarian Posted at: 2018-02-05T20:09:17.755Z Reads: 37

```
Ok got it. Then really the loop key _is_ the best solution, cost effective and literally anybody from the baby age to the good ol' grandpa knows the use of a key and how to use it.

Really make a nice looking case for the XT90 loop printed in 3D so it doesn't _look_ like an electronic plug anymore and voilà. 

What's simpler for the common people than inserting a key into a vehicle to start it ?
```

---
## \#45 Posted by: RosyRoseman Posted at: 2018-02-05T20:13:05.475Z Reads: 36

```
I think you've convinced me. I'm just worried that people will lose it or do something else dumb that I can't foresee, like accidentally stick something in the socket board-side...
```

---
## \#46 Posted by: Vanarian Posted at: 2018-02-05T20:24:57.041Z Reads: 35

```
Nah make the plug big enough so it can't be put in the wrong pins :wink:
```

---
## \#47 Posted by: laurnts Posted at: 2018-02-06T00:41:23.297Z Reads: 34

```
Just find dpst swtich that runs 20A. Since its double you can use both sides that will run 40A in total. Yet it will run 40A only for a few seconds, so evsn single seitch would manage.

Anti spark is a resistor only be used to fill capacitor bank of vesc or esc. Thats all no more no less... So it only require 100ohm resistor and a momentary switch. It only need to close the circuit no more than 1second. Dont make things too complex for your self.

The most idiot proof build and simple is loop key. This is what I use in the end. Its the most cost efficient and reliable.
```

---
