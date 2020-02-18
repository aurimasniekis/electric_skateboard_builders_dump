# Optimal motor KV for offroad and top speed?

### Replies: 77 Views: 788

## \#1 Posted by: JensSjogren Posted at: 2018-11-04T14:47:40.238Z Reads: 203

```
I use 2x 6374 turningy 149kv motors on my trampa build. I'm in love with the torque it provides and the hill climbing abillity. However my top speed is at 38 kph with a gear ratio of 6:1. 

I want to be able to reach around 60 kph just for the heck of it (i need to lower gear ratio and get other motors). How much offroad capabillity would i have to sacrifice if i switch to 190kv motors instead? I see alot of people running 190kv motors on their trampa boards. I'm not sure if they use their board primarily in urban areas. 

Basicly, i want higher top speed but i still want to be able to shred mountainbike tracks in the forest, would 6374 4400w 190kv motors and a gear ratio of 4:1 work fine in heavy offroad conditions and for hill climbing? 

Thanks in advance!
```

---
## \#2 Posted by: Eboosted Posted at: 2018-11-04T15:08:37.829Z Reads: 194

```
Do not change the motors yet, change the gear ratio, easiest way is to change the motor pulley first.

How many teeth you have on motor and wheel?

190kv + 4:1 is too much, I tested it and it has no torque and brakes are too weak, final speed is way too much a Trampa
```

---
## \#3 Posted by: JensSjogren Posted at: 2018-11-04T15:16:58.788Z Reads: 186

```
Ohh really? Is it too weak for offroad or does the urban driving also become limited? I feel that a trampa board should be able to handle higher speeds than a normal longboard setup? It feels more stable. 

I have the torqueboards motor mount and pulley kit, it is 72t 12t. It was the only option that TB offered. Ive already ordered 66t and 15t sets from trampa, this will get me to 47 kph. I also ordered 18t motor pulleys but im not sure if that one will work since the diameter might be to large. 

I've already ordered 2x pulley kits from trampa
```

---
## \#4 Posted by: rojitor Posted at: 2018-11-04T15:17:00.841Z Reads: 172

```
60 kh  on a flexible deck is not a good idea imho. I'd upgrade motors size, not kv.
```

---
## \#5 Posted by: JensSjogren Posted at: 2018-11-04T15:19:33.896Z Reads: 169

```
Oh okay, speed concerns are because of the flex. Didnt think of that tbh. Its not like i will be going at 60 kph frequently, more like i want to be able to do it 😅
```

---
## \#6 Posted by: rojitor Posted at: 2018-11-04T15:23:01.539Z Reads: 167

```
I think @Kug3lis uses big motors. I don't know how fast they are nor the ratio he is using
```

---
## \#7 Posted by: JensSjogren Posted at: 2018-11-04T16:12:30.338Z Reads: 155

```
6374 motors seems to be more than enough though. I know my gear ratio is high and i use 150 kv motors but from a standstill on steep hills i easily reach top speed in like 5 seconds. That's why im curious if a 190kv setup would work almost as good on hills and off-road. Right now i feel like the board could climb a wall, it has way more torque than necessary 😅
```

---
## \#8 Posted by: Trdolan03 Posted at: 2018-11-04T16:17:07.503Z Reads: 151

```
I use 190 on my off-road trampa build and have plenty of power and can hit 32mph.
```

---
## \#9 Posted by: JensSjogren Posted at: 2018-11-04T16:30:03.812Z Reads: 146

```
[quote="Trdolan03, post:8, topic:73379, full:true"]
I use 190 on my off-road trampa build and have plenty of power and can hit 32mph
[/quote]

What gear ratio do you use? 5:1? Have you tried hitting heavy off-road tracks like mountainbike tracks?
```

---
## \#10 Posted by: professor_shartsis Posted at: 2018-11-04T16:34:16.740Z Reads: 136

