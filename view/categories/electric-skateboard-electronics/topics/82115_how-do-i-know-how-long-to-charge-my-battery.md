# How do I know how long to charge my battery?

### Replies: 9 Views: 190

## \#1 Posted by: badger4life Posted at: 2019-01-26T05:07:05.901Z Reads: 68

```
Hey all, I'm new to eSkating and I have a question about how long I should charge my battery.  The site I bought the battery from says 3-4 hour charging time, but after seeing some pictures of batteries that caught fire I figured I'd ask just in case.

Here are my battery specs:

Li-ion battery 2P 10S 
Rated Voltage: 36V
Charge Voltage: 42V
Power: 216wh 
Discharge Current: 30ah

My board is a DIY board and I don't have the battery hooked up to an LCD display so I don't have a way to tell what the battery's charge level is.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-26T05:16:18.807Z Reads: 62

```
[quote="badger4life, post:1, topic:82115"]
Discharge Current: 30ah
[/quote]

Ah are not a discharge unit.

But the total Ah of your pack gives you an idea how long charging minimum takes.
If you have a 3Ah pack and you have a 3A charger it will take as min 1hour for a full charge.
I say min, because usual charger reduce the current the closer they come to the max voltage you want to charge up, plus it needs some time to balance the cells after you charged up your pack. This time depends on how much your cells drifted from each other.
```

---
## \#3 Posted by: badger4life Posted at: 2019-01-26T05:23:11.986Z Reads: 60

```
Sorry about the Discharge Current, I was just copying from their site.

I guess that I'm just wondering what the best charging practices are.  Should I store it discharged or charge it after each ride?  How long should I charge it for?  Stuff like that.
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-01-26T05:25:16.163Z Reads: 57

```
Whenever The Great Skatan says to stop
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-01-26T05:32:13.815Z Reads: 55

```
If you're using the board then you don't need to worry about voltage IF
1) your charger cuts off at full charge (42ish) (get the right charger or BMS)
2) your ESC cuts off at empty charge (30ish) (you need to set this value in the ESC)

You need to get it to storage voltage (37ish) if you're going to let it sit for a while (weeks)

If you put a connector like a female XT30 in parallel with the battery and ESC, and use the male end to seal it when riding, you can stick a voltage/multi meter in it to check (definitely easier to get an inline voltage display)

Ideally you get an alarm for low voltage and an indicator like a watt meter but you don't need them 

Someone correct me of my numbers are wrong
```

---
## \#6 Posted by: Indiangummy Posted at: 2019-01-26T05:35:08.667Z Reads: 50

```
[quote="ZachTetra, post:5, topic:82115"]
You need to get it to storage voltage (32ish)
[/quote]

Proper stroage voltage is about 3.7-3.8V. 3.2V is way to low for storage.
```

---
## \#7 Posted by: Eboosted Posted at: 2019-01-26T05:42:13.023Z Reads: 44

```
Leave it charging until the charger turns off. You can leave it there for days without issues
```

---
## \#8 Posted by: ZachTetra Posted at: 2019-01-26T05:46:54.460Z Reads: 41

```
You can probably leave it on and charging with no issues but it's probably best to disconnect the battery or at least power it down when not in use, and don't keep it on the charger forever since batteries often go up when charging
```

---
## \#9 Posted by: badger4life Posted at: 2019-01-26T05:49:39.065Z Reads: 39

```
Thanks @ZachTetra, I'll take that into consideration.
```

---
