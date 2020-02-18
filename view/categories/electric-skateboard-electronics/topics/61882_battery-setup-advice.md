# Battery setup advice

### Replies: 4 Views: 143

## \#1 Posted by: Teo Posted at: 2018-07-15T02:26:37.539Z Reads: 56

```
Hi Everyone!
Looking for some advice on how to setup my new battery pack. I currently have on my board a zippy compact 5s lipo 4500mah 35C continuos discharge (157 continuos amps at full throttle and over 200 amps - 45c - for bursts) which gives me 12km of range and 36km/h top speed. I'm 60kg, using street wheels, 260kv motor and 16T to 36T ratio.

I have now bought 21 Samsung 18650 30Q because I was planning to do a 7s 3p setup to increase range and top speed but I'm getting some doubts about the performance I can expect from this pack. From my understanding, since I have a higher voltage pack (passing from 5s to 7s) I should get the same performance with lower amps (P=V*I). This 7s pack should deliver up to 60amps (being a 3p) which is anyways what the vesc was limiting the current at even in the previous setup. This being said, I was expecting to get:
-higher top speed and acceleration given the higher voltage (same current, higher voltage --> higher power)
-at least doubling the range since I have 9000mah capacity (3x3000mah) and 40% higher voltage.

Now, reading more about it I'm starting to get worried about the amps you can get from a 3p setup and wondering if:

A) would I be stressing the batteries too much and (or) even just not get good performances out of it?

B)should I use the 21batteries I have (leaving one out) for a 5s4p setup to increase withdrawable current? I know I'd be reducing the voltage but the current set up I have with the current  5s lipo is already a beast... It starts uphill and accelerates fast without pushing (without getting hot!) Just not sure I can compare performances of lipo and 18650 just simply looking at voltage, capacity and amps. BTW this setup is very tempting also because I could skip the BMS and keep on using my charger.

Any advice or experience you had will be very helpful! I'd love to avoid having to set up the battery pack and take it apart several times to try all the combinations :joy:
```

---
## \#2 Posted by: E1Allen Posted at: 2018-07-15T03:01:31.574Z Reads: 46

```
@teo I use the same gearing on a 190kv motor.  If you did 7 or 6s4p it would be fine on the batteries.  You can still do 7s3p but limit battery amps.  Testing done on those batteries was done at 20a continuous.  I don't see you pulling 60a continuous on a 3p setup. They will sag more when you pull that many amps compared to lipo.  There are a bunch of different ways build a battery.  People do 10s2p setups so 3 or 4 is fine. Plus tons of opinions here.  If you don't want to buy more batteries or completely change things just go with what you got.

How many cells can your charger do? Six or seven?
```

---
## \#3 Posted by: Teo Posted at: 2018-07-15T03:24:38.555Z Reads: 37

```
@E1Allen, I have a 6cells charger so 6s 4p would work but I now live in Singapore (since a week) and getting those 3 extra cells shipped here is quite hard and very expensive.

7s3p. if it's 20amp continuos for each cell i thought it should be ok-ish to limit at 60amps as It will probably just draw that in acceleration.would you put 50amps? 40amps? In the vesc settings? 
At that point isn't it better to have higher current and lower voltage going for 5s4p?
```

---
## \#4 Posted by: E1Allen Posted at: 2018-07-15T03:41:22.176Z Reads: 32

```
Okay to push 60.  Up to you at this point. Sounds like 5x4
```

---
