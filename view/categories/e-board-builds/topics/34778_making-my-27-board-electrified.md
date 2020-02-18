# Making my 27&rdquo; board ELECTRIFIED

### Replies: 76 Views: 1768

## \#1 Posted by: Orin635 Posted at: 2017-10-04T19:33:00.002Z Reads: 175

```
I have a 27" (Amazon nickle board)and will be making it into an electric skateboard I won't be going at high speeds max 20 km/h (12.5 mp/h) my main goal is to go up steep hills so I will be using 59mm wheels and a 3:1 pulley ratio (280kb motor) just want your guys thoughts any tips or comments in general#

Brief components list:
Motor: Turnigy 5055-280KV Brushless motor
ESC: X-car Beast series ESC 120A
Batteries: 2x Turnigy 5000mah 3S 20C lipo pack

I will be posting the results probably on a new topic since It probably won't be done for another couple of months
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-04T19:35:47.361Z Reads: 162

```
59mm wheels will be too small for a 3:1 ratio. Think about moving up to 80mm+. If you want torque and not speed, lower your kv, 170~ should be good.
```

---
## \#3 Posted by: Orin635 Posted at: 2017-10-04T19:36:28.773Z Reads: 154

```
what do you mean they are to small?
```

---
## \#4 Posted by: Jinra Posted at: 2017-10-04T19:37:11.066Z Reads: 149

```
Think about how you fit a pulley on there. Most pulleys would already be as big as the wheel. You might be able to get it to work with a chain drive though. I don't have much experience with chain drives, however.
```

---
## \#5 Posted by: cwazy1 Posted at: 2017-10-04T19:38:27.446Z Reads: 142

```
If you run 59mm wheels, you're not going to be able to run a large wheel pulley. If you don't run a large wheel pulley you can't get a good reduction ratio down to motor pulley for the required torque you want for steep hills. The smallest pulley I'd ever consider running on a motor would be 13 for a 5M pitch. Any less than that and you'll have issues with slipping. If you're hard set on tiny ass wheels, then move to a 3M pitch.
```

---
## \#6 Posted by: Orin635 Posted at: 2017-10-04T19:39:43.467Z Reads: 126

```
Oh don't worry the pulley diamter is smaller than the wheel
```

---
## \#7 Posted by: Orin635 Posted at: 2017-10-04T19:40:19.531Z Reads: 124

```
it is 36:12T (5mm pitch)
```

---
## \#8 Posted by: Jinra Posted at: 2017-10-04T19:41:45.026Z Reads: 122

```
a 36T 5M pulley barely has any clearance for an 80mm wheel, it'll be wayyy too low on a 56mm wheel.
```

---
## \#9 Posted by: cwazy1 Posted at: 2017-10-04T19:42:55.953Z Reads: 117

```
agree, you might have like 2-3mm of clearance between your belt and the ground. Not a good idea.

just go with abec11's in the 83mm.
```

---
## \#10 Posted by: akhlut Posted at: 2017-10-04T19:43:41.967Z Reads: 115

```
Paging @Sapphirinia.  She just finished her nickel board.
```

---
## \#11 Posted by: jmasta Posted at: 2017-10-04T19:45:46.786Z Reads: 113

```
36T HTD 5mm pulley has an outside diameter of 56mm.  That's not including the belt.  With a 59mm wheel, the belt would basically be scraping the ground at all times

_56.16mm + (3.81-2.08)mm = 57.89mm_

_(59-57.89)/2 = 0.55mm_

You would literally have 0.5mm clearance
```

---
## \#12 Posted by: cwazy1 Posted at: 2017-10-04T19:47:18.056Z Reads: 108

```
sidenote, you may as well spend the extra 40$ and go with a VESC rather than a car ESC. it'll be infinitely more customizable.
```

---
## \#13 Posted by: Vieo Posted at: 2017-10-04T20:07:55.468Z Reads: 109

```
Penny do some really nice 70mm wheels and 4" trucks. Which makes quite a difference in ride-quality :)

