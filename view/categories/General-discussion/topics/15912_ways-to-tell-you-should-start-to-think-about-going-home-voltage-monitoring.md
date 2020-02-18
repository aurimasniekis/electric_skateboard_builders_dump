# Ways to tell you should start to think about going home (voltage monitoring)

### Replies: 40 Views: 3307

## \#1 Posted by: Okami Posted at: 2017-01-11T19:55:20.746Z Reads: 267

```
Hi there! I was thinking today..

 **how do you tell when you should start thinking about heading home and how do you tell when batteries are getting low?**

I think evolve had a good idea that it shows kilometers made or kilometers left on their new remote.. 

Thinking in similar fashion, I thought there could at least be some sort of beeper, similar like lipo alarms has, but for different voltage levels.. let's say, one beep is when you reach 50% battery left, then 30% left has 2 beeps, then 15% left has 3 beeps..

**I know u guys use these ''coulometers'' where the voltage / battery is shown as percent and you probably judge your distance from that.. but with this topic I wanted to come up, perhaps, with a few innovative / unique ideas, which could be used or implemented..**

I think a good way is also to put voltmeter in front of the board or just make a simple 4-5 led indicator, which also shows the voltage / battery left with how many leds are light (or in which color..)

---

Anyways, Im using wattmeter myself (with total voltage shown), so basically when voltage is around 21v (in my case) I know the cells are around 3.5v and that's when the ride should be soon ended.. but it is a bit hard to tell how much juice I got left when im in the middle range.. so a display with percentage would be better suited for this..

Lipo alarms (cheap ones) suck in this application, they are quite loud and it is not easy to turn them off once they start buzzing.. plus, for me they are inaccurate and show a big wrong voltage for a few cell groups.
```

---
## \#2 Posted by: anorak234 Posted at: 2017-01-11T20:05:59.259Z Reads: 250

```
figure out wh/km consumption in your system by testing with voltage meters, so that you can learn the maximum distance your board takes you. Track your route using GPS to know how far you've travelled and use that to see how much farther you could go...
```

---
## \#3 Posted by: Okami Posted at: 2017-01-11T20:12:54.277Z Reads: 245

```
Yeah I've already done this .. but the best way would still be direct kilometers/ miles, like the evolve does..

I know that my consumtion (emtb) is around 900mah per km or about 20wh/km (should try harder tires) but to make a calculation in real time I still need to figure out my batteries parameters (at what voltage how much is left etc)

Would be great to know how much km I can do with 1volt of drop in total battery voltage.. 

So yeah, thanks @anorak234 for leading me onto this path.. I might actually consider just wiring up my wattmeter, so that it stays on the whole ride and then just see the total ah consumed and from that I can calculate how much is left.. this should give me a somewhat accurate result.. the only donwside is that ah consumtion is not shown constantly on the screen.
```

---
## \#4 Posted by: treenutter Posted at: 2017-01-11T20:27:45.401Z Reads: 227

```
@Okami here's my low-tech solution: I do a range test on my build from a full charge. Then I use the distance I've travelled to estimate available charge at any given point. It's not a great system because unpredictable factors influence the use of energy (temperature, terrain, detours from the planned route, etc). However, I've never been stranded using this system. 

I carry a skate tool with me and my backup plan is to disconnect the belt and push home if needed.

A better solution would be a programmable power meter that could use range from full-charge as an input to calibrate available energy.

Yes voltmeters suck because as we all know there is a long period during use where voltage is the same and then it rapidly drops!
```

---
## \#5 Posted by: Mark Posted at: 2017-01-11T20:44:56.912Z Reads: 216

```
When my acceleration is noticeably lower
```

---
## \#6 Posted by: Okami Posted at: 2017-01-11T21:05:42.778Z Reads: 216

