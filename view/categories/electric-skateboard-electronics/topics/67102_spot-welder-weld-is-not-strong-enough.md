# Spot Welder - Weld is not strong enough

### Replies: 56 Views: 1303

## \#1 Posted by: Zentaria Posted at: 2018-09-05T14:20:43.664Z Reads: 233

```
Hey there fellow eskaters, I made an Spot Welder using a 600W Microwave and an Arduino and Relais. But when I want to weld a 0.15mm Nickelstrip onto an 18650 battery it doesnt really hold well, its not strong enough.

I am measuring about 1.5V on the secondary winding (using a 35mm² Wire). Also here are some pics if that would help.

Any help will be appreciated!

![20180901_150140|666x500](upload://v5blIDM7z8f0m52Ab2OfLHwL8se.jpg)![20180901_150217|666x500](upload://wZY9tCfTnZbcikMdpILH5S106R1.jpg)![20180901_150153|666x500](upload://1kKuDtCyAKvpgyCRxyccAgMK2sC.jpg)![20180901_150201|666x500](upload://ot1DL4d70VsUnavp8GaJKZhzXDp.jpg)
```

---
## \#2 Posted by: sztamas Posted at: 2018-09-05T14:34:38.926Z Reads: 211

```
What pulse time did you tried? Can we see the welded nickel? Are those electrodes copper?
```

---
## \#3 Posted by: Zentaria Posted at: 2018-09-05T14:59:48.033Z Reads: 207

```
Tried from 50 ms to 450 ms and yes its made from copper. Will post pics soon
```

---
## \#4 Posted by: JonathanLau1983 Posted at: 2018-09-05T15:38:42.315Z Reads: 203

```
@Zentaria I had exactly the same issue, I had the pulse set to about half a second and would see the nickel glow but the weld was crap.
I added another loop to the secondary winding, voltage went up to 3.5 or something and now I need a pulse with of 0.01s to get a nice strong weld.

So try adding another winding to the secondary coil.
![image|666x500](upload://zMNPqlb7zOg4eyGg2IObJdTzBFy.jpg)
```

---
## \#6 Posted by: JonathanLau1983 Posted at: 2018-09-05T16:02:12.314Z Reads: 190

```
[quote="moon, post:5, topic:67102"]
Also, do you happen to have the old relay lying about? I want to make some welds while I wait for the other (better) relay to come from china :D. Could trade for like a motor pulley or something
[/quote]

Who me?
Here's mine prior to the new timer board and case. Three windings. 
![IMG_20180715_150620|666x500](upload://a7hVQaafkdU7MzDuVt3sTqhnJqu.jpg)
```

---
## \#7 Posted by: Zentaria Posted at: 2018-09-05T16:02:15.166Z Reads: 180

```
It has 1 1/2 windings, cable is to thick for another winding
```

---
## \#9 Posted by: Zentaria Posted at: 2018-09-05T16:09:03.747Z Reads: 179

```
Sorry, old timer of what?
```

---
## \#10 Posted by: JonathanLau1983 Posted at: 2018-09-05T16:11:07.673Z Reads: 177

```
I do will PM you
```

---
## \#11 Posted by: moon Posted at: 2018-09-05T16:12:28.005Z Reads: 169

```
Sorry i am confusing things. Sorry

Ignore me
```

---
## \#12 Posted by: Zentaria Posted at: 2018-09-05T17:11:38.688Z Reads: 169

```
Should I try an thinner cable?
```

---
## \#13 Posted by: LukePL Posted at: 2018-09-05T17:18:59.996Z Reads: 157

```
Are you pushing hard? I had the same problem and almost exactly the same setup. No matter what time I put in welds were weak. Than I read somewhere that force that you use is very important. Now without changing anything I'm making welds that won't let go (have tear nickel strip) and my time setting is 0,25s. I'm just touching nickel with electrodes and it works perfect almost zero pressure.
```

---
## \#14 Posted by: Zentaria Posted at: 2018-09-05T17:24:35.419Z Reads: 151

```
Tried it while pushing hard and just laying down, same effect sadly
```

---
## \#15 Posted by: LukePL Posted at: 2018-09-05T17:26:52.121Z Reads: 150

