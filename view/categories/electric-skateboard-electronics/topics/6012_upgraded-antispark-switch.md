# Upgraded AntiSpark Switch

### Replies: 69 Views: 7097

## \#1 Posted by: emepror Posted at: 2016-07-13T02:39:54.888Z Reads: 756

```
Hi All,

Been working on my second electric longboard and wanted to upgrade the anti spark switch a bit. This is mostly the same to vedder's antispark, with the changes being an additional FET, an additional resistor as per fechter's 3b revision to the schematic (below) and an upgraded fuse, using the same fuse as used on JTAG's BMS, available in many different ratings. The last two changes are larger trace sizes to better handle current and an option to supply 12V/5V power for an LED switch.

<img src="/uploads/db1493/original/2X/7/7170d5557005bf9019cb5709c4b6a430a31c4e62.png" width="500" height="400">
fechter schematic 
<img src="/uploads/db1493/original/2X/c/c451bc45e0047acc5f779295a3bceeaa86e32404.PNG" width="500" height="350">
My schematic
<img src="/uploads/db1493/original/2X/b/bbaa23d71e21430a6d3d866c2b771a6e05cfac02.PNG" width="500" height="400">
Front of PCB
<img src="/uploads/db1493/original/2X/4/4b8c06924c5c397f1277e1c85d5fe307fd3dc3e5.PNG" width="500" height="400">
Rear of PCB

Board dimensions are 42mm H x 63.25mm W and will be made using 2oz copper. The plan is to look over the design once more in the next day or so and order hardware right afterwards.

Feedback is welcome! If anyone sees anything wrong please let me know. I've also got a power distribution board in the works for supplying 12V and 5V loads as I have plans for lots of LED's, as well as my own BMS, more info on all of that later.

Finally, a link to my github repo as well as a mention that all credit goes to vedder and fechter for the original hardware and schematic designs. https://github.com/msglazer/Anti-Spark_Switch
```

---
## \#2 Posted by: mason Posted at: 2016-07-13T02:49:35.520Z Reads: 622

```
awesome stuff! you should sell these :)
```

---
## \#3 Posted by: emepror Posted at: 2016-07-13T02:59:17.229Z Reads: 614

```
I''d like to, I'll definitely update with a BOM and costs in the next day or so. I want to test it first before I start selling it.
```

---
## \#4 Posted by: DougM Posted at: 2016-07-13T04:09:12.305Z Reads: 623

```
when I did my board I used Through-hole for both the input wires and the output wires.  Seems to me that it has both mechanical and electrical advantages over soldering 10AWG wires to a pad on top of the board.

<img src="/uploads/db1493/original/2X/5/55071cb1ef93dbaa23ab3a0ceac155d9438d0720.png" width="472" height="500">

Otherwise your design looks good.

DougM
```

---
## \#5 Posted by: emepror Posted at: 2016-07-15T22:07:30.402Z Reads: 521

```
I finished the BOM, pushed it to the github repo. It's about ~$30 in components including PCB, cheaper as the buy quantity goes up. I'll update again when I get hardware in hand.
```

---
## \#6 Posted by: emepror Posted at: 2016-08-17T02:15:37.576Z Reads: 511

```
Been a while, got the boards in and assembled one. Guess I got a bad FET or something as it only dropped the voltage ~3-4 volts when on. I've ordered some more parts (thought I could get away with just one set of components, you can see how that turned out). If anyone sees anything wrong with the schematic let me know, its a direct copy but who knows.
```

---
## \#7 Posted by: emepror Posted at: 2016-09-16T20:49:47.751Z Reads: 502