```
@treenutter, yeah this is something I am aiming for.. Im not quite sure yet how to make it happen but this ''arduino code / device'' thing should be able to measure spent energy and available energy.. 

I imagine something like cars have as ''bort computer'' (not sure how it is entirely called in usa) 
Basically it shows consumtion and other stats since the engine was started or sometimes from a longer period of time also..

So yeah, it should be able to see the average wh consumtion over a period of time or best over distance and from that give some sort of estimate how much range is left.. not sure how practical this might manifest in real life as the terrain and riding conditions might be quite diverse.. to make accurate prediction / calculation but there should be at least some guidelines to follow..similar like with this full/empty battery thing and the total distance you can do with it..

--

I imagine it could be way easier to manifest this ''prediction of distance left'' if someone is having a vesc.. that vesc monitor app looks quite handy and I believe it could do real precise measurements and suggestions too.. 

Unfortunately im not a vesc user yet and there's still ppl riding with non-vesc esc's.. so this ''product'' / device might be handy for more than a dozen ppl, if someone comes up with it..

---

@Mark mh that is also a good indicator but unfortunately it might be too late to find out you dont have much battery left.. If I can do 10km  / 6miles with full battery and im on ''budget'' with left battery capacity, it might be hard to tell whenever I can do these extra 3 - 4 km (~2miles) or not.. 

---

Will think about doing some more tests... especially at the lower end of voltage, since right now I have usually rode very conservatively.. only once I've ridden the batteries so empty that I could not get any speed at all from them..
```

---
## \#7 Posted by: NickTheDude Posted at: 2017-01-11T21:15:16.103Z Reads: 198

```
I think you'd need to gather a significant amount of data in a variety of different situations in order to make an accurate prediction of leftover range. Even something like windows can't properly predict the amount time a laptop battery has left.
```

---
## \#8 Posted by: Randyc1 Posted at: 2017-01-12T00:01:53.681Z Reads: 187

```
A simple $6.00 voltage meter is all you need to know excactly how much is left! <img src="/uploads/db1493/original/2X/1/18ef007ea900607e13a719f82570dfc9f61ada3c.jpg" width="690" height="388">
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-01-12T00:02:09.021Z Reads: 188

```
These 2 videos could be interesting for you. there you can see how the wh consumption changes with the way we ride. In the first video i tried to keep a constant speed at around 25km/h and in the second i did the same round and tried to be quick. And you can see that the consumption goes up by roughly 84%.

What really saves energy is when you don't accelerate and just push to your speed and only use the motor to keep the speed. This way you can safe a lot of energy.

https://youtu.be/Y2RGmAlJJy8

https://youtu.be/jmV2Q9WTbGk
```

---
## \#10 Posted by: Kaden56 Posted at: 2017-01-12T00:36:07.419Z Reads: 176

```
The % battery display on my DIY Electric battery pack is nice to have but when I hop off the board I can always count on it going up at least 5% to 10% within ten minutes of not riding. With this in mind my go home point is around 42% or so and I know I'll be fine :)
```

---
## \#11 Posted by: PXSS Posted at: 2017-01-12T02:21:02.289Z Reads: 172

```
Most accurate way:
-Get discharge curves for your pack
-Get a voltmeter on the board
-Figure out how much power you use in several conditions: slow cruise home, average way of riding, regular climbs, max climb, top speed. 

Based on discharge curves at a power condition, you can figure out what your voltage should be at 50%
You could also step off for a minute and let the voltage rise to its no load and then you only need the no load curve. As long as you have a .01v resolution, you should be able to measure capacity within a few percentage points. 

The easier way is to buy a coulomb counter and have it on your board. You know the capacity of your battery, you know how many ah you've spent, you know how much you have left. If you do it this way, you need to leave some buffer on the lower end depending on how hard you've been riding.
```

---
## \#12 Posted by: Mobutusan Posted at: 2017-01-12T05:38:34.612Z Reads: 171

```
Interesting comparison videos. Watched them both a few times. I really need to get my VESC set up and pick up one of those BT modules. They are just too cool.

What battery/motor/gearing were you using in that video? I assume it's 12s LiIon, but I was surprised to see your voltage sag from 49 to 35 volts under heavy acceleration. Is that normal?
```

---
## \#13 Posted by: Jebe Posted at: 2017-01-12T06:38:31.704Z Reads: 165

```
the evolve is only a guestimate. Personally I ignore it's % reading and go by the cell voltage readout.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-01-12T08:38:15.482Z Reads: 159

```
@Mobutusan Those batterys are from harvested **broken Laptop battery packs**. So they are absolutely not made for that purpose. But they work. So the voltage sag is huge with them. But i still can get around 2000W of power. Even 2500W is possible when they are fully charged. And gearing is 14/36 with 2 190kv Enertion R-SPEC.
```

