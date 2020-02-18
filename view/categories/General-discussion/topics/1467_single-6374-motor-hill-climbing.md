# Single 6374 motor hill climbing?

### Replies: 25 Views: 6033

## \#1 Posted by: michaelcpg Posted at: 2016-02-20T02:52:10.904Z Reads: 565

```
Hey guys,

I'm building a board almost identical to Enertion's Mono Raptor (Just with a different deck). I live in quite a hilly area so it's going to be interesting to see how well my board will handle my commute to work etc. 

I'm not expecting all my parts to arrive for another few weeks so in the mean time I would be interested to see see if anyone with similar setups have come across many (or any) hills that their boards can't handle?

Cheers
```

---
## \#2 Posted by: mattdig Posted at: 2016-02-20T03:23:35.032Z Reads: 562

```
Maybe don't expect it to start from a dead stop on a steep hill, but with a running start you'll never encounter a hill you can't make it up.
```

---
## \#3 Posted by: torqueboards Posted at: 2016-02-20T03:34:06.631Z Reads: 557

```
@mattdig depending on what your setup is there are some setups which you can't climb hills

@michaelcpg I'd go with a higher KV rating () and 16/36 on 10s/12s then you can climb almost everything.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-02-20T03:53:18.759Z Reads: 557

```
 I could be wrong but I thought a low KV rated motor was needed for more torque.
Anyway, one very important factor is your weight which can make a huge difference in your ability to climb hills.
I am about 185 lbs and i have ridden the yuneec ego which has a 29v battery and a single 400 watt motor, up a 1-2 deg hill with no problem at all. but anything steeper like 4 or 5 deg and forget it !
```

---
## \#5 Posted by: evoheyax Posted at: 2016-02-20T03:58:53.838Z Reads: 545

```
Using enertions r-pec on a 6s setup with an fvt esc and going at full speed (~20 mph), I could go up very steep hills. But it depends on the setup. The issue I had with this setup was belts braking over time. The teeth would eventually tear themselves apart from going up such steep hills so much. Thus why I'm building a hub motor dual drive setup now.
```

---
## \#6 Posted by: torqueboards Posted at: 2016-02-20T04:57:47.919Z Reads: 538

```
You can go 190kv or 245kv, 230kv. It's up to you. I personally prefer the higher KV motors for climbing hills. 230KV works great and still provides more then enough torque.

I go up hills faster than 200kv or less.

I find belts not even an issue. I haven't changed my belts in 6 months+.

230KV on 16/36 on 10s/12s gets me up any hill. Get's me the quickest to my top speed. There's no benefit for me going down in gearing or KV. But that's just how I enjoy riding.
```

---
## \#7 Posted by: NNGG Posted at: 2016-02-20T05:43:04.542Z Reads: 518

```
I would think a 149-190kv motor is optimal
```

---
## \#8 Posted by: psychotiller Posted at: 2016-02-20T05:55:20.168Z Reads: 508

```
245 kv is the best for pretty much every situation.
```

---
## \#9 Posted by: treenutter Posted at: 2016-02-20T06:02:00.990Z Reads: 508

```
I haven't found a hill I n my area that I can't climb with my sk3 245kv and 8s. I use 5 inch pneumatic wheels and a 4:1 gearing ratio.
```

---
## \#10 Posted by: torqueboards Posted at: 2016-02-20T07:09:09.957Z Reads: 504

```
When you climb real steep hills at 20-25% inclines... You try using a 200kv motor with 16/36 or even why would you use a 20/36. 200kv outputs less power, adds to more resistance/drag. I prefer the higher KV motor which has less drag and higher power output. Of course, I probably wouldn't go higher than 280KV. I think for eBoards that's where there's no benefit.

You'll notice the difference when your going up a 20-25% incline on 200KV 16/36 and you slow down or ease off the throttle. You try to accelerate up the hill again after losing momentum and your now crawling up the hill since you can't get that needed RPM. Think of it in relation to a stick shift car going uphill.

230/245KV and your flying again after losing momentum and engaging the throttle. At least, that's my experience with it.
```

---
## \#11 Posted by: NNGG Posted at: 2016-02-20T09:59:57.334Z Reads: 490

```
So would a 149kv on 10S be comparable to a 230kv on 6S?
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-02-20T10:56:18.727Z Reads: 490

```
Thanks for all the replies guys, been interesting to read. Think I'm going to have to do a bit more reading up on motor kv values because I still don't really understand how it all works. I've ordered a VESC, Enertion Space Cell and Enertion R-Spec 6374 motor though, so would be particularly interested to here from anyone using the same setup :)
```

---
## \#13 Posted by: torqueboards Posted at: 2016-04-04T06:55:47.739Z Reads: 464

