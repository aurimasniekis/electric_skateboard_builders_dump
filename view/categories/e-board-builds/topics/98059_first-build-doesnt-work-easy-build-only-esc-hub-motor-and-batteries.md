# First Build &#124; doesnt work &#124; easy Build only esc ,hub motor and batteries ;*(

### Replies: 44 Views: 564

## \#1 Posted by: Bobo Posted at: 2019-07-08T14:59:08.894Z Reads: 133

```
Hello Guys 
I have a problem . The whole setup doesnz work.
I have  Meepo esc, dual hub motor max. 36v
And 2x 3000mah 5s Zippys

So only the brake does work and i dont know what to do with the wires( hall sensor)

![20190708_165615|375x500](upload://ArxdrMfSCzavag010vbNNuYxvGO.jpeg) ![20190708_165606|374x500](upload://KYRuvsT3qBOS0kFtsKleLRvSNO.jpeg)
```

---
## \#2 Posted by: totalgeek9224 Posted at: 2019-07-08T17:56:24.490Z Reads: 112

```
So you need a JST connector for those sensor wires, and they could be the reason why the ESC isnt working (im not familiar with the Meepo ESC so idk if it runs FOC, BLDC, sensored or unsensored)
```

---
## \#3 Posted by: Bobo Posted at: 2019-07-08T18:29:56.535Z Reads: 105

```
Thx for the answer . Should i solder the wires ?
```

---
## \#4 Posted by: totalgeek9224 Posted at: 2019-07-08T18:32:05.105Z Reads: 106

```
Again, not sure if theyre even necessary. Could you link the ESC? 
Tbh you'd probably get more help on the other forum, since theyre more experienced (link is in my profile)
```

---
## \#5 Posted by: M.Hboards Posted at: 2019-07-08T19:16:21.180Z Reads: 98

```
Try chargeing your remote and your board because the esc your useing has a feature that allows you to break but not accelerate at low remote or board battery.
```

---
## \#6 Posted by: Bobo Posted at: 2019-07-08T20:13:49.702Z Reads: 95

```
I will try it :)
```

---
## \#7 Posted by: Bobo Posted at: 2019-07-09T11:32:31.523Z Reads: 89

```
https://www.meepoboard.com/accessories/esc/
```

---
## \#8 Posted by: totalgeek9224 Posted at: 2019-07-09T11:40:18.973Z Reads: 79

```
[quote="Bobo, post:1, topic:98059"]
So only the brake does work
[/quote]

* As a safety feature, this ESC disables acceleration and only allows braking whenever the battery on your remote or board is critical low.
```

---
## \#9 Posted by: totalgeek9224 Posted at: 2019-07-09T11:41:38.660Z Reads: 76

```
Also, it appears as though this ESC only runs sensorless FOC, in which case, your sensor wires are unneeded and can be tucked aways somewhere
```

---
## \#10 Posted by: Bobo Posted at: 2019-07-09T17:13:21.769Z Reads: 71

```
Hm. I charged my batteries at 4 volt per cell and it shows me that i only have low batterie and the breaks only work
```

---
## \#11 Posted by: totalgeek9224 Posted at: 2019-07-09T17:16:11.085Z Reads: 68

```
How about your remote? Is it charged? And what is the total pack voltage?
```

---
## \#12 Posted by: Bobo Posted at: 2019-07-09T17:30:48.226Z Reads: 67

```
My remote was fully charged and i dont know what my total volatage is. I charged it to 75% . So that shows me the charger
```

---
## \#13 Posted by: totalgeek9224 Posted at: 2019-07-09T17:40:05.336Z Reads: 62

```
Do you have access to a voltmeter? and is the charger (or rather meter) set to the right voltage?
```

---
## \#14 Posted by: Bobo Posted at: 2019-07-09T17:53:43.877Z Reads: 58

```
So when in charging i can see how much volts it has. And when im charging i select balance charger and 5s 3000mah. I dont think that i did an mistake
```

---
## \#15 Posted by: totalgeek9224 Posted at: 2019-07-09T18:07:46.595Z Reads: 53

```
Waity, youre running a 5s battery?
```

---
## \#16 Posted by: Bobo Posted at: 2019-07-09T18:09:26.981Z Reads: 53

```
Yes but im connected it parralel with an xt80 atapter
```

---
## \#17 Posted by: totalgeek9224 Posted at: 2019-07-09T18:11:27.271Z Reads: 56

```
So do you have 2 5s batteries connected in parrallel? Im not sure if 5s is in the operational voltage of the ESC
```

---
## \#18 Posted by: Bobo Posted at: 2019-07-09T18:14:01.317Z Reads: 55

```
10s is the best voltage for a esc. But i heard that when im running 2x 5s in parrallel it goes to 10s. And should i buy an voltage meeter ?
```

---
## \#19 Posted by: esk8_hui Posted at: 2019-07-09T18:19:37.306Z Reads: 55

```
2 x 5s in serial gives you 10s not parallel.
```

---
## \#20 Posted by: Bobo Posted at: 2019-07-09T18:20:57.626Z Reads: 57

```
I mean that. I need 10s for my esc and the motors
```

---
## \#21 Posted by: esk8_hui Posted at: 2019-07-09T18:23:45.922Z Reads: 54

```
If you don't have a multimeter you should get one and if you want to see battery voltage and percentage built in board you need to get a voltage meter.
```

---
## \#22 Posted by: Bobo Posted at: 2019-07-09T19:34:02.422Z Reads: 51

```
Ok i will buy it
```