---
## \#15 Posted by: devin Posted at: 2017-01-12T08:45:10.769Z Reads: 154

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#16 Posted by: jga Posted at: 2017-01-12T13:38:54.947Z Reads: 151

```
Sorry, I'm volunteering today to ask the dummy question in this post: I thought the ESC/VESC had a cut-off limit where the whole thing would stop to avoid going too low in voltage?
Are we just here talking of not being cut-off 5Km from home in the middle of nowhere and not actually avoiding to damage the battery?
```

---
## \#17 Posted by: Okami Posted at: 2017-01-12T13:40:29.604Z Reads: 135

```
@jga No, Im referring here to outside methods of reading your total battery voltage.. and being able to tell midway when battery is reached 50% of usable capacity.. to head back home (if it is a ''joy ride'' where you basically just go in one direction and then head back..)
```

---
## \#18 Posted by: Okami Posted at: 2017-01-12T13:46:53.375Z Reads: 144

```
@PXSS 

You know, I was reading your first part of text and you just made me: woah.. wont probably do this in the future :D 

Though I would agree that if there was a specifically designed coulometer with some advanced functions, like predicting the distance left based on your existing speed and power consumtion, then yes, it might work..

Otherwise I would probably believe my ''gut feeling'' and look at simple capacity display and tell from that how much further can I go :D

---

So thank you too @devin for the tip, as I will probably just improve my current wattmeter (coulometer) and will make it stay on the whole time.. it just happens that if you dont have outside power attached to it, it loses all its values once it is reset. 

This way it is not easy to keep track of the energy spent, if it is reset each time you turn your board off..

---
```

---
## \#19 Posted by: Mrmoonlight Posted at: 2017-01-12T15:31:07.137Z Reads: 136

```
I just use a coulometer. Check my percentage before my ride and make sure I have at least half that to get back home. How far you can go on how much depends a lot on how you ride, the temperature, grades, terrain... I've gotten as much as 30 miles on a charge and as little as 15. If I'm running low and home is still a ways off, I push more to start off and up hills.

No meter is going to be anything more than a rough guestimate of how many miles you have left. There are too many variables. One thing for sure is that having any sort of meter helps a lot. My Gen2 Evolve didn't have any indicators so you had to guess. Had to push myself home a couple times. Especially a pain since you can't tell how much charge your battery has when you first start out. Once I did a DIY build with the LCD display, I haven't been stranded once. I just know that when I get down to 35%, I have about 8 miles left. 10 if I push a little.
```

---
## \#20 Posted by: PXSS Posted at: 2017-01-13T06:53:24.272Z Reads: 125

```
Tell me how much power you use on average on your way home and what type of battery you have. I'll tell you at what voltage at that power and no load you have 50% left.
```

---
## \#21 Posted by: lowGuido Posted at: 2017-01-13T07:49:22.915Z Reads: 111

```
One of my boards actually has a primary and a secondary pack. So once the primary is out you know you shpuld have enough juice to get you at least most of the way home.
```

---
## \#22 Posted by: okp Posted at: 2017-01-13T08:10:14.235Z Reads: 113

```
When I ride, I just use endomondo... when I reach 25/27km I know that's gonna be the end soon. In fact you need to be consistant at riding, know your board and how to maximize the miles coverage when having a blast in the streets! cause that's the most important !!!
```

---
## \#23 Posted by: Okami Posted at: 2017-01-13T10:19:34.842Z Reads: 120

