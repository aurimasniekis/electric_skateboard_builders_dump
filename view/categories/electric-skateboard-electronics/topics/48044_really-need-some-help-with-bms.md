# Really need some help with BMS

### Replies: 31 Views: 804

## \#1 Posted by: Orin635 Posted at: 2018-03-03T17:01:34.689Z Reads: 70

```
 I've made a couple of post about this but I've never gotten a specific answer.

So I have 2x 6s LiPo's in parallel and a 6s BMS. do I solder the corresponding  balance lead to the other (Blue-Blue, Red-Red etc) 

I made a really shit diagram if you can understand it good job but this is what I think I should do. could someone please confirm it. Thanks![BMS|690x345](upload://18vJZPkVS6CbjBbQ8VBZ0j8o2nB.PNG)
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-03T18:09:40.756Z Reads: 56

```
Did you not get any printed instruction in the box? The balance leads you drew from the batteries are kind of confusing. :thinking: Yes they balance leads go there if that's what you are wondering. Order maybe shifted depending on what bms you're using. It looks like you are doing 6s2p right?
The positive and negative leads from the batteries go in series with the the bms and esc. :exploding_head:
```

---
## \#3 Posted by: Orin635 Posted at: 2018-03-03T18:24:20.389Z Reads: 49

```
I didn't get any instructions (yeah 6s2p)

I don't understand the last part about the series.
```

---
## \#4 Posted by: bevilacqua Posted at: 2018-03-03T18:24:47.892Z Reads: 48

```
Maybe the best solution is to use a charge only BMS and charge them in Series...
```

---
## \#5 Posted by: Orin635 Posted at: 2018-03-03T18:25:50.485Z Reads: 47

```
Yes forgot to mention that I'm only charging with my BMS.  Will I have to get a 12s BMS to charge in series?
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-03-03T18:25:55.724Z Reads: 48

```
http://i0.wp.com/www.ebikeschool.com/wp-content/uploads/2015/05/bms-diagram.jpg?resize=640%2C454

You can see that the bms and load is in series instead of parallel as you suggested.
You can use any bms as a charging bms as long as you don't exceed the charging amperage
```

---
## \#7 Posted by: Orin635 Posted at: 2018-03-03T18:26:33.596Z Reads: 41

```
So does that mean my diagrams right?
```

---
## \#8 Posted by: bevilacqua Posted at: 2018-03-03T18:26:47.053Z Reads: 42

```
exactly
10char
```

---
## \#9 Posted by: Orin635 Posted at: 2018-03-03T18:27:17.141Z Reads: 41

```
I'd prefer not to have to get a new BMS and charger
```

---
## \#10 Posted by: bevilacqua Posted at: 2018-03-03T18:27:20.806Z Reads: 42

```
no....
10char
```

---
## \#11 Posted by: Orin635 Posted at: 2018-03-03T18:27:40.172Z Reads: 37

```
What do you mean 10char sorry
```

---
## \#12 Posted by: bevilacqua Posted at: 2018-03-03T18:28:12.731Z Reads: 37

```
min 10 Characters: 
"No" is just too short
```

---
## \#13 Posted by: ZackoryCramer Posted at: 2018-03-03T18:28:15.125Z Reads: 37

```
[quote="Orin635, post:7, topic:48044, full:true"]
So does that mean my diagrams right?
[/quote]

No, you are using it in parallel. The vesc would go between the positive leads(or negative depending on your bms).
```

---
## \#14 Posted by: bevilacqua Posted at: 2018-03-03T18:28:42.707Z Reads: 33

```
off topic.....
```

---
## \#15 Posted by: Orin635 Posted at: 2018-03-03T18:28:57.673Z Reads: 31

```
Oh OK thats useful to know
```

---
## \#16 Posted by: ZackoryCramer Posted at: 2018-03-03T18:29:11.760Z Reads: 32

```
How? 
10char
```

---
## \#17 Posted by: Orin635 Posted at: 2018-03-03T18:30:39.237Z Reads: 31

```
I have an esc idk if that changes anything(budget build btw)
```

---
## \#18 Posted by: ZackoryCramer Posted at: 2018-03-03T18:31:15.787Z Reads: 32

```
My bad. As long as it's a load, it goes in series like in the diagram. :sweat_smile:
```

---
## \#19 Posted by: Orin635 Posted at: 2018-03-03T18:31:53.943Z Reads: 30

```
So my diagrams right? Sorry Im so confused here
```

---
## \#20 Posted by: bevilacqua Posted at: 2018-03-03T18:32:07.845Z Reads: 29

```
I suggest you do some research on the forum. 
About using 1 BMS for 2 Lipos in Parallel: I think it is not possible (Please correct me if im wrong)

What is your goal exactly? BMS for charge and discharge? Charge only?
```

---
## \#21 Posted by: Orin635 Posted at: 2018-03-03T18:32:53.217Z Reads: 27

```
I did try but didn't find much information.
```

---
## \#22 Posted by: bevilacqua Posted at: 2018-03-03T18:34:34.326Z Reads: 28

```
Trust me there is.

But still if you don't want to do the research: Get one 12S BMS (Low amperage because charge only) and a 12S Charger
```

---
## \#24 Posted by: Orin635 Posted at: 2018-03-03T18:39:57.633Z Reads: 29

```
Just looked more into. I found this diagram ![0ad944c936a12334832c0247c44f183a77d60577_1_659x500|659x500](upload://uShuUNZTyoxFuG0LgWSHCYvRauQ.png).
```

---
## \#25 Posted by: Orin635 Posted at: 2018-03-03T18:41:04.381Z Reads: 28

```
So you say to put my esc in between the bms and battery
```

---
## \#26 Posted by: ZackoryCramer Posted at: 2018-03-03T18:41:30.324Z Reads: 27

```
OMG I got you wrong bro. The charging port goes in series, and esc is in parallel. :mask: For a charging bms.
```

---
## \#27 Posted by: bevilacqua Posted at: 2018-03-03T18:41:56.954Z Reads: 26

```
yes... thats for discharge, thus power to the ESC. 

I thought you were asking about charging through the BMS + Balance Wire arrangement
```

---
## \#28 Posted by: Orin635 Posted at: 2018-03-03T18:42:15.643Z Reads: 27

```
So what does that mean (sorry I'm really bad at understanding this)
```

---
## \#29 Posted by: Orin635 Posted at: 2018-03-03T18:43:58.665Z Reads: 27

```
Yes I think😂
I'm so confused I'm really sorry.

I think I've drifted of from my original question.
```

---
## \#30 Posted by: ZackoryCramer Posted at: 2018-03-03T18:44:13.408Z Reads: 28

```
![07f87ee6ad53b724faed330904a692cede7cf99f_1_690x345|690x345](upload://rrr7eMwBdriPIskgdy0nxtSvAnM.png)
```

---
## \#31 Posted by: Orin635 Posted at: 2018-03-03T18:45:58.637Z Reads: 28

```
I understand that now. My esc is one of the ebay esc's
```

---
## \#32 Posted by: Orin635 Posted at: 2018-03-03T20:54:05.548Z Reads: 18

```
![IMG_20180303_205039|666x500](upload://4fO6IPuqDc9cWjwpdxhc3hfc3A8.jpg)![IMG_20180303_205044|666x500](upload://cl3tv8h9QzzdgpWdCdlMXbtzrbR.jpg)
```

---