```

<img src="/uploads/db1493/original/3X/7/6/768d39453355a01de0a10b1a37103b09e3974ad0.jpg" width="375" height="500">
Only slightly broke this one hah. While this one may have had a dead 12V zener, turns out I needed to have a load connected, everything worked great once I assembled a 2nd.

<img src="/uploads/db1493/original/3X/d/4/d4b3649f81ea23055b7a1c70ee175a88b20c6974.jpg" width="375" height="500">
assembled board!

<img src="/uploads/db1493/original/3X/c/b/cb68bdc84e7164b71e329517356edfdd0ac97d7e.jpg" width="690" height="460">
assembled with connector and switch.

I know some were interested in buying some (they'll be approx $40-45ea), ill be making a sales thread, feel free to PM me if interested. Feel free to shoot me any questions.
```

---
## \#8 Posted by: chaka Posted at: 2016-09-17T04:12:09.226Z Reads: 461

```
Looks good but you will want to route the via from R1 to the "out +" pad to be sure you break the circuit if the fuse blows.
```

---
## \#9 Posted by: emepror Posted at: 2016-09-17T04:24:38.749Z Reads: 460

```
I've made that change for rev 1.1, good point though!
```

---
## \#10 Posted by: akira Posted at: 2016-09-20T12:25:28.069Z Reads: 418

```
Hi emepror
Nice design !
Do you plan to publish your gerber files for v1.1 with the R1 modification ?
I would like to try your design but I would prefer to wait for this v1.1 fix.
```

---
## \#11 Posted by: emepror Posted at: 2016-09-20T20:30:15.776Z Reads: 399

```
Just updated the github repo.
```

---
## \#12 Posted by: Eboostin Posted at: 2016-09-21T00:12:57.873Z Reads: 388

```
@chaka Are the ones on your site complete or just the board? There isn't any info on the product page.
```

---
## \#13 Posted by: chaka Posted at: 2016-09-21T02:34:02.192Z Reads: 384

```
They are complete with a switch. You need to add your connectors of choice.
```

---
## \#14 Posted by: akira Posted at: 2016-09-21T07:24:57.597Z Reads: 376

```
Thanks !!
But I could not find the new version. 
I can only see the master branch with the last commit in August : 
 https://github.com/msglazer/Anti-Spark_Switch/commits/master

Do you have this commit public ?
```

---
## \#15 Posted by: sl33py Posted at: 2016-09-22T20:35:25.348Z Reads: 365

```
Same here.  I see v1.0 w/ 2 month old updates.

Would love to try this v1.1 when available!
```

---
## \#16 Posted by: emepror Posted at: 2016-09-23T01:12:17.773Z Reads: 373

```
Everything looks up to date on my end, any luck now? I did make a couple changes today, i.e. switched smd pads to "handsolderable" versions, increased size of the connector solder pads, and a text change on the schematic.

https://github.com/msglazer/Anti-Spark_Switch
```

---
## \#17 Posted by: zmoney Posted at: 2016-09-23T01:13:03.717Z Reads: 354

```
Will definitely give this a go on my personal build. Kudos!
```

---
## \#18 Posted by: emepror Posted at: 2016-09-23T01:58:41.290Z Reads: 360

```
Hi all, the BOM was out of date and i've just fixed the issue. Hopefully no one ordered parts off the BOM before pretty much now (everything would be fine value wise).

Also, would a 60A fuse be more reasonable, or what value would people prefer on their builds.
```

---
## \#19 Posted by: Pantologist Posted at: 2016-09-23T02:03:24.752Z Reads: 349

```
I'm using 60A fuses for my pack, but it all depends on your battery specs. You are using LittleFuses right?

They have a decent selection of fuses. I'd say the most common ones are 40A(2P) 60A(3P) and 80A(4P) considering 18650 builds.
```

---
## \#20 Posted by: emepror Posted at: 2016-09-23T02:05:32.059Z Reads: 345

```
Yeah i've got a LittleFuse on my build. I'm placing an order for a small run and I want to try and cover the most options, probably going to get a 60A fuse.
```

---
## \#21 Posted by: Pantologist Posted at: 2016-09-23T02:09:26.299Z Reads: 308

