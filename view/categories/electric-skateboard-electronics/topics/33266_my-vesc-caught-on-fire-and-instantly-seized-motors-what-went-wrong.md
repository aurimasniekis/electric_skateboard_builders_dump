# My VESC caught on fire and instantly seized motors - what went wrong

### Replies: 26 Views: 1989

## \#1 Posted by: cody00 Posted at: 2017-09-16T15:21:55.587Z Reads: 274

```
Hi All,
I'm trying to trouble shoot what just happened while I was out for a ride.  I was 3.9 miles into a ride when all of the sudden both motors seized and I was launched off of the board (luckily landing on my feet).  After I got home, I took off the enclosure and noticed that one of the VESC had caught on fire.

[Here is my board](http://www.electric-skateboard.builders/t/acorn-duster-loaded-vanguard-2x-torque-6355-190kv-10s3p/32585/6)
[Here are my VESC settings](http://www.electric-skateboard.builders/t/vesc-setting-check-for-first-time-builder-10s3p-2x-6355-190kv/32576)

I'm 99% certain nothing shorted out as I made sure to wrap ever piece of exposed metal and secure all items in the enclosure.  I have ridden this board 50+miles without issue.  
<img src="/uploads/db1493/original/3X/c/4/c420d2a719a7aacb7b149a902e2e4d63417c9125.jpg" width="375" height="500">
```

---
## \#2 Posted by: ThierryGTLTS Posted at: 2017-09-16T15:33:03.375Z Reads: 264

```
I don't like VESC in shrink tubes!

They are overheating.

See tests a guy has done with and without ventilation, temp is about 2 times higher when not air cooled.

Have a Nice Day.

Thierry
```

---
## \#3 Posted by: cody00 Posted at: 2017-09-16T15:38:36.736Z Reads: 260

```
Thanks Thierry - Don't the VESC have Min and Max MOSFET temp to protect against this?
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-09-16T15:40:29.905Z Reads: 258

```
Yea they do.  It shouldn’t have caught on fire.  Must’ve been faulty
```

---
## \#5 Posted by: cody00 Posted at: 2017-09-16T15:43:16.445Z Reads: 256

```
@torqueboards - Have you had any other reports of this?  

Hopefully, it was somewhat contained.  To completely seize up the motors it had to have thrown some weird power its way.
```

---
## \#6 Posted by: Jinra Posted at: 2017-09-16T16:43:18.065Z Reads: 243

```
i have seen another tb vesc recently where the mosfet caught fire
```

---
## \#7 Posted by: torqueboards Posted at: 2017-09-17T00:36:29.421Z Reads: 208

```
@cody00 I haven't heard of anything like that before. I believe, the BMS or a fuse should have prevented that.
```

---
## \#8 Posted by: Ulfberht Posted at: 2017-09-17T00:53:49.026Z Reads: 204

```
Anybody think that the 16t/36t gearing with those 100mm plus MBS wheels might be an issue?
```

---
## \#9 Posted by: cody00 Posted at: 2017-09-17T00:55:04.116Z Reads: 200

```
@torqueboards You think this is current issue vs heat issue?  I am currently discharging through BMS.  Other VESC on other side of splitter is fine.
```

---
## \#10 Posted by: torqueboards Posted at: 2017-09-17T01:06:31.063Z Reads: 200

```
@cody00 It could be a current issue through the BMS. What BMS are you using? BMS should shut down if there's too much current. MCU will shutdown mosfet if too much heat.

We should probably run a fuse on custom battery setups. I do know there was one guy before on this forum who's setup caught on fire and he was using a custom battery setup. But those are the only two instances I recall otherwise it's folks shorting power wires but that's just a mistake.

@Ulfberht I don't think that's the issue at all. Seems more like a power issue. Would need some ridiculous gearing for it to be an issue.
```

---
## \#11 Posted by: cody00 Posted at: 2017-09-17T01:15:35.641Z Reads: 192

```
10s3p with 

https://m.ebay.com/itm/221769582503?_trksid=p2057872.m2749.l2649&_mwBanner=1

Technical Parameters:
Balanced current: 60mA (VCELL = 4.20V when)
Balanced for: 4.20 ± 0.05 V

Over-charged Protection: 4.20 ± 0.05 V
Over-charged delay: 55mS
Over-charged release: 4.05 ± 0.05 V
Over-discharged threshold: 2.90 ± 0.05 V
Over-discharged delay: 5mS
Over-current Protecton: 60 A

Max Continuing discharge Current : 60A

Max Charge Current : 30A

Static power consumption: less than 200uA

Short-circuit protection function: disconnect the load from the recovery.

Size: 112mm * 53mm
```

---
## \#12 Posted by: torqueboards Posted at: 2017-09-17T03:28:14.454Z Reads: 170

```
Yeah, not sure what to tell you. I'd probably install a fuse that way the VESC's aren't damaged. We haven't had any of these issues from what I know.

Part of what I've been focusing on lately is more reliability in all parts. We've also been working on more custom electronics in-house that way we can manage upgrades, bug fixes, reliability on our end. I'll probably look into building a fuse an our ESC and/or on external option.

You can wire one of these on the positive side after the batteries to the VESC - https://www.digikey.com/product-detail/en/littelfuse-inc/142.5631.6102/F6794-ND/2515912.
```

---
## \#13 Posted by: chuttney1 Posted at: 2017-09-17T04:19:32.122Z Reads: 163

```
It looks like you got some fried capacitors. What was the last thing you were doing before you got off your board and went home?
```

---
## \#14 Posted by: cody00 Posted at: 2017-09-17T04:29:35.821Z Reads: 164

```
I was going on about 3.5 miles.  Last 1/2 mile was completely flat with about 100 ft of slight incline right before motors seized and launched me off board.
Average Speed 16MPH. Top Speed 31MPH were trips stats.  

