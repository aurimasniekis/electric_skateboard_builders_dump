# Best way to calculate &ldquo;mileage&rdquo;?

### Replies: 23 Views: 1771

## \#1 Posted by: TheFluffiest Posted at: 2018-04-13T18:32:28.364Z Reads: 263

```
I would like a good way to consistently calculate the range on my board. I am making a spreadsheet to get my average top speed and "mileage" on my board. 

The easiest thing that comes to mind is using volts/mile (v/m), but that will be different depending on the Ahr of a person's battery. The reason I say this is (assuming you use your battery down to 3.2v) you will have a 1 volt of usable charge, so it will be easy to calculate distance. However, this could be pretty easy to compare to a car. "My board gets x amount of miles per volt" or "I have a (.9 or 1v) tank." Kinda like cars get miles per gallon with a x gallon tank.

Most use Watt hours per mile (Whr/m) to calculate, but what from what I can gather this is difficult to consistently measure. 

So what do you guys use?

Edit: If this has been discussed before, I apologize. I wasn't able to find that information. If so, please link the page!
```

---
## \#2 Posted by: NickTheDude Posted at: 2018-04-13T18:40:23.472Z Reads: 252

```
Without doing a lot of measurements and calculations it will be difficult to get a very accurate measurement.

A general figure a lot of people here use is 10Wh = 1km of range.
```

---
## \#3 Posted by: FredrikHems Posted at: 2018-04-13T18:46:36.920Z Reads: 243

```
Dont use volts, it will be unprecise as it will depend on your Ah. Volts isnt a way of measuring energy, wh is, so use that. 
A rule of thumb is 10wh/ km, but its different for everyone. A 4wd board pulling a 100 kg man will use alot more than a single drive pulling a 50 kg man, for example.
 Just charge your battery full, and ride until its empty while tracking the distance..
```

---
## \#4 Posted by: taycro Posted at: 2018-04-13T18:49:17.829Z Reads: 224

```
This calculator should do the trick for you: http://esk8.today/2016/12/28/how-far-can-i-ride/
```

---
## \#5 Posted by: professor_shartsis Posted at: 2018-04-13T18:56:19.232Z Reads: 209

```
If you prefer a value that increases with increasing efficiency like miles per gallon then use miles per kilowatt hour. By contrast with watt hours per mile or kilometer a "better" value is a "lower value." 10 watt hours per kilometer is equivalent to 100 kilometers per kilowatt hour.
```

---
## \#6 Posted by: TheFluffiest Posted at: 2018-04-14T14:57:57.590Z Reads: 183

```
Huh. That's pretty interesting! never thought of it that way!
```

---
## \#7 Posted by: Brad Posted at: 2018-04-14T16:19:26.077Z Reads: 162

```
I just divide it into two. One for economical at 11watts per km/mile and the other for heavy use at 22 watts per km/mile.

![Mileage|690x117](upload://zGw0JNgRgcNUbswNJy6ZCZMLsbn.PNG)
```

---
## \#8 Posted by: Sapphirinia Posted at: 2018-04-14T23:03:55.597Z Reads: 133

```
Wouldn't hills and regenerative breaking come into account?
```

---
## \#9 Posted by: Brad Posted at: 2018-04-15T04:30:49.205Z Reads: 124

```
Yes, you are right. 

It just averages out over a trip. One day might be nice and calm weather, the next day on the same trip might have some strong headwind.

As some others has said, there is just too many variables affecting range.

I just consider any additional range from braking as a bonus instead of part of the calculation.
```

---
## \#10 Posted by: pat.speed Posted at: 2018-04-15T04:57:21.038Z Reads: 121

```
Your watt hours per km will be different than watt hours per mile as a mile is longer, meaning more watt hours are required to travel a mile
```

---
## \#11 Posted by: Brad Posted at: 2018-04-15T05:03:21.940Z Reads: 115