```
Are the solder pads on your modified BOM smaller than Vedder's original design? I think it might be nicer if it was a tad larger for the people using 10-8 AWG wire.
```

---
## \#22 Posted by: emepror Posted at: 2016-09-23T02:12:15.285Z Reads: 302

```
No, they're actually larger, 8x7mm vs 6x5mm. This is one rev 1.1, I too noticed the size is a tad small.
```

---
## \#23 Posted by: sl33py Posted at: 2016-09-23T04:33:03.709Z Reads: 309

```
Super cool you are sharing this.  What are the square pinhole sections on the bottom/negative under FETs for?

So this is really a Vedder/Fechter/Emepror Anti-spark right?  Talk about it takes a village...

:)
```

---
## \#24 Posted by: akira Posted at: 2016-09-23T07:55:38.654Z Reads: 298

```
It's updated now.
Thank you very much for sharing this !!
```

---
## \#25 Posted by: Pantologist Posted at: 2016-09-23T12:59:26.885Z Reads: 292

```
What are those standoffs for the fuse called? Any idea what their amp limit is?
```

---
## \#26 Posted by: DeathCookies Posted at: 2016-09-23T13:07:49.130Z Reads: 307

```
[quote="Pantologist, post:25, topic:6012"]
Any idea what their amp limit is?
[/quote]

Common people.... please dont be so lazy....

I took my 20 seconds to get this answer.
--> Github
--> Bom
--> Fuse
--> Go to the mouser link
--> 58V / 70A (70 because the number on the fuse says it)

Your approach by asking cost you much more than 20 seconds.

But no problem, i am not mad ;) Just try to motivate the lazy folk :D
```

---
## \#27 Posted by: Pantologist Posted at: 2016-09-23T13:42:27.441Z Reads: 295

```
I'm not talking about the fuse lol....

I'm taking about the standoffs that it screws into...
```

---
## \#28 Posted by: chaka Posted at: 2016-09-23T13:45:40.386Z Reads: 303

```
I noticed a few problems with your layout, you may need to rework your schematic.  Nothing is routed to your 12v pin and you have SW shorted to positive. Looks like R3 is also grounded with a via.

I had started work on a similar switch a few months ago, I should dust off the file and finish it up. Was going for something a little more compact in width and thickness. Still need to incorporate some fuse terminals and through holes for a jst-ph connector. Needs some vias to finish stitching some of the main power traces too.

<img src="/uploads/db1493/original/3X/7/d/7d6112a3247d1ccb58344ed82c759328e0345a59.png" width="690" height="291">
```

---
## \#29 Posted by: DeathCookies Posted at: 2016-09-23T13:49:07.456Z Reads: 289

```
My fault... i am sorry :unamused:
```

---
## \#30 Posted by: Pantologist Posted at: 2016-09-23T15:34:59.390Z Reads: 282

```
Will you be using a similar style fuse and fuse holder design?
```

---
## \#31 Posted by: SORRENTINO Posted at: 2016-09-23T16:30:51.825Z Reads: 281

```
THEY ARE120 AMP STANDOFFS. http://www.mouser.com/ProductDetail/Wurth-Electronics/7460408/?qs=lykWx4dhCCG7IAhyxQ5B4w%3D%3D
```

---
## \#32 Posted by: akira Posted at: 2016-09-23T17:07:54.750Z Reads: 280

```
Nice one.

Thanks for having looked at the new v1.1 version. 
I could cancel my OSHPark order just in time ;-)
```

---
## \#33 Posted by: chaka Posted at: 2016-09-23T20:07:54.336Z Reads: 273

```
Yeah, I  really like the little fuse brand.
```

---
## \#34 Posted by: emepror Posted at: 2016-09-23T20:13:37.386Z Reads: 273

