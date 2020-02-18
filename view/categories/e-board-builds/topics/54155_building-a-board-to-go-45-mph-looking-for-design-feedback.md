# Building a board to go 45 mph. Looking for design feedback

### Replies: 29 Views: 1361

## \#1 Posted by: kaaaaahle Posted at: 2018-05-02T17:01:07.835Z Reads: 260

```
Hey all,

I'm in the process of building a new high speed board, and wondering if I could get some input or feedback if anyone has built a board already that can actually go that fast. I know it's been done before, but most of the one's I've seen are highly customized and gigantic (like Moe Stooge's board). I already built a board using mostly Torque Boards parts that can reliably do 36, and am looking to take it to the next level and push the limits a little bit. I only plan on going 45 wearing full face helmet and leathers because a crash at that speed can be catastrophic.

My biggest concern is not blowing out the controller trying to get that fast, so I'm wondering how much can be done with the gearing. The standard limit is 60,000 erpm for vesc controllers.

the following configuration gives me a maximum of 61,740 erpm, with 55.2 mph theoretical maximum 46 mph weighted:

**Landyachtz Evo deck**

**2x 245kv Turnigy SK3**

**10s 30Q battery**

**2x FOCBOX VESC**

**107mm super fly's**

**2:1 gearing**

I've never seen anyone using a gearing ratio less than 2:1. Is there a reason for this? It would be easier for me to get the speed I need out of smaller wheels using like a 22T:36T gearing ratio and I would prefer this for a lower center of gravity. I'm not sure the 107mm superfly's would be very good at that speed.

Anyone have any advice? Maybe anyone that has done this before and have something you would do differently?

Thanks
```

---
## \#2 Posted by: Blitz Posted at: 2018-05-02T17:10:38.110Z Reads: 246

```
Maybe just Copy @Deckoz's  build and put higher gear like 16t on the motor pulley.
https://www.electric-skateboard.builders/t/master-evo-landyachtz-abec-107-13s5p-focbox-6374-190kv-metr/44411
Or copy this Carvon Evo build. 
https://www.carvonskates.com/collections/boards/products/carvon-evo-4wd
```

---
## \#3 Posted by: onepunchboard Posted at: 2018-05-02T17:11:16.941Z Reads: 235

```
i would go 12s and lowe kv. torque will be limited and brake force would not adquit for 245kv. I did go 43mph with 260 is 1:3 ratio in control environment, with 10s lipo pushing 100amp. I was in down hill as well. problem was acceleration before end of the road and slowing down.
also as you go faster air resistance build up quickly so you might not get the highend torq u need to push through that.

I dont know the motor size so I can't say for sure tho
```

---
## \#4 Posted by: evoheyax Posted at: 2018-05-02T17:11:44.492Z Reads: 220

```
vesc six's have higher erpm limit than 60000, that was the 4.12 vescs and lower.

Gearing wise, not the guy to talk to since I build hub motors, lol.

It's not that hard to do. But it's hard to maintain torque while also having those speeds.
```

---
## \#5 Posted by: Deckoz Posted at: 2018-05-02T17:18:40.590Z Reads: 216

```
I run FOC Sensored on 13s with 15/36T on 107mm wheels..

You either need bigger wheels or less reduction to get speed. My board is nothing short of a rocket...if you go my route please build carefully and meticulously
```

---
## \#6 Posted by: professor_shartsis Posted at: 2018-05-02T19:11:33.904Z Reads: 198

```
[quote="kaaaaahle, post:1, topic:54155"]
2x 245kv Turnigy SK3

10s 30Q battery

2x FOCBOX VESC

107mm super fly’s

2:1 gearing
[/quote]


looks like you can reach about ~47-48mph before your wind drag surpasses the vehicle thrust... (bottom left chart assuming 60a battery limit & 90a motor limit per motor):

https://image.ibb.co/eLY3G7/47mph.jpg
```

---
## \#7 Posted by: Battosaii Posted at: 2018-05-02T19:14:45.191Z Reads: 182

```
My build has done 44mph with a human riding lol

Dual focbox
12s4p 30q
Dual 6374
16/33t pullies
Abec 107mm wheels

Done
```

---
## \#8 Posted by: kaaaaahle Posted at: 2018-05-02T19:21:42.275Z Reads: 177