```
See the "converted to kilometres" column :slight_smile:

watt hour divide by the same number of watts consumed would give the same answer regardless of metrics which is why kilometers and miles is the same, so look to the right for converted to km or miles and you will see two very different answers in "converted to miles" and "converted to kilometers which accounts for the different distance between a mile and a kilometer.

I had trouble wrapping my head around that for a bit as my brain was telling me that no, the answer is wrong cos the distance cannot be the same :yum:
```

---
## \#12 Posted by: pat.speed Posted at: 2018-04-15T05:14:14.360Z Reads: 111

```
Um I’m not sure what you were saying exactly but I do know that the conversion is roughly 10Wh/km which should be something like 17Wh/mi. 


Oh okay I looked at the column but it’s not correct. 11Wh/km is about average where as a mile is ~1.6 times the length of a km meaning 1.6 times the Wh needed.

So it should be something like 17Wh per mile. You will still get the same distance in total either way
```

---
## \#13 Posted by: Brad Posted at: 2018-04-15T05:26:49.992Z Reads: 109

```
Still correct mate :grin:

The answer gets rounded to the nearest whole number.

My spread sheet says 18Wh per mile which if it was not rounded up would be something like 17.8Wh per mile or something to get exactly 57 kilometers.

I can just input that in my spreadsheet and see the converted kilometer of which I have a better sense of distance. Just like flying at 15 km gives me a better sense of height than 25 thousand feet.

![18wh|690x117](upload://uwfmBgXvcR4vCiu5I6bF7jyJEi.PNG)
```

---
## \#14 Posted by: oyta Posted at: 2018-04-15T05:27:41.287Z Reads: 100

```
https://www.vesc-project.com/calculators

This one is quite comprehensive.
```

---
## \#15 Posted by: Brad Posted at: 2018-04-15T05:29:16.815Z Reads: 92

```
Yes it is quite comprehensive.

I just like to play with spreadsheets so I have my own calculator which is good enough for my use.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-04-15T05:34:29.865Z Reads: 87

```
Ahhh yeah your right just that I don’t think the first spread sheet changed. As it says 11wh for both miles and km that’s why I thought you didn’t understand. 

The second is right though
```

---
## \#17 Posted by: b264 Posted at: 2018-04-15T05:51:48.751Z Reads: 76

```
[quote="pat.speed, post:12, topic:52186"]
So it should be something like 17Wh per mile.
[/quote]

Yes, I can confirm 17Wh/mile is pretty normal for a 200lb person
```

---
## \#18 Posted by: ZackoryCramer Posted at: 2018-04-15T06:12:08.013Z Reads: 72

```
[quote="b264, post:17, topic:52186"]
Yes, I can confirm 17Wh/mile is pretty normal for a 200lb person
[/quote]

How!?! I get 17wh/mile at 110lb 20mph
```

---
## \#19 Posted by: pat.speed Posted at: 2018-04-15T06:13:12.746Z Reads: 67

```
Also depends on hills, gearing, motors and speed
```

---
## \#20 Posted by: b264 Posted at: 2018-04-15T06:22:42.482Z Reads: 70

```
[quote="ZackoryCramer, post:18, topic:52186"]
How!?!
[/quote]

That's a maximum when going for max range.  If I'm accelerating at-will it's closer to 30Wh/mile
```

---
## \#21 Posted by: ZackoryCramer Posted at: 2018-04-15T06:24:39.452Z Reads: 67

```
Oh yea? Bet I can squeeze that to 10wh/mi. 
I went walking speed with my friends one time and got 6wh/mi efficiency.
```

---
## \#22 Posted by: Battosaii Posted at: 2018-04-15T12:46:11.007Z Reads: 57

```
I'm 300lbs and I was doing 18wh on my dual 6374 set up going for max range and I did about 30miles.

Weight dosnt affect efficiency much when just cruising it's does when you ride hard.
```

---
## \#23 Posted by: Acido Posted at: 2018-04-15T12:50:17.506Z Reads: 54

```
Get a bluetooth module, they can track everything and you will already have a csv file of it
```

---
