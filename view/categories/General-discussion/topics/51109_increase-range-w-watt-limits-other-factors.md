# Increase Range w/ Watt Limits + Other Factors?

### Replies: 5 Views: 782

## \#1 Posted by: skatardude10 Posted at: 2018-04-03T20:14:44.251Z Reads: 105

```
I'm on the final step of [my build](http://www.electric-skateboard.builders/t/lbl-build-longboard-larry-stingray-tb-218-tb-6374s-190kv-tb-mounts-chibattery-10s4p-dual-focboxes-in-progress-build/50610) right now and have a few questions. My end goal is to have a board that I can select a high wattage mode to increase torque that is geared for high top speed, but with the ability to select a lower wattage mode that becomes efficient enough to travel much further with extremely reduced amp draw.

Primary question: how effective is decreasing watt limits on ackmaniacs firmware, or in general limiting amps, at increasing range substantially?

Background: I've gone through many calculators, and I'd like to hear some real world examples of people messing with settings to increase their range rather than just reading calculator results to myself. 

Based on calculator results, I could get anywhere from 20+ miles with limits on the amp output / watt limits / keeping under 20 watt hour average, all the way down to 4 miles when pushing my components to the max.

Secondary question: this is more of a loose question on the thoughts of running 1.6:1 gear ratio instead of the standard higher gear ratio, how that might *realistically* affect my efficiency, torque, amp draw, heat output, distance, etc, with 2x 6374 190kv motors and 10s4p battery. I know it's against the general recommendation to run 16/36t w/ 90mm flywheels, I am going to try 20/32t instead, with 15/36t on hand incase it's horrible. I am gearing for higher top speed, but would decreasing my watt limit to 500 Watts max for range on such a low gear ratio even make any sense? I don't care too much about torque if it means I get better range, and with my BT module I assume it's easy enough to swap to a higher wattage temporarily if I need to climb 10%+ grades for a short period of time. I'd prefer to have the ability to already be geared for high top speed and simply change available Watts / amps to push me faster on demand and limit Watts to increase my range when needed.

Again, I've been reading all the threads lately and via searching about gear ratios, voltages, and running through calculators for all these variables, and I know that lower gear ratios will draw more amps... I'd just like to hear some of the communities thoughts and experiences on these things. I know the sentiment is to run somewhat close to 16/36t, but for those that have not or do not, I'd love to hear your thoughts as well... Also I'd like to hear from people who prefer speed to torque in general too. 

Thanks guys!
```

---
## \#2 Posted by: wafflejock Posted at: 2018-04-03T20:21:39.206Z Reads: 98

```
I don't think limiting amps is going to have that substantial of an effect, reason being you aren't typically spending much time at those extremely high amp ratings unless you're a big guy racing up hills.  Even if the limit is at say 40A if you only ever draw 20A then that high ceiling doesn't matter.  https://metr.at/r/hmtOO <-- if you were to say spend most of your time at the peak amperage then yeah limiting that down will make a difference I just don't know how realistic that is.
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-04-03T20:29:58.213Z Reads: 91

```
As my max, I plan on limiting each of 2 escs to 40A for 80A total. I do weigh about 90kg and plan on climbing a few hills. Im thinking that with such a low gear ratio, it's going to take more energy / amps to get me moving as opposed to gearing for more torque and less speed which is why I ask about limiting the amp draw for flats. I hope you are right and I hope I'm not drawing near the max for a lot of my riding ☺️, and if it ends up that I am constantly drawing more amps than expected due to my gear ratio, I'll change my gear ratios at that point.

Side question to the main post... Do you guys think it's realistic to expect the torque output of two 6374 motors geared low to roughly equate to a single less powerful motor's torque?
```

---
## \#4 Posted by: Battosaii Posted at: 2018-04-03T21:16:43.989Z Reads: 70

```
I don't have any settings low or high settings on my board it's tuned to where I like it power wise and if I know I'm gonna do a long ride I don't go around and go heavy on throttle. I've done 30miles on my dual 6374 set up with 12s4p, if in go easy on the throttle to accelerate gently and not go passed 25mph I can go far as hell.
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-04-16T23:27:29.319Z Reads: 50

```
Update: So since i've had my board I have had the chance to test this quite a bit... limiting amps and setting a total wattage limit. It's pretty crazy:

* Limiting to 30A Total / 300W: average wh/mi	4.75
* Limiting to 60A Total / 1320W: average wh/mi	7.72
* Limiting to 60A Total / 1680W: average wh/mi	21.74

By limiting my board to the "*eco mode*" I have setup, I can go QUITE far... like 35 miles on a charge. Or, I can leave my default on, which limits max watts to what can be delivered down to 33v after accounting for voltage drop and have a sort of *fun* mode that can go maybe 10 - 12 miles on a charge. Again, I can up the amps, remove wattage limits, have crazy voltage drop but get a **TON** of power for about 4 or maybe 5 miles. :-D  Even on the "*eco mode*", it still gets up to speed pretty fast and goes fast overall thanks to the gearing... just without **all** of the *umph* it could have to get there.

I love the flexibility of the VESC and Ackmaniac's firmware/app.
```

---
