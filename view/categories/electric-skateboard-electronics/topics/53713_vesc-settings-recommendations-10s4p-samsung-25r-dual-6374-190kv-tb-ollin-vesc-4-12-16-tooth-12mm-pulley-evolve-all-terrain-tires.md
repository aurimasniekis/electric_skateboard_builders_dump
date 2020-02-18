# VESC SETTINGS Recommendations &#124; 10s4p Samsung 25r &#124; DUAL 6374 190kv TB &#124; Ollin VESC 4.12 &#124; 16 Tooth 12mm pulley &#124; Evolve All Terrain tires &#124;

### Replies: 14 Views: 1157

## \#1 Posted by: Jcullinan09 Posted at: 2018-04-28T01:03:13.948Z Reads: 233

```
Hi everyone, just wanted to double check, and tweak some settings in BLDC tool.

 I'll post some screenshots of my current settings, and go from there, I look forward to hearing what you guys think I could adjust. Thanks.

![36 PM|690x395](upload://1Z3o01aV3gchj2Q8eBiJmRXegfb.png)
```

---
## \#2 Posted by: Namasaki Posted at: 2018-04-28T05:00:37.816Z Reads: 219

```
These are my settings for a dual drive with 10s Lipo battery

![30 PM|690x398](upload://s2mu3XLgiQqmD9a8gxJkLQLhsy5.png)
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-04-28T05:08:08.161Z Reads: 210

```
If you feel like you want more low-end punch and acceleration, you can increase your motor max to 60-80. 

FOR THE LOVE OF GOD, uncheck the box that says "limit ERPM with negative torque". Leaving that box checked translates to you saying "yes, please slam on the brakes when I reach full speed, I want to eat pavement."

You could also stand to lower the max. ERPM at full brake in current control mode to like 500 which will help keep the board from bucking at low speed when braking.

I'd also increase your battery cutoffs a little to ~35 and 32 to help improve the cycle life of the cells.
```

---
## \#4 Posted by: Jcullinan09 Posted at: 2018-04-28T06:08:51.043Z Reads: 198

```
@MysticalDork I do want more low end punch because I was drag racing somebody today, and I got to say I felt ashamed a boosted was beating me off line. :sweat_smile:

Are you saying to me though that it is fine if I bump motor max to 60-80 amps for each motor?? I thought that the 60-80 amps must be split between each motor individually. Thats how I got 35.00 amps because I assumed 70 amps divided by 2.
```

---
## \#5 Posted by: Jcullinan09 Posted at: 2018-04-28T17:34:49.140Z Reads: 178

```
@Namasaki. Do you run those exact settings on each of your 2 VESC's?
```

---
## \#6 Posted by: threebysix Posted at: 2018-04-28T18:21:17.710Z Reads: 175

```
I believe motor max and min is per motor, no need to divide by 2. Batt max and min are what needs to be halved. At least this is what I learned using the Extended BLDC tool and reading each setting's description.
```

---
## \#7 Posted by: Jcullinan09 Posted at: 2018-04-28T18:29:59.693Z Reads: 166

```
Thats good to know, I could have kicked the shit out of that boosted then haha.
```

---
## \#8 Posted by: Namasaki Posted at: 2018-04-28T19:32:22.017Z Reads: 169

```
[quote="Jcullinan09, post:5, topic:53713, full:true"]
@Namasaki. Do you run those exact settings on each of your 2 VESC’s?
[/quote]

Yes I do...
My BMS is rated for 80a continuous and 240a peak
My battery is good for about 100a
```

---
## \#9 Posted by: MysticalDork Posted at: 2018-04-29T00:30:01.714Z Reads: 167

```
If you're running dual, then the amps coming out of the pack will be split between both vescs, so if you have 75-amp pack (You do) then you can pull a maximum of 35 **battery amps** per vesc, but that doesn't limit you to 35 **motor amps** per vesc. At anything other than full speed/throttle, thevesc can take the battery power (40 volts, 30 amps for example) and step down the voltage/step up the current (20 volts, 60 amps for example). 

Increasing the motor amps thus only really affects low/medium speed performance, not top speed or power at top speed.
```

---
## \#10 Posted by: Boxer86 Posted at: 2018-09-20T04:23:48.644Z Reads: 107

```
Hi I am about to set up my board using 10s graphene 60c lipo's with focboxes and dual sk3 6374's but am using ppm cable instead of canbus. If I copy your exact settings will this work for me? Thanks heaps
```

---
## \#11 Posted by: Namasaki Posted at: 2018-09-20T05:12:51.406Z Reads: 99

```
Yes but you might want to run the Battery cutoff start a little higher than 34v
36v would be better for your Lipos.
And set the cutoff end to 34v
And if your discharging through a bms, make sure it can handle the current
```

---
## \#12 Posted by: Boxer86 Posted at: 2018-09-20T05:53:53.839Z Reads: 90

```
Awesome thanks for that. I was just confused as I read conflicting posts about halving motor and batt numbers ect. Which I know you do with canbus but was unsure if running ppm. I am actually going to only run them to 3.6 hard cutoff as I have 8 5000ah lipos (4 pairs) for my commute to and from work. It is a bit overkill but have read it will really increase the life of the battery’s. I have read lots of your threads and very much subscribe to the theory of over engineering your board so it is under stressed and last longer with fewer problems. Thus the dual 6374’s over single, bldc over foc, ppm over canbus, 10s over 12s and the battery cutoffs. Can’t go wrong.....well let’s hope😳
```

---
## \#13 Posted by: Namasaki Posted at: 2018-09-20T16:23:04.206Z Reads: 71

```
Sounds like your playing it safe on all accounts.
Note that running BLDC mode with non sensor motors requires a push to get the board rolling and then you apply throttle.
```

---
## \#14 Posted by: Boxer86 Posted at: 2018-09-20T21:18:14.262Z Reads: 66

```
Yes no worries. Thanks for your help 👍
```

---
