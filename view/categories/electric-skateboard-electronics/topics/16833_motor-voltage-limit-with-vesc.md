# Motor Voltage Limit with Vesc

### Replies: 23 Views: 2783

## \#1 Posted by: IsTalo Posted at: 2017-01-28T22:23:33.058Z Reads: 191

```
Hi, I have a 4260 Alien Motor, That suport Max 6s Batteries, but everywhere I read I see someone saying To use 12s with Vesc, Wouldn't It burn my motor?
And this 300kv motor can handle my weight? I'm like 55 Kg
```

---
## \#2 Posted by: mmaner Posted at: 2017-01-28T22:28:02.265Z Reads: 191

```
The ERPM limit stops u from using 260kv or 300kv motors with anything over 6s.  It'll burn up the VESC.
```

---
## \#3 Posted by: IsTalo Posted at: 2017-01-28T22:45:32.606Z Reads: 188

```
Oh, cool, do you think 300kv can handle my Weight?
```

---
## \#4 Posted by: mmaner Posted at: 2017-01-28T23:47:44.818Z Reads: 177

```
I don't think 300kv will give u much torque, you will definitely have to kick off.  Maybe dual 300kv, but even then I don't know.  I have a board with dual 280kv and it's fun but I have to kick a lot, especially up hill.
```

---
## \#5 Posted by: IsTalo Posted at: 2017-01-29T08:30:51.760Z Reads: 157

```
Lol, so just Kv matters in a Skateboard motor? Because mine have like 1500w, like an Dual Boosted Board
```

---
## \#6 Posted by: mmaner Posted at: 2017-01-29T22:35:38.325Z Reads: 139

```
I'm just giving u my experience.  I like 190kv on 10s and 260 on 6s, lots of torque and high speed.  Speed without torque mens a lot of pushing.  

I wouldn't use 300kv, doesn't mean you 'cant', just means it's a waste of money if you end up having to upgrade to increase performance.
```

---
## \#7 Posted by: LukeL Posted at: 2017-01-29T23:05:59.037Z Reads: 135

```
There's some dispute to whether lower kv means more torque

http://www.electric-skateboard.builders/t/does-lower-kv-really-mean-more-torque/4529/2
https://www.rcgroups.com/forums/showthread.php?1096719-Mythbusters-Lower-KV-more-torque

I think it's more likely the size of the motor that matters (but higher kv motors are usually smaller anyway)

the power rating will matter as it will limit the max motor current for your system voltage (and torque is proportional to motor current

your motor seems a bit small compared to what most people are using, i'm using an alien 6374 240kv 10S and weigh 80kg it has enough torque to get me up pretty steep hills
```

---
## \#8 Posted by: IsTalo Posted at: 2017-01-29T23:57:52.141Z Reads: 121

```
Yes, I think I'll Buy Another One, but you know, they are not cheap, especially for me that in Brazil one Dólar is like 4 Reais (Brasil Money)... I between Sk3 and Enertion Ones
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-01-30T04:56:08.925Z Reads: 110

```
I have a 270kv motor on 12s, it does work. But I have 4:1 gears which makes the wheel pulley huge it will only fit 97mm wheels. Even then it's close to the ground. You have to set ERPM max to 60k though. 

I have heaps of tourqe. But I would prefer lower KV and smaller wheel pulley.

Motors are limited by amps not voltage, overheating is the thing to watch out for.
```

---
## \#10 Posted by: Vieo Posted at: 2017-01-30T15:34:16.949Z Reads: 102

```
I use 4260 Alien Motor (300KV) and I'm about 55KG in weight. I use 2x ZIPPY Flightmax 3000mAh 3S1P 20C to make a 6S pack. And for my weight it has a fair amount of torque and top speed around 18mph
```

---
## \#11 Posted by: IsTalo Posted at: 2017-01-30T15:36:09.710Z Reads: 93

```
Oh 'Man, Thats is really great. Do you use Vesc? And tell, It can go fast?
```

---
## \#12 Posted by: Vieo Posted at: 2017-01-30T15:42:06.751Z Reads: 88

```
Not yet, I'm using some cheap RC ESC. 