```
It's the cold season here so once again I dont have many chances to take the board out (uh).

I wont be really able to tell average power consumtion, as im running car esc with just a coulometer/wattemeter installed. From the few ''loose'' tests I did, it looked like board consumes about 20wh per km or close to 900mah/km (at ~8000mah 6s4p li-ion, 4.1v-24.6v when fully charged).

I still need to take a test at constant speed and just straight road, I was willing to this but the next day the snow came, so I had to leave this for later.

---

As of now, when voltage is around 3.8-3.9v per cell I assume it is somewhere in the middle!

I would like to have percentage display I think, so perhaps I will just look into getting one of these coulometers ppl are using! But I was concerned about the reliability of these percetanges.. as I was not entirely sure does 5-10% percent stand for the same distance in all scenarios (voltage levels).

I know that my turnigy charger shows up around 10% charge level, when the cells are at ~3.5v no load voltage. Though, its max charge voltage is set to 4.1v per cell, so I assume it calculates the percentage level using these 0.6-0.7v of range. Not sure what counts 0% for it, have not ridden the board so far yet :)

--

So far I usually just assume that I can do a distance of 8-10km, and so far the longest recorded one was about 6-7km. But this takes into consideration that you need to log the kilometers with a phone app which is not always so conveniant, if you want to go somewhere in a hurry without looking at the phone every 5-10min  /2-3km to check the distance :D

---
<img src="/uploads/db1493/original/3X/9/e/9e00b8e563d680b346a0dc42660ebcfadfd15793.jpg" width="362" height="155">

This is the deepest I've discharged my battery, unfortunately I did not do a full discharge test on these batteries but I might do a seperate test on just one battery at ~3A load, to see what capacity it has.. From the manufacturer, it states these batteries have 2100mah capacity, or around 2000mah when discharged at 5+ A per cell. 

As im not pushing them till 4.2 and I also stop at around 3.5v I assume 7.600mah is pretty fair.
```

---
## \#24 Posted by: Okami Posted at: 2017-01-13T12:36:56.368Z Reads: 112

```
@PXSS I did not mean to kill the conversation with my lenghty text / detailed description..

As I was not able to tell you average watts consumed I tried to answer in different terms.

So far I only know that I reach a peak of 800-1200w very easly but Im not sure how much is spent on a regular ride on average. As I said, I will need to pump the tires even more(as they are not max inflated) and just do a few tests at different constant speeds to see what wh consumtion/ mileage I get :) 

Though, this is maybe a side topic, as I opened this discussion to dwell upon ideas on how I could see the energy left in batteries in a better way to determine the distance. 

And so before I know what distance at which speed can I do, I do like to look at the possible options of showing voltage / percentage / estimated capacity left etc :) (which was already done in the topic anyways ;) )
```

---
## \#25 Posted by: PXSS Posted at: 2017-01-13T13:22:39.173Z Reads: 102

```
No worries. It's 8am. Thats why I didn't reply! I will write a response later :slight_smile:
```

---
## \#26 Posted by: Okami Posted at: 2017-01-13T13:49:15.311Z Reads: 100

```
On a side note - I remembered that this app ''Runkeeper'' had the option to tell with sound/voice when you have made 1km/1mile, so if you can trust the gps/app accuracy, this might also be a great way to tell when to go back.. 

_(Endomondo might also offer this feature but last time I used it, it did not call out the distance out load, might perhaps search for this option, as I installed it only recently and have not checked all of it)_

Though this will probably only work if the power consumtion is constant..but at least it should give a somewhat accurate estimate on how much has been traveled versus max possible distance and then looking at the voltage display (or coulometer), determine about how much more it is possible to do based on that.

On a side note.. vesc monitor app still would be the best, no need to turn on logging apps on phone (since they tend to get stuck for me or not always easy to activate them before the ride)


---
```

---
## \#27 Posted by: SORRENTINO Posted at: 2017-01-13T14:39:23.580Z Reads: 92

```
Why not use a bluetooth chip that sends data to your phone? I know theres a bunch out there now with apps. Im sure there is a setting to alert your phone when you reach your pre set volatge
```

---
## \#28 Posted by: Ackmaniac Posted at: 2017-01-13T14:54:57.896Z Reads: 100

```
Would you guys be interested in smart display? 
You need a Arduino Nano for it and a SSD1306 display.
Here is a example of what i mean. It can show way more information then only the range.
It could be attached to the slave VESC so that the master has the Bluetooth connection and this one the connection for the display. Originally that display was planned from me to add it in a remote so that via the remote the drive modes could be changed. But then i didn't find a propper way to add all the components. Maybe i find the time again in the future to finalize that. But it could be modified to add the display at the front truck mount when it is a dropthrough  or in the enclosure. Could give a lot of information. And with attached buttons the drive modes could be changed.

https://youtu.be/JkzSKb3Kmic

But as i already told, maybe in the future.
```

---
## \#29 Posted by: Okami Posted at: 2017-01-13T21:59:46.267Z Reads: 100

