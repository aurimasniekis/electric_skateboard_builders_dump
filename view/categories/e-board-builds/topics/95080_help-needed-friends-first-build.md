# Help needed: friend&rsquo;s first build!

### Replies: 21 Views: 237

## \#1 Posted by: ZachTetra Posted at: 2019-05-26T23:36:13.386Z Reads: 75

```
Heya guys!  I'm here on behalf of a friend, she is trying to make an electric penny board for $250.  This type of build is not what I'm used to so I need help finding better options.  Currently it's looking like $310 which is too much

Requirements:
- $250 max
- 22" penny board deck
- TKP trucks
- 80mm wheel max
- 10 mph min

Prefrences
- $200 max
- 70mm wheels
- single hub

General parts list:
- [$18] [22" plastic penny board](https://tinyurl.com/y2lysyz2)
- [$40] [6s 4000mAh li-poly](https://tinyurl.com/yy3jhpqe)
- [$24] [iMax B6](https://tinyurl.com/ycbk22oo)
- [$47] [6s hub ESC w/ remote](https://tinyurl.com/yyodgysm)
- [$10] vacuum form HIPS enclosure
- [$158] [72mm TKP hub kit](https://tinyurl.com/y293jt92)
- [$10] general hardware
```

---
## \#2 Posted by: Baumeister_RHGB Posted at: 2019-05-27T00:11:33.399Z Reads: 63

```
Hi, it certainly is possible to build such a cheap board that works.

If it can be a bit more work then plug and play, you could use an small brushless outrunner with a belt or a chain. The belt probably would have to be HTD3 due to the wheel size, so Id recommend the chain, as my HTD3 belt was skipping a lot.

You can buy a whole penny board with trucks and wheels off of eBay for around 25Dollar (or at least in Germany you can, I don't know how it is in the US, as I guess that's where you're coming from). The board won't be good for that prize, but it will be working.

You could make the motor mount yourself pretty easily if you can work with aluminum or know someone who can.

Doing it the way of building most of it yourself will be the cheapest, but also the hardest. If you want I can share a few pictures of how I made my mount.
```

---
## \#3 Posted by: ZachTetra Posted at: 2019-05-27T00:23:01.297Z Reads: 56

```
I think I can get a board for $25ish off eBay, mount with pulleys and belts for $40, a motor for $30, and clone wheels for $20 but I'm not sure if the mounts will even fit

I'd really like to see what you made
```

---
## \#4 Posted by: Baumeister_RHGB Posted at: 2019-05-27T00:36:47.846Z Reads: 51

```
The problem I had with the mount is that the axle doesn't have the length for standard motor mounts. What I came up with is basically a block that gets screwed and glued onto the truck. The plate which holds the motor gets screwed on to that block with two countersunk screws.

I hope the pictures make it more understandable.
![IMG_20190527_022501|375x500](upload://7IBO1iWMvohAsjSPeoyKZi85PtK.jpeg) ![IMG_20190527_022515|666x499](upload://vcCKAfpS1ejN8JvFsRVuVMYBL3U.jpeg)  ![IMG_20190527_022538|666x499](upload://j3l6yc3yDug0oBH1VkRqq7fG7UT.jpeg) ![IMG_20190527_022613|375x500](upload://dobFxIcjOHJH7CK7KfsrZyxSGlp.jpeg)
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-05-27T00:43:14.774Z Reads: 41

```
Damn that's clever, and that is a normal penny board truck?
```

---
## \#6 Posted by: Baumeister_RHGB Posted at: 2019-05-27T00:48:57.798Z Reads: 41

```
Yep, it is. I just turned it down to make room for the pulley and drilled the hole(s) into. If done right only one hole needs to be drilled into the truck, but I don't think you can get away without turning (or filing) at all. The benefit of working on a cheap truck is that the aluminium is pretty soft, so it wont take that long to get the truck ready to accept the mount and pulley.
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-05-27T00:50:15.062Z Reads: 39

```
How did you do the pulley?
```

---
## \#8 Posted by: Baumeister_RHGB Posted at: 2019-05-27T00:57:10.644Z Reads: 38

```
I bored it to the right diameter on the lathe, and then drilled the holes for the screws on the drill press.  You can maybe get around this step by printing a pulley. You would only need to drill holes into the wheel then, which is pretty easy with a drill press. There are some topics about 3d printed pulleys you could have a look into then.
```

