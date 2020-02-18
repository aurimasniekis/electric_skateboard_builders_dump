# High current switch solutions?

### Replies: 45 Views: 13591

## \#1 Posted by: stuxtruth Posted at: 2015-12-17T01:22:53.754Z Reads: 879

```
I'm trying to figure out a solution so that I don't have to open my case and plug/unplug the batteries every time I ride. I do have a power switch on my ESC bit I've heard that you shouldn't use that as an on off switch and that you shouldn't keep your batteries plugged in. My main goal is to have the batteries permanently plugged in and just have an on off switch. Any solution other than the $60 torque boards option?
```

---
## \#2 Posted by: sk8ace Posted at: 2015-12-17T04:07:20.381Z Reads: 882

```
The cheapest solution that I have found is a big circuit breaker. I picked up a ~$7 60amp AC breaker on Amazon to try. My VESC and Motor just shipped so I won't be able to test it until they get in next week. Someone else here mentioned that they also used a circuit breaker (more amps than the one I have) and it worked fine as a switch and never switched off unexpectedly.

Keep in mind that I am not really recommending this as I don't have personal experience using it yet.. It's big, ugly and not  designed to be used as a DC switch.. but it's cheap and may be what you are looking for. I was also turned off by the $60 price tag for torqueboards switch..
```

---
## \#3 Posted by: trbt555 Posted at: 2015-12-17T05:56:02.970Z Reads: 854

```
You could make a loop key. Cheap and reliable. Use the search funtion, you can't miss.
```

---
## \#4 Posted by: longhairedboy Posted at: 2015-12-17T13:48:34.718Z Reads: 845

```
I've tried a number of toggle, rocker, and even slide switches on the power mains. It's not worth it. I use @torqueboards $60 electronic switch because i don't really want to build my own, but its the cleanest option. It allows you to keep your mains in place and then the only other thing you have to worry about if figuring out a charging port option. Unless you're using a space cell, then neither of these things are an issue. 

The tiny little slide or pushbutton switches on the ESCs could easily be replaces by a a different, more durable pushbutton switch that could then be mounted into your box. The switch that's current;y on the ESC may not be able to withstand the abuse of being on the outside bottom of an electric skateboard. 

I don't know why its considered a bad idea to cut power at the ESC while leaving the batteries connected on ESCs that come with outboard power switches. Maybe somebody could enlighten me on this because it makes little sense. It seems like they were designed to work this way.
```

---
## \#5 Posted by: lowGuido Posted at: 2015-12-18T01:36:49.600Z Reads: 789

```
I don't like to leave my batteries hooked up to anything if its not on. "soft power" options scare me a little.
I like to sleep knowing that my batteries are physicaly air gapped from everything and are not going to catch fire and burn me in my sleep because some 2c Chinese Cap went dry.
```

---
## \#6 Posted by: stuxtruth Posted at: 2015-12-18T02:00:31.416Z Reads: 773

```
So basically the only options are:

Loop Key
Big ass circuit breaker
$70 DIY switch

I guess I'll go with loop key. I don't want to take apart my board everytime I want to use it
```

---
## \#7 Posted by: lowGuido Posted at: 2015-12-18T02:15:20.482Z Reads: 754

```
the big breaker is big and ugly. but I have integrated 1 into one of my builds with limited uglyness
http://www.electric-skateboard.builders/uploads/db1493/original/1X/a354b60e467b31e861b120f44f74c36c911814d8.jpg

http://www.electric-skateboard.builders/t/diy-eboard-builds-and-specs/33/34
```

---
## \#8 Posted by: treenutter Posted at: 2015-12-18T13:07:02.869Z Reads: 723

```
@lowGuido I always liked the way you incorporated that! What do you call that circuit breaker? Is it just a "100A circuit breaker" or is it something more specific?
```

---
## \#9 Posted by: lowGuido Posted at: 2015-12-18T13:29:36.468Z Reads: 710

```
yeah it's just a 100A circuit breaker.
```

---
## \#10 Posted by: psychotiller Posted at: 2015-12-18T13:44:31.100Z Reads: 706

```
Look up "hi amp circuit breaker"
```

---
## \#11 Posted by: scoobiext Posted at: 2015-12-22T03:15:00.743Z Reads: 699

