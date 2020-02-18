# Battery size and weight comparison

### Replies: 15 Views: 916

## \#1 Posted by: Jammeslu Posted at: 2017-03-21T21:13:47.526Z Reads: 89

```
HI, I was ready for my build but then I looked closely at upgrading the batteries, from 6s to maybe 8s or 10s ( Zippy 5000mah ) I was afraid of it being much bigger and heavier but now I looked in to it and size wise its not so much difference. So if I go 8s 5000mah with a sk3 245kv motor that would work but if I go 10s it will blow my vesc? but is I want more power can I go 8000mah instead still use the same bms and rest of the electronics or what does the mah if I increase ?
```

---
## \#2 Posted by: mmaner Posted at: 2017-03-21T21:17:40.711Z Reads: 88

```
and increase in MAH gives you range, an increase in voltage gives you speed.  If you never ridden a powered board before, you will be surprised how much power there is in a 245kv on 6s setup.  One of mine is and it will 22mph and tackle most hills.
```

---
## \#3 Posted by: jga Posted at: 2017-03-21T21:19:01.343Z Reads: 86

```
Increasing the mAh will give you a bigger range, not more power.
What ESC do you have? If it's a VESC it should support 10S normally.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-21T21:38:15.588Z Reads: 78

```
245kv and 6s seems to be a sweet combo especially with the Tacon Big foot
```

---
## \#5 Posted by: mmaner Posted at: 2017-03-21T21:40:44.040Z Reads: 74

```
[quote="Namasaki, post:4, topic:19440, full:true"]
245kv and 6s seems to be a sweet combo especially with the Tacon Big foot
[/quote]

I don't know about the bigfoot, I dont own one, but I have 1 board with a 260 and 1 board with a 245, I like the 245 better.  Its as fast as the 260 and has measurably more torque.
```

---
## \#6 Posted by: Jammeslu Posted at: 2017-03-21T21:41:42.997Z Reads: 71

```
But will A 8s and 245 kv work Well or is 6s better? @Namasaki @mmaner
```

---
## \#7 Posted by: mmaner Posted at: 2017-03-21T21:51:41.183Z Reads: 65

```
8s should work, just be sure ti limit your ERPMs,  6s is easier and cheaper, to run and charge.
```

---
## \#8 Posted by: Jammeslu Posted at: 2017-03-21T21:53:57.531Z Reads: 62

```
Okej Thanks
```

---
## \#9 Posted by: mmaner Posted at: 2017-03-21T21:54:48.759Z Reads: 59

```
no worries
```

---
## \#10 Posted by: Namasaki Posted at: 2017-03-21T21:55:08.090Z Reads: 58

```
8s and 245kv is well below the 60k erpm limit
8 x 4.2=33.6v
33.6 x 245=8232 rpm
8232 x 7= 57624 erpm
```

---
## \#11 Posted by: Jammeslu Posted at: 2017-03-21T21:58:13.221Z Reads: 55

```
Really usefull, but What would you go with 6s or 8s?
```

---
## \#12 Posted by: Namasaki Posted at: 2017-03-21T21:58:47.014Z Reads: 56

```
8s would be better for performance and range
More top speed, more torque and more range.
Voltage x amp hours = range
so you get about the same range with 6s/10000mah as you would with 12s/5000mah
```

---
## \#13 Posted by: wmj259 Posted at: 2017-03-21T22:15:12.457Z Reads: 58

```
Why do you multiply by 7? Is that a conversion factor?
```

---
## \#14 Posted by: Namasaki Posted at: 2017-03-21T22:16:48.623Z Reads: 56

```
That factor is for the number of pole pairs in the motor.
So if your motor has 14 magnets the factor is 7
14 is standard for 63mm motors
```

---
## \#16 Posted by: PXSS Posted at: 2017-03-21T22:41:05.259Z Reads: 52

```
14 poles is standard for outrunner motors in general in the sizes used for eskate. 

To better answer your question @wmj259, to get electrical rpm which is the what the ESC cares about, you need to take into account the number of magnetic poles in a motor. This number can vary from 2 poles as is in small inrunner motors to 30something or higher in really large outrunner motors. 

The equation to get this is:
Motor RPM * Number of Poles/2
The reason you divide by 2 is because you really care about pole pairs since you need a north and south pole to align with.


---

I'd like to point out that increasing your capacity will also increase the power your battery is able to put out as long as the C rating is the same.
For example a 5Ah 20C can output 100A, while a 10Ah 20C can output 200A.

8S and 10S both work well with a 245kv motor.
Your battery is never going to be at 4.2V realistically while under load so I usually go by 4.0V to get my max eRPM.
An 8s setup gives you around 55k erpm while a 10S setup gives you 68k eRPM. Going with the 8S is safer on your ESC so that's what I recommend but I think some people do have their ESCs up to 70k eRPM without issues.
The advantage of the 10S would be a higher top speed and if you're using the same capacity battery then more power and range.
```

---
