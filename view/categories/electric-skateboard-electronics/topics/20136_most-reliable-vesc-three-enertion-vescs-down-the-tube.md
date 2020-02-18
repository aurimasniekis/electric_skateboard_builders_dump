# Most reliable VESC? Three Enertion VESCs down the tube

### Replies: 34 Views: 3538

## \#1 Posted by: Alanhunt123 Posted at: 2017-04-02T08:48:58.163Z Reads: 379

```
Hi all,

I've been using Enertion VESC v4.12 boards for a while, and I've just gone through my third (only paid for 1, thankfully), and all have given me the drv8302 error. This third one was a used one from Enertion, that they said had thorough testing, and had worked fine. 

The last 2 saw a pampered operating environment in terms of temperature, as they were mounted in my custom made aluminum case, with direct mosfet heat sinking. Made hill climbs easy with a single motor! So I can't imagine I have had any temperature issues. 

I'm quite disappointed with the lack of reliability these boards have been giving me. I've kept the battery current at 50A or less, and the motor current 120A or less, which I've heard is fine. I've heard of others using 200A on the motor without issue.

So, my question is, who sells the most reliable VESC? Is the VESC-X any good? At this point I'm hesitant to try anything else from Enertion...
```

---
## \#2 Posted by: smurf Posted at: 2017-04-02T09:00:38.412Z Reads: 368

```
Some people fix them. Some pics would help.
```

---
## \#3 Posted by: Alanhunt123 Posted at: 2017-04-02T09:05:09.398Z Reads: 365

```
Not interested in fixing it, I've had that done for the past two boards, so I have doubts that this one will be any different.<img src="/uploads/db1493/original/3X/f/c/fc6c4f52084b2de3b0acec71d91ce8ac63862b21.jpg" width="690" height="388">
No burn marks on the DRV, just like the last two boards, it just gave up.
```

---
## \#4 Posted by: dogeatgod Posted at: 2017-04-02T10:04:07.792Z Reads: 359

```
Do you insulate/separate phase wire push connections on motor connection. I didn't once and although very little exposed I reckon a short here caused a DRV to fail, just like yours, no visual evidence just game over. Like you I'd taken so much care with settings, heat and current draw just missed something simple.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-04-02T10:31:53.103Z Reads: 356

```
120A for the motor is already very high. 200A is recommended by hummie and makes absolutely no sense. 
Do you run in FOC or BLDC? And did you have errors where the VESC shut down in between before they died? And did you do a proper motor detection? 
And I would not recommend to go higher than 100A for motor max to give the VESC the chance to handle current spikes a bit better.
```

---
## \#6 Posted by: Alanhunt123 Posted at: 2017-04-02T11:03:49.426Z Reads: 342

```
The mosfets are rated for well over 200A if I recall correctly, so I don't think the 120A limit really caused any issues. Besides, it would only be able to deliver that 120A up to around 41% duty cycle, at which point the 50A battery limit would kick in. (120A * 0.41 = ~50A) I would like to keep a higher motor current setting, as it makes startup torque and smoothness so much better than when it was set to 80A.

So far, nobody has answered my question as to what VESC they think is the most reliable.
```

---
## \#7 Posted by: Alanhunt123 Posted at: 2017-04-02T11:05:27.329Z Reads: 337

```
I did have the motor wires insulated, so I don't think that was the issue.
```

---
## \#8 Posted by: dogeatgod Posted at: 2017-04-02T11:55:56.372Z Reads: 330

```
I've only used Enertion so can't really advise.

Ollin boards have great reviews and customer service - try @ Chaka
```

---
## \#9 Posted by: Jebe Posted at: 2017-04-02T12:10:40.015Z Reads: 331

```
<img src="/uploads/db1493/original/3X/4/a/4a4ff61bc402927d115549b50d7ae1fce796c5e3.JPG" width="281" height="500">
Only 3? Lucky you. I'd try ollinboards. My vesc x died just as easy as the standard enertion vesc.
```

---
## \#10 Posted by: onloop Posted at: 2017-04-02T12:25:04.795Z Reads: 322

```
@jebe, We offer extended warranty that covers faults & also covers user error to a certain extent....
http://www.enertionboards.com/electric-skateboard-parts/1yr-vesc-x-replacement-warranty/?setCurrencyId=1