```
Try to barely touch it. When I do that I have big spark and it burns through. 
You are welding nickel not copper strip right?
```

---
## \#16 Posted by: Zentaria Posted at: 2018-09-05T17:31:53.844Z Reads: 144

```
yea I am welding pure Nickel, will try later with just laying down
```

---
## \#17 Posted by: xilw3r Posted at: 2018-09-05T18:37:24.163Z Reads: 140

```
In commercial spot welders there usually is a double pulse weld, the first short pulse like up to 10ms if im not mistaken is meant to soften the material and the second completes the weld. And yes you better be pushing hard on that weldspot. Also, try adding a small cut with a dremel or something in between the electrode touching points on the nickel, makes more current go through the cell casing, ergo better welds. You can see this on all of the chinese premade battery pack nickel strips as well.
Also for trying another loop you might just strip that fat ass insulation and wrap the wire in kapton or somehing, I bet you will have plenty of space left.

@LukePL  0.25 s welds are insanely long my dude :D you need moar powaaa I bet your cells get rather toasty.
```

---
## \#18 Posted by: Zentaria Posted at: 2018-09-05T18:39:25.582Z Reads: 134

```
I actually built a dual pulse spot welder, a short activation and then the time i selected on my menu.Where should I cut it?
```

---
## \#19 Posted by: xilw3r Posted at: 2018-09-05T18:41:11.612Z Reads: 138

```
![image|500x500](upload://pTgzhDBDC5Hbzps3iOFYz1Z7ZAe.jpg)

You see that tiny cut in the nickel? One electrode goes on one side of the cut, another ..well, on the other side.
```

---
## \#20 Posted by: Zentaria Posted at: 2018-09-05T18:42:15.162Z Reads: 132

```
ah thank you, can try tomorrow, but shouldnt it work without the cut too?
```

---
## \#21 Posted by: LukePL Posted at: 2018-09-05T18:42:41.324Z Reads: 128

```
How can I do that? My microwave transformer is 700w. They don't get so hot I think but for sure I need to learn more and have more practice,
```

---
## \#22 Posted by: xilw3r Posted at: 2018-09-05T18:50:18.722Z Reads: 124

```
Yes it should, if your welder has the balls or it. But this thing can help a lot. I was surprised to see the difference with and without that cut.

@LukePL hell man, idk, rewind the transformer like @JonathanLau1983 mentioned, use some fancy mosfets for activating your welder as relays usually have some "bounciness" to them, not sure, but it could compromise the current output to the weld spot.
And if you are going full balls to the wall making many battery packs, you might just go ahead and get a k-weld
https://www.keenlab.de/index.php/product-category/kspot-welder-kit/

We have this at work, powered by 5 supercapacitors in series (2.7 V and I think 1200F each), god damn that thing can weld anything. I personally love it. The darn thing decides on the weld time on its own, because you set the power output in joules. Yea, its smart
```

---
## \#23 Posted by: Zentaria Posted at: 2018-09-11T07:06:18.653Z Reads: 106

```
So literally tried everything mentioned here. Still doesnt weld. Now I dont even see the weld spots, even tho it really gets hot..
```

---
## \#24 Posted by: xilw3r Posted at: 2018-09-11T13:03:52.561Z Reads: 102

```
hot and no weld means you need a way shorter pulse with way more current.
```

---
## \#25 Posted by: Zentaria Posted at: 2018-09-11T13:19:49.273Z Reads: 103

```
It only has 1 1/2 windings an i am measuring 1.5VAC. I dont think the current is the problem
```

---
## \#26 Posted by: xilw3r Posted at: 2018-09-11T13:23:51.436Z Reads: 103

```
Well you described the symptoms that I had to deal with when trying to weld 0.3mm nickel, long pulse low current. 

And we had a really beefy transformer based welder, the aliexpress sunko stuff looks tiny compared to what we had, still no dice. We had to use supercapacitors. The nickel would glow and smoke and all, but the weld would still suck.
```

---
## \#27 Posted by: Zentaria Posted at: 2018-09-11T13:25:18.290Z Reads: 96

```
Oh forgot to meantion, I used times from 50ms to 450ms.
```

---
## \#28 Posted by: xilw3r Posted at: 2018-09-11T13:29:29.069Z Reads: 95

