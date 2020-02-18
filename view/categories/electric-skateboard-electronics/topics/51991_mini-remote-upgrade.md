# Mini Remote Upgrade

### Replies: 49 Views: 2928

## \#1 Posted by: SkaterBoy58 Posted at: 2018-04-11T23:41:17.654Z Reads: 386

```
Have been using a mini 2.4GHz remote with dual vescs for about 8 months now with no issues at all. - very reliable and consistent. Love the trigger control .

Have now decided to do a bit of an upgrade on it with following features:

* Fit a small Li-Ion battery to replace need for AA cells - including micro USB charging port with leds

* Replace the mini remote stock slide power switch with a more robust rocker switch

* Fit a mini electric bell on side of remote -with a push-button switch - powered from new battery

I will include links for all material in case others want to repeat process.

Battery - went for Hobby King 750mAh  [battery ](https://www.amazon.com.au/dp/B0767CWL8L/ref=pe_2361882_283709292_TE_3p_dp_1)

![battery|551x479](upload://tGTXaxx89KHXbmD412ojAH7kuAP.jpg)

BMS - went for AliExpress - this has mini usb port and staus leds (charging and fully charged led)  [AliExpress 1S BMS](https://www.aliexpress.com/item/1-2-5-10pcs-Lithium-Battery-Charging-Board-TP4056-5V-USB-1A-Board-LiPo-Charger-Module/32846400654.html?spm=a2g0s.9042311.0.0.w3yJ6q)
![bms|487x390](upload://oTFGPcJWlliAwQM8FxzcY87JKGC.jpg)

Electric Bell [mini bell ](https://www.ebay.com.au/itm/ROCKBROS-Electric-Cycling-Bike-Bells-Horn-Rainproof-MTB-Bicycle-Handlebar-Bell/162695433212?ssPageName=STRK%3AMEBIDX%3AIT&var=461713258551&_trksid=p2057872.m2749.l2649)

First step is to carefully separate the two halfs of the remote body . Then remove AA battery cell pouch and this opens up quite a bit of depth to mount stuff
![mini 1|666x500](upload://ee5yjjS7IThGyKekSPZoOL1sXMt.jpg)

Then hot glued battery to bottom of housing
![mini 3|666x500](upload://i0YTWH0mIEksI06nZCiC9Do6uXB.jpg)

Then hot glued BMS to battery 
![mini 4|666x500](upload://pLI63A3cywJ3MtkwCFgPSXKKNbc.jpg)
![mini 5|666x500](upload://ac2TJyVVGxnrll0nRNv8hevTs09.jpg)

Will update as build progresses
```

---
## \#2 Posted by: dg798 Posted at: 2018-04-12T01:41:56.381Z Reads: 355

```
just a word of advice, dont keep the hotglue on the battery for too long as its not good to get liion cells too hot
```

---
## \#3 Posted by: SkaterBoy58 Posted at: 2018-04-12T23:34:41.063Z Reads: 346

```
Bit more progress - fitted miniature rocker switch and "charging"  and "fully charged" leds. These leds are wired in parallel with leds on BMS pcb. Works OK.
Put a bit of thought into the right position for the bell switch. - finally settled in a position were I can operate bell switch with right hand thumb without interfering with trigger throttle control.   I used a miniature tactile switch here to achieve positive activation.  ( [Tactile Switch link](http://www.altronics.com.au/p/s1178-spst-red-led-90-deg.-metallic-round-tactile-switch/)

Wired it all up including a diode in series with battery +ve to rocker switch ( inside red heat shrink)  to drop full charge voltage a bit.  Did a trial discharge on battery down to 3.4V  - then charged up OK via mini USB port with red light on for charging and amber light on for fully charged ( battery at 4.2V)


![mini 1|666x500](upload://tbFOD9TqeIvYKSe7FzuovLd9frr.jpg)![mini 2|666x500](upload://k3bVZQRDl1iLMmkacvsgaXDT87F.jpg)![mini 3|666x500](upload://ymXdmM3mYrMcI4OvbvYRiuRczhh.jpg)
```

---
## \#4 Posted by: will_manners Posted at: 2018-04-13T15:02:57.957Z Reads: 292

```
Looks great! What's the rated voltage range for the mini remote? Since it uses 2 AAs I assumed 4.2v would be too much. How has the remote handled the increase in input voltage?
```

