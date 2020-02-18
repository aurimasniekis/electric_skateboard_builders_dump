# Battery pack won&rsquo;t turn on while connected

### Replies: 29 Views: 2751

## \#1 Posted by: zool774 Posted at: 2015-10-25T23:06:15.467Z Reads: 77

```
Hi guys
It seems like I can't figure out what's going on with my E-board,  I definitely need help cause this thing is driven me nut...... 
Here's the situation:
Ive a battery pack purchased from Alien Power System, 6S 8000 mAh, 5065 275 kv Outrunner motor from APS as well, EZRUN MAX 8 ESC 150A, and and a Quantum reciver/transmitter 2.4 Ghz from Hobbyking. 
The battery pack turn on normally whenever is disconnected, the voltage meter built in shows the correct voltage (22.8)  but as I  wire evening together the battery pack won't even turn on, and the voltage meter shows the voltage amount for a second then it fades off. I've discovered that by disconnecting the negative wire, between the battery and the esc, only then the battery will turn on, and if I reconnect the wire back the all system start working normally, till I turn the battery pack off. 
I've already replaced the esc unit, with a way better one then the  original so definitely that wasn't causing the issue. 
Unfortunately I can't replace all the part lol I'm not that rich,  so I was hoping to get some heads up here. 
Please guys,  any input will be more then welcome. 
Thanks again
```

---
## \#2 Posted by: psychotiller Posted at: 2015-10-25T23:27:27.593Z Reads: 69

```
Man, that is frustrating..I would test the components individually.
battery and just esc.
esc, motor and a different battery.
esc, battery and different motor..

What's the max amp output of that battery?

Hope you get it sorted out soon!
```

---
## \#3 Posted by: zool774 Posted at: 2015-10-25T23:37:41.258Z Reads: 65

```
Trust me man, it is really frustrating lol
I don't really have another battery to check them  individually. I've checked the  battery output witha voltage meter so far, it seems in terms of voltage is fine but I don't know another way to check the overall output. 
The battery pack should have a 35C discharging rate, if that was you were asking.
```

---
## \#4 Posted by: psychotiller Posted at: 2015-10-25T23:47:08.106Z Reads: 59

```
Maybe you could go to a local hobby shop or E-bike shop and they'll let you plug in a battery? If not let me know and I'll ship you a battery and you can just send it back to me after you test everything. 

Output would be my concern. Maybe it has a faulty cutoff built into it.
```

---
## \#5 Posted by: zool774 Posted at: 2015-10-26T00:07:28.970Z Reads: 59

```
Good idea.... I'll look for an hobby store and see what happening. 
Thanks so much for helping and the support, hopefully I'll find it out soon what's wrong with it
```

---
## \#6 Posted by: zool774 Posted at: 2015-10-26T00:20:02.816Z Reads: 60

```
New updates.... 
I've just checked the battery pack, connected with the esc only,  no motor, and same problem, so you were right, it has to be something in the battery. 
I got to contact the guy at the Alien Power System one more time, extremely disappointed with those products, I'll probably ask for the full refund and ship everything back, so here I go again looking for a new  set up lol
```

---
## \#7 Posted by: psychotiller Posted at: 2015-10-26T00:47:29.191Z Reads: 57

```
That sucks..from everything I have read I have chosen to stay away from aps. Not because of bad customer relations, just too many issues.
I believe the west coast warehouse for hobby king has stock again. 
Multi star batteries aren't that pricy and are good. You could also check with subcreative about his packs.
```

---
## \#8 Posted by: zool774 Posted at: 2015-10-26T01:11:41.395Z Reads: 54

```
You won't believe this; the esc stopped responding, 
No way to program it anymore, it's not holding the setting anymore....... Now I'm pissed
```

---
## \#9 Posted by: zool774 Posted at: 2015-10-26T01:21:14.704Z Reads: 56

```
I wish I knew it..... 
Ill check those guys out, now I got to start from scratch..... Definitely no more Alien Power System stuff, that's total garbage.
```

---
## \#10 Posted by: psychotiller Posted at: 2015-10-26T01:40:26.391Z Reads: 56

```
Seriously? Hobbywing will take care of you. Switch it for the max6. Worst case, once you get your refunds, I've been holding on to some parts, fit a build.  I have a Bigfoot 160 motor and an Ezrun pro 150a.
```

---
## \#11 Posted by: zool774 Posted at: 2015-10-26T01:44:27.091Z Reads: 55

```
Ok one more thing, I still need your help if you don't mind, I'd like to order a new motor before they run out off stock. So for a single drive E-board, with 90mm wheels, 16T/44T drive wheel kit, riding mostly on flats, just a bit of inclinations sometime, 
not really hills,  150lb rider,  what typeof  motor and what battery should I  get? 
Thanks again man
```

---
## \#12 Posted by: emotiva Posted at: 2015-10-26T02:01:28.483Z Reads: 55

