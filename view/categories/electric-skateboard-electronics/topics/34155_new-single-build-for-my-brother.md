# New Single Build for my Brother

### Replies: 55 Views: 1867

## \#1 Posted by: florensvb Posted at: 2017-09-28T07:48:26.600Z Reads: 201

```
Hey guys,

I am looking into making a new board for my brother. Haven't decided on decks and wheels etc yet but starting with the electronics:

Thinking to make a 6s2p or would 3p be better? He wanted it to be as light as possible... Are those cells good?

https://eu.nkon.nl/samsung-18650-inr18650-25r.html

Would a 60a bms like this one be sufficient?

http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html

Thinking to go with a 245kv motor like this one

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html?___store=en_us

What are your thoughts on this setup?
```

---
## \#2 Posted by: nadir35 Posted at: 2017-09-28T08:22:41.289Z Reads: 185

```
I have this motor with a 6s2p battery and am very happy. Depending on your gearing of choice, you can either get better startup torque or higher topspeed. I get up to 35kmh with 15t / 36t and 76mm wheels.
```

---
## \#3 Posted by: florensvb Posted at: 2017-09-28T08:23:46.855Z Reads: 176

```
did you build the 6s2p yourself?
```

---
## \#4 Posted by: florensvb Posted at: 2017-09-28T09:21:38.690Z Reads: 167

```
Would you say that the batteries I chose are good for 6s2p? They can discharge at 20A so that'd give me 40A but the motor is 70A ... ?
```

---
## \#5 Posted by: florensvb Posted at: 2017-09-28T09:58:44.946Z Reads: 152

```
what BMS do you have with it?
```

---
## \#6 Posted by: florensvb Posted at: 2017-09-28T10:02:43.371Z Reads: 148

```
Hey @Namasaki why do you think a 6s2p Li-ion isn't good for esk8ing?

http://www.electric-skateboard.builders/t/6s2p-battery-diagram/30661/12?u=florensvb
```

---
## \#7 Posted by: pat.speed Posted at: 2017-09-28T10:06:49.157Z Reads: 141

```
I would suggest maybe a 3p just for some head room. Is it flat where you live? if so 2p should be ok. If you go with the 2p I would suggest a 40/45amp bms that way it will cut the load if you draw too much current and it won't ruin the cells.
```

---
## \#8 Posted by: florensvb Posted at: 2017-09-28T10:08:37.280Z Reads: 135

```
He lives in Hamburg so pretty much flat all along. But i don't want it to have a big voltage sag etc .. so might go with 3p i guess. What BMS do you suggest for 6s3p?
```

---
## \#9 Posted by: florensvb Posted at: 2017-09-28T10:09:45.264Z Reads: 131

```
[quote="pat.speed, post:7, topic:34155"]
I would suggest a 40/45amp bms that way it will cut the load
[/quote]

What do you mean "cut the load"? If i draw more than the bms can handle- won't it just fry my bms?
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-09-28T10:59:34.082Z Reads: 119

```
Go with 3p definetly, my 6s2p sags almost 40% after a nice Hill 😂
```

---
## \#11 Posted by: pat.speed Posted at: 2017-09-28T11:41:47.891Z Reads: 123

```
Most will cut the load I think or maybe they do just fry I'm not sure. I got the impression that they would stop the current from flowing and blowing up other things. With the 3p it will be rated at 60amps from your batts so the first bms you were going to get will be good
```

---
## \#12 Posted by: nadir35 Posted at: 2017-09-28T12:17:28.255Z Reads: 114

```
No,I just hooked up two Zippy Flightmax 3s1p 5Ah 20c in series.
```

---
## \#13 Posted by: pjotr47 Posted at: 2017-09-28T14:01:07.787Z Reads: 102

```
Maybe this BMS is something? http://www.ebay.co.uk/itm/162414146757?var=461438635593 
I have the same 10s in order
```

---
## \#14 Posted by: NickTheDude Posted at: 2017-09-28T15:05:05.821Z Reads: 97

```
Are you planning on using a VESC? If so go with a lower kV motor and a 10S2P. It's only 2 cells more than a 6S3P and you'd have significantly more power. Plus your VESC would stay cooler.

