# Connecting Battery to VESC

### Replies: 9 Views: 1286

## \#1 Posted by: cicero Posted at: 2016-11-13T21:04:21.346Z Reads: 160

```
This is a first time build and I am going to buy the VESC from here https://electric-skateboard.market/product/meb-vesc/ and 2 5000mah 3s batteries https://hobbyking.com/en_us/zippy-5000mah-3s1p-20c-hardcase-pack.html 
I just wanted to know how would i connect these batteries in series and then to the VESC? What connectors will I need?
Any helps appreciated, Thanks
```

---
## \#2 Posted by: yaca Posted at: 2016-11-13T21:28:33.386Z Reads: 152

```
Batteries in series: for example

<img src="/uploads/db1493/original/3X/b/b/bba2c13c0bdcc52ee0fcaa5541106b385ab99b12.png" width="625" height="500">

I use XT 60 to connect the batt to the vesc. Be careful with sparks so you should use an antispark loopkey or a antispark switch. It's easy to find this in this forum.
```

---
## \#3 Posted by: cicero Posted at: 2016-11-13T21:35:57.588Z Reads: 134

```
So i could connect the bullet connectors to the xt 60? I am planning on buying an easy off/on switch with anti-spark
```

---
## \#4 Posted by: yaca Posted at: 2016-11-13T21:38:52.118Z Reads: 132

```
you have to solder the wires to the xt 60. Female for batt and male for vesc.
```

---
## \#5 Posted by: Esrapp21 Posted at: 2016-11-13T22:04:48.136Z Reads: 124

```
There are some series connectors with 4mm bullet connectors, but for your check your VESC to see the power connector. If it requires XT60, do what @yaca said. If you don't have access to a soldering iron, they sell 4mm bullet to XT60 adapters at most hardware stores and online.
```

---
## \#6 Posted by: cicero Posted at: 2016-11-13T22:16:09.487Z Reads: 123

```
Ah okay I see thank you guys @Esrapp21 and @yaca
```

---
## \#7 Posted by: omitchell11 Posted at: 2018-11-07T17:47:26.479Z Reads: 29

```
I bought the same battery’s and vescs for a dual motor set up I’m making for a school project I was wondering if you could help out because I’m not 100% sure how to set this up on the BLDC seems like someonething isn’t working and I can’t figure out what it is.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-11-07T20:29:33.907Z Reads: 26

```
Can you post some pictures?
What you already set up and how?
Maybe you made some diagrams after which you wired everything up. That you could post too.
Would help a lot to find out what’s wrong on your project
```

---
## \#9 Posted by: omitchell11 Posted at: 2018-11-07T20:48:57.191Z Reads: 25

```
![image|375x500](upload://qCZTbOVT1D6BJUYNhUQNpwJSMjk.jpeg) I have the battery’s attaches to a series connector then to both VESCs which are parallel then the motors are attached to the vesc with a adapter to take it from 4 mm bullet to a 5.5 mm bullet. The VESCs are attached using a can bus connection and the remote receiver is attached using a male to male servo plug
```

---
