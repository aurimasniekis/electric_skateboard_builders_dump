# 6355 260kv voltage question

### Replies: 14 Views: 846

## \#1 Posted by: ProgressionOfFun Posted at: 2018-02-15T14:50:42.246Z Reads: 113

```
Long story short ive been researching for a long time now for my first build and finally decided to bite on some TB 260kv motors with the intention of running 10-12s as theyre website recommends. The night after biting i learned the actual erpm limit for the vesc is somewhere around 60k. I now know this obviously wont work. I was wondering what experience you guys have with this, i understand 8s is going to be safe, what about 9s(its right at the limit). I really dont wanna go through the hassle of exchanges for the 190kv motors
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2018-02-15T14:53:10.615Z Reads: 112

```
If you use a very high quality VESC, such as FOCBOX's, VESC6, Ollin VESC... you will most likely be fine however not on a TB VESC unfortunately.
```

---
## \#3 Posted by: ProgressionOfFun Posted at: 2018-02-15T14:55:47.785Z Reads: 110

```
@BoostedBuilder interesting, could you link me to some of these higher quality vescs? Are you saying a 10-12s pack would work with these?
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-02-15T15:02:55.770Z Reads: 103

```
Well I'm not saying that it will, but there is a high chance. Just search the names : )
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-02-15T15:03:17.135Z Reads: 98

```
Focbox: virtually non existent 
Ollin vesc: literally non existent
Trampa vesc6: insanely overpriced ($350)

ESCape isn’t too bad tho

I definitely recommend you just trade them for 190kv’s tho, it’ll lead to a board with more power and will be much more reliable in the long run. also, with 260kv and 10s or 12s it will be highly inefficient
```

---
## \#6 Posted by: mmaner Posted at: 2018-02-15T15:05:03.343Z Reads: 91

```
here's the math...

S      Nominal Peak
6S    22.2v   25.2v
8S    29.6v   33.6v
9S    33.3v   37.8v
10S   37.0v   42.0v
12S   44.4v   50.4v

ERPM (Electrical RPM)
  KV * MAX Voltage * 7 = ERPM

260KV * 25.2v * 7 = 45864 ERPM
260KV * 33.6v * 7 = 61152 ERPM
260KV * 37.8v * 7 = 68796 ERPM
260KV * 42.0v * 7 = 76440 ERPM
260KV * 50.4v * 7 = 91728 ERPM
```

---
## \#7 Posted by: ProgressionOfFun Posted at: 2018-02-15T15:12:43.301Z Reads: 85

```
Thanks for the wisdom guys, once again this site is the best. Ill look around and make a decision a little later. Leaning towards exchanging at this time however.
```

---
## \#8 Posted by: Deckoz Posted at: 2018-02-15T15:13:33.019Z Reads: 81

```
I know this is almost irrelevant but a couple of us have some miles in on 

13s 
54.6v * 190kv * 7poles = 72618 erpm

On the focbox and Stewii ESC. It's awfully close to the 10s 260kv... But I feel like the 260kv would be dealing with terrible heat saturation
```

---
## \#9 Posted by: ProgressionOfFun Posted at: 2018-02-15T15:17:39.382Z Reads: 79

```
Hear saturation? @Deckoz

Edit, nvm. Ill look it up
```

---
## \#11 Posted by: ZackoryCramer Posted at: 2018-02-16T02:03:51.209Z Reads: 55

```
I am pretty sure 260kv bldc’s are meant for 6s packs. Tb could be just saying that it supports 12s to push them out into the market since everyone’s starting to use 10 or 12s.
```

---
## \#12 Posted by: ProgressionOfFun Posted at: 2018-02-16T05:40:52.095Z Reads: 45

```
Thats what im saying tho, you shouldnt give the implication that it could be run at 10/12s when it really cant. Just frustrating
```

---
## \#14 Posted by: ProgressionOfFun Posted at: 2018-02-16T13:59:02.695Z Reads: 35

```
Im talking about where they say they recommend a 10s/12s battery setup. (Without mention of the 190kv motors) To me, that implies the 260s are ready to go for that 10/12s setup. I dunno man, i guess its just a stupid mistake on my part. Thanks for all the help. Im sure ill have more questions later. Looking forward to opening a build thread.
```

---
## \#15 Posted by: GrecoMan Posted at: 2018-02-16T14:52:24.009Z Reads: 31

```
did you miss the “designed specifically for a 6s battery setup” part?

not trying to be rude, just seriously wondering
```

---
## \#16 Posted by: ProgressionOfFun Posted at: 2018-02-16T15:04:40.347Z Reads: 30

```
I didnt miss it, but just because its specifically designed for one thing doesnt mean its not capable of something different. Its my bad tho, will be exchanging them.
```

---
