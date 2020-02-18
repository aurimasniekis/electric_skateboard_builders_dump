# VESC FAQ &#124; Optimized S.P.A.C.E Cell Settings

### Replies: 14 Views: 5460

## \#1 Posted by: onloop Posted at: 2015-11-05T00:20:05.454Z Reads: 423

```
Using the VESC & The S.P.A.C.E Cell together to build your esk8 is a great combination!.. It gives you a system which is not only very safe, simple to build and easy to use whilst being super slim, but one that is offering a level of technology that is unmatched in many of the commercially available boards the have been born from various crowdfunding campaigns. The technology available in the VESC alone puts you in a league of your own when it comes to eboard performance and configurability. In this article I will explain how to configure the VESC to get maximum performance.

**First, let's discuss the limitations of the S.P.A.C.E. Cell**
1. It has a 30A fuse, this is a safety feature to prevent you from ruining your battery if you make a mistake with wiring or if there is a short in the circuit after the battery. 30A fuses can actually throughput bursts of current that exceed 30A for a few seconds, any longer than this and they will blow and protect the other components. You can expect bursts of up to around 40-60A for 1-2 second without it blowing.
2. The BMS inside the S.P.A.C.E. Cell Can handle 30A continuous throughput and peak of 60A for a few seconds, anymore and it will blow also. This protects the cells from over discharging, overheating and self destructing leading to a catastrophic thermal runaway event..
3. The cells inside the S.P.A.C.E Cell in a 10S3P configuration can easily support a discharge of 60A continuous but will never be able to as the Fuse & BMS will prevent it.

**Why is the S.P.A.C.E. Cell limited?** 
1. It is limited by the FUSE & BMS to save itself & save you money just incase something bad happens.
2. It prevents you from inadvertently punishing the cells & the other componentry to the point of early failure. For example; some people might think it is a good idea to tow their friends on a non-powered skateboard... in most cases this will be ok, but if you then decide to tow them up a steep hill, without current protection, the electronics will just keep heating up and eventually the weakest link will catch fire or melt. The S.P.A.C.E Cell won't allow this and you will blow a $2 fuse instead of a $200+ worth of electronics..
3. This is DIY & Accidents do happen, with a fuse in place if you accidentally short circuit your wiring the fuse will blow & save you $200+

**How can I ensure I don't blow up my S.P.A.C.E Cell?**
1. Firstly, you should always be thinking about your system and how you are using it, knowing its limits and being respectful of them is important. This is the same for any electric vehicle.
2. Most importantly - Use a Motor Controller, like the VESC, that has built in protection features such as current control.

> So what are the best VESC settings to use to ensure your S.P.A.C.E Cell lives a long and happy life?
> ------------------------------------------------------------------------

As I mentioned the VESC has current limiting functionality which is what we will focus on. It also has built in temperature sensors and rpm limiting and a whole bunch of other really useful features that need to be discussed in another topic.

**NOW Let's configure the VESC for S.P.A.C.E Cell**

Open BLDC tool / Motor Configuration *TAB* / Motor *TAB*

You should see this screen:
<img src="/uploads/db1493/original/1X/476f9b881a9d2b7310f7afd7af78fe8a45b7c094.png" width="690" height="461">

We will be working on the "Current Limits"
<img src="/uploads/db1493/original/1X/e68b0dfd5e1990ca2b1713e39af7d63020202a97.png" width="538" height="215">


1. This is the MAX amps you want inside your motor, set it at 80 Amps
2. This is the MAX amps you want inside the motor during braking, it's set to (-60) 60 Amps by default, leave that.
3. This is the MAX current draw from the battery, set it to 30Amps which matches the BMS inside the S.P.A.C.E Cell
4. This is the MAX regen-charging current you want to flow into the battery whilst braking. (-12) 12 Amps is the Maximum safe level for the Cells inside the S.P.A.C.E Cell. The lower you make this setting the weaker your brakes. You could go higher if you want stronger brakes just be aware that high sustained regen current can reduce cell life. 

*NOTE: This is the setting you would use for a single VESC, for Dual VESC you might need to reduce "Batt MAX" to 15A in each VESC making the combined total across two VESC equal 30A Max battery current.*
*NOTE: The negative "-" value indicates power running backwards through the VESC back into the Battery.*

With these settings you cannot blow your fuse or damage the S.P.A.C.E Cell by riding aggressively. However a short will still blow the fuse no matter what settings you have inside the VESC

**So how does the Motor MAX & Batt Max settings work?** 
The VESC is able to independently measure & control the current at the battery & at the motor simultaneously! This means you can achieve impressive start up power whilst keeping overall currents low when cruising at higher speeds. 

I can't explain to you *exactly* how this works because I am not an electrical engineer.... but for fun I will take a guess! I think it has something to do with ohm's law **V = I R**  if the battery can output a peak of 1080 Watts total it means current in the motor can be high whilst the voltage is low. This means when you have a lower RPM and less voltage in the motor you can have higher current. As the RPM increases and Voltage increases the motor current will become more & more limited.

In a propulsion system that is geared for a top speed of about 45km/h the motor current can reach the 80A peak up  until you reach 3/8s of your top speed which is about 16km/h... Once you have reached this speed the current will begin dropping down. 

With this functionality you can have high starting current and not blow your battery up!
```

