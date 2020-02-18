# Can 245kv and 260kv motors be used at 10S with VESC

### Replies: 25 Views: 3003

## \#1 Posted by: willpark16 Posted at: 2016-12-01T06:31:28.698Z Reads: 200

```
So I talked to my friend and will soon have a brand new enertion vesc 4.12 not sure about batch or anything. My only question is I currently am running a 10s 3p li ion pack with a tb esc and tacon 245kv, I also have a nearly new 260kv sk3, my only question is do I need to sell these motors or can I run them safely with my new vesc. I know about limiting rpm but this is more so a question of not overstressing the components to the point where I fry them going 25mph
```

---
## \#2 Posted by: Tuomalar Posted at: 2016-12-01T06:38:14.201Z Reads: 196

```
Yes, but lower voltage battery than 10s. If I calc it right 8s should be fine.
```

---
## \#3 Posted by: Maxid Posted at: 2016-12-01T06:38:23.799Z Reads: 191

```
Not sure what that title has to do with your question.
```

---
## \#4 Posted by: willpark16 Posted at: 2016-12-01T06:40:36.295Z Reads: 185

```
im uprgrading the 12s tb esc to a vesc
```

---
## \#5 Posted by: willpark16 Posted at: 2016-12-01T06:41:26.923Z Reads: 181

```
cant switch the battery only esc and motor unless i wanna run 6s4p but i think 10s has way more efficiency
```

---
## \#6 Posted by: saul Posted at: 2016-12-01T07:48:35.555Z Reads: 166

```
yea those are too high kv for 10s, 190's work well.

I would hold on to the tacon tho, those are rare now.
```

---
## \#7 Posted by: Maxid Posted at: 2016-12-01T08:04:36.211Z Reads: 161

```
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#8 Posted by: Namasaki Posted at: 2016-12-01T14:52:15.329Z Reads: 144

```
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#9 Posted by: aigenic Posted at: 2016-12-01T14:56:49.407Z Reads: 137

```
Would it be possible to use 10s with 245kv motor and change gearing ration to lower the max speed and increase torque?
```

---
## \#10 Posted by: LukeL Posted at: 2016-12-01T15:21:47.681Z Reads: 135

```
I don't think gear ratio would effect it, it's about the max ERPM so only the motor side max rpm matters not the wheel rpm. you can limit the max ERPM with the BLDC tool but no one seems to know what the vesc does when you reach this limit, whether it just cruises or shuts off.
```

---
## \#11 Posted by: LukeL Posted at: 2016-12-01T15:39:47.968Z Reads: 129

```

I have been using 240Kv with 10S lipo for over month it's been fine but i haven't tried to test top speed which is when i think problems would occur. I have set the max ERPM setting to 60,000 which is the recommended max.

If all your other components are the same as someone with 190Kv 10S setup and they can reach 25mph then so can you without frying anything, the problem is that a 245Kv can reach higher RPM with same max voltage which fries the drv chip so you can either try to stay under a certain speed or use the settings in BLDC tool

The point of choosing a motor battery combo that stays under the 60,000 ERPM limit is that there is no chance of frying the drv (you're not relying on yourself/software to stay under it) and i guess your not paying for more than you need
```

---
## \#12 Posted by: Namasaki Posted at: 2016-12-01T16:04:55.468Z Reads: 121

```
You should get 25mph easily with 10s and 190kv. 
That's a safe setup for Vesc.
```

---
## \#13 Posted by: Rob69de Posted at: 2016-12-08T01:13:24.808Z Reads: 97

```
I have been running a tb 245kv motor with a vesc at 10s
For about 3 months,and put about 120miles on it without 
So much as a slight problem..
```

---
## \#14 Posted by: willpark16 Posted at: 2016-12-08T01:35:01.175Z Reads: 91

```
What vesc?
```

---
## \#15 Posted by: Rob69de Posted at: 2016-12-08T18:20:55.107Z Reads: 83

```
Tb vesc 4.12
```

---
## \#16 Posted by: willpark16 Posted at: 2016-12-08T18:23:20.481Z Reads: 82

```
ill need to talk to tb about his stock i have about 130 to spend on vesc rn and have been offered 2 brand new enertion 4.12vesc for 65  a piece
```

---
## \#17 Posted by: Rob69de Posted at: 2016-12-08T18:28:52.118Z Reads: 82

```
I'm not particularly fond of enertions vesc.
Even though I have never lost a tb vesc, and i have two in current use, however for my e-mtb i bought a ollin vesc
```

---
## \#18 Posted by: willpark16 Posted at: 2016-12-08T18:31:55.170Z Reads: 79

```
preference on reliability? and is the 245kv an sk3?
```

---
## \#19 Posted by: saul Posted at: 2016-12-08T18:32:28.314Z Reads: 80

```
This is a good deal! I have a really early enertion vesc working fine. they are most likely from maytech anyways..
```

---
## \#20 Posted by: willpark16 Posted at: 2016-12-08T18:36:13.952Z Reads: 76

```
fair enough id just like a reliable vesc that can handle ur motor
```

---
## \#21 Posted by: saul Posted at: 2016-12-08T18:42:39.890Z Reads: 74

```
well yea i've just been using one from enertion, and one from diy. both earlier batches but I think quality has improved if anything.
```

---
## \#22 Posted by: willpark16 Posted at: 2016-12-08T18:45:10.167Z Reads: 71

```
i havenet heard as many bad reviews from the improved enertion 4.12 i think people just hate wait times so hence the bad reviews
```

---
## \#23 Posted by: saul Posted at: 2016-12-08T18:53:32.000Z Reads: 68

```
yea thats true. i waited for months and months for both of them....they are finally in stock now, or should be.
```

---
## \#24 Posted by: willpark16 Posted at: 2016-12-08T18:58:03.674Z Reads: 67

```
so enertion or diy
```

---
## \#25 Posted by: Rob69de Posted at: 2016-12-09T04:30:16.037Z Reads: 58

```
There was a survey taken on vesc failures,somewhere 
In the forum 
It lists vesc's from various brands,and the failure rate,
Asside from ollin's vesc being least prone to fail.
I do believe tb did very well.
```

---