Also you probably won't need a motor that big for the kind of power you're looking for. A 6354 would be fine if you wanted to save some weight.

Also most people reccomend Samsung 30Qs over 25Rs since they preform better despite their rating.
```

---
## \#15 Posted by: florensvb Posted at: 2017-09-28T15:21:46.681Z Reads: 92

```
yes ill use the focbox
```

---
## \#16 Posted by: florensvb Posted at: 2017-09-28T15:22:42.660Z Reads: 90

```
it has a switch with it? i was planing on using an anti spark .. can i just ignore the switch? also: is 50a discharge enough? :)
```

---
## \#17 Posted by: florensvb Posted at: 2017-09-28T15:24:19.436Z Reads: 88

```
[quote="NickTheDude, post:14, topic:34155"]
If so go with a lower kV motor and a 10S2P. It's only 2 cells more than a 6S3P and you'd have significantly more power.
[/quote]

Would it voltage sag more or less than a 6s3p?

Whats the ultimate kV if id go with 10s?
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-09-28T15:27:45.997Z Reads: 80

```
50a isn’t enough, go for 60a plus or bypass discharge
```

---
## \#19 Posted by: Namasaki Posted at: 2017-09-28T15:39:04.455Z Reads: 80

```
[quote="florensvb, post:6, topic:34155"]
Hey @Namasaki why do you think a 6s2p Li-ion isn't good for esk8ing?
[/quote]

Low voltage like 6s is gonna mean higher current pulled from the battery. 
And to only have a 2p is going to compound the problem.
```

---
## \#20 Posted by: florensvb Posted at: 2017-09-28T15:41:07.923Z Reads: 78

```
Fair enough ... What would you say is a good setup for a lightweight, low speed but occasional burst? He just needs to get from A to B on mostly flat ground and i don't want it to sag or anything like that. quality is a must
```

---
## \#21 Posted by: pjotr47 Posted at: 2017-09-28T15:41:09.588Z Reads: 76

```
I have go for a 10s build with the bms so the amps will be lower than 6s. So it will work for me & you can buy a lowe amps & volt switch
```

---
## \#22 Posted by: florensvb Posted at: 2017-09-28T15:59:02.762Z Reads: 78

```
so now i am completely wondering what is the best?

10s2p
8s2p
6s3p

?? :D

I think for it to stay light i'd have to stay under ~20 cells? This is my first diy pack so i am not sure
```

---
## \#23 Posted by: GrecoMan Posted at: 2017-09-28T16:00:20.226Z Reads: 74

```
For 245kv I would go with 6s3p, more continuous discharge and range
```

---
## \#24 Posted by: GrecoMan Posted at: 2017-09-28T16:01:01.121Z Reads: 74

```
Also, do you plan on soldering the cells or do you happen to have a spot welder laying around?
```

---
## \#25 Posted by: florensvb Posted at: 2017-09-28T16:01:23.990Z Reads: 68

```
soldering for the win! :P
```

---
## \#26 Posted by: GrecoMan Posted at: 2017-09-28T16:01:41.102Z Reads: 69

```
Is it super powerful?
```

---
## \#27 Posted by: florensvb Posted at: 2017-09-28T16:01:44.448Z Reads: 67

```
I can always change the motor as well ... maybe go with a smaller one
```

---
## \#28 Posted by: florensvb Posted at: 2017-09-28T16:02:14.319Z Reads: 66

```
yeah i have a 30w for small things and a 100w for bigger things. i read 80w is the minimum for getting the heat in and out quick enough
```

---
## \#29 Posted by: GrecoMan Posted at: 2017-09-28T16:02:44.618Z Reads: 68

```
100w should be good, glad you’ve done some reading unlike some other people on here...

Good luck!
```

---
## \#30 Posted by: florensvb Posted at: 2017-09-28T16:05:54.448Z Reads: 72

```
Ok now i am thinking 6s3p like @GrecoMan suggested, as its gonna give me less sag and my bro doesn't need crazy much power anyways. 

Would this 220kv motor from alien systems work well with 6s3p? I'd prefer to buy the motor from a skate shop rather than hobbyking's sk3s ... Also this one is 5055 so i can save some weight and $

http://alienpowersystem.com/shop/brushless-motors/alien-5055-sensored-outrunner-brushless-motor-220kv-2200w/
```

