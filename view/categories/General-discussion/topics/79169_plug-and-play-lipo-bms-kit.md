# Plug and play lipo bms kit?

### Replies: 46 Views: 641

## \#1 Posted by: venom121212 Posted at: 2018-12-28T01:25:20.146Z Reads: 128

```
Not very familiar in the lipo making world but they clearly have a positive/negative cable and a balance cable. Ideally I'm looking for a system where I can buy a 10s configuration of lipo packs from hobbyking and plug into a magical bms black box and only have to make xt90 series/parallel connectors. Does this wizardry exist?
```

---
## \#2 Posted by: Indiangummy Posted at: 2018-12-28T01:27:14.523Z Reads: 126

```
I've only ever seen upto a 6s lipo. You will have to make some series conntections to get to 10s. You could get 2x 5s and connect them In series. It's pretty simple tbh.
```

---
## \#3 Posted by: venom121212 Posted at: 2018-12-28T01:28:08.052Z Reads: 121

```
I'm golden on the series and parallel connections. I need to know the bms wiring.
```

---
## \#4 Posted by: AlanZhou Posted at: 2018-12-28T01:28:39.707Z Reads: 122

```
Nope just use a tutorial on YouTube on how to hook up two 5s lipos to a normal 10 pin bms simple.

https://m.youtube.com/watch?v=_yrYG5skwvs&t=823s
```

---
## \#5 Posted by: AlanZhou Posted at: 2018-12-28T01:30:05.123Z Reads: 118

```
Just look at the vid for balance wire connections lol.
```

---
## \#6 Posted by: Indiangummy Posted at: 2018-12-28T01:31:27.832Z Reads: 111

```
Yeah it depends on the bms but pretty simple overall. Let us know which batteries you are getting and we can give you a diagram of how to wire it.
```

---
## \#7 Posted by: venom121212 Posted at: 2018-12-28T01:33:34.381Z Reads: 105

```
I watched that video already and was just hoping someone was smart enough to make a bms where you just plugged in the balance cables and you're done. Just being hopeful
```

---
## \#8 Posted by: J_Dizzle Posted at: 2018-12-28T01:33:41.669Z Reads: 102

```
That video does some things right, and some things wrong. Please don’t hot glue your balance cables into the connectors
```

---
## \#9 Posted by: mynamesmatt Posted at: 2018-12-28T01:33:43.847Z Reads: 94

```
short answer, nein. very easy to make though. i can give ya a hand with schematics and whatnot
```

---
## \#10 Posted by: ryansinatra Posted at: 2018-12-28T01:33:48.921Z Reads: 98

```
Watching this thread for when I go to set up my 10s lipo and bms set up
```

---
## \#11 Posted by: venom121212 Posted at: 2018-12-28T01:36:04.807Z Reads: 99

```
You guys are far too kind. 
1) What's a good c rating for a 10s hub street board (150 lbs mild to moderate hillage) ? 
2) What's the difference between 5 X 2s batteries and 2 x 5s batteries of equal capacity?
```

---
## \#12 Posted by: Indiangummy Posted at: 2018-12-28T01:37:07.983Z Reads: 94

```
Oh no pretty much all of them require some type of soldering, if that's what you meant.
```

---
## \#13 Posted by: AlanZhou Posted at: 2018-12-28T01:37:16.350Z Reads: 94

```
Well I believe most of us are smart enough to make are on corrections.

Oops replied to the wrong person, was meant for j dizzle
```

---
## \#14 Posted by: Indiangummy Posted at: 2018-12-28T01:38:22.448Z Reads: 92

```
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014

Edit: I used this as a guide for my lipo build. Honselty the best thread for lipo related build/questions
```

---
## \#15 Posted by: AlanZhou Posted at: 2018-12-28T01:39:30.773Z Reads: 84

```
Well having 5x 2s means having 5, 2s cells in series and  2x 5 means having 2, 5s cells in series or some people refer to it as the same

Also 20c means capacity times c rating

So 5s 5000mah 20c means 20x 5 which is 100a

And basically no difference if there the same capacity
```

---
## \#16 Posted by: venom121212 Posted at: 2018-12-28T01:39:32.083Z Reads: 80

```
I'm handy with soldering so it shouldn't be a problem
```

---
## \#17 Posted by: venom121212 Posted at: 2018-12-28T01:40:24.228Z Reads: 83

