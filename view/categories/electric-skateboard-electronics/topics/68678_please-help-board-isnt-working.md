# Please help&hellip;&hellip; board isn&rsquo;t working :(

### Replies: 47 Views: 348

## \#1 Posted by: KeivanM Posted at: 2018-09-20T20:56:59.618Z Reads: 110

```
Hello, sorry for the desperate title but I need help, my board is not working and im not sure what the problem is. I rode it yesterday and all of a sudden it just stopped working, I am not sure if the FOC BOXes are fried or if its just a simple fix but yeah.![IMG_5466|666x500](upload://A5g4piOP7uB9n74zOMfFHkdk8D6.jpeg) ![IMG_5469|375x500](upload://eAoHo4gAMGCqCZxVIo6wh0NJaN7.jpeg) 


the lights on both FOC BOX's are lit up, both power and signal, the controller lit up too. im not sure whats wrong here...please help me!
```

---
## \#2 Posted by: yelnats8j Posted at: 2018-09-20T20:59:12.086Z Reads: 105

```
Check all you connection, and can you give us a little more detail?
```

---
## \#3 Posted by: KeivanM Posted at: 2018-09-20T21:02:03.667Z Reads: 100

```
I double checked all the connections and made sure they were tight. Maybe the phase leads came off during my ride? would that do anything? 

Some more info I can provide is the board is a 12s4p, 97mm, 18T/36T, with two sk3 192kv motors and i have [this](collections/remote-controller/products/torqueboards-2-4ghz-mini-remote-controller) controller.
```

---
## \#4 Posted by: KeivanM Posted at: 2018-09-20T21:02:58.732Z Reads: 96

```
I am also connecting the two FOC BOX's with a canbus and i have it configured to have a master vesc and a slave one and the master one is the one that has the controller receiver connected to
```

---
## \#5 Posted by: yelnats8j Posted at: 2018-09-20T21:05:25.139Z Reads: 97

```
check the phase wires
```

---
## \#6 Posted by: KeivanM Posted at: 2018-09-20T21:08:28.314Z Reads: 97

```
i just checked, they have a solid connection, i feel like theres a problem with the controller, how can i verify this?
```

---
## \#7 Posted by: yelnats8j Posted at: 2018-09-20T21:09:40.673Z Reads: 99

```
Plug in the VESC to a computer and check for faults using the Tool
```

---
## \#8 Posted by: KeivanM Posted at: 2018-09-20T21:10:42.996Z Reads: 99

```
how do i do that?
```

---
## \#9 Posted by: TowerCrisis Posted at: 2018-09-20T21:11:51.408Z Reads: 99

```
When the board is on and your USB is connected to the controller, open up the terminal in the vesc tool and type"faults" without quotes.

It should display any issues it detects.
```

---
## \#10 Posted by: Blasto Posted at: 2018-09-20T21:11:56.288Z Reads: 98

```
sounds like no motor detection was performed
```

---
## \#11 Posted by: KeivanM Posted at: 2018-09-20T21:12:41.451Z Reads: 94

```
it says "No faults registered since startup"
```

---
## \#12 Posted by: KeivanM Posted at: 2018-09-20T21:13:03.643Z Reads: 91

