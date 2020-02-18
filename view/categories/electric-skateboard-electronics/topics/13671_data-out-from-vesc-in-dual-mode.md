# Data out from VESC in dual mode

### Replies: 8 Views: 826

## \#1 Posted by: B4Me Posted at: 2016-11-25T23:54:13.057Z Reads: 94

```
Hey
I'm about to make my setup using two VESC in dual mode via CAN, is there a way to get information out of both boards using only one seriel connection ?
I need things like, Current, Voltage, temp, mah, mwh... I have seen people reading these things through the UART on the VESC, but only for single boards...
I would like the information, to show it on my upcomming remote with a build-in oled screen... But would be neet to have the actual data from both, instead of multiplying the numbers, and guestimate the actual current and so :)

Please feel free to point me in the direction of docomentation explaining my needs :)
```

---
## \#2 Posted by: saul Posted at: 2016-11-26T05:58:56.996Z Reads: 76

```
not currently.
but the canbus should be able to send/rec the same data as uart. but its not implemented to relay.

assuming a symetrical drive, doubling the numbers should be accurate enough for most uses.
```

---
## \#3 Posted by: B4Me Posted at: 2016-11-26T08:26:44.633Z Reads: 66

```
You are right..  Most of the time they will be the same, or canceling each other out turning left and right..  Maybe I was overthinking it 😁
```

---
## \#4 Posted by: evoheyax Posted at: 2016-11-26T10:00:45.207Z Reads: 58

```
There is a COMM_FORWARD_CAN command that I suspect might be able to be used to forward the data via canbus. But that's as far I've gotten into sending data between vescs. It's on my longer term to do list for sure.
```

---
## \#5 Posted by: B4Me Posted at: 2016-11-26T14:11:29.107Z Reads: 50

```
Have you tried to check whats being send in dual mode over the CAN allready.. guess its only current / rpm .. but maybe more :)
```

---
## \#6 Posted by: evoheyax Posted at: 2016-11-26T16:51:49.394Z Reads: 42

```
I've been trying to figure out myself what is being sent and what's not. I though the only thing that all vescs have in common would be voltage and rpm. I'm pretty sure current is different per vesc. I only see 18 amps max which is my limit on each vesc. And x4 would give me my overall limit of 72 amps. The numbers make me believe its only one vesc in the current numbers.
```

---
## \#7 Posted by: Pedrodemio Posted at: 2016-11-26T21:45:35.780Z Reads: 29

```
http://vedder.se/forums/viewtopic.php?f=6&t=119
```

---
## \#8 Posted by: rpn314 Posted at: 2016-11-26T21:49:49.289Z Reads: 29

```
It is possible, just hasn't been implemented in any application to my knowledge, mostly due to not really having a need for it, since most of those parameters are very close to the same on each VESC (as was said above).

Edit:
BLDC Tool has implemented it actually. I forgot that I tested it a few weeks ago. You can fully write and read the secondary VESC connected over CAN-Bus via the bluetooth connection on the primary vesc.
```

---
