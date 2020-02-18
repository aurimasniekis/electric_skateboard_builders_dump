# Low Cost Buck Converter for Esk8

### Replies: 29 Views: 2494

## \#1 Posted by: JdogAwesome Posted at: 2016-12-13T00:11:36.446Z Reads: 206

```
Ive seen a lot of people looking for UBEC's or other step down converters for there boards, to power things like LED's, USB Chargers, etc. Problem is most of them are expensive and output at 5V and/or are not built for Esk8. I was looking around for something like this to power a set of LED lights, and I couldn't find any good options. So I decided to look into creating an HV step down converter. Eventually I came across the LM2576HVS-12 Simple Switcher which takes anywhere from 4-60V input and steps it down to 12V at a max of ~3A. I put together a parts list and some schematics for building something like this and the price per piece came out to only around $1.50 per module, buying in semi-bulk. Ill provide a BOM and schematics once ive sorted it all out completely, but I wanted to see if anybody would be interested in something like this, either for building themselves or for purchasing one fully assembled. And please drop any questions, comment or concerns below!

**[GitHub Repository](https://github.com/JdogAwesome/Esk8-UBEC)**
```

---
## \#2 Posted by: smurf Posted at: 2016-12-13T00:28:00.903Z Reads: 198

```
Why 12 volts ? I thought led's run at between 2-5 volts natively and need to be tuned to the right voltage with a resistor anyway. I don't really know what's more efficient
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-12-13T00:36:44.586Z Reads: 188

```
https://www.ebay.com/itm/381807336269
```

---
## \#4 Posted by: JdogAwesome Posted at: 2016-12-13T01:28:11.563Z Reads: 169

```
[quote="smurf, post:2, topic:14573, full:true"]
Why 12 volts ? I thought led's run at between 2-5 volts natively and need to be tuned to the right voltage with a resistor anyway. I don't really know what's more efficient
[/quote]

This would be for LED Strips or LED Lights that normally run on 12V.
```

---
## \#5 Posted by: jmasta Posted at: 2016-12-13T01:50:33.210Z Reads: 158

```
[quote="smurf, post:2, topic:14573, full:true"]
Why 12 volts ? I thought led's run at between 2-5 volts natively and need to be tuned to the right voltage with a resistor anyway. I don't really know what's more efficient
[/quote]

Most LEDs have a forward voltage of 1.9 - 2.0 V.  You can string 6 together in series and run them off 12V without a resistor.  I plan on doing that for my tail lights.  My headlights are 12V already and are very very bright
```

---
## \#6 Posted by: JdogAwesome Posted at: 2016-12-13T01:51:06.614Z Reads: 149

```
Hey @Michaelinvegas thats actually very interesting because I hadn't seen anything like that before. Though like I said in the main post, it isn't necessarily built for Esk8 and it costs $6.29 shipped, while mine would cost just around $1.50 per module.
```

---
## \#7 Posted by: JdogAwesome Posted at: 2016-12-13T01:53:01.773Z Reads: 146

```
<s>Be careful doing that though because the first LED in that string will be carrying the current of all the other LED's in said string and it can die prematurely due to higher current. That works fine if your doing it in just short chains, but for longer strings, its better to have separate smaller chains of LED's. <s>
```

---
## \#8 Posted by: jmasta Posted at: 2016-12-13T01:55:34.695Z Reads: 141

```
[quote="JdogAwesome, post:6, topic:14573, full:true"]
Hey @Michaelinvegas thats actually very interesting because I hadn't seen anything like that before. Though like I said in the main post, it isn't necessarily built for Esk8 and it costs $6.29 shipped, while mine would cost just around $1.50 per module.
[/quote]

Just curious, why does it need to be specifically "built for esk8"?  An LED doesn't care whether it's on a skateboard or not :wink:

The lower cost would be great though.  My 12V 3A BEC was like $15 shipped from Amazon, since I didn't want to wait for it come from China

[quote="JdogAwesome, post:7, topic:14573, full:true"]
Be careful doing that though because the first LED in that string will be carrying the current of all the other LED's in said string and it can die prematurely due to higher current. That works fine if your doing it in just short chains, but for longer strings, its better to have separate smaller chains of LED's.
[/quote]

They are in series, so every LED in the loop sees the same current
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-12-13T02:05:21.098Z Reads: 127

```
Hey I'll take 5 at buck fifty ... as long as don't gotta put it together lol
```

---
## \#10 Posted by: JdogAwesome Posted at: 2016-12-13T02:11:44.962Z Reads: 130

```
[quote="jmasta, post:8, topic:14573"]
Just curious, why does it need to be specifically "built for esk8"?  An LED doesn't care whether it's on a skateboard or not :wink:
[/quote]

Yeah I know that kinda sound stupid "Built for Esk8" lol. What I meant more of was its built by people in the community so you can have more support because you would be talking directly to the creator or whatever, instead of some guy in China using the crappiest google translate software out there. 

[quote="jmasta, post:8, topic:14573"]
They are in series, so every LED in the loop sees the same current
[/quote]

Ahh your right sorry lol, I guess I was thinking parallel, woops.
```