```
I like the idea @Ackmaniac . 

But could somebody tell, is it possible **to feed the battery pack's voltage into the arduino**? I assume there needs to be some sort of voltage step down module or a shunt module, which is able to measure the voltage/current. 

With voltage step down, I assume some resistor - voltage dividers might work, at least that is how I understand a higher voltage is measured on an arduino, it will just miss the most precise measurements this way, if it in 1024 bit / step in or whatver system converted. 

Not so smart about shunts, so if someone has experience with them, that would be great!

Shunt would be best, because it could measure capacity / amp hours, too, but for the start, simple volt meter would also suffice.. It would be great, if it was possible to make a custom percentage display based on voltage left :) perhaps with additional sound signal or flashing display at set levels..
```

---
## \#30 Posted by: Ackmaniac Posted at: 2017-01-13T22:08:02.440Z Reads: 95

```
Sadly in the video the battery percent value didn't work because i adjusted it to a 12S battery. But it was comnnected to a 10S. So it shows 0%. Value in the upper right corner. Adn because of that the Range (value R) also was calculated to 0.
And this display works with the VESC. So there is no need for any resistors because the arduino can be connected directly.
```

---
## \#31 Posted by: Okami Posted at: 2017-01-13T22:32:56.151Z Reads: 97

```
I know. Still not owing a vesc, so I will have to pass this.. (unless someone ''donates it'' for ''scientific purposes'' haha)

I will create a seperate - arduino only - thread about this. It will / should work for 25v max at first, so ideal for 6s Li-ion 4.1v x 6cells users!

Anyways, nice idea / job @Ackmaniac I believe other ppl will also find it useful, just tell them about it, create a seperate thread or post this info into the topics about remote controllers,, / vesc monitor app, I believe it might catch up, who knows..
```

---
## \#32 Posted by: Okami Posted at: 2017-01-15T01:57:30.103Z Reads: 97

```
Will add these little guys to the discussion:


http://www.ebay.com/itm/Lithium-Battery-Capacity-Indicator-Module-Blue-Display-Electric-Vehicle-Tester-/122299410400?var=&hash=item1c799ce7e0:m:mPITzCDzV3Wbf-mBUXYWZlw

<img src="/uploads/db1493/original/3X/f/a/fa5ea4c4e368211c1a0a6267e50b9ff7ace69577.png" width="690" height="151">

----
http://www.ebay.com/itm/Waterproof-12v-24V-48v-72v-Acid-lead-Battery-indicator-capacity-Tester-voltmeter/232099381203?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D40778%26meid%3D4d563d892e994567a7a773fb84743d8c%26pid%3D100005%26rk%3D1%26rkt%3D6%26sd%3D221797490150

For this one price not that great, I hope to find cheaper units for these, though, the principle with bars/percentage or volts included, looks really nice!

---
http://www.ebay.com/itm/12V-24V-36V-48V-LCD-Battery-Capacity-Tester-Indicator-car-Lead-acid-Lithium-Cell/222293145050?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D40778%26meid%3Dbe8753b7419541bd95d80d5f45b006f4%26pid%3D100005%26rk%3D2%26rkt%3D6%26sd%3D172143986261

Did not know these can be so cheap.. They only got 5 bars of voltage indication (some more perhaps, would have been welcome) but non the less in overall this display looks really good.
```

---
## \#33 Posted by: mrplaygood Posted at: 2017-02-08T17:46:14.796Z Reads: 79

```
Hi,

This thread is awesome, it's exactly what I've looked for. 
I'm on a halt right know because I try to figure out how to make my own battery indicator with 4 or 5 LEDs. 
I found a lot of these voltage indicators which @Okami already posted but I don't like the look and would love to have something like the old MacBooks had.
https://i.stack.imgur.com/fzWwr.jpg
I already read about Zener Diodes and op amps and so on... Fact is I'm to damn stupid for that :D 
Maybe someone of you could help me out. When I have results I would love to share these with all of you.

Thanks a lot!
```

---
## \#34 Posted by: Okami Posted at: 2017-02-08T18:00:48.136Z Reads: 77

```
I would advise to you to get ''acrylic panel''.. Then you mount some leds, perhaps SMD preferabbly onto that panel.. You could buy ''individually controllable'' Led stip.. you wouldnt need a lot of it..

Then hook that up to arduino.. get a voltage reading for just one cell from your balance connector.. then make the arduino display it on your individually addresable led strip..
```