```
So changing the footprints to "handsolderable" the footprint references got all messed up, they're fixed now. Does that clear up the things you saw, because looking at the schematic, those issues you mentioned weren't apparent. Also I did make one other change, the through holes for posts for the fuse were ever so slightly too small and while it still works you pretty much need to use a hammer to get them in. This has been fixed (I hope) by making the posts  0.1mm larger. I wish I knew where my calipers are.


For anyone else reading, if you've ordered PCB's for this design and still can change the gerber files go ahead, if not everything will still work, the posts are just a pain in the butt to get in.
```

---
## \#35 Posted by: s28400 Posted at: 2016-09-28T03:12:45.816Z Reads: 260

```
Very good stuff guys! @chaka are you planning on selling/using these at Ollin?
```

---
## \#36 Posted by: B4Me Posted at: 2016-09-28T07:57:51.765Z Reads: 261

```
Just a small comment, I dont know if it allready was said...
BUT... it is normaly bad practice to place the switch so if it fails everything is ON

Normally you would make it pull-down to off by default, and then the switch pulls in up, and turns it ON :slight_smile:
```

---
## \#37 Posted by: Bender Posted at: 2016-09-28T12:06:38.874Z Reads: 254

```
Maybe not in this application, I'm not sure what's worse while your riding, stopping suddenly or not being able to stop?!? :astonished:
```

---
## \#38 Posted by: B4Me Posted at: 2016-09-28T12:41:24.157Z Reads: 256

```
You got a point ! 
better to have a on fet than off for ud :) sorry
```

---
## \#39 Posted by: Bender Posted at: 2016-09-28T13:51:41.788Z Reads: 244

```
No really, not sure which is worse
```

---
## \#40 Posted by: emepror Posted at: 2016-10-01T02:45:05.758Z Reads: 254

```
I'd personally rather have the switch fail to on, having a switch fail to off going 20+ mph is not something I want to experience. However your point of either option being bad, I agree with, faulting on isnt a great solution. Eventually im moving to having the cutoff built into a BMS with a bit more control/notification in the case of a failure. Also if the fuse goes, everything is powered down, at least w/ rev 1.1.
```

---
## \#41 Posted by: SORRENTINO Posted at: 2016-10-14T17:27:51.095Z Reads: 230

```
Did you guys get a 1oz or 2oz for this pcb. OSH Park normal is 1oz but have option for 2oz. Is 2oz Needed? Thanks
```

---
## \#42 Posted by: chaka Posted at: 2016-10-15T02:20:31.646Z Reads: 236

```
If you order my revision you will be fine with 1oz but you will want 2oz for the original design.
```

---
## \#43 Posted by: SORRENTINO Posted at: 2016-10-15T02:41:34.573Z Reads: 242

```
ah ok Thanks Chaka
```

---
## \#44 Posted by: Eboostin Posted at: 2016-10-15T02:52:57.176Z Reads: 251

```
Is the revision you mentioned the one currently for sale on your site or a new one?
```

---
## \#45 Posted by: chaka Posted at: 2016-10-15T02:55:41.508Z Reads: 251

```
The one on my site is that same as the one I am sharing on OshPark. I wire them without a fuse since most people want more than 50 amps. You can solder a fuse in place if you like but it is probably best use a higher rating than 50 amps and use something inline. I recommend something around 100 amps but this can vary depending on your system gearing ect...
```

---
## \#46 Posted by: Eboostin Posted at: 2016-10-15T05:10:57.438Z Reads: 241

```
I have a 10S4P 30Q pack. I am planning to use a 80A fuse on the positive battery pack lead since the pack is good for 80A continuous. Would another fuse on the antispark be redundant?

This is the fuse I was looking at https://www.amazon.com/gp/aw/d/B004ZJ0S2M/ref=ox_sc_saved_image_2?ie=UTF8&psc=1&smid=ATVPDKIKX0DER
```

---
## \#47 Posted by: emepror Posted at: 2016-10-15T20:51:23.710Z Reads: 241

