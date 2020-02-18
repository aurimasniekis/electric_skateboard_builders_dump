# Motor Watt calculate issue

### Replies: 7 Views: 1235

## \#1 Posted by: Hoho0220 Posted at: 2016-09-27T15:23:32.632Z Reads: 159

```
Hi guys

I built a e board  with 
fvt120a ESC support 6s battery
6355 motor 
Battery undecided( ruin a lipo 6s 5200mah 25c)
In lipo battery the max current is 125 amp 
so the Watt in 24v 24v*120a=2880watt?
If I build Samsung 25r 6s3p ,the max current is 75a
So the Watt in 24v 24v*75a=1800 watt
My home to office has a uphill
When I use the lipo battery is easy to uphill
Is 6s3p can easy uphill or I need build 6s4p 6s5p for more Torque?
Any suggestions?
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-09-28T19:23:06.384Z Reads: 131

```
how much amp is your motor capable of?
it´s never a good idea to stress these specs to their max. because you won´t have long fun with your components this way. Always leave a bit room with your motor, esc and specially your batterys!
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-09-28T19:41:53.321Z Reads: 126

```
[quote="TarzanHBK, post:2, topic:10230"]
how much amp is your motor capable of?
[/quote]

That is the most important question![quote="TarzanHBK, post:2, topic:10230"]
it´s never a good idea to stress these specs to their max. because you won´t have long fun with your components this way. Always leave a bit room with your motor, esc and specially your batterys!
[/quote]

Thats right **but**
you can set the motor max to the specs of the motor.

Why?
Because you will hardly reach that point that the motor is pulling the max amp! So you will mostly have this breathing room ;)
```

---
## \#4 Posted by: sl33py Posted at: 2016-09-28T19:45:06.014Z Reads: 114

```
Tarzan has good suggestions.  I would also add an inline watt meter to measure your actual amps.

regardless of the Watts - it's about the performance.  I take almost all claimed watts and other performance measurements with a grain of salt (it's marketing).  Real world performance, and real world amp draw (or amp capacity/supply from your batteries) is the critical issue.

So measuring todays amp draw w/ a simple watt meter should help you design a li ion pack that is able to at least match performance!

here's one i tried:
[img]https://images-na.ssl-images-amazon.com/images/I/41EWf6ZWYhL.jpg[/img]
https://www.amazon.com/Makerfire®-Precision-Power-Meter-Analyzer/dp/B00ORGDQOK

HTH - GL!
```

---
## \#5 Posted by: Hummie Posted at: 2016-09-28T21:52:46.726Z Reads: 93

```
You can put as many amps in ur motor as u want till it gets as hot as the magnet's max temp after that it can make it a weaker motor.  watts is volts x amps.
```

---
## \#6 Posted by: lamjiasheng Posted at: 2016-10-19T14:22:52.674Z Reads: 85

```
Hey guys u guys seem good to it
I have a question here
Let say 10S3P capable of delivering 2960 watts of peak power.
and Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor have a max power of 2700 watt

With this build cause the motor to break because of the higher watt supply or will it work just fine ?
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-10-23T17:41:12.247Z Reads: 72

```
you can use a battery able to deliver 70000W on an motor which is capable of 400W, your VESC is doing a limitation of power when you set it up correctly
```

---
