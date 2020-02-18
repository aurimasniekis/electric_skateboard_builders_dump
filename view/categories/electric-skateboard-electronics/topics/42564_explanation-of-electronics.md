# Explanation of electronics

### Replies: 15 Views: 896

## \#1 Posted by: DjamboBuksne Posted at: 2018-01-02T11:42:37.539Z Reads: 192

```
Hello everyone! When I started building my board there was a lot stuff that i didn't understand, like what are battery cells and what wire do i need to get for about 70A of current... Now that I know a lot, I would try my best to explain almost everything and if there's something that i missed, just ask!
```

---
## \#2 Posted by: DjamboBuksne Posted at: 2018-01-02T12:06:29.574Z Reads: 187

```
BATTERIES

TYPES OF BATTERIES:

There are lots of battery types but in this territory we usually use lithium ion or lithium polimer batteries
(Li-ion, Li-po for short)

When you need more voltage, connect your batteries in series and when you need more capacity, connect them in parallel

Batteries have voltage, capacity and C rating which tells you how much current can you drain from one cell in moment of time

--VOLTAGE: (Li-ion, Li-po)

One cell:

Li-ion:
Nominal= 3.6
Max=4.2
Min=2.5

Lipo:
Nominal=3.7
Max=4.2

If you get them under min or over max you can damage them

--CAPACITY:

Amper is for current and Amp•hour is for capacity.
1Ah is 1000mAh
If the battery is 1Ah and your consumer takes 1A than you can run it for about an hour.
There is also that C rating
C rating tells you how much Amps you can "pull" from the battery.
My batteries are 5000mah and 20C so 5Ah*20C = 100A
That means that i can pull up to 100A from them

--CHARGING: (Li-ion, LI-po)

If battery is 3s 1p (2300mah) for example
3s * 4.2V = 12.6V, so that is the voltage that your gonna be charging your battery at
You also need to limit the currant because if you charge the battery too fast it can also explode
You need to look for charging C rating, multiply that with capacity and that is your maximum charging currant!

If there is more questions, feel free to ask!
```

---
## \#3 Posted by: PXSS Posted at: 2018-01-02T12:11:12.179Z Reads: 162

```
[quote="DjamboBuksne, post:2, topic:42564"]
Batteries are made in cells, one cell is maximum 4.2V, in the middle 3.7V and minimum 3.0V
[/quote]

Only true for Lipos. Not 18650.

[quote="DjamboBuksne, post:2, topic:42564"]
Amper/hour is for capacity.
1Ah is 1000mAh
[/quote]

Amp/hour is not the correct unit for capacity. 
Amp•hour is.

[quote="DjamboBuksne, post:2, topic:42564"]
battery is 2300mah so 2000mA or 2A is maximum charging currant.
[/quote]

False. Depends on the battery. Some are capable of 0.5C, some are capable of 5C. Refer to the spec sheet.
```

---
## \#4 Posted by: DjamboBuksne Posted at: 2018-01-02T12:58:49.982Z Reads: 145

```
Okay, thank you for correcting me but Li-po and Li-ion voltages are same
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-01-02T13:08:32.495Z Reads: 143

```
No they're not.
Li-ion:
Nominal= 3.6
Max=4.2
Min=2.5

Lipo:
Nominal=3.7
Max=4.2
Min= There is alot of different numbers here but abselout min is 3.0 before the battery takes alot of damage, but 3.6 If you want your batteries to last and not loose capacity
```

---
## \#6 Posted by: wafflejock Posted at: 2018-01-02T13:15:03.678Z Reads: 134

```
Would also add typically 1C is safe charge rate but in general slower is better (cells have internal resistance and build up heat like any other component more current equals more energy dissipated as heat due to resistance, C rating is a round about way of communicating internal resistance).  The C rating is a maximum and ideally you want much higher than you will ever draw, higher current draw on a cell with high resistance will cause more voltage dip while under load as well.

Also would add take C rating with a grain of salt look to third party discharge tests when possible.
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2018-01-02T13:32:05.988Z Reads: 120

```
IMO,

"Quick and simple explanation of electronics"
-> "Quick and simple explanation of batteries"

No talk about any electronics... yet at least.
```

---
## \#8 Posted by: tung Posted at: 2018-01-02T14:16:04.400Z Reads: 109

```
should i worry about frying the ESC or motor because the original battery is 33v, while my 12s1p will have 50.4v?
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-01-02T14:17:44.634Z Reads: 108

```
yes

10chars
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2018-01-02T14:56:57.221Z Reads: 90

```
[quote="DjamboBuksne, post:2, topic:42564"]
When you need more voltage, connect your batteries in series and when you need more capacity, connect them in parallel
[/quote]

Capacity (wh) is the same.  Amp hours (and therefore maximum current) is increased in parallel. a 1s12p board will not have 12x the range of a 12s1p board (even in an ideal world where 1s is as efficient as 12s)
```

---
## \#11 Posted by: PXSS Posted at: 2018-01-02T18:20:21.647Z Reads: 72

```
[quote="faithfulpuppy, post:10, topic:42564"]
Capacity (wh) is the same
[/quote]

Capacity is measured in amp•hours not watt•hours. So @DjamboBuksne is correct here. 

Energy is measured in watt•hours, range is more closely related to energy than capacity, so you are kind of correct in that aspect but had the terminology messed up
```

---
## \#12 Posted by: faithfulpuppy Posted at: 2018-01-02T19:38:53.001Z Reads: 61

```
oh whoops. Thanks for the correction.
```

---
## \#13 Posted by: DjamboBuksne Posted at: 2018-01-03T11:43:35.593Z Reads: 46

```
Watt hours is energy and you calculate if like this;
Voltage*capacity

If you need to calculate something else, there is one simple formula, R=U/I 
R-> resistance
U-> voltage
I-> current

And also power -> P=U*I
```

---
## \#14 Posted by: willpark16 Posted at: 2018-01-03T11:47:46.671Z Reads: 46

```
Maybe read a bit more or look a bit more there is already a thread like this appreciate the effort though
```

---
## \#15 Posted by: DjamboBuksne Posted at: 2018-01-03T11:48:26.750Z Reads: 45

```
Thank you :grin:
```

---
