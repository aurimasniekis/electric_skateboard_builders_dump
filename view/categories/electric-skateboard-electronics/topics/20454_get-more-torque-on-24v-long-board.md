# Get More Torque on 24V long board

### Replies: 29 Views: 1834

## \#1 Posted by: shaohad Posted at: 2017-04-06T18:18:36.526Z Reads: 163

```
Hi guys.
im runing long board with single pulley motor.
turnigy SK3-6374-192KV
runing 16mm 15T timing belt
7S3P 24V 18650GA 3C battery pack
VESC 50A
2.4GHZ remote controll

BLDC TOOL settings
<img src="/uploads/db1493/original/3X/9/5/95b0444c610506b37b5689bfa3c1727f034b9eef.jpg" width="690" height="200">

right now while im riding flat serface it has no problem, but with a small hill it just wont take me.
any ideas how buff up the toruqe without change motor, vesc or battery??
thanks in adanced,
```

---
## \#2 Posted by: Blasto Posted at: 2017-04-06T18:24:34.076Z Reads: 147

```
Post your vesc settings
```

---
## \#3 Posted by: shaohad Posted at: 2017-04-06T19:20:47.218Z Reads: 137

```
done upload picture with the settings
```

---
## \#4 Posted by: Stef Posted at: 2017-04-06T19:22:22.584Z Reads: 139

```
At 24V your Vesc can only provide 1200W to your motor, which is equivalent to the max performance of a 5055mm motor. Your 6374 is capable of much more than that, but youll have to increase the voltage of your battery. Also 3C battery means you can only provide 3*(Ah) Amps, which is likely less than 30Amps, which is quite little, you probablyexperience a lot of voltage sag which further decreases motor performance.

Edit: With 30A motor max, your max motor power is only 720Watt, less in practice, and voltage sag makes it even lower.
```

---
## \#5 Posted by: Hummie Posted at: 2017-04-06T19:50:43.785Z Reads: 125

```
Your battery can only do 30 amp continuous and you're running a low voltage so ultimately low power possible as said. Setting the battery max at 30 makes sense although you coul Likely kick it up a bit as those cells are rated to take bursts at a higher current.  The motor amp limit ...160!!  There's no reason I've found not to an will give you much more power yet still keep the battery under its limits set in the battery amp
Limit.
```

---
## \#6 Posted by: shaohad Posted at: 2017-04-06T19:52:44.668Z Reads: 118

```
i didnt understood did you recommend change nay of the settings?
if you did , change what?
i want the board to be light weight as possible.
```

---
## \#7 Posted by: Blasto Posted at: 2017-04-06T19:59:12.949Z Reads: 118

```
did you perform a motor detection? those seem to be the default values

anyways... perform a motor detection

and set 
motor max 60A
batt max 30A
batt min -12A

please don't put your motor max to 160A
```

---
## \#8 Posted by: Hummie Posted at: 2017-04-06T20:00:16.856Z Reads: 108

```
i was told on vedder's forum that the sensor is good to 160 amps.  Is there a reason not to do 160 motor?
160 motor will still, at max load and throttle, only possibly be a true 30 amps if that's what the battery amp is set to.   with the way the escs use pwm it's possible to give much higher amperage (160 in this case) but only for fractions of a time period and the motor and battery effectively are seeing the real battery amp number after it is smoothed out throughout the whole period and through the inductance of the motor...and maybe the battery wires.
```

---
## \#9 Posted by: saul Posted at: 2017-04-06T20:05:00.308Z Reads: 108

```
Safety margin.

Running at Max spec is bad practice...
```

---
## \#10 Posted by: PXSS Posted at: 2017-04-06T20:05:33.883Z Reads: 105

```
Batt min: -15
Batt max: 30
Motor min: -60
Motor max: 120
Absolute max: 150

Min eRPM: -60000
Max eRPM: 60000

Min input voltage: 8V
Max input voltage: 57V

Battery Cutoff start: 21
Battery Cutoff end: 19.6

E: I personally have my gfs motor max at 75A but she only weighs 115lbs
I weigh 145 and run mine at 95A but I like to carve a lot and often hit full throttle to accelerate fast even though I dont ride fast.
```

---
## \#11 Posted by: Hummie Posted at: 2017-04-06T20:12:27.831Z Reads: 99

```
if the power is available why not have access to it.   It's like getting a fararri and then putting a limit on the motor otherwise.  Maybe that's wanted but I've been looking for a reason not to do 200 motor amps, and there is one, but not 160.
i dont get the absolute max variable.  seems redundant and I assume its the motor amp limit really as well, meaning highest current even for a fraction of the
```

---
## \#12 Posted by: shaohad Posted at: 2017-04-06T20:22:39.818Z Reads: 96

```
i'll run some test and try again.
anways i'll consider upgrade voltage and battery dicharge rate, again i just want to keep the board low weight 
and i dont really want to ride fast
```

---
## \#13 Posted by: PXSS Posted at: 2017-04-06T20:28:49.002Z Reads: 92

```
Starting to sound a lot like Devin...
I would never use 160A as my limit because I do not feel comfortable with that kind of torque beneath my feet. 
At 100rpm that is 600 lb-in of torque, that means accelerating from 0.36 mph to 26 mph in under half a second. That is stupid. And I was being extremely conservative with my numbers as in factor of 10 conservative...
```

