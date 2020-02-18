# BMS compatibility question

### Replies: 7 Views: 127

## \#1 Posted by: TreeFactory Posted at: 2018-11-11T16:34:10.641Z Reads: 44

```
Hello, I am working on my first build and I believe I am approaching the end of the build. But I am currently a bit tripped up by the electronics. I've bought 4 of the Turnigy Graphene 6000mAh 3S 65C Lipo Pack W/XT90 to run as a 12s on dual Focboxes. My question is will these batteries work with the MiamiBoard[https://miamielectricboards.com/shop-1/12s-bms] 12s BMS thats for their stealth batteries?
```

---
## \#3 Posted by: Andy87 Posted at: 2018-11-11T17:08:31.118Z Reads: 27

```
You need a lipo bms for lipos if you want to use it for charge and discharge.
If their stealth battery is lipo than it should work.
If it’s LiIon than no.
With this bms you limit your power output to 50a.
That’s a batt max value for 25a per focbox instead of 50a per focbox which you could use with your battery.
```

---
## \#4 Posted by: TreeFactory Posted at: 2018-11-11T17:12:40.041Z Reads: 24

```
I see. Thanks for the help
```

---
## \#5 Posted by: Andy87 Posted at: 2018-11-11T17:15:25.104Z Reads: 23

```
You can get a 80a bms from bestech.
Should be not much more expensive.
```

---
## \#6 Posted by: TreeFactory Posted at: 2018-11-11T17:19:19.610Z Reads: 20

```
With that 80a BMS does it need to be specifically designed for LiPos or is it just a numbers thing?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-11-11T17:23:34.266Z Reads: 19

```
If you order you need to ask for lipo configuration.
Lipos have a higher cut off voltage.
You can use a LiIon bms for lipos too, but it will not protect from over discharge. 
If you don’t set your cut off limit in the focbox than you can over discharge your lipos in this case.
```

---
## \#8 Posted by: TreeFactory Posted at: 2018-11-11T17:30:28.793Z Reads: 19

```
Gotcha. I haven't gotten to the research phase about programing the focboxes just yet. I figured I'd buy all the equipment first then learn what to do with software. Thanks again for the quick response and info.
```

---
