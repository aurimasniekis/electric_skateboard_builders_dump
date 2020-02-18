# Input on my first build? Will it work?

### Replies: 14 Views: 968

## \#1 Posted by: marcus Posted at: 2017-04-30T13:50:31.721Z Reads: 104

```
Hey guys, I am getting into my first build and was wondering what your thoughts were on this setup. i.e. it will not blow up. 

Motor: Turnigy Aerodrive 245kv motor
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html

Battery: (2x) ZIPPY Flightmax 8000mAh 5S1P 30C (Wired in series to make 10s1P) 
https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html

VESC: VESC BLDC by DIY Skateboards 
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

Gearing: 16/36 with mounts and pulleys/wheels/trucks from DIY skateboards

Charger: HOBBYMATE Imax B6 Clone Lipo Battery Balance Charger
(I will be removing each 5s battery and charger individually. I know this will be a bitch but a 10s charger and its setup is too much money/complication for me being a novice.)
https://www.amazon.com/Clone-Battery-Balance-Charger-Adapter-HOBBYMATE/dp/B01NB9A36R/ref=sr_1_9?ie=UTF8&qid=1493559175&sr=8-9&keywords=lipo+balance+charger

Controller: HobbyKing® ™HK-GT2B 3CH 2.4GHz 
https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html

Would love to hear your thoughts!!
 

Marcus
```

---
## \#2 Posted by: KTMinni Posted at: 2017-04-30T13:54:34.886Z Reads: 88

```
The ideal motor kV for 10s is about 180-210 while 245 will work fine this will supply some extra torque for going up hills.  Other than that it seems fine, naturally I recommend liion over lipo but hey a budget is a budget.
```

---
## \#3 Posted by: AbrownMN Posted at: 2017-04-30T14:47:33.827Z Reads: 83

```
I have to agree with KT here..you're already $150 plus charger on that battery setup. Halfway to buying a really nice li-ion pack that is going to guarantee you won't need to upgrade when you get bored with a single motor, and even with a single motor it will make the ride a lot more fun with better range and power. If you can make it work, I'd wait the extra couple of weeks for the next paycheck and save yourself money in the long run by making the build fully worthwhile. Other than that, I'd just advise you to make sure that you're factoring in the cost of all the little stuff. You can easily spend $100-$200 on little shit needed to put it all together. Keep this in mind when your coming up with your overall budget.
```

---
## \#4 Posted by: mmaner Posted at: 2017-04-30T14:47:34.583Z Reads: 82

```
@KTMinni  I'm not sure I understood what you meant there...but 245kv will provide less torque and more top speed that a 190kv for example.

@marcus you might look at the 192kv  turning motors, you will be wasting some of a larger motor as it will exceed the ERPM limit of the VESC so you will need to limit the ERPMs.
```

---
## \#5 Posted by: KTMinni Posted at: 2017-04-30T15:12:03.453Z Reads: 76

```
That's exactly what I meant, I did not mean to cause confusion.
```

---
## \#6 Posted by: Iam319 Posted at: 2017-04-30T15:18:57.439Z Reads: 74

```
If you get a cheap bms for your lipos you can use the 42v hover board charger which is only 11 bucks on eBay.
```

---
## \#7 Posted by: marcus Posted at: 2017-04-30T17:16:09.299Z Reads: 60

```
Thanks for the input, so perhaps the Turnigy 213kv might be a bit better? I understand the correlation between kv and torque/top speed. however the rides I will be taking will not include many hills and am more concerned with speed than bombing up hills.
```

---
## \#8 Posted by: KTMinni Posted at: 2017-04-30T19:28:25.944Z Reads: 52

```
Yes, just understand that you will be sacrificial some torque.

Edit: this includes torque at startup
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-01T05:44:02.599Z Reads: 41

```
204kv with 10s would put you right at the ERPM limit of 60k
190kv eskate motors are very common and will provide a good balance between torque and speed.
```

---
## \#10 Posted by: marcus Posted at: 2017-05-01T09:56:58.838Z Reads: 43

```
I really appreciate the input guys. Did not think of the erpm limit, went tith te 192kv Turnigy!
```

---
## \#11 Posted by: JULMTL Posted at: 2018-03-21T18:11:39.704Z Reads: 32

```
Hi guys,
 I am a  diy noob and working on my first build!
Looking to use the same Lipo batteries on a 10s configuration with diyelectric 190kv 6374 motor. I am hopping to get a top speed around 25mph and a range of at leat 10 miles. I am 170 lbs. Do you think this would suit my needs?

My other batterry option would be diyeboards.com 10s3p pack with 36v, 6.6Ah, 238Wh. 18650LG Lithium Battery. would this be a better option? at 148$ they seem really cheep compared to other sites 10s30 packs.

Thanks!
```

---
## \#12 Posted by: RedEagle Posted at: 2018-03-21T19:36:05.510Z Reads: 30

```
When calculating range take 10wh/km as a general rule of thumb. So the lipo pack should give you around 28.8km and the lion 23km.

If you're comfy handling lipos I'd go for it. If not, then lion.

You can calculate if it suits your needs here:
[calc.esk8.today](http://calc.esk8.today)
```

---
## \#13 Posted by: JULMTL Posted at: 2018-03-21T23:18:40.459Z Reads: 29

```
Also im wondering if I would need a BMS with the Li-on pack and the lipo. From what I understand I can use the lipos without a BMS if I balance charge then, but do I need a BMS for the li-ons? really trying to keep this build simple without any soldering!
Thanks
```

---
## \#14 Posted by: RedEagle Posted at: 2018-03-22T14:52:21.127Z Reads: 23

```
Bms is required for lions. Highly recommended for lipo's. You can charge them without a bms, only do this if you know what you're doing.
```

---