```
what does that mean and what did it to to the board
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-09-20T21:13:06.637Z Reads: 90

```
He set them up in a master slave config so I'm sure he actually programmed them
```

---
## \#14 Posted by: TowerCrisis Posted at: 2018-09-20T21:13:44.741Z Reads: 91

```
Connect your remote and view the live data. Is your board registering any throttle? The green bar should increase and decrease for throttle and brake.
```

---
## \#15 Posted by: Battosaii Posted at: 2018-09-20T21:14:10.540Z Reads: 91

```
When you give throttle do the lights change on the Focbox? If not there is a problem with the receiver
```

---
## \#16 Posted by: KeivanM Posted at: 2018-09-20T21:14:17.652Z Reads: 88

```
its not showing any throttle what so ever
```

---
## \#17 Posted by: KeivanM Posted at: 2018-09-20T21:14:35.553Z Reads: 89

```
no lights change.
```

---
## \#18 Posted by: yelnats8j Posted at: 2018-09-20T21:14:52.092Z Reads: 89

```
Check you remote connection
```

---
## \#19 Posted by: Battosaii Posted at: 2018-09-20T21:15:04.997Z Reads: 87

```
That means the Focbox is not getting a signal from the receiver
```

---
## \#20 Posted by: TowerCrisis Posted at: 2018-09-20T21:16:02.978Z Reads: 87

```
Ding ding ding!
```

---
## \#21 Posted by: KeivanM Posted at: 2018-09-20T21:16:49.955Z Reads: 88

```
![IMG_5470|375x500](upload://lEducqxZnzpoUmHy2u8Qfg90243.jpeg) ![IMG_5472|375x500](upload://xWb8lAzFysUbC8x8MJhlNe8EM6n.jpeg) ![IMG_5471|375x500](upload://p8OFQwS9Pcf8biGfWPmxSOLN76g.jpeg) 


here is the controller i am using, I dont see any problems with it at all, is the problem from the focbox not being able to receive a signal?
```

---
## \#22 Posted by: Battosaii Posted at: 2018-09-20T21:17:38.956Z Reads: 85

```
Make sure the receiver plug is on the right way
```

---
## \#23 Posted by: psychotiller Posted at: 2018-09-20T21:18:16.517Z Reads: 84

```
Is your receiver wire from the master or the slave vesc plugged in? Is it plugged in backwards?
```

---
## \#24 Posted by: Blasto Posted at: 2018-09-20T21:19:15.283Z Reads: 82

```
![image|458x349](upload://jH792LMjo3I3mC7zefJ1rbEkiuO.jpeg) 

dont remember the exact pinout of the mini remote receiver.... pretty darn sure this is not right
```

---
## \#25 Posted by: KeivanM Posted at: 2018-09-20T21:19:49.667Z Reads: 82

```
i have it plugged into the master and its connected correctly, from left to right it should be black to white right?
```

---
## \#26 Posted by: psychotiller Posted at: 2018-09-20T21:20:54.662Z Reads: 82

```
It needs to be on channel 2. And if the bind plug wasn't pulled out after the first binding, then board turned off, binding needs to be done again.

after you do the binding procedure, pull the bind plug out.
```

---
## \#27 Posted by: Blasto Posted at: 2018-09-20T21:21:43.835Z Reads: 83

```
the header seems to be shifted 1 pin
```

---
## \#28 Posted by: Mikenopolis Posted at: 2018-09-20T21:22:28.626Z Reads: 85

```
Does that receiver have 4 pins per row?
```

---
## \#29 Posted by: psychotiller Posted at: 2018-09-20T21:23:23.243Z Reads: 82

```
No. He just has it plugged into channel 1
```

---
## \#30 Posted by: KeivanM Posted at: 2018-09-20T21:23:27.051Z Reads: 80

```
Okay I got it working now wow I want to thank everyone who helped me!!!
```

---
## \#31 Posted by: KeivanM Posted at: 2018-09-20T21:23:48.215Z Reads: 81

```
Yall are the best 
:grinning:
```

---
## \#32 Posted by: Blasto Posted at: 2018-09-20T21:24:48.341Z Reads: 80

```
[quote="KeivanM, post:12, topic:68678, full:true"]
what does that mean and what did it to to the board
[/quote]

you really should do a motor detection...  or you might blow them for real
```

---
## \#33 Posted by: KeivanM Posted at: 2018-09-20T21:25:31.453Z Reads: 79

```
another quick question, what are the maximum setting for: 

motor current max
motor current max brake 
motor current max
battery current regen


on this build?
```

---
## \#34 Posted by: KeivanM Posted at: 2018-09-20T21:25:42.156Z Reads: 78

```
how would i enable that?
```

---
## \#35 Posted by: KeivanM Posted at: 2018-09-20T21:27:16.989Z Reads: 78

```
setup is 
12s4p on samsung 30qs 
192kv sk3  6374 ( Max Loading:  **80A**Max Power:  **4032W**)
97mm
36/18 ratio
```

---
## \#36 Posted by: Saturn_Corp Posted at: 2018-09-20T21:27:41.434Z Reads: 74

```
Under the bldc tab at the bottom there's a button to run motor detection. Do that and apply the values on each focbox.
```

---
## \#37 Posted by: KeivanM Posted at: 2018-09-20T21:28:35.306Z Reads: 74

```
it said detection failed
```

---
## \#38 Posted by: Saturn_Corp Posted at: 2018-09-20T21:29:38.522Z Reads: 71

```
Hmm. Not sure what that means. I've only detected 2 motors in my lifetime so perhaps someone else can help you out.
```

---
## \#39 Posted by: Blasto Posted at: 2018-09-20T21:33:19.611Z Reads: 72

```
you should look at some video tutorials... there's a bunch on tube
```

---
## \#40 Posted by: Mikenopolis Posted at: 2018-09-20T21:49:28.302Z Reads: 68

```
[quote="KeivanM, post:37, topic:68678"]
detection failed
[/quote]

trying increasing the D (duty) value in that motor detection area.

go from 0.05 to 0.10
```

---
## \#41 Posted by: KeivanM Posted at: 2018-09-20T21:52:28.809Z Reads: 64

```
after clicking the play button i got this:


Detection results:

Integrator limit: 105.76

BEMF Coupling: 971.72

Unknown hall error: 255



do i click apply now?
```

---
## \#42 Posted by: Sebike Posted at: 2018-09-20T22:52:06.095Z Reads: 61

```
But you don't have hall sensors right?
```

---
## \#43 Posted by: mynamesmatt Posted at: 2018-09-20T23:00:19.711Z Reads: 59

```
they're sk3's so no. unless he got them specifically made by the manufacturer with hall sensors or added his own
```

---
## \#44 Posted by: TowerCrisis Posted at: 2018-09-21T00:48:52.762Z Reads: 58

```
Make sure you have your belts disconnected while you're running motor detection.
```

---
## \#45 Posted by: briman05 Posted at: 2018-09-21T01:27:36.384Z Reads: 56

```
So since you have no idea how to do the motor detection I’m guess you didn’t do it when you put the board together. You are super lucky you didn’t blow up something. Look up jacobby’s vesc tutorials they are very in-depth
```

---
## \#46 Posted by: torqueboards Posted at: 2018-09-21T03:36:40.551Z Reads: 51

```
@ [KeivanM](https://www.electric-skateboard.builders/u/KeivanM) Your mini remote also doesn't look like it's installed properly. White knob should be at 2 oclock.

https://www.youtube.com/watch?v=ywUfqtKF8Zg
```

---
## \#47 Posted by: Andy87 Posted at: 2018-09-21T04:54:50.623Z Reads: 42

```
You don’t have sensors on the sk3 motors.
Make sure you set the mode to sensorless before you run motor detection and losen the belts.
With this it should run through without issues
```

---
