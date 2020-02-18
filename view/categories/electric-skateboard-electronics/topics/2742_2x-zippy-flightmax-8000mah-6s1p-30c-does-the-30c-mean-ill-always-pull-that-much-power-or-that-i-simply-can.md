# 2x ZIPPY Flightmax 8000mAh 6S1P 30C&hellip;does the 30c mean I&rsquo;ll always pull that much power, or that I simply can

### Replies: 12 Views: 2178

## \#1 Posted by: itsmikeholland Posted at: 2016-04-30T04:42:02.474Z Reads: 160

```
I'm wondering if this battery rig will be too much for my 120A ESC 12s motor to handle. Living in the west side of LA, I'm not really comfortable going more than 15mph, which seems to be well within the capabilities of a 6s. Will this board constantly be putting out 30c, or will it vary depending on how hard/soft I push it?

I'm using a Turnigy Aerodrive SK3 - 6374-149kv. I'm hoping to get close to a 25 mile range to get me where I need to go, which, using the 10wh=1km rule would require me to have a 18,500 mah rig at 22.2v. This rig appears to get me close enough, but I want to make sure there isn't any major oversight going on, since after all this is my first build
```

---
## \#2 Posted by: NNGG Posted at: 2016-04-30T04:49:31.872Z Reads: 159

```
buy a pair of 3S 5000mah 30C batteries and run those on your SK3 149kv. Limit the punch, acceleration and trim so you wont go faster than 15mph. Realistically, a 149kv should get around 20-25 mph MAX, but on pavement would be at 15-25 mph. 

TL;DR  run 12S on your SK3 and limit your throttle and I didnt answer your question.
```

---
## \#3 Posted by: itsmikeholland Posted at: 2016-04-30T04:54:08.326Z Reads: 156

```
I didn't know that about the 149k! I jumped on the sale just because I heard low kv = low IR = higher efficiency = higher torque, good to know I'm not stuck going 10mph or something. 

so I can program my ESC to limit the punch and acceleration, which will effectively allow me to draw less amps and get more range at the sacrifice of speed, right?
```

---
## \#4 Posted by: NNGG Posted at: 2016-04-30T05:03:03.403Z Reads: 148

```
Whats the esc?  1jknqjnqjnw
```

---
## \#5 Posted by: itsmikeholland Posted at: 2016-04-30T05:04:56.274Z Reads: 137

```
[TorqueBoards 12s 120A ESC for $145 plus shipping](product/torqueboards-12s-120a-car-esc-opto-hv/)
```

---
## \#6 Posted by: Namasaki Posted at: 2016-04-30T06:18:30.298Z Reads: 137

```
I'm using the torqueboards 12s. with 2 6355 230v motors currently and have also used them with dual Carvon 145kv hub motors.
I found that if I set the motor timing on high to very high and the acceleration on high to very high and forward power on 40%
the results is about 15mph top and a lot of control with very easy acceleration.
some of the settings are misleading. 
especially the acceleration setting.
if you set it on low, you will have a lot of torque and jerky acceleration especially at low speed
set it on high to very high and you will have smoother more controllable acceleration
most important is the forward power setting. 40% is like beginner mode. very easy to control
about the batteries, 
it's always better to have more battery than you need.
8ah x 30c = 240 amp capability.
with your esc limited to 120 amps and the motor limited to 80amps you will never have to worry about over taxing the battery. I think you are on the right track.
12s is better way to go because you can limit it for control now and turn it up later if you decide to go faster.
higher voltage means less amps. so if your going 15mph with 12s you should be pulling less amps than if your going 15mph with 6s. Less amps means less heat.
```

---
## \#7 Posted by: itsmikeholland Posted at: 2016-04-30T06:38:40.768Z Reads: 135

```
awesome! 99% of the time they'll be wired in series as a 12s to get me to and from work. The furthest ever need to go is about 11 miles from work to my studio house, then getting to my actual house is about 9 miles all downhill, so it might make sense to switch to parallel every once in a while and use the downhill to my adavantage
```

---
## \#8 Posted by: Namasaki Posted at: 2016-04-30T07:14:28.761Z Reads: 127

```
I'm using 2 zippy compacts. 6s 5000mah in series and I can go 7 miles without using up the battery. 
Yo shoul be able to go 11 miles on 8000 mah. 
Skateboard mileage formula 
22.2 wh per mile. 
Wh = Voltage x Ah
22.2 x 16 = 355 wh/22.2= 16 miles
44.4 x 8 = 355 wh/22.2= 16 miles
(Actual mileage may vary)
Depending on your weight, how fast you ride, going uphill, riding against strong winds, rough roads etc. 
With more voltage, you pull less amps. 
Pull less amps and your battery lasts longer. 
So double voltage or double capacity, your distance should be the same. 
The reason 12s is better is lower amp draw means less heat in your motors, electronics and batteries.
One thing I almost forgot to mention, you need to be very carful not to drain lipos too low, especially Zippy's. 
I ruined two new packs because I rode a little too long one time. It has been recommended to me not to go below 3.7 volts per cell. 
It's best to put a low voltage alarm on each pack. 
Now I swap out my pack when it gets down to 44 volts. It's 50.3 volts when fully charged.
```

---
## \#9 Posted by: itsmikeholland Posted at: 2016-04-30T14:03:21.322Z Reads: 101

```
sweeeet and yeah I have a low voltage alarm for both packs as well, all batteries become expensive batteries when you have to buy them multiple times from not taking care of them. I think I'm going to pull the trigger on the zippys, everything appears to be in their favor...of course theres always time to do one more quick browse lol
```

---
## \#10 Posted by: Namasaki Posted at: 2016-04-30T15:17:57.855Z Reads: 95

```
Zippy's are a real bargain. I got my compacts on sale from HK for only $26 ea. And they perform very well. 
The flight max 8000/30 will be much better. 
Be sure to check the voltage on each cell before charging them. I have gotten a pack from HK that was bad right out of the box with one or two cells below min voltage. When that happens, they will replace it or issue refund.
```

---
## \#11 Posted by: itsmikeholland Posted at: 2016-04-30T15:28:05.469Z Reads: 88

```
Thanks for the heads up checking the voltage! You can check this with a balancer, right?
```

---
## \#12 Posted by: Namasaki Posted at: 2016-04-30T16:17:50.320Z Reads: 89

```
Yes, or you can check it with voltage alarm or a Turnigy voltage/internal resistance meter like the one hobby king sells. 
If you get a bad pack, they will have you send pics of the battery with s/n number and the voltage readout. 
They will replace the battery and tell you do not send it back. You'll have to dispose of it.
```

---