---
## \#23 Posted by: totalgeek9224 Posted at: 2019-07-09T19:38:16.804Z Reads: 51

```
Could you take a couple of photos so that we can see the setup?
```

---
## \#24 Posted by: leroy Posted at: 2019-07-09T23:12:40.352Z Reads: 49

```

the max current is 24 Amps FOC. It's max output is 12amps per motor, 
The speed controller is the most important component,
you bought the cheapest one available, and seem genuinely surprised you are having issues.
Throw that piece of shit in the trash and spend at least $100 on a decent ESC.
This is how people get hurt, seriously.
```

---
## \#25 Posted by: Bobo Posted at: 2019-07-10T15:12:07.984Z Reads: 42

```
I saw other people with the same setup and it worked
```

---
## \#26 Posted by: Bobo Posted at: 2019-07-10T15:49:38.415Z Reads: 43

```
Do you mean fron the esc ? Or what
```

---
## \#27 Posted by: totalgeek9224 Posted at: 2019-07-10T16:02:41.743Z Reads: 41

```
Yes, primarily the connections between your ESC and motors (I saw the ones already attached), but also how you've connected your batteries and ESC
```

---
## \#28 Posted by: Bobo Posted at: 2019-07-11T13:39:06.316Z Reads: 41

```
![15628522269877987385411414003147|375x500](upload://cDO6WXuVuoXef6Fc8PAMcXSXQU1.jpeg) ![15628522716376147507469754842020|666x500](upload://bYVsnuH1cfuselmHniWhl985dYK.jpeg)
```

---
## \#29 Posted by: totalgeek9224 Posted at: 2019-07-11T14:00:35.483Z Reads: 39

```
Hm. So as it is youre running 5s with those two batteries in parrallel giving you 6000mAh of capacity. Theres nothin that i can see that blatantly suggests why the ESC isnt working. I would check the cell voltages because what can happened (and has happened before) is that 
1) Someone gets a cheap battery meter from ebay 
2) Plugs it to 10s battery 
3) see's 100%
4) Board has low power/ wont work
5) checks cell voltages
6) finds them low
7) turns out battery meter was configured for 8s or something lower
```

---
## \#30 Posted by: Bobo Posted at: 2019-07-11T14:56:12.794Z Reads: 37

```
Ye i bought an lipo checker and i must wait 7 days.
```

---
## \#31 Posted by: Super Posted at: 2019-07-11T16:21:19.775Z Reads: 37

```
Buy a 10s battery and try it with that.
```

---
## \#32 Posted by: totalgeek9224 Posted at: 2019-07-11T16:28:52.541Z Reads: 34

```
He simply needs to connect the batteries he has in series and make sure theyre charged
```

---
## \#33 Posted by: L3chef Posted at: 2019-07-11T17:29:32.701Z Reads: 33

```
So you are running 5s 6Ah right? Probably tl low voltage flr the esc. Rewire it as 10s and try again
```

---
## \#34 Posted by: Bobo Posted at: 2019-07-11T17:36:12.815Z Reads: 34

```
I thought when im doing 2x 5s 3000mah it goes to 10s 3000mah. I saw somebody and he used the same setup
```

---
## \#35 Posted by: L3chef Posted at: 2019-07-11T17:49:22.726Z Reads: 34

```
Well it depends on how you connect your batteries.. This will help you understand
![batteryWireDiagram|400x200](upload://wXgLOzrdhzWS84FnmCGVt9Gowzt.jpeg)
```

---
## \#36 Posted by: Bobo Posted at: 2019-07-12T16:55:55.146Z Reads: 27

```
Oh lol.
I think my connector is an parrallel one.
```

---
## \#37 Posted by: Bobo Posted at: 2019-07-12T17:03:29.869Z Reads: 27

```
Fucckkk i saw my order on hobby kind and this an parallel one . Fuck my life.
```

---
## \#38 Posted by: L3chef Posted at: 2019-07-12T17:23:59.057Z Reads: 27

```
I think you should reconsider your battery option.. Even tho you connect them in series you only have 3000mah.. That's almost no range at all..
```

---
## \#39 Posted by: Bobo Posted at: 2019-07-13T06:42:48.311Z Reads: 26

```
How much range is that ?
```

---
## \#40 Posted by: L3chef Posted at: 2019-07-13T08:43:02.846Z Reads: 23

```
not close to satisfy
```

---
## \#41 Posted by: Bobo Posted at: 2019-07-13T10:13:12.126Z Reads: 23

```
Do you know which batteries should i use ?
```

---
## \#42 Posted by: L3chef Posted at: 2019-07-13T10:56:25.782Z Reads: 21

```
There's many options out there. Many of them have missleading or incorrect stats like capacity and discharge value..
You should start by meassuring how much room you have for batteries. Check the stats of the esc what it can handle. And go from there
```

---
## \#43 Posted by: Bobo Posted at: 2019-07-15T13:30:13.614Z Reads: 20

```
Hey guys !
Thank u soo much for helping. U guys made my day.
I will change maybe my batteries and develope my board. THANK YOU FOR TAKING THE TIME !!![15631973941504847749520045836861|374x500](upload://bD6YePeIJ9QzczJCfKGNhBcdLEY.jpeg)
```

---
## \#44 Posted by: Bobo Posted at: 2019-07-15T14:22:47.868Z Reads: 17

```
Is it normal when i switch to fast mode that my batteries and the motor gets really hot. Im scared that they can explode or smt. And should i always connect the electricity cable ( xt60
```

---