---
## \#31 Posted by: GrecoMan Posted at: 2017-09-28T16:07:12.255Z Reads: 71

```
I highly recommend the Tacon 245kv 6364.

It is amazing and I run it on 6s2p, ships from hobbypartz I think
```

---
## \#32 Posted by: florensvb Posted at: 2017-09-28T16:08:25.406Z Reads: 70

```
ahhh looks amazing, but don't wanna order from the US because i am in europe .. 245kv does seem to be the sweet spot for 6s mhm?
```

---
## \#33 Posted by: GrecoMan Posted at: 2017-09-28T16:09:17.550Z Reads: 68

```
245kv at 6s is great, it’s a perfect balance of torque and speed

I recommend the sk3’s over the 5055 from APS
```

---
## \#34 Posted by: florensvb Posted at: 2017-09-28T16:12:38.560Z Reads: 69

```
[quote="NickTheDude, post:14, topic:34155"]
Also most people reccomend Samsung 30Qs over 25Rs since they preform better despite their rating.
[/quote]

This the cells you're referring to?

https://eu.nkon.nl/samsung-inr-18650-30q-3000mah.html
```

---
## \#35 Posted by: NickTheDude Posted at: 2017-09-28T16:22:15.661Z Reads: 63

```
Those are the ones.

1000W / 37V (10S) = 27A
27A / 2 (2P) = 13.5A per cell

1000W / 22.2V (6S) = 45A
45A / 3 (3P) = 15A per cell

With a 10S2P you'd be drawing less amps per cell for the same amount of power as a 6S3P and have less voltage sag. There would also be less stress on your VESC due to lower amperage.
```

---
## \#36 Posted by: pjotr47 Posted at: 2017-09-28T16:27:06.858Z Reads: 63

```
I have a 10s4p build with those cells: https://eu.nkon.nl/rechargeable/18650-size/lg-18650he2-imr-battery.html
But i have now ordered a spotwelder to make a new 10s4p pack with the same cells. I don't know in what time you want to build you're board. But when making my own pack go good. I want to make also packs for the esk8 community. 

PS: I am from Belgium
```

---
## \#37 Posted by: florensvb Posted at: 2017-09-28T17:09:54.846Z Reads: 62

```
Thank you for that beautiful explanation!
```

---
## \#38 Posted by: florensvb Posted at: 2017-09-28T17:16:15.449Z Reads: 62

```
In your calculations, do the 1000W mean we are assuming this single drive build brings out a 1000W?
```

---
## \#39 Posted by: NickTheDude Posted at: 2017-09-28T17:30:06.562Z Reads: 62

```
I just chose 1000W as an arbitrary value. The ratio stands for any amount of power though.

Since 2 30Qs in parallel could put out 40A, I'd set your VESC to output 30A just to leave some headroom to keep the cells healthy. That should give you a little more than 1000W which a 6355 would be able to handle fine. Look for a motor around 190kV.
```

---
## \#40 Posted by: florensvb Posted at: 2017-09-28T20:03:00.994Z Reads: 70

```
ok so i think i am gonna go for a 10s2p as this gives me more power and less voltage sag than any of the other options, while having about the same amount of cells. furthermore i have been reading that voltage sag can influence range so significantly that 10s2p should still outperform a 6s3p in terms of range, even though it would have more mAh. 

That said, i have questions about building a 10s2p:

I understand how to wire up balance leads in a 1p battery like here

<img src="/uploads/db1493/original/3X/3/1/317517c3d5852785d44d06136b1126fa04535bf5.jpg" width="666" height="500">

but how do i go about that in a 2p? Do i join the balance leads on the packs in parallel as well before they go into the bms etc ?
```

---
## \#41 Posted by: GrecoMan Posted at: 2017-09-30T02:18:17.624Z Reads: 62

```
Calling all battery builders 

@barajabali @longhairedboy @willpark16
```

---
## \#42 Posted by: willpark16 Posted at: 2017-09-30T03:12:24.222Z Reads: 61

```
You simply add the cells to those single rows however if you don't u derstamd how to add parallel cells I wouldn't advise to go out and build a battery, have someone do it for you or read some more
```