```
Man get outta here with this please haha. I'm asking on a much more technical level. I know cell configs from lithium ion well.
```

---
## \#18 Posted by: AlanZhou Posted at: 2018-12-28T01:42:24.920Z Reads: 85

```
Haha was woundering why you were asking such easy questons
```

---
## \#19 Posted by: Indiangummy Posted at: 2018-12-28T01:42:40.342Z Reads: 84

```
Yeah I dont k now if you'd see a profomance difference between the two but you can make a slimmer pack if you go with 5x 2s lipos
```

---
## \#20 Posted by: AlanZhou Posted at: 2018-12-28T01:44:02.439Z Reads: 84

```
What kind of hubs are you using
```

---
## \#21 Posted by: AlanZhou Posted at: 2018-12-28T01:44:40.303Z Reads: 76

```
It's way easyier to do 2x 5
```

---
## \#22 Posted by: mynamesmatt Posted at: 2018-12-28T01:45:26.899Z Reads: 75

```
60-80a is always safe. standard vesc 4s are pretty happy at 40a battery amps so if you're running dual an 80a bms is fine. thats if you want to discharge through the bms. the charge only bms can be anything as long as it's rated to charge at your desired current
```

---
## \#23 Posted by: dareno Posted at: 2018-12-28T01:47:29.866Z Reads: 72

```
Read that namasaki thread, its gold but somewhere on here and I can not for the life of me find it is a clever bastard that has built a charger with a built in bms so you don't need one in the enclosure.  Thought I bookmarked it but alas....
```

---
## \#24 Posted by: Indiangummy Posted at: 2018-12-28T01:48:03.849Z Reads: 74

```
Debatable but ok. I've done both and don't find one easer than the other
```

---
## \#25 Posted by: AlanZhou Posted at: 2018-12-28T01:49:05.071Z Reads: 74

```
Well you do more series connections, 5 to be exact and the is more space to mess up, and you don't mess around with lipos. 

Funnly my first build was with lipos.
```

---
## \#26 Posted by: Indiangummy Posted at: 2018-12-28T01:50:52.403Z Reads: 69

```
Wait what?!?!? I've been thinking about doing this myself. Must find.
```

---
## \#27 Posted by: dareno Posted at: 2018-12-28T01:52:40.070Z Reads: 69

```
I think its in a build thread and a recent one.  I will do some research and get back to you
```

---
## \#28 Posted by: deucesdown Posted at: 2018-12-28T01:56:21.401Z Reads: 72

```
[quote="J_Dizzle, post:8, topic:79169"]
Please don’t hot glue your balance cables into the connectors
[/quote]

Explain please!
```

---
## \#29 Posted by: dareno Posted at: 2018-12-28T01:57:38.053Z Reads: 78

```
https://www.electric-skateboard.builders/t/la-croix-long-range-cruiser-carving-machine/76960

Its in here but its aimed at lion cells.  Still a bloody good idea and if you can combine the  namasaki thread info and this then lovely stuff
```

---
## \#30 Posted by: venom121212 Posted at: 2018-12-28T02:10:23.832Z Reads: 72

```
I like that idea a whole lot. Thanks for the search. Any input on what c rating on a lipo pack to use. 20 to 45 is the range I see most. Thinking about getting 2 of [these](https://hobbyking.com/en_us/zippy-compact-4500mah-10s-35c-lipo-pack-xt90.html) and maybe adding a 3rd down the road.
```

---
## \#31 Posted by: Indiangummy Posted at: 2018-12-28T02:11:20.082Z Reads: 69

```
Most c ratings are over exagurated by a long shot. 30c will actually be like 10c. Id say min 60c.
```

---
## \#32 Posted by: AlanZhou Posted at: 2018-12-28T02:12:40.581Z Reads: 68

```
Even 10c is 50a at 5000mah lol
```

---
## \#33 Posted by: dareno Posted at: 2018-12-28T02:13:19.064Z Reads: 66

```
I don't use lipos in esk8 tbh but that namasaki thread has it all.  From what i can gather though 40c minimum.
```

---
## \#34 Posted by: Indiangummy Posted at: 2018-12-28T02:13:34.952Z Reads: 65

```
That's also true. You should be fine with that pack @venom121212
Edit: especially if your putting them in parallel it should be more than enough.
```

