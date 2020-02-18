# Discharge levels of batteries and build advice needed

### Replies: 12 Views: 2164

## \#1 Posted by: Frankenstein Posted at: 2016-06-26T03:29:42.180Z Reads: 118

```
Hi everybody,

So I've read a lot about E-boards and what parts I should get, gear ratios, Motor Kv's, wheel types, etc. 

But I'm going for a little bit of an unconventional approach.

I'm just a little confused on batteries. First, let me tell you what I've already bought.

Gears:
15 Teeth and 40 Teeth both 5mm pitch.

Motor: 
400KV 1375W 80A Brushless Outrunner
http://www.ebay.com/itm/181913535441?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

Connections:
10 Gauge wire

Belt:
65 Tooth Pulley Belt
https://www.amazon.com/gp/product/B008IGUK1M/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1

ESC: 
150A Car ESC
http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=65973

So my question is what battery I should get. I was looking at this 5000MaH 4S 20C battery: 
http://www.hobbyking.com/hobbyking/store/__18631__Turnigy_5000mAh_4S1P_14_8v_20C_Hardcase_Pack_US_Warehouse_.html

Wheels:
83mm Flywheels

With the gears, it is a 2.667 ratio and at 14.8 V, @ 5,920 RPM, it goes to 22 MPH. I'm looking for a top speed of around 20, but I probably don't need to go that fast to be honest. 

Unfortunately, I cannot find any batteries that are 5000 MaH 6S 20C, which is what I planned on. Would a different C value battery at 4S or 6S be possible? I'm afraid that a higher amperage like that would negatively effect heat and possibly be too much for my components.

This is mostly for commuting about 2-3 miles on flat ground on city streets.

Thank you for any input, it is greatly appreciated.
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-06-26T04:00:05.518Z Reads: 105

```
http://toddy616.blogspot.ca/2013/07/electric-skateboard-calculator.html?m=1

http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas

Take a read

I would suggest you move away from such a high KV ....

Better options out there
```

---
## \#3 Posted by: Frankenstein Posted at: 2016-06-26T04:26:49.255Z Reads: 98

```
Thank you but I have read that.

Like I said, I'm going for an unusual build. I've seen quite a few posts where people have used higher KV's than everyone always suggests to use with perfectly acceptable results. 

I'm sorry if my question was worded incorrectly. I am asking about the Discharge Rate (C) and whether or not that will effect my components. It is much easier to find a battery at a higher C than 20, but 100 Amps current, which is what a 5000MaH 4S 20C battery puts out max, might be the max for my components.

Is a higher C rating a constant value? In other words, does a 5000MaH 4S 20C battery always have to put out 100 amps or can it fluctuate?
```

---
## \#4 Posted by: Jinra Posted at: 2016-06-26T04:35:12.082Z Reads: 86

```
components draw as much power as they need. If it drew 100amps constantly you'd be out of power in less than 5 minutes!
```

---
## \#5 Posted by: trbt555 Posted at: 2016-06-26T04:35:22.479Z Reads: 87

```
The C ratingj tells you how many amps the battery can safely supply.
The actual amps you draw frim the battery will depend on the load you put on your system and the voltage you're running.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-06-26T04:39:02.990Z Reads: 90

```
You won't have a problem with the battery...higher the c rating the better....the strain will be on the motor with your setup...That's your weakest link

You mentioned that  abt 3 miles you are going...not sure what kind of riding that is but you will find lower torque will be better on the motor...at low speed it may have a harder time thus reducing the life of the motor
```

---
## \#7 Posted by: Michaelinvegas Posted at: 2016-06-26T04:44:37.593Z Reads: 87

```
If you wanna stay cheap 

https://www.ebay.com/itm/181913685694 

I promise you...this will suit you better....this is the highest kv I'll go unless it's the g160 at 295kv and that's a bigger can size

This will lessen the effect of the load on the motor....I find that issues happen at low speed and top speed...pushing the motor with amps to get you moving...then the amps they drop off...higher speeds trying to squeeze out a little more speed with a load will increase those amps....both resulting in the magic smoke with the wrong motor set up
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-06-26T05:27:16.730Z Reads: 75

```
[quote="Frankenstein, post:3, topic:5152"]
I've seen quite a few posts where people have used higher KV's than everyone always suggests to use with perfectly acceptable results.
[/quote]

Please note those are few and far between...special cases, not the norm...and rare they post continuing success with those types of setups
```

---
## \#9 Posted by: Frankenstein Posted at: 2016-06-26T06:44:29.769Z Reads: 70

```
Thank you all for the input. If it turns out I fucked up by ordering too soon, which is highly likely, I'll just have to buy a new motor and gear set i guess, since I can't return the motor.

I'll just have to try it out and if it works or doesn't, I'll make a post about it either way so people can see the results.

Thanks again.
```

---
## \#10 Posted by: Hummie Posted at: 2016-06-26T07:06:14.936Z Reads: 68

```
I think 400kv should be fine. Your calculating above using 14 volts though and youll be at higher voltage with 6s and faster.   U could always increase the gear ratio and then it's oranges to oranges really. 

In a way the higher kv the safer as the windings are thicker or at least have less resistance and can take more amps 
Strangely this motor is said to be able to take 80amps continuous but only able to do 1375watts at a max of 8s. The math doesn't add up but it's all bunk with those stats for almost all motors anyway and 80 amps through it for more than a couple seconds and it's a paperweight
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-06-26T18:36:45.127Z Reads: 52

```
That's the thing...there isn't anything wrong doing it the way you want...we just want you to have a solid build that won't break on you.... Sure you can gear it so that it works...sure you can...but sometimes the effort in searching for the correct items makes building it difficult.... 
It's like why not choose the path of least resistance to achieve the same result..

We hope it works well mate...and will still be here to help on that set up....and the worst thing that could happen...just get a new motor...every thing else can stay


 Look forward to seeing what you build 🤘🏻
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-06-26T18:43:12.854Z Reads: 45

```
He would have to be really easy on the throttle at low speeds and def always kick off as not to ramp up the amps ....... I've seen motors burned out at very low speed with too much load ..... POOOF ... CRACKEL CRACKEL
```

---