---
## \#43 Posted by: pat.speed Posted at: 2017-09-30T04:48:15.431Z Reads: 60

```
You connect the 20 batteries into parallel and then you will have 10x 2p packs once that is done you connect the 2p packs into series to give 10s2p. The balance leads go onto all of the series connections I believe
```

---
## \#44 Posted by: longhairedboy Posted at: 2017-09-30T04:59:36.729Z Reads: 59

```
you're going to need blood. A lot of blood. And a transmutation circle.
```

---
## \#45 Posted by: florensvb Posted at: 2017-09-30T10:11:55.079Z Reads: 54

```
haha thanks for the input guys :) i understand how to wire cells in series or parallel, no problem. what i dont understand is 

1. in a 1p obviously each cell can be measured individually through the balance leads. but in a 2, 3 ... 550p :D how does that work? i join two cells in parallel an just have them use the balance leads together?

2. if i wanna make a really flat pack, so lets say 10 x 2 next to each other (not stacked on top), how do i go about seperating them, so they dont short on the poles when the two rows are lying „next to each other“? just a bunch of isolating tape? 

hope you understand what i am asking here hahah :) cheers guys
```

---
## \#46 Posted by: pat.speed Posted at: 2017-09-30T11:34:27.521Z Reads: 60

```
1. Yes the two cells just use the one balance lead

2. You can use whatever you like eg. cardboard, tape, rubber or foam. Anything that is nonconductive

Maybe some battery builders can let you know what they use
```

---
## \#47 Posted by: florensvb Posted at: 2017-10-07T11:06:54.246Z Reads: 54

```
Hey so i was thinking ... a 7S3P would still be better than a 10S2P?

1000W / 25.9V (7S) = 38.61A
38.61A / 3 (3P) = 12.87A per cell

Is this thinking correct? The 10S BMS on alien systems is sold out for a while, thats why i am looking into other options. Are there reasons why a 10s2p would still be preferred over a 7s3p? The cell count only differs by 1 cell ...
```

---
## \#48 Posted by: pjotr47 Posted at: 2017-10-07T11:13:54.404Z Reads: 50

```
I have this small BMS but i don't have tested yet http://e-greenmotion.com/index.php?route=product/product&path=111_128&product_id=288
```

---
## \#49 Posted by: florensvb Posted at: 2017-10-07T11:15:54.185Z Reads: 52

```
Interesting! Cause that one also has a switch and a cable for LED indicators ... Do you think they are shipping from within Europe?
```

---
## \#50 Posted by: pjotr47 Posted at: 2017-10-07T11:23:55.109Z Reads: 50

```
Yeah its a very small bms included the switch and led indicators cable :slight_smile: . I'am from belgium but i have orderd from them with ebay but they have stopped selling on ebay. You can send them a mail, they answer very fast
```

---
## \#51 Posted by: BoostedBuilder Posted at: 2017-10-07T14:14:47.204Z Reads: 47

```
You could get these, they look good! 
https://eskating.eu/product/10s2p-eskating-electric-skateboard-battery/
https://eskating.eu/product/7s3p-eskating-electric-skateboard-battery/
```

---
## \#52 Posted by: florensvb Posted at: 2017-10-07T14:19:25.808Z Reads: 49

```
its true thats a pretty cool offer. only thing is that id prefer 30q cells over 25r and i kind of wanna take the challenge and build my own battery pack :)
```

---
## \#53 Posted by: BoostedBuilder Posted at: 2017-10-07T14:27:09.474Z Reads: 47

```
It'd honestly be cool if you make it yourself! I'm just scared since I think it's the most important/dangerous part and I just don't trust my hands((
Do you have any tools? Spot welder, soldering iron?
```

---
## \#54 Posted by: florensvb Posted at: 2017-10-07T14:27:35.809Z Reads: 49

```
Yes i have a 100w soldering iron :)
```

---
## \#55 Posted by: florensvb Posted at: 2017-11-11T19:16:44.240Z Reads: 39

```
A while later ... :D 

<img src="/uploads/db1493/original/3X/3/c/3ca155fb3812da59bc3b947176f9f18a4c4ea6e4.jpeg" width="374" height="500">

Not the best hot glue and soldering job but the cells stayed cool and the connections feel legit :)
```

---
