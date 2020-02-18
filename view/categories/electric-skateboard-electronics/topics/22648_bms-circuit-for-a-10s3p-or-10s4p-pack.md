# Bms circuit for a 10s3p or 10s4p pack?

### Replies: 18 Views: 3238

## \#1 Posted by: Bloop Posted at: 2017-05-08T17:10:49.815Z Reads: 248

```
Hello guys im thinking to buy 40 batteries Samsung INR18650-25R 2500mAh - 20A and im looking for a bms any idea if this one is any good or should i use another ( im in europe so would be nice if i could find something around here)

http://www.batterysupports.com/36v-37v-42v-10s-30a-10x-36v-lithium-ion-lipolymer-battery-bms-p-265.html

Anyone can help me understand how to charge the batteries with this bms ? .. is it posible to use a laptop charger or something like this?? 

Really apreciate.
```

---
## \#2 Posted by: Tobi Posted at: 2017-05-08T17:28:06.278Z Reads: 242

```
If you are going to build a 10s4p with those batteries you need atleast a bms that can handle 80A current, unless you bypass it for charging only which i wouldnt recommend.

might get this one 

http://www.batterysupports.com/36v-37v-42v-10s-80a-10x-36v-lithium-ion-lipolymer-battery-bms-p-389.html

And yes for charging you could use some regular 42 volt charger 

https://www.amazon.com/s/ref=nb_sb_noss_2?url=search-alias%3Daps&field-keywords=42+v+charger

if i were you just take a look around some building threads here in the forum there are plenty of good informations
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-08T20:11:48.884Z Reads: 211

```
The word on the street is that 25R's are not the best choice available now.
30Q's are suppose to be much better.

And as @Tobi stated, you should get a bms with higher amp capability than the one you listed.
The reason is that these bms's are designed to protect the battery during charge and discharge cycles.
And although some people will bypass the discharge protection either to save money or space, it is much better to have the full protection that the bms offers.

And it is a good rule of thumb to always build with supply being greater than demand. Also know as "headroom"
Your battery and bms should be capable of more than what the motor and controller will need.
```

---
## \#4 Posted by: markyoe Posted at: 2017-05-08T20:29:16.697Z Reads: 188

```
[quote="Bloop, post:1, topic:22648"]
40 batteries Samsung INR18650-25R 2500mAh - 20A
[/quote]

Not trying to hijack the thread, but maybe the answer to this question would be helpful to @bloop too. Can that BMS do regenerative braking if the VESC is set up to do it?
```

---
## \#5 Posted by: OskarCastrone Posted at: 2017-05-08T20:42:59.794Z Reads: 180

```
I have a shipment of BMS units on the way from Bestech. All the units is with a built in e-switch, so you do not have to buy an additional power switch. The BMS units will have eother 60a (for Samsung 25r or similar in 10s3p config) discharge or 80a (for Samsung 25r or similar in 10s4p config).

The Samsung 25r cells is pretty cheap on nkon.nl (the go to battery webshop in EU). They are so cheap that I would not even consider choosing other cells because they are about double the price! 
I have been using the 25r's a lot, I am very happy with them. Sure, you can get something that perfoms better, but I dont think that you get more value for money than with the 25r cells.
```

---
## \#6 Posted by: eitan Posted at: 2017-05-08T22:40:24.348Z Reads: 169

```
@OskarCastrone Are you selling the Bestech BMS's?
```

---
## \#7 Posted by: Bloop Posted at: 2017-05-09T06:03:17.894Z Reads: 168

```
I understant now and now i see ... i did not consider i need to use that for discharge too (but i dont want to bypass) so ill look for something with more amps.

As @markyoe asked (and i suppose is possible but i want to make sure) with the BMS on is posible to have regenerative breaking ? 

And now back to the batteries.. i found the 30q but they offer a little less amps than 25R but for price they are really similar so i dont know right now. With the 25R i would have 80A discharge while with 30Q would be only 60A. now im not sure how many Ams do my motor need. I have the one form enertion tho.

Anyone could help with that? which one is better and worth buying?

Thank you everyone for your answers.
```

---
## \#8 Posted by: markyoe Posted at: 2017-05-09T06:07:03.122Z Reads: 158

```
I got 40 of these after I saw someone on here use them :grin:: https://www.imrbatteries.com/lg-he2-18650-2500mah-20a-flat-top-battery/
What do you other guys think of that battery? Obviously it's a little late to change for me, but maybe it'll be helpful for @Bloop
```

---
## \#9 Posted by: L3chef Posted at: 2017-05-09T06:29:52.166Z Reads: 152

```
 is 60amp bms for a 10s4p pack enough or do I really need 80?
Just bought an 60 amp from ebay so..
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-09T06:31:23.337Z Reads: 149

```
60 is good enough, you'll like never pull that much, plus the BMS supports burst currents higher than 60A
```

---
## \#11 Posted by: L3chef Posted at: 2017-05-09T06:45:15.600Z Reads: 142

```
Jinra you are everywhere here on this forum :smile: 
Thank you again!
```

---
## \#12 Posted by: OskarCastrone Posted at: 2017-05-09T08:25:48.557Z Reads: 144

```
From nkon.nl these batteries is very good for the price! I just ordered a bu ch of them too. 
As I remember, the Samsung 25r has a slighty better discharge curve - but hey! It is a great deal!
```

---
## \#13 Posted by: OskarCastrone Posted at: 2017-05-09T08:26:58.143Z Reads: 148

```
Yes. I will be selling 80a and 60a BMS units (including build in e-switch) from Bestech. They will arrive at my door by the end of this month.
```

---
## \#14 Posted by: Bloop Posted at: 2017-05-10T06:40:27.978Z Reads: 140

```
So how do you use the BMS with regen breaks from vesc ?
```

---
## \#15 Posted by: Bloop Posted at: 2017-05-10T07:36:54.639Z Reads: 138

```
Ok so i did some math and 

For my 10s3p i will have 42V max with my motor that has 2400W ill need max 60A for a BMS.

Now between 
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
and 
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

Wich one would be better and why ? Also how do i connect them ? the one from batterysupports i saw it has 3 pads P N and B but for bestechpower i couldnt find any instructions ? 

Any help here ?
Thank you
```

---
## \#16 Posted by: Bloop Posted at: 2017-05-11T05:58:41.633Z Reads: 129

```
I found a charger for li-ion batteries with 42V and 2A is that good for charging my pack ?? Also what should i have in mind when i get a charger ? 

What other chargers are good for a 10s4p batery pack of li-ion ?? 

Thank you
```

---
## \#17 Posted by: SpeedyGornzallez Posted at: 2019-02-04T16:34:25.838Z Reads: 41

```
A dumb question but I’m guessing the 42v charger charges up to 42v, same for 36v charged up to 36v etc??
```

---
## \#18 Posted by: Andy87 Posted at: 2019-02-04T16:40:25.063Z Reads: 39

```
It depends on the label of your charger.
36v is the nominal voltage of a 10s pack which would be 42v.
You can look for 10s charger which charge till 42v but labeled for 36v
```

---
