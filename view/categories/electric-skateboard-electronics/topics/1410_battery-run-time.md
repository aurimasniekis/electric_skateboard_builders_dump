# Battery run time

### Replies: 24 Views: 3438

## \#1 Posted by: willpark16 Posted at: 2016-02-17T04:28:28.473Z Reads: 220

```
Is it possible to get a battery that will last for an hour and get me 6 or 7 miles?
```

---
## \#2 Posted by: barajabali Posted at: 2016-02-17T05:14:46.698Z Reads: 221

```
Of course! What's your system like? Your esc, motor, dual drive? , voltage?  A lot of us get over 20 and sometimes 30 miles
```

---
## \#3 Posted by: willpark16 Posted at: 2016-02-17T05:24:41.122Z Reads: 214

```
Im running alien 42mm 300kv motors dual drive with dual vesc
```

---
## \#4 Posted by: willpark16 Posted at: 2016-02-17T05:25:28.570Z Reads: 215

```
83mm wheels and a 15t to 32tooth gearing
```

---
## \#5 Posted by: willpark16 Posted at: 2016-02-17T06:57:19.546Z Reads: 213

```
Do u think 6s would work???????
```

---
## \#6 Posted by: gamma2 Posted at: 2016-02-17T06:59:06.000Z Reads: 210

```
If you choose to go 6s (22.2v), my calculator says you should have a theoretical top speed of 30mph. If you got 12s, you would be pushing 60mph, again theoretically. Range is dependent on the capacity of the battery. Typically you get 1km per 10Wh. So say you went with dual 6s 8,000mAh batteries. Wired in series: 12S 8ah = 44.V x 8 = 355Wh. Wired in parallel: 6S 16Ah = 22.2V x 16 = 355Wh. Either way you would be looking at about 30km and some change. All kinds of factors will affect the real world results you get.
```

---
## \#7 Posted by: willpark16 Posted at: 2016-02-17T07:01:26.124Z Reads: 200

```
damn those are amazing numbers what calculator are u using? Ive personally had trouble calculating dual motor setup
```

---
## \#8 Posted by: gamma2 Posted at: 2016-02-17T07:03:17.738Z Reads: 191

```
[This][1] is the calculator for top speed. The range is a rough calculation discovered by the community. Typically dual motors will only add a little bit to the top end. The real benefit of dual motors is double the traction and double the torque for hill climbs.


  [1]: http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html
```

---
## \#9 Posted by: willpark16 Posted at: 2016-02-17T07:04:28.460Z Reads: 184

```
Nice haha too bad i didnt ask three months ago when I was still trying to calculate this
```

---
## \#10 Posted by: Sharkface Posted at: 2016-02-17T08:22:55.643Z Reads: 177

```
I have my 149kv on 12S with 5000mah battery. I am on a stupid stupid config of a 20T to 36T config. Top speed of 27mph with weight, ive tested. Since my top speed is so high, when I run a really low speed i can get really darn far. I ride 3-4 miles with hills all the time and batteries wont go below 3.9volts per cell. 

You may not get the same results as you have a lot more speed and a lot less torque than I do. Buuutttttt having that high speed has shown me a longer distance at 20mph than the 12T to 36T (top speed of 15mph) did at 15mph. So... 12S you will get crazy good distance, but good luck keeping it at a low speed. Also since its 12S you would have that punch compared to 6S. 300kv motor is an interesting one. Do 12S, do it for science!!!
```

---
## \#11 Posted by: willpark16 Posted at: 2016-02-17T08:24:56.430Z Reads: 169

```
haha well my only problem with the lower kv is that it will cost more with the vescs and I have a $500 budget
```

---
## \#12 Posted by: laurnts Posted at: 2016-02-17T08:54:39.481Z Reads: 160

```
normally 1 hour and 6 - 7 mile range you will need 6s 5000mah for single motor setup from 149kv - 270kv. Hence any quantities of batteries voltage and or amphours larger than this number would get what you want (considering you have 2 motors, might be 6s 6000mah and or 8000mah to begin with).
```

---
## \#13 Posted by: mostwanted Posted at: 2016-02-17T09:29:36.674Z Reads: 153

```
whoahh ! that far ?

my dual setup consumes alot of juice and climbing and braking took me abt 12km or so . never did really measure .
```

