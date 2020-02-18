# DRV8302 Error? I need help!

### Replies: 42 Views: 2832

## \#1 Posted by: aigenic Posted at: 2017-05-13T18:58:41.243Z Reads: 170

```
Hi,
Today I have connected my Maytech VESC and I couldnt get it to work...the BLDC tool says DRV8302 Error :frowning:

I am 100% sure there have been no shorts/sparks or anything like that, before the error occured I had embedded my motor leads into the deck (LHB style) with polyester resin and I might have switched them. I also resoldered two leads to the sensors of the motor. That are the changes I made before reconnecting the VESC.

Before the VESC had been running smoothly and I have never had any issue...

Here are pictrues of the VESC
<img src="/uploads/db1493/original/3X/b/a/baca4e2644fe1a49bd4f91e014957dbb1677c8ca.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/a/1a2cea42b7986ed4d96823259f43e4181bd87172.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/2/12ca3437bb573e92f6e5bdebe037474ea92461c2.JPG" width="666" height="500">

and pics of the BLDC tool:
<img src="/uploads/db1493/original/3X/a/7/a7547b2816fefe0be821e60ba80a529625795d55.JPG" width="690" height="343"><img src="/uploads/db1493/original/3X/e/1/e158ae6632dfd969ede77c7c44bf9b279513e4e2.JPG" width="690" height="398">
```

---
## \#2 Posted by: aigenic Posted at: 2017-05-13T19:04:18.879Z Reads: 158

```
What is the problem with the VESC? May it be manufacturing mistake? Would changing the DRV chip help?
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-13T21:11:06.270Z Reads: 156

```
Battery Max is a bit high, also you should leave your min/max voltage alone (8/57 default). Some of these settings may have blown the DRV. You'll need to swap it out or get a new VESC. SMD soldering the chip is a bit difficult though. You may want to consult @JohnnyMeduse for a swap.
```

---
## \#4 Posted by: aigenic Posted at: 2017-05-13T21:17:08.278Z Reads: 154

```
Ok...few more questions from me :slight_smile:
My friend studies electrotrchnics so he could repair it cheaply for me :) Is there something importnant he should know? 
I have to exchange just the DRV? 
Where can I buy DRV in EUrope? I know I can buy from aliexpress, but are there any european vendors where I could get it faster than 19 days?

Ty @jinra
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-13T21:19:19.933Z Reads: 147

```
No idea about any european vendors, but people typically order off mouser in the States I believe. Just make sure to show your friend Vedder's schematic from his site. There are two pairs of leads that need to be bridged on the chip.
```

---
## \#6 Posted by: aigenic Posted at: 2017-05-13T21:20:39.233Z Reads: 139

```
OKok :) ty
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-05-13T21:50:02.258Z Reads: 141

```
Hi @aigenic, as @Jinra mention always leave min max voltage to the original limits. 

Also, It's look like the integrator limit are the default one, those should have change after your motor detection, maybe you did push the write button after the motor detection, witch could lead to a drv faults

<img src="/uploads/db1493/original/3X/8/f/8fc1cc0cfa12d24cd2f69098b8756bf5b243aac8.JPG" width="690" height="398">

You best choice to get the part fast is probably MOUSER.
```

---
## \#8 Posted by: aigenic Posted at: 2017-05-14T07:00:40.606Z Reads: 125

```
Ok, I have done some research...can i buy hits DRV? Is this the right one? 
http://uk.farnell.com/texas-instruments/drv8302dca/motor-predriver-3ph-56htssop/dp/2078553?CMP=GRHB-OCTOPART
```

---
## \#9 Posted by: okp Posted at: 2017-05-14T07:07:49.064Z Reads: 121

```
hey, just go with mouser. I changed two DRV yesterday that I burnt and to be honest I thought it would be more difficult. It's really accessible if you have an hot air station and patience.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-05-14T15:02:00.098Z Reads: 114

```
Don't really care about the different Name for the DRV8302, they are packaging types identification.
```

---
## \#11 Posted by: aigenic Posted at: 2017-05-14T17:04:54.761Z Reads: 108

```
How much grades does the hot gun need to be able to output?
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-05-14T17:06:08.841Z Reads: 110

```
around 240 celsius
```

---
## \#13 Posted by: OskarCastrone Posted at: 2017-05-14T18:10:55.415Z Reads: 105

```
I am in the same boat! Although this is happening to 2 of my VESCs which have never been used before..... 
are you @JohnnyMeduse still soing repairs in Europe?
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-05-14T18:14:22.926Z Reads: 107

```
I can do repair from Europe, but the shipping cost a little bit higher, and also the delay (because of longer shipping time)....
```