```
you can go 38kmh & want to go 60kmh...

60kmh/38kmh=1.5789

6 gear ratio / 1.5789 = 3.8:1 gear ratio

1 / 1.5789 = 0.633

^you need a 3.8:1 gear ratio for ~60kmh and you’ll have about 63.33% as much acceleration as you have now after changing the gearing (~36.7% loss of thrust/acceleration)

you can recover the loss of acceleration from the gearing change by increasing your present motor current limit x 1.57

since heating increases at the square of current your motors and controllers will heat 1.57^2=2.46x faster as they did before for the same acceleration.
```

---
## \#11 Posted by: Trdolan03 Posted at: 2018-11-04T16:38:22.330Z Reads: 132

```
5:1 I ride on dirt hiking trails and at times I will do a burn-out on 80 motor amps. Yet to find a hill I can't do
```

---
## \#12 Posted by: JensSjogren Posted at: 2018-11-04T16:46:15.394Z Reads: 130

```
[quote="Trdolan03, post:11, topic:73379, full:true"]
5:1 I ride on dirt hiking trails and at times I will do a burn-out on 80 motor amps. Yet to find a hill I can’t do
[/quote]

Cool man, thanks for the info! :) as you have experience of a trampa going at 32 mph (roughly 52 kph) would you say that the board handles the speed well? Do you consider higher top speed to be dangerous?
```

---
## \#13 Posted by: JensSjogren Posted at: 2018-11-04T16:49:04.942Z Reads: 128

```
[quote="professor_shartsis, post:10, topic:73379"]
you can go 38kmh &amp; want to go 60kmh…

60kmh/38kmh=1.5789

6 gear ratio / 1.5789 = 3.8:1 gear ratio

1 / 1.5789 = 0.633

^you need a 3.8:1 gear ratio for ~60kmh and you’ll have about 63.33% as much acceleration as you have now after changing the gearing (~36.7% loss of thrust/acceleration)
[/quote]

Nice to see some math! Hmm well that much loss in torque is not worth it i guess. How about using 190kv motors? My current motors are 149 kv 3500 watts (80a max). Would motors rated with 192 kv 4400 watts (100a) max automaticly mean less torque? Since they are rated for more watts that should eliminate some differences?
```

---
## \#14 Posted by: professor_shartsis Posted at: 2018-11-04T16:49:54.140Z Reads: 124

```
You’ll experience the same loss of acceleration if you change the KV as if you change the gearing…
```

---
## \#15 Posted by: JensSjogren Posted at: 2018-11-04T16:51:54.659Z Reads: 124

```
[quote="professor_shartsis, post:14, topic:73379, full:true"]
You’ll experience the same loss of acceleration if you change the KV as if you change the gearing…
[/quote]

Okay, i see. But shouldnt 4400 watts provide more torque than 3500 watts? If the motots was the same kv that is
```

---
## \#16 Posted by: Andy87 Posted at: 2018-11-04T16:52:23.070Z Reads: 121

```
50km/h is the mark for me when it gets more hard to don’t fall into speed wobbles.
If you have a confident stand and the right dampas 55-60 shouldn’t be an issue on good roads.
Which ply deck you have and how heavy you are?
```

---
## \#17 Posted by: professor_shartsis Posted at: 2018-11-04T16:53:38.335Z Reads: 121

```
[quote="JensSjogren, post:15, topic:73379"]
Okay, i see. But shouldnt 4400 watts provide more torque than 3500 watts? If the motots was the same kv that is
[/quote]


@JensSjogren see what i added to my original post:

[quote="professor_shartsis, post:10, topic:73379"]
you can recover the loss of acceleration from the gearing change by increasing your present motor current limit x 1.57

since heating increases at the square of current your motors and controllers will heat 1.57^2=2.46x faster as they did before for the same acceleration.
[/quote]
```

---
## \#18 Posted by: JensSjogren Posted at: 2018-11-04T16:53:44.055Z Reads: 117

```
[quote="Andy87, post:16, topic:73379, full:true"]
50km/h is the mark for me when it gets more hard to don’t fall into speed wobbles.
If you have a confident stand and the right dampas 55-60 shouldn’t be an issue on good roads.
Which ply deck you have and how heavy you are?
[/quote]

I got 16 ply and red (stiff dampas). I weigh 88 kg.
```

---
## \#19 Posted by: Andy87 Posted at: 2018-11-04T16:55:39.394Z Reads: 114

