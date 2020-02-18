# Does mah matter when buying a lipo battery

### Replies: 16 Views: 2949

## \#1 Posted by: dg798 Posted at: 2017-07-28T20:22:33.439Z Reads: 139

```
how much does mah matter when it comes to buying a lipo battery.
```

---
## \#2 Posted by: pennyboard Posted at: 2017-07-28T20:24:16.780Z Reads: 139

```
Yeah. It matters a lot. Mah is battery size. While cell count is voltage. So the mah that you choose for your batteries will affect range. More mah=bigger battery= more range
```

---
## \#3 Posted by: dg798 Posted at: 2017-07-28T20:26:51.259Z Reads: 137

```
how much range approximately would a 10s 4000 mah battery vs a 5000 mah 10s battery?
```

---
## \#4 Posted by: pennyboard Posted at: 2017-07-28T20:29:52.861Z Reads: 134

```
I'm just estimating here, but probably about 8 miles of range for 4000mah 10s and 10 miles of range for 5000mah 10s
```

---
## \#5 Posted by: dg798 Posted at: 2017-07-28T20:30:33.254Z Reads: 123

```
also was does the "c"mean?
```

---
## \#6 Posted by: SirDiff Posted at: 2017-07-28T21:12:48.691Z Reads: 112

```
Discharge rate, how many A can the battery send to the motor. Higher C is better
```

---
## \#7 Posted by: dg798 Posted at: 2017-07-28T21:13:25.879Z Reads: 112

```
whats the average "C" for a good battery
```

---
## \#8 Posted by: Achmed20 Posted at: 2017-07-28T21:14:36.264Z Reads: 108

```
my 9S 5000mAh has a range of about 16-18km of continues riding. stop and go however is what will reduce this value drasticly
```

---
## \#9 Posted by: dg798 Posted at: 2017-07-28T21:14:59.961Z Reads: 104

```
and whats the "c" rating for it
```

---
## \#10 Posted by: Cobber Posted at: 2017-07-28T21:20:14.147Z Reads: 101

```
The batteries "c" ratting is a measure of its discharge rate per amp hour. So more amp hours will provide a higher discharge rate. You will heat up the batteries less and get less sag (voltage drop) under load with a higher amp hour pack(s).
```

---
## \#11 Posted by: dg798 Posted at: 2017-07-28T21:20:46.736Z Reads: 99

```
what do you think is a good "c" rating
```

---
## \#12 Posted by: faithfulpuppy Posted at: 2017-07-28T21:26:32.797Z Reads: 97

```
"c" is a rating of the maximum discharge of the battery as a function of capacity.  Multiply the capacity of the battery by the C rating to find the maximum discharge.  For example, if you have a 2000mAh lipo battery with a 30c rating, the maximum discharge will be 2ah * 30c = 60a.
```

---
## \#13 Posted by: Cobber Posted at: 2017-07-28T21:27:07.800Z Reads: 99

```
The higher the better, is also safer because you are less likely to over discharge them under load. You often get more range too as your low voltage (v)esc cut off doesn't kick in because of a negative voltage spike under load (sag).
From the experience of others minimum 20-30c, the 10-15c packs are too low. I have [65c](https://hobbyking.com/en_us/graphene-6000mah-6s-65c-w-xt90.html) and 12Ah for my eMTB build.
```

---
## \#14 Posted by: SilentException Posted at: 2017-07-28T21:53:55.856Z Reads: 91

```
I would suggest reading this and then asking questions, if anything is unclear (it won't be):

https://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010
```

---
## \#15 Posted by: sl33py Posted at: 2017-07-28T22:44:54.489Z Reads: 84

```
Yes mAh/Ah matters - not only for range but for discharge current ability (as "C").  

A 1000mAh / 1Ah battery w/ 10c = 10A discharge current ability.  Bad.
A 10,000mAh / 10Ah w/ 10c = 100A discharge current ability.  Decent (I'd avoid the multistars w/ this)

So mAh matters a lot, but as it relates to the C rating of the battery.

The mentions above on their range for their setup is likely accurate, but doesn't say what the estimated range is per Wh.  10Wh = 1km (depending on rider weight, hills, aggressive/fast or chill - all huge factors, but ballpark).  Wh (watt hours) = Ah (amp hours) * voltage.

So the 10s 5000mAh = 10s/42v * 5Ah = 210Wh = 21km/13mi.

Good info from @cobber and @SilentException's battery thread.

I think unless tested like the 18650 li-ion cells by mooch and similar - the "C" rating of most lipos is total marketing.  Don't count on it actually providing that constant current unless in a lab or even then...  So i also try to get the highest C i can afford.  My personal minimum is 100A current discharge ability or better.

Measured w/ eagletree data logger here's a similar ride w/ two different setups - both single motor (149kv and 190kv) - the biggest difference to look at is the "sag" under high current load:
 
(reposting from basen thread to save typing):
[quote]I'm not a normal sized human (6'8"/2m - 265lbs/120kgs'ish) - on 'The Suga' (guest board) - 149kv 8s2p 60c (2x8s 5.8Ah 30c parallel) -  i saw 51A peak:
[img]https://goo.gl/Y6ou4z[/img]
(i have a nice bike path across the street and did a quick 4'ish miles with a couple nice long gradual hills, and a short steep one behind me i tried to stress it)  Most boards won't take me up, it did though slowed down midway to top.

On my GF's Vanguard - 190kv 8s 30c (2x4s 8Ah) -  i saw 46A:
[img]https://goo.gl/bYowz1[/img] 
Just a short ride to test, did not do the long gradual hill, just the one steep behind house.  (12mm belt started skipping and almost made the top of the last steep hill)[/quote]

You can see a big difference as the packs get pushed to provide their peak amps (46 and 51A) - and more noticeably is the voltage sag to provide that current.  Top is 60c, bottom 30c.

HTH - GL!
```

---
## \#16 Posted by: Cobber Posted at: 2017-07-28T23:03:14.873Z Reads: 63

```
[quote="sl33py, post:15, topic:28968"]
I think unless tested like the 18650 li-ion cells by mooch and similar - the "C" rating of most lipos is total marketing
[/quote]

Yeah like @sl33py said, which is why I normally don't do the math and describe the relationship instead. Within the same manufacturer they are good for comparisons though...
```

---
