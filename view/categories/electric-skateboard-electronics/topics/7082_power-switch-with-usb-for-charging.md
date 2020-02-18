# Power Switch with USB for charging

### Replies: 61 Views: 4995

## \#1 Posted by: mikey Posted at: 2016-08-03T19:42:44.009Z Reads: 403

```
Does anyone know where I can find a power switch for a 12s1p battery pack with a female USB port for charging stuff?
I've seen this on battery packs. Is the USB a feature on the BMS or is it something I can add in line with a power switch?
```

---
## \#2 Posted by: JLabs Posted at: 2016-08-03T19:58:40.999Z Reads: 390

```
Hmm. I havnt seen anyone do this recently on the forum. I could suppose you could use a UBEC.. I may have a fuzzy feeling @longhairedboy knows himself of knows someone who knows.
```

---
## \#3 Posted by: Nordle Posted at: 2016-08-03T19:58:58.049Z Reads: 388

```
i oredered those 2 parts for my next 10S battery
[PART1](http://www.aliexpress.com/item/freeshipping-DC-DC-Step-Down-Module-6-24V12V24V-to-5V3A-Car-USB-Phone-Charger-Power-Supply/32324225083.html?spm=2114.13010208.99999999.282.U9QBas) & [PART2](http://www.aliexpress.com/item/DC-DC-Converter-Adjustable-Power-Supply-DC-DC-Step-Down-3A-LM2596HVS-LM2596HV-DC-Step-Down/32485142548.html?spm=2114.13010208.99999999.288.U9QBas) from aliexpress
hope it works but i'm confident
```

---
## \#4 Posted by: Hillso Posted at: 2016-08-03T20:06:55.554Z Reads: 377

```
I see only 6s chargers: http://www.aliexpress.com/wholesale?catId=0&initiative_id=AS_20160803220405&SearchText=lipo+phone+charger
```

---
## \#5 Posted by: Nordle Posted at: 2016-08-03T20:11:54.689Z Reads: 363

```
therefore is my 2nd part, a step down module
```

---
## \#6 Posted by: sl33py Posted at: 2016-08-03T20:13:28.354Z Reads: 366

```
That looks really promising.  Use part 2 to step down voltage, and the USB charges up to 2.1 amps (long term vs 3a rating)?

Alternatively a cheap HK ubec would work, but still be more $.

let us know how it goes!  I might do similar and get a spare or two w/ an easy to swap connector...  at these prices it's easy enough to have one in the box for just in case!
```

---
## \#7 Posted by: mikey Posted at: 2016-08-03T20:21:22.311Z Reads: 354

```
This looks interesting! Please update us on your progress.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-08-03T20:25:11.915Z Reads: 349

```
Just got it but haven't installed it yet 

https://www.ebay.com/itm/272076571075 


Connect this to anything that needs 12v
```

---
## \#9 Posted by: Pablo_702 Posted at: 2016-08-03T20:58:57.406Z Reads: 333

```
Will the 3A output be enough to power like 2 meter of the high density rgb 5050 led strips at its max brightness?
```

---
## \#10 Posted by: Nordle Posted at: 2016-08-03T22:02:56.652Z Reads: 323

```
I'll report back how it works, however that could take a good amount of time, cause parts arrive from china slowly 1-2months, and it's just for my 2nd board. So i'm not in hurry to finish this :slight_smile:

Don't know about your leds, maybe link them and tell us how many leds one meter has^^ for sure it is enough to charge my remote or phone and thats all i want.
```

---
## \#11 Posted by: saul Posted at: 2016-08-03T22:11:11.692Z Reads: 307

```
I got a 5a buck module that's sealed in plastic package with mounting holes. Should work fine. You can add another small bag or voltage regulator like the super mini 3a version you can for about $1 and use this to get down to 5v. Solder a usb port or 2and your set.

Those rgb strips use about 1a/meter, but that will be crazy bright on the bottom of a board. I'm going to use about 50cm on my board and that seem like plenty.
The rest of the power goes to a pair of 3w leds with lens.
```

---
## \#12 Posted by: mikey Posted at: 2016-08-04T00:08:27.118Z Reads: 294

```
What voltage regulator do I need for this? I'm running a 12s1p
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-08-04T00:22:26.974Z Reads: 306

