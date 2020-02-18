# Soldering receiver and canbus to avoid injuries

### Replies: 14 Views: 976

## \#1 Posted by: Hummie Posted at: 2016-06-16T18:27:29.907Z Reads: 167

```
U do it?
Dangerous and all my injuries are from these bad connections. Im gluing or taping them the wire in already.  

!!  I've had the breaks spontaneously go on when the batteries are unplugged but the receiver connection isn't good !!!  Just pushing around.
```

---
## \#2 Posted by: Jinra Posted at: 2016-06-16T18:31:10.144Z Reads: 163

```
When I get my parts, I'm going to gauge how tight the connections are, and if they're too loose, I'll probably hot glue them down.
```

---
## \#3 Posted by: Hummie Posted at: 2016-06-16T18:33:19.935Z Reads: 164

```
Not working for me. DIYElectricSkateboard 2.4.  Not that I think it's the receiver and it's a standard connector that's the problem
```

---
## \#4 Posted by: Namasaki Posted at: 2016-06-17T04:53:12.475Z Reads: 130

```
if your brakes are going on while the batteries are unplugged. Then it sounds like a short on the 3 phase motor wires.
Anytime you touch 2 of the 3 motor wires together it makes them brake even if they are disconnected from the system.
Try disconnecting the motors and spin them by hand, moving the wires around as you spin them and see if the brakes come on. 
I just don't see how the problem could be the receiver connection if it happens when the batteries are disconnected.
```

---
## \#5 Posted by: Nordle Posted at: 2016-06-17T05:21:12.923Z Reads: 118

```
Yeah, should run free if the rx disconnects, not brake? And yes I soldered them.
```

---
## \#6 Posted by: Hummie Posted at: 2016-06-17T06:33:06.965Z Reads: 106

```
The vesc lights up when coasting so there's some electricity doing something in there.  I thought it was maybe just me and I was delusional but after its happened now repeatedly as I repeatedly break receiver connections I'm sure.  Batteries unplugged, motors work fine, brakes slam on with bad receiver connection randomly
```

---
## \#7 Posted by: Nordle Posted at: 2016-06-17T06:37:52.202Z Reads: 101

```
Just solder them, these little connectors would make me crazy while riding on my board. or use 2mm gold connectors lol :D
```

---
## \#8 Posted by: Namasaki Posted at: 2016-06-17T15:47:08.302Z Reads: 89

```
So is that a common attribute of the Vesc, to slam on the brakes when it looses signal?
```

---
## \#9 Posted by: CSN Posted at: 2016-06-17T16:01:50.765Z Reads: 89

```
yeah the VESC has a dead man switch behavior if the controller is turned off.

The motor will still turn but a lot of resistance if I turn off my GTB.

Probably a good thing if the rider falls off then the board will try to slow down and not just rocket off a cliff or into a curb.

I use that feature if I want to walk away from the board to press a crosswalk signal etc and when I turn off the receiver it acts like a parking brake when I walk away.
```

---
## \#10 Posted by: trbt555 Posted at: 2016-06-17T16:05:28.371Z Reads: 91

```
You can set the behavior by setting the brake current at timeout.
After timeout, the vesc applies this current. If you set zero, it just coasts along.
```

---
## \#11 Posted by: Hummie Posted at: 2016-06-17T16:07:40.885Z Reads: 90

```
This is a "feature" as apposed to what I experienced which is a result of a loose receiver to vesc connection
```

---
## \#12 Posted by: Namasaki Posted at: 2016-06-17T17:37:08.181Z Reads: 83

```
Think I would just solder the signal wires to the Vesc but another thing you can try, if you don't want to solder them, is to bend the plug pins on the Vesc a little so that the connectors fit tighter.
```

---
## \#13 Posted by: Jebe Posted at: 2017-02-25T01:11:10.929Z Reads: 40

```
+1 for hot glue
```

---
## \#14 Posted by: PXSS Posted at: 2017-02-25T02:43:05.007Z Reads: 39

```
I suggest Amazing Goop over hot glue. Hot glue sucks
```

---
