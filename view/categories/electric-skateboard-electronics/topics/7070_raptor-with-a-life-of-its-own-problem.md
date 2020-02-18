# Raptor with a life of its own? Problem!

### Replies: 12 Views: 753

## \#1 Posted by: Drbrule Posted at: 2016-08-03T14:04:45.254Z Reads: 126

```
My raptor had been working flawlessly for about a week, then I went for a skate a few days ago, I was cruising at about 25km and it suddenly went full acceleration no brakes or anything, turning the remote off did nothing, luckily I managed to bend Down and switch it off the board. But I nearly lost it going full speed.

I'm a bit scared to ride it now, especially around traffic ect. 
I feel a remote kill switch perhaps between the vescs and the battery.

Anyone had a similar issue? Or any idea what could have caused it?

It was going crazy everytime I turned it on for about 5min after. 
I've been testing it upside-down and have had no issues in the last few days?
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-03T14:09:09.112Z Reads: 126

```
Could be interference in the ppm signal. I had this happen when some metal from my heatsink touched the antenna board on my receiver. It also happened when the the receiver got very close to the phase wires and mosfets. The AC current may be interfering with it.

Try installing a ferrite ring on the ppm signal wire and moving the receiver away from the mosfets and phase wires.

More info: http://www.rchelination.com/ferrite-rings-on-escs-what-do-they-do-and-how-can-you-use-them/
```

---
## \#3 Posted by: onloop Posted at: 2016-08-03T14:12:33.446Z Reads: 126

```
It should be checked over carefully to make sure there are no faults.

Rf interference, loose wires, sorted wires.

Also. Make sure the remote battery is charged.
```

---
## \#4 Posted by: chaka Posted at: 2016-08-03T14:19:18.853Z Reads: 121

```
You should upgrade to a GT2B remote. Plenty of modified enclosures available to give it a better form factor.
```

---
## \#5 Posted by: Pablo_702 Posted at: 2016-08-03T19:35:31.620Z Reads: 97

```
I just completed my mastercho mod for the gt2b and its sturdy, compact and easy to do
```

---
## \#6 Posted by: JTAG Posted at: 2016-08-03T22:46:58.473Z Reads: 86

```
I had random throttle peaks / breaking actions a couple of times (but this was only short like 1 second), in all the cases it was a lose wire between the master VESC and receiver.
```

---
## \#7 Posted by: Drbrule Posted at: 2016-08-04T12:23:55.742Z Reads: 67

```
I think the problem was, a lose wire and my battery is playing up, any slight pressure or bump and it cuts out and back on!

Also anyone got a fix for the braking issue i've been having!

The brakes don't ease off until you get back to the middle with the joy sick, then it's a bit of a jolt back to free rolling. They stay at the strongest braking level you've reached, then turn off completely when the joystick is back to the middle!

There's no easing off like the accelerator!
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-08-04T12:37:15.450Z Reads: 58

```
check the wiring between the receiver and VESC for broken connections. The last time this happened to one of my boards it was a loose signal cable. Same thing could happen to a soldered connection if the joint stressed and broke for any reason such as components coming loose in the box area that start tugging on things.
```

---
## \#9 Posted by: Drbrule Posted at: 2016-08-04T12:50:17.664Z Reads: 54

```
Is this in response to the brakes?
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-08-04T13:42:14.014Z Reads: 50

```
no, sorry, i should have quoted. It was in response to the board "entering rocket mode" and taking off full speed on its own and the remote losing control of the board which also included control of the brakes.
```

---
## \#11 Posted by: Drbrule Posted at: 2016-08-04T14:30:26.831Z Reads: 42

```
Do you have the same problem with braking down hills?
```

---
## \#12 Posted by: longhairedboy Posted at: 2016-08-04T14:47:01.169Z Reads: 37

```
[quote="Drbrule, post:11, topic:7070, full:true"]
Do you have the same problem with braking down hills?
[/quote]

only in extreme situations, but fine tuning things seems to help. Upping the absolute batt max helped a little while also lowering the min regen (and by that i mean moving further from zero in the negative direction) The issue i'm having at the moment is finding a balance between resolving that issue and having a board that doesn't feel quite so aggressive yet still has plenty of hill climbing and top end. To further exacerbate the issue, rider weight makes a difference, so a solution for a 150 pound lunatic like your truly may or may not work for a 220 pound rider. If VESC6 solves the regen cutting out issue as rumored maybe it won't be such a hassle. In the mean time, it takes tweaking specifically for the rider which is very challenging at best and near impossible and expensive at worst for people like me building customs.
```

---
