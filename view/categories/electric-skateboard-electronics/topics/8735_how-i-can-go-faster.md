# How I can go faster?

### Replies: 24 Views: 6613

## \#1 Posted by: tueboard Posted at: 2016-08-31T23:24:49.013Z Reads: 403

```
hi,

my top speed is 27 kph on flat street, my weight is 73,8 kg and my setup is:

Enertion Mono Drive R-SPEC Pro Kit
http://www.enertionboards.com/diy-electric-skateboard-kits/enertion-single-motor-mount-pro-kit/

Enertion VESC standard

Enertion wheels 83mm

Enertion 12mm belt

2 lipo batteries in series Floureon 3S 35C 11.1V 5500mAh

BLDC tool motor config is

<img src="/uploads/db1493/original/2X/8/8782c297f40759b05cad58d6519bc59a05d8c41f.png" width="690" height="339">

How I can go faster with the same components and without burning the motor, vesc or other components?

i have to upgrade the batteries or something?

thanks
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-31T23:26:15.176Z Reads: 375

```
higher voltage batteries, tighter gearing, bigger wheels, higher kv motor would all make you go faster
```

---
## \#3 Posted by: Pantologist Posted at: 2016-08-31T23:27:27.897Z Reads: 371

```
You can could upgrade to 12S. That would be the easiest way.
```

---
## \#4 Posted by: tueboard Posted at: 2016-08-31T23:27:40.421Z Reads: 366

```
do you know if is possible to run faster with the same build and another BLDC-VESC config ?
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-31T23:29:57.540Z Reads: 353

```
no speed is limited by the factors stated above. It would only be possible if the VESC was being limited by eRPM
```

---
## \#6 Posted by: sl33py Posted at: 2016-08-31T23:35:54.722Z Reads: 346

```
No.  As @Jinra said it's set by the components.

Your voltage = RPM's on your motor (kv, so 190 rpm per volt).  Transferring those set RPM's (they drop as pack voltage drops too) to your wheels is your gearing.

So on the same settings, the best way to get more speed is to change your motor gear.  But your startup and hill torque will suffer for more top speed.

A better solution would be to add another battery in series.  So adding another 3s Fleureon battery for 9s would give you 33% more speed roughly.  

BOOM! (where's the mic drop emoji?)
```

---
## \#7 Posted by: monkey32 Posted at: 2016-09-01T03:36:03.885Z Reads: 297

```
Yea more speed will need a higher number of cells in series. 9 (+ 1x 3s lipo) or better 12s ( +2x 3s liposuction) will bump up voltage significantly. Hobby King is always having deals check their eu site.
```

---
## \#8 Posted by: Hummie Posted at: 2016-09-01T03:48:08.033Z Reads: 280

```
if you increase the battery max amps and then get more amps at high speed to get closer to his no load speed.  generally you don't draw many amps at high speeds and i haven't seen what would really be pulled at high speed but it makes sense to have more amps to get closer to the no load speed, which he isnt at yet.

but of course more cells is the way to go really.
```

---
## \#9 Posted by: tueboard Posted at: 2016-09-01T07:06:54.331Z Reads: 253

```
do you know if two of these are too powerful ? FLOUREON 13000mAh XT60 22.2V 6S 25C
http://www.ebay.es/itm/FLOUREON-13000mAh-XT60-22-2V-6S-25C-Lipo-Bateria-para-RC-Helicoptero-Truck-Hobby-/361543026919?hash=item542da4c8e7:g:c-oAAOSwYmZXH0un
```

---
## \#10 Posted by: Hummie Posted at: 2016-09-01T07:17:58.355Z Reads: 242

```
wow big.  you can never have a too powerful battery.  the bigger and higher c rating the better.
```

---
## \#11 Posted by: sl33py Posted at: 2016-09-01T17:04:58.755Z Reads: 231

```
Umm... each of these 13000mAh (13Ah) batteries is 1.8kg!  So 4lbs each.  288Wh each 6s battery...  

It's not a matter of too powerful - and the capacity does not give you more power, the voltage does (6s/9s/12s).  You'll get more range, but will adding 8lbs of batteries to your board be needed?

Figuring out range on two of these batteries (288.6Wh ea) = 577Wh/10 (10wh=1km) = 57.7km/35mi.  

add in the individual dimensions: 146*88*89mm - it's going to be tough to fit 90mm/3.5in under most boards and still clear the ground!

@miquelcamps - your original question was "how to go faster" - simple.  regear or add more batteries in series for more voltage.  More voltage doesn't require more capacity.  And you will want cells with the same capacity in series (usually all the same age is even better so they all have the same capacity over time). 

So, adding in an additional 3s 5500mAh 35c matching battery or two would give you 9s or 12s voltage.  It will also increase your range as higher voltage is more efficient and gives you more Wh.

2 in series for 6s (your current setup) = 122Wh (again 10Wh=1km so approx. 12.2km/7.5mi)
3 in series (adding one additional Fleureon 3s 5500mAh 35c) =  (Voltage x Ah = Wh) so 9s(3.7v x 9 = 33.3v).  33.3v x 5.5Ah = 183Wh (/10 = 18.3km/11.3mi)
4 in series (adding two additional Fleureon batteries) = 44.4v x 5.5Ah = 244Wh (/10 = 24.4km/15mi)

So more batteries in series also will give you additional range.  These are all rough estimates, so if you are a heavier rider, or going up hills, or accelerating really fast (racing) - you'll get less than the 10wh = 1km conversion.  But a good ballpark to start.

HTH - GL!
```

