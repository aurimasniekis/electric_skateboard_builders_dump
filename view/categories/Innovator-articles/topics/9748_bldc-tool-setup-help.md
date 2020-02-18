# Bldc tool setup help

### Replies: 31 Views: 2613

## \#1 Posted by: Sunstart Posted at: 2016-09-17T14:15:30.433Z Reads: 173

```
Hey guys i have a sk3 245kv motor and a 2 3s battery to make 6s battery how do i set up my bldc tool for the vesc. When i go up mabe 5% hill i slow down alot I'm about 270 pounds plz help
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-17T14:19:23.534Z Reads: 176

```
You'll probably need to upgrade to dual motor, and consider going 10s. Current will be high at 6s single, 10s will help with that and so will dual motors. The cheapest thing to do is to just lose weight. 270 pounds at 6s single motor slowing down during hills sounds pretty normal.

It'd be helpful to know your current amp limits as well.
```

---
## \#3 Posted by: Lsalt Posted at: 2016-09-17T23:00:22.728Z Reads: 150

```
You didnt mention your gear/pulley ratio. Id suggest using the  app rc calc and like Jinra said 10s. I'm 250 and tall lol so no weight loss possible bu I'm using 13/36 83mm wheels at 230 kv 10s ...ratio is 2.77 motor turns before wheel makes one complete rotation. I bet you need less teeth on your motor pulley. Although that presents belt slipping under hard brake/acceleration.
```

---
## \#4 Posted by: Sunstart Posted at: 2016-09-18T00:43:39.839Z Reads: 143

```
I have the enertion kit mono Drive
```

---
## \#5 Posted by: Sunstart Posted at: 2016-09-18T00:51:55.250Z Reads: 130

```
I have 2 yuneec E-GO skateboard and i go fast on them full power no problem can i use the battery off of there for my application or i sould just use lipo batterys im a beginner Builder so any information is good information
```

---
## \#6 Posted by: Jinra Posted at: 2016-09-18T01:20:49.754Z Reads: 127

```
what are your amp limits on the VESC?
```

---
## \#7 Posted by: Sunstart Posted at: 2016-09-18T03:10:23.004Z Reads: 125

```
Where do i find amp limits
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-18T04:16:30.323Z Reads: 126

```
In bldc tool. Have you not configured it yet? You're supposed to configure the VESC depending on your setup and motor before you ride with it. Just hook up the mini usb to your computer and connect your battery. Open BLDC tool on your computer and configure.
```

---
## \#9 Posted by: Sunstart Posted at: 2016-09-18T05:31:45.118Z Reads: 122

