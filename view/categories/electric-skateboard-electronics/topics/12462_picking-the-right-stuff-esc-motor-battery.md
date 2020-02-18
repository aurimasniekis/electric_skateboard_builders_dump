# Picking the Right Stuff (ESC/MOTOR/Battery)

### Replies: 14 Views: 4457

## \#1 Posted by: wmj259 Posted at: 2016-11-04T17:10:55.064Z Reads: 218

```
I am interested in making a e-board for my get around on university campus. Theres a big hill that I have to walk up to get to my car lot which is annoying, University is built on a hill slope side. The main paths between buildings are flat but just that hill to the car. 

I have made a deck, trucks  wheels will be 83mm. I might use the 36 to 15/16 tooth gear.
Am thinking about the 192kv or 247kv sk3. Any advice here?

Also i need some advice what battery packs to pick. **I wanna get as much run time as possible,** maybe low speeds like 15-20mph but a lot of torque. 
I was wondering if it is possible to make a 3 group 5s pack such that its in parallel and series at the same time? I know you can make 2 packs into series and parallel but is that idea scalable to more packs?
[Turnigy 5000mAh 5S 25C Lipo Pack $45.57 w/o shipping](https://www.hobbyking.com/en_us/turnigy-5000mah-5s-25c-lipo-pack.html)
[RC ZIPPY Flightmax 5000mAh 5S1P 40C $ 64 w/ shipping.](http://www.ebay.com/itm/RC-ZIPPY-Flightmax-5000mAh-5S1P-40C-/251621222565?hash=item3a95cb28a5:g:U-IAAOSweW5VSHSO)
or any other suggestions. 


ESC, not sure how to pick this out, I heard it depends on what the max AMPs the batteries can kick out?
```

---
## \#2 Posted by: anorak234 Posted at: 2016-11-06T00:07:16.825Z Reads: 197

```
Here's the right stuff based on everything you stated:

192Kv motor (more torque) 
14/36 or 15/36 ratio
10s4p lion battery (I recommend buying a custom pack from @barajabali )
VESC from @chaka or ESC from @oriol360
You want it to have long run time - this means it needs to be reliable as well. I'm not saying these parts are cheap and I realize you are likely on a budget but let me just say from the start cutting corners will cost you more in the long run
```

---
## \#3 Posted by: DilatedPupils Posted at: 2016-11-06T03:07:18.534Z Reads: 180

```
Specially with the batteries. Charging lipos becomes annoying after awhile. Specially when you have a lot. So it's better to go with liion from the start.
And 6374 190kv
```

---
## \#4 Posted by: wmj259 Posted at: 2016-11-06T03:21:28.804Z Reads: 178

```
Yeah I was thinking about going the li-ion route from laptop batteries but then I went towards getting clean 18650's from aliexpress/alibaba. Then it was expensive after I got quotes. Started leaning towards lipos, but I guess back to li-ion it is.
Cheapest quote so far for 40-50 batteries was by @tumich

I would probably make a 10s4p as suggested, I am still trying to find a 192-190kv
```

---
## \#5 Posted by: wmj259 Posted at: 2016-11-07T18:28:13.900Z Reads: 159

```
Anyone know if I should get a sk3 192kv ($71) [https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html)

or a 
6374 190kv ($79) [http://www.electric-skateboard.builders/t/56-5065-motor-group-buy-6354-6374/12604](http://www.electric-skateboard.builders/t/56-5065-motor-group-buy-6354-6374/12604)

Also noticed that the builders DIY for beginners mentioned the Tacon 110 motor which i'm finding for 70 shipped.
```

---
## \#6 Posted by: anorak234 Posted at: 2016-11-07T23:18:54.192Z Reads: 146

```
Go for the 6374 group buy - more torque for about the same price
```

---
## \#7 Posted by: wmj259 Posted at: 2016-11-08T00:01:06.708Z Reads: 140

```
Where do you see the specs if I may ask? I tried on the diy website but all it says is the like connector size......and little more
```

---
## \#8 Posted by: anorak234 Posted at: 2016-11-08T02:43:51.684Z Reads: 130

```
There aren't usually specs for torque... I don't know exactly how that's measured but believe me it's noticeable when testing the motor itself. The 6374 is a bigger motor and will be able to propel you up hills much better
```

---
## \#9 Posted by: wmj259 Posted at: 2016-11-09T21:42:00.893Z Reads: 126

```
Planning to make a either 18650 pack with either 10s3p setup or a 26650 with a 6s2p.
```

---
## \#10 Posted by: wmj259 Posted at: 2016-11-15T17:11:27.755Z Reads: 111

```
Might change from single drive to dual drive. I checked myhills.com or something like that and the hill im trying to go up is steepest 7%. Maybe 2 192kv's? or 2 236kv's?
```

---
## \#11 Posted by: jmasta Posted at: 2016-11-15T19:02:44.991Z Reads: 112

```
<img src="/uploads/db1493/original/3X/9/e/9e6bc6e622cdbee6cba3634e464c44288bb2dcec.jpg" width="348" height="500">
```

