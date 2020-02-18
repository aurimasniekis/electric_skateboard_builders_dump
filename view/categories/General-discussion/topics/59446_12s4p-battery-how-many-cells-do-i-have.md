# 12s4p battery how many cells do I have?

### Replies: 6 Views: 348

## \#1 Posted by: Dogman1247 Posted at: 2018-06-20T03:40:19.013Z Reads: 110

```
I have a 12s4p bldc tool the new vesc tool wants to know how many cells for battery cutoff limits

do I have 12? or do I have 48 cells? 12x4=48 is my math here.. help please :D
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-06-20T03:41:31.617Z Reads: 110

```
You have 12 cells. This is what you should choose. If you had a 10s4p (Like I do) you would choose 10.

![esk8|690x103](upload://imbMX6AOdpNkjuk2rlvipUW63Dz.png)
```

---
## \#3 Posted by: Dogman1247 Posted at: 2018-06-20T03:48:56.882Z Reads: 99

```
thank you very much!
```

---
## \#4 Posted by: PatRocks Posted at: 2018-06-20T03:49:45.153Z Reads: 100

```
What the cutoff calculator is"asking" is how many packs do you have in series. It's a voltage based protection. You have 12 packs of 4 cells in series.
```

---
## \#5 Posted by: Dogman1247 Posted at: 2018-06-20T04:01:27.183Z Reads: 85

```
another question, I am running motor detection with kaly nyc 6374 motors, on a kaly nyc street carver setup

i am running detection in FOC and it says FOC detection failed? should I run the motors in bldc?
```

---
## \#6 Posted by: SeanHacker Posted at: 2018-06-20T04:03:14.885Z Reads: 76

```
Are your sensors connected correctly? I've had them fail when detecting FOC when my wires weren't correct.
```

---