---
## \#5 Posted by: SkaterBoy58 Posted at: 2018-04-15T01:46:03.771Z Reads: 278

```
I dont know rated voltage of mini is.

See post above - I connected one diode in series with +ve from battery to switch so mini electronics will only see 3.6V max for fully charged condition.
The mini bell has 3V cells and I think it will be fine operating at 3.6V (max)

The mini remote electronics draws 20mA so 750mAh cell will give around 35 hours before recharging.
```

---
## \#6 Posted by: deucesdown Posted at: 2018-04-15T03:34:54.592Z Reads: 263

```
I've been too lazy to do all this stuff, and it's paid off. I'm just gonna copy everything you've done here. :) Thanks for posting!

Is the mini bell mounted in the remote? Or is that the yellow wire?
```

---
## \#7 Posted by: SkaterBoy58 Posted at: 2018-04-15T03:48:10.516Z Reads: 268

```
no worries
i do not use the steering wheel on RHS of remote -so removed that and I will fix bell on outside of remote where the steering wheel was
Will post pictures when complete
Cheers
```

---
## \#8 Posted by: deucesdown Posted at: 2018-04-18T04:38:54.783Z Reads: 266

```
@SkaterBoy58 genius, especially the diode. Much thumbs up.

![IMG_20180418_002921|666x500](upload://yQrlQcg82prHidP0F9bvQDcrP7E.jpg)![IMG_20180418_003056|666x500](upload://tETgPuZPFnSPWMATkks4HsOyxwH.jpg) 

It's all fits in the 2xAA cavity under the cover, and is reversible for now.

The diode drops the voltage from 4.2v to 3.3v at the battery contacts with the remote turned on.

Issues:
- the usb charger module has a little bms built in. The overdischarge voltage cutoff is 2.8v, scary low for lipo. Perhaps eventually will put in a cylindrical cell, maybe even 18650.
- the board's charge rate is 1a, which is a bit higher than necessary. Generic usb ports will only give 500mah. I'll be looking to change a resistor somewhere to adjust this.
- the little voltmeter shows 4.01 but actual voltage is 4.2v.

Kind of scared to test this on a ride :) Maybe I'll leave it on for a few hours and see how it does.
```

---
## \#9 Posted by: b264 Posted at: 2018-04-18T05:52:34.839Z Reads: 242

```
18650 won't fit in a Mini Remote.  An 18500 or a 14650 will, take your pick.  I modded one as well...

Also I have an extra 14650...
```

---
## \#10 Posted by: SkaterBoy58 Posted at: 2018-04-18T06:26:09.764Z Reads: 252

```
The BMS I went with has adjustable charging from 130mA to 1A by adjusting a resistor - see details in BMS  link above.   
This BMS is used for charging only so no undervoltage discharge protection  ( which I don't see as a major problem) 
The mini remote led starts to flash on low voltage but I haven't measured when this starts. 
 I will end up charging remote after every few rides so will probably never get below 75% . 
I may be able to fit a small voltmeter ( similar to yours) above the rocker switch - just to finish it off.  

Cheers

Edit - To add to above - the LiIon battery itself has a small BMS inbuilt into top of battery - presumably to provide over and under discharge protection for the battery

![LiIon cell|172x291](upload://ixebAFmbRSaqvQ8ZyvOzpPfstD.jpg)
```

---
## \#11 Posted by: ervinelin Posted at: 2018-04-18T07:40:33.315Z Reads: 248

```
![IMG20171116065413|281x500](upload://xGeZucIHgzp68ILSGCZmZ7gMi8j.jpg)

I went one step further with my mini remote mode...
```

---
## \#12 Posted by: SkaterBoy58 Posted at: 2018-04-18T08:12:40.263Z Reads: 232

```
cruise control or horn pb?
```

---
## \#13 Posted by: ervinelin Posted at: 2018-04-18T11:10:52.888Z Reads: 230

```
The button? No it's for changing telemtry information on the screen
```

---
## \#14 Posted by: SkaterBoy58 Posted at: 2018-04-18T23:44:19.241Z Reads: 234

