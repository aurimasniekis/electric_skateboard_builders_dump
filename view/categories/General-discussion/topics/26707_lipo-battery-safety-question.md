# LiPo battery safety question

### Replies: 17 Views: 1620

## \#1 Posted by: TSThunder Posted at: 2017-07-03T22:49:10.068Z Reads: 130

```
So lets say I have two LiPo batteries. I connect one positive end of one battery with the negative end of the other battery to create a bigger battery. Would this connection be dangerous if I were to plug it in and out occasionally to charge it?
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-07-03T23:03:27.458Z Reads: 130

```
Usually the way people make this safe is through the use of a loop key.  People do this setup all the time in order to get more voltage out of the smaller HK battery packs.  e.g. two 3S packs in series to form 6S.  Positive to negative leads increase the voltage while positive to positive increases the total MAH, or range of the pack.

Read up some articles on the forum about loop keys and battery setups :) 

https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204?u=shuttershock

Also see this for examples of lots of electrical setups:
https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179?u=shuttershock
```

---
## \#3 Posted by: TSThunder Posted at: 2017-07-03T23:07:30.463Z Reads: 105

```
Would DIY Electric's on/off switch have the same effect as a loop key?

Also, if I were to CONSTANTLY (like just plug it in and out for fun)  plug the positive connector from one battery with the negative end of another, would it damage the batteries or no?
```

---
## \#4 Posted by: evoheyax Posted at: 2017-07-04T00:01:17.721Z Reads: 97

```
Be careful with those switches. I and many others have had issues with them. He should be releasing a better one any day now...
```

---
## \#5 Posted by: TSThunder Posted at: 2017-07-04T00:14:21.404Z Reads: 93

```
What was wrong with them?
```

---
## \#6 Posted by: evoheyax Posted at: 2017-07-04T00:16:14.489Z Reads: 92

```
They can fail shorty after installation. I have had multiple do the same thing. Dozens of others even chimmed in. Theres an entire thread full of people complaining of the same issue. He said he's working on a new design, but he never had the issue at hand.
```

---
## \#7 Posted by: ShutterShock Posted at: 2017-07-04T00:16:43.843Z Reads: 88

```
I would still put a loop key in my system even with the DIY switch if I was to buy it.  It is always good to have a way to completely isolate the electronics from the batteries

I can't really think of any good reason why you would need to constantly plug and unlpug it lol but the only thing it would do is wear out the connector faster, as long as it is not plugged into the VESC or the rest of the system.  You should never just plug and unplug the battery with it plugged into the VESC or ESC because it can create huge sparks, and destroy the connectors.  Thus, the antispark connector.
```

---
## \#8 Posted by: TSThunder Posted at: 2017-07-04T01:05:04.011Z Reads: 81

```
@ShutterShock Thank you so much. You literally just answered like 10 of my questions :))
```

---
## \#9 Posted by: evoheyax Posted at: 2017-07-04T01:16:12.646Z Reads: 79

```
I ride daily and just use a 5.5mm bullet as my on/off switch. Leave my negative connected, break the positive wire.

It sparks, it pops, but at the end of the day, it does no damage to the electronics. I just replace the plugs every 6 months or so. A lot less painful than soldering a switch that fails 15 seconds after the first or second use... lol

I agree, anti spark is better, but if you don't, make sure you replace the plugs every few months.
```

---
## \#10 Posted by: ShutterShock Posted at: 2017-07-04T02:02:05.397Z Reads: 73

```
Lol no problem!  You're welcome!
```

---
## \#11 Posted by: ShutterShock Posted at: 2017-07-04T02:03:55.620Z Reads: 70

```
Yeah you have a point.  I realize that as well.  I don't really know how the DIY switches do on the longevity side, so if you wanted to, you could forgo the switch and just use a plug like that :p 

I just hate the idea that I would be slowly damaging my hard earned purchases haha

What voltage are you running?  @evoheyax
```

---
## \#12 Posted by: evoheyax Posted at: 2017-07-04T16:51:05.683Z Reads: 60

```
50.4v, or 12s. I know some will have issues with the wasting of money, but it's like, $5 to buy a bag that'll last you 3 years, lol. A penny in the bucket compared to the cost of building boards (or at least the boards I build, lol).
```

---
## \#13 Posted by: Namasaki Posted at: 2017-07-04T17:25:57.177Z Reads: 57

```
Here is a bullet antispark connector that I have used.
They work very well 
Only the red one has the antispark so I just used it on the positive side. 
https://www.amazon.com/dp/B00RVM93YO/ref=cm_sw_r_cp_api_J48wzbFDW0YRM
```

---
## \#14 Posted by: ShutterShock Posted at: 2017-07-04T18:42:34.491Z Reads: 49

```
@Namasaki So you've got that as your on switch in addition to a loop key? Or is this all you use?  I was thinking of using this [switch](https://www.amazon.com/gp/product/B00MR1LVZS/ref=s9u_simh_gw_i2?ie=UTF8&fpl=fresh&pd_rd_i=B00MR1LVZS&pd_rd_r=GGBGZ2RPRBJ5W71XWB51&pd_rd_w=J4rkz&pd_rd_wg=Si6Gk&pf_rd_m=ATVPDKIKX0DER&pf_rd_s=&pf_rd_r=1V1G7812NP0M96Q3F001&pf_rd_t=36701&pf_rd_p=781f4767-b4d4-466b-8c26-2639359664eb&pf_rd_i=desktop), in addition to a traditional XT-90S loopkey.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-07-04T22:34:38.589Z Reads: 37

```
I don't use this antispark bullet anymore because my bms has an on/off E-switch.
I used this back when I was running 2 6s lipos that I would remove from the board to charge.
I did use it to turn the board on and off and I did not use a loop key.
```

---
## \#16 Posted by: wafflejock Posted at: 2017-07-05T03:09:11.574Z Reads: 34

```
@ShutterShock check the dimensions out on that switch it's pretty big, I picked up something like this too not realizing it was going to be massive so I just use the XT-90 Anti-spark male plug (loop-key) as the final connector by plugging into the female part that connects between the two batteries.
```

---
## \#17 Posted by: ShutterShock Posted at: 2017-07-05T06:20:20.749Z Reads: 33

```
Oh my god that thing is massive.   Thanks for mentioning that lol
```

---
