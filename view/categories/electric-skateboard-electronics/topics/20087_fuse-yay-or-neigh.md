# Fuse, yay or neigh?

### Replies: 9 Views: 698

## \#1 Posted by: brandon Posted at: 2017-04-01T00:05:16.882Z Reads: 137

```
The fuse (40A) on my antispark blows every single time I turn on the switch. I've been running fine without the switch straight from the batteries no problem. Is the fuse really necessary or can I just bridge the connection points?
```

---
## \#2 Posted by: Pantologist Posted at: 2017-04-01T00:22:11.216Z Reads: 136

```
Just from turning the switch on? Why would a 40A switch blow that fast unless 40A+/a short is taking place.
```

---
## \#3 Posted by: brandon Posted at: 2017-04-01T00:35:31.861Z Reads: 131

```
I took the fets off the board, resoldered one, stuck an LED on the output and it seemed to be functioning correctly. I put the second fet back on the board, plugged it into my vesc, and turning it on immediately blew the fuse. I am just testing now, and for some reason I am getting voltage on the output regardless of switch position. Fuck.
```

---
## \#4 Posted by: Pantologist Posted at: 2017-04-01T00:48:23.448Z Reads: 127

```
Yup something is screwed up. 

Mosfets are hard to solder with improper soldering bits. A hot air station would be ideal.
```

---
## \#5 Posted by: brandon Posted at: 2017-04-01T00:49:37.679Z Reads: 120

```
I was sure at least the one was still good though. I'm getting voltage through it even with no voltage on the gate pin though so I guess its blown. Same thing with the second fet.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-04-02T04:05:13.944Z Reads: 82

```
Time to put that switch in the electronic recycle bin.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-02T04:09:12.252Z Reads: 79

```
An easy and safe way to have an LED on//off light is to get a push button with built in LED and connect the pos/neg pins for the light to an rc signal cable and plug it into an empty channel on your receiver. 
I did mine that way and it works perfectly.
```

---
## \#8 Posted by: brandon Posted at: 2017-04-02T22:07:08.776Z Reads: 57

```
ummm no I don't think so, the replacement mosfets are cheap
```

---
## \#9 Posted by: LukeL Posted at: 2017-04-03T02:00:35.757Z Reads: 52

```


[quote="brandon, post:5, topic:20087"]
I'm getting voltage through it even with no voltage on the gate pin
[/quote]

do you mean current through it?

you're supposed get a voltage across an open switch ie when the gate voltage is low
```

---