```
if you would be putting a fuse on the pack and then the switch, you'd have a redundant fuse.

Replying to the copper question a couple posts back, with my board i prefer 2oz copper. I've used a company called smart prototyping for boards (cheaper than oshpark) and they'll do 2 oz. 1 oz should be fine but i'd like to be able to either handle as much current as possible or lower the operating temperature of the board.
```

---
## \#48 Posted by: DeathCookies Posted at: 2016-11-07T07:53:01.241Z Reads: 260

```
Is GitHub uptodate? Is the Github version failsafe or are there any problems left?

"One other change is an optional 12V supply tap that can be used for an LED button if desired, the 12V (5V) must be supplied externally."
When reading this i get the feeling that you have to supply the PCB with your battery and when i want to use the LED of the switch i need to attach additionaly 12V? That does not make sense for me but it is what i expect with the given sentence....

Why does it only have 3 holes instead of 5? (right side for the switch)? Does this make trouble when ordering from a pcb factory?

https://cloud.githubusercontent.com/assets/12124823/18770961/bea18c10-8108-11e6-946d-03154ce8d010.PNG

Would be nice if you could enlighten me ;)
```

---
## \#49 Posted by: JdogAwesome Posted at: 2016-11-08T23:55:34.589Z Reads: 235

```
Hey DeathCookies instead of using a separate 12V source you could just use a couple high value resistors to act as if it was 12V. My MOSFET switch design has this integrated on the PCB but you can easily add this to Vedders design.
```

---
## \#50 Posted by: emepror Posted at: 2016-11-09T01:08:57.170Z Reads: 227

```
Hey, ill do a double check over the files in a few, and update the repo if need be. the reason you need a seperate 5 or 12V source for the button LED is that I didnt want to overload the zener diode and there's no other DC-DC regulation on the board, I could have used a voltage divider but that wastes a lot of energy to heat. The image with only three holes on the five pads is just a graphics glitch, I have had no problems with the batch im getting ready to sell.
```

---
## \#51 Posted by: emepror Posted at: 2016-11-09T01:09:43.148Z Reads: 226

```
The only problem is that it wastes a lot of energy to heat when you use just a voltage divider, especially when your dealing with 40+V down to 5V or 12V
```

---
## \#52 Posted by: JdogAwesome Posted at: 2016-11-09T03:13:27.223Z Reads: 221

```
I wasn't talking about using a voltage divider, just using a high value resistor to limit the current though the LED. And it definetly doesn't waist that much power to heat lol, your only powering an LED. It's what I do in my switch and it works fine.
```

---
## \#53 Posted by: emepror Posted at: 2016-11-09T03:34:39.346Z Reads: 220

```
if you have an LED with a forward voltage of say 2V @ 20mA and a fully charged 42V battery your wasting (42V-2V) * 20mA = 0.8W of power, which isnt a huge amount compared to motor draw, but when you design your electronics to idle in the lower milliwatts or lower, its a large amount.
```

---
## \#54 Posted by: JdogAwesome Posted at: 2016-11-09T03:47:49.519Z Reads: 216

```
True but the LED is only on when the board is on and constantly drawing around 15A so personally I don't think it really matters. Also theres no reason to run 20mA through it you could just run 10 or less for pretty much the exact same brightness.
```

---
## \#55 Posted by: jmasta Posted at: 2016-11-09T04:12:06.604Z Reads: 214

```
Most probably won't like this option, but I just use a 12V UBEC.  Overkill for just a lighted switch, but it also allows me to power my headlights, USB charge port, and Arduino (if desired)
```

---
## \#57 Posted by: chinzw Posted at: 2016-11-09T16:52:40.018Z Reads: 206

```
Yep, a 12 switching regulator would do the job, for less money. Something like SI-8010GL.
```

---
## \#58 Posted by: JdogAwesome Posted at: 2016-11-09T20:55:32.608Z Reads: 209

```
Yes thats true but like I said you don't need to run 20mA through it. If you just ran 12 then you would only be using 1.2W which is still very minimal and I think completely irrelevant.
```

