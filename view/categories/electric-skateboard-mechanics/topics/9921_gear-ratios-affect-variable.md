# Gear ratios affect variable

### Replies: 11 Views: 1389

## \#1 Posted by: NewbieBoardBuilder Posted at: 2016-09-21T03:13:27.131Z Reads: 163

```
Hey guys, I'm pretty new to all the electric building, so I don't know many sources to check. I was wondering how gear ratios can affect speed, acceleration, and torque. Also, should wheel size be chosen off of your gear ratios to balance out the torque, acceleration and speed? I know y'all are a great help. Thanks
```

---
## \#2 Posted by: rodriguejoe1 Posted at: 2016-09-21T03:40:45.237Z Reads: 159

```
http://toddy616.blogspot.ca/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2016-09-21T03:42:12.716Z Reads: 150

```
Thanks, but I wasn't looking for a calculator. I wanted to know how gear ratios affect torque acceleration and speed😕
```

---
## \#4 Posted by: saul Posted at: 2016-09-21T04:13:55.794Z Reads: 151

```
A bigger ratio give more torque **and** less top speed.


----------

say a hub motor has a ratio of 1:1 so very fast (40mph) but not crazy acceleration.

a standard belt drive has 16/36t = 1:2.25, so 2.25 X the torque of a direct drive, but less top speed. see calculator.

on my build going from 16/36 to 14/36 = 2.57, better for hills and acceleration, abot 3-4 mph slower max.
```

---
## \#5 Posted by: cryzies Posted at: 2016-09-21T05:11:09.850Z Reads: 142

```
Not only gear ratios affect speed, acceleration, and torque. Don't forget everything about the motor will, motor width, 50mm vs 63mm. Motor length 54mm vs 64mm vs ~74mm. KV rating of the motor. Then you have the ESC which can control the voltage to the motor. Then you have the actual batteries themselves, cell count, voltage sag, amperage. Then wheel size, wheel surface area.

But for your question, gear ratios, you trade off between higher top speed lower torque/acceleration and lower top speed and higher torque/acceleration. 

What build is best? We definitely need your desired results to figure that out, the environment as in how hilly you'll be skating around, and the rider's weight.
```

---
## \#6 Posted by: sl33py Posted at: 2016-09-21T05:49:15.722Z Reads: 136

```
Yes, you are looking for a calculator.  It's going to be a swap between speed and torque.

Use a calculator.  Plug in your setup.  My example for you will be a really vanilla one using Enertion's typical:

83mm (flywheel or clone) - 190kv (RSpec example) - 8s (safe starting setup) - 15/36 (motor/wheel gearing):

My calc vs RC Calc is pretty close.  22-26mph top speed.  5400-6300 rpm.  According to Benjamin Vedder the sweet spot is around 8600 rpm (someone correct - this is from memory).

to your point - this is a gear reduction of 2.4:1.  The higher the ration (i usually top out around 3:1) - the better the startup accel and torque, with less top speed.  I also target a top speed of 25mph.

Maybe clarify what you're trying to accomplish.  How heavy are you, how steep of hills do you want to climb (or flats?), and how fast do you want to go?

HTH - GL!
```

---
## \#7 Posted by: NewbieBoardBuilder Posted at: 2016-09-22T21:18:58.730Z Reads: 104

```
Thanks for the great help. I'm writing a presentation with a compilation of basic facts, diagrams, and pictures for the beginner builders like me.
```

---
## \#8 Posted by: NewbieBoardBuilder Posted at: 2016-09-22T21:34:09.760Z Reads: 104

```
How do the number of teeth on a belt affect the gear ratios and the boards overall torque, acceleration, and speed?
```

---
## \#9 Posted by: sl33py Posted at: 2016-09-22T23:33:18.401Z Reads: 105

```
run a calculator and do the math if you want exact ratios.

i usually see 3mm wheel difference equals about 1-1.5mph increase/decrease.  Pretty linear (as you'd expect).  the voltage makes the biggest difference, with 6s to 12s = 2x the speed (also as expected).

this is good 'ol transmission and differential gearing equations.  What we don't' usually have is actual torque output in ft lbs or similar.  No idea how to get that unless you are going to Dyno your esk8!  (someone do it for science!)
```

---
## \#10 Posted by: makevoid Posted at: 2016-09-23T00:01:12.658Z Reads: 103

```
according to the code I found on the calculator @rodriguejoe1 linked to you (I translated that code from JS to ruby), you can see at this line (original HTML page code line 742), or on my code at [this line here](https://github.com/makevoid/esk8-calc/blob/master/app/calc.rb#L31)... there's something similar to this "simple" formula:
    
 
    top_speed_km_per_hour = motor_rpm * wheel_size_in_mm * Math::PI * gear_ratio

(this is actually valid code #ruby_ftw ^^)

You derive `motor_rpm` from the motor KV and the voltage you are running, `Math::PI` is always π and `gear_ratio` you get it from your pulley teeths. That altogether gets you the (theoretical max) top speed.


original code (JS in HTML page line 742):

    var topspeedMPH = motorRPM * gearWheelSize * 3.1415926535897932 * 0.00003728226 * gearRatio;


^^
```

---
## \#11 Posted by: mm6ix Posted at: 2016-11-24T18:10:38.656Z Reads: 73

```
What is the "0.00003728226" value in the top speed calculation ?
```

---
