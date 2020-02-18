# \[SOLVED\] Two 3S as 6S weird charger behaviour

### Replies: 2 Views: 262

## \#1 Posted by: murloc992 Posted at: 2018-09-20T20:55:33.410Z Reads: 30

```
Greetings,

I am facing bad charger behavior when trying to use a self-made 2x 3S to 6S balance harness.

The charger is a genuine iMax B6 AC with Chea-Li firmware.

I am quite sure I set my harness up correctly as nothing is exploding and I get correct voltages when measuring the pinout that goes to the 6s plug.

Yet when I plug it to the charger to do a calibration weird readings seem to happen when measuring straight at the charger(disassembled for calibration).

The diagram I based my harness on:
![image|682x299](upload://uNg4dmk07viePl3oZU05ZqBK6fD.png) 

This is how my harness looks like:
![07|690x388](upload://50iYDLqfQZbW557Em3o5Jq1EdWP.jpeg) 
First cell balancer first pin is black colored wire.

![37|690x388](upload://i5LPgXPH49iVhKOmcMvSc4JEOFg.jpeg) 
The last pin of first battery is connected to first pin of second battery both being combined on the orange cable.

All cells report good readings except for cells 3(red/orange) and 5(yellow/green).

All cells show 4.11, the same as the voltmeter, but those problematic ones show 4.26(while voltmeter at the plug shows 4.11)! 

When I connect my 3S batteries normally, they show correct cell voltages.

When I connect a 4S battery, even it shows normal voltages, so it cannot be a charger issue I think..

Anybody has faced such an issue and might know what's up?

I want to charge these lipos as a single battery! :smiley:
```

---
## \#2 Posted by: murloc992 Posted at: 2018-09-21T12:40:37.350Z Reads: 18

```
Apparently removing the third pin connection from the first battery balancing plug and putting it to first one of the second battery instead (3+4 instead of 4+3 and a connection in the middle) made everything work. No idea why though..
```

---