I also made 22" Penny run at 59mm wheels 32T 300KV 6S and at my weight 60KG worked surprisingly well but not amazing at hills.
```

---
## \#14 Posted by: Orin635 Posted at: 2017-10-05T16:56:00.940Z Reads: 81

```
In what ways?
```

---
## \#15 Posted by: Orin635 Posted at: 2017-10-05T17:05:04.170Z Reads: 79

```
would stepping down to a 2:1 make alot of diference for hill climb capability?
```

---
## \#16 Posted by: thisguyhere Posted at: 2017-10-05T17:05:23.378Z Reads: 80

```
you're asking questions that have been answered over and over again, how much research have u done?
```

---
## \#17 Posted by: Orin635 Posted at: 2017-10-05T17:06:37.564Z Reads: 84

```
alot lol :P the question are very specific to my board and i like other peoples updated opions
```

---
## \#18 Posted by: Orin635 Posted at: 2017-10-05T17:08:00.581Z Reads: 80

```
Should I use a 30T:10T?
```

---
## \#19 Posted by: cwazy1 Posted at: 2017-10-05T17:08:21.867Z Reads: 83

```
Yeah I'm not going to answer that question because clearly you have not done much research on VESC and BLDC tool or VESC tool. There is a whole category dedicated to VESC and also BLDC.
```

---
## \#20 Posted by: thisguyhere Posted at: 2017-10-05T17:10:59.931Z Reads: 80

```
you asked in what ways the vesc is better, so you know then?
```

---
## \#21 Posted by: Orin635 Posted at: 2017-10-05T18:42:48.760Z Reads: 66

```
im not intrested in a vesc since i am on a very tight budget
```

---
## \#22 Posted by: jmasta Posted at: 2017-10-05T18:48:03.396Z Reads: 64

```
[quote="Orin635, post:18, topic:34778, full:true"]
Should I use a 30T:10T?
[/quote]

No. You would only have 4 teeth in mesh on the 10T gear, which is terrible for torque transfer
```

---
## \#23 Posted by: Orin635 Posted at: 2017-10-05T18:49:48.462Z Reads: 68

```
Ok thats unfortunate better go for 30T:15T :/
```

---
## \#24 Posted by: Orin635 Posted at: 2017-10-05T19:02:32.422Z Reads: 69

```
I've found a 48:16T  pulley kit and the 48T pulley is only 51mm diameter so I will be going with that
```

---
## \#25 Posted by: Jinra Posted at: 2017-10-05T19:03:24.231Z Reads: 68

```
wont fit with a 56mm wheel
```

---
## \#26 Posted by: Orin635 Posted at: 2017-10-05T19:09:37.518Z Reads: 69

```
theyre 59mm so i should have 5mm between the ground and the belt?
```

---
## \#27 Posted by: Jinra Posted at: 2017-10-05T19:10:35.000Z Reads: 70

```
The belt alone adds another 6mm. Trust what everyone is saying, you're wheel is too small.
```

---
## \#28 Posted by: Orin635 Posted at: 2017-10-05T19:12:18.697Z Reads: 67

```
the belt is not 6mm thick. the pulley has a 3mm pitch
```

---
## \#29 Posted by: GrecoMan Posted at: 2017-10-05T19:13:48.139Z Reads: 73

```
I don’t think you realize how small 5mm is...

<img src="/uploads/db1493/original/3X/b/c/bc12347b25f5897199c9928f0603e7413db0a475.jpg" width="375" height="500"> 

That caliper is set to 5mm, my finger for comparison

YOU NEED BIGGER WHEELS
```

---
## \#30 Posted by: Jinra Posted at: 2017-10-05T19:13:54.562Z Reads: 68

```
I mean 3mm each side, but I guess the top clearance doesn't matter. It's your money, but you'll be burning through belts, and probably pulleys.
```

---
## \#31 Posted by: L3chef Posted at: 2017-10-05T19:14:34.512Z Reads: 66

```
51 vs 59 = 8mm . You will only have 4mm groundclerance. And that's without a belt
```

---
## \#32 Posted by: Orin635 Posted at: 2017-10-05T19:15:03.423Z Reads: 61

```
I have a measuring tape in front of me ik what 5mm looks like
```

---
## \#33 Posted by: Orin635 Posted at: 2017-10-05T19:15:25.658Z Reads: 63

```
How? please explain
```

---
## \#34 Posted by: Jinra Posted at: 2017-10-05T19:15:48.007Z Reads: 64

```
Because your clearance is nearly non existent.. we've been over this.
```

---
## \#35 Posted by: Orin635 Posted at: 2017-10-05T19:16:10.604Z Reads: 61

```
how much clearance is good?
```

---
## \#36 Posted by: GrecoMan Posted at: 2017-10-05T19:16:14.690Z Reads: 60

```
[quote="Orin635, post:33, topic:34778, full:true"]
How? please explain
[/quote]

