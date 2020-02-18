# Hobbyking Turnigy Vesc

### Replies: 67 Views: 9058

## \#1 Posted by: rolexbene Posted at: 2017-09-04T19:09:29.399Z Reads: 577

```
After the Hobbyking Vesc got taken offline  a while ago, it seems to be back but rebranded as an ESC (apart from the url lol).

Has anyone had a chance to try one of these yet, would be good to see a review. They claim - Bootloader and Firmware Loaded. With Motor Detection & FOC Tested.

What do people think, possible?

https://hobbyking.com/en_us/vesc.html
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-09-04T19:45:22.614Z Reads: 531

```
nah with no direct fet, think it's ganna be a good cooker. why do they hook it up with 125kv motor otherwise. obviously it lacks motor amp in foc.
probably better than Maycrappy vesc tho
```

---
## \#3 Posted by: marsrover001 Posted at: 2017-09-04T19:46:53.274Z Reads: 524

```
Hope it's possible. Definitely bringing down the cost of one of the most valuable components. On one hand that's great, on the other, what corners did they cut?

Compared to the average 100a RC car ESC going for $40. The extra $30 for regen brakes, custom throttle curves, higher than 4s batteries. If it works, it should be a very popular product for DIY builders. I'd order one now if I wasn't broke from my other hobbies.

As for the suggested combined motor, I doubt much thought was put into that, hope no one accidentally buys one.
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-09-04T19:58:03.546Z Reads: 490

```
focbox 4 ex factory price is around $50 plus from china. obviously they need make margin so that's probably 100 percent margin when everything considered. (Austin dollar is cheeper) given that this would factory cost about under 30. Just speculation but shouldn't expect too much from
```

---
## \#5 Posted by: rolexbene Posted at: 2017-09-05T12:59:48.748Z Reads: 475

```
They have also uploaded a 'manual'. Does this give anyone any insight on the quality of them? I there any way of telling if these are missing or have low quality components?

Also does anyone have any expirence with Hobbykings return policy, they state they run FOC so if and when they blow could we just return them under there 1 year warranty?

 https://docs.google.com/viewer?url=https%3A%2F%2Fhobbyking.com%2Fmedia%2Ffile%2Ft%2Fg%2Ftgy_vesc_manual_pv.pdf
```

---
## \#6 Posted by: danielz Posted at: 2017-09-06T23:54:42.579Z Reads: 437

```
Received one yesterday, here are 6 images in case they are any good to anyone. I expect it to fail like so many do due to the VESCs poor design. When it does ill try the warranty, then just use a regular ESC.

https://imgur.com/a/L5AhQ
```

---
## \#7 Posted by: marsrover001 Posted at: 2017-09-09T01:23:27.883Z Reads: 418

```
Have you tested it at all yet?

For smaller setups it should work without blowing up right?
```

---
## \#8 Posted by: danielz Posted at: 2017-09-09T02:14:14.112Z Reads: 420

```
Will be a week or two unfortunately, the parts are nearly hear, but ive a broken foot lol.

Ill be running 12s2p 5000mah 30c, 6374 192KV, 6:1, 200mm wheels, im 65KG.

Ill limit to 60,000 erpm
Wont use foc mode
Upgrade filter caps to 100v low esr
Small wire as possible from battery to ESC ( 3 inch)
Cable tie the leads together
Active cooling with a fan, maybe heatsinks, however i dont think its very effective on the wrong sides of the mosfets.

If it still fails, there is no hope for thr turnigy vesc lol. Ill update the post asap.
```

---
## \#9 Posted by: hobbyking_ian Posted at: 2017-09-09T03:10:03.903Z Reads: 411

```
Hi There Guys, 

Just thought I would pop in and say hello. Any issues or suggestions I'd be happy to hear them so feel free to PM me

ian
```

---
## \#10 Posted by: marsrover001 Posted at: 2017-09-09T03:36:06.100Z Reads: 402

```
Same, was planning a 12s1p (budget restrictions) build.

How does disabling FOC help the ESC last longer? (I get how erpm would help though) And any cooling is better than no cooling, must help somehow.
```

---
## \#11 Posted by: danielz Posted at: 2017-09-09T04:23:53.753Z Reads: 395

```
Just from research. Ive read so many post of the drv8302 burning up when users tested foc mode, apparently if you upgrade the c26(I think) capacitor it lessens the probability of damaging the drv8302 in foc mode. Im just staying away from it to be safe. Im too poor to keep replacing Vescs lol

Here an interesting post
http://vedder.se/forums/viewtopic.php?f=7&t=145&start=30
```