```
You speak about the sk8 motors?
Can you explain me why the 150kV is rated only to 80a and the 190kv to 100a with the same size, same weight?
190kV is rated 4400w 
150kV only 3500w
```

---
## \#20 Posted by: JensSjogren Posted at: 2018-11-04T16:56:45.395Z Reads: 112

```
Oh shiiet, that would require some serious heatshrinks on the focboxes i guess! Maybe better off to try 4:1 ratio on the 150kv motors. That should give a top speed of 51 kph. Lets just start there 😅
```

---
## \#21 Posted by: JensSjogren Posted at: 2018-11-04T16:57:31.145Z Reads: 104

```
Sorry i cannot, that is wierd to me to!
```

---
## \#22 Posted by: Andy87 Posted at: 2018-11-04T16:58:12.246Z Reads: 104

```
Should be good. 
With my urban carve i had 15ply front yellow, back red dampas and 85kg.
As i said for me it was like exactly at 50km/h it start to wobble but if you train your stand and confident you can add some speed on.
```

---
## \#23 Posted by: Andy87 Posted at: 2018-11-04T17:00:00.371Z Reads: 103

```
Me too, that’s why I don’t trust this hobbyking specs. 
Not the first time that they mixed something up in there description.
Don’t want to say it’s not like they write, but who knows 😅
```

---
## \#24 Posted by: JensSjogren Posted at: 2018-11-04T17:02:01.254Z Reads: 102

```
Yeah its better to start increasing to 50 kph anyways. Not to make any crazy changes. I really want to find a sweet spot where i can do heavy offroading with high torque to tackle every hill and still be able to reach good top speeds. 38kph is definitly to slow of a top speed on asphalt streets 

Sure it is possible to bring different pulleys for different tasks but in the best of worlds you wanna avoid to change the pulleys all the time
```

---
## \#25 Posted by: Andy87 Posted at: 2018-11-04T17:02:52.935Z Reads: 97

```
I see there is a need for a second board 😅😅😅
```

---
## \#26 Posted by: JensSjogren Posted at: 2018-11-04T17:03:12.376Z Reads: 98

```
3500 watts is already overkill for a eboard if i understand correctly, the motors never really uses 80a right?
```

---
## \#27 Posted by: professor_shartsis Posted at: 2018-11-04T17:03:15.050Z Reads: 95

```
@JensSjogren or switch to 3.8:1, keep the present motor current limit, but go 4 wheel drive, and you'll get less heating per motor than you have now to obtain the same acceleration as you have now...

1.57 / 2 = 0.785

0.785^2= 0.616

^you'd get about 0.616x the heat per motor/controller for the same acceleration you have now, but with the 60kmh top speed you want...
```

---
## \#28 Posted by: JensSjogren Posted at: 2018-11-04T17:13:01.425Z Reads: 91

```
That would be cool, however i dont really like the idea of having motors in the front, if i hit into something when i drive in the forest the motors would take the hit right in the face, which could be problematic 🤔

Also thats another 700€ or so on the build 😅
```

---
## \#29 Posted by: notepad Posted at: 2018-11-04T17:16:16.236Z Reads: 90

```
[quote="Eboosted, post:2, topic:73379"]
190kv + 4:1 is too much,
[/quote]

Just piggybacking on this thread.  what do you think to 2x 168Kv 3.5:1 ratio for a ATB, but only for road use? Do you think there would be enough torque?
```

---
## \#30 Posted by: Trdolan03 Posted at: 2018-11-04T17:18:03.612Z Reads: 91

```
[quote="JensSjogren, post:12, topic:73379"]
Cool man, thanks for the info! :slight_smile: as you have experience of a trampa going at 32 mph (roughly 52 kph) would you say that the board handles the speed well? Do you consider higher top speed to be dangerous?
[/quote]

I am super comfortable riding full speed. I do it on every single ride I take one roads. Super stable, mainly due to the wide and long wheelbase. Still can turn on sidewalks too so it isn’t just a limo trying to turn😂 I am getting the barrels from trampa on Monday so I can give you a comparison on those vs. springs then. Supposedly should give me tighter turning and more stability at high speeds
```

