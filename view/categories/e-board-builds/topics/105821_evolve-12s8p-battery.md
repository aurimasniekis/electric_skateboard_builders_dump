# Evolve 12s8p battery

### Replies: 10 Views: 318

## \#1 Posted by: gaven120 Posted at: 2020-02-06T23:56:27.947Z Reads: 81

```
Hello everybody! This is my current attempt at building a 12s8p battery for the evolve Gtx skateboard using all Samsung 30q batteries. Some batteries are different colors because I had to rewear them, updates coming soon!![image|375x500](upload://4TTm03N6dAVmNyEXQFdxcnNalIz.jpeg) ![image|666x500](upload://67fYbHqrpYnvSHESG9UdHeV459.jpeg) ![image|375x500](upload://qxIHgC1Tg5IlVOARtKDkDOTwBKb.jpeg) ![image|666x500](upload://5iM0Szgqv1GFhRUKqNGTAOcSwhf.jpeg)
```

---
## \#2 Posted by: Schulerbible Posted at: 2020-02-08T08:20:48.790Z Reads: 50

```
Holy moly, I am curious to see where you put the BMS, switch, and the receiver. That's going to be pretty hard to figure out.
```

---
## \#3 Posted by: gaven120 Posted at: 2020-02-08T16:48:04.879Z Reads: 42

```
It all should fit there in the back, I still have about half an inch on top of the vescs to play with
```

---
## \#4 Posted by: taz Posted at: 2020-02-08T20:27:33.102Z Reads: 39

```
It fits easily


![20190506_082417|375x500](upload://vmavNTCWVh7IEguZdOzM3YsmEsF.jpeg) 
![20190506_082325|375x500](upload://nBjdANT1pZnHACjGvmf2wHikznJ.jpeg) ![20190508_184907|666x500](upload://nPGlZbCxoFlSDYFvgcJM1qWecja.jpeg) ![20190510_174919|666x500](upload://zjQSzmGDw6GNt9ebd2ff9nqICYf.jpeg)
```

---
## \#5 Posted by: gaven120 Posted at: 2020-02-08T21:02:42.867Z Reads: 33

```
Looks good!
```

---
## \#6 Posted by: gaven120 Posted at: 2020-02-08T21:25:55.346Z Reads: 33

```
@taz isn’t that a 10s8p?
```

---
## \#7 Posted by: taz Posted at: 2020-02-08T21:31:08.671Z Reads: 34

```
Yeap and now I feel stupid for responding without reading the thread title more carefully :roll_eyes:
```

---
## \#8 Posted by: beckw Posted at: 2020-02-09T10:56:22.792Z Reads: 33

```
I'm using the q30 as well but I had to make a copper bus bar because each of those cells can deliver 15 Amps. If you want to use the 15Amps on a 8 parallel pack you will end up with 120 Amps on the serial connection point. As I can see on your picture the wire would not handle that. I have 10s5p and I've designed the battery that it can deliver 75Amp continues current. My BMS is quite big with a Massive cooling body. My battery cable is not the silicone insulated cable it is a high gauge copper cable because the core should not get hot at all by such a high current otherwise you wasting energy.
```

---
## \#9 Posted by: gaven120 Posted at: 2020-02-09T23:17:22.251Z Reads: 31

```
@beckw will be using8awg for the battery’s mains and 12awg to each motor which should be enough to handle the amperage and voltage of the battery pack, also I am using dual fox boxes which I’ll program to a max draw of 45 amps each
```

---
## \#10 Posted by: beckw Posted at: 2020-02-12T20:09:54.123Z Reads: 16

```
Cool, If you planning to draw 90 Amps that should be fine. 

That's gonna be a beast 42V x 90Amps = 3780W x ~90% motor efficiency will give you 3.4KW motor power Wow!!!.

On my Mountain board battery I've added a 80Amps Forklifter fuse before it's connected to anything else.
```

---