---
## \#11 Posted by: saul Posted at: 2016-12-13T02:28:37.402Z Reads: 123

```
I've used this one. and these too

I think this is pretty similar to the lm2576hvs. but adjustable output. I have a few they work ok but they dont recommend more then 30V difference. 
http://www.ebay.com/itm/LM2596HVS-LM2596HV-DC-DC-Adjustable-Step-Down-Buck-Converter-Power-Supply-Module-/310788581728
```

---
## \#12 Posted by: JdogAwesome Posted at: 2016-12-13T02:31:21.513Z Reads: 114

```
Yeah uses a very similar IC. Though that one is still $3.11 so building this one would be cheaper, but that is definitely a good alternative. I was more looking to see if people were interested in this, and possibly building one themselves, if there into that, then really finding the cheapest option.
```

---
## \#13 Posted by: saul Posted at: 2016-12-13T02:33:38.192Z Reads: 108

```
I bought 10 so its only about 1.5-2 each. are you sure you're counting pcb and time to build them?

unless you add in something like led driver, switch pins...I don't think it would be worth it. they are very similar.
```

---
## \#14 Posted by: JdogAwesome Posted at: 2016-12-13T02:35:43.604Z Reads: 101

```
If your building this on like perf board, then there goes PCB cost pretty much lol. And Like I said this is mainly for people who want to build there own and get the experience. Though i definitely get were your coming from.
```

---
## \#15 Posted by: Michaelinvegas Posted at: 2016-12-13T02:41:37.105Z Reads: 97

```
Yeah I find the adjustable ones can't handle dropping the voltage down....that's why I just get the one with a fixed output ...that's not perfect either but it's closer to 12v output at 13v
```

---
## \#16 Posted by: saul Posted at: 2016-12-13T02:43:42.143Z Reads: 98

```
yea perf board takes time tho. it is really simple just 4 caps, 1 diode, 1 resistor, 1 pot, 1 to package.

@Michaelinvegas this one seems to hold output voltage constant, just gets hot bucking 12s (50v) down to 12v...
should work fine with 6-8s.
```

---
## \#17 Posted by: JdogAwesome Posted at: 2016-12-13T02:44:20.614Z Reads: 97

```
Also have you used that LM2596HVS at more than 40V because I cant find a datsheet for the LM2596HVS, so I was thinking it might be a re-branded LM2596 which can only handle 40V.
```

---
## \#18 Posted by: saul Posted at: 2016-12-13T02:48:44.911Z Reads: 95

```
no its a high voltage version. works for up to 60v. I've used on 12s fine. I'll test it a bit more to see how warm it gets.
```

---
## \#19 Posted by: JdogAwesome Posted at: 2016-12-13T02:50:54.875Z Reads: 97

```
Well do be careful because ive seen some videos were right when they get to about 50V the thing stops regulating... so yeah, heres the link https://www.youtube.com/watch?v=JLwJb4MVbls
```

---
## \#20 Posted by: saul Posted at: 2016-12-13T02:58:27.390Z Reads: 97

```
Yea I saw that video, seems like a bad batch. I don't have an adjustable supply that goes that high so I just tested with 12s pack.
```

---
## \#21 Posted by: Michaelinvegas Posted at: 2016-12-13T03:01:06.119Z Reads: 89

```
I use it for 12s .. it works
```

---
## \#22 Posted by: JdogAwesome Posted at: 2016-12-13T03:02:03.869Z Reads: 87

```
Alright well if there working for you then thats good. If you do ever want to test anything at its limit, I got a cheap 60V boost converter for testing some of my circuits out at high voltages. http://www.ebay.com/itm/New-DC-DC-Boost-Converter-10V-32V-to-12V-60V-Step-Up-Power-Supply-Module-100W-/111687919495?hash=item1a011e6787:g:EegAAOSwstxVOvdK
```

---
## \#23 Posted by: treenutter Posted at: 2016-12-13T18:58:31.768Z Reads: 78

```
@JdogAwesome Yes I'd buy a few! I'd buy one assembled and then some kits so I can copy the build. I'm a visual learner :) 

I need soldering projects for the winter.
```

---
## \#24 Posted by: JdogAwesome Posted at: 2016-12-13T19:10:41.663Z Reads: 73

```
Good to hear! Stay tuned for when I start selling the kits, or full assembled versions.
```

---
## \#25 Posted by: JdogAwesome Posted at: 2016-12-13T23:25:41.793Z Reads: 70

```
I created some schematics for the UBEC, there still early versions and im sure ill make revisions, but its a start. Also I created a GitHub Repository for a place to store the .brd and .sch files. [LINK](https://github.com/JdogAwesome/Esk8-UBEC)

<img src="/uploads/db1493/original/3X/3/9/39c7b6deddefaa169c86b761699a2591c3232862.jpg" width="689" height="379">
<img src="/uploads/db1493/original/3X/e/1/e183930f5f3020f6c21dd385e3ad17f13af22c1c.jpg" width="690" height="331">
```

