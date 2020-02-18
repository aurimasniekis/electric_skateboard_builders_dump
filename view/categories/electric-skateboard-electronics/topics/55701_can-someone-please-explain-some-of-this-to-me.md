# Can someone please explain some of this to me

### Replies: 14 Views: 565

## \#1 Posted by: Orin635 Posted at: 2018-05-16T21:22:38.367Z Reads: 156

```
Edit: been making a couple of topics recently so I don't want to make another for just this question. 

Could someone please explain some of this information ![Screenshot_2018-05-17-23-41-24|281x500](upload://fKD3JdDh9WBagdLjDTJZs3gcdZi.png)
Like what's the difference between detection voltage and release voltage, I can guess but it doesn't really make sense and then there's balance voltage for single cell and they're all different, at what voltage will it cut off? 


___________________________________________________

Hi Guys,

When I was building my board I was on a tight budget so I got 2 of these LiPos and ran them in parallel: 
https://hobbyking.com/en_us/multistar-high-capacity-6s-5200mah-multi-rotor-lipo-pack.html

They've done me well and still are but I would like a little more AMPs output and more capacity (Only run them down to 3.8v per cell because after that it starts to have to much voltage sag) I currently don't have the money to upgrade my LiPos to a good Li-On 10s5p pack so I'm thinking to buy another battery (once they're in stock) and add it in parallel to have in total 3 in parallel. 

I know it not good to do this though so I would like your guys opinions nd thoughts.

Thanks all!

edit: also looking for a 6s BMS (bypass discharge)
```

---
## \#2 Posted by: pat.speed Posted at: 2018-05-16T21:49:27.321Z Reads: 137

```
Why would it not be good to do this, there is nothing wrong with it as long as you wire all the balance leads in parallel too and connect them to the bms. They aren’t the best batteries but in a 3p should be alright
```

---
## \#3 Posted by: Orin635 Posted at: 2018-05-16T22:04:42.776Z Reads: 129

```
Well I thought using 2x 2 month old battery's and a brand new one arent good , I dont know why I just thought I read that somehwere to not use used with new
```

---
## \#4 Posted by: pat.speed Posted at: 2018-05-16T22:06:23.561Z Reads: 113

```
Ahh yeah good point but it should be fine as your running it in parallel so the cells will pretty much be combined together making one big battery. If it was in series then it’s another story because the old cells might drain before the new ones
```

---
## \#5 Posted by: Orin635 Posted at: 2018-05-16T22:07:16.385Z Reads: 99

```
So it should be ok? thats good just needed to check
```

---
## \#6 Posted by: pat.speed Posted at: 2018-05-16T22:18:04.546Z Reads: 90

```
Yep, as long as there aren’t too many cycles it will be all good. 25+ cycles and I would get some advise from someone more knowledgeable than myself. Also remember when connecting the batteries to have them at the same voltage
```

---
## \#7 Posted by: E1Allen Posted at: 2018-05-16T23:13:11.247Z Reads: 77

```
Just monitor them when you charge. Look for cells going bad.  Less overall draw on each cell so it should be fine.  I wouldn't worry about 25ish discharge cycles though.
```

---
## \#8 Posted by: Orin635 Posted at: 2018-05-17T17:13:11.403Z Reads: 63

```
excellent cant wait
```

---
## \#9 Posted by: Orin635 Posted at: 2018-05-17T22:45:58.399Z Reads: 57

```
Couple of questions added them to the top of the topic
```

---
## \#10 Posted by: rich Posted at: 2018-05-17T23:29:23.834Z Reads: 53

```
[quote="Orin635, post:1, topic:55701"]
Like what’s the difference between detection voltage and release voltage, I can guess but it doesn’t really make sense and then there’s balance voltage for single cell and they’re all different, at what voltage will it cut off?
[/quote]


When you use the BMS for charging only it means that the cells at the end of charging get balance charged with 4.2V per cell and 42mA. Better BMS have 60-130mA but if your cells don't drift too much it is not a big difference in time. If one cell would reach 4.28V then the BMS would stop charging this cell (and in theory release it again when the voltage dropped below 4.08V).

The other parameters are only interesting when you use a BMS for discharge, too (but not this one).
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-05-17T23:55:47.792Z Reads: 45

```
http://www.electric-skateboard.builders/t/bms-detection-and-release-voltages/40154
```

---
## \#12 Posted by: Orin635 Posted at: 2018-05-18T07:12:45.584Z Reads: 27

```
Huh OK, so would your recommend this for LiPos?
```

---
## \#13 Posted by: Orin635 Posted at: 2018-05-18T07:13:00.968Z Reads: 25

```
Thanks I'll go read that now
```

---
## \#14 Posted by: b264 Posted at: 2018-05-18T07:27:56.626Z Reads: 28

```
[quote="Orin635, post:3, topic:55701, full:true"]
Well I thought using 2x 2 month old battery’s and a brand new one arent good , I dont know why I just thought I read that somehwere to not use used with new
[/quote]

Don't mix old and new in series -- mixing old and new in parallel is okay.  If you don't understand EXACTLY how to do that, ask for help.
```

---
