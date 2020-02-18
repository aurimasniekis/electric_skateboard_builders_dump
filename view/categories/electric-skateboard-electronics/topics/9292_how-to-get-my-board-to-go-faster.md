# How to get my board to go faster?

### Replies: 12 Views: 2046

## \#1 Posted by: nick.schweng Posted at: 2016-09-09T20:54:20.144Z Reads: 120

```
I just upgraded from a single motor setup that could go about 11mph to a dual motor setup. I was expecting the speed to increase because I got the second motor, but it is still at 11 mph. 

My setup is:
(2) 10000 mAh, 14.8v, 4 Cell lipos
(2) VESC 4.12
(2) Enertion R-Spec 

The VESCs are connected via CAN-Bus. Am I stuck with this speed unless I upgrade the battery or are there settings i can tweak in BLDC to get a higher speed?
```

---
## \#2 Posted by: ajaynagra Posted at: 2016-09-09T20:55:46.575Z Reads: 122

```
Dual motor = more torque.
```

---
## \#3 Posted by: Karmannghiagirl Posted at: 2016-09-09T20:56:03.799Z Reads: 120

```
Paint it red, right @longhairedboy?

really though, higher voltage = higher speed

Just because you added a second motor, the speed limit is based on the Kv of the motors (basically its RPM per volt) which is limited by the voltage of the battery. the second motor just gives you more torque, not more speed.
```

---
## \#4 Posted by: ajaynagra Posted at: 2016-09-09T20:59:22.639Z Reads: 119

```
This thread helps i think http://www.electric-skateboard.builders/t/figuring-out-range-and-speed-of-an-electric-longboard/202

Red wheels my friend , red wheels
```

---
## \#5 Posted by: Titoxd10001 Posted at: 2016-09-09T21:00:36.519Z Reads: 114

```
You need to connect your batteries in series or change gearing
```

---
## \#6 Posted by: cjoliver Posted at: 2016-09-09T21:05:34.778Z Reads: 114

```
You should look into a different battery for your setup, even in series your batteries would only support up to 30v and on a 192kv(guessing kv cause enertion) motor it's not a setup meant for speed
```

---
## \#7 Posted by: Titoxd10001 Posted at: 2016-09-09T21:12:50.592Z Reads: 106

```
I'm pretty sure you have your batteries in parallel and if you connect them in series you'll double your speed.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-09-09T21:20:42.454Z Reads: 98

```
Tuck a lot
```

---
## \#9 Posted by: treenutter Posted at: 2016-09-10T00:47:34.061Z Reads: 81

```
[quote="Titoxd10001, post:5, topic:9292"]
connect your batteries in series
[/quote]

This is it @nick.schweng - put those battery packs in series. Make sure to adjust the voltage settings in BLDC Tool accordingly. Check to make sure that you don't have a low ERPM limit set as well.
```

---
## \#10 Posted by: Pablo_702 Posted at: 2016-09-10T04:48:02.594Z Reads: 68

```
Whats the kv of your motors?
```

---
## \#11 Posted by: 2-alex-2 Posted at: 2016-09-10T07:34:18.233Z Reads: 55

```
Also your gearing would make a difference but up the voltage as well. I run a single 6364 245kv on 24v 6s lipo and have reached 27mph sofar with a little more throttle left to go.
```

---
## \#12 Posted by: kaziupir Posted at: 2016-09-10T10:05:03.422Z Reads: 46

```
You should use at least 8s at 190kv.
```

---
