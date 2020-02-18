# Will this Battery work with my board?

### Replies: 22 Views: 2524

## \#1 Posted by: joeykache Posted at: 2016-04-13T02:29:25.038Z Reads: 130

```
Hey everyone, I'm a little newer in the DIY scene. I wanted to buy this Battery for a tacon 160 motor, would It function properly? Thanks again in advanced. I'm also using a VESC from chaka.

http://www.hobbyking.com/hobbyking/store/__55805__Multistar_High_Capacity_Lightweight_8S_12000mAh_2C_Multi_Rotor_Lipo_Pack.html
```

---
## \#2 Posted by: wallaboo Posted at: 2016-04-13T02:44:38.639Z Reads: 126

```
Those batteries are very common. I bought something very similar myself. Instead of buying the 8S pack, I got multiples of a smaller S rating battery. This is going to give a lower profile and I get the added bonus of wiring my first circuit :grinning:

You should also look into getting an anti-spark on/off switch of some sort.
```

---
## \#3 Posted by: onloop Posted at: 2016-04-13T02:45:29.674Z Reads: 122

```

It only has a 2C discharge rate (3C peak), but you can control the discharge rate using the VESC.

I suppose it depends on how you design the drive train & what your expectations are. I think it will work.

ALSO read this:


http://www.electric-skateboard.builders/t/what-is-battery-c-rating-is-it-important-for-electric-skateboards/36
```

---
## \#4 Posted by: mattdig Posted at: 2016-04-13T02:51:41.109Z Reads: 108

```
The C rating is way too low. 3C only gets you 36A (3 x 12Ah) max discharge and you want at least 60A constant, maybe 100A max or more. Find something with a higher C rating, I'd go with at least 10C constant, depending on the battery capacity.
```

---
## \#5 Posted by: joeykache Posted at: 2016-04-13T03:05:57.511Z Reads: 103

```
Wow, thanks for the quick responses guys. Really appreciate it. I'll see what I can get done on my end.
```

---
## \#6 Posted by: chaka Posted at: 2016-04-13T03:16:13.198Z Reads: 94

```
If you discharged two of those in parallel you would have a usable pack. It would be big and bulky but you would have really good range. The pack can be flattened and the cells rewired if you are ambitious.
```

---
## \#7 Posted by: joeykache Posted at: 2016-04-13T05:27:34.235Z Reads: 84

```
Hey Jeremiah, thanks for the info. Any tutorials or write-ups you've come across with flattening and re-wiring? Thanks again.
```

---
## \#8 Posted by: Kaly Posted at: 2016-04-13T09:47:13.174Z Reads: 80

```
This battery is no good for eBoard,  in my experience you do not want anything lower than a 10C discharge rating. 

Because once you get more comfortable with your eBoard you'll be lacking speed and power due to the low discharge capacity of the pack.
```

---
## \#9 Posted by: chaka Posted at: 2016-04-13T12:28:27.004Z Reads: 77

```
@lowguido is doing a build. You need a special flux for aluminum to solder the tabs.
```

---
## \#10 Posted by: chaka Posted at: 2016-04-13T12:30:26.123Z Reads: 74

```
@kaly  Low C cells are usable but you need to increase the total size of the pack. Anything above 600 watt hours can run cells with a max 2C constant discharge.
```

---
## \#11 Posted by: Kaly Posted at: 2016-04-13T14:05:33.472Z Reads: 73

```
@chaka i have use 30C and 10C batteries and the performance takes a big hit with the lower discharge rating. 

It's no that the battery won't work but once you get more comfortable with your eBoard, that boost provided by the high discharge battery becomes a necessity.  Personally I like my board to respond like a dirt bike really snappy.
```

---
## \#12 Posted by: chaka Posted at: 2016-04-13T14:35:57.695Z Reads: 77

```
@kaly If you are after snappy performance than a large pack will give you what you need. I typically use about 1500 watts max when accelerating, sometimes more, and regardless of C rating it is not good to discharge at a rate greater than 2C for extended periods. It decreases cell life. So we take 1500 watts and divide by 2 to find the capacity we need. So if we have a pack with 750 watt hours we will only need to discharge each cell at a rate of 2C to get 1500 watts output. Cells discharged at 2C also have very little voltage sag which gives us a very snappy throttle response and an almost flat discharge curve.

The other side of the coin is cruising performance and range. We only use about 300 watts when cruising at roughly 20mph so we are looking at a discharge rate 1/2C when cruising. Cells will live a long and happy life and have gobs of power when in this configuration.
```

