# Series or Parallel? Battery

### Replies: 17 Views: 3157

## \#1 Posted by: NewbieBoardBuilder Posted at: 2016-11-21T20:06:03.822Z Reads: 261

```
I know this is a beginner question, but it will help others in the future... Is it better to arrange your battery  in a series or parallel circuit, and why or why not?
```

---
## \#2 Posted by: Fiori Posted at: 2016-11-21T20:10:57.408Z Reads: 260

```
Parallel is going to give you more range, whilst Series is going to up your Voltage(essentially more power). It's a little more complicated than that, but that's the basic gist. 

You're going to want to read up on some of the stickies on  batterys posted around here. There is tons of information on this forum alone.
```

---
## \#3 Posted by: LukeL Posted at: 2016-11-21T21:02:43.457Z Reads: 242

```
You don't really choose between series or parallel 
 
Decide what voltage and capacity you want your battery to be then wire it in the configuration needed, whether that be series, parallel or both.

wiring two of the same batteries in series gives double the voltage, in parallel gives double the capacity.
```

---
## \#4 Posted by: NewbieBoardBuilder Posted at: 2016-11-21T22:37:06.254Z Reads: 218

```
What is more common? 
Like the Enertion cell and the boosted?
```

---
## \#5 Posted by: Esrapp21 Posted at: 2016-11-21T22:40:05.725Z Reads: 207

```
Series is double the speed because it is double the voltage, but the same amps. Parallel and series will go the same range assuming you are on full throttle in the same conditions, but if you're not going full throttle the whole time, Parallel has a longer range. Series is more common.
```

---
## \#6 Posted by: NewbieBoardBuilder Posted at: 2016-11-22T01:53:40.440Z Reads: 188

```
[quote="Fiori, post:2, topic:13422"]
Parallel is going to give you more range, whilst Series is going to up your Voltage
[/quote]

What is more common?
What is the boosted board and space cell?
AND WHY
```

---
## \#7 Posted by: anorak234 Posted at: 2016-11-22T05:02:23.934Z Reads: 170

```
Parallel won't necessarily give you more range, sometimes it's about efficiency. 6s 10000mah lion battery will give you 10 miles of range, whereas a 12s 5000mah lion battery will give you 12-15. Point is parallel increases mah whereas series increases voltage. Series is more common. 10s4p is the space cell and I believe 12s2p is the boosted battery.
```

---
## \#8 Posted by: lox897 Posted at: 2016-11-22T11:15:50.399Z Reads: 155

```
More in series is more common because we need a higher voltage for our boards. Enertion is 10s3p 60amp continuous and boosted is 12s1p 70amp continuous because they use A123 cells. As others have said though, it is suited to your needs, there isn't a standard configuration. But I'd say currently 10S is the most common and probably 3-4p.
```

---
## \#9 Posted by: XplodingLarsen Posted at: 2017-06-15T19:30:50.401Z Reads: 117

```
for anyone who is totally noob on this. here is a bad analogy.

series is like the engine of a car and parallel is the fuel tank. you probably want the biggest of both, but your physical size will determine how big you can go.

series gives Voltage (horsepower) and parallel gives you mAh (fuel tank capacity)
```

---
## \#10 Posted by: benhemingway Posted at: 2017-12-01T23:04:09.337Z Reads: 91

```
Would it be possible to have a motor act as a generator to charge one battery, and then have a second motor draw power from a second battery? Once the first battery got down to say 20% the system would switch and begin drawing from the second battery and charging the first?
```

---
## \#11 Posted by: wafflejock Posted at: 2017-12-01T23:15:01.779Z Reads: 88

```
This would require more than 100% efficiency it's called over-unity and no it doesn't work.  You could do this for a while but only until you bleed off all the energy in the form of heat (vibrating molecules), sound (vibrating air), and moving air around the motors.  Most of us use regenerative braking which does use the motor as a generator to put charge back into the battery but this only gives back some of the energy you put into getting moving since some if is lost in heat in the wires and drag (moving air) etc.

Just watched this earlier and is releavnt:

https://www.youtube.com/watch?v=-suxSqrP_X4

https://www.youtube.com/watch?v=06xFhUHFnx8
```

---
## \#12 Posted by: Proxy Posted at: 2017-12-03T05:03:39.397Z Reads: 72

```
Can i wire 2 3s 5000 mah battery in serials to give me 6s 5000 mah and then a 3rd one in paralle to give me 6s 10000mah? Or will my shit blow up?
```

---
## \#13 Posted by: E1Allen Posted at: 2017-12-03T06:39:31.195Z Reads: 65

```
No. U need four batteries.
```

---
## \#14 Posted by: Fatos Posted at: 2017-12-03T10:33:40.715Z Reads: 64

```
It won't blow up. But you will end up damaging the first cell pretty fast. In that case you should only buy 2 of them and have them series. Or 4 of them with 2 in series and 2 parallel.
```

---
## \#15 Posted by: LukeL Posted at: 2017-12-03T13:50:39.774Z Reads: 61

```
Like others have said this is not a good idea you will damage the cells

You would effectively have wired a 3S 5000mah battery in series with a 3S 10000mah battery

this isn't 6S 10000mah, the smaller one would discharge a lot quicker

as it discharged the voltage would probably drop to 3S and the cells would get damaged
```

---
## \#16 Posted by: achatham Posted at: 2018-06-04T19:44:47.512Z Reads: 44

```
I'm interested to dig a little deeper into the numbers. I understand what series and parallel mean, I get mah is essentially the container size of the battery and voltage is the pressure, but help me understand the numbers and what it means if you have a 10s4p vs a 10s3p.  One thing I have read is that higher parallel = less voltage sag.

I get its 10 cells with 4 parallel and 3 parallel, but how does this effect the actually ride distance, speed, etc? I'm running lipo's at the moment and have @eboosted building me a 10s4p, but what to understand it.
```

---
## \#17 Posted by: Brontech Posted at: 2018-06-04T21:02:14.359Z Reads: 39

```
Here's my 2 cents..
So for the sake of this demonstration, lets say that the lithuum ion cells you are using are 3000Mah.
Every P you add to a 10s battery pack, it will gain 3000Mah in this scenario.

So, if you have 10s3p, you will have a total capacity of 9000Mah, factoring out other losses like charge cycles and stuff...

With 10s4p, you will have a total capacity of 12000Mah, which will give you about a 25% increase with range and will also reduce voltage sag, which may give you a very slightly higher top speed because of the slightly raised voltage.
```

---