```
<img src="/uploads/db1493/original/3X/d/e/de8695ea26b5e075266b02471dde5d6aca7aaa5b.jpg" width="690" height="388">
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-18T06:09:15.971Z Reads: 116

```
raise your battery max to 40-50a if it's within spec of your battery. 80a motor max seems a bit high, you can probably lower that to 60. Change max input voltage back to default (57v).
```

---
## \#12 Posted by: Sunstart Posted at: 2016-09-18T12:07:02.492Z Reads: 110

```
I have 2 3s turnigy 5000 mah 25-35 discharge
```

---
## \#13 Posted by: Jinra Posted at: 2016-09-18T12:11:54.625Z Reads: 109

```
I'm going to assume you mean 25-35C, in which case yea raise your battery max to 40-50 and see how it goes.
```

---
## \#14 Posted by: Lsalt Posted at: 2016-09-18T21:32:57.306Z Reads: 104

```
You have 15/36 that's 2.4 turns . Drop your motor pulley to 13 or 12 teeth. 5 amps times 25c rate is 125 amp discharge. In which case you can make your batt max match your motor max. Although I have heard you should make sure you have good cooling around your vesc
```

---
## \#15 Posted by: Sunstart Posted at: 2016-09-18T22:49:06.510Z Reads: 99

```
Where can i buy motor pulley from
```

---
## \#16 Posted by: Lsalt Posted at: 2016-09-18T23:01:40.368Z Reads: 98

```
Either from enertion or from . make sure it matches the width of your belt
```

---
## \#17 Posted by: Sunstart Posted at: 2016-09-19T00:26:54.144Z Reads: 96

```
I just did a 9s battery it pulled me up a hill like 10 % not at full power not pushing the trigger all the way. Ill do more testing and get back to you
```

---
## \#18 Posted by: Lsalt Posted at: 2016-09-19T03:50:21.017Z Reads: 94

```
Did you raise your batt max vesc setting
```

---
## \#19 Posted by: Sunstart Posted at: 2016-09-19T16:26:18.116Z Reads: 83

```
I have it set to 50a is that ok or i need to pick it up more
```

---
## \#20 Posted by: Sunstart Posted at: 2016-09-19T16:59:43.422Z Reads: 87

```
I did some testing last night it go's full power up a hill for a little bit and slows down alot like the motor was going to stop the motor was warm not to hot vesc was warm to. The batteries where at 12 volts for the 3 3s batteries mabe i need to change some settings in the bldc tool.
```

---
## \#21 Posted by: Lsalt Posted at: 2016-09-19T18:28:14.368Z Reads: 85

```
50 is a safe bet with vesc. You can experiment with higher just be careful. You said your batteries were at 12 volts total? Did you parrallel them or run them in series? You had mentioned 9s before, that would be around 36 volts...I would really suggest reading everything you can about batteries, motor kv in correlation to gear ratios and wheel size. Either way for your weight and motor kv regardless of what batteries you use, which is still important, your gear ratio is too much for your weight. Like I said I have 230 kv and 13 teeth on motor pulley and 36 teeth on drive wheel. I weigh 250. On 10s (series) setup. You need to have more than enough power  and torque so when you do go at regular speed you can have head room to go up hills and such....
```

---
## \#22 Posted by: Lsalt Posted at: 2016-09-19T18:30:47.964Z Reads: 83

```
Since your motor is a higher kv you may need to have an even smaller pull on it like 12. It's just that with your weight you can floor it or slam on the break too hard because your belt can slip over the teeth easier.
```

---
## \#23 Posted by: Sunstart Posted at: 2016-09-19T19:16:48.559Z Reads: 79

```
I can make it up hill if i dont slow down on them but going to do what u say and get the 12t.
```

---
## \#24 Posted by: Sunstart Posted at: 2016-09-19T19:17:58.250Z Reads: 79

```
Or im going get 13t ill see what i can find
```

---
## \#25 Posted by: michaeld33 Posted at: 2016-09-19T21:24:20.996Z Reads: 73

```
12T won't work though, that's the issue, if you need more torque, get a bigger motor, but going that small in pulley size is gonna cause problems. You should probably go with at least 14.
```

---
## \#26 Posted by: Lsalt Posted at: 2016-09-19T23:29:29.873Z Reads: 65

```
Michael is right. If you can afford it, get a lower kv motor. However if not, he weighs 270 lbs. I weigh 250 lbs on 230 kv 10s 83mm and rarely skip teeth on 13t. Michael, add some sand bags to your board and try his setup, then recommend. I would try buying a couple of different pulleys. Then trying them. Twenty bucks or 80 for new motor. I think he is trying to make what he has work though.
```

---
## \#27 Posted by: michaeld33 Posted at: 2016-09-20T02:22:44.731Z Reads: 59

```
God man I feel like you're stalking me (kidding :stuck_out_tongue_closed_eyes:)

I'm not saying my board works for everyone. If you want a 6S 20:36 ratio on your board, you will need dual drive, anyone over 140lbs will probably. I'm just saying I think if the option is available get the bigger motor and use a ratio which will benefit the belt more.
```

---
## \#28 Posted by: Lsalt Posted at: 2016-09-20T02:35:00.168Z Reads: 56

```
Lol. Funny. Yup dual drive would work
```

---
## \#29 Posted by: Bfreak Posted at: 2016-09-28T15:41:13.241Z Reads: 59

```
HI there Folks, hoping someone can help me with a BLDC setup issue.

I have my controller connected, via PPM, using current no reverse with brake. I have configured min and max pulsewidth, so all looks good. 

When I push the stick forward, the motor accelerates smoothly all the way to full speed. HOWEVER, it does this when i even hold the stick just past idle, at 1% input. I can't hold the throttle at a certain speed, it just accelerates too 100%!

With braking, this does not seem to happen, it can be controlled properly.

All help is appreciated! Thanks.
```

---
## \#30 Posted by: TheImmortalJew Posted at: 2016-09-28T15:50:54.951Z Reads: 55

```
I'm assuming your doing this on the bench with no load....that is normal behavior. It will be more smooth accelerating when you have weight on the board.
```

---
## \#31 Posted by: Sunstart Posted at: 2016-12-06T00:22:28.752Z Reads: 42

```
Im back did alot of testing and have it all the same settings  the only problem i had is heat on the vesc that's why I couldn't make it uphill so I brought Mini aluminum heat sink to get the heat out with a small fan to cool it down it works beautifully
```

---
## \#32 Posted by: Ackmaniac Posted at: 2016-12-06T01:13:21.283Z Reads: 40

```
Set the maximum input voltage to 57V. Doesn't matter which kind of battery you have. And do you have those 3 batteries in parallel or in series. Because you have to put them in series for your weight so that the battery becomes a 9S. Then also adjust the battery start and cutoff voltage to be safe.
I think the best would be you post some screenshots of your settings again. Please also from the BLDC tab, not only the general tab.
```

---