---
## \#9 Posted by: Baumeister_RHGB Posted at: 2019-05-27T00:59:47.690Z Reads: 39

```
If you meant the motor pulley, that is just bored to the shafts diameter and then glued onto the motor shaft with Loctite 648. If you glue it right and give it enough time to cure it will hold up just fine.
```

---
## \#10 Posted by: ZachTetra Posted at: 2019-05-27T01:02:17.530Z Reads: 33

```
Is that a 650kv motor?
```

---
## \#11 Posted by: Baumeister_RHGB Posted at: 2019-05-27T01:04:23.080Z Reads: 33

```
Yes, i only ran it on 4s but the kv is still way to high. I wouldn't recommend useing such a high kv at all.
```

---
## \#12 Posted by: ZachTetra Posted at: 2019-05-27T01:06:13.773Z Reads: 33

```
What's the fastest you can safely go?
```

---
## \#13 Posted by: Baumeister_RHGB Posted at: 2019-05-27T01:21:22.451Z Reads: 32

```
Speed? 
Depends on who you ask, I won't go above 45kmh for now.

If you meant kV its not that easy. You should take the max speed, voltage, wheel size, and gear ratio into consideration. When using a belt with normal wheels, the gear ratio shouldn't be more than about 1:3 (just a guess, I'd rather stay underneath). If the ratio is too high, there won't be enough teeth engaged to transmit the power and the belt will skip.

If you use a chain I'd say you can have slightly higher gear ratios, as skipping teeth won't really happen here.

Here is a calculator where you can enter all your variables and see which speed you will achieve:

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:6,%22motor-kv%22:350,%22system-efficiency%22:85,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:30,%22wheel-size%22:70}|

Using 6s and a wheel of 70mm I think 350kv is about the max you want to have, with a 1:2 ratio you would be capable of 27 mph.
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-05-27T01:23:22.631Z Reads: 29

```
Oh I can get the specs, I've got some motors in a cart and a custom calculator, I just wanted to know what nominal speed I'm aiming for, I'm guessing 17mph is the highest you can reasonably go?  I got to 22 on a cheap nickle board with RKP trucks and it nearly killed me
```

---
## \#15 Posted by: ZachTetra Posted at: 2019-05-27T01:29:41.556Z Reads: 31

```
I can get a 180kv 5055 motor with a 16:36 ratio and 80mm wheels for about $75, should go 15mph on 6s
```

---
## \#16 Posted by: Baumeister_RHGB Posted at: 2019-05-27T01:31:06.732Z Reads: 27

```
On my current board I drive around at around 27mph pretty often if the road is in good condition. The board has RKP trucks whitch are 180mm wide, but the board isn't that much longer then a penny board.

On my penny board I had a max speed of around 20mph. I had gone that speed occasionally, but I wouldn't go any faster on an penny board myself.
```

---
## \#17 Posted by: ZachTetra Posted at: 2019-05-27T01:31:46.204Z Reads: 25

```
Can you put 80mm wheels on a penny board with stock trucks?  I think the stock wheels are 59mm
```

---
## \#18 Posted by: Baumeister_RHGB Posted at: 2019-05-27T01:34:40.553Z Reads: 28

```
I haven't tried it myself, but i have seen some pictures of penny boards with 80mm or bigger wheels, i don't know if they were with or without risers anymore tho. It could get pretty tight with 80mm wheels, but you can still use risers, and bigger wheels mean more comfort and a smoother ride.
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-05-27T01:50:59.049Z Reads: 25

```
Currently it looks like $150 for deck, charger, battery, esc, enclosure, hardware

The drive train should be $20 trucks, $25 wheels, $35 motor, $40 mount and pulleys, still high but it shouldn't take long to put together
```

---
## \#20 Posted by: danile Posted at: 2019-05-27T02:08:19.673Z Reads: 26

```
I have an "ebay esc" for belt drive, and 2 3s LiPos 4000mah.
lmk if interested, I'll let it go for cheap,
Dani
```

---
## \#21 Posted by: ZachTetra Posted at: 2019-05-27T02:18:19.158Z Reads: 24

```
Ooh I'm very interested, if the project goes through I will most definitely contact you about it
```

---
