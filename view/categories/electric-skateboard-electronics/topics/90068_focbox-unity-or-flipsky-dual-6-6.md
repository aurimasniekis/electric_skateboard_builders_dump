# FOCBOX Unity or Flipsky dual 6.6

### Replies: 19 Views: 923

## \#1 Posted by: Rcsup1 Posted at: 2019-04-10T18:00:56.069Z Reads: 245

```
Hi all,

I am building a razor crazy cart and will be installing dual Sensored 6384 170kv motors. I have done a ton of research but still can't decide on what esc/controller to use.

 I will be running it on 12s with a hall effect foot throttle and want it to light up the front tire when I hit the gas, so I need one that will be able to take that kind of abuse..lol

What are would be your preference for the best bang for the buck esc??
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-10T18:01:42.539Z Reads: 245

```
https://www.electric-skateboard.builders/search
```

---
## \#3 Posted by: brenternet Posted at: 2019-04-10T18:04:33.262Z Reads: 241

```
Unity is largely an unknown at the moment. Obviously loads of people are using them and results seem to be positive.

6.6 dual has improved slightly recently but even the first iteration was reliable if it came out the factory correctly, common Asian QC concerns.

I use unities but if I was going to really blast it I would consider 6.6 architecture to be better personally.
```

---
## \#4 Posted by: Steven1 Posted at: 2019-04-10T19:58:08.231Z Reads: 224

```
I would go for the Unity over the 6.6. It has much better QC and will be easier to setup. Beta testers had a hard time killing the unity. The 6.6 has the voltage issue and some people have had issues with them i.e. half the board not working anymore
```

---
## \#5 Posted by: Arzamenable Posted at: 2019-04-10T20:03:36.988Z Reads: 214

```
The unity footprint is worth it. It’s sooo little, how do all those electrons even fit?

I abused mine at a legit amateur level without issue, Longhairedboy tortured them at a professional level without issue.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-04-10T21:02:27.011Z Reads: 204

```
Don't worry I'll abuse them at 13s and see how they hold up
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-04-11T05:37:08.055Z Reads: 176

```
The fit because they are not capable of outputting the rated current for more than a few seconds. I have heard alot of complaints about the unity and how much torque is missing. The flipsky ones are not always flawless but cs has been helpful and quick to fix everything. They can output brutal amounts of power for quite a long time.
```

---
## \#8 Posted by: Rcsup1 Posted at: 2019-04-11T14:34:28.513Z Reads: 161

```
Well that is certainly a concern since this will be on a cart, that I will be thrashing pretty hard. I definitely need the output to be up to the task!
```

---
## \#9 Posted by: Dirt_Bag Posted at: 2019-04-11T16:12:43.556Z Reads: 151

```
If you have motors bigger than 6384, i would recomend the maytech 200a vesc 6. Its a single vesc with 200a output
```

---
## \#10 Posted by: sayekim Posted at: 2019-04-12T10:59:42.309Z Reads: 134

```
Neither. 

Focbox or vesc6 or chaka’s esc.
```

---
## \#11 Posted by: Rcsup1 Posted at: 2019-04-12T14:43:05.668Z Reads: 118

```
Yeah I saw the maytech 200a  but it would be considerably more money for two of those. The motors I have are 6384's.
```

---
## \#12 Posted by: Dirt_Bag Posted at: 2019-04-12T15:26:18.451Z Reads: 114

```
You definetely need the flipsky 6.6 dual for its 100a abilities. I would recommend adding a small fan as well. Karts can pull alot more current because you are sitting down and can handle acceleration better. Buying cheap means you buy twice.
```

---
## \#13 Posted by: taz Posted at: 2019-04-12T15:42:16.597Z Reads: 108

```
Why buy a vesc? Won't you have mechanical brakes?
```

---
## \#14 Posted by: Rcsup1 Posted at: 2019-04-12T15:43:43.264Z Reads: 107

```
Yes I will. What would you recommend I get ?
```

---
## \#15 Posted by: taz Posted at: 2019-04-12T15:47:40.254Z Reads: 105

```
Vescs are fantastic controllers with a lot of adjustability and the best electrical brakes so far.

However they also have some shortcomings such as input voltage limited to 60V (essentially 13s is the max limit), limited power output, low max erpm limit, high price etc.
```

---
## \#16 Posted by: Rcsup1 Posted at: 2019-04-12T18:46:17.362Z Reads: 95

```
I found this one from flier which seems like a pretty good deal, but my motors are sensored and this esc is sensorless so i'm not sure how well it would work?

# FLIER 150A 2-12S dual drive two motors 2-way ESC brushless speed controller with power switch for Electric Skateboard

https://www.aliexpress.com/item/FATJAY-FLIER-150A-2-12S-dual-drive-two-motors-2-way-ESC-brushless-speed-controller-with/32949537829.html?spm=2114.10010108.1000013.5.77dd7a03YN0Y1J&gps-id=pcDetailBottomMoreThisSeller&scm=1007.13339.99734.0&scm_id=1007.13339.99734.0&scm-url=1007.13339.99734.0&pvid=54f55e54-cc2c-43ea-ab47-6565b3aadb57
```

---
## \#17 Posted by: brenternet Posted at: 2019-04-12T18:48:20.407Z Reads: 90

```
You would just run it sensorless and not plug the sensor wires in?
```

---
## \#18 Posted by: Arzamenable Posted at: 2019-04-12T19:37:48.309Z Reads: 84

```
I didn’t read the whole post. Bang for buck and a go cart? You got the space then for cooling. I built a 4wd board for a buddy with naked/exposed flipsky 6.6 singles that come in the aluminum case. 

I got them for half off during their holiday sale. 

Here is Metr Pro telemetry and battery stats.  We are using high discharge drone lipos, this is single esc data, multiply some values by 4, others by 2. 

https://metr.at/r/0Ad9G

These ESCs stay pretty cool, and tolerated fairly high continuous demands. Rider plus board wt is 210lbs + 30lbs. He also splashes water on them with no issue despite my concerns (yet 😒)

Only issue with controllers is the voltage reading variability. Only an issue for data nerds. 

Here is me riding on two unity’s for comparison:
https://metr.at/r/XLO1O
Accurate top speed, but just a sprint. His runs are sustained and daily since January. 

Finally, I burned up Half a dual 6.6 that didn’t have the aluminum sink. I’m still butt hurt about that.  Wanna buy a half dual 6.6 for 3wd? Jkjk.
```

---
## \#19 Posted by: Rcsup1 Posted at: 2019-04-12T20:13:19.999Z Reads: 74

```
Awesome thanks! I'll be using high discharge lipos as well 12s 75c!
```

---
