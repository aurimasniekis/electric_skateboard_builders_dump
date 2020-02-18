# How much voltage sag is to much?

### Replies: 15 Views: 287

## \#1 Posted by: ZachTetra Posted at: 2019-04-11T15:48:28.186Z Reads: 121

```
I'm using a 10s2p of Littokita 30Q cells and in theory I get 216Wh out of them (3.6V * 3Ah * 20) but according to the power meter online with the ESC I'm getting about 140Wh before the battery drops below 30V while pulling 5A to 10A (17mph on flat ground) but if I let it sit for a minute the battery goes back up to 35V

Is this reasonable behavior for knockoff cells or is my battery already fucked?  It's only at like 15 cycles or something like that

The max power the motors draw is 19A uphill on startup so even these cells should handle it fine, I can't imagine they suffered any damage since they have always been at good voltage and we're never abused

Im getting 16Wh/mi with aggressive acceleration/hills to 8Wh/mi with light cruising on flat ground so I'm still getting 15 good miles before it dies but I should be able to go way father in theory
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-04-11T15:54:24.139Z Reads: 119

```
Im late to the party, are the littokita 30qs  genuine samsung 30qs?
```

---
## \#3 Posted by: olestra Posted at: 2019-04-11T15:54:29.317Z Reads: 118

```
my guideline for various electronic projects is voltage sage on critical systems be no more than 10% of total voltage.

since a 10s pack is basicaly a 36v system, I would suggest no more than 3.6v drop under max load
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-04-11T15:56:36.169Z Reads: 110

```
I've hit 6V sag after only a couple minutes at 2/3 of the continuous rated amp draw
```

---
## \#5 Posted by: ZachTetra Posted at: 2019-04-11T15:57:12.548Z Reads: 107

```
No, same capacity but significantly more internal resistance
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-04-11T15:59:35.496Z Reads: 104

```
I mean, its an unfortunate amount of voltage sag but if the pack isnt giving any alarming signs then I think its just normal for the cell :thinking:
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-04-11T16:03:37.070Z Reads: 99

```
As long as it isn't dangerous then I guess I can live with it...65% of the expected energy isn't ideal but it's acceptable if there isn't a significant risk of a fire from damaged cells
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-11T16:52:48.321Z Reads: 91

```
Litokala has been know to sell b grade cells

6v sag is insane.. also some 18650s like the 30q can be discharged to 2.5v that's the only way you'll get full capacity out of them
```

---
## \#9 Posted by: Hummie Posted at: 2019-04-11T16:59:07.962Z Reads: 89

```
If ur only doing 10a those cells should have a lot more capacity.   Like full capacity 3ah.  And when u let it sit after even that minor discharge and pops back up is bad sign
```

---
## \#10 Posted by: thisguyhere Posted at: 2019-04-11T17:01:49.819Z Reads: 88

```
if you're pulling like 0.2c on these fake cells, yes you get rated capacity.

but they sag like crazy and generally have fluctuating IR.

https://www.youtube.com/watch?v=q2o3Wc-0fVk

https://www.youtube.com/watch?v=1GcDK0bLLyA

i think you should just be happy with the range you're getting now and not having it go up in flames (so far).

sag at 20a should be 0.5v, so 1v for your 2p pack:

![image|592x366](upload://s4gLply7Bfym7rI8WTofECwAnn6.png)
```

---
## \#11 Posted by: ZachTetra Posted at: 2019-04-11T17:05:42.837Z Reads: 80

```
But it doesn't have enough voltage for any speed
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-04-11T17:06:03.888Z Reads: 78

```
Yes but that's how they rate the cells

My 13s 10p pack can prolly discharge to 2.5v cause of the 10p
```

---
## \#13 Posted by: Hummie Posted at: 2019-04-11T17:09:59.359Z Reads: 78

```
20a an hour n half😃
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-04-11T17:10:21.841Z Reads: 79

```
Yep 10a, it will take 3 hours to charge

So itll basically be like charging a 10ah pack in 1 hour.
```

---
## \#15 Posted by: AlanZhou Posted at: 2019-04-11T17:11:53.017Z Reads: 79

```
I'm not bringing a 20a charger to a group ride, heck Insted I would bring a 30a charger and it would only take one hour

To charge a 30ah pack. 🤣
```

---
