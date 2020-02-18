# Single 3S Viable?

### Replies: 19 Views: 1108

## \#1 Posted by: chinzw Posted at: 2016-08-26T02:36:28.576Z Reads: 146

```
Hey guys, so i had a pretty bad accident last Friday, when my remote went unresponsive and my board went full throttle. I had to bail and ended up with very bad road rash on my elbows, hands and hips. After thinking this through, i want to make sure this doesn't happen again, so im willing to sacrifice speed for peace of mind. I currently run 2x3s lipos which give me about 40km/h (so pretty bad for full throttle unresponsive board). What i was thinking is using just one 3s lipo, which in theory should give me half the speed, but im not sure how torque would be affected, etc.
Any insight on this would be very much appreciated!

Thanks!
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-08-26T03:04:07.705Z Reads: 139

```
Heal fast....


I find that 4s actually works pretty ok...

Less speed less torque
```

---
## \#3 Posted by: Chris_KP Posted at: 2016-08-26T03:05:51.086Z Reads: 137

```
Torque and speed will be cut in half.
you could keep at 6s and just gear down so you get more torque but less speed
```

---
## \#4 Posted by: chinzw Posted at: 2016-08-26T03:10:08.194Z Reads: 136

```
[quote="Chris_KP, post:3, topic:8352, full:true"]
Torque and speed will be cut in half.
you could keep at 6s and just gear down so you get more torque but less speed
[/quote]

Im using 16t, i dont think i will be able to get 8t pulley for this
```

---
## \#5 Posted by: saul Posted at: 2016-08-26T03:23:49.756Z Reads: 128

```
14t will drop speed by a decent amount. any smaller and the belt will skip.

I'm more curious about why the remote cut out.
what remote and esc are you using?
```

---
## \#6 Posted by: chinzw Posted at: 2016-08-26T03:24:57.322Z Reads: 126

```
[quote="saul, post:5, topic:8352, full:true"]
14t will drop speed by a decent amount. any smaller and the belt will skip.

I'm more curious about why the remote cut out.
what remote and esc are you using?
[/quote]

Im using a HK GT2-E with a Turnigy 150A ESC
```

---
## \#7 Posted by: treenutter Posted at: 2016-08-26T05:43:05.354Z Reads: 112

```
@chinzw sorry to hear about the accident. Hope you're doing OK. If you're using a VESC, just use the ERPM limits to control your max speed. Then you can keep the torque of 6S. EDIT: sorry I see that you're not using VESC.
```

---
## \#8 Posted by: sl33py Posted at: 2016-08-26T06:38:44.237Z Reads: 104

```
Hey @chinzw - like @treenutter said - if you can swing $ it VESC might be a good solution with limited ERPM (max rpm = set a max speed).

I also would gear down to 14t - no lower than 13t.  If you have a single setup 12 or 15mm wide belt helps with less skipping, but still pushing it and almost impossible to avoid skipping on 9mm w/ 12t no matter how tight the belt.
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2016-08-26T06:49:20.491Z Reads: 96

```
It should work but connect the batteries in parallel instead of in series. Also sounds like you have a failsafe issue. You should be able to turn off remote and the motors go to neutral
```

---
## \#10 Posted by: Cptanpanic Posted at: 2016-08-26T09:33:59.376Z Reads: 92

```
Not sure about turnigy ESC, but at least with FVT one you can limit max throttle percentage.
```

---
## \#11 Posted by: chinzw Posted at: 2016-09-02T18:12:09.079Z Reads: 78

```
So i got a new controller (GT2b, now it cuts off after 1 second instead of 5). The Turnigy 150A ESC doesnt have a throttle or rpm limit, so i have no way of limiting speed.

I tried 3s and it did work pretty good, the only time i had some trouble was going up a very steep ramp from a dead start.

What im wondering if there's any issues from using 3s, like if something can get damaged?
```

---
## \#12 Posted by: Stevemk14ebr Posted at: 2016-09-02T18:37:58.111Z Reads: 67

```
Your amp draw will quadruple I believe, so your board will get much hotter. Just change your gearing, 3s is very inefficient
```

---
## \#13 Posted by: chinzw Posted at: 2016-09-02T18:45:18.730Z Reads: 64

```
I just ordered a VESC from @torqueboards, ill go back to 6s and just use the limiter, plus i think the VESC will handle any sort of fault much better than the turnigy 150a
```

---
## \#14 Posted by: racidon Posted at: 2016-09-03T06:37:16.484Z Reads: 57

```
Just so you know too that GT2B has a failsafe much like that of the Winning remote, so if it's not setup right and it drops out it will go full throttle so you'll need to fix that :slight_smile:
```

---
## \#15 Posted by: sl33py Posted at: 2016-09-03T07:56:34.652Z Reads: 56

```
[quote="racidon, post:14, topic:8352"]
Just so you know too that GT2B has a failsafe much like that of the Winning remote, so if it's not setup right and it drops out it will go full throttle so you'll need to fix that :slight_smile:
[/quote]


Huh - learn something new every day...  have a link to the steps to configure?  I've been riding for over a year on GT2b and not done this.  Luckily it's a rock solid connection and i haven't had any issue, but would like to configure it correctly for the behavior i want at interruption.

Thanks @racidon!!
```

---
## \#16 Posted by: racidon Posted at: 2016-09-03T07:59:43.895Z Reads: 57

```
[quote="sl33py, post:15, topic:8352, full:true"]
[quote="racidon, post:14, topic:8352"]
Just so you know too that GT2B has a failsafe much like that of the Winning remote, so if it's not setup right and it drops out it will go full throttle so you'll need to fix that :slight_smile:
[/quote]


Huh - learn something new every day...  have a link to the steps to configure?  I've been riding for over a year on GT2b and not done this.  Luckily it's a rock solid connection and i haven't had any issue, but would like to configure it correctly for the behavior i want at interruption.

Thanks @racidon!!
[/quote]

When I get my new VESC from Chaka I'll try to set it up to cause the full throttle and then attempt to fix it.
But if I remember right I got my reading from full brake and put this as min PWM and then full throttle as max PWM I then used the trim to get a solid 50% readout. That's the only difference I had with that VESC vs my First one that I didn't trim it etc and when I turned it off before the board it would cause full throttle
```

---
## \#17 Posted by: Titoxd10001 Posted at: 2016-09-03T14:46:24.038Z Reads: 50

```
To set failsafe on gt2b and vesc you need to set throttle trim so it reads 50℅ in neutral when turned on. There is a failsafe button on the gt2b receiver that you press and it makes the neutral you just set as the neutral when it turns off. So now when you turn off your remote it should stay at 50℅ when viewing in bldc tool.(if your doing a 3d printed case you want to make sure you limit the amount of the brake travel on the trigger rather then setting a lower pulsewidth)
```

---
## \#18 Posted by: DivenParker Posted at: 2016-10-18T06:02:35.175Z Reads: 24

```
If you use a single 3s lipo battery, it may not only reduce your speed, and reduce your running time.when  2x3s lipo battery in Parallel, its voltage is still 3s 11.1v, you can try to use a 4s lipo battery or others, I'm not sure which do you need, you'd better have a deep think about it .
```

---
## \#19 Posted by: chinzw Posted at: 2016-10-18T06:10:40.319Z Reads: 21

```
Got a VESC so i can limit ERPM, stuck to 6s which works just fine :slight_smile:
```

---
