# How to charge 2 soldered in series lipos?

### Replies: 8 Views: 1196

## \#1 Posted by: chewydinosaurs Posted at: 2017-01-23T00:12:42.839Z Reads: 122

```
So I didnt have all of the connectors to make a Y harness and so I soldered my two 3s lipos together in series. Now how do I go about charging them through the balance leads? I have a 2x3s to 6s balance cable but it shorts when I connect both balance cables together. I have a b6 lipo charger and heard somewhere that I can connect the balance leads into the 3s and 6s ports on the charger and it should be fine? I attached a picture of my battery setup and balance harness that shorts. <img src="/uploads/db1493/original/3X/2/d/2d61d86260edd0c2f0ff0b415392513ccb88f5d9.JPG" width="375" height="500">

Edit: I realized I was plugging in the wrong balance cables into the wrong sides of the harness. Im still a bit reluctant to charge through it though...has anyone else charged this way? <img src="/uploads/db1493/original/3X/8/6/8657c65b4aec2eea8face3c757eb836f7ed49ad5.jpg" width="666" height="500">
```

---
## \#2 Posted by: Okami Posted at: 2017-01-23T00:24:43.779Z Reads: 113

```
If charger sees it as 1x 6s then no problems.
It should tell if theres wrong polarity. At least my turnigy accucel 6 80w does this!
```

---
## \#3 Posted by: Okami Posted at: 2017-01-23T00:27:07.893Z Reads: 113

```
I had "twin charger" it worked great for 2x3s lipos + it did not need the discharge plugs to be inserted into adapter as it had its own xt60 plug (the 3s x2 to 1x 6s harness)
```

---
## \#4 Posted by: mmaner Posted at: 2017-01-23T00:57:37.658Z Reads: 108

```
I use a Turnicy Accucel to Charge x2 Zippy 8000mah 30c Lipos, never an issue.  You will be fine as long as your connections are good.  
I would suggest heat shrink on the balance plugs and balance adaptor if you are not taking them.out to charge, as in using a method to out a charging port in the enclosure. 

I use the MEB Simple Charging Port.

https://miamielectricboards.com/shop-1/ez
```

---
## \#5 Posted by: adamm Posted at: 2017-01-23T01:18:28.264Z Reads: 96

```
I had the same problem, If your using the adaptor make sure to go into your charger settings into "battery Check" if it isn't reading as a 6s pack the balance leads need to be switched around. Once it reads at one 6s pack you should be good to charge it. You might also want to cut the 2nd positive lead on the negative side of the adaptor as that is known to cause problems. thats how mines setup and it works great
```

---
## \#6 Posted by: jmasta Posted at: 2017-01-23T03:09:29.238Z Reads: 87

```
Cut the middle black wire on your 2x 3S -> 6S adapter.  This will prevent a short if incorrectly connected, since your batteries are permanently connected in series
```

---
## \#7 Posted by: Davey Posted at: 2017-07-08T15:55:55.338Z Reads: 54

```
@jmasta sorry for gravedigging but if I plan to use a BMS I do not need to cut this black cable, right?   :smile:
```

---
## \#8 Posted by: jmasta Posted at: 2017-07-08T17:48:06.067Z Reads: 47

```
You don't technically have to cut one of the middle wires.  If hooked up correctly, it will work either way.  That said....

Your batteries are wired in series with the main power lines.  Wiring the balance connectors in series again is redundant.  So if hooked up correctly, it will just fine.  But if the main leads are wired A+B and you hook up the balance leads as B+A... poof!  You just shorted out one of the batteries.  Cutting one of the middle wires* (usually B negative) prevents this issue. Then if the batteries are accidentally swapped, it just won't work

*To clarify, cut the middle ground wire on the balance adapter, not the actual battery
```

---