---
## \#14 Posted by: Hummie Posted at: 2017-04-06T21:24:15.211Z Reads: 88

```
maybe a hub motor will benefit much more from upping the motor amp limit as it's running at a  much lower rpm than a pulley setup.   at 100rpm I'd be at a faster speed.    for me it's not stupid but a much better performer.  I dont know how you came up with 600 ft/lbs of torque but for me at 200 motor amps and 48 battery I have a good solid acceleration from 0 dead still and I'm very comfortable pulling the throttle fully.  
none the less, you're bringing another element into the equation, being able to stand on it,  but 160 motor amps from what I read shouldnt be any more of a burden on the motor or esc really.  It just comes down to if you want that power at low speed.  I definitely appreciate it.
```

---
## \#15 Posted by: Hummie Posted at: 2017-04-06T21:52:33.068Z Reads: 84

```
wait a second, I dont know how you're getting the torque number, which is insanely high and a typical 63 outrunner might put out less than a twentieth of that,  but regardless of what the motor amps are set to the battery amps are the REAL amps so it's still going to be a maximum of 30 amps at the 22 volts...and 660 watts.  you'll get 660 watts maybe at 160 motor amps with the 30 battery amps.   upping the motor amps just ALLOWS YOU  to actually get those max battery amps at low speed/duty cycle.
```

---
## \#16 Posted by: PXSS Posted at: 2017-04-06T22:40:42.542Z Reads: 80

```
Power = torque x angular velocity 
700W = X * 2pi/60 * 100 (rpm)
X = 66.87N-m
66.87 Nm = 591.92 lb-in

I know how the limits work. Thanks

Reread the units I posted 
Ft/lbs is not a unit of torque
```

---
## \#18 Posted by: shaohad Posted at: 2017-04-14T18:16:48.348Z Reads: 65

```
i have this remote controll 
<img src="/uploads/db1493/original/3X/2/3/23c9f52229c3f01a7af4deb66e22c15fb2e2d5d8.jpg" width="666" height="500">

did anyone use this remote?
the throttle on my board is not consistent, it can kick to much tourqe or stuck onto same speed without let me break, or even sometime just wont respond.
any idea how do i solve it?
and there is a good way to make the accelaration more stable and easy?
thanks in advanced
```

---
## \#19 Posted by: EssEnn Posted at: 2017-04-16T14:35:59.723Z Reads: 63

```
I had one of those remotes, its the Wining remote, search the forums to confirm but I think those remotes are just dangerous. Threw me off my Mountain board a number of times, would cut out and then go full throttle, just jam on full breaks. This was all in the first 10 mins. The thing went straight into the bin. 

Get the Mini remote (look it up on the forums, a number of people sell them), its rock solid, never drops out and not expensive
```

---
## \#20 Posted by: JLabs Posted at: 2017-04-16T14:40:30.146Z Reads: 59

```
:wink:  https://electric-skateboard.market/product/2-4ghz-mini-remote-receiver/
```

---
## \#21 Posted by: shaohad Posted at: 2017-04-16T15:37:23.349Z Reads: 55

```
Its too big
anyone about remote in simillar size as the one i posted
```

---
## \#22 Posted by: Hummie Posted at: 2017-04-16T15:46:56.582Z Reads: 55

```
I've heard the benchwheel remote is good and it's smaller.  
The attraction of small can go out the window in many ways.
```

---
## \#23 Posted by: shaohad Posted at: 2017-06-02T10:57:49.463Z Reads: 42

```
hi guys so i have follow those specs:
Batt min: -15
Batt max: 30
Motor min: -60
Motor max: 120
Absolute max: 150

Min eRPM: -60000
Max eRPM: 60000

Min input voltage: 8V
Max input voltage: 57V

Battery Cutoff start: 21
Battery Cutoff end: 19.6

the board have a lot of torque but it only hiting around 25 km/h top speed.
and way i can raise it?
thanks in advanced
```

---
## \#24 Posted by: Tuomalar Posted at: 2017-06-02T11:03:31.906Z Reads: 40

```
What is your gearing and wheel size?
```

---
## \#25 Posted by: shaohad Posted at: 2017-06-02T15:17:19.136Z Reads: 32

```
[quote="shaohad, post:1, topic:20454"]
runing 16mm 15T timing belt
[/quote]

runing 16mm 15T timing belt  (all the informaion in the start of the thread)
83mm wheels
is there a way to solve this with programming the vesc?
```

---
## \#26 Posted by: Tuomalar Posted at: 2017-06-02T15:35:19.552Z Reads: 31

```
15T timing belt doesn't say anything. I think you mean 15T motor pulley 16mm wide? And what is your wheel pulley? 

I don't think you can get more speed by changing vesc settings.
```

---
## \#27 Posted by: shaohad Posted at: 2017-06-02T15:50:20.406Z Reads: 30

```
36T HTD5 from diy electric skateboards
and 15T motor pulley 16mm wide
```

---
## \#28 Posted by: Tuomalar Posted at: 2017-06-02T16:47:17.809Z Reads: 31

```
You still use 7s? If so you need more cells
```

---
## \#29 Posted by: shaohad Posted at: 2017-06-02T17:05:39.413Z Reads: 30

```
yes still 7s, prefer stay with small slim battery.
```

---
## \#30 Posted by: Tuomalar Posted at: 2017-06-02T17:43:03.864Z Reads: 26

```
Then bigger wheels or different pulley ratio
```

---