From our experience, if you keep having the same problem over & over again you might need to rethink your setup to be sure nothing else is causing the fault.
```

---
## \#11 Posted by: onloop Posted at: 2017-04-02T12:27:14.519Z Reads: 311

```
if you can show us some photos of your enclosure that would be good, how did the vesc get the dirt on it? was the vesc protected with some shrink tube?
```

---
## \#12 Posted by: Alanhunt123 Posted at: 2017-04-02T12:36:57.656Z Reads: 313

```
This is my setup. Perhaps a little dirt was able to get through the holes for the wires.

http://www.electric-skateboard.builders/t/upgrading-from-8s-to-10s-with-vesc-and-245kv-6364-sk3/18019/25?u=alanhunt123
```

---
## \#13 Posted by: mmaner Posted at: 2017-04-02T14:18:29.487Z Reads: 291

```
You are using the most reliable VESC and keep burning them up, so noone really knows what to tell you.
```

---
## \#14 Posted by: Hummie Posted at: 2017-04-02T16:09:53.685Z Reads: 301

```
Id think Olin or axle vesc more tested and reliable
http://www.electric-skateboard.builders/t/safety-psa-vesc-x-users-partial-recall-read-if-you-have-a-new-vesc-x/17043
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2017-04-02T16:21:59.492Z Reads: 293

```
@Hummie the problem with these unit was that the resistor they place where still passing the test, and it was a complete manufacturer  error, NOT A PROBLEM WITH THE DESING. 

@Alanhunt123 I can read that you use a 245KV with a 10S battery.... I do not recommend that kind of configuration since the VESC is more sensible with high ERMP, you don't want to exceed 60k, or it can damage the DRV. (245 * 42 * 7 = 72 030 ERMP). You can put the MAX ERPM at 60K, but still your borderline with the limit of your electronic.
```

---
## \#16 Posted by: mmaner Posted at: 2017-04-02T16:28:05.755Z Reads: 295

```
[quote="Hummie, post:14, topic:20136"]
Id think Olin or axle vesc more tested and reliable
[/quote]

Probably Olin, but aren't people having g issues with delivery times?  Seems like I've read a couple of time where people have waited weeks. 

Axle, I don't know.  They seem pretty new.  I've read that @longhairedboy likes them.  I might give them a try. 

Honestly I usually buy VESCs based on my support experience, meaning it's more valuable to buy from someone that I KNOW is going to be there to assist.  

I'd have to recomend @oriol360 or @torqueboards, both have been awesome for me.  But their VESCs do not have the upgraded FETs like the VESC-X, which is why I thought it strange to look for a "better" VESC. 

Frankly, after 3 I'd think it was an issue with another component causing the problem, not the VESC itself.
```

---
## \#17 Posted by: Alanhunt123 Posted at: 2017-04-02T16:45:15.974Z Reads: 283

```
@JohnnyMeduse I have my ERPM limited to 50k, which is plenty fast for me, and also well under the 60k limit. 

I found the issue, it seems my VESC case had too sharp of edges on the wire holes that it cut a tiny slit in two of my motor leads, and led to a short. 😣

Looks like I'll have to fix that, and that should fix the issue once I get a new VESC.
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-04-02T17:00:04.482Z Reads: 278

```
[quote="Alanhunt123, post:17, topic:20136"]
it seems my VESC case had too sharp of edges on the wire holes that it cut a tiny slit in two of my motor leads, and led to a short. :persevere:
[/quote]

Maybe using some type of grommets, so the wire won't be in direct contact with the enclosure. :wink:

<img src="/uploads/db1493/original/3X/3/a/3acece0605fab71832de7988f33fa02c255296b8.jpg" width="375" height="500">
```

---
## \#19 Posted by: Pantologist Posted at: 2017-04-02T19:41:57.545Z Reads: 258

```
This board looks like it has salt on it. What is all the white powder stuff?
```

---
## \#20 Posted by: Alanhunt123 Posted at: 2017-04-02T20:58:44.858Z Reads: 247

```
@Pantologist You mean the stuff that's on the MOSFETs? That's CPU thermal paste. I used it to help transfer heat to the aluminum enclosure.
```

---
## \#21 Posted by: chuttney1 Posted at: 2017-04-02T21:33:49.494Z Reads: 231

```
OP could always wait for VESC 6.0.
```

---
## \#22 Posted by: Jebe Posted at: 2017-04-02T21:54:39.867Z Reads: 232

```
I've bought the warranty, been told I'm not covered but not why.. Set-up?  2 enertion vescs to 2 r specs connected by can
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2017-04-02T21:59:19.337Z Reads: 235

