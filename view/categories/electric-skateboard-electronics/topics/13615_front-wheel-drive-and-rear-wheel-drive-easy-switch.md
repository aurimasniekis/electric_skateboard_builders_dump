# Front wheel drive and rear wheel drive easy switch?

### Replies: 9 Views: 925

## \#1 Posted by: Michael319 Posted at: 2016-11-24T22:40:02.383Z Reads: 125

```
So my deck is symmetrical on both sides. If I wanted to easily switch between between FWD and RWD, is there a easy VESC setting for that?
```

---
## \#2 Posted by: Luke Posted at: 2016-11-24T22:44:32.465Z Reads: 123

```
my 2 cents: I believe the GT2b remote lets you switch the way which the motor spins, making a FWD board work as a RWD
```

---
## \#3 Posted by: Blasto Posted at: 2016-11-24T22:46:54.340Z Reads: 122

```
Switch twophase wires on your motor to the vesc
```

---
## \#4 Posted by: Michael319 Posted at: 2016-11-24T23:23:09.080Z Reads: 110

```
I know that works, but I don't want to open up the enclosure just to switch, I would much rather just connect the vesc or use a remote
```

---
## \#5 Posted by: Jinra Posted at: 2016-11-24T23:28:16.011Z Reads: 105

```
Just use "current" control mode which will give you reverse
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-11-25T08:31:35.617Z Reads: 80

```
Just use "Current with reverse". After you have brake to still stand and keep pushing brake you will drive backwards without changing or swapping anything ;)
```

---
## \#7 Posted by: Okami Posted at: 2016-11-25T11:17:11.673Z Reads: 66

```
But the trigger has to be pushed the other way around! :D

So I think it still comes to two choices, if you want that trigger direction stays the same

The mentioned:

Hard-wiring method - make a switch which makes the current go both ways (depending on switch position)

Software method - making it possible to switch settings (direction) on the go.. which probably is not yet so easy to do,,
```

---
## \#8 Posted by: rpn314 Posted at: 2016-11-25T16:54:37.327Z Reads: 54

```
I know with nunchuckRF on the VESC it's as easy as pushing a button, so it can't be too hard to implement something similar for the GT2b, but you're definitely looking at a custom firmware since I don't think it's already there.
```

---
## \#9 Posted by: saul Posted at: 2016-11-25T20:05:47.456Z Reads: 46

```
You can use the nunchuck but there were connection issues..
An nrf remote would work but you'd have to make one.
The easiest would be current with reverse and a gt2b so you can flip directions of the control instead of holding backwards and trying to remember
```

---
