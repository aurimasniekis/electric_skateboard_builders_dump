# Went from unsensored to sensored motors and now it&rsquo;s way less powerful

### Replies: 20 Views: 530

## \#1 Posted by: Celt Posted at: 2019-03-29T21:59:08.675Z Reads: 217

```
Hey guys!

I've got dual Torque Board's 6355's, Focbox Unity and a 12S4P battery.

I just sensored my 6355's and I noticed that I have way less power. I use to use 58 amps and it felt plenty fast and now at that it's just lethargic. What's going on?

I tried bumping it up to 70 amps and once I get going it's decent but off the line it's so slow, it's ridiculous. Also I'm running 60 battery amps, -10 on regen and -60 for motor amps. Also I'm confused on how to know what the maxes can be for my battery and motors?

Thanks so much!
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-03-29T22:01:18.148Z Reads: 213

```
Motor 
 specs:https:///collections/electric-skateboard-motors/products/electric-skateboard-motor-6355-190kv \
To calculate your max battery discharge we need a bit more information. :slight_smile:
```

---
## \#3 Posted by: Eboosted Posted at: 2019-03-30T02:41:31.805Z Reads: 182

```
Are you runing hybrid mode? That's the setting you need to select
```

---
## \#4 Posted by: Celt Posted at: 2019-03-30T04:48:17.058Z Reads: 172

```
I'm just using whatever the stock setting of the unity is.
```

---
## \#5 Posted by: Celt Posted at: 2019-03-30T05:11:13.603Z Reads: 162

```
Are you saying that's just the way sensored FOC feels?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-03-30T05:53:44.960Z Reads: 152

```
Yeah I had the same issue lol, try 80a, 

Unsensored raptor hubs can throw me off my board at foc but sensored can not...
```

---
## \#7 Posted by: Celt Posted at: 2019-03-30T06:03:56.007Z Reads: 146

```
I set it at 70a already lol...i don't understand whats going on to make it need so much more juice. 

That's so strange!  Almost makes me want to run unsensored.  On the plus side everything and feels really smooth.
```

---
## \#8 Posted by: Dirt_Bag Posted at: 2019-03-30T06:17:17.498Z Reads: 140

```
Correct me if im wrong, but one of the main advantages of sensorsed mode is to provide rpm data allowing the esc to apply power more gently under load.
```

---
## \#9 Posted by: b264 Posted at: 2019-03-30T07:04:06.633Z Reads: 134

```
Sensored mode is most useful for starting from a stop -- or starting if you're rolling backwards.  Once the motors are turning, it makes little difference.
```

---
## \#10 Posted by: goldrabe Posted at: 2019-03-30T08:09:37.131Z Reads: 114

```
Did you noticed a difference in old and new Unity firmware? 
Somehow I feel like the latest firmware isn't as torquey as the old firmware, but haven't looked into the acceleration curves.
```

---
## \#11 Posted by: Bjork3n Posted at: 2019-03-30T08:23:48.397Z Reads: 110

```
I've also noticed this on my new build. 
Running Foc sensored with dual 6374 and my previous build was bldc uncensored dual 6355. 
The old build felt more like a wild beast compared to the new one.
```

---
## \#12 Posted by: Gamer43 Posted at: 2019-03-30T09:02:40.780Z Reads: 104

```
Try lowering the sensored RPM. The speed estimator on the VESC kinda sucks tbh, sensors are only useful if the motor cannot synchronize to open loop commutation, which normally happens with hill starts and high inertia loads.
```

---
## \#13 Posted by: Celt Posted at: 2019-03-30T11:16:49.769Z Reads: 91

```
Nope never noticed a difference. Literally just after installing the sensors.
```

---
## \#14 Posted by: Celt Posted at: 2019-03-30T11:20:36.048Z Reads: 91

```
That's not been my experience so far. I had Carl Collins help me with my remote disconnect issues and one of the things we did was the test erpm in the unity app. Maybe that could have done something?
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-03-30T12:42:28.423Z Reads: 84

```
Yeah once I get past 10-15mph I really feel the power kick in, but Durning startup it's not fun, might set my unsensored erpm to 500
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-03-30T12:42:53.965Z Reads: 83

```
My two unitys is actually getting delivered today 🤣
```

---
## \#17 Posted by: Bjork3n Posted at: 2019-03-30T16:02:34.137Z Reads: 62

```
Let us know if it's a improvement :slight_smile:
```

---
## \#18 Posted by: AlanZhou Posted at: 2019-03-30T23:55:01.973Z Reads: 49

```
Yeah too bad I have no battery packs that are working... And my next build is 13s10p so can't test it on that....
```

---
## \#19 Posted by: Sn4pz Posted at: 2019-03-31T02:13:59.194Z Reads: 47

```
you better go ballistic with safety materials... thats alot of lithium to go up in flames o.O
```

---
## \#20 Posted by: AlanZhou Posted at: 2019-03-31T04:28:42.829Z Reads: 34

```
get a better soldering iron :rofl::wink:

the focbox bullet's that you soldered was cold

i finally got around to undersolder the bullets.
```

---