```
Try these:
https://endless-sphere.com/forums/viewtopic.php?f=31&t=73800&sid=bd51ce1246574e249e53a2b301400ab1

One cost me about $40 landed in Oz.  They are nice and compact and are soft switching (i.e. no sparking)  I had to assemble the PCB and components (which isn't too difficult) and purchase a SPDT switch from Jaycar (cost about $5 and a few different options).  If you were to upload the design to OSH Park or similar and source the parts from Mouser they would work out a fair bit cheaper.

This is what mine looks like finished, ready for connection to two VESCs:
<img src="/uploads/db1493/original/2X/e/e8a9a906a1a709a4e09a61ecd86965124b4bf869.png" width="690" height="390">

Note that I used fuse wire (3 strands of 16A in parallel) instead of the automotive fuse.

Previous to that I used a loop key in my charge port (wired in series) that worked ok, until I lost my loop key and I didn't like the sparking.

The circuit breaker option looks good as well, although I would be a bit worried about vibration tripping the breaker and you also need to ensure that the breaker is rated at the correct DC current (house type CBs are rated for AC voltage).
```

---
## \#12 Posted by: lowGuido Posted at: 2015-12-22T04:29:19.417Z Reads: 647

```
Yeah I'm not big on that soft power setup for the reasons stated above.

My breaker is ugly. But has never tripped in >700km worth of travel.
```

---
## \#13 Posted by: longhairedboy Posted at: 2015-12-22T21:05:10.726Z Reads: 643

```
i had a problem early in with the switch that came with my original Flier-type dual ESC that came from enertion, but it was the push-switch not the circuit that was the issue. Vibration would throw it. I fixed that eventually with a rocker switch, but when i got the one from DIY i didn't have a problem anymore. I've been using it for a year now with zero issue on my terribly paved streets.
```

---
## \#14 Posted by: lowGuido Posted at: 2015-12-22T22:34:17.255Z Reads: 635

```
my biggest issue with solid state (or soft switching) is that it needs power to work.

don't get me wrong. its great. those FETs can handle loads of current and they are an elegant hi current switching solution.

but. the way it works is that the switch allows a a connection from the b+ to the gate which in turn allows current to flow across the source/drain on the -ve wire.
the switching side (left side in the photo) is ALWAYS live. if I was to use one of those soft switches I would have to physically disconnect my battery every time for piece of mind.

again. 99 times out of 100 there is no issue with leaving the batteries connected to the device, I just dont want to be the 1%
a good friend of mine actually burned his whole house down with lipos. I don't want to play that lottery.
```

---
## \#15 Posted by: treenutter Posted at: 2015-12-23T01:12:46.467Z Reads: 599

```
[quote="lowGuido, post:14, topic:744"]
a good friend of mine actually burned his whole house down with lipos. I don't want to play that lottery.
[/quote]

Word to that! I keep my lipos disconnected in a fireproof bag when I'm not riding. It's a pain, but I sleep better. Not saying everyone should do that, it's probably overkill!
```

---
## \#16 Posted by: psychotiller Posted at: 2015-12-23T17:14:11.279Z Reads: 602

```
What can happen when using the little slider or soft ESC supplied switches is that in the soft switch is the cutt off can fail. This will turn on your board, drain your cells below their LVC and possibly cause a fire. On the sider switches like with Castle ESC's they can wear and eventually the current will bridge in that small area.

Neither are really an issue if you're in close proximity. But lets say, you're back from a long day, you don't have time to recharge your battery after you hit your LVC. You put your gear away and go to sleep. While your sleeping the slider switch fails, drains your battery further and...
```

---
## \#17 Posted by: stuxtruth Posted at: 2015-12-23T17:26:07.368Z Reads: 592

```
So it's safe to say that the best bet is a disarming switch aka loop key?
```

---
## \#18 Posted by: scoobiext Posted at: 2015-12-24T01:18:39.640Z Reads: 633