Your belt will be dragging on the ground half the time.  You will go through a belt about every 5 minutes of riding
```

---
## \#37 Posted by: L3chef Posted at: 2017-10-05T19:17:00.266Z Reads: 63

```
~20mm or more
```

---
## \#38 Posted by: Orin635 Posted at: 2017-10-05T19:18:12.373Z Reads: 71

```
Ok so will a 42mm diameter pulley be ok??? :joy:
```

---
## \#39 Posted by: GrecoMan Posted at: 2017-10-05T19:18:48.002Z Reads: 71

```
I run with about 12mm of clearance with belt on.  Probably about 20-21mm with no belt

<img src="/uploads/db1493/original/3X/5/1/51a0508caa5179694eb031192938c31ee6177f88.jpeg" width="375" height="500">
```

---
## \#40 Posted by: Orin635 Posted at: 2017-10-05T19:19:51.203Z Reads: 69

```
Ok, i see. why do you need so much ground clearance?
```

---
## \#41 Posted by: L3chef Posted at: 2017-10-05T19:20:33.269Z Reads: 65

```
Then you have 8.5 mm from ground to pulley. Add the belt and you are about 7mm from ground. Not good egnouff yet
```

---
## \#42 Posted by: GrecoMan Posted at: 2017-10-05T19:21:12.815Z Reads: 60

```
It sounds like a super unlikely situation but...

If you get a rock that hits that perfect spot and snaps/ weakens your belt, you are left with no brakes.  Also, you don’t want rocks or sticks getting caught in your drivetrain
```

---
## \#43 Posted by: Orin635 Posted at: 2017-10-05T19:22:54.456Z Reads: 63

```
Well if I 3D print a pulley cover I will only need like 2mm of clearance :P?
```

---
## \#44 Posted by: GrecoMan Posted at: 2017-10-05T19:23:19.219Z Reads: 62

```
That cover would take the hits and break.  Then you would have the same problem
```

---
## \#45 Posted by: L3chef Posted at: 2017-10-05T19:27:00.656Z Reads: 60

```
Dude get bigger wheels :smile:
```

---
## \#46 Posted by: Orin635 Posted at: 2017-10-05T19:27:21.429Z Reads: 60

```
I really ready dont want bigger wheels lol
```

---
## \#47 Posted by: Orin635 Posted at: 2017-10-05T19:27:44.835Z Reads: 61

```
I can easily replace it for a lot cheaper
```

---
## \#48 Posted by: MrHappy Posted at: 2017-10-05T19:27:52.692Z Reads: 63

```
then you must not want a decent electric board.
```

---
## \#49 Posted by: L3chef Posted at: 2017-10-05T19:28:17.363Z Reads: 59

```
Allright. Well good luck with your build mate! Post pics when it's done :)
```

---
## \#50 Posted by: GrecoMan Posted at: 2017-10-05T19:28:26.292Z Reads: 59

```
Dude.  BUY BIGGER WHEELS.  They are like $30 on eBay
```

---
## \#51 Posted by: MrHappy Posted at: 2017-10-05T19:29:02.690Z Reads: 61

```
Please wear a helmet when you go to ride it. I don't want someone to get hurt over ignorance.
```

---
## \#52 Posted by: Orin635 Posted at: 2017-10-05T19:29:11.452Z Reads: 62

```
30 is alot when your budget is 220 :P
```

---
## \#53 Posted by: GrecoMan Posted at: 2017-10-05T19:30:04.644Z Reads: 64

```
random question: how old are you?
```

---
## \#54 Posted by: MrHappy Posted at: 2017-10-05T19:30:08.593Z Reads: 62

```
Save your money and wait until you can afford building a decent board. Your not going to be happy with anything you make for $220
```

---
## \#55 Posted by: cwazy1 Posted at: 2017-10-05T19:30:19.197Z Reads: 61

```
go buy a meepo. jesus.
```

---
## \#56 Posted by: Orin635 Posted at: 2017-10-05T19:30:20.774Z Reads: 60

```
also, im planning on adding physical breaks like the one on a scooter
```

---
## \#57 Posted by: MrHappy Posted at: 2017-10-05T19:31:01.743Z Reads: 64

```
there goes your budget right there.
Shits expensive.
You either need to make a custom solution, which isnt going to work first take first try, or your going to spend alot of money.
```

---
## \#58 Posted by: Orin635 Posted at: 2017-10-05T19:31:44.080Z Reads: 65

```
I might see if I can 3D print custom pulleys for my scenario.
```

---
## \#59 Posted by: GrecoMan Posted at: 2017-10-05T19:34:43.594Z Reads: 62

```
alright I'm done trying to convince you.  bye
```

---
## \#60 Posted by: Orin635 Posted at: 2017-10-05T19:35:29.093Z Reads: 61

```
hahha sorry bud
```

---
## \#61 Posted by: Sapphirinia Posted at: 2017-10-07T18:57:49.754Z Reads: 46

```
The zombie hawgs wheel are really nice on my penny nickel. I got the 76mm ones. They're on my build log.
```

---
## \#62 Posted by: b264 Posted at: 2017-10-07T19:42:41.162Z Reads: 43

```
[quote="GrecoMan, post:42, topic:34778"]
It sounds like a super unlikely situation but...