---
## \#26 Posted by: FredSaberhagen Posted at: 2016-12-14T21:24:18.364Z Reads: 61

```
Dude!  Please use planes (not traces) for your layout.  You want to minimize resistance and inductance especially on an input path to the buck converter - because it's discontinuous you will see large di/dts.

That big package (looks like TO-220) - why do you think it has such a huge pad on the opposite side of the 5 fingers?  That's what it wants to dissipate all its heat through - and it has an integrated switch, meaning that's where all the heat is generated.  Copper is FREE (all they do is remove it in process) and your package design depends on copper to pull the heat away from the package and increase your surface area to radiate heat from.  You can also spec 2oz copper foils instead of standard 1/2 oz and get a little lower Tja.

Great idea to build a schematic/PCB , you will learn a bunch from it, but hell no should you send them out for sale and advertise them as made for esk8 until you understand the design.  That three dollar one on amazon is probably a lot more robust and therefore a better pick for esk8.  And it's had all the cost optimized out of it by buying in large quantity - yours is gonna be more expensive.

Another good idear would be strain relief for the contacts.  Punch a hole through the PCB by those exposed pads and you can run the wire thru the hole then over to the SMT pad.  Any stress on the wire will then be taken up by the insulated part on the hole, and not your solder pad ;-)  At the very least stitch your SMT pads with a couple vias and that'll give you some through-board strength (not just relying on epoxy holding that very small pad down). Esk8 = high vibration environment!!
```

---
## \#27 Posted by: JdogAwesome Posted at: 2016-12-14T21:46:02.115Z Reads: 62

```
[quote="FredSaberhagen, post:26, topic:14573"]
Dude!  Please use planes (not traces) for your layout.  You want to minimize resistance and inductance especially on an input path to the buck converter - because it's discontinuous you will see large di/dts.
[/quote]

Was definitely going to do that, I realize the current pads were way to small for the contact area on the back of the package.

[quote="FredSaberhagen, post:26, topic:14573"]
That big package (looks like TO-220) - why do you think it has such a huge pad on the opposite side of the 5 fingers?  That's what it wants to dissipate all its heat through - and it has an integrated switch, meaning that's where all the heat is generated.  Copper is FREE (all they do is remove it in process) and your package design depends on copper to pull the heat away from the package and increase your surface area to radiate heat from.  You can also spec 2oz copper foils instead of standard 1/2 oz and get a little lower Tja.
[/quote]

Like I stated before hand, I was planning on expanding the pad size. And I was planning on using 2oz copper anyways.

[quote="FredSaberhagen, post:26, topic:14573"]
Great idea to build a schematic/PCB , you will learn a bunch from it, but hell no should you send them out for sale and advertise them as made for esk8 until you understand the design.  That three dollar one on amazon is probably a lot more robust and therefore a better pick for esk8.  And it's had all the cost optimized out of it by buying in large quantity - yours is gonna be more expensive.
[/quote]

First off I wasnt "sending them out for sale and advertisement" this was merely to see if people were interested in something like this, and I was just saying I might consider selling them as well, thats all. I totally understand that mine may end up being more expensive looking over were to source parts from, though like I said before, this was to gauge interest in the topic. 

[quote="FredSaberhagen, post:26, topic:14573"]
Another good idear would be strain relief for the contacts.  Punch a hole through the PCB by those exposed pads and you can run the wire thru the hole then over to the SMT pad.  Any stress on the wire will then be taken up by the insulated part on the hole, and not your solder pad :wink:  At the very least stitch your SMT pads with a couple vias and that'll give you some through-board strength (not just relying on epoxy holding that very small pad down). Esk8 = high vibration environment!!
[/quote]

Those are great ideas and I will definitely look into doing that, I know how shitty the copper adhesive can be lol. And yes I know Esk8 has a hell of a lot of vibrations, trust me my legs after riding on bricks know that a lot better than I do. You clearly have a very good understanding of PCB design and board layouts, and I thank you for your comments.
```

---
## \#28 Posted by: FredSaberhagen Posted at: 2016-12-14T22:01:45.527Z Reads: 55

```
Cool and I think you should still do it.  If you go in for a job interview and show them some shit you designed and built they will immediately throw all other applications in the trash.  Please post up your progress.  Another suggestion - a real connector footprint rather than just some SMT solder pads.  Crimp-and-poke FTW or even an IDC connector would be super easy and robust.  if you need to ever service it don't want to grab a solder iron every time you need to pull it out ;-)
```

---
## \#29 Posted by: JdogAwesome Posted at: 2016-12-15T01:33:48.570Z Reads: 56

```
Thanks for the kind words! I will make sure to update my progress here, but it will be slow because I have a lot of other stuff going on as well, if you, or anyone else, want to try and improve any of the designs or whatever, feel free to do so! I will definitely add some connectors I was just using pads for place holders mainly. I was thinking about just using some standard screw terminals like  [these](http://www.alpha-crucis.com/3468-5255-thickbox/screw-terminal-block-2-pin-35-mm-pitch-side-entry-4-pack.jpg), because of there simplicity and ease of use.
```

---
