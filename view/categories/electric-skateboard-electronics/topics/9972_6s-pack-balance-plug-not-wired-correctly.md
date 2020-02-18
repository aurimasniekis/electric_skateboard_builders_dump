# 6S Pack Balance Plug Not Wired Correctly

### Replies: 10 Views: 726

## \#1 Posted by: michaeld33 Posted at: 2016-09-22T04:25:42.672Z Reads: 71

```
Hello,
The pictures explain this best, but basically, I am having an issue with a battery I just threw together when my last one broke, basically the voltages are all over the place, even tho the individual cells read correct voltage (around 3.5v)
Take a look at the images to get a better understanding. I believe there is a mistake in the balance plug wiring but I don't understand what. It doesn't even think the pack is 6s, it thinks it's 5S.

<img src="/uploads/db1493/original/3X/a/4/a45fe5268b148531f3ef97682931cc63ee105e9a.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/7/f7a8a148333ca2a1ec9249c030a27f1eb6183f23.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/3/5/35d65663866dc7a4b819cf707604b8abb67faceb.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/8/2/82a559aba8f73931bf41ee433b303d9d0e2b7dcd.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/7/e76e1a42945358133855334c26600c2b9233ef7e.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/8/f84be29db260b4e155dc9b2c2e0434da1e00806e.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/7/1/7120226a998060ad443932dd51431b684d20ff1f.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/0/e0a0b9436ca75793a4715ddac07a3e0f89cc51bb.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/7/c/7cc2dabb208c8942062a980c12c754b5f100fadf.jpg" width="375" height="500">
```

---
## \#2 Posted by: saul Posted at: 2016-09-22T04:57:47.785Z Reads: 57

```
got a wiring diagram? should be one wire between each series cell.

maybe some hot glue on that jst is getting in the way from making contact. did you check cell voltage directly? try on the jst to see if theres a break.
```

---
## \#3 Posted by: michaeld33 Posted at: 2016-09-22T04:59:08.177Z Reads: 57

```
Tried it on the JST, it's weird, doesn't work right. the 6th cell reads 22v.
```

---
## \#4 Posted by: saul Posted at: 2016-09-22T05:06:55.265Z Reads: 57

```
maybe one pin out of order? double check, just be careful not to short anything :thinking:
```

---
## \#5 Posted by: lox897 Posted at: 2016-09-22T08:11:01.967Z Reads: 42

```
If those numbers are what order you are putting the cables in, I am quite sure they are wrong. You need to do it at each series connection.
```

---
## \#6 Posted by: michaeld33 Posted at: 2016-09-22T11:27:46.315Z Reads: 35

```
Yes that is where I connected the balance leads... Really? That's how it looked on ebikeschool.com tutorial...
```

---
## \#7 Posted by: TheImmortalJew Posted at: 2016-09-22T14:26:22.233Z Reads: 34

```
It's hard to see, but I think your wiring is off on the balance connector. Your numbering is a little confusing to me...I like to start from my main (+) as wire 1, in this case your only red wire. Then go in line with wires 2,3,4,5,6 on your successive (+) terminal of each pack. In your case I would solder 2-6 right between the two (+) on the nickel strip. If you have 1 wire left and it's on the correct (-) side of the plug you should be good.

But in this picture it looks like you have (in your numbering) wires 3 and 6 backwards? I can't see the connector that well. 
<img src="/uploads/db1493/original/3X/b/2/b22d22f5887370590fc0ad29e6ed29e86eaf5485.jpg" width="375" height="500">
```

---
## \#8 Posted by: Blasto Posted at: 2016-09-22T14:32:20.778Z Reads: 33

```
should be this

<img src="/uploads/db1493/original/3X/a/5/a5cba9c9af9a99ebf32797952b141b591418c3cd.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/b/2b0dba04ace168ee5a796a0e6c9800598b44652e.jpg" width="375" height="500">
```

---
## \#9 Posted by: michaeld33 Posted at: 2016-09-22T21:06:05.141Z Reads: 25

```
Aw sweet! It works! Thanks so much man!
```

---
## \#10 Posted by: lox897 Posted at: 2016-09-22T22:19:09.286Z Reads: 21

```
Here is a diagram from whitepony:
<img src="/uploads/db1493/original/3X/1/9/1981de739604e2d86da82ea20a8c3d56e60e5876.jpeg" width="690" height="175">
```

---