---
## \#15 Posted by: aigenic Posted at: 2017-05-22T07:50:48.313Z Reads: 98

```
Ok, my friend is not able to change it...he just took away the old DRV and damaged my VES a little...he said he had put everything back in right order and tested everything so it should work, but it doesnt look well :/
```

---
## \#16 Posted by: aigenic Posted at: 2017-05-22T08:00:02.539Z Reads: 102

```
Here are photos of the VESC after removing of the DRV...
<img src="/uploads/db1493/original/3X/6/6/66345a37bf64002663f80ed2d1e59bbbe6bf9a37.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/d/ad2d2dbfe6950be78c8bf2aeb6ff6dc4c6462543.JPG" width="666" height="500">

Is it still usable, if the DRV would be replaced or do I have to buy new one?
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-05-22T11:26:07.540Z Reads: 105

```
C41, C23, C10, C39 and probably more components are destroyed or out of place.
I´d get a new one. Too much hussle
```

---
## \#18 Posted by: aigenic Posted at: 2017-07-14T11:42:35.038Z Reads: 87

```
Am I cursed or what?! 
So I have bought a new VESC from goaxle.com...after some time it was dispatched and then the parcel got lost...However I got my money back from axle (really nice customer support :O )
So I orerd from Vandaelectronics.com...the VESC was dispatched this monday and it was delivered yesterday....today I checked all the fucking cables, everything is well isolated...and guess what...I connected it and the DRV blew up!!! FUCK THIS
```

---
## \#19 Posted by: aigenic Posted at: 2017-07-14T12:01:27.614Z Reads: 85

```
 I just tooka apart my connectors which were inside the deck...they are ok...the only problem might be in the motor...
```

---
## \#20 Posted by: TranxFu Posted at: 2017-07-14T12:05:10.590Z Reads: 83

```
Check your motor resistance ?  Maybe it has a short somewhere. unplug it and try turning it and then hold 2 phase wires together and turn it again. There should be a increase in resistance. 

Also you could check your ramp step setting in the bldc tool. Older bldc_tool versions had an issue there.
```

---
## \#21 Posted by: aigenic Posted at: 2017-07-14T12:09:05.133Z Reads: 78

```
yeah, there is an increase...I have 6A in detect parameters...
```

---
## \#22 Posted by: TranxFu Posted at: 2017-07-14T12:11:39.314Z Reads: 76

```
Does this apply ?

https://www.electric-skateboard.builders/t/psa-remember-to-reset-your-max-current-ramp-step-when-programming-your-vesc/6262
```

---
## \#23 Posted by: aigenic Posted at: 2017-07-14T12:18:30.479Z Reads: 72

```
yes, tehre is 0,04 and not 0,004 :( Did this caused the problem and DRV failure? I guess I will have to have DRV changed...
```

---
## \#24 Posted by: TranxFu Posted at: 2017-07-14T12:19:55.062Z Reads: 72

```
probably :/ ... next time try to use the latest firmware for bldc and vesc. Hope you'll get back on the road soon ! :+1: This is all part of DIY-Life :wink:
```

---
## \#25 Posted by: aigenic Posted at: 2017-07-14T12:21:03.028Z Reads: 72

```
Yeah...i know...but its kinda weird that it worked with MayTech VESC once and then it destroyed the DRV...
```

---
## \#26 Posted by: Jinra Posted at: 2017-07-14T14:33:12.222Z Reads: 68

```
.04 is the correct value you should be fine for that
```

---
## \#27 Posted by: aigenic Posted at: 2017-07-14T14:58:38.809Z Reads: 63

```
So what could have caused the dead DRV? Motor is OK, also connector and cables...
```

---
## \#28 Posted by: Jinra Posted at: 2017-07-14T15:10:38.187Z Reads: 62

```
[quote="aigenic, post:1, topic:22978"]
I also resoldered two leads to the sensors of the motor.
[/quote]

Just curious, you say you resoldered the sensor leads, but you're using sensorless right?
```

---
## \#29 Posted by: aigenic Posted at: 2017-07-14T15:14:36.176Z Reads: 61

```
when the MayTech VFESC failed, it was in sensored, the Vanda VESC was unsensored without sensore wires connected
```

---
## \#30 Posted by: aigenic Posted at: 2017-07-14T15:14:57.847Z Reads: 60

```
It failed during motor detection
```

---
## \#31 Posted by: Jinra Posted at: 2017-07-14T15:16:44.110Z Reads: 61

```
Your Maytech (OP) screenshots say sensorless. Anyway, you're now saying your Vanda VESC DRV blew up during detection and now fails detection? Could you post pics on how you have everything hooked up, and what kind of battery you have?
```

---
## \#32 Posted by: aigenic Posted at: 2017-07-14T15:19:39.909Z Reads: 63

```
ok I might have had it in sensorless when it failed, i dont remember correctly...
I will post the pics later (in 2 hours), I have to leave now...
```

---
## \#33 Posted by: aigenic Posted at: 2017-07-15T18:27:04.167Z Reads: 63

```
About the pics...I am sure everything is hooke up correctly, I took everything apart yesterday and removed all insulating tape from the connectors, when I was looking for the mistake...I dont think the photos of the board, cables and connectors would help. but I can send them :)