---
## \#35 Posted by: venom121212 Posted at: 2018-12-28T02:19:50.104Z Reads: 67

```
Looking at doing a charge only bms if you can recommend one. Do you have any thoughts on the [linked battery](https://hobbyking.com/en_us/zippy-compact-4500mah-10s-35c-lipo-pack-xt90.html) above?
```

---
## \#36 Posted by: J_Dizzle Posted at: 2018-12-28T02:24:08.117Z Reads: 64

```
If you watch the video you will see that he pushes the balance wires into the male ends of the jst connectors from the battery. He then hit glues them to stay in place. Just solder the damn wires!
```

---
## \#37 Posted by: AlanZhou Posted at: 2018-12-28T02:27:23.209Z Reads: 65

```
Mabye it was for demastration purposes lol
```

---
## \#38 Posted by: J_Dizzle Posted at: 2018-12-28T02:30:28.442Z Reads: 64

```
nah, that guy was on the forum last year and had a shitty “company” for a while. The pictures on his site were literally taken from the Just Pictures thread! :joy:

Edit: morale of my story, he is and idiot
```

---
## \#39 Posted by: deucesdown Posted at: 2018-12-28T03:25:21.162Z Reads: 57

```
I just skipped around all over the video looking for hot glue. 20 minutes of bumbling and mumbling, don't have the time and energy to sit though it. Couldn't find any, but he took the bare end of the bms balance wires and stuck them into the jst of the lipo balance connector? Yow.
```

---
## \#40 Posted by: Namasaki Posted at: 2018-12-28T04:25:01.705Z Reads: 62

```
[quote="AlanZhou, post:21, topic:79169, full:true"]
It’s way easyier to do 2x 5
[/quote]


The reason I did five 2s instead of two 5s was to keep the battery as thin as possible for maximum ground clearance under the deck.
I agree with you though, it would be less work to put two 5s together.

As for the C ratings, many of us have come to the realization that the C rating x capacity does not give a accurate max current rating.
For example, my 5ah 60c Lipos are no where near capable of 300a.
They start sagging at less than 50a
They are good Lipos with very low internal resistance. Only about 2 miliohms per cell.
Look at these charts showing voltage drop at only 23a
charts where run on only one vesc in a dual setup so I double the current.

![IMG_8772|230x500](upload://3NnQsdZro5MsjaHkA65c9L7V4xB.jpeg) 

![IMG_8774|230x500](upload://bFPJWfWAzeSQvmpOLXHI09OmSlx.jpeg)
```

---
## \#41 Posted by: mynamesmatt Posted at: 2018-12-28T04:25:21.154Z Reads: 54

```
the d140 bms from bestech is pretty damn good. i just wouldn't use a 10s LiPo battery as they're bloody huge. id be using either 2 5s batteries or 5 2s batteries
```

---
## \#42 Posted by: venom121212 Posted at: 2018-12-28T04:32:25.249Z Reads: 56

```
It's going in a top mount box so if it fits it sits. Thanks for the input. I might pm you about wiring if I need further guidance
```

---
## \#43 Posted by: J_Dizzle Posted at: 2018-12-28T04:32:56.546Z Reads: 58

```
Yeah he didn’t actually hot glue them in the video. He said he was going to. But at the end when he was actually charging, they were just stuck in there :joy:
```

---
## \#44 Posted by: Fre.dw Posted at: 2019-06-03T22:42:11.346Z Reads: 29

```
Just get [this](https://wheelspinmodels.co.uk/i/305401/?gclid=Cj0KCQjwitPnBRCQARIsAA5n84krmPUPfrHtn7EBVrieLVEThJVlepH0YqukXSdlfOlcB7CFFabt1iUaAlbMEALw_wcB) and connect to 2 5s lipos and into a bms with 10s balance conector (most of them).

![image|550x412](upload://uU3wztEwCsWXo3yaHUbBEc0tEpw.jpeg)
```

---
## \#45 Posted by: louwii Posted at: 2019-06-03T23:39:16.860Z Reads: 25

```
Psst, it might be a bit too late since that was in December last year :grin:
```

---
## \#46 Posted by: Fre.dw Posted at: 2019-06-03T23:41:16.409Z Reads: 25

```
Pssst, ok. I do t know how long this person is taking on there build.🙄
```

---
