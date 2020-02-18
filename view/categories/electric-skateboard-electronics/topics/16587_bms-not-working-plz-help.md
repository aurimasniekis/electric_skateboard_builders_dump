# Bms not working plz help

### Replies: 11 Views: 1528

## \#1 Posted by: Ryanliu Posted at: 2017-01-24T04:25:34.759Z Reads: 123

```
I am using a 4p 10s configuration of 18650 batteries with this BMS http://www.ebay.com/itm/262590563841 and a charger that was tested with other 10s batteries and works. I wired the BMS with all the balance leads and c-,p- and b- but it didnt charge. I plugged it in and it doesn't work. I was very frustrated so i started checking every wire and pack of parallel cells and the wires were all in the right places and the packs all read between 3.6-4.2v. The weird part is that when i discharge it with my 45a motor for a couple seconds then charge it, it charges for a couple minutes before the led on the charger turns from red(charging) to green(not charging). 
simplified list
BMS: brand new and hasn't been shorted or anything, checked all the connections 
Batteries: Voltage tested and in good range of 3.6-4.2v
Problem: Not charging
Details: after discharging for a couple seconds with my 45a motor it charges for a couple minutes before stopping early (before the voltage gets to 42v)
Charger is a 42v charger and i measured it with my multimeter
```

---
## \#2 Posted by: Blasto Posted at: 2017-01-24T04:28:39.311Z Reads: 118

```
[quote="Ryanliu, post:1, topic:16587"]
and the packs all read between 3.6-4.2v
[/quote]

Is it possible that your bms cutoff the whole charge cycle when one of your packs reaches 4.2V?
```

---
## \#3 Posted by: Ryanliu Posted at: 2017-01-24T05:30:08.760Z Reads: 111

```
The balancing circuit would stop charging the 4.2v cells and keep charging the ones lower than that i think. I will test your theory though by discharging the cells then charging them back up and seeing how long it takes to charge to full
```

---
## \#4 Posted by: Namasaki Posted at: 2017-01-24T08:01:59.126Z Reads: 104

```
I experienced a similar problem once when I had to replace a portion of my battery.
because the voltage of the new cells was much lower than the rest, my BMS could not fully charge the whole pack.
To solve the problem, I had to charge up the new cells separately and then join them to the pack. After that it worked fine.
I think your problem is that your cells have too much difference in voltage 3.6-4.2  is way too much variance.
If you can get hold of a hobby charger, then you could balance charge your parallel cell groups individually and then connect them to the bms. I'll bet that would solve your problem as well as it did mine.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-01-24T08:08:21.270Z Reads: 99

```
Funny thing about BMS's. Your pack needs to be balanced already when you hook it up to the BMS. 
I can't explain why this is the case I just know from experience that it is.
```

---
## \#6 Posted by: Ryanliu Posted at: 2017-02-01T00:26:29.158Z Reads: 81

```
i just charged all my cells to 4v and it still is having the same problem
```

---
## \#7 Posted by: Namasaki Posted at: 2017-02-01T02:20:50.824Z Reads: 81

```
Do you meant it won't charge the pack past 40v?
Are you sure you have everything wired correctly?
Can you draw a quick diagram of your wiring so we can check it?
```

---
## \#8 Posted by: Ryanliu Posted at: 2017-02-01T04:55:24.839Z Reads: 75

```
it wont charge and it is at 40v, i checked the wiring and i followed the wiring diagram in this link, http://www.ebay.com/itm/262590563841. I have wired BMS before so i am pretty confident i did it correctly.
```

---
## \#9 Posted by: Ryanliu Posted at: 2017-02-01T04:57:46.752Z Reads: 75

```
i attatched all the B1, B2, B3 to the positive ends of the B1, B2 and so on and i put the B- on the negative terminal of the battery and i used P- to discharge minus and C- to be charge minus. I connected the positive charge and discharge leads directly to the positive terminal of the whole battery
```

---
## \#10 Posted by: Supdapram Posted at: 2017-11-07T04:06:29.896Z Reads: 48

```
Ik it's been awhile, but I'm having the same problem and I was wondering if you figured it out
```

---
## \#11 Posted by: Ryanliu Posted at: 2017-11-08T05:28:16.851Z Reads: 47

```
I gave up and bought rc batteries.
```

---