---
## \#31 Posted by: notepad Posted at: 2018-11-04T17:22:19.161Z Reads: 89

```
[quote="Trdolan03, post:30, topic:73379"]
Supposedly should give me tighter turning and more stability at high speeds
[/quote]

Have you tried removing your dampas,  Im tempted to do that to mine but I dont know how it would handle.
```

---
## \#32 Posted by: Andy87 Posted at: 2018-11-04T17:24:40.578Z Reads: 88

```
Get a Bluetooth module and look what you really use. My max was around 2000w per motor so far.
I didn’t have had the opportunity to go full off-road for now. Only park with small hills etc.
If you anyhow want to buy new motors think about getting some 170kV maybe.
It’s a sweet spot for speed and torque as for me.
Have a look at the torqueboard 6380 motors.
They also have a long shaft and you could use 20mm belts with them.
```

---
## \#33 Posted by: JensSjogren Posted at: 2018-11-04T17:25:11.505Z Reads: 87

```
Ahh ive seen those! so wait, are they supposed to give both better turning and more stability? 🤔
```

---
## \#34 Posted by: Andy87 Posted at: 2018-11-04T17:25:44.614Z Reads: 86

```
Definitely not to recommend if you wanna go over 50km/h 😅
Don’t ask from where I know 😅
```

---
## \#35 Posted by: Andy87 Posted at: 2018-11-04T17:27:05.986Z Reads: 84

```
I know only one who tried the elastomer damper...and this guy is just about to type 😂 @rich
```

---
## \#36 Posted by: notepad Posted at: 2018-11-04T17:27:15.552Z Reads: 85

```
Im guessing there just is not enough torque to break at those speeds.
Ive got some 13tooth's which I can replace the 20tooth ones I currently have equipped
```

---
## \#37 Posted by: JensSjogren Posted at: 2018-11-04T17:31:17.644Z Reads: 83

```
Yeah maybe that's a good idea, i already use 20mm belts with my turningy motors. However the motor pulley goes over the got the shaft by like 3mm. Not aproached any trouble with that so far.
```

---
## \#38 Posted by: rich Posted at: 2018-11-04T17:32:14.752Z Reads: 82

```
[quote="notepad, post:31, topic:73379"]
Have you tried removing your dampas, Im tempted to do that to mine but I dont know how it would handle.
[/quote]


Without dampas the speed wobbles started below 40km/h on my MTB. After 1000km with yellow dampas they weakened and got speed wobbles above 40km/h.

With elastomere dampers I've never had speed wobbles. But also 50km/h is my max speed, I'm scared above because I love life.
```

---
## \#39 Posted by: JensSjogren Posted at: 2018-11-04T17:33:29.794Z Reads: 78

```
[quote="notepad, post:36, topic:73379"]
Ive got some 13tooth’s which I can replace the 20tooth ones I currently have equipped
[/quote]

You use 20t for motorpulley? What is ypur slave pulley? How long is your belt? Im curious since i ordered 18t motor pulleys and 465mm belts to fit with my 72t slave pulleys. However im worried that the belt will be to short or that a 18t is to big to use as a motor pulley
```

---
## \#40 Posted by: Andy87 Posted at: 2018-11-04T17:33:56.804Z Reads: 77

```
So with elastomer it’s stable like with yellow dampas just turning radius is smaller, right?
```

---
## \#41 Posted by: Andy87 Posted at: 2018-11-04T17:35:32.658Z Reads: 72

```
You can calculate your belt length here
https://www.bbman.com/belt-length-calculator/
```

---
## \#42 Posted by: JensSjogren Posted at: 2018-11-04T17:39:21.971Z Reads: 72

```
Nice! Seems like i need 462mm and i ordered 465. Spot on :)
```

---
## \#43 Posted by: notepad Posted at: 2018-11-04T17:40:51.137Z Reads: 74

```
So I actually have two slave pullies,  70t and 80t because I have a 168Kv and 192Kv motor on the same build.
I use a 460t and 440t belts, but my motor mounts are unique. as you will soon see :confused:

![image|375x500](upload://c32cnTqVFPNbXMIyAyVL6tuXrUP.jpeg) ![image|666x500](upload://mYGfsDtAhqKYE1NeDEW1Km7hTrm.jpeg) ![image|666x500](upload://yEyy5RypnPp4wKbIwKTnHdrQuHx.jpeg) ![image|375x500](upload://kNSmSu91VNagxfC7I1EpOumpCrk.jpeg)
```