Before I my first blown DRV I had hidden cables inside the deck and I had sunk them with polyester resin to hol on place...from what I know Polyester resin is not conductive and also the cables were isolated...I had been using the cables with same isolation before and they were OK, so the reason of the failure might be only the resin, but since they are well isolated there shouldnt be a problem?

COuld it be caused by too long phase motor wires? They are about 20cms long, but as I said I used them without any issue before...

Also 3 of my bullet connectors under the truck are connected to the wires in angle/from the side so they can fit under the truck...Could this cause the problem?

I have 10s LiPo 5000mAh 20C
```

---
## \#34 Posted by: aigenic Posted at: 2017-08-15T19:55:42.147Z Reads: 50

```
Ok...im angry...why the fuck me? 
3rd time, all new wires and connectors, everything seems ok, everything well isolated (2 layers of isolation)...i connected VESC to batteries and it gets hot and starts smelling like somthing is being burned...IDK what is wrong, the heat comes fsomewhere from the drv or maybe the coil next to it i am not sure...just constantly flashing red light...i didnt even hit connect in BLDC tool...

I think I giv up on this shit...I have spend too muc hmoney on these VESCs, IDK what i am doing wrong because i always follow guides and there is always something wrong...........

So I was wondering I could buy a normal HV ESC, what ESC do you recommend? 
[This one from APS?](http://alienpowersystem.com/shop/esc/alien-120a-3-12s-jet-esc-hv/) Is it reliable?
[Or the MayTech ESC?](http://www.michobby.com/product/maytech-120a-12s-brushless-esc-for-electric-skateboardse-bike-golden-color/) They have too hard brakes am I right? Where can I buy the FVT ESC?

I want simple plug and play solution, no **** VESC, because I dont have luck with this...
```

---
## \#35 Posted by: onepunchboard Posted at: 2017-08-15T20:54:23.627Z Reads: 47

```
just don't buy 4.12, buy from ollin's enertion etc, modified version. you will have less headache.
if you want, you can try fvt sleeping lion, but you have to update firmware, do some experiment with throttle.
```

---
## \#36 Posted by: aigenic Posted at: 2017-08-15T20:55:28.190Z Reads: 46

```
Not a problem for me, do you have any link where I can buy it? I have send a inquiry via alibaba, but I would prefer buy it now option...
```

---
## \#38 Posted by: aigenic Posted at: 2017-08-15T21:00:14.811Z Reads: 48

```
I mean FVTs sleeping lion...
```

---
## \#39 Posted by: onepunchboard Posted at: 2017-08-15T21:08:51.048Z Reads: 49

```
Oh, I never used fvt, but I believe alien power makes copy version. I saw one live link in the forum to alibaba as well.
```

---
## \#40 Posted by: aigenic Posted at: 2017-08-15T21:09:28.377Z Reads: 50

```
https://www.alibaba.com/product-detail/120A-6-12s-high-voltage-brushless_60572726526.html?spm=a2700.7724857.main07.30.2bd13975bEsssR

Do you think this one could work if it had car ESC firmware?
```

---
## \#41 Posted by: onepunchboard Posted at: 2017-08-15T21:13:05.306Z Reads: 51

```
I found this https://www.alibaba.com/product-detail/FVT-New-developed-120A-brushless-ESC_60552149704.html?spm=a2700.details.maylikever.10.697a8c3e02DpYz

im not sure if the diff model can change firmware
```

---
## \#42 Posted by: aigenic Posted at: 2017-08-15T21:18:16.512Z Reads: 50

```
And what about these two from HK? 
[1](https://hobbyking.com/en_us/turnigy-k-force-120a-hv-opto-v2-5-12s-brushless-esc-1.html)
[2](https://hobbyking.com/en_us/turnigy-sentilon-v4-100a-5-12s-hv-bulletproof-speed-controller-w-rpm-sensor.html)
```

---
## \#43 Posted by: onepunchboard Posted at: 2017-08-15T21:35:34.180Z Reads: 47

```
I can't tell for sure, but these can work. you can program it too so
```

---