---
## \#2 Posted by: RandV Posted at: 2015-11-05T07:06:12.205Z Reads: 340

```
Very helpful and informative.

Looking forward to lots more VESC tutorials.
```

---
## \#3 Posted by: onloop Posted at: 2015-11-05T07:23:29.899Z Reads: 332

```
link to all the vesc FAQ so far, http://www.electric-skateboard.builders/search?q=vesc%20faq
```

---
## \#4 Posted by: locktight Posted at: 2015-11-09T22:55:08.511Z Reads: 323

```
If using dual vesc would you change the max regen to -6?
```

---
## \#5 Posted by: onloop Posted at: 2015-11-09T23:23:47.818Z Reads: 308

```
i probably wouldn't worry about it, regen current spikes are very rapid. they are not sustained constant currents that will over heat your battery.

the exception to this is if you are on a super steep hill, one that is so steep when the brake is applied 100% you are still travelling rapidly... this would max the regen current and potentially overcharge the battery.
```

---
## \#6 Posted by: t1m0007 Posted at: 2016-07-25T04:43:47.934Z Reads: 219

```
@onloop could you update this for the spacecell3 with the newer fuse? Isn't the amp limit 40-50 nowadays? I want to be sure I set these values correctly
```

---
## \#7 Posted by: philipp Posted at: 2016-07-31T15:57:09.534Z Reads: 208

```
[quote="t1m0007, post:6, topic:414"]
@onloop could you update this for the spacecell3 with the newer fuse?
[/quote]
this... :)

10 chars
```

---
## \#8 Posted by: BlakeA Posted at: 2016-07-31T16:45:29.819Z Reads: 201

```
Check out his posts in [this thread](http://www.electric-skateboard.builders/t/lost-of-brakes-when-going-full-speed-enertion-parts/6895). It may help a bit.
```

---
## \#9 Posted by: t1m0007 Posted at: 2016-08-01T19:32:42.766Z Reads: 196

```
Good catch- Thank you. This is exactly what I need since I'm currently waiting on SCP3 to go with my 6374 RSpec. Posting Information here for future reference:

http://www.electric-skateboard.builders/t/lost-of-brakes-when-going-full-speed-enertion-parts/6895/3?u=t1m0007
```

---
## \#10 Posted by: rodriguejoe1 Posted at: 2016-08-28T21:00:15.829Z Reads: 162

```
Trying to do some math here on how to calculate amps in a battery pack.. 10s3p vs 10s 4p for example. Sorry for the over simplistic noobie guy explanation/question. I get that series increases volts and keeps milliamps the same. parallel series increase milliamps and keeps volts the same. but the numbers do not add up. Do i need more battery specs. i am assuming 2500 to 3000 milliamps per battery..multiplied by ??? then divided by??? to get the answer. i also understand c ratings and watt hour.. can someone show me the math please. Thanks.
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-28T21:21:38.701Z Reads: 152

```
2500 per cell times 3 or 4p = 7500/10000 milliamps.
10s = 36v nominal

36 x 7.5/10 = 270/360watt hours
```

---
## \#12 Posted by: rodriguejoe1 Posted at: 2016-08-28T21:35:23.573Z Reads: 153

```
Thanks..got it..
```

---
## \#13 Posted by: Monte Posted at: 2016-08-29T07:40:52.175Z Reads: 139

```
Is the setting the same if i want to use foc mode?
```

---
## \#14 Posted by: rodriguejoe1 Posted at: 2016-08-29T17:03:28.509Z Reads: 136

```
Can  you post dual vesc 10s3p Raptor set up values please. Thanks
```

---