```
6354 size (nominally specifies the diameter as 63mm and length as 54 mm) seems to be a popular choice, as it typically allows enough room for dual motors on the same truck if you decide to go that route at some point. That said, if you know you want to go with one, a longer one, like 6374 will allow more torque/power, although for flat ground and at 150lb, you probably don't have to worry about that. I don't personally have experience with this, as of yet, but from what I've read, that's the case. There's tons of information to soak up here and at the  endless sphere forums regarding this. I know the Turnigy sk3 series is pretty well regarded, as is the enertion r-spec. I have both ordered, but have not used either yet. 

The common wisdom at the moment appears to suggest ~230-260 kv for a 6s setup, whereas the 190 kv of the enertion rspec appears well-suited to 10s or 12s battery setups. Of course, gearing plays an important role. This calculator might help get a feel for what to expect with gearing ratios, motor rating, etc. http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html. 

Give some of the build threads a read and see which builds appeal to you, to get an idea of what to model yours after.
```

---
## \#13 Posted by: zool774 Posted at: 2015-10-26T02:18:21.548Z Reads: 53

```

Thanks for the  load of useful info, I appreciate that you took the time to write back, thanks again. 
One more question; whats the difference, in terms of power and performance between the 6354 and the  6374?  What's the length means?
```

---
## \#14 Posted by: psychotiller Posted at: 2015-10-26T02:22:24.779Z Reads: 51

```
@emotiva @zool774  That sounds about right. My best builds have used motors between 245 and 290kv. at 6s when geared correctly they perform very well. Even climbing! And I weigh 200lbs. Depending on the wheels I'm using I shuffle between 14/32, 16/36 and 14/42. 

My Tacon bigfoot 160 is 6364. $55 bucks.
```

---
## \#15 Posted by: zool774 Posted at: 2015-10-26T02:28:55.734Z Reads: 49

```
I've heard the tacon are quite beefy, but there is no way to find them anywhere, do u have a secret store where they are still available?
```

---
## \#16 Posted by: psychotiller Posted at: 2015-10-26T02:30:16.314Z Reads: 47

```
I have a secret box in my shop with one in it. I don't think there are any more anywhere.
```

---
## \#17 Posted by: emotiva Posted at: 2015-10-26T02:39:17.037Z Reads: 46

```
I found this a while back. Lots of information on which other motors are made by the same factory and rebadged.. 
http://www.rcuniverse.com/forum/brushed-brushless-motors-speed-controls-gear-drives-123/11426913-chinese-factories-make-various-brushless-motor-brands-2.html
```

---
## \#18 Posted by: zool774 Posted at: 2015-10-26T02:40:12.316Z Reads: 45

```
Hahaha 
Well if you are in a mood of charity, I wouldn't mind to buy it...... Lol
```

---
## \#19 Posted by: zool774 Posted at: 2015-10-26T02:44:41.508Z Reads: 44

```
No wander why all the suppliers are out of them, cause of one major factory make them all.....  they do the same with flat screen tv lol
```

---
## \#20 Posted by: psychotiller Posted at: 2015-10-26T02:53:42.064Z Reads: 45

```
Yeah just let me know.
```

---
## \#21 Posted by: zool774 Posted at: 2015-10-26T03:11:38.347Z Reads: 44

```
Ok Great!!! Let's do it!!!
```

---
## \#22 Posted by: psychotiller Posted at: 2015-10-26T04:12:38.360Z Reads: 45

```
@zool774  Just Paypal me $55 and I'll ship it to you this week!
```

---
## \#23 Posted by: zool774 Posted at: 2015-10-26T04:36:13.991Z Reads: 45

```
ok copy that.......thanks again
btw I may need a new enclosure lol I let u know
```

---
## \#25 Posted by: psychotiller Posted at: 2015-10-28T11:25:30.409Z Reads: 42

```
Did you get my PayPal email? I need your address
```

---
## \#26 Posted by: zool774 Posted at: 2015-10-29T22:31:46.646Z Reads: 41

```
Hey D
you ve mentioned something like to get the Max6 instead or you have one for sell?
btw I got my $back from Hwing
```

---
## \#27 Posted by: psychotiller Posted at: 2015-10-30T00:09:11.500Z Reads: 41

```
I have a 6s ezrun pro, but you should get the max 6 because it's 8s compatible.
```

---
## \#28 Posted by: Zac13 Posted at: 2018-05-18T20:50:37.093Z Reads: 18

```
If you want an extra pair I have 2
```

---
## \#29 Posted by: psychotiller Posted at: 2018-05-19T00:11:59.129Z Reads: 16

```
LOL Nope! I'm good  Thanks
```

---
## \#30 Posted by: Sender Posted at: 2018-05-19T01:48:28.658Z Reads: 14

```
Reviving a 3 year old thread... sick!
```

---