```
Sorry @Jebe, could you please handle your problem with enertion in private and stop hijaking other people thread...

I you want send them to me and I will handle the repair free of charge...

Regards 
JF
```

---
## \#24 Posted by: Alanhunt123 Posted at: 2017-04-02T22:01:38.576Z Reads: 228

```
[quote="chuttney1, post:21, topic:20136, full:true"]
OP could always wait for VESC 6.0.
[/quote]

I could, but that would mean no esk8 for me for several months!
```

---
## \#25 Posted by: Pantologist Posted at: 2017-04-02T22:56:37.909Z Reads: 218

```
The board looks to be in a toasted shape. The JST connectors are all warped and the board is covered with crud... I don't know what the aluminum case looked like but it seems to just contain the heat within the area of the VESC instead of moving it away.
```

---
## \#26 Posted by: flatsp0t Posted at: 2017-04-02T22:59:17.871Z Reads: 211

```
The warped JSTs are normal for the 4.12 Enertion vescs, their shrink wrap is too tight.

But tere also seems to be a bit too much thermal paste.
```

---
## \#27 Posted by: Alanhunt123 Posted at: 2017-04-02T23:05:44.077Z Reads: 221

```
[quote="Pantologist, post:25, topic:20136"]
I don't know what the aluminum case looked like but it seems to just contain the heat within the area of the VESC instead of moving it away.
[/quote]

My aluminum case is detailed below. I don't quite follow, it was specifically designed to sink the heat from the MOSFETs to the casing, which has lots of airflow from the movement of the board. This should sink heat away from the board better than most solutions out there, since it is made of aluminum. Only copper and gold beat aluminum in terms of thermal conductivity.

http://www.electric-skateboard.builders/t/upgrading-from-8s-to-10s-with-vesc-and-245kv-6364-sk3/18019/25?u=alanhunt123
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-04-03T14:06:54.491Z Reads: 202

```
[quote="mmaner, post:16, topic:20136"]
Axle, I don't know.  They seem pretty new.  I've read that @longhairedboy likes them.  I might give them a try.
[/quote]

HEre's my take on AXLE at the moment:

I bought three VESCs from AXLE recently. Two of them are working amazingly well, and i do really like them. They actually behave a lot like the VESC-X despite being more of a traditional 4.12 with the usual mosfet type and pcb layout. 

The other one was throwing undervoltage errors and i'm sending it back. I have not had a minute to start the RMA process, but i think that if their service turns out to be "yeah let us take care of that for you no problem" kind of service, then Ollin will have some serious competition in the VESC 4.12ish market. If they don't deliver a good experience, then Ollin will still be the clear winner. 

I have ollin VESCs that have been in customer's boards for almost a year with no issues. I simply can't say that about anyone else's yet.
```

---
## \#29 Posted by: smurf Posted at: 2017-04-03T18:02:54.225Z Reads: 185

```
Where do you get your grommets?
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2017-04-03T18:23:55.893Z Reads: 184

```
McMaster... but I think you need a compagnie address
```

---
## \#31 Posted by: longhairedboy Posted at: 2017-04-10T13:27:16.570Z Reads: 162

```
just wanted to update my comment and say that when I contacted AXLE they simply sent me a shipping label and said to send it back in. 

That's what i'm talking about. Customer Service.
```

---
## \#32 Posted by: Alanhunt123 Posted at: 2017-04-10T14:42:12.072Z Reads: 158

```
Wow! Nice to hear that getting your VESC fixed has been going smoothly. Fortunately, someone from Enertion contacted me and has offered to repair my VESC. So, looks like I might still get some life out of this board!
```

---
## \#33 Posted by: curtis Posted at: 2019-12-20T17:20:08.604Z Reads: 27

```
Holly crap they give you a whole year warranty when you pay $300 for the fox-box. I would at least expect a 2 year warantee maybe even a 5 year one because if it's only one year that you stand behind your products. Generally that means they suck if they only last 1 year.
```

---
## \#34 Posted by: deucesdown Posted at: 2019-12-20T23:32:31.504Z Reads: 24

```
3

Year

Necro
```

---
