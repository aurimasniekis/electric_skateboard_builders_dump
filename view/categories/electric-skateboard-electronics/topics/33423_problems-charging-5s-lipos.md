# Problems charging 5s lipos

### Replies: 6 Views: 245

## \#1 Posted by: Mikkiller Posted at: 2017-09-18T17:51:45.549Z Reads: 59

```
I am about to complete my esk8 and I wanted to charge my batteries, which I had put in storage mode. When I charged them in storage mode I used 1 Amp because I thought it was probably safer (don't know why) and it all went well. Now I wanted to charge my batteries and I wanted them charged fast, so I selected BALANCE CHARGE in my IMAX-B6, I selected 5S and 5A and started charging. This is what happened:

https://www.youtube.com/watch?v=cV03tPCRbcg&feature=youtu.be

I trued using the normal charge mode and the result is the same. It just restarts as soon as it hits 1.5A. Is it possible that I haven't soldered the batteries correctly? Otherwise, what could be the problem?
```

---
## \#2 Posted by: marsrover001 Posted at: 2017-09-18T18:41:54.899Z Reads: 50

```
Your power supply to the charger is tripping. Resetting the charger in the process. Either charge slower or get a bigger power supply.
```

---
## \#3 Posted by: SORRENTINO Posted at: 2017-09-18T18:47:32.935Z Reads: 46

```
Imax is also a 50w charger so max you can charge is about 2.7amp at nominal voltage. Its either your psu tripping or the charger resetting because it exceeds the max limit of the charger.
```

---
## \#4 Posted by: Mikkiller Posted at: 2017-09-18T20:11:49.141Z Reads: 37

```
that is a reasonable explanation. I just found a random 12V power supply at home and thought it would be alright. I will look for a better one :)
```

---
## \#5 Posted by: Mikkiller Posted at: 2017-09-18T20:13:43.270Z Reads: 34

```
By the way, can I use just one battery at storage charge to program the vesc or should I use them charged fully? I don't have other power supplies to use
```

---
## \#6 Posted by: Boardnamics Posted at: 2017-09-18T22:27:06.166Z Reads: 24

```
If you're powering it with 12v, make sure it is rated to at least 5A. Anything less and it won't have the watts needed and will restart like so. Also, charge in Balance mode not charge. Balance makes sure to keep all the cells at the same voltage.
```

---