---
## \#12 Posted by: wmj259 Posted at: 2016-11-26T04:53:26.474Z Reads: 101

```
What type of C rating should I look for?

I am looking for good deals on battery and so far came up with these 3 

6 FLOUREON 11.1V 3000mAh 3S 30C for 90 bucks with shipping
1 Turnigy 2450mAh 3S 30C 11.1V Lipo Pack for 11.30+shipping
1 Turnigy nano-tech 6000mah 4S 25~50C 14.8V Lipo Pack for 47.30+shipping
or
1 MultiStar High Capacity 6S 12000mAh Multi-Rotor 20C PEAK 22.2V Lipo Pack  for 63+shipping

I so far know that higher capacity (mAh) = longger ride time based on loading on motor. But I think the motor I am going for the sk3 192kv requires a **MAX VOLTAGE** of 44V and a MAC CURRENT of 80A.

My assumptions:
~I think my maximum factor would be hitting the 44V mark so I will consider going to roughly 20-35V threshold to not blow up my motor as the max current probably would never reach 80A?

~So I don't think I would need the multistar in series but could in parallel. but that would be above my $100 limit
~The 6000mAh turnigy 14.8v I could use in either 2 series (29.8V 6000mAh) or 2 parallel (14.8V 12000mAh)
~or the 6 floureon in a (series by parallel):  2by3 (22.2V 9000mAh) or 3by 2  (33.3V 6000mAh)

Any advice? My main goal is to get long rides so I want capacity, but what happens when the motor doesn't get enough voltage/current? Does it run sluggishly?
```

---
## \#13 Posted by: wmj259 Posted at: 2016-11-26T14:10:45.521Z Reads: 91

```
I might have gotten a little confusion out of my head by reading the C rating article by onloop

[quote="onloop, post:1, topic:36, full:true"]

........

**So how can you determine the discharge rate of a battery?** 

Well fortunately this is clearly written on the label. **The 'C' rating of the battery below is 20C**. This means the the battery can peak output at 20X its capacity. 

So what is the Capacity? Thankfully it is also on the label of all batteries, this one below is 3000mAh or 3Ah. So this pack can output 20 x 3Ah making the rated **peak output for this battery 60Ah.** You can get Lipo batteries with much higher C rating and also batteries with much higher mAh. 

<img src='/uploads/db1493/original/1X/4701df3e4c64f6df95ed16a2b27bb2ac00148776.jpg'>

*My first battery for an eboard was an 8000mAh 30C Lipo, So 30Cx8Ah = 240A output! Wow! thats alot... so my board will be much better right?.... well not necessarily*
.................

You will notice it will peak when starting from stationary, when you go up hills it will peak, basically when ever the motor has a load to push it will peak, But cruising around your board should only be using 15-20A of power. Actually you want low numbers you don't want high amps.

**So don't go brag to your mates about how awesome your 6KW (24V X 250AMPS) electric skateboard is!**

So yes your motors might be rated to 2400Watts (2.4kW) Each & Your Lipo might be able to out put 240AMPs and you might have a 150A Continuous ESC....  but you don't really want to reach the peak... its way to hot there & heat is bad!. 
......................
......................

I recommend that 60A Peak is enough for an electric skateboard. If you are constantly needing more then this amount of amps you should increase battery voltage & increase the mechanical reduction to lessen the load on the motor. Or go on a DIET!

**Higher Voltage = Lower Currents**
**Less Load = Lower Currents**
**Lower Current = Less Heat.**
**Less Heat = Longer Life & Improved Reliability of electronics.**
[/quote]

I also read this which states the same as above

[quote="paragon, post:6, topic:7389, full:true"]
The more the merrier (generally higher "c" batteries are heavier and more expensive though).
Put really basically, c rating tells you the continuous amp discharge that a battery can provide;
having a c rating that is too low will make a lipo sag, heat up, and/or puff.
The "c" just means capacity, so 10c means that your max continuous discharge rate is 10 times the pack's capacity. For example, a 10c 5000mah (5ah) pack, would have a continuous discharge rate of 50 amps (50000mah)*.

*Keep in mind that lipo manufacturers (very) often overstate their c ratings.
[/quote]
```

---
## \#14 Posted by: jmasta Posted at: 2016-11-28T01:51:03.647Z Reads: 75

```
[quote="wmj259, post:12, topic:12462, full:true"]
...

But I think the motor I am going for the sk3 192kv requires a **MAX VOLTAGE** of 44V and a MAC CURRENT of 80A.

My assumptions:
~I think my maximum factor would be hitting the 44V mark so I will consider going to roughly 20-35V threshold to not blow up my motor as the max current probably would never reach 80A?

...
[/quote]


44V is the nominal voltage.  The SK3 6374 192kv motor is designed for 10 to 12S.   12S is 44.4 V nominal, 50.2 V max.  You want to run at higher voltages to minimize current draw.  You aren't going to "blow up" your motor by running it at 12S
```

---