---
## \#12 Posted by: Mobutusan Posted at: 2016-09-01T17:43:08.425Z Reads: 203

```
Cheapest option = larger motor pulley ~$15
2nd cheapest option = 90 or 97mm flywheel clones ~$25-30

Otherwise, add batteries or change motor to higher kv = more costly.
```

---
## \#13 Posted by: sl33py Posted at: 2016-09-01T17:57:06.920Z Reads: 203

```
[quote="Mobutusan, post:12, topic:8735, full:true"]
Cheapest option = larger motor pulley ~$152nd cheapest option = 90 or 97mm flywheel clones ~$25-30

Otherwise, add batteries or change motor to higher kv = more costly.
[/quote]

agreed.  Running a speed calc w/ your settings (83mm - 190kv - 6s - 15/36) = 26kmh

So wheels would get you:
90mm = 29kmh/17mph
97mm = 31kmh/19mph

your 83mm setup on 9s = 40kmh/24mph
12s = 53kmh/32mph

If you decide to re-gear your motor pulley - you likely will need a larger belt too.  just to factor that cost in too.  probably another $10-15.
```

---
## \#14 Posted by: Mrmoonlight Posted at: 2016-09-01T17:59:31.107Z Reads: 185

```
How much more speed do you want?
```

---
## \#15 Posted by: tueboard Posted at: 2016-09-01T23:44:01.675Z Reads: 192

```
thank you everybody for your comments, i'm learning a lot of you :)

i've some questions about my specs and c rate.

**VESC specs**
5V 1A output for external electronics from the buck converter integrated on the DRV8302.
Voltage: 8V – 50V (Safe for 3S to 10S LiPo).
Current: Up to 240A for a couple of seconds or about 50A continuous depending on the temperature and air circulation around the PCB.

**Motor specs**
190KV
2400W
4-12S  (14 Volts - 44 Volts MAX)


1- what it means "Safe for 3S to 10S LiPo"? if i put 12s i can burn the VESC? someone tried to put 12s in the enertion vesc standard?

2- my motor max is 12s, but the vesc safe max is 10s, so the limit is 10s right?

3- @Hummie says "higher c rating the better", i know that it's better to choose another battery with the same c rating, mAh, etc, but i like the idea to have another 2 backup batteries and i see a lot of options out there 35C, 40C, 45C, 50C, 60C.. which is the limit for my motor-vesc specs?

I'm sorry if I'm asking a lot of questions, i've no idea about electronics...

thank you
```

---
## \#16 Posted by: sl33py Posted at: 2016-09-02T00:03:09.552Z Reads: 181

```
[quote="miquelcamps, post:15, topic:8735"]
VESC specs5V 1A output for external electronics from the buck converter integrated on the DRV8302.Voltage: 8V – 50V (Safe for 3S to 10S LiPo).Current: Up to 240A for a couple of seconds or about 50A continuous depending on the temperature and air circulation around the PCB.
[/quote]
Where did you get these specs?  everything except the 3-10s looks correct.  This might be to avoid too high of a KV motor on >10s?    (more below)

[quote="miquelcamps, post:15, topic:8735"]
1- what it means "Safe for 3S to 10S LiPo"? if i put 12s i can burn the VESC? someone tried to put 12s in the enertion vesc standard?
[/quote]
Actually the VESC can handle 12s, but it's pushing it depending on your motor.  @Chaka has a great "cheat sheet" of voltage to kv that work well.  What you want to avoid is exceeding 60k ERPM.  This can cause VESC DRV chip failures.  So conservatively i usually stick around 8-10s as this avoids a lot of problems.  The definite no-go is >200kv on 12s.  

[quote="miquelcamps, post:15, topic:8735"]
2- my motor max is 12s, but the vesc safe max is 10s, so the limit is 10s right?
[/quote]

You can run 12s with 190kv.  It should have ERPM of 57k so a bit of room before the recommended 60k max.  It's worth noting that you are at the limit of voltage on the VESC at 12s, so it's a good idea to be gentle when bench testing (i killed 2 DRV chips hammering hard start/stops on 2 different VESC's bench testing - not smart).

[quote="miquelcamps, post:15, topic:8735"]
3- @Hummie says "higher c rating the better", i know that it's better to choose another battery with the same c rating, mAh, etc, but i like the idea to have another 2 backup batteries and i see a lot of options out there 35C, 40C, 45C, 50C, 60C.. which is the limit for my motor-vesc specs?
[/quote]

It's all about amps - what the ESC and motor want vs what the battery can provide.  Your C rating gives you some simple math to determine the batteries constant amps it can provide, vs burst amps for a few seconds (usually 10 seconds).  AND it's marketing from the battery company, so i don't really believe them.  As a result - and from testing a dual VESC on 8s i saw 65A peak (likely only a few seconds) on my inline watt meter - i target batteries that "claim" 100A output.  So the formula to determine amps is simply the pack Ah x C.  Ex: Turnigy 3s 5000mAh 20c = 5Ah x 20 = 100Amps  If you go to a smaller capacity battery (like a 4500mAh nano-tech - just make sure you get a 20-25c battery).

[quote="miquelcamps, post:15, topic:8735"]
I'm sorry if I'm asking a lot of questions, i've no idea about electronics...
[/quote]

Good questions and a couple back at you.

**How fast do you want to go?**

**How heavy are you?**

**What kind of riding are you doing?  Commuting or cruising or racing - hills or flats?**

GL!
```