```
yoooooo you are def the guy i want to talk to haha..

first off, your Evo board looks absolutely amazing, great work man.

i read your build thread that the other person linked above. i have a couple questions that i didn't see answered there if you wouldn't mind giving some info... i'm also prone to missing things in threads so sorry if you repeat yourself

- how fast have you gotten going on that bad boy?
- What do you expect the top speed is?
- how high erpm have you run the FOCBOX at?

thanks!!
```

---
## \#9 Posted by: kaaaaahle Posted at: 2018-05-02T19:22:49.009Z Reads: 167

```
amazing. thank you so much for this, as an engineer this is the kind of stuff i like to see
```

---
## \#10 Posted by: kaaaaahle Posted at: 2018-05-02T19:25:24.895Z Reads: 161

```
how'd you get that setup to go that fast? downhilling? cause according to eskate calculator it's not possible
```

---
## \#11 Posted by: ksfacinelli Posted at: 2018-05-02T19:27:45.285Z Reads: 154

```
Be very careful....I would suggest a running track with rubberized surface and open bail out space .....I would also investigate running pneumatic wheels 6-8inch slick tires.

good luck
```

---
## \#12 Posted by: Deckoz Posted at: 2018-05-02T19:32:18.888Z Reads: 156

```
[quote="kaaaaahle, post:8, topic:54155"]
how fast have you gotten going on that bad boy?
What do you expect the top speed is?
how high erpm have you run the FOCBOX at?
[/quote]

47mph down hill, 43 flat land.

Top is somewhere around there at full charge

FOC Sensored and Sensorless has no ERPM.. though if it was in BLDC it would be around 73kerpm at max.

As a side note
Please don't take this the wrong way by any means...

I know you've been a member over a year, and the OP says you've built and ridden a 36mph board.. but I see no posts. I only want to say, please be careful... I don't want to call you a liar, I just want you to know a 40+ mph board is serious, so please take it seriously. Again no offense, I just want all safe, and acting intelligent in the capabilities of the boards they are building.  :)
```

---
## \#13 Posted by: Battosaii Posted at: 2018-05-02T19:32:34.155Z Reads: 145

```
What settings are you putting in cause esk8 calculator gives me this.

![Screenshot_20180502-153018_Chrome|243x500](upload://clA1QhKgsIQGKkFVX0wOuo7rGyc.jpg)

Also my board was recorded with a radar gun ask @longhairedboy he's the witness that held the gun.
```

---
## \#14 Posted by: kaaaaahle Posted at: 2018-05-02T19:34:06.946Z Reads: 139

```
i forgot to change the wheel size :sweat_smile:
```

---
## \#15 Posted by: professor_shartsis Posted at: 2018-05-02T19:42:18.836Z Reads: 138

```
i'd imagine that you can top 50mph (bottom left chart) with 1.83:1 gear ratio (for example 24t motor 44t wheel)

https://image.ibb.co/f7Ldin/50mph.jpg

assuming 12S (46v) & 2:1 reduction I get 55mph...

https://image.ibb.co/m9YQUS/55mph_2.jpg
```

---
## \#16 Posted by: Deckoz Posted at: 2018-05-02T19:47:43.758Z Reads: 132

```
Just in case your curious.. 13s full noload spool
https://youtu.be/lLq1TqGgnI0
```

---
## \#17 Posted by: petter Posted at: 2018-05-02T19:47:56.859Z Reads: 131

```
About the gear ratio, hub motors are basically 1:1 so i think you can try a lower ratio if you want. though start tourque might suffer, but once you get rolling there should be no problems. also you probably have enough power to get around even at low speed anyways..

But one thing i would think about would be the currents. I had a lipo setup with a 370kv motor and a tourqueboards esc, 4s battery. Man that thing had a sick kick. but when i got a vesc it suddenly got pretty tame, it was just not capable to push those amps.. 

Though, if you were to go for higher amps, that would mean higher power and also affect the battery and so on
```

---
## \#18 Posted by: pat.speed Posted at: 2018-05-02T20:25:58.934Z Reads: 120

```
My current setup could theoriticaly push 47-48mph with the 14:27 gearing but I have now changed it to 10:27 as I was getting low torque and awful mileage. 

I’m using 12s, 190kv, 10:27 or 14:27 and 97mm wheels.
```

