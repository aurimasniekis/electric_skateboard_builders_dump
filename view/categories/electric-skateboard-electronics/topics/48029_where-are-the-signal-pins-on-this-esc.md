# Where are the signal pins on this ESC?

### Replies: 5 Views: 433

## \#1 Posted by: caprabianca Posted at: 2018-03-03T14:44:54.791Z Reads: 54

```
Hi guys! I need the help of more experienced users than me: I am going to buy this ESC, but I first need to know if I can use it as I need.
In a few words, I need to control the ESC (and so the motors) with an external microprocessor. Thus, I need to connect it to the ESC through some pins (one of which gives the PWM signal). Do you think that in the pic/link ESC I'll be able to find these pins (they should be 3), or the receiver for the remote is built-in and I'll not be able to make the connection? 

https://meepoboard.com/products/electronic-speed-controller

![69_2000x|500x500](upload://5Dd4AW5FFjjpxhLvZ3zKgPY8CMH.jpg)
```

---
## \#2 Posted by: Lumaci Posted at: 2018-03-03T15:14:12.895Z Reads: 45

```
The reciever is built into the pcb on that one, you might be able to find the signal wires but theres no direct pins for it.
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2018-03-03T17:20:33.466Z Reads: 35

```
like lumaci said, this ESC has an integrated receiver and therefore isn't intended to be used with a separate receiver. That being said, it is (in theory) possible to find the receiver output, break the trace, and connect your own receiver in its place. Nobody's done it yet but that doesn't mean it cant be done.

Take this with a grain of salt though, because i'm no expert
```

---
## \#4 Posted by: caprabianca Posted at: 2018-03-03T17:30:51.414Z Reads: 28

```
Okay thanks, I'll try that then when I'll get the board
```

---
## \#5 Posted by: caprabianca Posted at: 2018-03-03T17:38:11.793Z Reads: 28

```
Are you aware of any other cheap single Hub motor e-board(under 200€)? (with a good quality/price ratio, as the Meepo should have)
```

---
