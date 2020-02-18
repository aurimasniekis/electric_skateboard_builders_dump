# Any ideas why I get such short range?

### Replies: 17 Views: 1054

## \#1 Posted by: evoheyax Posted at: 2016-11-17T22:37:07.789Z Reads: 117

```
So here's whats happening. Using my Bluetooth module and testing my new app, I can see more of what's going on in my board. One problem I've had with this board is I am using a 12s4p 10Ah 18650 battery pack, yet, I only get about 5 miles of range... So I wanted to see what's going on to cause this. 

My route is 4.63 miles. I start at 50.4v and end around 41.2v. Full discharge would be at about 38v.
To commute this route, I take about 16 minutes and 5 seconds. I average 2.55 amps from my battery per vesc, so 10.2 battery amps average over the whole system.

Running these numbers through [this calculator](http://www.powerstream.com/battery-run-time-calculator.htm), for a 10Ah battery at 10.2 amps, I get .98 hours of ride time, or about 58 minutes of ride time. I'm getting about 1/4th of that, so where is all of my electricity going?

Any suggestions on other data I could calculated in my app to help determine what's going on?
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-17T23:23:50.747Z Reads: 104

```
Are you sure your cells are not fake? 5 miles seems very very low for 12s4p
```

---
## \#3 Posted by: evoheyax Posted at: 2016-11-17T23:25:51.565Z Reads: 102

```
Is there an easy way to test for fake cells? They looked like the images for these cells online, but they make the fakes look so real these days, idk how to tell the difference...
```

---
## \#4 Posted by: Smorto Posted at: 2016-11-17T23:27:46.720Z Reads: 101

```
Im no expert but the easiest way to test for fake cells I know of is just to weigh them. A good cell should way between 43 and 45 grams if I am not mistaken. If that doesn't work then I would measure volts and mah as well.
```

---
## \#5 Posted by: chinzw Posted at: 2016-11-17T23:37:21.527Z Reads: 97

```
You can measure the real AH rating by placing a high power resistor and discharging it. You can use an arduino to do this in a very automated way, or you can just take the measurements manually and then calculate the Ah.
```

---
## \#6 Posted by: evoheyax Posted at: 2016-11-17T23:39:07.520Z Reads: 99

```
Do you have a guide or any further info on how I could do this with an arduino? I've got one laying around...
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-17T23:39:43.304Z Reads: 94

```
You can discharge a couple sample cells at 1A and see how many AH you end up with, that's a decent way to test, but you'll have to take a cell out of your pack to do so, unless you had spares from the same batch laying around.

I always though your range was a bit low. I know hubs lose a lot more energy through heat, but it shouldn't be 5 miles for 440wh low.
```

---
## \#8 Posted by: chinzw Posted at: 2016-11-17T23:40:34.551Z Reads: 93

```
http://www.instructables.com/id/Arduino-cell-capacity-meter/
```

---
## \#9 Posted by: evoheyax Posted at: 2016-11-17T23:44:20.440Z Reads: 93

```
Yes, and if the calculator I linked above is correct, I should be getting 4 times the range I am getting. I always wondered why I sag sooo much also... If the real capacity of this pack is 2.5 Ah instead of the 10 Ah it should be, that would explain the high sag and low range...
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-17T23:45:45.505Z Reads: 91

```
what cells are these btw? HE4's?
```

---
## \#11 Posted by: evoheyax Posted at: 2016-11-17T23:45:50.028Z Reads: 92

```
Thank you for the link, I'll check it out.
```

---
## \#12 Posted by: evoheyax Posted at: 2016-11-17T23:49:06.424Z Reads: 89

```
LG HE2 cells. More economical, low resistance, and looking at those charts someone posted last week, they seem to be one of the better cells... Most of these cells came from my space cell, so if they are fake, I'd be surprised. I added another 21 cells to it with low millage (under 50 miles) to up it from 10s3p to 12s4p.
```

---
## \#13 Posted by: Hummie Posted at: 2016-11-17T23:49:41.879Z Reads: 90

```
Can't u just ride it and see how many watt hours spent on the vesc?  Maybe just ride so it keeps it at a reasonable low discharge
```

---
## \#14 Posted by: Jinra Posted at: 2016-11-17T23:51:44.248Z Reads: 90

```
21 cells? you mean 28?
```

---
## \#15 Posted by: evoheyax Posted at: 2016-11-17T23:54:26.779Z Reads: 89

```
Actually, it's 18. 10s3p is 30 cells, 12s4p is 48 cells, so 48-30 = 18 :stuck_out_tongue:

*math fail FTW*
```

---
## \#16 Posted by: Hummie Posted at: 2016-11-17T23:54:32.472Z Reads: 89

```
Or maybe not watt hours which would need a more complicated program I guess to incorporate voltage sag I think.   but just amp hours u could records at least
```

---
## \#17 Posted by: Jinra Posted at: 2016-11-17T23:56:30.851Z Reads: 89

```
oh, DOUBLE math fail!
```

---