---
## \#44 Posted by: Eboosted Posted at: 2018-11-04T17:41:54.848Z Reads: 72

```
It would be just a tad slower for road use, I'd suggest 4:1 on 168kv or 5:1 on 190kv
```

---
## \#45 Posted by: notepad Posted at: 2018-11-04T17:44:09.490Z Reads: 73

```
I think ill definitely throw the 13t pulleys on then. and I guess by the looks of it im going to be getting the Elastomere Damper's aswell, as I was going to run without dampas and just pretension!
```

---
## \#46 Posted by: Eboosted Posted at: 2018-11-04T17:56:11.017Z Reads: 73

```
13t would skip, increase your wheel pulley
```

---
## \#47 Posted by: JensSjogren Posted at: 2018-11-04T17:57:36.304Z Reads: 74

```
Really? I have 12t motor pulley with 72t slave and it never slipped.
```

---
## \#48 Posted by: Nemesis Posted at: 2018-11-04T18:31:43.230Z Reads: 76

```
[quote="Eboosted, post:44, topic:73379"]
4:1 on 168kv
[/quote]

Music to my ears...... my setup by luck rather than judgement.. :ear::musical_score:
```

---
## \#49 Posted by: rich Posted at: 2018-11-04T20:10:39.893Z Reads: 72

```
[quote="JensSjogren, post:26, topic:73379, full:true"]
3500 watts is already overkill for a eboard if i understand correctly, the motors never really uses 80a right?
[/quote]

I have SK8 149kv motors with 5:1 gearing on 8" wheels. My settings are motor max 160A and batt max 100A (of course both vescs together). The highest value in real life was 150A motor and 97A batt max but usually the motors need at least 100-130A max each ride and 50-90A batt max depending on riding style/terrain.

[quote="JensSjogren, post:3, topic:73379"]
already ordered 66t and 15t sets from trampa
[/quote]

I used this gearing with 136kv motors. 136kv was too slow but 149kv should be good for a bit above 50km/h on nice roads. I would keep the motors and try it first with 15T/66T and eventually 18T. 

Personally I often hit top speed if I ride fast on concrete but on the other hand I like this restriction to protect myself :laughing:. I don't want to crash above 50km/h...

[quote="Andy87, post:40, topic:73379, full:true"]
So with elastomer it’s stable like with yellow dampas just turning radius is smaller, right?
[/quote]

Yes, exactly.
Springs without dampas feel a bit loose and spongy for me and unstable at speed including speed wobbles. With yellow dampas it's much better but not for turning at lower speed, turning radius is like a car so always need to jump or lift the front for tighter turns.

Elastomere can get more compressed than springs that's why it's possible to make sharp turns with hard leaning and bindings but it's still stable at speed. It's different to springs and takes some rides to get used to it but I love it. Feels like a Mountainlongboard now, that's how I describe it, more alive than with springs where it's restricted. It's f***** smooth and I won't go back to springs, never ever. E-Toxx 4 life, @Nowind and @Duffman for president!

https://youtu.be/S1ezP3P8HSg
```

---
## \#50 Posted by: Eboosted Posted at: 2018-11-04T20:12:18.781Z Reads: 70

```
Sorry I must have added 7" pneumatics because 8" are a bit too much
```

---
## \#51 Posted by: Nemesis Posted at: 2018-11-04T20:20:22.780Z Reads: 69

```
[quote="Eboosted, post:50, topic:73379"]
a bit too much
[/quote]

Please elaborate as im looking at new tires at this time, a bit much how?
```

---
## \#52 Posted by: Trdolan03 Posted at: 2018-11-04T20:33:21.514Z Reads: 70

