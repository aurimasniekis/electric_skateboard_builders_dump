# 12s4p 30q batteryquestion

### Replies: 24 Views: 336

## \#1 Posted by: Bobby Posted at: 2019-01-23T02:45:27.404Z Reads: 136

```
So the max that my 12s4p is charing to is 47.9... shouldnt it be closer to 52 volts? It this a bad p group or bad bms? I opened the battery and everything looks connected...i keep making plans to take it to psychotiller but life keeps getting in my way??? Any ideas would be helpful. I bought it used from a member on this site Nd it came not working properly tho i was told it had no issues
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-23T02:48:50.996Z Reads: 136

```
12x4.2=50.4V
Was it charging up to that before?
How is your bms set?
Does your charger went green when reaching the voltage you mentioned?
```

---
## \#3 Posted by: AlexBE Posted at: 2019-01-23T03:00:50.899Z Reads: 123

```
What are all your cell-group voltages? What charger are you using? What BMS are you using?
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-01-23T03:06:23.417Z Reads: 121

```
Check your cells. Check your charger.
```

---
## \#5 Posted by: accrobrandon Posted at: 2019-01-23T03:13:08.689Z Reads: 118

```
[quote="AlexBE, post:3, topic:81782"]
What are all your cell-group voltages?
[/quote]

Yup... Disconnect the bms.pigtail.. And measure each group voltage to see where the variance is... If one group is off then.just charge that group back up to the same level as all the others...
```

---
## \#6 Posted by: Bobby Posted at: 2019-01-23T03:44:39.353Z Reads: 109

```
Didnt set anythinf... its a torque boards battery i got second hand from @Mattmccrary8. It only charges up to 47.9 volts then goes green.... i have no idea how to do anything anyone suggested lol. I dont even own any kind of reader so if anyone has suggestions im game... i figured i could learn a lil something so im gonna try to fuck with it instead of havin it sit around.  Been reading a lot about batteries but its still all greek to me. Only way to learn is to roll up your sleeves and get dirty
```

---
## \#7 Posted by: torqueboards Posted at: 2019-01-23T03:47:21.270Z Reads: 103

```
@bobby - yeah that's most likely a bad p group.
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-01-23T04:04:39.482Z Reads: 101

```
Buy a multimeter. It doesn't have to be a $150 Fluke, I have a little uni-t ac/dc clamp meter and it does everythign I need. You'll find an endless number of uses for it.
```

---
## \#9 Posted by: AlexBE Posted at: 2019-01-23T04:04:51.511Z Reads: 100

```
So in reality we don't even know if 47.9V is true. Get a $5 multimeter and do some checking.
```

---
## \#10 Posted by: Bobby Posted at: 2019-01-23T04:13:36.355Z Reads: 96

```
I know its bad because i only got about two miles before it would die... next step, multimeter
```

---
## \#11 Posted by: pat.speed Posted at: 2019-01-23T04:20:45.256Z Reads: 90

```
Did you buy it in this condition? Did Matt tell you it didn’t work correctly?
```

---
## \#12 Posted by: Bobby Posted at: 2019-01-23T04:30:47.924Z Reads: 86

```
Nope. Had no clue... i was told everything was good and spent about 420 bucks thinking id have a battery i could use. Hasnt worked since i got jt Nd hasnt even been used really for that reason. My first test run, it died in about 20 min of riding and has been sitting in the garage since. I just took it as a loss and not to buy batteries used from here
```

---
## \#13 Posted by: Bobby Posted at: 2019-01-23T04:32:08.195Z Reads: 83

```
I mean i have the whole conversation on this website archived....
```

---
## \#14 Posted by: pat.speed Posted at: 2019-01-23T05:17:57.792Z Reads: 79

```
I’d have a chat with him. See if you can sort something out
```

---
## \#15 Posted by: Bobby Posted at: 2019-01-23T05:25:20.867Z Reads: 79

```
Honestly, i was a rookie back then and didn’t know if i set it up wrong or what the deal was. It was only after some realized it wasnt me.... ill send him a message but im pretty sure nothing will come out of it... just chalk it up to a lesson learned kind of deal. I expect the ol “it worked perfectly fine when i sent it” reply
```

---
## \#16 Posted by: MysticalDork Posted at: 2019-01-23T06:54:53.184Z Reads: 73

```
Even if it's got a bad P group or something, most of the cells are probably still good. You could take out two P sections and have a working 10s. It's just a matter of finding what's borked. Hell, it might just be a problem with the BMS, which is a fairly cheap fix.
```

---
## \#17 Posted by: Marsen Posted at: 2019-01-23T08:23:42.936Z Reads: 66

```
Does sound a lot like a bad cell group. The charger goes green because they are set to indicate full charge when the battery charge current drops below about 300mA not when it reaches max volts.
```

---
## \#18 Posted by: MysticalDork Posted at: 2019-01-23T08:38:57.824Z Reads: 70

```
Yeah. If the BMS detects one of the groups is dead while the others are full, it'll stop the charging and start balancing, to get all the cells to match. But if one group is faulty, it'll never be properly balanced, and the pack will never reach 50.4V. When riding, the cell group that's low will hit LVC very fast, and probably have a high internal resistance, which is what causes the awful range.

Get a multimeter and check each adjacent pair of balance wires (from 1 to 2, then from 2 to 3, 3 to 4,etc). Whichever one reads significantly (more than 0.1V) different than the other is likely bad.
```

---
## \#19 Posted by: pjotr47 Posted at: 2019-01-23T08:46:33.012Z Reads: 68

```
Hmm, I take the guess on two broken cells spread over 2 p groups. The p group with a broken cell will charge faster. When that cell group is 4,2v the bms cut off the power.
```

---
## \#20 Posted by: MysticalDork Posted at: 2019-01-23T09:24:40.075Z Reads: 61

```
If one cell in a P group is screwed, I'd guess all the cells in that group are likely damaged from being driven to either or both voltage limits, or beyond. That, or if on of the cells has developed a soft short, the entire P group will be dead.
```

---
## \#21 Posted by: Friskies Posted at: 2019-01-23T09:45:27.440Z Reads: 59

```
One of your cells in one of the P groups is most likely dead or not connected properly. This is causing that P group to charge faster and hit full capacity earlier than the rest of the pack and causing your BMS to cut off charging. 

All you need to do is find the P group that will be at 4.2 volts and then test the cells in that group to find the battery that is dead/not connected. Once you have found it you will need to charge the cell up to the rest of the P group and then potentially charge up each other group to 4.2v separately.
```

---
## \#22 Posted by: Mattmccrary8 Posted at: 2019-01-23T14:26:51.726Z Reads: 45

```
Youve had this battery for like 6 months if not more and now its bad.
```

---
## \#23 Posted by: Bobby Posted at: 2019-01-23T14:55:46.589Z Reads: 43

```
Before shit goes south, i dont blame @Mattmccrary8 for any scamming or trying to cheat me. I did post questions about it not working when i got it... all on the site. Pmed you about it.
```

---
## \#24 Posted by: Benjamin899 Posted at: 2019-01-23T16:22:55.068Z Reads: 38

```
did you check your charger? Sometimes they don't deliver as advertised.
```

---