---
## \#12 Posted by: Cobber Posted at: 2017-09-09T04:29:03.386Z Reads: 391

```
Hi @hobbyking_ian
welcome dude... :grin:

you might get more than you bargained for here though :joy:
GL ;)

are you fielding general questions about any HK products?
```

---
## \#13 Posted by: Wilsonliang777 Posted at: 2017-09-09T04:46:27.798Z Reads: 382

```
I am in the market for a vesc but too poor to spend $150 to $200 for a vesc.   I would like to see how this esc perform.
```

---
## \#14 Posted by: Fiori Posted at: 2017-09-09T05:05:31.598Z Reads: 378

```
"Hardware version 4.10" That's even older than maytech
```

---
## \#15 Posted by: danielz Posted at: 2017-09-09T06:24:31.973Z Reads: 377

```
Yep i can confirm its 4.10.

4.11 just added a thicker trace.
4.12 added an extra capacitor c18, this was again for resolve another foc issue. you could modify this yourself.
```

---
## \#16 Posted by: hobbyking_ian Posted at: 2017-09-09T11:15:36.830Z Reads: 363

```
Hey Cobber, 

I'll try and answer questions however my key responsibilities are Trains, ESC, Motors, Planes, 

Ian
```

---
## \#17 Posted by: Cobber Posted at: 2017-09-09T13:13:18.349Z Reads: 367

```
between motors and speed controllers I'm sure there will be plenty of people interested in what you have to say :slight_smile:
won't be long before people will be dropping your name in posts...
shame you don't do batteries as well ;)
```

---
## \#18 Posted by: darkkevind Posted at: 2017-09-09T19:47:11.617Z Reads: 367

```
I have a question: Why are your VESCs really old hardware? You're not supporting FOC?
```

---
## \#19 Posted by: hobbyking_ian Posted at: 2017-09-10T00:40:52.086Z Reads: 360

```
I used to look after the battery category so I can talk to that as well.
```

---
## \#20 Posted by: hobbyking_ian Posted at: 2017-09-10T00:44:43.488Z Reads: 363

```
I inherited this project but I can build anything you like. I'm here to learn a bit more about what the community is after and how we can facilitate. Have you got a link to the project you referenced?
```

---
## \#21 Posted by: Cobber Posted at: 2017-09-10T00:50:45.385Z Reads: 351

```
I'm not a vesc guy @hobbyking_ian I'm on _rc_ speed controllers, but from what I have read the firmware you have on the vedder designed esc's you have atm is a older version that needs to be updated before use...

I'm sure one of the vesc :nerd: will chime in any moment :)
```

---
## \#22 Posted by: darkkevind Posted at: 2017-09-10T07:41:53.130Z Reads: 349

```
The fact that you don't know what I'm referring to doesn't bode well for results on this matter, but you sell a version of the VESC under the guise of a 50A skateboard ESC.

https://hobbyking.com/en_us/turnigy-skateboard-esc.html

The hardware version is pretty ancient, the latest iteration in that form factor is at version 4.12 with updated and uprated components to cope with FOC.

To be a worth while purchase, I'd suggest you update the hardware to that at least for the time being anyway, but then work to improve things (if you're saying you build these things) to bring it up to FOC-Box standards/specifications. If you do this at a reasonable price, you'd sell loads!

We're here to help you improve your products...
```

---
## \#23 Posted by: bigben Posted at: 2017-09-10T07:48:31.799Z Reads: 330

```
In my opinion the community would really like is a well made, reliable, nicely priced version of the vesc that is available off the shelf all over the world. Also made by a supplier who gives back directly to Benjamin Vedder.
```

---
## \#24 Posted by: Cobber Posted at: 2017-09-10T08:20:38.733Z Reads: 334

```
I agree @bigben, and I think @hobbyking_ian is here on his own accord wanting to help and asking what needs to be done to improve HK service/products, I'm sure he doesn't make all the decisions. This is a real opportunity to be productive and work with someone on the inside. Sometimes I wonder how people actually talk to people in the real world?

[quote="darkkevind, post:22, topic:32260"]
The fact that you don't know what I'm referring to doesn't bode well for results on this matter, but you sell a version of the VESC under the guise of a 50A skateboard ESC.
[/quote]
_this doesn't really help does it?_

Personally I think trying to upgrade the old VESC4.xx design too much is a bad business decision over the medium to long term, energy could be spent else where. It is a old design and will only be used for budget builds going forward, get the most out with the least effort. Maybe limit voltage, Field Orientated Control (provides quiet operation & smooth start up) and it would be better to pursue BV's new design the VESC6 that does it all...

but hey what do I know :smirk:
```