It goes pretty fast for me 18MPH (28KPH) - I think my weight helps a lot
```

---
## \#13 Posted by: IsTalo Posted at: 2017-01-30T16:05:22.551Z Reads: 84

```
Yeah, I'm 50Kg too
```

---
## \#14 Posted by: Theshiatispimpin Posted at: 2017-02-03T16:29:45.473Z Reads: 77

```
What about 12s? Im running 2 6s 5000mah lipo at 40c and cant decide what motor. the 190kv or 240kv or in between
```

---
## \#15 Posted by: mmaner Posted at: 2017-02-03T16:33:08.795Z Reads: 79

```
I think the max you can run on 12s is 190KV.  I may be wrong about that, but as I understand it...

8600 / MAX Voltage = MAX KV so in your case 8600 / 44.4 = 193.69KV

Let some people here that are better versed in VESC math and configs double check that.
```

---
## \#16 Posted by: Theshiatispimpin Posted at: 2017-02-03T18:44:44.138Z Reads: 88

```
What is 8600 mean?

So on the motor specs where it says voltage your batter has to match that?

for example

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
says 10-12s

2 of these 
https://hobbyking.com/en_us/turnigy-5000mah-6s-40c-lipo-pack.html 
would be 12 s

Would it just be safer for me to use 10s setup?
```

---
## \#17 Posted by: mmaner Posted at: 2017-02-03T18:57:41.908Z Reads: 81

```
To find your Max KV use the following formula
  8600 / MAX Voltage = MAX KV

8600 = Max RPM 
To find the Max RPM use the following formula
  Max Voltage * KV = RPM
In your case...
  44.4v * 193.69kv = 8599.836 RPM > rounded up = 8600

Another way to look at it is Max Voltage
  8600 / Motor KV = Max Voltage
In your case...
  8600 / 192kv = 44.79v

So assume you were going to use a 240 KV motor, using the formula above...
  8600 / 240 kV = 35.83
So the Max Voltage for a 240kv motor is 10s or 37v

I am too scared to use 12s, the tolerances are too tight, and I don't think there's much of a performance boost...at least not for how I ride.  If you want to be really safe, use a 6s battery pack.  If you want to be pretty safe and leave yourself some room use a 10s battery pack.
```

---
## \#18 Posted by: PXSS Posted at: 2017-02-04T01:33:27.554Z Reads: 76

```
The VESC should be limited to 60k erpm or you might blow it. This is the rpm * pair of poles in your motor. Most motors have 14 poles (7 pole pairs)

That's why your RPM limit is ~8600
```

---
## \#19 Posted by: Ingvarjedi Posted at: 2017-06-16T12:40:37.849Z Reads: 61

```
Hi People
Whats best motor Turnigy SK3 62mm 192kv 12s or 240kv 10s?
```

---
## \#20 Posted by: IsTalo Posted at: 2017-06-16T16:43:26.276Z Reads: 58

```
Depends, one you have more torque and other more speed, but just one works with 10s and Vesc, the 192 one, because there is a erpm limit... Read More
```

---
## \#21 Posted by: Ingvarjedi Posted at: 2017-06-16T17:16:24.307Z Reads: 57

```
Other motor do's not work with VESK?
```

---
## \#22 Posted by: IsTalo Posted at: 2017-06-16T17:21:31.116Z Reads: 60

```
Read about the Erpm limit, if you pass 60k your DVR will burn
```

---
## \#23 Posted by: Aggdaddy Posted at: 2017-06-16T17:36:19.070Z Reads: 56

```
I have a mountainboard that came with a 300kv motor and a 10s battery.  Before I knew what I know now, I was able to get it to run on dual vescs.  Ran good and scary fast.  Brakes were decent, but you'd have to give the board a little nudge forward with your hips to get it to go.  So it was dual non-sensored 300kv motor.  I think I got up to around 26mph, before it seemed too scary.  Loved playing with the cyclists. muwhahaha, but unfortunately it didn't last long.  One of the vescs decided to not start up one day and it was broke until I switched out all of the electronics.   

I think I had that erpm set at the default 100000.  Didn't know any better, but once it got going, it had the torque to make it up the steep inclines in the park.

Now, Using the same gearing with a torqueboards 12 esc and 6355 190kv motors and 10s battery, it has the torque after you nudge it, (non-sensored ESC) but nowhere near the top-end speed I was getting with the 300kv motor and vesc.

I might try the vesc again with this set up.  I will have sensored starts and maybe better brakes) I still have two vescs (one warranty repair and the other unused since the other one failed.), but they are Flier (chinese company) brand vescs.  Not sure how long they will last even if I configure them better than last time.
```

---
