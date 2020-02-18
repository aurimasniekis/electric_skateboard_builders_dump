# VESC question? I have no idea what Im doing :)

### Replies: 15 Views: 1552

## \#1 Posted by: mmaner Posted at: 2016-12-19T22:02:39.574Z Reads: 103

```
I have the following setup...
[DIY VESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)
[TB 6355 260kv motor](diy-electric-skateboard-kits-parts/6355-260kv-epower-motor/)
[ZIPPY FlightMax 8000mAh 3S1P 30C LiPo Battery x2](https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html)

I am running at 6S, just wanna use BLDC mode to keep it simple.  Any idea what voltage limits I should use in the in the BLDC tool?
```

---
## \#2 Posted by: sl33py Posted at: 2016-12-19T22:10:10.351Z Reads: 99

```
I've typically just run the defaults unless i was getting an error when braking from regen.

Are you wanting to have the VESC limit voltage when your batteries hit 3.4/5/6v?  I prefer an audible buzzer and they are super cheap insurance.
```

---
## \#3 Posted by: flatsp0t Posted at: 2016-12-19T22:15:05.627Z Reads: 99

```
Leave MIN and MAX Input voltage at their default values(8V and 53V), change "battery cutoff start" to 21V and "battery cutoff end" to 19.8V
```

---
## \#4 Posted by: mmaner Posted at: 2016-12-19T22:16:15.424Z Reads: 98

```
I just assumed I'd have to do some programming, and I am not really understanding enough from the tutorials I am finding to feel confident.  I read [here](http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980), and its full of great info but not the Voltage Limits I need or info about the specific motor I am running.  I went to http://vesc.net.au and watched the tutorials, once again nothing specific about my setup or 6S at all really.  I used this table from @paul775 ...
<img src="/uploads/db1493/original/3X/2/0/200647bf1b03668113e1e975fa4678d88df08dd0.png" width="586" height="196">
...but I'd like to be sure as its kind of old.
```

---
## \#5 Posted by: mmaner Posted at: 2016-12-19T22:16:46.885Z Reads: 88

```
Cool, Ill give it a go :)
```

---
## \#6 Posted by: mmaner Posted at: 2016-12-19T22:21:59.998Z Reads: 82

```
This is a screen shot from the [DIY Tutorial](https://www.youtube.com/watch?v=dxDXUrk-7ek)...
<img src="/uploads/db1493/original/3X/5/a/5aa7143d649e970fffb5601d00e86f1778f5ec2c.jpg" width="415" height="268">

It shows...
Motor max:  40 A
Motor min (regen):  -30 A
Battery max:  25 A
Battery min (regen):  -10 A
Absolute max:  130 A

My defaults are...
Motor max:  60 A
Motor min (regen):  -60 A
Battery max:  40 A
Battery min (regen):  -20 A
Absolute max:  130 A

Seems like a pretty large spread, where should I be?
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-12-19T22:26:06.845Z Reads: 79

```
That highly depends on your setup. in general, I would try it with the lower settings(DIYs), and if you need more braking force or power, you can adjust them.
```

---
## \#8 Posted by: sl33py Posted at: 2016-12-19T22:43:48.200Z Reads: 76

```
21v / 6 = 3.5v
19.8v / 6 = 3.3v

Personally i think those are way too low.  I typically stop at 3.7/3.6v or so.  Figuring sag will potentially pull them a little lower under load.  I don't want to damage or over-draw my batteries, which i know impacts long-term life.

My .02
```

---
## \#9 Posted by: Namasaki Posted at: 2016-12-19T22:54:52.132Z Reads: 73

```
IMO, 25a for Battery max is too low, especially at 6s. Your battery can handle 240a continuous so no worries there.
Assuming your doing a single drive setup, I would do:
 Motor max at 60
 Motor Min -30 or maybe more if the brakes are not strong enough.
 Battery Max  60
 Battery Min  -20 depends on what charge rate your battery can handle. Max charge rate on your batteries is 5c. That's 40a This setting will also affect brake power.
```

---
## \#10 Posted by: mmaner Posted at: 2016-12-19T23:01:12.126Z Reads: 70

```
I've got it running, but both my nano and gt-2b remote are crazy now.  I have about 1/4 inch that is nothing and then full throttle.  I tried playing with he pulse width while watching the pulswidth display, but all it did was move where the 1/4 inch is in the total travel of the trigger.  Anyone else have that issue?
```

---
## \#11 Posted by: Namasaki Posted at: 2016-12-19T23:02:51.543Z Reads: 71

```
SL33PY is right! You have to be careful with Lipo batteries. Don't take them down too low or you will ruin them.
The chart that you posted is for Li-ions which can go lower than Lipos.
Once I ruined a brand new set of Lipos because I took them too low one time.
If you use voltage alarms on both packs, you can set the alarm at 3.4.
If you depend only on the vesc to monitor, then you will have to set the cut off higher because your cells will not deplete evenly and you could have one or more cells drop too low by the time the vesc cuts off.
```

---
## \#12 Posted by: Namasaki Posted at: 2016-12-19T23:06:39.047Z Reads: 67

```
Here is a great tutorial on how to calibrate your remote controller with the vesc.
https://youtu.be/OtuofrQr3F8
```

---
## \#13 Posted by: mmaner Posted at: 2016-12-19T23:14:45.758Z Reads: 64

```
I was actually watching that when you replied.  I still dont have an answer though, It may resolve itself under load, it just feels like there's only 1/4 inch of travel that actually does anything.  Im about to mount everything and give it a try, ill post back in a few.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2016-12-19T23:19:53.649Z Reads: 64

```
Just don't think in amps because it is always depended on your battery's voltage.
I think it is easier if you think about in watts. You have lipo batterys so they will be around 3,7V under load for each cell officially. Li-ion are 3,6V.
So the maximum power output at 40A for "Battery max" would be 6S * 3,7V * 40A = 888 Watts. And if you have dual drive (2x motors, 2x VESC) you would have double 888 * 2 = 1776 Watts.

Now it depends if you are a beginner, inermediate or experienced Longboard or skateboard rider.
For beginners i would recommedn 250 Watts just to get used to it. Then maybe 700 till 1000 Watts for intermediate which will give you a lot of fun for a while. At 1500 the real fun begins. And at 2000 watts you need to concentrate when you pull the throttle fully. I weigh around 80 kg with clothes + helmet (<-fucking important). So if you weigh 100 kg (25%more) calculate those values by that factor.
And motor max should never be lower than battery amps. And the motor amps handle mainly the power delivery at slow speed. So the higher the motor amps the more power you have at low speeds and startup.

Hope that gives you a rough overview about the amp settings.
```

---
## \#15 Posted by: mmaner Posted at: 2016-12-20T00:58:49.848Z Reads: 55

```
@Ackmaniac Very nice information.  I read through it, but am still looking for threaded inserts :) so Ill read it again in a bit.  

@Namasaki The remote seems to fine under load.  Its not great as the top half of the travel is still useless, but its usable.  Im not gonna worry too much about it, still waiting on 1 of the  benchwheel remotes I ordered to get her.
```

---