---
## \#59 Posted by: DeathCookies Posted at: 2016-11-10T09:20:05.150Z Reads: 212

```
@emepror
Is Github uptodate? Is everything working? How much can this switch handle? Are you going to change the LED 12V supply?

Thanks in advance ;)
```

---
## \#60 Posted by: emepror Posted at: 2016-11-15T15:05:23.178Z Reads: 197

```
Hey, sorry for the delay, I lost my laptop and didn't have the ability to work on my designs during that time. I have a 70A Fuse on mine, and the board should handle peaks up to that no problem. I have no plans to change how the LED supply works, as I can pull 5V off the VESC and pass it to the switch in my eboard, a similar approach can be done on other eboards.
```

---
## \#61 Posted by: DeathCookies Posted at: 2016-11-15T15:12:55.571Z Reads: 201

```
Real question:
Why did you add the additional two pins for the LED power supply?
```

---
## \#62 Posted by: emepror Posted at: 2016-11-15T16:22:34.496Z Reads: 211

```
Because the goal for this Switch was to make it cheap'ish and simple, theres no need to add a regulator onto the board when you can run 2 wires from a local source you have already. Plus this is a stop gap for me as I move onto a smartBMS eventually. 

On a different note the CAD files are good to go
```

---
## \#63 Posted by: DeathCookies Posted at: 2017-01-14T19:34:30.616Z Reads: 194

```
Do you know how much amp this switch can handle?
The fuse standoffs are rated to 120A. What about the mosfets and the other stuff?

Why did you choose to use 3 Mosfets instead of 2? Just about more  reliability?
```

---
## \#64 Posted by: emepror Posted at: 2017-01-22T00:05:10.044Z Reads: 197

```
I've got a 70 amp fuse, which is the max I would go. Went with three MOSFETs for a bit more reliability on the higher current side by lessening heating on the FETs, etc.
```

---
## \#65 Posted by: emepror Posted at: 2017-02-02T00:50:59.287Z Reads: 190

```
If anyone has used this design , **DO NOT** hook up the LED power connector to anything, unfortunately the ground for it is separated in such a way that it will short if the board is in an "off" state. I'll spin a fix to this ASAP and apologize if anyone made these for their personal boards.
```

---
## \#66 Posted by: The_Dude Posted at: 2018-06-25T11:24:11.539Z Reads: 111

```
Hi @emepror,
did you already fix this issue in the current version on github? If I want to go for higher ampere like 150A, do I simply have to use more mosfets in parallel (like 5)?

Thanks!
```

---
## \#67 Posted by: koralle Posted at: 2018-06-25T12:27:53.610Z Reads: 102

```
you need to make sure to increase thickness or width or both of your copper on the pcb accordingly.

Some people just double up using solder or through hole solid copper wire
```

---
## \#68 Posted by: emepror Posted at: 2018-07-01T15:09:21.466Z Reads: 92

```
first up:

There's a newer revision of my switch now, ill update the top post soon. Less likely to fry things now!

but @The_Dude, koralle is right. You can increase the amount of FET's to 4-5 for that much current but your going to run into issues with copper thickness and current handling. one way around that is to leave the copper traces exposed and add solder but still going to be a lot of current. One other thing that I would start looking into at more than 3+ FET's is a simple mosfet driver so its a bit more durable.
```

---
## \#69 Posted by: D_Sk8 Posted at: 2019-02-01T20:47:10.268Z Reads: 65

```
Hey Matt,

The github mentions "provides a convenient on off ability."

I've seen some anti-spark switches on the market that turn on automatically during a kick start, and auto/off. Can you confirm what you mean by convenient on/off?
```

---
## \#70 Posted by: ARetardedPillow Posted at: 2019-03-19T23:58:55.012Z Reads: 43

```
Hey @emepror, where can I get my hands on one of these?
```

---
