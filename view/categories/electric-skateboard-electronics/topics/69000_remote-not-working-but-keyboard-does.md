# Remote not working but keyboard does

### Replies: 39 Views: 420

## \#1 Posted by: dg798 Posted at: 2018-09-23T22:02:58.171Z Reads: 100

```
Ever since I got some water on my vesc my remote hasn’t been working however when I plug it in to the vesc tool there are no faults and I can use the keyboard to control the motor but the remote doesn’t work. I already went to the ppm settings and everything is fine. I had an extra receiver lying around so I tried that one as it came from a different mini remote I don’t have anymore but that still doesn’t work. Is it possible the ppm port on the vesc is the problem?
```

---
## \#2 Posted by: dg798 Posted at: 2018-09-26T02:02:28.201Z Reads: 82

```
can anyone help me please
```

---
## \#3 Posted by: threebysix Posted at: 2018-09-26T02:05:52.981Z Reads: 78

```
Looks around where the ppm port and see if you can identify any shorts or signs of water damage?
```

---
## \#4 Posted by: dg798 Posted at: 2018-09-26T02:10:25.630Z Reads: 77

```
i did it doesnt look like any shorts and no burn marks
```

---
## \#5 Posted by: mmaner Posted at: 2018-09-26T02:30:49.329Z Reads: 72

```
[quote="dg798, post:1, topic:69000"]
Is it possible the ppm port on the vesc is the problem?
[/quote]

Its possible but its more likely the RX is just messed up from water damage.
```

---
## \#6 Posted by: mmaner Posted at: 2018-09-26T02:31:12.321Z Reads: 68

```
Borrow another remote and receiver from someone and test to see if thats the case.
```

---
## \#7 Posted by: dg798 Posted at: 2018-09-26T02:32:09.894Z Reads: 67

```
ok i will try that and post back soon
```

---
## \#8 Posted by: dg798 Posted at: 2018-09-27T02:05:27.855Z Reads: 60

```
So I tried a different remote and still nothing. I realized that when I turn in the vesc the blue and green light stay on all the time. Isn’t the green light supposed to only go on when you add throttle. Here’s a pic![image|666x500](upload://zsSXvzYXJe2Xzt99VvJxBJm36Xu.jpeg)
```

---
## \#9 Posted by: dg798 Posted at: 2018-09-27T02:09:46.304Z Reads: 59

```
when i use the keyboard the green light just gets a little lighter
```

---
## \#11 Posted by: dg798 Posted at: 2018-09-27T02:18:47.448Z Reads: 57

```
now periodically the keyboard works but then it will stop working and the motor will stutter
```

---
## \#12 Posted by: dg798 Posted at: 2018-09-27T02:20:55.884Z Reads: 56

```
now when i unplugged the receiver from the vesc the keyboard works. is the ppm port possibly the problem
```

---
## \#13 Posted by: mmaner Posted at: 2018-09-27T02:49:30.115Z Reads: 51

```
I have no clue. 8d talk to @JohnnyMeduse, see what he says.
```

---
## \#14 Posted by: dg798 Posted at: 2018-09-27T02:51:27.111Z Reads: 52

```
@JohnnyMeduse can you please try to help me out here if i have to replace me vesc or something.
Thanks
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-09-27T03:01:09.394Z Reads: 51

```
Do you have a Multimeter ?? Could you check if R20 is 10Kohms
```

---
## \#16 Posted by: dg798 Posted at: 2018-09-27T03:01:28.716Z Reads: 48

```
sure will check now
```

---
## \#18 Posted by: dg798 Posted at: 2018-09-27T03:04:16.338Z Reads: 47

```
nevermind found it.
```

---
## \#19 Posted by: dg798 Posted at: 2018-09-27T03:05:08.353Z Reads: 47

```
its 9.87k. Is that good or bad?
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2018-09-27T15:18:26.481Z Reads: 42

```
that good... humm can you post your setting?
```

---
## \#21 Posted by: dg798 Posted at: 2018-09-27T19:40:36.672Z Reads: 39

```
Also the green light doesn’t blink 3 times when it starts up.
![image|354x142](upload://cQn9mhKwrBHmVkS09dc84lVskHr.jpeg)
```

---
## \#22 Posted by: b264 Posted at: 2018-09-27T19:59:58.688Z Reads: 40

```
What software are you using?
```

---
## \#23 Posted by: dg798 Posted at: 2018-09-27T20:02:48.083Z Reads: 35

