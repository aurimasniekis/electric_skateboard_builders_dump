# 4.10 VESC with nunchuck

### Replies: 12 Views: 1903

## \#1 Posted by: tomtnt Posted at: 2015-11-15T06:32:11.608Z Reads: 88

```
I purchased and received an absolutely beautiful VESC from @chaka.  It came with nunchucky adapter and JST connector.  Tried that but got intermittent drop outs (only when riding, never on bench).  

Tried to solder JST directly to nyko dongle but still had dropouts.  Finally, soldered directly onto VESC pads but still getting dropouts!

Any possible solution other than switching to gt2b?
```

---
## \#2 Posted by: elkick Posted at: 2015-11-15T09:42:05.706Z Reads: 88

```
I'm using the Kama Nunchuk on 4 different boards with VESCs (V4.7 & 4.10) and never had any dropouts. All of them are soldered to a JST connector plugged into the VESC. 

Did you check if the receiver is placed well for connection and if the Kama transmitter is really stable? They tend to vary in quality.

Also, when using the beercan board (aluminum deck) I placed (and sealed) the Kama receiver at the outside of the electronics box just in case that the deck could prevent proper connection.
```

---
## \#3 Posted by: tomtnt Posted at: 2015-11-15T15:00:08.915Z Reads: 85

```
[quote="elkick, post:2, topic:471"]
Did you check if the receiver is placed well for connection and if the Kama transmitter is really stable? They tend to vary in quality.
[/quote]

Do you place it far away from the VESC and motor?
```

---
## \#4 Posted by: tomtnt Posted at: 2015-11-15T21:03:38.250Z Reads: 79

```
knock on wood, but I think I solved my disconnect issue by powering the nyko wireless dongle with 5v rather than 3.3v - the arduino guys using the nunchuck seems to be using it without issues for awhile @5v without issues... will test more and hope the thing doesn't fry when I'm going at high speeds!
```

---
## \#5 Posted by: elkick Posted at: 2015-11-15T21:55:12.579Z Reads: 79

```
I placed it at the edge of the board because of the massive aluminum deck. It's more a precaution then a need I guess. But I don't know how those different makes of the Kama receiver behave, I've connected mine with 3.3V though.
```

---
## \#6 Posted by: tomtnt Posted at: 2015-11-16T17:50:18.068Z Reads: 77

```
I spoke too soon... still getting tons of random dropouts.. will buy a new wireless nunchuck to test....  pretty annoying
```

---
## \#7 Posted by: tomtnt Posted at: 2015-11-19T04:29:24.402Z Reads: 71

```
well, I replaced the nunchuck dongle with another nyko kama dongle and it works with no dropouts... looks like some of these dongles aren't as robust as others..
```

---
## \#8 Posted by: lowGuido Posted at: 2015-11-19T11:02:09.234Z Reads: 70

```
Was it one with the massive PCB or the small one?
```

---
## \#9 Posted by: tomtnt Posted at: 2015-11-19T15:03:08.725Z Reads: 70

```
They were both the small ones
```

---
## \#10 Posted by: treenutter Posted at: 2015-11-20T17:03:43.259Z Reads: 70

```
@tomtnt @elkick @lowGuido Has anyone tried using a ferrite ring on the wires between the Nyko Kama receiver and the JST connector plugged into VESC help prevent interference? I've wondered if that might help reduce dropouts. It's hard to figure out whether they are caused by a physical disconnection or radio interference.
```

---
## \#11 Posted by: tomtnt Posted at: 2015-11-20T17:38:29.023Z Reads: 68

```
that's a good point - I'm just going to wait for enertion to release the Vedder/Jaccoby nunchuck transmitter/receiver.  I don't trust the current nunchuck.  I tried using the big GT2b but, damn, that thing is huge and looks really out of place
```

---
## \#12 Posted by: elkick Posted at: 2015-11-20T22:34:57.315Z Reads: 67

```
I have used the ferrite ring but no difference, no dropouts for months on none of the boards. Beside soldering carefully I only used some hot glue to keep the JST plug in place on the VESCs and made sure that the wires to the Kama receiver do not cross the motor wires.
```

---