---
## \#35 Posted by: mrplaygood Posted at: 2017-02-08T18:05:54.310Z Reads: 75

```
So you mean instead of meassuring al 8 cells in series (about 33,6V - 25,6V) just meassure one(4,2V - 3,2V) and apply that to all the other cells?
```

---
## \#36 Posted by: Okami Posted at: 2017-02-08T18:07:33.863Z Reads: 84

```
yeah, if you look up what I wrote elsewhere there was one user who already did this.. you get ''better resolution'' this way.. as arduino can only measure ''1023 steps'' of voltage, I believe.. It has a range of 0-5v.. and you have ''bring down the voltage'' anyways.. for the arduino to be able to read it..

At least this is how I understand it.. I havent yet hooked up mine.. been busy doing other things.. but non the less, it just seems easier to base everything on single cell, especially if your cells stay ''in shape'' more or less.. all the time

If you got lipo pack.. u might as well go for full voltage.. then you would have to downgrade it with some resistors..

---

http://www.instructables.com/id/LED-Glass-Desk/

I think you should strive for achieving / getting something like that
```

---
## \#37 Posted by: Okami Posted at: 2017-02-08T18:26:50.251Z Reads: 86

```
Here are some of the ''options'' I think you should go after:

http://www.ebay.com/itm/DIYmall-7Bit-8bit-12-bit-16-bit-24-bit-WS2812-5050-RGB-LED-Lamp-Ring-Light-/282225658296?var=&hash=item41b5f5c9b8:m:mrgI0fJ1ljXSc3QbEbBUxgQ

Click the last item - 8bit led strip

--

If you want something from usa.. for a bit more money, you can look up ''NeoPixel Ring''..

Though you will have to look up some tutorials on how to do this..

The leds inside of these are called WS2812.. there should be some tutorials around the net on how to control them.. you can basically choose any color you want for them, if you know how to adjust it..

---

Here's some resources on how to do that ''voltage divide'' thing:
---


https://startingelectronics.org/articles/arduino/measuring-voltage-with-arduino/

https://learn.sparkfun.com/tutorials/voltage-dividers

There's a calculator on the 2nd site on how to calculate what resistors you need, I believe.

--

As said.. if your voltage stay all the same more or less, I think this step can be left out.. but if you want it somewhat more reliable.. to see the total voltage, then go for ''voltage dividers'' option..
```

---
## \#38 Posted by: mrplaygood Posted at: 2017-02-08T18:33:14.489Z Reads: 79

```
Hi @Okami,

I am completely into Arduino, so this won't be a problem for me. I'm just really bad in calculating electronics because I never really learned it ;) I already have a Neopixel ring but will use a strip for this project. Thank you very much for this idea of just measuring one cell instead of all 8S.

When I'm ready I will upload the code an some pictures but that could take a little while :)
```

---
## \#39 Posted by: Okami Posted at: 2017-02-12T18:19:38.876Z Reads: 76

```
@mrplaygood Found today this nice ''solution''

http://www.banggood.com/1-5S-Lipo-Battery-Voltage-Display-Indicator-Board-p-1073721.html?rmmds=category

You would probably need to modify that button, so you can permantely turn it on / off..
```

---
## \#40 Posted by: Okami Posted at: 2017-05-02T20:18:15.472Z Reads: 66

```
Will add this one to the list:

https://youtu.be/hSCaZBwgpFs

Seems to be quite good, also 3 mode screens..

<img src="/uploads/db1493/original/3X/f/f/fff371e567480e933a9cdef845a3ca366ae5d43b.png" width="388" height="401">

~20usd at banggood..
https://www.banggood.com/ISDT-BC-8S-Battery-Checker-with-Two-85dB-Buzzer-for-LiPo-LiHv-LiFe-LiIon-Batteries-p-1128253.html?rmmds=category

(though for similar price, coulometer could be bought too.. but hey, the screen looks somewhat good and monitors up to 8s battery)

--

One more screen, showing voltage sag:

<img src="/uploads/db1493/original/3X/3/4/34c0eced09224df78aea39c51e91aa747c20a480.png" width="690" height="391">
```

---