```
450ms is insane, of course the cell will get hot.

Perhaps you cant get enough current since your output voltage is too low, since ...ohms law lol. You said you tried everything, yet didnt mention if you tried to do one more winding on the secondary.

You could try to clean the surfaces well before welding reduce that resistance and junk
```

---
## \#29 Posted by: Zentaria Posted at: 2018-09-11T13:34:30.909Z Reads: 89

```
theres literally no space anymore xD I will try to search an smaller gauge wire
```

---
## \#30 Posted by: moon Posted at: 2018-09-11T13:44:13.165Z Reads: 90

```
6awg wire should be good, thats what @JonathanLau1983 is using

And what I am going to use

That gives you about 3 coils if you buy 1 meter of it.
```

---
## \#31 Posted by: Pedrodemio Posted at: 2018-09-11T13:48:40.315Z Reads: 91

```
This is definitely low current, had the same problem with mine when the battery I was using was crap, you need a lot of current for the shortest amount of time, I use double pulse, the first 1.5ms and second 9ms, you want to tear the nickel when trying to rip it for a strong connection 

You could add a second transformer in parallel

At longer times, you instantaneous power is too low and the heat has time to spread out instead of fusing the nickel and cell together
```

---
## \#32 Posted by: Zentaria Posted at: 2018-09-11T13:52:07.728Z Reads: 90

```
oh my, i am using a 35mm² cable. Guess that is too overkill. Will try to find a thinner cable
```

---
## \#33 Posted by: Zentaria Posted at: 2018-09-12T05:47:53.241Z Reads: 85

```
found a metre of 16mm² cable. That would be good too?
```

---
## \#34 Posted by: moon Posted at: 2018-09-12T10:37:56.201Z Reads: 79

```
Yeah I think that's the same thing
```

---
## \#35 Posted by: JonathanLau1983 Posted at: 2018-09-12T11:49:20.731Z Reads: 82

```
[quote="Zentaria, post:33, topic:67102, full:true"]
found a metre of 16mm² cable. That would be good too?
[/quote]

That's exactly what I used
```

---
## \#36 Posted by: moon Posted at: 2018-09-12T12:33:25.767Z Reads: 81

```
![IMG_20180912_133246|375x500](upload://jDmIoc7ru1zsMc9Jbx0AnRUs6Se.jpg)

3 coils with 6awg
```

---
## \#37 Posted by: Zentaria Posted at: 2018-09-13T12:39:27.697Z Reads: 77

```
Looks good. My Welder still doesnt weld tho. Maybe I should hook up the Copper nail directly to the cable?
```

---
## \#38 Posted by: moon Posted at: 2018-09-13T13:15:48.748Z Reads: 75

```
What with 6awg/16mm2 yeah maybe try direct
```

---
## \#39 Posted by: Zentaria Posted at: 2018-09-13T14:11:14.954Z Reads: 73

```
yea with 16mm².
```

---
## \#40 Posted by: Zentaria Posted at: 2018-09-17T06:32:55.568Z Reads: 73

```
![20180916_133519|666x500](upload://lm19Y4GqaFFaRzFzJEEuubXVwvc.jpg)

Looks fine I guess
```

---
## \#41 Posted by: JonathanLau1983 Posted at: 2018-09-17T17:27:45.302Z Reads: 70

```
Where's the fish paper?
```

---
## \#42 Posted by: moon Posted at: 2018-09-17T17:30:02.119Z Reads: 70

```
Yep fishpaper is needed :slight_smile:

So it works now?
```

---
## \#43 Posted by: Quezacotl Posted at: 2018-09-17T17:50:47.120Z Reads: 69

```
When i made a spot welder, i saw that the connections really matter. Heat goes to the weakest spot on the link. Bad crimp or loose screw etc...
```

---
## \#44 Posted by: Zentaria Posted at: 2018-09-17T18:13:53.039Z Reads: 68

```
No fishpaper, just a ton of Isolation tape. Should work too I guess
```

---
## \#45 Posted by: JonathanLau1983 Posted at: 2018-09-17T18:49:07.038Z Reads: 66

```
Should be adding tape under your nickel strip too then, less useful around the outside like the pic.
```

