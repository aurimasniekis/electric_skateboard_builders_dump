# Multistar battery

### Replies: 18 Views: 1927

## \#1 Posted by: Gabriel_Robinson Posted at: 2017-01-24T20:29:35.072Z Reads: 147

```
https://hobbyking.com/en_us/multistar-high-capacity-3s-5200mah-multi-rotor-lipo-pack-1.html
 Can I use two of these batteries in Series with a 3000w motor and a vesc? Or do i need a higher c rating? Or is 10 enough
```

---
## \#2 Posted by: mmaner Posted at: 2017-01-24T20:48:10.197Z Reads: 141

```
Most people run at least 20C, I run 30C.  THat being said, I have heard that as far as lipo performance is concerned, the C rating is stackable.  I wouldn't testify to that but I am curious if its plays out in practice.
```

---
## \#3 Posted by: Hummie Posted at: 2017-01-24T20:56:43.599Z Reads: 140

```
if the c numbers were real it would be fine at 52 amp ability continuous, but it seems all the lipos are exaggerated by about half the c rating.
```

---
## \#4 Posted by: Maxid Posted at: 2017-01-24T21:00:43.401Z Reads: 134

```
C rating means nothing without the capacity of the battery.
A 10C at 5000mAh is 52amps.
A 10C at 10000mAh is 100amps
With Chinese Lipos however it is best to use as high of a C rating as you can afford usually.
```

---
## \#5 Posted by: Hummie Posted at: 2017-01-24T21:17:54.588Z Reads: 120

```
also the motor's rated supposed watt ability, at 3000, would be a continuous rating if it were real.  unlikely.  but my real point is the power the motor will put out can be set by the vesc.  You could get those batteries and set the vesc battery amp limit to 25amps if you want the batteries to last a long time and also not suffer from voltage sag, or higher amp settings on the vesc and the battery will last less time.    
If you put those two batteries in series together and then 6s, 50 volts, you can reduce the amp draw necessary for the same power.  you will have more power and not suck from the battery as hard.  25v x 25 amps is...like 750 watts.  best to get as much voltage as you can.  if you got up to 50v, 12s, plus that 25 amps, 50x25...1250 watts.   as long as the motor is a low enough kv so the electrical rpm doesn't go faster than the vesc can do with a high spinning high voltage.   you'll need to do 10 or maybe 11s max if the kv is higher than 200 I think.
super high c ratings aren't necessary.  i recommend the hobby king flightmax packs. 30c  8 or 5 ah.
```

---
## \#6 Posted by: mmaner Posted at: 2017-01-24T21:22:47.362Z Reads: 110

```
[quote="Hummie, post:5, topic:16628"]
but my real point is the power the motor will put out can be set by the vesc
[/quote]

I am absolutely sure I do NOT understand this, but...does that mean you can set a 260kv motor to be logically 180kv in the VESC config?
```

---
## \#7 Posted by: Hummie Posted at: 2017-01-24T21:25:31.060Z Reads: 109

```
you could set the max electrical rpm to something the vesc could handle, forget what number, and that way you could run a higher kv.  you have to keep under the max erpm the vesc can do and kv times voltage x 7 i believe will give you the number that could happen if the vesc is not limited.  i want to say 86000 erpm is the max.  maybe

 but to reduce power you can simply lower the amps the vesc will pass on
```

---
## \#8 Posted by: Gabriel_Robinson Posted at: 2017-01-24T21:47:22.717Z Reads: 96

```
[quote="Hummie, post:5, topic:16628"]
hobby king flightmax packs
[/quote]

Like this one https://hobbyking.com/en_us/zippy-flightmax-5000mah-2s1p-30c-hardcase-pack-roar-approved-de-warehouse.html ?
```

---
## \#9 Posted by: Hummie Posted at: 2017-01-24T21:48:28.199Z Reads: 91

```
the hard case adds to the height but otherwise good.  anything 20c is probably good and 30c even better
```

---
## \#11 Posted by: Gabriel_Robinson Posted at: 2017-01-24T22:48:52.233Z Reads: 78

```
https://hobbyking.com/en_us/zippy-compact-5800mah-8s-25c-lipo-pack.html
Would this work better?
```

---
## \#12 Posted by: Hummie Posted at: 2017-01-24T22:55:38.579Z Reads: 72

```
what kv is your motor?  that will tell whats the max voltage you can run on the vesc..actually as I wrote you could just put the electrical rpm limit in effect and run 12s I think.  

that pack is huge brick.  I wouldn't get it but it would work.  8s is not optimizing the vesc but it might not matter to you.

need your kv
and your gear ratio and wheel size if not a hub motor
```

---
## \#13 Posted by: Gabriel_Robinson Posted at: 2017-01-25T00:24:14.886Z Reads: 65

```
180 kv with a 16th and a 36th on 93mm flywheel clones.
```

---
## \#14 Posted by: Gabriel_Robinson Posted at: 2017-01-25T00:24:56.832Z Reads: 66

```
^^^^^^^^^^^ I forgot to have it reply to you
```

---
## \#15 Posted by: Hummie Posted at: 2017-01-25T03:13:05.564Z Reads: 64

```
Sounds good. If I were u I'd do 12s and foc program on vesc
```

---
## \#17 Posted by: Gabriel_Robinson Posted at: 2017-01-25T03:24:30.559Z Reads: 61

```
https://hobbyking.com/en_us/zippy-compact-5000mah-6s-25c-lipo-pack.html
Could i do two of these in series or are they to large
```

---
## \#18 Posted by: Hummie Posted at: 2017-01-25T03:38:29.496Z Reads: 59

```
I like the 2s 8ah most but have also gotten 3s and 5ah. That 6s brick is also huge. If u want to be daring and cheap u could split it w a cc but it's a pain.
```

---
## \#19 Posted by: AndyPG Posted at: 2017-01-26T15:39:26.904Z Reads: 47

```
[quote="Gabriel_Robinson, post:1, topic:16628, full:true"]
https://hobbyking.com/en_us/multistar-high-capacity-3s-5200mah-multi-rotor-lipo-pack-1.html Can I use two of these batteries in Series with a 3000w motor and a vesc? Or do i need a higher c rating? Or is 10 enough
[/quote]

Hi G_R.

I've been using Multistar packs for a year or so in other applications.
They are great batteries and the extra capacity is real.
They can cope with the odd 10C burst.
The thing is, when I say "cope", what I mean is, they survive it undamaged.
If you go anywhere near 10C sustained, they will get hot.
The main problem is, even as you approach 5C, they suffer quite a lot of voltage drop and your top speed may suffer.
I'd stick with 20C packs minimum.
```

---
## \#20 Posted by: Gabriel_Robinson Posted at: 2017-01-26T16:48:00.206Z Reads: 45

```
Thanks man!
```

---
