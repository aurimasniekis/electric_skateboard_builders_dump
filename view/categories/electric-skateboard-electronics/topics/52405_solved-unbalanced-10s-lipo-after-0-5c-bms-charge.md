# \[SOLVED\] Unbalanced 10S Lipo after 0.5C BMS charge

### Replies: 6 Views: 364

## \#1 Posted by: drassak Posted at: 2018-04-16T07:20:47.156Z Reads: 52

```
Hello All,

I took my board out for a ride yesterday and rode it untill empty battery with some steep hill climbs (SF like). I then realized that the cells where not evenly discharged: all where around 3.7 except one at around 3V. 

I put the pack back on charge using a 42V, 2A charger and a 10S BMS from battery support. After the charge was completed the cell read like this:
#1 : 4.08V
#2 to 9 : 4.21V
#10 : 3.85 V

Is there a way to get it back on track? I was thinking about disassembling it and charging individually the low cells using my Imax B6 to get them back to 4.2V.

Or is my pack dead? Should I change some cells?  

Thanks
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-04-16T08:37:42.577Z Reads: 39

```
[quote="drassak, post:1, topic:52405"]
After the charge was completed the cell read like this
[/quote]

How do you determine that it was fully charged?

I think if the green led on the charging brick goes on it only means that the target voltage was reached. Then you should leave it connected for some time because just now the balancing is Happening. So maybe you reached the voltage without going into balancing?
```

---
## \#3 Posted by: drassak Posted at: 2018-04-16T08:52:35.440Z Reads: 39

```
Yes I left it plugged in a whole night
```

---
## \#4 Posted by: b264 Posted at: 2018-04-16T08:52:58.271Z Reads: 39

```
[quote="drassak, post:1, topic:52405"]
Is there a way to get it back on track?
[/quote]

Leave it plugged-in overnight and check the voltages again.  I think there are two problems here, don't mix them together.

Problem 1) you need the pack correctly charged
Problem 2) you need to verify that your charging setup works

If you want to be free of problems, work on #2 and #1 will come naturally.
```

---
## \#5 Posted by: DeathCookies Posted at: 2018-04-16T09:02:15.395Z Reads: 36

```
Check the voltage of your power supply.
```

---
## \#6 Posted by: drassak Posted at: 2018-04-19T14:51:18.848Z Reads: 23

```
Hello all, to follow up on this issue: 

It seems that the BMS won't be able to bridge a too big gap between cells. 

What I did was isolate the 2S packs with the low cells and go through multiple charge and discharge cycles at a low amp rate using a Imax B6 charger. Every new cycle the gap would get smalled until finally reaching equals.
```

---