```
@NNGG - Similar yes, but 230KV will always be a faster spinning motor with less resistance than a lower KV.

37v * 149kv = 5513
22.2 * 230kv = 5106

Going uphill with 149KV motor and slowing down in the middle of the hill. It will take you much more effort to get a few revolutions to push that eboard uphill and re-continue at the speed at which you stopped at. Sometimes, with a low KV motor with high torque.. You'll stop in the middle of the hill. You'll have to walk it up otherwise you'll result in burning out those motors.

Versus.. with a 230KV motor your RPM's are quicker. You can slow down and re-continue quicker.

For a 230KV motor, you only need 22.2v to hit 5106 rpm.

For a 149kv motor, you need 37v to hit the 5513 rpm.

For flat ground, it doesn't matter too much.

But personally, I like the higher KV rating (to a certain extent). The setup is smoother and there is less resistance so it's easier to kick on it's own.

This is just how I prefer my riding experience. Although, with the VESC max erpm issue depending on how things go I may need to do some re-thinking.
```

---
## \#14 Posted by: NNGG Posted at: 2016-04-04T07:33:25.762Z Reads: 441

```
Wouldnt you use 12S? at 4.1 volts a cell?

RPM: 7330?

Or is a SK3 192kv on 12S the best way to go?
```

---
## \#15 Posted by: Randyc1 Posted at: 2016-04-11T21:05:56.103Z Reads: 427

```
Torqueboard,....about your KV theory,...would 'nt a smaller motor gear like a 14t or 12t allow you to have even more RPM, at cruising speed , taking even more advantage of high RPM for power ???
```

---
## \#16 Posted by: Malibujv Posted at: 2017-02-14T22:21:48.212Z Reads: 317

```
I rarely encounter and climb hills from a dead stop so with momentum I don't think a slightly lower kv motor will make much of a difference.
```

---
## \#17 Posted by: memesupreme Posted at: 2017-06-22T16:22:29.398Z Reads: 275

```
I'm looking at building a 2nd board using a 42.3v battery and I want to go dual 6374 230kv motors, diyelectricskateboard used to sell them and they were 3000+ watts, I can't find anywhere else that sell them that can handle 12s batteries and diyelectricskateboard stopped making them, it's really annoying so I'll probably have to settle with their 190kvs bleh
```

---
## \#18 Posted by: Wolfcola Posted at: 2017-06-22T17:38:05.869Z Reads: 272

```
That would be retardedly fast with duals.
```

---
## \#19 Posted by: memesupreme Posted at: 2017-06-23T11:02:54.741Z Reads: 257

```
Absolutely, I plan on gearing it for about 65km/h, on paper my current board can but it doesn't have the torque to do it, mainly I want my next board to hit top speed even with heaps of wind resistance, and hills
```

---
## \#20 Posted by: Alanhunt123 Posted at: 2017-06-23T20:31:38.456Z Reads: 250

```
I live in a pretty hilly area, with some pretty steep ones! Don't know the exact grade, but I would say the steepest is somewhere between 18%-22%, which is quite steep indeed! I had a single SK3 6364 with 15/40 on 83mm wheels, and the board tackled it no problem, once I sorted out heat dissipation issues on my VESC. I could cruise up a 15% grade hill at around 18+mph! That is, given I had a running start.

By bumping up my motor max to around 120A, I was able to get the board to start from a standstill on flats, and it even had enough torque to start uphill on a single push. I weigh 175lb, so if you weigh around my weight, you should be able to get up most hills on a single 6374, assuming you gear it right!

Good luck!
```

---
## \#21 Posted by: jaymu86 Posted at: 2017-06-29T08:12:31.663Z Reads: 238

```
Good to Kno I weigh like 120 lol can't to get mine in
```

---
## \#22 Posted by: themegak Posted at: 2017-06-29T15:35:18.317Z Reads: 215

```
my man @psychotiller has what you are looking for.  https://psychotiller.com/product/6374-sensored-powerplant
```

---
## \#23 Posted by: Pedrodemio Posted at: 2017-06-29T15:43:43.291Z Reads: 213

```
The main problem I had with single wheel drive is loss of traction, some hills have really rough pavement or all deformed due to heavy vehicles, so you have to change your riding to put the most weight on the drive wheel and even so it will slip, but power wise I've climbed 17% with 230kv on 10s and 12/36 gearing, only limited by vesc overheating and weak battery
```

---
## \#24 Posted by: memesupreme Posted at: 2017-07-01T08:29:39.916Z Reads: 196

```
power plant, 230 kv, 3+kw, red and black colours, I'm crying, its perfect heheh
```

---
## \#25 Posted by: boardman5000 Posted at: 2017-08-04T20:58:41.402Z Reads: 164

```
Is there any other info out about that motor? I can't seem to find much on it, just wanted to make sure I had the right info to feed into my calcs to make sure i'm getting the right motor.
```

---