```
Managed to fit a small volt meter    [mini voltmeter link ](https://www.aliexpress.com/item/0-28-Inch-2-5V-30V-Mini-Digital-Voltmeter-Voltage-Tester-Meter-LED-Screen-Electronic-Parts/32737103272.html?spm=a2g0s.9042311.0.0.8MTU2p) above rocker switch . Could connect this volt meter direct to battery if you want direct battery voltage displayed. Looks quite nice . These are simple two wire devices so connected -ve to BMS output -ve and +ve after rocker switch. This draws 5mA current so about 25mA in total including remote electronics. Basically cut a rectangular hole in enclosure and hot glued display in level with outside face- then poured hot glue over the lot to hold it all in place.

![mini 15|666x500](upload://q9VmRDYjeYNawDW6nDQdPVXLBDA.jpg)![mini 16|666x500](upload://8juffuYtgEut8QOxjuodCAsFJXP.jpg)
```

---
## \#15 Posted by: SkaterBoy58 Posted at: 2018-04-18T23:49:11.294Z Reads: 229

```
@ervinelin   any details of this remote upgrade?
```

---
## \#16 Posted by: ervinelin Posted at: 2018-04-19T00:29:14.205Z Reads: 228

```
See here [http://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231](http://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231)
```

---
## \#17 Posted by: SkaterBoy58 Posted at: 2018-04-20T00:01:47.934Z Reads: 233

```
Next thing is to attack the bell. The RockBros mini bell looks like ![rockbros bell|458x403](upload://mdRcaAswddw1WEPHgjv2X8P1cBR.jpg) 

First thing is to pull it to bits (as per normal) and see how it is built. It has 2x 3V button cells in it so 6V supply.
You take off the rubber cover and can get to the internals. ![mini 20|666x500](upload://cIXoYUppzC51cKZyXhtSKzIOZON.jpg) 
First thing is to cut off the 3V cell metal holder . Then soldered +ve and 0V wires in place of cell. I will connect these directly to battery to give it a bit more voltage and to provide constant supply to bell pcb. Then soldered two wires in parallel with switch on horn ( yellow wires) for connection to the tactile switch on remote handle . If you don't have power on bell pcb constantly - you need to set up the preferred sound every time which is a bit of a PITA.  ![mini 21|666x500](upload://qCvvi1z8hB1cYOSGb1BtrdFxsfA.jpg)

Then cut rear plastic cover with a junior hacksaw to provide a level surface to mount bell to side of remote. 
Used araldite to glue bell mount to remote poking wires through hole that was for steering pot wires . ![mini 22|666x500](upload://ubhOHZtNYDjcWMeC2fwO0jkvvxk.jpg)  

Final step is to cut rubber cover to suit and stick back on .

Tested out and works fine . There are three choices for the sound and you change by long press of bell pushbutton.
```

---
## \#18 Posted by: deucesdown Posted at: 2018-04-20T14:17:53.766Z Reads: 210

```
[quote="SkaterBoy58, post:14, topic:51991"]
Managed to fit a small volt meter    mini voltmeter link
[/quote]

Are you finding this meter accurate? I'm off by .2v at 4.2v. I think maybe there's a calibration resistor...
```

---
## \#19 Posted by: SkaterBoy58 Posted at: 2018-04-22T12:39:26.268Z Reads: 220

```
All complete and works well

![mini 41|600x500](upload://9WxsJX6AVqnXX74dIhNFfIwHlb3.jpg)![mini 45|600x500](upload://aHOA8c2wZ2wbF9deeayFxWjvAu9.jpg)![mini 40|600x500](upload://aH38EAuDvjX3qWoZPnFDR50NFis.jpg)
```

---
## \#20 Posted by: SkaterBoy58 Posted at: 2018-04-22T12:42:20.944Z Reads: 212

```
checked on my multimeter and display reads about 0.1V higher. no big deal for this application!
```

---
## \#21 Posted by: deucesdown Posted at: 2018-04-25T21:42:21.753Z Reads: 194

```
Hey I zoomed in on your gutshots. Your voltmeter has a pot on the pcb, which I bet is for adjusting voltage offset. My voltmeters have a resistor instead.
```

---
## \#22 Posted by: SkaterBoy58 Posted at: 2018-04-29T03:42:10.697Z Reads: 189

```
Thanks for that 
you are absolutley right re calibration pot on back of these mini displays!
need a magnifying glass to see it and a bees dick size screwdriver to adjust pot but it does change displayed voltage
Cheers
```