```
3.38
10 charc
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2018-09-27T20:04:30.354Z Reads: 36

```
I need the parameter from the vesc tools
```

---
## \#25 Posted by: dg798 Posted at: 2018-09-27T20:06:44.522Z Reads: 36

```
I can get you that tonight. Don’t have a laptop now. 
Do u want the app parameters or the motor parameters
```

---
## \#26 Posted by: dg798 Posted at: 2018-09-28T03:20:12.247Z Reads: 36

```
![image|375x500](upload://oGD0bd7ucR3VhqCEgaqTtQltrgn.jpeg) ![image|375x500](upload://14SyntlsQSlxPR31FvF4AQrwEck.jpeg) ![image|374x500](upload://hyGwLLz1hgffvRnEXsajNsYG5hs.jpeg) ![image|375x500](upload://exiX7r1hFr7DIgEXqlanlYeng1k.jpeg) ![image|375x500](upload://z15dD7kAQYvzwWlD7xmXG2Wqk7u.jpeg) ![image|374x500](upload://72hH1waBpBRsVRtFGJAFprsJrUt.jpeg)
```

---
## \#27 Posted by: TowerCrisis Posted at: 2018-09-28T03:25:18.613Z Reads: 32

```
Just to check, you have done a full cleaning of the vesc right? Like after you got it wet you used alcohol to clean it up and remove any possible corrosion?
```

---
## \#28 Posted by: dg798 Posted at: 2018-09-28T03:29:24.372Z Reads: 32

```
No I just riced it. Should I use alcohol pads
```

---
## \#29 Posted by: dg798 Posted at: 2018-09-28T03:48:20.735Z Reads: 32

```
just used alcohol pads on them. @JohnnyMeduse can you see anything wrong with my vesc settings
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2018-09-28T03:51:01.654Z Reads: 31

```
Can you check the PPM tabs?
```

---
## \#31 Posted by: dg798 Posted at: 2018-09-28T03:57:57.484Z Reads: 29

```
thats one of the pics
```

---
## \#32 Posted by: dg798 Posted at: 2018-09-28T04:07:22.053Z Reads: 28

```
oh you mean the ppm mapping tab. I will do that tommorrow morning as its midnight already and i have to get to bed.
thanks
```

---
## \#33 Posted by: dg798 Posted at: 2018-09-28T15:45:51.749Z Reads: 26

```
![image|375x500](upload://wMYXy8Gqdyiz23f2KS4GbJaE4NQ.jpeg)
```

---
## \#34 Posted by: dg798 Posted at: 2018-09-28T17:49:09.628Z Reads: 22

```
Is that what u are looking for @JohnnyMeduse?
```

---
## \#35 Posted by: indyglassman Posted at: 2018-09-28T19:49:25.720Z Reads: 22

```
Following:  I'm having what seems to be the same issue.  
I got a new TB VESC and a 6355 motor.  Upgraded the firmware from VESC tools, confirmed it's updated.  Went through wizard and verified motor works by using keyboard.  However, when connected to my mini remote / receiver it will not turn the motor.   I've confirmed that the receiver is working by connecting a servo.  I've also tried another servo lead between the receiver & VESC.   May be the same issue as dg798's??
```

---
## \#36 Posted by: JohnnyMeduse Posted at: 2018-09-28T19:57:34.785Z Reads: 22

```
Yeah but I don't really see anything... Have you try to go back to 2.18 firware?
```

---
## \#37 Posted by: dg798 Posted at: 2018-09-28T20:08:08.110Z Reads: 21

```
No how do I go back and is it dangerous to do
```

---
## \#38 Posted by: indyglassman Posted at: 2018-09-29T02:44:25.180Z Reads: 21

```
Just updating my post since I had the same issue.  Mine ended up being resolved by going through the input setup wizard.  This was my first time ever using the software and I wasn't sure what steps were required.  After setting it to PPM with brake the remote now works.   
Hope you get yours worked out soon!
```

---
## \#39 Posted by: dg798 Posted at: 2018-09-30T00:01:14.975Z Reads: 18

```
Hope so too. Any other possible problems that u can think of @JohnnyMeduse??
```

---
## \#40 Posted by: dg798 Posted at: 2018-09-30T19:17:17.918Z Reads: 15

```
I’m stupid. This whole time the ppm cable was on the 3rd channel not the second channel. After I connected it to channel 2 it started working fine. Sorry for all the trouble guys.
```

---
## \#41 Posted by: Volts Posted at: 2018-10-30T06:49:23.872Z Reads: 11

```
I'm having this same problem, only it was working fine till I charged my battery with the controllers in the circuit so charging while the controllers were on, now my ppm remote doesn't work, I thought it was a broken remote but I bought another one and still the same thing, going to try it with the UART remote from eboardshop see if that works, but if it doesn't i really don't know what to do?
```

---