If you get a rock that hits that perfect spot and snaps/ weakens your belt
[/quote]

Doesn't sound unlikely at all... that sounds like "Tuesday morning" to me
```

---
## \#63 Posted by: GrecoMan Posted at: 2017-10-07T19:44:51.579Z Reads: 42

```
Lol I actually just had something like that happen while I was out riding a couple minutes ago...

I was going uphill and a stick managed to hop up in the perfect spot and hit the power button for my board, turning it off :joy:
```

---
## \#64 Posted by: b264 Posted at: 2017-10-07T19:45:07.723Z Reads: 40

```
Dude, you should buy a meepo.  But if it's going to keep you from killing yourself in an accident, I bet someone in here can donate some pretty worn-out wheels that are bigger
```

---
## \#65 Posted by: b264 Posted at: 2017-10-07T19:47:49.649Z Reads: 41

```
[quote="GrecoMan, post:63, topic:34778"]
I was going uphill and a stick managed to hop up in the perfect spot and hit the power button for my board, turning it off
[/quote]

Funny as it sounds, if you ride a board for hundreds of miles, shit like this WILL happen to you at least once
```

---
## \#66 Posted by: GrecoMan Posted at: 2017-10-07T19:48:54.099Z Reads: 41

```
I'm moving to an integrated enclousure with power button on top of the deck so this risk will hopefully be eliminated...
```

---
## \#67 Posted by: mmaner Posted at: 2017-10-07T19:49:28.701Z Reads: 44

```
If you need Wheels I've got five or six sets of flywheel clones in different colors and sizes that I've tried over the last couple of years that I don't ride anymore. Just tell me what size you want and I'll let you know what colors I've got in those sizes and you can have them.
```

---
## \#68 Posted by: b264 Posted at: 2017-10-07T19:53:27.615Z Reads: 44

```
I have a set of evolve 83mm that I will never ever use, they are actually brand new.  But I won't ever put them on anything
```

---
## \#69 Posted by: GrecoMan Posted at: 2017-10-07T19:56:25.142Z Reads: 45

```
Does that offer apply to everyone :joy:
```

---
## \#70 Posted by: Orin635 Posted at: 2017-10-07T20:15:54.283Z Reads: 46

```
How much would you charge for those :P?
```

---
## \#71 Posted by: Orin635 Posted at: 2017-10-07T20:16:42.903Z Reads: 42

```
Also, where would you get trucks for those? I have done no research into wheels and trucks
```

---
## \#72 Posted by: b264 Posted at: 2017-10-07T20:23:40.508Z Reads: 41

```
You could use a riser pad to get clearance so there is no wheel bite.  They're a few dollars
```

---
## \#73 Posted by: Orin635 Posted at: 2017-10-07T20:26:39.759Z Reads: 41

```
Yes I could even make the risers but the trucks I have now are extremely short
```

---
## \#74 Posted by: mmaner Posted at: 2017-10-07T21:40:13.030Z Reads: 40

```
Yeah, I don't care.  They are just in the way right know. My abec 97 Flywheels are gonna ride till they die 😀.
```

---
## \#75 Posted by: GrecoMan Posted at: 2017-10-07T22:13:01.989Z Reads: 45

```
what sizes do you have in black?
```

---
## \#76 Posted by: mmaner Posted at: 2017-10-07T22:52:15.526Z Reads: 42

```
I've got some.83mm, maybe 90mm but I'll have to check.
```

---
