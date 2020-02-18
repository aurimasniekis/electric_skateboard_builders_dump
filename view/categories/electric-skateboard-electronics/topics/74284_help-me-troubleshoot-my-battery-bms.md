# Help me troubleshoot my battery/BMS

### Replies: 9 Views: 192

## \#1 Posted by: taz Posted at: 2018-11-11T15:50:48.621Z Reads: 66

```
Today my board had shut downs while still at 43-44V (12S5P).
I had to call my wife to come and get me and endure all the snarky comments on the reliability of an esk8 :face_with_symbols_over_mouth:
Anyway I opened up the battery when I got home. The series connections were fine but the last P group measured at 3.10V when all the others were at 3.70V.
This explains the shutdowns as I use a discharge BMS (Bestech HCX-D223V1).
I am currently charging that particular P group by itself until it reaches 3.70V as the others and will then continue through the BMS.

Now my question is how/why this happened?

When I measure the output voltage on my BMS I get approx. 1V lower with the e-switch in the off position and the actual battery voltage in the on position.
Is this normal? Shouldn't I get 0V with the e-switch in the off position?

I don't think I have a defective cell since I would probable get shut downs in other situations since I tend to push my board really hard from time to time.
My guess is that it is a faulty BMS that somehow leaks current only from the last pack.
What do you guys think?
```

---
## \#2 Posted by: Acido Posted at: 2018-11-11T16:16:55.740Z Reads: 60

```
I would try with another bms and see what happens

This is a weird problem..
```

---
## \#3 Posted by: taz Posted at: 2018-11-11T16:53:11.471Z Reads: 52

```
[quote="taz, post:1, topic:74284"]
When I measure the output voltage on my BMS I get approx. 1V lower with the e-switch in the off position and the actual battery voltage in the on position.
Is this normal? Shouldn’t I get 0V with the e-switch in the off position?
[/quote]

Do you know anything about this?
```

---
## \#4 Posted by: Acido Posted at: 2018-11-11T18:00:24.915Z Reads: 48

```
For some reason me and bestechs discharge bmss hate each other, i managed to fry 4 up to now so i switched to charge only

I wish I had a working one so I could test this out for you, @Namasaki do you know anything about this?
```

---
## \#5 Posted by: Namasaki Posted at: 2018-11-11T21:59:06.154Z Reads: 42

```
[quote="taz, post:1, topic:74284"]
When I measure the output voltage on my BMS I get approx. 1V lower with the e-switch in the off position and the actual battery voltage in the on position.
Is this normal? Shouldn’t I get 0V with the e-switch in the off position?
[/quote]


This happens if you don't have a load on the bms output. Like when you don't have the Vesc or Vescs connected.
With no load, there is nothing to drain the voltage down when you turn the bms off.
```

---
## \#6 Posted by: mynamesmatt Posted at: 2018-11-12T00:00:05.710Z Reads: 38

```
when you charge do you make sure the eswitch is on? i had this issue yesterday with one of my lipo cells and was getting cut outs because c1-9 were at 3.7v and c10 was at 3.0v. so ya
```

---
## \#7 Posted by: taz Posted at: 2018-11-12T05:28:51.473Z Reads: 31

```
Yes I do.
However there is always the chance the switch did not engage fully or something like that I guess.
Hopefully this was it.
```

---
## \#8 Posted by: taz Posted at: 2018-11-12T08:16:51.614Z Reads: 26

```
So far it looks like it is the BMS. :rage:
I charged all cells to 3.84V last night.
Checked this morning. All were at 3.84V apart from the 12th P-group which was at 3.80V.:disappointed:
I will check again this afternoon. If it has dropped any further, I will disconnect the balance cable to see if it continues dropping.
```

---
## \#9 Posted by: taz Posted at: 2018-11-14T05:17:38.729Z Reads: 17

```
Another update.
It's not the BMS.
One of the batteries on that 5p group is shorted (or something like that) and bleeds voltage. 
I took the p group apart and charged all cells individually. All of them charged at 4.19V last night but one of them measured 4.08V this morning.
```

---
