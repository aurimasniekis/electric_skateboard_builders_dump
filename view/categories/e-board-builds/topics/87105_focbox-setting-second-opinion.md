# FocBox setting second opinion

### Replies: 18 Views: 436

## \#1 Posted by: TreeFactory Posted at: 2019-03-14T02:39:23.711Z Reads: 134

```
Hello. I have just completed my first build! I have my mountainboard down my hall ways a couple of times and nothing has exploded. Awesome. But before I take it outside and go for a long run I am hopping to get some second opinions on the focbox setting to make sure I've got the best settings. 
I'm running dual focboxes with twin 170kv 6380's with a 12s1p 6000mah 65s lipo setup with an 80amp BMS. Its also a mountainboard so the gearing is 14t-72t and the wheel size is 200mm I think? whatever the standard trampa wheel is. ![1|690x388](upload://gufAf2uEKaAMjyxyqcvJfp1lVDr.jpeg) 
![2|690x388](upload://hmJhTbzJhgPIzc5n14uU6QNPR7f.png) 
Any input is appreciated. Thanks!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-03-14T02:53:46.839Z Reads: 118

```
hey bud,
don't know much about foc bc its bloody annoying, but apart from that your motor settings look good. just be aware that your battery min regen in total is 30a. that's alot of charging current. maybe dial it down to 25 or 20a total.
(ik someone else will have a go at me but idc
```

---
## \#3 Posted by: TreeFactory Posted at: 2019-03-14T03:06:15.955Z Reads: 110

```
Righto, I went with the max and minimums on the focbox site for those. Also I think the battery settings for max and min they had where for the 1860 variety and dug around on here till i came up with they numbers for the lipos
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-03-14T03:18:27.246Z Reads: 104

```
i mean if you're happy with 30a charging on your lipos then sure. if they're graphenes or nano techs you'll be fine but standard lipo might not like it
```

---
## \#5 Posted by: TreeFactory Posted at: 2019-03-14T04:00:44.798Z Reads: 98

```
they're graphenes
```

---
## \#6 Posted by: TreeFactory Posted at: 2019-03-14T04:54:34.229Z Reads: 90

```
Also my lipos max charge is 44.4v should the maximum input voltage be 57vs?
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-03-14T05:41:42.286Z Reads: 83

```
maximum really doesn't matter. it's minimum you wanna be careful about.
```

---
## \#8 Posted by: mynamesmatt Posted at: 2019-03-14T05:42:05.305Z Reads: 82

```
and yeah 30a will be fine on graphenes
```

---
## \#9 Posted by: TreeFactory Posted at: 2019-03-15T02:35:36.143Z Reads: 66

```
gotcha, i was worried about the max cause of regen braking
```

---
## \#10 Posted by: meesie Posted at: 2019-03-15T08:34:35.912Z Reads: 61

```
you can calculate your max braking with lipo's this way:

lipo mAh * C-rating = max output current.
--
for charging it really depends on the chemistry of the battery. since you have a graphene battery you can charge at 10C, so:

lipo mAh * C-rating (10) = max charge current.
--
hope this helps!
```

---
## \#11 Posted by: TheSebas Posted at: 2019-03-15T09:35:03.896Z Reads: 57

```
Don't forget to convert mAh to Ah :stuck_out_tongue:

And most packs charge at 1C or can LiPo charge at 10c?
```

---
## \#12 Posted by: meesie Posted at: 2019-03-15T09:53:29.160Z Reads: 58

```
You should charge normal lithium polymer batteries with 1c, however they can take more in bursts. This is about a Turnigy Graphene battery which, according to what i’ve read on various forums, can take up to 10C
```

---
## \#13 Posted by: Blitz Posted at: 2019-03-15T09:53:35.212Z Reads: 57

```
[quote="TheSebas, post:11, topic:87105"]
can LiPo charge at 10c?
[/quote]
Noooooooo

10jason
```

---
## \#14 Posted by: TreeFactory Posted at: 2019-03-16T03:17:56.530Z Reads: 46

```
So it's 6ah*65c=390?! that doesn't seem right. Do i convert that to voltage? I assume I do. Or is it 6000mAh*65c=390000?
```

---
## \#15 Posted by: meesie Posted at: 2019-03-16T07:07:01.977Z Reads: 44

```
[quote="TreeFactory, post:14, topic:87105"]
6ah *65c=390?!*
[/quote]
Yup that’s correct, 390A max draw. Lipo batteries have crazy max discharge capabilities sometimes.

[quote="TreeFactory, post:14, topic:87105"]
Do i convert that to voltage?
[/quote]
You can’t convert Amps to Volts. It’s two different things. Think of gnomes running through a pipe. Voltage is how fast your gnomes run and Amps is how fat your gnomes are.

For your focbox settings i’d just start with:
50A batt max
-20A batt min
50A motor max
-20A motor min
Adjust after testriding.
```

---
## \#16 Posted by: b264 Posted at: 2019-03-16T07:23:02.052Z Reads: 39

```
Manufacturers inflate C ratings.  I would not trust that.
```

---
## \#17 Posted by: meesie Posted at: 2019-03-16T08:15:54.499Z Reads: 39

```
Which is why i said

[quote="meesie, post:15, topic:87105"]
i’d just start with: 50A batt max
[/quote]

390 is more than you’d ever need on an eskate. The focbox can handle less than that too so it wouldn’t be a problem anyway. 

But indeed, manufaturers are known/suspected to inflate C ratings. Never go max on your lipo
```

---
## \#18 Posted by: Hummie Posted at: 2019-03-16T08:23:33.670Z Reads: 35

```
Max voltage you need high to account for voltage spikes or will shut down. I think 57 is good enough

But 12s max voltage is 50.4 not 44 with those cells (assuming their stated max charge is 4.2$ More like out of charge at 44 or 43. 
 There should be a stated max charge rate besides the discharge rate but I bet with those cells u would need some insane power supply to take full advantage. If u can discharge that much the charge rate should be crazy high too
```

---
