# How to safetyproof board?

### Replies: 7 Views: 413

## \#1 Posted by: nikoli280 Posted at: 2017-12-11T20:55:47.416Z Reads: 119

```
Hi everybody.

I am almost done making my board. I am just begining to think about safety. What if the remote stops working, and the board just continues. What if i need to stop quick and no response from the remote.

I would like to make a remote switch that could turn off the power from battery to VESC fast. But i dont think that is possible with so high Amps. 

So what would you do. i have thought of adding this https://hobbyking.com/en_us/turnigy-signal-loss-and-low-battery-fail-safe.html 

But im not sure it would help anything
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-12-11T21:25:29.255Z Reads: 102

```
Most remotes have a failsafe built in so that in the event of a signal loss, the receiver goes to the "neutral" position (neither gas nor brakes) and you'll coast to a stop. If you need to stop faster than that, you should learn to slide the board, and/or be prepared to run/jump/roll off the board.
```

---
## \#3 Posted by: nikoli280 Posted at: 2017-12-11T22:08:35.469Z Reads: 86

```
I am going to make a bluetooth remote with some components such as a nRF24 module and an arduino Nano. Do you think it could be programmed into that?
```

---
## \#4 Posted by: banjaxxed Posted at: 2017-12-11T22:12:29.637Z Reads: 78

```
@mmaner has a good xt90 safety loop built in a voltage monitor LCD case which mounts to the truck bolts , kills two stones with a safe power cycle and emergency cord
```

---
## \#5 Posted by: JdogAwesome Posted at: 2017-12-11T23:29:57.184Z Reads: 60

```
You could, plenty of people have talked about doing that, look around on the forum. Though it's going to be a pain in the ass and very time consuming to make something that works and is safe. I'd recommend just getting a good reliable remote like the GT2B and printing a housing for it. I've never had any signal drop out problems with it, even at different levels of my house, and I've been using the same module for 2 years.
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2017-12-11T23:31:50.746Z Reads: 55

```
i cannot recommend learning how to slide enough. having the skills necessary to stop an unpowered board may very well save your life. It's also fun as hell to go bomb some hills on an old-fashioned board.
```

---
## \#7 Posted by: chuttney1 Posted at: 2017-12-11T23:54:06.473Z Reads: 50

```
I still use the RC transmitter. I'm am not confident with the use of using Bluetooth because random dropouts in a noisy environment make it unstable. I need 100% fail-proof solution, like mission-critical grade.
```

---