```
[quote="notepad, post:31, topic:73379"]
Have you tried removing your dampas, Im tempted to do that to mine but I dont know how it would handle
[/quote]
Yes. I ran just springs in the front and yellow Dampa in the back. This is common appearantly when you don’t run dampas ![image|375x500](upload://4vtYjQ3sGS0wsoJb5XnAk7cQ49f.jpeg) ![image|375x500](upload://bS8Y4lqDLaqHCkRDwmRoQK2KHfo.jpeg)
```

---
## \#53 Posted by: notepad Posted at: 2018-11-04T20:40:33.714Z Reads: 68

```
Woah,  the fuck.   I wonder if I could get away with putting a decent bit of pre-tension into the spring if that would stop it.  unfortunately im incredibly light (60kg) so even the softest dampas reduce my turning circle into a truck.

someone needs to get around to making thoes inserts out of metal. they wont break that way!
```

---
## \#54 Posted by: Jmding Posted at: 2018-11-04T21:27:27.300Z Reads: 64

```
Gearing up to 60 kmh reduces torque by 65 percent or so.

Going up in Kv to 200 increases maximum current capability by 35 percent or so.

So if you don't touch your gearing, go up to 200 Kv motors and increase your motor current by 35 percent, you won't meaningfully affect your current either up or down
```

---
## \#55 Posted by: professor_shartsis Posted at: 2018-11-04T21:29:32.980Z Reads: 66

```
[quote="Jmding, post:54, topic:73379"]
Gearing up to 60 kmh reduces torque by 65 percent or so.
[/quote]

Gearing up to 60 kmh reduces torque **to about** 65 percent or so.

Gearing up to 60 kmh reduces torque **by** 35 percent or so.
```

---
## \#56 Posted by: rich Posted at: 2018-11-04T21:44:30.921Z Reads: 67

```
Haha I just wanted to say it can happen with dampas, too but after checking the pics I realized that it happened to me once when using springs only :rofl:

![164404|690x388](upload://2FCqki9UGE19Y0Ir6LVnjkLNR8M.jpeg) 

![214025|690x388](upload://4mZ3I1UYTwzlbzjmwmMotyCUVBT.jpeg) 

[quote="notepad, post:53, topic:73379"]
I wonder if I could get away with putting a decent bit of pre-tension into the spring
[/quote]

I don't know but in any case I would add some pre-tension otherwise the springs can pop out on hard leans or including spring retainer like here (achieved with extreme lean at home)

![174214|690x388](upload://2hAcBzLG8o7waDxAlGOv3TJJsjb.jpeg) 

Do you use bindings?
Just give it a try with a bit pre-tension and don't ride too fast.
```

---
## \#57 Posted by: notepad Posted at: 2018-11-04T22:02:45.843Z Reads: 66

```
[quote="rich, post:56, topic:73379"]
Do you use bindings?
Just give it a try with a bit pre-tension and don’t ride too fast.
[/quote]

I do use bindings, but only because they came with the deck.  Its only going to be a road runner so no heavy duty terrain hopefully.
```

---
## \#58 Posted by: rich Posted at: 2018-11-04T22:14:34.167Z Reads: 66

```
Good reason :wink:
Bindings help you to make tighter turns.
```

---
## \#59 Posted by: pjotr47 Posted at: 2018-11-04T22:14:51.105Z Reads: 65

```
I was thinking of a 6384 motors 170kv with those etoxx 1:4 hellical drives and 8or7 inch wheels. 

But i would be better with something around 140-150kv?
```

---
## \#60 Posted by: professor_shartsis Posted at: 2018-11-04T22:16:22.035Z Reads: 66

```
[quote="pjotr47, post:59, topic:73379"]
But i would be better with something around 140-150kv?
[/quote]


it depends on the top speed vs acceleration you want...
```

---
## \#61 Posted by: pjotr47 Posted at: 2018-11-04T22:18:12.097Z Reads: 63

```
At this moment I had, 10s 190kv with 107mm. Hit around 50km/h top speed. I want  something close to that on my trampa. I weight only 60kg and my trampa will have a 12s battery pack
```

---
## \#62 Posted by: professor_shartsis Posted at: 2018-11-04T22:19:25.197Z Reads: 65

```
@pjotr47

12s / 10S = 1.2

190 / 1.2 = 158.33kv for the same top speed
```