---
## \#25 Posted by: darkkevind Posted at: 2017-09-10T08:38:40.473Z Reads: 318

```
What I suggested was a quick and cheap win in the short term whilst better solutions are worked on for the longer term...

In business, it's an idea to have a product that's bringing in the cash, a 'cash cow' that might not be the best product you can produce, but you can make some decent money with it, that can then fund r&d to either make a better version of that product or towards developing a new product...

Like I said, of they even just bright it up to 4.12 spec at a HK price point, they'd seek like hot cakes...
```

---
## \#26 Posted by: Cobber Posted at: 2017-09-10T08:46:30.851Z Reads: 316

```
So what is 4.12 spec bro?
what needs to be done?
& what is the outcome or benefit to what they have now?
```

---
## \#27 Posted by: darkkevind Posted at: 2017-09-10T09:02:40.628Z Reads: 314

```
Some components need to be upgraded as stated previously and that's been covered loads of time before on this forum...
```

---
## \#28 Posted by: c4Lvin Posted at: 2017-09-14T06:56:38.355Z Reads: 308

```
Not everybody runs FOC. If you enjoy tinkering and risk blowing it up go ahead but dont blame HK and the other makers of the Vescs for not being up to date on certain parts. Don't expect to buy an iphone X for the price of an iphone 7. Ive been running 4.10 enertion with 190kv for over a year now. Only blown drv i got was due to the motor wires touching/shorting out without me knowing.
```

---
## \#29 Posted by: bigben Posted at: 2017-09-14T07:00:28.571Z Reads: 305

```
@hobbyking_ian one thing you guys could look at is putting a 3mm keyway on your current range of 63mm motors. If you were to use silicone phase wires too I think you would be on to a winner.
```

---
## \#30 Posted by: Cobber Posted at: 2017-09-14T09:16:43.927Z Reads: 305

```
strand count on motor wires is low, so they will never be _flexy_, I'd rather see fixed posts I could attach flexible wire to...
as for a keyway, it just weakens the bond of my loctite ;)
```

---
## \#31 Posted by: danielz Posted at: 2017-09-22T20:05:09.576Z Reads: 294

```
Well it passed test one. Hasn't instantly fried after 30 mins on the bench. Its 12s. Added extra 100v 680uf caps, heatsinks and cable tied all wires together. Its firmware updated fine using vesc tool. Ill update after first ride in a few days.

https://youtu.be/cvlZ9JBVgys
```

---
## \#32 Posted by: Jinra Posted at: 2017-09-23T00:08:01.414Z Reads: 293

```
100v cap? is that safe?
```

---
## \#33 Posted by: SilentException Posted at: 2017-09-23T00:15:00.078Z Reads: 295

```
Why not? Capacitor voltage rating is just it's maximum. It does not mean it will store and discharge 100V.
```

---
## \#34 Posted by: scepterr Posted at: 2017-09-23T00:22:48.613Z Reads: 282

```
Completely safe, you'll get more life out of them not running near max voltage and harder to damage with V spikes. A few of the smd cap upgrades bump them from 50V to 100V
```

---
## \#35 Posted by: Jinra Posted at: 2017-09-23T00:32:36.518Z Reads: 283

```
Just wondering :) only ask because the default electrolytic caps are 63v
```

---
## \#36 Posted by: SilentException Posted at: 2017-09-23T00:43:51.949Z Reads: 289

```
Yeah it is alright to have some breathing room, not dangerous :)
```

---
## \#37 Posted by: danielz Posted at: 2017-09-29T20:44:30.498Z Reads: 283

```
Still all good so far. First ride, 30 minutes of riding.

12s 2p 5000mah 30c
1 x 6374 192kv
5:1 gear ratio. 8 inch wheels

Latest firmware
60,000 limit

Mods
Removed Heatshrink
Added 2 x 100v panasonic low esr caps
2 heatsinks
Fully enclosed with 50mm fan cooling everything (powered with a 12v buck).

I cant believe how powerful just a single motor is. I still plan to move to two motors for reliability and to stress the vesc. less. I need to add hall sensors too i think.
```

---
## \#38 Posted by: scepterr Posted at: 2017-09-29T20:47:07.771Z Reads: 281

```
If you find somebody selling the internal hall PCB let me know, I can't find them. APS has them...but out of stock
```

---
## \#39 Posted by: pat.speed Posted at: 2017-09-29T22:55:56.006Z Reads: 281

