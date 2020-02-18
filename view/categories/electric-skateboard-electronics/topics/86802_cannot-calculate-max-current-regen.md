# Cannot calculate max current regen

### Replies: 8 Views: 146

## \#1 Posted by: Aleks1 Posted at: 2019-03-10T23:57:18.434Z Reads: 52

```
Hello pips, need help! I got two lipos 4500mAh 6s 40c in series, and also I use BMS (https://cdn.shopify.com/s/files/1/1929/9189/products/12s_LiPo_Datsheet.JPG?v=1521457713). I have 3 questions 
1. Will my batts regen because of BMS if I use discharging? 
2. What will be the max current regen? 
3. What is my batt max current? 
Might seems a stupid questions but I only started) Thanks
```

---
## \#2 Posted by: b264 Posted at: 2019-03-11T00:08:33.624Z Reads: 46

```
What cells/lipos are you using?
```

---
## \#3 Posted by: Aleks1 Posted at: 2019-03-11T00:09:54.554Z Reads: 41

```
https://hobbyking.com/en_us/zippy-compact-4500mah-6s-40c-lipo-pack-xt90.html
```

---
## \#4 Posted by: b264 Posted at: 2019-03-11T00:12:48.213Z Reads: 33

```
I would set "battery max" at 45A and "battery min" at -13.5A
```

---
## \#5 Posted by: b264 Posted at: 2019-03-11T00:14:38.782Z Reads: 35

```
[quote="Aleks1, post:1, topic:86802"]
* Will my batts regen because of BMS if I use discharging?
* What will be the max current regen?
* What is my batt max current? Might seems a stupid questions but I only started) Thanks
[/quote]

1) yes
2) I would limit it to about max 3C, or about 13.5A.
3) The lower value will give you more range and your cells will last longer, but I'd try 40A or 45A
```

---
## \#6 Posted by: Aleks1 Posted at: 2019-03-11T00:15:46.218Z Reads: 32

```
Thank you!
```

---
## \#7 Posted by: b264 Posted at: 2019-03-11T00:16:49.924Z Reads: 30

```
To clarify, that's for a single motor.  For dual motor, halve the "battery" numbers for each motor but don't halve the "motor" numbers.
```

---
## \#8 Posted by: Skunk Posted at: 2019-03-11T00:27:59.146Z Reads: 26

```
I just stopped by to say that when I was scrolling through the forum I thought the title of this was "cannot reach climax"
```

---