```
[quote="Pablo_702, post:9, topic:7082, full:true"]
Will the 3A output be enough to power like 2 meter of the high density rgb 5050 led strips at its max brightness?
[/quote]

Humm 🤔

Maybe 

<img src="/uploads/db1493/original/2X/0/01b0e2a91fef4bb7d09d642dd20400fa07292c86.jpeg" width="509" height="500">
👆🏻some of my builds
```

---
## \#14 Posted by: sl33py Posted at: 2016-08-04T00:40:33.597Z Reads: 285

```
i actually used my lab power supply to test the full roll (15') of 5050 single color LEDs and it was around 1.8A max.  So you should be fine with only 6ft/2m!

I can grab my 5050 rgb's and test as well, but i'm positive you are fine w/ 3a.
```

---
## \#15 Posted by: oriol360 Posted at: 2016-08-04T01:16:04.157Z Reads: 276

```
http://miamielectricboards.com/shop-1/dual-output-ubec

I got a dual output UBEC that is great for hooking up LEDs and/or USB chargers! Outputs at 5-6v at up to 12amps
```

---
## \#16 Posted by: sl33py Posted at: 2016-08-04T01:21:45.086Z Reads: 274

```
Nice!  One thing to note, most of the 5050 LED's are 12v not 5-6v so just make sure you get the right ones for a UBEC to power like @Oriol360 linked.  You can find the lower voltage LEDs which take ~6v, but confirm or go 12v to power them.
```

---
## \#17 Posted by: KMeyerson Posted at: 2016-08-04T03:55:31.197Z Reads: 265

```
Safety alert - not all buck converters use authentic components.  This is more of an issue at higher voltages, but beware that some may overheat and or catch fire. If your LEDs flicker of fade weirdly. The buck converter is failing to provide a smooth current.  You should disengage it asap.

Look for YouTube reviews for an up to date list of authentic buck converters.
```

---
## \#18 Posted by: Pablo_702 Posted at: 2016-08-04T04:07:28.562Z Reads: 254

```
Do ubhave the link for such video?
```

---
## \#19 Posted by: KMeyerson Posted at: 2016-08-04T04:13:19.612Z Reads: 252

```
Watch this video to get started: 
(https://youtu.be/JLwJb4MVbls)

Then watch reviews on Onstates LED Lighting's  channel.

Have fun :-))))
```

---
## \#20 Posted by: Michaelinvegas Posted at: 2016-08-04T04:26:08.311Z Reads: 248

```
And to back up what @KMeyerson shared....

Always test the converter before you hard wire it in....

I had the same experience with a similar converter...These do come from China after all 

So use a voltage meter!
```

---
## \#21 Posted by: mason Posted at: 2016-08-04T08:03:37.980Z Reads: 219