```
I understand your concerns with soft switches and believe you should go with whatever you feel comfortable with.  For me I like solid state switches because of the the size, soft switching (no spark) and the ability to use a small form factor switch mechanism.  

I think blaming soft switches for LiPo fires is a little far fetched, a LiPo fire would most likely occur in the event of a short circuit within or across the battery pack.  With the soft switch design developed by Vedder and Fetcher (the schematic can be found here: https://github.com/vedderb/SparkSwitch/blob/master/Plot/Schematic.png ) it is very improbable a short would develop in the switch across the battery pack.  If this somehow did occur (most likely water ingress or something similar) the switch has a fuse which would protect the pack.

I am not so concerned with FETS failing as this would be rare and the worst that would happen is the load may become powered on (as psychotiller mentions) in the event of a source to drain short in which case you may drain your batteries depending on the type of ESC connected to the switch.  I have my battery pack connected to a BMS to protect against this and other conditions that are bad for the battery pack.

If you really dont like solid state switches the loop key is a good option as it is cheap, and compact.  Having said that it would pay to look at the likes of Boosted, Marbel, Evolve, Enertion etc. and look at what they are using.
```

---
## \#19 Posted by: Jasiekxl Posted at: 2016-11-02T20:58:38.732Z Reads: 451

```
Here is what you need to buy cheap high voltage switcher:
-car relay 80A (7 euro)
-step down converter (6 euro)
-waterproof blue led bipolar switch (7 euro) 

It cost me in Poland 20 euros. <img src="/uploads/db1493/original/3X/2/f/2fac4ec390d121fa2526c1191c66285cb086f18c.JPG" width="690" height="330">
```

---
## \#20 Posted by: CaptainMerricka Posted at: 2016-11-11T09:05:12.454Z Reads: 420

```
I dont know why I don't see more  auto relays as switches. Anyone have  a good reason why they wouldn't work well for esk8?
```

---
## \#21 Posted by: Maxid Posted at: 2016-11-11T09:48:24.590Z Reads: 394

```
Because relais cause a spark inside at high voltages - so they will wear fast and will not work after a number of "switchings". There is a reason they are used at only 12V.
```

---
## \#22 Posted by: lowGuido Posted at: 2016-11-11T20:44:35.406Z Reads: 384

```
relays will burn out very quickly if used for eskate. the current and voltage ratings on auto relay are no where near high enough.
```

---
## \#23 Posted by: johnny_261 Posted at: 2016-11-12T09:19:40.830Z Reads: 371

```
Can you post some links???  I'm also trying to figure out how this is wired. If you are stepping down the voltage how are you getting enough volts through to the ESC?
```

---
## \#24 Posted by: Jasiekxl Posted at: 2016-11-14T00:17:58.490Z Reads: 358

```
There will be no problem at all. Of course is not a pernament solution and you will need change after  1000 switch or more but is still best choice. You can use a 24v relay if you are afraid.
```

---
## \#25 Posted by: xBRAZILx Posted at: 2018-01-27T11:09:30.245Z Reads: 194

```
@lowGuido
sorry for digging this, but it has been almost two years since you post it about this circuit breaker car system.
my questions are:
1)are you using this method yet? if no, what are you using instead?

2)have you had any problem so far in these two years? if yes, how many times did you have problem as far you remember?

thanks for your time
```

---
## \#26 Posted by: LukePL Posted at: 2018-01-27T11:20:09.015Z Reads: 202

```
So I have a question here also. One of ebike shops here is offering this ![bezpiecznik-63a-nadpradowy-softstart|500x500](upload://iVdWL8pNOJUTI7FkztQLnM3aOA6.jpg)
it's 63 amps fuse with switch and they are saying that they add some resistor to have a "softstart" together with this switch.
What do you think?
```

---
## \#27 Posted by: lowGuido Posted at: 2018-01-27T11:57:42.570Z Reads: 198

```
my daily rider, (the one in the pictures above) that I have been skating for 4 years now uses the circuit breaker.
still going stong.
I used a simmilar system on another board but somone crashed it into a kerb and it physically broke. (but still worked oddly enough) 
https://www.youtube.com/watch?v=tjJ9_wc4ugI


I replaced it with a loop key because its cheaper and easier.
all my later builds just use a loop key.
```

---
## \#28 Posted by: barajabali Posted at: 2018-01-27T15:22:23.389Z Reads: 183

```
Solid stuff. The biggest downside for me was the size
```

---
## \#29 Posted by: lowGuido Posted at: 2018-01-27T15:27:14.552Z Reads: 185