---
## \#23 Posted by: Scoo_B_SK8 Posted at: 2018-04-29T04:26:32.213Z Reads: 184

```
NIce work! @SkaterBoy58 & @ervinelin
```

---
## \#24 Posted by: Dmaxx Posted at: 2018-04-29T20:49:12.349Z Reads: 189

```
@SkaterBoy58, did you simply remove original power switch and direct solder the positive lead somewhere in that location? Ive got everything wired up and it works, just left original switch on, but id like to remove that thing for peace of mind
![20180429_132819|281x500](upload://o9alFekzq3ghEbQT6eytsn8Zyz6.jpg)
```

---
## \#25 Posted by: SkaterBoy58 Posted at: 2018-04-29T22:08:36.356Z Reads: 182

```
left it in on position 
then cut off plastic toggle
and hot glue over old switch hole
cheers
```

---
## \#26 Posted by: Allofyoush Posted at: 2019-01-14T01:15:29.335Z Reads: 138

```
do you guys want to make tutorials for those mods? I'm interested in getting the mini, but the only thing I don't like about it is that you can't recharge it.
```

---
## \#27 Posted by: b264 Posted at: 2019-01-14T07:31:10.027Z Reads: 144

```
This is DIY, just look at what we did and take inspiration ;-)

![20171227_015215%20(copy)|350x499](upload://kqL5LqGoTWwWUiP3IoJXGG4jyRu.jpeg) 

![20171227_024410|249x499](upload://hU7q0Sn8g83QkmpxuUgELVutQxE.jpeg) 

![20171227_031414%20(another%20copy)|690x345](upload://xthO8N98q91xTGY2oMGJaVGzEL6.jpeg) 

![20171227_031929|690x345](upload://8aOydlQtfwEO2CuSZvGJcLIo9gS.jpeg) 

![20171227_033012|690x345](upload://8alVEAu3KGQkofoCMOaLezafsM7.jpeg) 

![20171227_033105|249x499](upload://6qT5MpjlikhVY4okhZClAa6mBjT.jpeg) 

![20171227_033124|690x345](upload://7upOlYAa46tq9TMuTv4ta9FPs0u.jpeg) 

![20171227_033152|249x499](upload://h6NCz6BIHk00fUGS3qPuVKhgr1w.jpeg) 

![20171227_033157|249x499](upload://x0b2uyC5UeMJqrnCGLFRCpFClCF.jpeg) 

![20171227_033216|249x499](upload://1jB1RGWrn55Q2LuyPwI7DjmkZCG.jpeg) 



I can say that 2200mAh is way overkill and I've only recharged this one once in 13 months (despite heavy usage) so you could even use a 100mAh if you wanted to, without issue.

Also never use glue.  *Ever.*  Use JB Weld or another kind of epoxy and follow the directions exactly.
```

---
## \#28 Posted by: SanderG Posted at: 2019-05-14T21:07:20.809Z Reads: 104

```
So if i understand correct you just need to place a diode in front of the rf remotes board to not fry it with 4.2v? Wiil any kind of diode work? How is that charger/protector working out? Cut of voltage good/safe?
```

---
## \#29 Posted by: b264 Posted at: 2019-05-14T21:52:34.965Z Reads: 103

```
I didn't even use a diode, I just drive it directly on 3.0V to 4.2V from the lithium-ion cell.  I've been using it for 18 months almost daily.

"Because it worked for me" generally does NOT ever equate to "it's safe to do".  (as evidenced by people running 12S and 13S on VESC hardware)  But I don't personally think it's a problem at all.  But, I also have no schematic or proof of that.
```

---
## \#30 Posted by: Arzamenable Posted at: 2019-05-15T00:12:27.684Z Reads: 92

```
[quote="SkaterBoy58, post:22, topic:51991"]
bees dick
[/quote]

This is going in my vernacular.
```

---
## \#31 Posted by: mutantbass Posted at: 2019-05-15T00:16:44.057Z Reads: 93

```
ditto this. Been using a 14500 battery from 4.2v downwards. no problems
```

---
## \#32 Posted by: b264 Posted at: 2019-05-15T03:44:31.742Z Reads: 86

```
I found that a 14650 or an 18500 both fit (as well as a 14500) but an 18650 does NOT fit inside a Mini Remote unless you remove support pieces that you really don't want to remove.
```

