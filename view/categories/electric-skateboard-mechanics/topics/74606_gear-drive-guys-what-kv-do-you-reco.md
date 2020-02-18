# Gear drive guys - what KV do you reco?

### Replies: 6 Views: 191

## \#1 Posted by: brently Posted at: 2018-11-13T19:24:29.026Z Reads: 85

```
So I have some 4:1 @Kaly gear drives that I'm going to be hooking up to some 6384 motors, battery is a 10s6p, wheels are 6.5'' trampa.

From what I gather the esk8-calc (http://calc.esk8.it/#{%22batt-type-lipo%22:0,%22batt-cells%22:10,%22motor-kv%22:200,%22system-efficiency%22:87,%22motor-pulley-teeth%22:10,%22wheel-pulley-teeth%22:40,%22wheel-size%22:165}|) isn't the best for calc'ing gear drive top speed. 

I was talking to a guy who has the set up I'm looking at with 6380 motors that are 170kv and he was saying he gets up to around 35 and still has more to go. 

So I figured I'd ask the forum and see what you all have to say. Basically I want to be topping out at around 37- 40. What KV would everyone reco? I like 170kv a lot on my DIY. But wasn't sure if that would be enough to get me over 34ish? 

Can anyone let me know their actual confirmed top speed (either good GPS or Bluetooth connected to motors or Speed Gun) with 4:1 gear drive and let me know what their KV and battery set up is?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-11-13T19:29:46.721Z Reads: 76

```
Why the calculator isn’t good for gear drive?
The values are very close to the real world values you will get.
If somebody tells you something different he put wrong numbers or lay you.

Keep in mind that other 6384 motors like the aps motors have a 10mm shaft which will not fit to the kaly gear drive.
```

---
## \#3 Posted by: brently Posted at: 2018-11-13T19:36:51.199Z Reads: 71

```
I don't know - not that mathematically inclined. My assumption is the "efficiency" factor. From my sample size of one other boarder saying they're getting 35 and over with a 10s and 170kv in real world I'm assuming that gears are more efficient than belt. So I'm asking the forum what top speed, battery and KV they're getting so that I can better understand what efficiency is being achieved with gear drive set ups. 

For example with belts I'm getting around 88% efficiency so maybe gears are something like 95%?
```

---
## \#4 Posted by: Acido Posted at: 2018-11-13T19:40:33.541Z Reads: 63

```
put it at 70 and be surprised with real world results
being picky is just a waste of time trust me once you get on the board you will be amazed anyways
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-13T19:41:22.424Z Reads: 60

```
The calculator is using nominal voltage.
So with full charged battery the end speed is higher.
Use 11 or 12s for 170kV and 85 percent and you get your 35mph
So for 10s a bit less than this
http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":170,"system-efficiency":85,"motor-pulley-teeth":10,"wheel-pulley-teeth":40,"wheel-size":200}|
```

---
## \#6 Posted by: dg798 Posted at: 2018-11-13T19:42:51.489Z Reads: 52

```
You could use @Kug3lis new calculator. The thread is on here somewhere. He posted a link to it. Seems very good
```

---
