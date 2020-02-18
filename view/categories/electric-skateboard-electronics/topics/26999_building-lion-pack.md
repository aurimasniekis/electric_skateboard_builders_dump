# Building lion pack

### Replies: 17 Views: 976

## \#1 Posted by: twan Posted at: 2017-07-07T18:41:28.698Z Reads: 129

```

What do you guys think? I'm trying to build 10s battery pack with Samsung 18650 30q running 10 in series and 2 sets to make 10s2p they are at 3000mah so I'll get a 6000mah pack @ 10s . Is the discharge current too low? Think they are rated at 20c

10s2p enough for my single drive 6374 motor? With 15/40 gearing on 97mm wheels
```

---
## \#2 Posted by: abenny Posted at: 2017-07-07T18:47:09.633Z Reads: 127

```
20c is about the minimum recommended discharge rate for esk8 i believe.
you may want more packs in parallel to prevent voltage sag and elongate battery life.
Also, if your 6374 is ~190kv , i think that 10s is about optimal for that motor.
```

---
## \#3 Posted by: Okami Posted at: 2017-07-07T18:48:48.306Z Reads: 125

```
Do you also have hills? You should have about 30-40A max discharge.. 25A (for safer figure) X 36 = ~900W

I would say enough for flats but if you wanna race hard and go maybe over 25-30mph or something, then more packs in parallel might be welcome (everyone else will probably say you the same thing here)
```

---
## \#4 Posted by: twan Posted at: 2017-07-07T19:06:34.232Z Reads: 111

```
Thank you for the insights!!

How do I know many packS in parallel to put? It's there a way to calculate the max current output ? Or its always going to stay 15c since the battery are rated that way
```

---
## \#5 Posted by: mmaner Posted at: 2017-07-07T19:08:46.344Z Reads: 109

```
I wun a 10s3p with 30q's on a 40in deck with 6x2 AT wheels and it screams.  I would guess 10s2p with 30q's would be discharge (AMP delivery) pretty well, at least as good as a 10s3p with 25r's, but I would suggest at least a 3p pack.
```

---
## \#6 Posted by: Jinra Posted at: 2017-07-07T19:11:08.650Z Reads: 106

```
30Q's dont have anywhere near 15/20C discharge. That's 60 amps. They have a 15A continuous rating, but people have been fine using 20A. I'd recommend at least 4 in parallel.
```

---
## \#7 Posted by: twan Posted at: 2017-07-07T19:19:48.515Z Reads: 107

```
I'm kinda dumb but so I know putting packs in parallel will increase the amp hours and not the voltage. So does that mean it will also increase the output current ( the C rating)  and make it stronger?
```

---
## \#8 Posted by: smurf Posted at: 2017-07-07T19:22:42.964Z Reads: 107

```
If you have to use a 2 parallel battery because of space constraints. I recommend the Sony 18650 VTC4  that will at least give you 60a of power.

https://liionwholesale.com/collections/batteries/products/sony-18650-vtc4-battery-genuine-tested-30a-2100mah-flat-top-wholesale?variant=1038136780
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-07T19:34:11.309Z Reads: 104

```
C ratings are a constant and never change for a cell. When you put more cells in parallel you're directly increasing the output potential (in amps) of the pack. Doesn't mean the output current will be that value, just that it has the potential to be at that value.
```

---
## \#10 Posted by: pjotr47 Posted at: 2017-07-07T19:54:26.096Z Reads: 97

```
60a? Read this message: https://www.e-cigarette-forum.com/forum/threads/sony-vtc4-2100mah-18650-bench-test-results-a-20a-cell-that-can-be-used-to-30a.684876/
```

---
## \#11 Posted by: twan Posted at: 2017-07-07T20:02:36.612Z Reads: 92

```
Ahhh I get it , so I general electric sk8 needs above 40C from what I heard and to get that lets say my q30 gives 15c so I should make at least 3 pack in parallel which will give me 15x3 about 45c which will reduce voltage sag and give good power output.
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-07T20:32:09.618Z Reads: 90

```
You're still not using the term C rating correctly. C rating x amp hours is the discharge rating. There's no "Minimum C rating" for esk8
```

---
## \#13 Posted by: thisguyhere Posted at: 2017-07-07T20:45:46.758Z Reads: 90

```
just ditch the C rating concept for a second.

the continuous discharge and capacity of an individual cell is multiplied across the parallel pack.

your 30q cell has 15amp continuous discharge and 3000mah capacity.

in your proposed 10s2p pack, the continuous discharge and capacity will be 30amps and 6000mah.

so...30amp is the continuous discharge rate of your 10s2p pack.

i think most would agree that 30amps is a bit low for an esk8, as your motor(s) will easily exceed that during acceleration or goin uphill or both.

if you draw more current out of your cells than what they're intended, they will for sure heat up and heat will eventually kill your cells prematurely or worst blow up.

so then, if you add an additional cell to your parallel pack, your continuous discharge will go up to 45amp and total capacity to 9000mah.
```

---
## \#14 Posted by: twan Posted at: 2017-07-07T20:51:04.766Z Reads: 80

```
Ohh understood. Thank you so much for the clarification was a bit confused.  😊😊🙏🏽🙏🏽 40-60 amps would be ideal then?
```

---
## \#15 Posted by: thisguyhere Posted at: 2017-07-07T20:53:34.360Z Reads: 83

```
more the better, but i would say 45amp minimum for the very basic vanilla build.

but it all depends on what you're planning, your weight, types of roads, whether you're hitting hills, etc.
```

---
## \#16 Posted by: sl33py Posted at: 2017-07-07T22:13:29.110Z Reads: 76

```
@thisguyhere

THIS!

Unless you know your actual consumption of current when riding (coulometer or similar data of real-world-use for YOU and where you ride) - i'd suggest building more towards the 60A *MINIMUM*.  If you don't, i think you'll have a short lifespan of those cells.  A lot of heat as well, and heat is just energy (range) wasted.

Maybe work backwards from your weight, single/dual motor, hills, and range wanted?
```

---
## \#17 Posted by: rojitor Posted at: 2017-07-07T22:33:36.241Z Reads: 67

```
I have a 2p pack done with Konions.  Works like a charm. I tested the heat after rough rides. It is ok. If you use low amp cells they overheat quick and makes 2p unviable. 3-4p is always better. So you use top rated cells or make more parallel.

[https://ru.nkon.nl/sony-us18650vtc6.html](https://ru.nkon.nl/sony-us18650vtc6.html)
```

---
