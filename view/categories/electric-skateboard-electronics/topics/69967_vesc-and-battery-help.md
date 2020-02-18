# Vesc and Battery Help

### Replies: 10 Views: 328

## \#1 Posted by: aDamnd Posted at: 2018-10-03T09:39:00.224Z Reads: 69

```
Complete Newbie here, have done a few days reading but I am a bit stuck here.

First build.

Im looking at buying this Vesc (the only one I can find in NZ) [link](https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html)

The specs are:
Amps: 50A continuous / 240A peak
Cells: 3-12S LiPo
Voltage: 12.6-60V
BEC: 5V@1.5A
BEC type: Internal driver support 
Timing: Software calibration 
Cutoff Voltage: Programmable
Frequency: PWM input 
Governor: No
Weight: 80g
Size: 60x40x20mm
Programming card: No
Reverse: No

My battery is going to be a 10sp2 Li Ion which will (I think) produce 120A Cont. / 180A Max dis.

Is this going to be too much for the VESC? 

The motor I am using is a 90A 37V 190Kv motor. 

Do you think this setup will work?

Thanks in advance.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-03T09:44:18.177Z Reads: 61

```
the hobbyking vesc i wouldn´t stress more than 35a bat max.
which LiIon battery in 2p constilation will give you 120A?
i guess you mean lipo right?
which exact lipos you plan to buy?
which motors you plan to buy?
everything from hobbyking?
```

---
## \#3 Posted by: aDamnd Posted at: 2018-10-03T09:49:39.261Z Reads: 58

```
Thanks for replying,

What do you mean by your first sentance?

I am planning to spot weld my own li Ion battery using a 10s2p config with LG 3000mAh 20c batteries. 

The motor I am thinking of is this one from hobby king. I don't **need** to get everything from hobby king but so far it is the most accessible/reasonable shop I have found for an NZ buyer.

[Motor:](https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html)
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-03T09:58:26.170Z Reads: 55

```
you can program the vesc.
there you need to set the may current which the vesc can/should draw from your battery and you set the max current for your motor too.
(it´s called motor max and motor min setting and battery max and min setting in the bldc or VESC tool)
if you set the value to 50A this vesc will probably heat up and in worst case brake.
as this is a hw 4.12 based esc without heatsink you shouldn´t set the battery max value higher than 35a.
which LG cells you will use?
LG HG2? if yes than read the datasheet please. they rated to 20A max constant current, not 20c. It´s different things.
you will get max 40A out of this 2p pack.
which means later for you that you need to set your vesc bat max settings to 20A (if you run dual) or 35 (if you run dual)

for the motor, if you have a bit a budget left, I would recommend you to get sensored motors. I think with this vesc you will run in bldc anyhow so sensored driving will be more smooth without joggin when start from stand still. 
If you want to go with hobbyking motors than have a look at the SK8 series.
```

---
## \#5 Posted by: aDamnd Posted at: 2018-10-03T10:07:43.476Z Reads: 48

```
Thanks for the detailed reply, and yes you are correct I had confused A with C ratings on the batteries.

You say

> which means later for you that you need to set your vesc bat max settings to 20A (if you run dual) or 35 (if you run dual)

Do you mean if you run dual for both statements?

Can you recommend any other retailers you know of?
Thanks

I will have a look at the sk8's
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-03T10:18:04.200Z Reads: 46

```
you first need to calculate your max battery output current.
as you already made you come to 40A total.
the vesc will be wired in parallel to your battery, which means you need to devide the max battery current to 2.
that means you need to set your vesc bat max limit to 20a in each vesc.
if you run only single it is 35a (not 40a) as it is the max current your vesc can handle.

there are a lot of shops out there.
I mainly know about the ones in europ.
like eskating.eu or unikboards.com
depends what you plan to build you could also have a look at 
https://www.trampaboards.com/
if you buy batteries, make sure you get them from a legid sorce like ru.nkon.nl if they ship to you (if you have the space I would also reccomend you to go for 3p min)
enclosures you can get from @Eboosted at https://www.eboardsperu.com/
for vesc options you could have a look for focbox or flipsky.
just google it ;)
```

---
## \#7 Posted by: aDamnd Posted at: 2018-10-03T10:26:53.784Z Reads: 46

```
You've been a huge help, I haven't actually made my battery yet, would you recommend 10s3p instead?
 
I am planning to do a single VESC.

How would I calculate the maximum battery output current?
```

---
## \#8 Posted by: Andy87 Posted at: 2018-10-03T10:36:19.509Z Reads: 42

```
if you stay with lg hg2 cells than you have 20a max per cell.
in parallel you add it up to the count of cells you have in parallel.
so 2p 40a 3p 60a and so on.
the more p the less voltage sag you have.
means you cells run cooler, live longer and you can climb steaper hills ;)
2p would theoretically be enouph for a single drive, thou.
but if you have the money and the space on your board go with 3p.
you will definitely not regret it!
and more range for sure too ;)
```

---
## \#9 Posted by: aDamnd Posted at: 2018-10-04T23:05:34.160Z Reads: 27

```
I know I'm replying a little late, but I was wondering if the [VESC from DIY Electric Skateboards](collections/esc-speed-controller/products/torque-esc-bldc-electronic-speed-controller#description) can handle its stated 50A continuous current. 

Another thing, if I were to use a 10s3p config with one motor with that VESC, could I run it at the max 50A current or would that damage it? 

Thanks.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-10-05T03:35:37.625Z Reads: 21

```
I don’t think that it can handle that 50a const.
It’s a hw4.12 vesc without heatsink.
The normal limit is around 30-35a depending on the location and airflow around the vesc.
If you want to go single, look for a focbox or Flipsky 6.6.
There I would also just start with 40a and look how warm they become. If they work cool you can ride up the amps.
```

---
