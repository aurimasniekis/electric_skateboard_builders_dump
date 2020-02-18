# Help with understanding &ldquo;sagging&rdquo; with 10s2p battery

### Replies: 15 Views: 504

## \#1 Posted by: Hannes Posted at: 2018-05-30T18:11:57.407Z Reads: 114

```
Hello, I am building my first board and I have done alot of research but the one thing that I just can't wrap my head around is if a 10s2p battery will do it for my setup, i'm reading about it "sagging" and not being able to supply enough amperage but I cant wrap my head around it.

This is the battery im looking to buy, https://eskating.eu/product/flat-10s2p-eskating-electric-skateboard-battery-30q/

and this is the rest of my setup,
[TORQUE ESC](collections/featured-items/products/torque-esc-bldc-electronic-speed-controller)
[Mechanical kit with 218mm trucks, 36t wheel, 16t motor, 97mm wheels, 15mm bel](collections/featured-items/products/single-motor-mechanical-kit)t
[6374 190kv motor](collections/electric-skateboard-starter-collection/products/electric-skateboard-motor-6374-190kv)

My weight is 70kg

What does it mean when it's sagging, will it have slow acceleration? will it bog down? (I live in medium to no hilly area, mostly flat) Is it purely acceleration that will take a hit?

And this is pretty much what i can afford right now 250eur is it better to go with [2 of these zippy](https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c-xt90.html)?
/Hannes
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2018-05-30T18:29:06.083Z Reads: 102

```
Voltage sag means that voltage is 'traded' for higher amps. So when you're going up a steep hill, you'll need more amps: for that voltage decreases and you won't be going as fast up a hill like on flat ground.
```

---
## \#3 Posted by: Hannes Posted at: 2018-05-30T18:31:36.293Z Reads: 98

```
Okay, so the only time i will notice it is struggling is on a steep hill, is there a drastic drop or will it be more of a "experienced users" will notice the difference?

There are some hills or "larger bumps" but nothing like san fran or anything like that.
```

---
## \#4 Posted by: BoostedBuilder Posted at: 2018-05-30T18:32:48.980Z Reads: 92

```
Depends on the hill. If it's like 3%-4%, you'll most likely not notice much of a difference. If it's a steep hill, you could be going twice slower, or possibly even come to a stop.

With a single motor, you should be fine. But at some point, you might want more power.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-05-30T18:34:10.197Z Reads: 86

```
you should know that your range and battery life suffers the more you push them to the limit.
```

---
## \#6 Posted by: Hannes Posted at: 2018-05-30T18:35:13.147Z Reads: 83

```
okay, If i go with their [10s3p](https://eskating.eu/product/flat-10s3p-eskating-electric-skateboard-battery-samsung-30q/) instead will that give me a "33% better battery" and thus giving the skateboard more breathing room? is it more recommended? will i regret going 2p?
```

---
## \#7 Posted by: BoostedBuilder Posted at: 2018-05-30T18:37:47.877Z Reads: 78

```
Not a better battery, just more power as well as a bigger range. You'll have 60a instead of 40a, so if you're planning on riding a lot of hills, that would be a better choice. You'll have a higher battery life, and less chance of failures. But if it's just 1 or 2 small hills and the rest is flat, 10s2p is enough for a single setup in my opinion.
```

---
## \#8 Posted by: Hannes Posted at: 2018-05-30T18:40:28.757Z Reads: 76

```
Okay, then i might just go with 10s2p and live and learn from it. If i go with the [zippy](https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c-xt90.html) instead (2pcs) will those give me the same as the pack or will they be better? thinking about the 8000mah, will they give me a higher amperage?
```

---
## \#9 Posted by: Benjamin899 Posted at: 2018-05-30T18:42:31.453Z Reads: 71

```
Here play with this, i found it to be quite accurate. http://calc.esk8.today/advanced/
```

---
## \#10 Posted by: Hannes Posted at: 2018-05-30T18:42:53.982Z Reads: 70

```
Thanks, will tinker with it :)
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-05-30T18:47:12.706Z Reads: 70

```
funny thing is, since i use the focbox with my zippy lipos they always discharge perfectly balanced, makes me wonder if should have only bought a bms for charging only
```

---
## \#12 Posted by: MoeStooge Posted at: 2018-05-30T18:48:29.417Z Reads: 66

```
First hand explanation of volt sag..    100m accel test on 8s 20ah 10c 200 available amps.  https://youtu.be/gKbogLAs_ac.                
                                                                           50m accel test 8s 10ah 10c 100 available amps. Same drive system. Batteries hit amp limit, voltage starts dropping till esc's cut out. 
Make sure your battery can keep up.with your load or you could end up like this 
poor fella.   https://youtu.be/jQcbA5fYCws
```

---
## \#13 Posted by: Hannes Posted at: 2018-05-30T18:53:21.903Z Reads: 62

```
hahah poor fella, Could you explain what happened to his board? his battery could not deliver the amperage needed?
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-05-30T18:55:47.784Z Reads: 60

```
battery converted voltage to amp and he probably hit his cutoff voltage
```

---
## \#15 Posted by: MoeStooge Posted at: 2018-05-30T18:59:55.301Z Reads: 58

```
Exactly.. when the battery could no longer deliver the 180a demand the voltage kept dropping till the esc's sensed low voltage and went into low voltage cut off. When your hauling ass up hill with your park helmet on is when it will get you. Build a good battery, no weak links in the chain.
```

---