```
yeah, its big and ugly.  but its pretty much idiot proof. the main reason I used them was so that I could wire it to turn on the board, isolate the lipos and turn on the lipo guard alarm all in one go. simple switch that anyone without an electronic engineering degree can operate.
```

---
## \#30 Posted by: oripaamoni Posted at: 2018-01-28T00:56:33.296Z Reads: 182

```
I was going to use a relay out of a li-ion golf cart, their system is 34s not sure on the amperage but it has huge gauge wire going to it. ![IMG_4360|375x500](upload://5iv2UOdmBESOojTNvPVKbewYnrD.JPG)
```

---
## \#31 Posted by: Toohat Posted at: 2018-07-13T18:16:47.313Z Reads: 112

```
Will this work? https://www.amazon.ca/Qiorange-Battery-Disconnect-Isolator-Caravan/dp/B07DKY2WW3/ref=cm_cr_arp_d_product_top?ie=UTF8
```

---
## \#32 Posted by: Matthias Posted at: 2018-11-12T18:48:45.614Z Reads: 76

```
Looks like it's sized right. I don't know much about that type of switch, though.
```

---
## \#33 Posted by: Mich21050 Posted at: 2018-11-12T18:50:50.711Z Reads: 76

```
You know that the thread it 4 months old lol :slight_smile:
@Matthias
```

---
## \#34 Posted by: Matthias Posted at: 2018-11-12T20:23:41.841Z Reads: 73

```
Yeah... I was googling automotive relays for esk8 and this was the first thread I saw. I want to use an [automotive relay](https://www.te.com/usa-en/product-2-1904058-7.html?q=v23700&source=header#pdp-docs-features) for mine. It's a bit undersized, but I doubt I'll draw 20A continuous.
```

---
## \#35 Posted by: Mich21050 Posted at: 2018-11-12T20:25:13.476Z Reads: 76

```
I won't recommend that. A relay is pretty sensetive so after a few weeks of use the vibrations may cause the relay to fail. ( sparks between the relay sides...) :smile:
```

---
## \#36 Posted by: Mich21050 Posted at: 2018-11-12T20:29:23.880Z Reads: 75

```
![Inkedrelay-parts-hd_LI|690x388](upload://6ckI4K8m8K5Y0jqZFIohFORE6IR.jpeg) 
Right here :wink:
```

---
## \#37 Posted by: Holyman92 Posted at: 2018-11-12T20:33:52.824Z Reads: 72

```
@hyperIon1 has a switch solution
```

---
## \#38 Posted by: Matthias Posted at: 2018-11-12T20:34:13.803Z Reads: 70

```
Huh, makes a lot of sense when you see it. Thanks for the info! Are [contactors](https://www.te.com/usa-en/product-2203194-1.html) subject to the same vibrational issues?
```

---
## \#39 Posted by: Mich21050 Posted at: 2018-11-12T20:38:20.676Z Reads: 69

```
I'm not 100% sure but I wouldn't risk it. Whata about a loopkey? :smile:
```

---
## \#40 Posted by: Matthias Posted at: 2018-11-12T20:42:04.626Z Reads: 71

```
I have a loopkey installed already, but I prefer it as a backup solution. I had the @torqueboards powerswitch, but they can't seem to process my RMA after 6 months, so I think its time to find an actual solution.
```

---
## \#41 Posted by: Mich21050 Posted at: 2018-11-12T20:42:55.931Z Reads: 67

```
How much current are you going to draw?
```

---
## \#42 Posted by: Matthias Posted at: 2018-11-12T20:45:57.875Z Reads: 68

```
I think I'll set my peak to 40A. I imagine that I'll see a much lower continuous draw.
```

---
## \#43 Posted by: Matthias Posted at: 2018-11-12T20:46:57.731Z Reads: 74

```
I'm trying not to buy anything beyond what I already have right now. I've got that relay in my parts box now, so I thought I might give that a shot.
```

---
## \#44 Posted by: Mich21050 Posted at: 2018-11-12T20:47:10.864Z Reads: 76

```
Then why not an antispark switch like the one from @Martinsp or @goldenHusky? They should be able to handle it :smile:
```

---
## \#45 Posted by: Battosaii Posted at: 2018-11-12T21:46:03.920Z Reads: 72

```
I ordered a 200a mini sparky from @Kug3lis should handle alot of power.
```

---
