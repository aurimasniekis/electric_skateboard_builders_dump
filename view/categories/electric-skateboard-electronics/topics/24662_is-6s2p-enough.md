# Is 6s2p enough?

### Replies: 22 Views: 1703

## \#1 Posted by: darkkevind Posted at: 2017-06-05T23:36:02.906Z Reads: 191

```
Currently I'm running 2 x 3s Lipos in series to give me 22.2v, I have a single motor setup and for all intents and purposes it's fine.
However I'm just about to create a new battery with some 18650s and wanted to know, if I wired a pack of 6 cells in series x 2, would that be enough to replicate or exceed my lipo performance? Forget the MAH for now...
```

---
## \#2 Posted by: Rinzler Posted at: 2017-06-06T00:58:38.788Z Reads: 185

```
How many cells are there going to be, total? You have to say the type of 18650s you are going to use, without the internal resistance aka the amp rating of the cells no one can tell you much. I can tell you if you use less than 30 cells altogether their life will be shortened and its just not worth it, low acceleration, hot batteries.Maybe you can give some more information :smile: to work with.For now i would say absolutely not going to exceed anything, maybe in the exploding and fireworks factor :smiling_imp:
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-06T01:01:29.606Z Reads: 177

```
18650's would almost never exceed the power output of prismatic lipos. You'd need a large amount in parallel just to match it.

As for 6s2p 18650 being enough? No, I'd say even 10s2p isn't enough save for ideal environments (all flats, no wind, light rider).
```

---
## \#4 Posted by: anorak234 Posted at: 2017-06-06T07:04:44.382Z Reads: 159

```
I used 6s1p li-ion for a travel board. Is it enough to get you moving? Yes. Is it enough to *really* get you moving? No. And I weigh 140lbs
```

---
## \#5 Posted by: Namasaki Posted at: 2017-06-06T07:08:55.322Z Reads: 150

```
[quote="anorak234, post:4, topic:24662, full:true"]
I used 6s1p li-ion for a travel board. Is it enough to get you moving? Yes. Is it enough to really get you moving? No. And I weigh 140lbs
[/quote]

How bad was the voltage sag on that setup?
```

---
## \#6 Posted by: anorak234 Posted at: 2017-06-06T07:22:29.828Z Reads: 144

```
About 12%. Not the worst - I used Basen 4500mah cells (60A each)
```

---
## \#7 Posted by: rojitor Posted at: 2017-06-06T09:23:41.198Z Reads: 144

```
If you use 2p the cells must have high C rates.  20-30 amps delivery at least. You will get low power otherwise. Samsung 20r and sony konion are up for the task.
```

---
## \#8 Posted by: darkkevind Posted at: 2017-06-06T10:10:57.797Z Reads: 143

```
What about what I'm proposing though? 6s2p
```

---
## \#9 Posted by: darkkevind Posted at: 2017-06-06T10:19:33.665Z Reads: 139

```
Thanks for the replies. Sorry I'd gone to bed so couldn't reply :confused:

OK, so at the moment I have 12 cells (I think you're going to tell me to get more), so what would be the best way to set them up? Bear in mind I've ridden my board on 11.1v before and found it to be adequate in top speed. (I'm no speed demon on my board, I've already had a bad injury!) lol
```

---
## \#10 Posted by: rojitor Posted at: 2017-06-06T11:15:47.888Z Reads: 129

```
What kind of cells are you using? Brand, model... new or laptop leftovers. ..
If you use brand new high C cells you are safe on 2p on an normal use.
Bad quality cells or full throttle rides will generate way too much heat and damage the cells. They will not last a month. Depends on your riding style and the cells specs. 3p will always be a better choice if you have that option.
```

---
## \#11 Posted by: Jammeslu Posted at: 2017-06-06T11:32:57.053Z Reads: 121

```
You can do like Boosted with a 6s2p A123 cells, but they are expensive tho but Will work great
```

---
## \#12 Posted by: darkkevind Posted at: 2017-06-06T12:08:26.961Z Reads: 114

```
CHRIST! They're expensive! :confused:
```

---
## \#13 Posted by: darkkevind Posted at: 2017-06-06T12:09:03.027Z Reads: 117

```
What about 4s3p?
```

---
## \#14 Posted by: Namasaki Posted at: 2017-06-06T12:39:52.388Z Reads: 118

```
[quote="darkkevind, post:13, topic:24662, full:true"]
What about 4s3p?
[/quote]

Increasing P will not help if you have to decrease voltage to do it. 
If you go with Li-ions, go big or don't go. 
You'll be better off sticking with Lipos than with an inferior Li-ion pack.
```

---
## \#15 Posted by: 2-alex-2 Posted at: 2017-06-06T13:19:41.821Z Reads: 112

```
I run a 6s4p with little voltage sag and getting 12 miles out of a charged. Upswing lghg2 cells.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-06-06T14:02:09.812Z Reads: 108

```
Thanks @Namasaki, I think I'll go big then! :slight_smile:
```

---
## \#17 Posted by: eldars Posted at: 2017-06-06T14:07:16.621Z Reads: 106

```
6s2p is not enough for sure. I tried both 6s2p and 6s4p on 1 and 2 motor setups. My favorite in terms of range so far is 6s4p with 1 motor setup. It gives me up to 24km of range with rather light 6kg board. My regular commute is about 14km (7km one way), but 6s2p gives a range below that.

However I am thinking about 6s6p, or 8s4p as the next thing to try. More range and more power is always better.
```

---
## \#18 Posted by: eldars Posted at: 2017-06-06T14:12:45.518Z Reads: 102

```
4s3p is not a good idea, since most of the brushless motors need at least 22V, while 4s will give you only 14V.

I used 24 Panasonic NCR18650 3.7V 3400mAh cells to make my own battery pack, but I am still not sure, if that was a better option compared to just buying four 3S ready made batteries.
```

---
## \#19 Posted by: darkkevind Posted at: 2017-06-21T09:35:04.566Z Reads: 86

```
I have a relatively noob battery question. If I'm making up a Li-ion pack and for example I go 6s4p with cells that can output 15A, does that make each parallel pack a 90A pack?

And on that note, if each cell is 2500mah, does that make each parallel pack 15000mah?

So that would basically end up to be a 22.2v 15000mah 90A pack (6s4p)?
```

---
## \#20 Posted by: TarzanHBK Posted at: 2017-06-21T09:40:17.480Z Reads: 84

```
No.
6S = 6 x 3,6V = 21,6V
4P = 4 x 2500maH = 10.000maH and 4 x 15A = 60A
```

---
## \#21 Posted by: darkkevind Posted at: 2017-06-21T09:57:24.911Z Reads: 82

```
Ahh so it's the parallel that determines the mah and A rating?

Aren't most Li-ion batteries 3.7v nominal? So 22.2v...
```

---
## \#22 Posted by: TarzanHBK Posted at: 2017-06-21T10:30:50.376Z Reads: 78

```
depends on the chemistry of the cell, but you could take 22,2V aswell for 6s.
```

---