---
## \#63 Posted by: rich Posted at: 2018-11-04T22:32:18.463Z Reads: 66

```
[quote="pjotr47, post:59, topic:73379"]
I was thinking of a 6384 motors 170kv with those etoxx 1:4 hellical drives and 8or7 inch wheels.
[/quote]


If you want about 50km/h top speed with 1:4 I would choose 130kv for 7" or 150kv for 8".
Just as a side note, APS motors are quite loud in FOC so your ride won't be "silent" with helicals, only during coasting. Since I changed to helicals on my MTB nobody turns around, even the dogs don't hear me coming and only start barking when I already passed by :laughing: The board sounds like a bicycle or e-bike with SK8 motors.

My commuter with belt drive and dual APS 6355 motors is much louder and people turn around and dogs hate me earlier or block my way.
```

---
## \#64 Posted by: pjotr47 Posted at: 2018-11-04T22:45:47.208Z Reads: 65

```
Thnx for your answer. I was thinking about those APS motors because of the longer stator. But those motors are noisy? 

I want something silent. I was running now a belt drive with a APS motor and the noise in foc was good for me.
```

---
## \#65 Posted by: rich Posted at: 2018-11-04T23:08:04.269Z Reads: 63

```
[quote="pjotr47, post:64, topic:73379"]
I was running now a belt drive with a APS motor and the noise in foc was good for me
[/quote]

I don't want to confuse you, the noise then might be alright for you. Just wanted to mention because you wrote "helicals" that APS motors seems to be louder than others. So far I had motors of 4 different brands running in FOC and APS are the loudest. 

I only have the 6355 but I've heard from other people as well that APS are loud in FOC compared to other motors. For example SK8 (and I think SK3) are not noisy in FOC.
```

---
## \#66 Posted by: pjotr47 Posted at: 2018-11-04T23:12:42.078Z Reads: 61

```
I understand. I want to enjoy the silence of the helical drive. It is difficult to understand the thing loud. It is for each person different :wink:

I heard some bad things from sk8 motors. Like strange noises etc after 150km.
```

---
## \#67 Posted by: Jmding Posted at: 2018-11-04T23:14:33.737Z Reads: 63

```
[quote="professor_shartsis, post:55, topic:73379"]
Gearing up to 60 kmh reduces torque **to about** 65 percent or so.

Gearing up to 60 kmh reduces torque **by** 35 percent or so.
[/quote]

Thanks for correction. You are right. And 65% * 135% is close enough to 100%
```

---
## \#68 Posted by: Jmding Posted at: 2018-11-04T23:17:45.696Z Reads: 62

```
[quote="Andy87, post:19, topic:73379"]
190kV is rated 4400w
150kV only 3500w
[/quote]

This is closer to reality than what we commonly see, where all 63xx class motors are described as "80A" motors regardless of Kv

Motor wattage ratings are not to be trusted, because our applications its current that kills motors, not wattage. Furthermore, high Kv motors have fewer windings, so they can use shorter, thicker motor wire, which means less winding resistance, as less heat. This is why high Kv motors handle more current, and can handle more electrical power.

The 4400 W / 3500 W "ratings" reflect this somewhat.  In my estimation though, Kv is proportional to motor max current for the same size motor. the 190 Kv motor should be close to 30% more powerful than the 150 Kv motor, assuming you have the electrical system to supply the extra power.

Thus you ALWAYS want to go higher in Kv when possible, then adjust gearing to bring the speed back down. Obviously dont go so high in Kv to go over the 60k erpm limit, and dont go so high in Kv that it would take wheel pulleys larger than your wheels themselves to achieve the gearing you want, but otherwise, when you have the choice, high Kv + high gearing is the way to go
```

---
## \#69 Posted by: Trdolan03 Posted at: 2018-11-05T04:03:35.916Z Reads: 58

```
@rich what do you fill your gear drives with?
```

---
## \#70 Posted by: mynamesmatt Posted at: 2018-11-05T05:43:55.024Z Reads: 56

```
[quote="JensSjogren, post:13, topic:73379"]
192 kv 4400 watts (100a)
[/quote]

sk8s 6474 at 192kv are amazing my friend
![Snapchat-1610229567|257x500](upload://27RnJwEIDLb20HR7fktWO9apLWX.jpeg)
```