---
## \#13 Posted by: barajabali Posted at: 2016-04-13T16:07:04.366Z Reads: 72

```
http://www.amazon.com/Aluminum-Solder-Wire-062-Flux/dp/B00DC3102Y?ie=UTF8&psc=1&redirect=true&ref_=oh_aui_detailpage_o03_s00

Youll need this and a good quality soldering iron.  to solder aluminum tabs.  thats what i use
```

---
## \#14 Posted by: Kaly Posted at: 2016-04-13T16:36:44.108Z Reads: 70

```
I can not argue with a 1500 watts/h pack but the battery here is around 365 watts/h.  It will not behave the same as the 1500 watts/h you have mention.  

@joeykache go for a high discharge rate even if cost you a little more without breaking the bank , you will not be disappointed.  A board with a snappy throttle is much much more fun. once you start in the esk8 path that's where you are going to end up Anyway, having as much fun as possible. :slight_smile:
```

---
## \#15 Posted by: chaka Posted at: 2016-04-13T16:43:19.168Z Reads: 69

```
If you follow the thread you can see that I recommended running two of these in parallel bringing the pack up to 700+ watthours. If you run two of them in parallel at 2C you will get over 1400 watts.
```

---
## \#16 Posted by: joeykache Posted at: 2016-04-13T16:52:29.835Z Reads: 69

```
Thanks for all the help guys, this is really good info. I already have a board made though - running CarvOn Single Hub, Chaka's Vesc, a really strong board and Space Cell from enertion. I'm working on my second build right now, I want to make it more custom this time around. <img src="/uploads/db1493/original/2X/a/ab17f59ab1b39cbb04f53d3afae788f8043e48ab.jpg" width="666" height="500">
```

---
## \#17 Posted by: Okami Posted at: 2016-06-03T07:56:56.883Z Reads: 46

```
Hey there, since this topic is already talking about the right battery (C rating).. wanted to ask a quick question..

Is 25C for 6s 5000 mah pack ok? Or can I also go lower with the C rating? (it would be probably 2x 3S 5000 mah battery)

I calculated that 5Ah x 25c = 125 A
5Ah x 20c = 100A

So,.. If I have a 120 A controller and 80A motor.. Should I go with the controller rating or the motor's one? 

Motor's power would probably be 2700w. Although, it is going to be a mountainboard, so the amp draw may be a little bit different (aiming for 4.27 reduction, with 245kv motor, 6s system)
```

---
## \#18 Posted by: DeathCookies Posted at: 2016-06-03T08:04:39.523Z Reads: 41

```
First you choose your motor and the batterycellcount (the s count) for calculating the top speed. When you have your aimed topspeed with motor and battery cell count you need a battery that can handle the max ampere of the motor. Maybe you aim 20% more amp from battery than the motor needs. Just to be safe.
Now you choose a ESC that can handle the given specs: Cell count and max ampere. Always take stuff that can handle more than needed! If you pull 70-90a most people here in this forum would recommend you a 150a ESC because the ESC specs are mostly shit.
```

---
## \#19 Posted by: Okami Posted at: 2016-06-03T08:08:56.291Z Reads: 39

```
Yeah, I know that you should add like 20% extra or downgrade a controller 20%.

For me that would be 120A * 0.2 = 96A. Motor is 80A continous, as I said.. 
So I think that gets me 2700w / 24v = 112A.. Which  yeah, kind of ''suggests'' to go with 150A (20% off and it is 120A)..

I suppose I could go with 25c.. to be on the safe side.. I've got to order batteries soon, and there's always a possibility to get bigger motor in the future (something like 3200w. which would probably draw a little bit more)
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-06-03T08:20:20.903Z Reads: 39

```
[quote="Okami, post:17, topic:2321"]
Should I go with the controller rating or the motor's one?
[/quote]

Go for the motor rating. The battery just releases as much energy as the motor needs. Even if the battery or the ESC has a higher rating!
```

---
## \#21 Posted by: Okami Posted at: 2016-06-03T08:22:33.940Z Reads: 39

```
Ok.. that puts me in place where I can also order 20c then..

Only though - isnt it better to have a 'safety gap' / reserve.. as not to stress the battery? Or the current is going to be for short amount of time (peak).. that it does not matter if it reached the peak output of battery?

Ok.. sorry for my incompetence.. Just figured out that the C rating is the continous one.. so.. I can probably go with as low as 15c (15x 5 = 75A), which is very close to the max motor can output.. continiously.
```

---
## \#22 Posted by: Kaly Posted at: 2016-06-03T14:24:39.000Z Reads: 33

```
Go with the 25C it performs better.
```

---