```
bought these also, hope it works good.
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-08-04T12:11:45.132Z Reads: 214

```
I'll bet that would handle a 12v EL inverter pretty well, huh? I'm actually looking for something like this too. I have a TRON build coming up.
```

---
## \#23 Posted by: Nordle Posted at: 2016-08-04T12:16:15.366Z Reads: 215

```
And anyways before use i have to adjust voltage trimming the pot on the converter, how should i do this without a voltmeter? :P
```

---
## \#24 Posted by: mikey Posted at: 2016-08-04T15:18:18.929Z Reads: 216

```
Is there an easy way to get power from the VESC?
```

---
## \#25 Posted by: Nordle Posted at: 2016-08-04T15:21:29.944Z Reads: 208

```
For very small currents _(receiver)_ there are 3.3v and 5v pins.
```

---
## \#26 Posted by: mikey Posted at: 2016-08-04T15:22:56.070Z Reads: 206

```
Doesn't a USB port only need 5v?
```

---
## \#27 Posted by: flatsp0t Posted at: 2016-08-04T15:24:39.545Z Reads: 207

```
Yes, but 1 or 2 Amps is used for phone charging.
Maybe it will work, but generate extra heat on your vesc, which is what you dont want.
```

---
## \#29 Posted by: JdogAwesome Posted at: 2016-08-04T17:01:16.578Z Reads: 208

```
You guys have some great ideas going, but I thought I could just say a couple things to benefit this. First off DONT EVER trust the "3A Max" rating a component and think, well then I can draw 3A fine! Like may be you can draw 3A... if its liquid oxygen cooled, but definitely not with normal air cooling. Now that's not always true but in my experience, it has been. I often use the same buck converter that Nordle was talking about in his PART 2 and I was recently working on a project drawing 1.5A at 12V and it overheated in about 10 seconds. But the thankfully I had 5A converter and I used that instead, though that thing still gets relatively warm drawing 1.5A. All I'm saying is be careful and air on the side of caution. And also you can buy a pack of 5 of those converters on eBay for $5 though I'm sure there not legitimate versions though they do work for smaller projects.
```

---
## \#30 Posted by: Stevemk14ebr Posted at: 2016-08-04T17:04:03.156Z Reads: 204

```
The turnigy dlux hv sbec is awesome. I use it myself, it has two output leads, can supply up to 10amps and is very solid. I run it at 12s and have had zero issues for a few weeks now. It also runs veeeery cool. I recommend very much, i got mine from hobbyking.
```

---
## \#31 Posted by: jrpwit Posted at: 2016-08-04T17:08:23.739Z Reads: 195

```
I got one of [these](http://www.ebay.com/itm/2PCS-DC-Buck-Step-Down-Converter-Module-LM2596-Voltage-Regulator-Voltmeter-Red-/311607688971?hash=item488d43ff0b) and jaun of [deez](http://www.ebay.com/itm/6-24V-12V-24V-to-5V-3A-CAR-USB-Charger-Module-DC-Buck-step-down-Converter-DIY-/221980647793). That step down converter has 2 buttons to display the output and intput voltages. Pretty nice addition if you ask me :smiley:
```

---
## \#32 Posted by: JdogAwesome Posted at: 2016-08-04T17:11:14.719Z Reads: 196

```
Totally depends on how much current the EL converter uses. If it only draws like an amp or two you may be fine with that blue buck converter (don't remember the chip name) though you may also want to use that HRD converter instead.
```

---
## \#33 Posted by: longhairedboy Posted at: 2016-08-04T19:15:17.105Z Reads: 192

```
i looked at the turnigy dlux hv sbec for my purposes but it doesn't do 12V output according to the page on hobby king, and the el inverters i bought are are 12v. 

I just emailed the people i bought them from to ask about amp draw. That's not something i thought about. I figured it would be pretty low, but i'm sure that's a mistake in the making, so i thought i'd check to be sure.
```

---
## \#34 Posted by: longhairedboy Posted at: 2016-08-04T19:17:38.543Z Reads: 193

```
damn they're fast! They emailed me back already. The draw is less than 300mA so i think we're good. I got a couple of the BECs linked in this thread from ebay and one i found on amazon to try out and see which works out best.  In the mean time i have a shitload of drawing and dremelling to do on one particular deck. Don't worry, build thread will come. That board is going to be epic.
```

---
## \#35 Posted by: Michaelinvegas Posted at: 2016-08-04T19:21:35.899Z Reads: 193

```
@longhairedboy if you are using el wire the amp draw is so low....

If you run a separate line from the the battery to a step down, you isolate the lights in their own system...anything goes wrong with the lights ...just turn them off.

I've used dual 10w LEDs for headlights and LEDs hooked up to this 
👇🏻
https://www.ebay.com/itm/172011102603 

No issues...
```

---
## \#36 Posted by: longhairedboy Posted at: 2016-08-04T19:27:19.313Z Reads: 183

```
I could totally use that on my 6S rat board as is. My son has already taken it upon himself to cover the whole thing in LEDs powered by the BECs on the Favourites its currently running. 

my plan for this build is to have a small kill switch on the lights but also have that wired in after the main switch so when the lights are in the on position, they just come on when the board is on and go off when the board is off so that it doesn't drain the pack and trip the BMS protections if accidentally left on for no reason, becuse it can't be accidentally left on.
```

---
## \#37 Posted by: Michaelinvegas Posted at: 2016-08-04T19:32:33.313Z Reads: 182

```
Yeah any voltage higher than 6s need to use a higher rated converter like the one I mentioned earlier in the post.

Trying to get the VESC to provide power to a lighting system is not the best idea...

The safest is just to run a seperste system...again if any issues...just switch it off...it will isolate the LEDs from the power
```

---
## \#38 Posted by: longhairedboy Posted at: 2016-08-04T19:38:42.508Z Reads: 181

```
[quote="Michaelinvegas, post:37, topic:7082"]
Trying to get the VESC to provide power to a lighting system is not the best idea...
[/quote]

i burned out 6 LEDs doing exactly that. It is indeed a terrible idea. You really can't count on that 12v line to do more than power the receiver and the led in one of those angel-eye push buttons, which is something i've done in the past with much success instead of getting an additional BEC to do it.
```

---
## \#39 Posted by: Michaelinvegas Posted at: 2016-08-04T19:40:07.076Z Reads: 174

```
Yeah run separate system mate...it will give you more lighting options
```

---
## \#40 Posted by: Michaelinvegas Posted at: 2016-08-04T19:42:26.556Z Reads: 186

```
@longhairedboy don't you want an option to run something like this off your boards? 

https://www.ebay.com/itm/221994763940 

Just got mine last week
```

---
## \#41 Posted by: longhairedboy Posted at: 2016-08-04T19:54:27.775Z Reads: 181

```
that's what i'm doing. I'm just wiring the bec or step downs it into the mains on the ESC side of the main switch so the whole thing will turn off when the board turns off.
```

---
## \#42 Posted by: longhairedboy Posted at: 2016-08-04T19:55:22.474Z Reads: 169

```
is that an audio amp? I'm sending that link to my son.
```

---
## \#43 Posted by: Michaelinvegas Posted at: 2016-08-04T19:55:44.924Z Reads: 165

```
Yes 50 watts
```

---
## \#44 Posted by: Michaelinvegas Posted at: 2016-08-04T19:56:27.376Z Reads: 172

```
Bluetooth...

Just add power and speakers and connect your phone
```

---
## \#45 Posted by: mikey Posted at: 2016-08-04T20:16:08.684Z Reads: 170

```
OMG you guys are awesome. Now I'm going to have a skateboard that goes 25mph, with EL wire for lighting, while charging my phone and listening to tunes really loud! I should vape while i do this!
```

---
## \#46 Posted by: Michaelinvegas Posted at: 2016-08-04T20:16:55.012Z Reads: 166

```
[quote="mikey, post:45, topic:7082"]
I should vape while i do this!
[/quote]



Lol don't get crazy now
```

---
## \#47 Posted by: Pablo_702 Posted at: 2016-08-04T20:17:13.131Z Reads: 164

```
probably becasue its 5V not 12V
```

---
## \#48 Posted by: Michaelinvegas Posted at: 2016-08-04T20:22:57.175Z Reads: 169

```
@Nordle I don't really trust those adjustable pots .... The vibration may mess it up and accidentally change the voltage out put .... Although never happened to me...it's something that could happen...that why I like the fixed 12v output
```

---
## \#49 Posted by: Nordle Posted at: 2016-08-04T20:24:19.215Z Reads: 166

```
Thx, i'll add some glue ^^
```

---
## \#50 Posted by: longhairedboy Posted at: 2016-08-04T20:41:18.624Z Reads: 164

```
The LEDs I used at the time were 3 to 5v range, the 5mm dome top kind. They were probably crappy, also.
```

---
## \#51 Posted by: JdogAwesome Posted at: 2016-08-05T00:23:07.632Z Reads: 165

```
Yeah like Nordle was saying I  just put a drop of hot glue on the screw so it won't vibrate to a different voltage lol. Oh and also you guys were planning on using 24V USB charging modules, though those then must have there own step down module on board which is less efficient and may make the board more expensive. So you could just get a 5V USB module and adjust the converter down to 5V so its more efficient and cheaper.

EDIT: I've used these modules in the past and they work super well and output right around 1.5-2A i know there's cheaper ones out there but all I know is these ones have worked well for me. http://m.ebay.com/itm/DC-DC-3V-3-3V-3-7V-4-2V-to-5V-USB-1A-2A-Step-Up-Vehicle-Power-Charge-Module-YG-/111866440588?txnId=1528632132001
```

---
## \#52 Posted by: JdogAwesome Posted at: 2016-08-21T16:23:33.201Z Reads: 167

```
Hey Nordle just to let you know, I can't find a datasheet for a "LM2596HVS" and if there isn't a datasheet for the chip, it's probably fake or just a re-labelled LM2596. Also there are some videos about fake HV LM regulators so do be careful. I wish there were 60V versions of the LM2596 but I don't believe there are, though I could be wrong so test it out and please report back with whether or not it works!

EDIT: I still can't find a LM2596HV chip, though I did find a LM2576HV chip which can take up to 60V. Here's the datasheet, and it would be a great chip for a 3A UBEC which I may build in the future. https://www.google.com/url?sa=t&source=web&rct=j&url=http://www.ti.com/lit/ds/symlink/lm2576.pdf&ved=0ahUKEwjdgbH1ttPOAhWRsh4KHSMFDGcQFggkMAA&usg=AFQjCNF7FcxJ3UzAUT6_FkqXNu4P5YedbQ&sig2=qIEe0Ph7qyrDCfFdvAJcaw
```

---
## \#53 Posted by: Nordle Posted at: 2016-08-22T06:50:16.250Z Reads: 153

```
Thx for the tips. When my parts arrive i'll wire them together, connect something for a day or so and if it gets to hot i know it's garbage. Or it's already broken then^^
```

---
## \#54 Posted by: johnny_261 Posted at: 2016-10-31T05:41:43.033Z Reads: 138

```
Hi Guys,

Read through the whole thread here and am trying to make sure I understand it all.  I'm planning on doing a 10S or 12S build next and wanted to have a USB charging port.

As far as I understand these are my options:
1) Buy something like this with input voltage of 5V and use power from a BEC that can go from 12S to 5V

http://www.ebay.ca/itm/Dual-USB-5V-1A-2-1A-Mobile-Power-Bank-18650-Battery-Charger-PCB-For-Phone-DIY-/171404149586

2) Buy something like this, that takes input voltage from 6-24V and use with a 12S to 12V BEC.  The advantage of this is that I can then power other things like lights with the 12V BEC if it has enough amps.