I still can't get past the point of it not being heat vs power surge if the shrink tube was melted - 

Thanks @torqueboards for tip - The whole situation just makes me uneasy - i hate slap in a fuse just to have the same thing happen again.  Are you ruling out the possibility of it being faulty and not shutting down under high heat? 

I'll probably remove the discharge through BMS, add fuse, add ventilation as additional measures.
```

---
## \#15 Posted by: torqueboards Posted at: 2017-09-17T04:56:37.244Z Reads: 150

```
@cody00 We'll I haven't seen this happen before or heard of anyone else with this issue before so it's more of a singled out issue. High heat isn't something we worry about. Something failed that's for sure.. what it actually is. I'm not 100% sure.

Certain things such as this is why I want to focus on building a much more reliable system but unfortunately that means not using other third party parts for a build. Overall it would provide a much better experience + warranty in the end. Working towards there but unfortunately not there yet. :cry:
```

---
## \#16 Posted by: Jinra Posted at: 2017-09-17T05:08:03.796Z Reads: 145

```
There was another one recently as well

https://media.discordapp.net/attachments/343080786078990338/355761763754573824/20170908_100915.jpg?width=622&height=830
```

---
## \#17 Posted by: torqueboards Posted at: 2017-09-17T05:20:39.214Z Reads: 142

```
@Jinra You have a link to the post?
```

---
## \#18 Posted by: Jinra Posted at: 2017-09-17T09:36:23.758Z Reads: 128

```
It was on the esk8 discord
```

---
## \#19 Posted by: ThierryGTLTS Posted at: 2017-09-17T11:18:03.535Z Reads: 127

```
Hello,

I continue to say that it's not a good idea to put a shrink tube around the VESC.

There is a protection, but ... the temp sensor is not on the die of the Mosfet, so there is a temp gradient between the Mosfet die and the temp sensor.

In pratice that means that the Mosfet temp can be much much higher than the sensor especially if the current is very high.

And a fuse in the power line will not help because the fuse is way too slow to react.

Keep your VESC cool, that's the best advice I can give you.

That's not inadvertently that the VESC 6 (and FOCBOX) are equipped with a very large heatsink.

Have a Nice Day.

Thierry
```

---
## \#20 Posted by: cody00 Posted at: 2017-09-20T14:16:05.408Z Reads: 100

```
So i took some advice from @ThierryGTLTS.  Drilled some holes in the front and back of my enclosure in hopes of getting some airflow through.  I installed bluetooth for live monitoring.    Setup everything to run on one motor and did some test.  I set the Max MOSFET temp to 90C from 100C just to give some type of buffer.  

After about 3min of riding here was the screenshot.  It recorded 88C.  Around this time the VESC cut out on a slight decline with slight braking.  My assumption was the braking threw the temperature over the top but I'm not sure as the VESC reset and no messages were captured. It should have been past the "Full Charge with OverVoltage Regen" situation. 
 (It didn't start out at 59C as you see in the screenshot.  I reset the app on accident midway through small ride.)

Is it normal to almost instantly be blasting up to about 80C+? 

I'm going to cut back some of the power to <1000W and cut windows out of the shrink wrap around the mosfets to see if I can get something to stabilize.

<img src="/uploads/db1493/original/3X/8/8/883a1dc504471bead6f17779ca8f0d700cb8f41f.jpeg" width="281" height="499">
```

---
## \#21 Posted by: Sebike Posted at: 2017-09-20T16:08:17.297Z Reads: 86

```
What software is this?
```

---
## \#22 Posted by: ThierryGTLTS Posted at: 2017-09-20T16:10:33.522Z Reads: 87

```
If you record 88°C after only 3 min. you've perhaps a problem with the motor or cables.

Remember that the temp of the Mosfets die is well above the sensor temp, perhaps 10 or even 20 °C.

With default settings 80/100°C the available power diminish above 80°C to protect the Mosfets.

Looking at the Mosfet datasheet will show you that above 100°C the current and power fall abruptly.

So check everything to find the problem.

Have a Nice Day.

Thierry
```

---
## \#23 Posted by: cody00 Posted at: 2017-09-20T16:32:34.273Z Reads: 81

```
http://www.electric-skateboard.builders/t/new-ios-app-eskate-vesc-for-standard-and-ackmaniac-fw/32340
```

---
## \#24 Posted by: cody00 Posted at: 2017-09-20T17:08:37.627Z Reads: 80

```
Thanks for the insight @ThierryGTLTS - Going to inspect everything and I've decided to bypass BMS for discharge and add a fuse.  I'll switch to the other motor while I'm at it to see if I can come up with any positive news in next couple of days
```

---
## \#25 Posted by: cody00 Posted at: 2017-09-22T13:19:49.069Z Reads: 68

```
Switched over to 100A Fuse - Still climbing fairly quickly.   I cut little windows out of the MOSFET and the thing cools down extremely fast as compared to before so it wasn't staying at high heat.  

I'm going to consider @Ulfberht suggestion and get 40t gear for these 100mm.  Maybe it will help take some of the load off. I can then just have a secondary set of smaller wheels with the 36t to change in and out as I need.  

2nd VESC comes in today so hopefully that should distribute even further helping situation.
```

---
## \#26 Posted by: cody00 Posted at: 2017-09-22T18:11:52.079Z Reads: 54

```
Anyone ever hook one of these up and blast air straight into the enclosure?
https://www.amazon.com/GDSTIME-Bearing-Centrifugal-Brushless-Radial/dp/B00ZFPDLE2/ref=sr_1_5?ie=UTF8&qid=1506103786&sr=8-5&keywords=Centrifugal+Blower%2C
```

---