---
## \#14 Posted by: barajabali Posted at: 2016-02-17T12:49:32.187Z Reads: 143

```
Oh yea for sure I have a dual drive and get 20 miles or so. Dual drives are only about 1/3 less range than single drives with the same batteries.
```

---
## \#15 Posted by: barajabali Posted at: 2016-02-17T14:35:07.854Z Reads: 136

```
@gamma2 answered it better than i would 

yes 6s is fine! as long as you are okay with the speed then you dont need a 12s system.  Personally i run 6s because im not all into speed as much as i am into range.   Try and at least use 16 amp hours, 22.2 volts thatll get you ~16-18 miles (approximation).
```

---
## \#16 Posted by: willpark16 Posted at: 2016-02-18T08:37:30.494Z Reads: 126

```
I aprreciate your help would it be okay with you if I put one of your builds in my blog. All the credit would go to you.
```

---
## \#17 Posted by: barajabali Posted at: 2016-02-18T13:44:34.124Z Reads: 123

```
Yea that's fine! I have a new build which I'm making a thread about very soon I'm almost done
```

---
## \#18 Posted by: laurnts Posted at: 2016-04-28T01:54:35.477Z Reads: 101

```
Now I have dual hub motor this run time is highly reduced, similar to @barajabali said. Reduced about 1/3 time although hub motor have less rolling resistance, it's still rolling resistance compared to free wheels. I guess the only different in belt drive vs hub drive is the rolling resistance when out of battery. My big capacitor for no reason really help improve the run time alot.
```

---
## \#19 Posted by: Sirshaunsta Posted at: 2017-12-21T15:56:38.010Z Reads: 42

```
Hey guys looking for tips from more seasoned builders here,  wondering if running a dual setup draws twice the power or if it would conserve my energy with less work in each motor to pull weight
```

---
## \#20 Posted by: egzplicit Posted at: 2017-12-21T16:52:27.642Z Reads: 38

```
[quote="Sirshaunsta, post:19, topic:1410"]
a dual setup draws twice the power
[/quote]

It doesn’t, the load is shared. I get around 15-16 Wh/mile on a dual 5065 with 97s and around 25-26Wh/mile with evolve AT wheels.
```

---
## \#21 Posted by: Sirshaunsta Posted at: 2017-12-21T16:59:05.791Z Reads: 36

```
Thank you I've been wondering about that, as I'm building a 4wd so I couldn't figure out if the calculator I'm using was going to be accurate. Idk if it's meant for single dual or quad drive setups and being my first build I didn't know how the motors would react. So the 4 motors will draw the same currant if not less than 1 motor to do same task? Is that what you're saying?
```

---
## \#22 Posted by: egzplicit Posted at: 2017-12-21T17:16:27.882Z Reads: 36

```
[quote="Sirshaunsta, post:21, topic:1410"]
So the 4 motors will draw the same currant if not less than 1 motor to do same task? Is that what you're saying?
[/quote]

As far as I know, to generate the exact same torque as a single drive, a dual setup will draw the same amount of amps , but will split the power to each of the motors. Since the load is shared, each motor needs only half the amps of that single drive to do half the job.

What i'm not so sure about is what difference is in terms of efficiency between a single drive and a dual. If my dual drive needs 15Wh per mile, what would a single drive need? A bit more due to not running as efficient as a dual drive? Maybe people who experimented with single drive builds could help with an answer. I might do a single drive at some point and would like to know how efficiency is affected.
```

---
## \#23 Posted by: Sirshaunsta Posted at: 2017-12-21T17:21:10.135Z Reads: 38

```
Alright what you did have to share was helpful, thank you. I had thought adding motors would distribute the load and power usage, so my original design should perform as I had thought, between the motors they will share the weight of the 25 to 30 lb board plus my 155lbs maybe a 15lb bag and with all my stored power be able to carry me upwards of 100km with hills and hit a max speed of77 to 85 kmph according to my calc
```

---
## \#24 Posted by: pedro Posted at: 2018-10-03T15:16:04.817Z Reads: 21

```
Hello, do you know how I can calculate my time travler and max distante with my skate? Have some siite can make this calculation. I almost finishing my skateboard, my motor is 270 kv, 14/42 (motor gear/ wheel gear) and 10S2P  lion 1 battery cell (2200 mA.22C)
```

---
