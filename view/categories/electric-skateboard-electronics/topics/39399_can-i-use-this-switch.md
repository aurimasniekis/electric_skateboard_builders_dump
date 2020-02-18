# Can i use this switch?

### Replies: 13 Views: 582

## \#1 Posted by: dg798 Posted at: 2017-11-26T23:38:30.881Z Reads: 98

```
can i use this switch to power my board?
it says on the side, "1 amp,125v DC and 4a 125v ac, and 2a 250v ac.
<img src="/uploads/db1493/original/3X/f/7/f78545263c28d0955505d63ea5eab93965c0e69f.JPG" width="375" height="500">
```

---
## \#2 Posted by: dg798 Posted at: 2017-11-26T23:39:14.688Z Reads: 94

```
i looked already but couldnt find any threads like this. sorry if i might have missed it
```

---
## \#3 Posted by: michaelcpg Posted at: 2017-11-26T23:43:33.020Z Reads: 93

```
You could use it but only as a softswitch with a BMS or antispark mosfet switch. A switch that size won't be able to handle the full battery current running directly through it
```

---
## \#4 Posted by: dg798 Posted at: 2017-11-26T23:45:56.615Z Reads: 89

```
So I can’t just use it as is?
```

---
## \#5 Posted by: darkkevind Posted at: 2017-11-26T23:46:44.677Z Reads: 86

```
DO NOT attempt to use this switch to cut off your main power from your battery... It will fry within seconds of riding...

You need a switch rated for at least 60A.
```

---
## \#6 Posted by: michaelcpg Posted at: 2017-11-26T23:47:37.962Z Reads: 78

```
This switch is rated for around 2A. We draw a LOT more than that so this will just blow instantly if you just use it directly in the circuit...
```

---
## \#7 Posted by: dg798 Posted at: 2017-11-26T23:49:23.487Z Reads: 77

```
So I can use though any switch that’s rated at least 60 amps? Any links?
```

---
## \#8 Posted by: michaelcpg Posted at: 2017-11-26T23:52:07.522Z Reads: 73

```
I would suggest you do some more research on these forums as it's a little more complicated than that. Even normal switches that are rated for 60A or more will create a big spark each time you connect them which isn't ideal.

Have a look into antispark mosfet switches and XT90S loop keys. I would recommend using an XT90S loop key personally
```

---
## \#9 Posted by: dg798 Posted at: 2017-11-26T23:54:21.620Z Reads: 67

```
Ok thanks guys
```

---
## \#10 Posted by: Namasaki Posted at: 2017-11-30T04:10:37.552Z Reads: 39

```
@michaelcpg is right, you cannot use a mechanical switch because of the rush of current when you turn it on.
I would also recommend using an antispark loop key. It's a sure bet and the least complicated.
There are some that have used automotive breaker switches for 6s builds with good results.
I tried to use a 200a auto breaker switch with 12s on my first build and it worked but wore out fairly quick.
The breaker switches are also rather bulky.
```

---
## \#11 Posted by: michaelcpg Posted at: 2017-11-30T06:47:48.070Z Reads: 30

```
As someone who initially used a BMS with an integrated mosfet switch, a loop key would be my recommendation as well. It's a simpler design and it also means that when your board is "switched off" the circuit is actually fully broken as opposed to a mosfet switch which doesn't technically fully break the circuit, instead just adding a large point of the resistance into the circuit. You'll probably find most examples of XT90S loop keys on this forum to be pretty bulky looking but its actually really easy to make them fairly inconspicuous. Here's mine for example

<img src="/uploads/db1493/original/3X/d/f/df556036b865f85adeea3e4bd1b6d37fbf07d0b7.jpg" width="281" height="500">
```

---
## \#12 Posted by: Vanarian Posted at: 2017-11-30T11:52:13.064Z Reads: 20

```
Funny fact I just realized : having a loop key is literally having a **key** to start your board :santa:
```

---
## \#13 Posted by: dg798 Posted at: 2017-11-30T12:25:28.695Z Reads: 19

```
Alright cool thanks
```

---
