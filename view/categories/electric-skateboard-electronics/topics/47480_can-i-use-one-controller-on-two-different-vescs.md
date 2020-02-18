# Can I use one controller on two different VESCs?

### Replies: 13 Views: 733

## \#1 Posted by: Snowi Posted at: 2018-02-26T05:25:14.380Z Reads: 157

```
I was to use one vesc for one motor, but have another vesc with its own motor, but each with its own channel. can i do that? i have the nano controller which i can switch channels. will i have to put one servo connector on ch. 1 and one servo connector on ch. 2? will that work?
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2018-02-26T05:31:41.234Z Reads: 151

```
For "vescs " there's 3 ways u can go about this 
1. Use canbus not really a expert on that one but u connect your vescs to each other over can bus and one vesc is a master slave that just mimics the other one 
2. Use a servo y splitter connect both ppm cables and turn them into one and just connect them like if it was one 
3. I think gt2b is the only remote that it applies for this. Get multiple receivers and bind them to one remote but to my knowledge as stated gt2b is the only one as known to be able to bind to multiple recievers
```

---
## \#3 Posted by: Mikenopolis Posted at: 2018-02-26T05:36:54.469Z Reads: 144

```
I second that. I’ve used GT2B with four separate receivers.
```

---
## \#4 Posted by: chuttney1 Posted at: 2018-02-26T05:58:55.297Z Reads: 133

```
[quote="Exiledd_Top, post:2, topic:47480"]
Use a servo y splitter connect both ppm cables and turn them into one and just connect them like if it was one
[/quote]

Giant WARNING on this because of the potential for a ground loop. The only solution is to use just the signal wire on the second VESC with the y-splitter as this is predominantly an issue seen in RC airplanes.
```

---
## \#5 Posted by: Jebe Posted at: 2018-02-26T06:00:35.382Z Reads: 123

```
Option 3. Dont use a y splitter. Ground loops can kill a vesc. Canbus works great, until it doesnt. 2 recievers bound to one controller is most reliable.
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-02-26T06:08:24.518Z Reads: 123

```
I've used y splitter all this time 0 issues I plan to use gt2b with 2 receivers and 2 y splitters for my 4wd
I allready have the gt2b recievers and y splitters
```

---
## \#7 Posted by: chuttney1 Posted at: 2018-02-26T06:16:20.704Z Reads: 115

```
The issue of the ground loop applies if you have any version of the VESC 6.X hardware.
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2018-02-26T06:37:56.061Z Reads: 108

```
Vesc 6  problem okay dam scared me for a sec it doesn't apply with 4.12 vesc's?
```

---
## \#9 Posted by: chuttney1 Posted at: 2018-02-26T06:51:54.041Z Reads: 102

```
Not really. I can't figure out why even though both designs of the VESC 6 and VESC 4.12 have the signal wire going straight to the MCU.
```

---
## \#10 Posted by: b264 Posted at: 2018-02-26T07:06:24.963Z Reads: 101

```
[quote="Exiledd_Top, post:2, topic:47480"]
Get multiple receivers and bind them to one remote but to my knowledge as stated gt2b is the only one as known to be able to bind to multiple recievers
[/quote]

Mini remote can
```

---
## \#11 Posted by: gigoy Posted at: 2018-02-26T10:36:24.276Z Reads: 85

```
Which one is the most recommended/reliable among the 3?
```

---
## \#12 Posted by: Exiledd_Top Posted at: 2018-02-26T11:21:39.216Z Reads: 82

```
Gt2b
10 char
```

---
## \#13 Posted by: Namasaki Posted at: 2018-02-27T02:44:59.304Z Reads: 58

```
[quote="Exiledd_Top, post:2, topic:47480"]
I think gt2b is the only remote that it applies for this. Get multiple receivers and bind them to one remote but to my knowledge as stated gt2b is the only one as known to be able to bind to multiple recievers
[/quote]


The Mini RC can also bind with multiple receivers and operate them simultaneously.
https://youtu.be/eSeTWe-GI8U
```

---
