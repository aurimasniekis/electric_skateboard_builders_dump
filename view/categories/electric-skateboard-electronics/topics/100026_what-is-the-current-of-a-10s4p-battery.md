# What is the current of a 10s4p battery?

### Replies: 5 Views: 123

## \#1 Posted by: Waiboard Posted at: 2019-08-10T01:57:26.443Z Reads: 49

```
Hello,

I am configuring my VESC 4.20 plus from Flipsky and I have doubts about how to calculate the value of the direct and peak current that my battery can deliver?

My battery is 10s4p Samsung 25r cells
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-08-10T02:04:33.470Z Reads: 50

```
You can comfortably output 60a total, or (with a big amount of sag) push 80a total. 

I think 20a battery max per vesc is a good place to start
```

---
## \#3 Posted by: Waiboard Posted at: 2019-08-10T02:18:41.121Z Reads: 49

```
Thank you very much for answering.
I consult you, how is the calculation to know that they are approximately 60A?
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-08-10T02:39:28.741Z Reads: 42

```
![Screenshot_20190809-223538_Chrome|243x500](upload://qZ150peWBkTZiI1m6ZaKmE4czzz.jpeg) 

It's not good to use 100% of the batteries potential if you want range, and sag free miles. That's why I said 15 per cell, and then then it's going to be saggy. Imo, 10a/12.5a(per cell) / 40a/50a (vescs total. Devide by two to get the 20/25a per vesc as I said earlier)
```

---
## \#5 Posted by: Waiboard Posted at: 2019-08-10T02:41:32.582Z Reads: 40

```
Perfect, there I understood where the 60 / 80A value comes from.
Thank you!
```

---
