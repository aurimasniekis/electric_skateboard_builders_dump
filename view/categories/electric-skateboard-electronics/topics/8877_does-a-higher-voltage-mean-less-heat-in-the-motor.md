# Does a higher voltage mean less heat in the motor?

### Replies: 10 Views: 1503

## \#1 Posted by: evoheyax Posted at: 2016-09-04T03:20:40.580Z Reads: 146

```
Pretty straight forward. My intuition says no, but I figured it would be best to ask the experts.

Besides the straight science behind it, I'm curious as to would it lower heat if you consider the fact I can climb hills quicker at higher voltages?

If I climb a hill slowly, I pull more amps than if I plow up the hill (due to momentum), so by this logic, shouldn't a higher voltage system mean I need less energy to climb a hill since I can keep my momentum up, which would mean less motor heat?

Any thoughts are appreciated.
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-09-04T03:24:57.326Z Reads: 142

```
Having a higher voltage means you draw fewer amps. It's Ohm's law! You can also calculate how much heat you will generate based on the wattage and such.
```

---
## \#3 Posted by: Jinra Posted at: 2016-09-04T03:29:13.148Z Reads: 140

```
higher voltage generally means lower heat due to needing less current for the same amount of wattage. A higher voltage system can go faster to allow forward momentum to assist in climbing and will draw fewer amps (less heat) vs a low voltage setup. 

Heat always means energy lost, which is why long distance power lines run in kilovolts, minimizing heat and increasing efficiency.
```

---
## \#4 Posted by: evoheyax Posted at: 2016-09-04T03:38:38.494Z Reads: 133

```
I know it means less amps to the esc, which will mean the esc will run cooler. But there was a debate a while ago as to whether or not it means the motor see's less energy, seeing as your not changing the amount of work that the motor needs to do (except somewhat on hills). There was one guy a while ago that did 6s vs 12s, and he seemed to insinuate that they both heat the motor the same, but the esc got hotter on 6s as it pulls more amps. I'm trying to understand if it just means the vesc runs cooler or if the motors will also.
```

---
## \#5 Posted by: Jinra Posted at: 2016-09-04T03:41:21.954Z Reads: 126

```
Not sure on that, though @hummie rides 12s dual hubs and his VESCs were very cool after our 8ish mile session.

I'd assume the motor would run cooler too, but have no proof of that.
```

---
## \#6 Posted by: michaeld33 Posted at: 2016-09-04T03:47:16.199Z Reads: 118

```
+1
I believe that since less current passes thru, less heat is generated. (That doesn't mean go 20S and single drive hub motor, but it does help if it's 10S vs 6S)
```

---
## \#7 Posted by: evoheyax Posted at: 2016-09-04T03:47:21.573Z Reads: 118

```
@hummie seemed to think that running 12s instead of 10s will heat the motors just as much. I'm waiting on ceramic bearings, as from what I was reading, they don't absorb heat nor create much heat since there's far less friction. I can ride 4 miles with  being the hottest I get, but the last mile runs away to 230 F+. I hope the ceramics help, as the only issue the motors have at these temps are the bearings are starting to seize and the lubricate is drying out. But ideally, I would like to reduce heat in the motors. So if 12s means less heat in the motor, that would be great.
```

---
## \#8 Posted by: Jinra Posted at: 2016-09-04T03:49:07.660Z Reads: 107

```
I'm curious to know the results, please post the results when you get it!
```

---
## \#9 Posted by: michaeld33 Posted at: 2016-09-04T03:49:21.625Z Reads: 114

```
I don't think they heat impact difference will really be that different. Maybe on the speed controller and such, but I just don't think the 10 vs 12 cell will decrease the heat significantly. I agree with hummie. But I may be wrong, I would be interested to see the results aswell.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-09-04T05:39:46.374Z Reads: 94

```
I'm tempted to buy 8 more cells, make a 2s4p to temporarily attach to the 10s4p. I want to try 12s and see how it hot it gets. My problem is right now, I'm at 420 Wh with my 10s4p. 40 cells is about the limit I can do, so a 12s4p is not possible. A 12s3p (36 cells) would reduce me be 375 Wh, which makes me worry about my range. At 10s3p, I hit my LVC in the last 4th of a mile of my route of 5 miles with 2wd.  But having gone to 4wd, I feel like I'm getting way better efficiency. I can get 8-9 miles with 10s4p without even hitting LVC. I would like to do an efficiency test at some point and see how they really compare. But part of the problem is the efficency is likely linked to the amount of heat and how quickly I build it on 2wd. I can do 3 miles of mostly uphills without breaking 150 F. I want to find a way to keep them there though. I hope the ceramic bearings have a positive effect. They should come in a about 2 weeks.
```

---