---
## \#46 Posted by: Acido Posted at: 2018-09-17T18:58:20.758Z Reads: 70

```
just use it, its dirt cheap
electrical tape is too thin


btw the negative terminal is right under this thin plastic 
![Screenshot_6|690x382](upload://d1jnpIjXJO7iQ4YqHJcykYyg9ur.jpg)
```

---
## \#47 Posted by: Zentaria Posted at: 2018-09-17T19:03:33.283Z Reads: 67

```
Yea i did with the other packs. This Was just a test pack
```

---
## \#48 Posted by: LukePL Posted at: 2019-03-18T15:04:43.821Z Reads: 58

```
Sorry for reviving old topic but I have exactly the same problem. I decided to ask for your help before I quit spot welding. I made from two to three turns but is looks like that does'n change anything. When I set it to 0,2 sek it makes some welds but most of the time I can rip it by hand. Super small pcs of strip stays on the cell but it's not strong enough. I want to be able to spot weld because I need to make more than just one battery. Any help is greatly appreciated.![IMG_20190318_141634|375x500](upload://pEIS3eU56B206aaPNnfESwXl8dX.jpeg) ![IMG_20190318_141640|375x500](upload://9eOCe8N0Dlta2PsLJefXHRLPhFi.jpeg)
```

---
## \#49 Posted by: Zentaria Posted at: 2019-03-18T16:56:43.163Z Reads: 56

```
How many Watts does your Transformer have?
```

---
## \#50 Posted by: LukePL Posted at: 2019-03-18T16:59:53.933Z Reads: 56

```
I believe it's 700W. What is notice now that my wires with electrodes are quite long. Maybe that's the of my problem?
```

---
## \#51 Posted by: Acido Posted at: 2019-03-18T18:12:24.202Z Reads: 51

```
Thats not really much, whats your output voltage, I was reading about these DIY spot welder and supposedly if the output voltage is too low the welds will be crap
```

---
## \#52 Posted by: Zentaria Posted at: 2019-03-18T18:31:43.234Z Reads: 50

```
I didn't really have success with holding it by hand so I built that:

https://youtu.be/NVCbswxxYkw

But I am using a 1200Watt MOT. But my weld are a bit too OP, the Nickel kinda gets holes lol
```

---
## \#53 Posted by: LukePL Posted at: 2019-03-18T19:28:49.706Z Reads: 43

```
I can get a 1200W one but would like to know how other welders works using what I have.
I'm kind of tired of failures in this area.
@Zentaria can you show how it welds?
```

---
## \#54 Posted by: Zentaria Posted at: 2019-03-18T19:48:19.826Z Reads: 41

```
What do you mean? I have an Arduino, where I can set the Timer and a foot pedal as a Switch.
```

---
## \#55 Posted by: LukePL Posted at: 2019-03-18T20:01:06.621Z Reads: 40

```
I have also a foot pedal and I can set the time and I can get a 1200W MOT if that's the only way. 
My question was how other welders with transformers like mine works and mine doesn't?
```

---
## \#56 Posted by: Zentaria Posted at: 2019-03-18T20:21:34.046Z Reads: 40

```
Maybe it really has too much resistance when the wires are too long. I would measure the Current and Voltage
```

---
## \#57 Posted by: JonathanLau1983 Posted at: 2019-03-18T21:50:02.376Z Reads: 36

```
Yeah, make the electrode wires are short as you can.
Also, the tips need to be filed quite often as they become oxidised I think it is and go dark. File them.so you get to the bright copper.
```

---
## \#58 Posted by: LukePL Posted at: 2019-03-20T10:23:20.982Z Reads: 30

```
Ok. Making wires shorter seems to help a lot. Still time to make good welds is not super short but it's not bad. 
Lesson is that 700W transformer is bearly enough so everyone whos planning to build one should look for something more powerfull.![IMG_20190320_111820|375x500](upload://uZW9852mTK11kK6ZySjgXtzTw7d.jpeg) ![IMG_20190320_111806|375x500](upload://8v3xqUO5NocFZza7lfmoIPKUn9o.jpeg)![IMG_20190320_113255|375x500](upload://19cKbL0UtIGHAvSqLcWO4uYqjsZ.jpeg)
```

---