---
## \#71 Posted by: JensSjogren Posted at: 2018-11-05T07:09:23.626Z Reads: 55

```
[quote="Jmding, post:68, topic:73379"]
when you have the choice, high Kv + high gearing is the way to go
[/quote]

Well explained! I assume that switching from 149kv 3500w to 192kv 4400w motor would shorten my range on the board though? Or would this just be the case during heavy riding?
```

---
## \#72 Posted by: lrdesigns Posted at: 2018-11-05T08:21:57.751Z Reads: 56

```
They should not use much more power just going regular speed. 

Change your gear ratio first for more top speed and increase motor amps for low speed torque increase.  

If the motors get too hot and or the acceleration is not enough you will need bigger motors not just kv change.
```

---
## \#73 Posted by: JensSjogren Posted at: 2018-11-05T09:01:52.337Z Reads: 55

```
Okay, my motor amps are already at 80a per motor so that's maxed out. However the battery max per vesc is set tp 45a max. Shouldnt that mean that my motors cant get more than 45a each anyhow? As you see im a newbie in building eboards and i followed a guide to set the values that i have. 

My motors are not getting very hot at all atm, im in sweden though and outside temp has been around 5°C since i started riding the board.
```

---
## \#74 Posted by: lrdesigns Posted at: 2018-11-05T09:09:28.533Z Reads: 56

```
[quote="JensSjogren, post:73, topic:73379"]
Shouldn't that mean that my motors cant get more than 45a each anyhow?
[/quote]

Not really, battery amps limits max system power. Motor power is not directly linked to battery amps as the voltage changes with speed.

Like 40 battery amps, 40 amp X 50 volts = 2000 watts. Is max system power.

But at slow speeds the motor is at much lower voltage. 

Like 2000w / 80amps = 25 volts.  Or go even slower and the 80amps starts to limit power, at 12.5 volts X 80 amps = 1000w Slower still 6vX80a=480 watts. So you see at slow speed motor amps limits torque.

As you pic up speed it starts to even out.

People say motor amps effect slow speed torque "mostly" and battery amps effect high speed torque "mostly".

Temperature is the only real limitation for BLDC motors, your lucky to have low temps outside. Lower your gear ratio and increase motor amps till your motors get too hot then turn it down a bit. If you want more torque AND more speed bigger motors is pretty much the only way. Or higher voltage but that might just make the motors hotter which means you need a bigger motor. Around 60c is ok operating temperature, which is quite hot to the touch. 80c or over is probably shortening their life.
```

---
## \#75 Posted by: JensSjogren Posted at: 2018-11-05T10:01:16.776Z Reads: 57

```
So you mean that i can increase the motor amps to more than 80a even though that is the rated max? Just keep an eye on the temperature so that it doesnt get to hot? 

Hmm i thought that the voltage was constant from the battery through the system, interesting.
```

---
## \#76 Posted by: lrdesigns Posted at: 2018-11-05T10:04:32.327Z Reads: 59

```
Yes you can. The max in reality is dependent on how long your at that load, ambient temp etc etc. monitoring temps and testing is the only way to find the actual limit.

The voltage from the battery to the esc is constant, then esc modulates it to control rpm and torque.
```

---
## \#77 Posted by: rich Posted at: 2018-11-05T22:49:36.071Z Reads: 54

```
[quote="Trdolan03, post:69, topic:73379, full:true"]
@rich what do you fill your gear drives with?
[/quote]

Mostly with this stuff, it's a spray grease which is thin and gets thicker after a short time and it's white.

![155939|690x388](upload://akRxuYDCwg3ylJM3BOAD8oiYDc9.jpeg) 

Once I used plenty of  thick black Lithium grease but that wasn't funny to remove from black gears. It was more silent for the first minutes but then sticked more to the housing than the gears.

I prefer spray grease because you can apply it as often as you like. Thanks for reminding me to do that today :laughing:. I was riding 140km since the last time and it feels a bit smoother after re-greasing. Normally I add a bit grease each 100km.
```

---