http://www.ebay.com/itm/6-24V-12V-24V-to-5V-3A-CAR-USB-Charger-Module-DC-Buck-step-down-Converter-DIY-/221980647793

3) Instead of a BEC buy a DC to DC Buck Converter like below and then buy one of the USB modules linked in 1 & 2.  For some of those Buck Converters can you select the exact output voltage? How does that work?

https://www.aliexpress.com/item/DC-DC-Converter-Adjustable-Power-Supply-DC-DC-Step-Down-3A-LM2596HVS-LM2596HV-DC-Step-Down/32485142548.html?spm=2114.13010208.99999999.288.U9QBas

http://www.ebay.com/itm/272076571075

Let me know if I got that straight and which method is preferable and why!
```

---
## \#55 Posted by: Monte Posted at: 2016-10-31T17:38:28.203Z Reads: 122

```
Guys, just use the 5v output from Vesc. I made a usb output for my remote to charge it sometimes when i forget to charg it.
```

---
## \#56 Posted by: johnny_261 Posted at: 2016-10-31T17:50:20.168Z Reads: 121

```
Reading above, I thought this wasn't recommended due to additional heat buildup in the VESC?  Also I don't have a VESC right now so not an option for me currently.
```

---
## \#57 Posted by: Monte Posted at: 2016-10-31T17:51:24.608Z Reads: 119

```
Im not charging while riding. So it should not be i problem i think.
```

---
## \#58 Posted by: johnny_261 Posted at: 2016-10-31T17:52:38.866Z Reads: 120

```
Right right, of course. I was planning on using it to charge some lights while riding potentially so would be a problem for me potentially if I go the VESC route in the future.
```

---
## \#59 Posted by: Monte Posted at: 2016-10-31T17:54:48.199Z Reads: 119

```
At the moment i removed the Port to install a old Laptop fan because i had all the time overheat problems (Even on flats). Now i can ez pizi take steep hills.
```

---
## \#60 Posted by: Lebram Posted at: 2018-01-08T12:31:16.845Z Reads: 63

```
How do I use the vesc 5v output?
```

---
## \#61 Posted by: killaton Posted at: 2018-09-13T05:12:10.349Z Reads: 39

```
How would you mount this usb port to the enclosure?
```

---
## \#62 Posted by: Nordle Posted at: 2018-09-13T06:05:31.734Z Reads: 36

```
i would print something
```

---