```
 
@scepterr Yes same problem here. I would get from aps but shipping to Aus is nearly 3x the price of the actual pcb. Let me know too please @danielz
```

---
## \#40 Posted by: danielz Posted at: 2017-09-29T23:01:24.304Z Reads: 278

```
iIl be using external sensors (I think) as my motor is inside an enclosure anyway.
```

---
## \#41 Posted by: pat.speed Posted at: 2017-09-29T23:15:58.984Z Reads: 268

```
Ok. Are you going to make them yourself or buy them?
```

---
## \#42 Posted by: ryan_pogi Posted at: 2017-11-12T02:47:06.461Z Reads: 248

```
Hey @danielz, any update on your Turnigy VESC?
Planning to use the same one.
Also planning to do the same mods as you did.
Can you (or anyone) show where to put (or replace) the 2x 100v low esr capacitors?
Thanks.
```

---
## \#43 Posted by: danielz Posted at: 2017-11-12T03:37:26.958Z Reads: 247

```
Ive done about 80 miles now, no problems, and its on  a mountain board with a single motor too, so quiet highly stressed. Ive now bought a second, haven't fitted it yet though.

You can fit the caps anywhere you like. I put one on the short wires between mainboard and the caps pcb. The other is attached to the solder pads on the caps pcb. So i have 5 in total. Mines all secured down nicely so nothing breaks off.
```

---
## \#44 Posted by: ryan_pogi Posted at: 2017-11-12T03:44:38.855Z Reads: 246

```
So it's durable. Torture tested. That's some good news.  That's why I wanna copy yours :smile: 
Can you post some photos or videos how you do it?  If it's not too much trouble.
Thanks.
```

---
## \#45 Posted by: danielz Posted at: 2017-11-12T04:22:37.004Z Reads: 249

```
Mine currently in pieces as im fitting sensors to the motor, but here it is in a mess.

<img src="/uploads/db1493/original/3X/8/4/84e734918077bab66ceb2c98d1b147897aca16ca.JPG" width="375" height="499">
```

---
## \#46 Posted by: chrisongtj Posted at: 2017-11-12T10:07:04.190Z Reads: 244

```
I have two of these in my dual belt drive. I'm running dual 5045 from racestar (banggood). Amp limit set at 40 as I'm running 10s2p.

So far it's working really well. No heat sink  added yet and to be fair, the esc doesn't heat up that much after riding. I'm running it in BLDC but I have a friend running FOC and both have been working great.I've run around 50k on them so far 

I would happily buy a newer vescs if pricing and availability was better. Too bad shipping to my country is at least $30-50 from many retailers if it's even in stock. HK can ship my order to me in 2 to 3 days, sometimes I can get it even before I have time to go to the local hobby store.
```

---
## \#47 Posted by: danielz Posted at: 2017-11-12T12:35:18.314Z Reads: 244

```
In response to pats earlier question. 3d printed some.

Just completed it and omg! What a difference, when non sensored i can hold the motor with my hand at low rpm and it stalls or moves back and forth. Sensored it just pulls and pulls.Very happy.

Honeywell ss411a
17.14 degrees

<img src="/uploads/db1493/original/3X/8/4/8425175fb7fb7baba26b184275ce6804f4a7fa17.JPG" width="375" height="500">
```

---
## \#48 Posted by: Acido Posted at: 2017-11-12T12:56:31.117Z Reads: 238

```
Bulk order of 2000 pieces maybe
```

---
## \#49 Posted by: Okami Posted at: 2017-11-12T14:50:00.533Z Reads: 236

```
Can u give more info on how u made your sensors? Looks somewhat easy to do.. at least better than making custom pcb or opening the motor and then gluing.halls
```

---
## \#50 Posted by: danielz Posted at: 2017-11-12T15:26:08.719Z Reads: 236

```
Ill make a small tutorial tonight.
```

---
## \#51 Posted by: danielz Posted at: 2017-11-13T14:14:10.606Z Reads: 231

```
Here you go.

https://www.instructables.com/id/How-to-Add-External-Hall-Sensors-to-a-Turnigy-SK3-/
```

---
## \#52 Posted by: notepad Posted at: 2017-11-13T14:36:28.960Z Reads: 225

```
Great read.  Very easy to see the differense.   in that last video though it looked like your mount was bending quite a lot though so Id be careful on that!

Time to do some reading and see if this mod can work of FOC aswell.
```

---
## \#53 Posted by: danielz Posted at: 2017-11-13T14:47:13.979Z Reads: 215

```
It bends a bit, the torque from the single motor makes it steer too left too, prototype mount until ive settled on a design. Second motor is here tomorrow.
```