---
## \#19 Posted by: kaaaaahle Posted at: 2018-05-02T20:34:58.504Z Reads: 114

```
you use 12s lipos right? did you make your own battery or buy a prepackaged one?
```

---
## \#20 Posted by: kaaaaahle Posted at: 2018-05-02T20:36:11.303Z Reads: 113

```
also that cap bank looks really cool. I have often wondered the possibility of building a cap bank to be used as for some "turbo boost" :japanese_ogre:
```

---
## \#21 Posted by: Naysh Posted at: 2018-05-02T20:50:33.722Z Reads: 104

```
Where did you find this ESK8 calculator?  Looks like its the most accurate since it takes other factors in such as wind drag in.
```

---
## \#22 Posted by: skatardude10 Posted at: 2018-05-02T21:29:07.203Z Reads: 98

```
I use 20/32T gearing on 90mm flywheels. You're in CO right? Are you the one with the inboard m1?

I run 190kv motors, so all below is assuming that. I'd suggest getting 6374 dual for the additional torque at high speed. For reference, calculators put me at 37.8 or so mph with 100% efficiency and I hit around 35-36mph on flats in a good tuck and exactly 37.8 or so mph downhill.

Anyways, 20/32 works great for me. Tried 15/36 and 15/32, both of which were way too slow on 90mm flywheels. I'd suggest 20-22T/32 on 97s or 107s, as my 10s setup tops out at 37... So if you want to go faster than that, 22 gearing on 10S, but I'd go at least 5P if not 6P on the pack to push the amps you need to still have pretty good torque.

Or, calculate accounting for 4-worst case6 volt voltage drop on a 12S with 97s and 107s, and more Ps for more amps, like 5/6p again... Maybe you could hit 45mph easy with 12S, 97-107mm wheels and 20/32 gearing.

So yeah, 1.6:1 gearing is great, but I can only pump 30A each vesc with 25r without crazy voltage drop. 5P on 30Q would be ideallllllllllllll.
```

---
## \#23 Posted by: professor_shartsis Posted at: 2018-05-02T21:41:21.452Z Reads: 91

```
it’s a custom apple numbers spreadsheet. start with ground speed -> wheel rpm -> motor rpm -> back emf -> duty cycle -> motor/battery current -> motor torque -> wheel torque -> vehicle thrust -> wind drag. present implementation isn’t very user friendly. i’d be happy to share the formulas if you get stuck somewhere.
```

---
## \#24 Posted by: Namasaki Posted at: 2018-05-02T21:47:15.458Z Reads: 94

```
[quote="kaaaaahle, post:1, topic:54155"]
the following configuration gives me a maximum of 61,740 erpm, with 55.2 mph theoretical maximum 46 mph weighted:
[/quote]


10s and 245kv is  72030 erpm at full charge 42v
```

---
## \#25 Posted by: Naysh Posted at: 2018-05-02T21:53:22.137Z Reads: 87

```
No thanks, that's beyond my pay grade. I think the advanced ESK8 calculator will work for me.
```

---
## \#26 Posted by: lrdesigns Posted at: 2018-05-03T00:56:07.825Z Reads: 83

```
[quote="pat.speed, post:18, topic:54155"]
I have now changed it to 10:27
[/quote]

10 tooth motor pulley, woaha! That must wear down quickly? So a 2.7 ratio. Why not go 36/13 or 40/15 comes pretty close to 2.7.
```

---
## \#27 Posted by: professor_shartsis Posted at: 2018-05-03T03:42:55.712Z Reads: 80

```
[quote="pat.speed, post:18, topic:54155"]
I’m using 12s, 190kv, 10:27 or 14:27 and 97mm wheels.
[/quote]

[quote="lrdesigns, post:26, topic:54155"]
10 tooth motor pulley, woaha! That must wear down quickly? So a 2.7 ratio. Why not go 36/13 or 40/15 comes pretty close to 2.7.
[/quote]

10 tooth vs 14 tooth:
https://image.ibb.co/hiN2b7/10t_vs_14t.gif
```

---
## \#28 Posted by: pat.speed Posted at: 2018-05-03T06:53:31.919Z Reads: 76

```
Chain drive ftw, @lrdesigns
```

---
## \#29 Posted by: lrdesigns Posted at: 2018-05-03T06:55:20.248Z Reads: 77

```
Ohhh makes more sense in that case.
```

---