---
## \#33 Posted by: SkaterBoy58 Posted at: 2019-05-15T03:58:44.820Z Reads: 83

```
fairly common Aussie slang term for 2/5 of 5/8 of FA
```

---
## \#34 Posted by: SanderG Posted at: 2019-05-15T05:37:43.471Z Reads: 84

```
So 4.2v should be good or do you need a stepdown like this? ![image|230x500](upload://6uhkJxxTNiVI7J0qtETjYnNq5bL.jpeg)
```

---
## \#35 Posted by: b264 Posted at: 2019-05-15T05:42:04.720Z Reads: 80

```
I personally would not use a stepdown, just straight 4.2V.

Also, be aware that a single 18500 li-ion cell lasts so ridiculously long in a Mini Remote, that it will very rarely be running at 4.2V.  Maybe once when you charge it, then a year or two later when you need to charge it again.
```

---
## \#36 Posted by: SanderG Posted at: 2019-05-15T05:44:30.484Z Reads: 82

```
Yea but im gonna use a 1s 750mah lipo...
```

---
## \#37 Posted by: b264 Posted at: 2019-05-15T05:45:35.896Z Reads: 81

```
It will last so long....

way longer than 750 milliattohours
```

---
## \#38 Posted by: SanderG Posted at: 2019-05-15T05:58:04.506Z Reads: 77

```
Yea but ist kinda big, i wanna make a new design and print it, so wanna make it really compact. Whats the capacity of the cell you have?
```

---
## \#39 Posted by: b264 Posted at: 2019-05-15T06:29:57.492Z Reads: 76

```
[quote="SanderG, post:38, topic:51991"]
Whats the capacity of the cell you have?
[/quote]

I modded one with a Panasonic NCR18500A (2000mAh) and it's overkill by about 5 times or more.

![20171227_031414%20(another%20copy)|690x345](upload://xthO8N98q91xTGY2oMGJaVGzEL6.jpeg) 

But then my other 6 Mini Remotes I just use as-is because the mods weren't worth it -- they really didn't make the remote any better.
```

---
## \#40 Posted by: SanderG Posted at: 2019-05-15T07:32:37.191Z Reads: 75

```
Doesnt it suck to use AA batterys?
```

---
## \#41 Posted by: b264 Posted at: 2019-05-15T18:57:04.908Z Reads: 69

```
I thought so at first, but if you get the "Energizer Ultimate Lithium" AA batteries, they last so long it's not really an issue.  It's more of a mental annoyance knowing it's not rechargable.

But, definitely mod it if you want to :smiley:
```

---
## \#42 Posted by: SanderG Posted at: 2019-05-16T05:50:53.548Z Reads: 63

```
Yea gonna put an 18650 inside i think :p

![image|230x500](upload://qTh6RzJKG5TJOWRlbHO9yPebSd5.jpeg)
```

---
## \#43 Posted by: b264 Posted at: 2019-05-16T06:46:30.522Z Reads: 59

```
It's not going to fit unless you cut out supports -- supports that are needed if you ever crash.  If you land on the remote in your hand, and you've cut those out, you might smash the remote.
```

---
## \#44 Posted by: SanderG Posted at: 2019-05-16T07:32:59.984Z Reads: 58

```
Im gonna make a new case and 3d print it, i hate this design of case lol ;) gonna re design it so it has a wheel on top instead of the trigger style.
```

---
## \#45 Posted by: b264 Posted at: 2019-05-16T07:43:31.854Z Reads: 56

```
I think that's already been done if you look around.
```

---
## \#46 Posted by: SanderG Posted at: 2019-05-16T09:23:47.490Z Reads: 53

```
Yea i know ;) just need to mod it to fit this kind of circuit board, i do not think it has been done with this remote?
```

---
## \#47 Posted by: b264 Posted at: 2019-05-16T09:50:38.287Z Reads: 50

```
It has been
```

---
## \#48 Posted by: SanderG Posted at: 2019-05-16T11:34:40.318Z Reads: 46

```
You know of any files?
```

---
## \#49 Posted by: b264 Posted at: 2019-05-16T11:36:14.816Z Reads: 47

```
https://www.electric-skateboard.builders/search?q=mini%20remote%20upgrade

https://www.electric-skateboard.builders/t/the-avio-mini-remote-mod/72074

https://forum./t/how-to-bind-the-mini-remote/95
```

---