---
## \#54 Posted by: ryan_pogi Posted at: 2017-11-13T17:12:14.417Z Reads: 210

```
Adding capacitor(s) to this particular VESC, is it best to use 680uf?
```

---
## \#55 Posted by: danielz Posted at: 2017-11-13T17:25:48.098Z Reads: 212

```
You can use more or less. The longer your battery wires the more Capacitance needed. Mine are actually very short and tied together. So the stock amount would have sufficed, The only reason I added more was a) Im running 12s b) I cant verify the quality of the current caps. If you are running less voltage, you can save yourself some space and not use 100v caps.

Im forever repairing other devices because the caps have blown. So im airing on the side of caution by adding two extra high quality, high voltage low esr caps.
```

---
## \#56 Posted by: yaca Posted at: 2017-11-13T18:26:15.825Z Reads: 208

```
Thank you for your tutorial about hall sensors even it came to late for me, because I already built in hall sensors in my hub motors. What I read from your tutorial I choosed the right hall sensors: Honeywell SS460P High Sensitivity Latching Hall-Effect sensor (Bipolar latching magnetics).

https://www.tme.eu/at/details/ss460p/hall-sensoren/honeywell/
```

---
## \#57 Posted by: telnoi Posted at: 2017-11-13T18:35:03.818Z Reads: 213

```
Thanks for the tutorial. Ordered the hall sensors.
Not sure if I've missed it, but which side of the sensor is pointed towards the motor? Does that even make a difference?
Judging by your wiring diagram, you have the signal wire on the left and +5V on the right, meaning you have the widest part of the sensor rotated towards the motor.

<img src="/uploads/db1493/original/3X/2/0/207f4d63f401f2a641421ea05e6231ba03984e2b.png" width="531" height="499">
```

---
## \#58 Posted by: danielz Posted at: 2017-11-13T18:56:09.650Z Reads: 211

```
If you are using the same as mine, the narrow side faces the motor. If its another model best to double check the datasheet they all have. Updated the instructable.
```

---
## \#59 Posted by: telnoi Posted at: 2017-11-13T19:01:48.558Z Reads: 213

```
Is your wiring diagram incorrect then or the image I attached? You have vcc on the right, where as the pic I posted would have it on the left.

Supposedly, the image I shared is the Honeywell sensor. Just making sure.
```

---
## \#60 Posted by: danielz Posted at: 2017-11-13T19:15:32.779Z Reads: 212

```
Nope they are both the same as the above image. Ive updated my wiring diagram so you can see the hall profile.
```

---
## \#61 Posted by: danielz Posted at: 2018-04-04T15:19:49.766Z Reads: 167

```
Update: One failed around 2 months ago. It probably had only 100-200 miles on it. Hobbyking customer service was good and they did refund quickly, there was no stock for a replacement.

The second of two i bought was the one that failed. It failed randomly one day when braking from about 10mph to 0. I cant see any physically damage at all. It refused to even connect via usb though.

Im probably going to make 2 escape bbox vescs soon.
```

---
## \#62 Posted by: Blitz Posted at: 2018-04-04T16:24:41.721Z Reads: 159

```
Hobbyking has good customer service but I only see bad reviews.
When My Imax b6 fake broke they refunded credits and I said I can't ship it out It costs to much the things only worth 15 euro so they let me keep it.
```

---
## \#63 Posted by: danielz Posted at: 2018-04-04T16:44:06.569Z Reads: 159

```
Yeah i still have the broken vesc too.
```

---
## \#64 Posted by: Blitz Posted at: 2018-04-04T16:57:14.612Z Reads: 159

```
I wonder can you fix it? and long would it live after a repair.
```

---
## \#65 Posted by: danielz Posted at: 2018-04-06T16:11:53.163Z Reads: 154

```
yeah im going to try, might as well, ill upgrade some caps and diodes to 100v version whilst im there too.
```

---
## \#66 Posted by: danielz Posted at: 2018-04-21T02:17:25.439Z Reads: 131

```
Updating this thread. Fixed the hk vesc, drv was fine. A fet had stuck closed, and it some how the bootloader and firmware became corrupted too. £5 fet and £5 st link and im back up and running. Very strange. 

Modified it some more, smaller 100v cap is now right on the + and - inputs. Ill shortly be upgrading all 50v ceramic caps to 100v.
```

---
## \#67 Posted by: FalconNL Posted at: 2018-07-25T20:34:23.389Z Reads: 86

```
So is it correct that the Hobbyking Vesc isnt any good without modifications?
```

---