---
## \#17 Posted by: tueboard Posted at: 2016-09-02T00:21:09.565Z Reads: 153

```
[quote="sl33py, post:16, topic:8735"]
Where did you get these specs?  everything except the 3-10s looks correct.  This might be to avoid too high of a KV motor on &gt;10s?    (more below)
[/quote]

i get the specs from the enertion website.

How fast do you want to go? i'm just curious about the top speed that my setup can reach and see if is possible to overcome the boosted boards.

How heavy are you? my weight is 73,8 kg.

What kind of riding are you doing? Commuting or cruising or racing - hills or flats? Commuting/cruising on flat steets.

thank you so much for your answers :)
```

---
## \#18 Posted by: sl33py Posted at: 2016-09-02T17:58:08.176Z Reads: 154

```
Cool - good info.

Spec on Enertion's site.  Probably stating 10s max as the DRV will die if over 200kv on 12s.  So they are being conservative.  I really like 8-10s as well as it gives me some peace of mind and leeway vs running at the very edge of possible.  I also have several VESC's that are over a year old w/o issue.  Likely since i don't push the envelope (no FOC, no 12s (yet)).

How fast you want to go.  If Boosted is your benchmark (it's a good one - great board besides range) then you want 22-25mph/35-40kph.  That's easy to reverse in any speed calc software to get what your gearing or voltage needs to be to reach this.  And i usually target a top speed of 25mph as well.  Plenty fast for me (usually too fast, but every once in a while you want to go just a little faster...).

With your weight a  single motor is plenty, so it's not restricting your top speed.  Your voltage and gearing (and motor KV) are.  Being on the flats and cruising vs racing - unless you want to get to your top speed faster - a second motor is overkill, expensive, and complexity you likely don't need.  You can add it later if you change your mind.

So back to your top speed need.  If you simply add one more 3s battery (matching your current one exactly (same brand, capacity, c rating, etc.)) - 83mm - 190kv - **_9s_** - 15/36 will get you to **40kph/24mph**.  Headwind/tailwind will affect the top speed, but that's as fast or more likely faster than boosted.  Top speed - if you are "racing" a Dual+ boosted, with dual motors they likely will out accelerate you off the line.  Just more torque w/ dual motors.

So again the simple "fix" for more speed is more voltage.  Go to 9s from 6s and you're set.
```

---
## \#20 Posted by: tueboard Posted at: 2016-09-03T19:40:43.502Z Reads: 148

```
thank you so much i will follow your advice
```

---
## \#21 Posted by: monkey32 Posted at: 2016-09-04T10:10:23.100Z Reads: 147

```
I saw two Evolve GTs out on Mazanares this morning- my apt looks out on the green bridge. Great time to ride.......I am in the process of swapping out my current runnning drivetrain to a different board... it should be ready by next weekend if you are interested in a meetup.
```

---
## \#23 Posted by: Nstroh Posted at: 2018-05-27T18:09:54.339Z Reads: 60

```
Hey so i have 83mm 9s and 270kv motors and its geared 35/16 and i am only going 15mph.
```

---
## \#24 Posted by: Sn4pz Posted at: 2018-05-27T20:48:55.627Z Reads: 55

```
you should aero tuck :laughing:

![image|450x300](upload://a1uZPzXnZIrfoGh17tQ6G3amvQS.jpg)
```

---
## \#25 Posted by: professor_shartsis Posted at: 2018-05-27T21:13:40.397Z Reads: 49

```
[quote="Nstroh, post:23, topic:8735, full:true"]
Hey so i have 83mm 9s and 270kv motors and its geared 35/16 and i am only going 15mph.
[/quote]

what kind of controllers and settings are you using? it should be able to go ~35mph on flat ground...

to only go 15mph top speed with that gearing i think it would need to be an issue involving extremely low battery current (less than ~5a battery current per motor) or steep hill.
```

---
## \#26 Posted by: Tomer Posted at: 2018-05-27T21:24:09.876Z Reads: 45

```
I recently switched from 80mm Orangatang Kegels to 100mm MBS All-Terrain wheels.
From 43km/h I reached to 47km/h, not such a significant change in my opinion. 
I expected much higher numbers to be reached.
```

---
