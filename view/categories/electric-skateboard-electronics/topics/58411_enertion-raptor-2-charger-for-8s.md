# Enertion raptor 2 charger for 8s

### Replies: 4 Views: 196

## \#1 Posted by: petter Posted at: 2018-06-10T11:54:10.874Z Reads: 63

```
So a pillar of smoke is slowly rising from my lab power supply. I was using it to charge my board while waiting for the proper charger. First it was OK, using a single channel for 33v for a few hours. Though since that is a bit low and the bms wont balance until 4.2v i seriesd up the two channels and boosted it to 34v, and that took about ten minutes until the psu cut out and started making chunky sounds.

I always suspected that it was bad quality even though it was expensive..

So now i dont have any more sources that will give 33+v, except for the raptor charger... Tho i really don't want to fry that one too so i'm wondering if it can handle the lower voltage of 8S? How is the CC circuit designed?
```

---
## \#2 Posted by: petter Posted at: 2018-06-10T12:45:52.042Z Reads: 54

```
![1528634508715-593643911|666x500](upload://er7HZaWRq3nxKNi871ZksPwGUpD.jpg)
Okay, so i kind of found a solution, i had a boost converter half suited for the job. 

It would still be nice to know if i could use the enertion charger though!
```

---
## \#3 Posted by: deucesdown Posted at: 2018-06-10T13:41:51.399Z Reads: 44

```
Raptor is 10s. The answer is no. You'll cook your bms or your pack. It's theoretically possible to use the charger and pull the plug when it hits 33.6v, but that is waaaay dangerous. 

You can also use a buck converter similar to your boost. But it'll be a pain and will cost as much as a charger.
```

---
## \#4 Posted by: petter Posted at: 2018-06-10T14:02:59.663Z Reads: 36

```
Yeah, im just waiting for the charger to arrive, it's nearly three weeks since i ordered..

And i won't Cook the bms, since it's made for protecting against overcharging :slight_smile: 

But i agree, it's not a good long term solution. I already know all this, i just want to know if the raptor charger can handle it or if it would overheat from a too big voltage drop
```

---
