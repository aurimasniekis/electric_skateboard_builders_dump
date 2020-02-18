# Bad Vesc Possibly?

### Replies: 6 Views: 571

## \#1 Posted by: Wallgreeens Posted at: 2017-09-14T01:50:11.887Z Reads: 121

```
It all started this morning.  I rode my board and it worked just fine.  Then I came home after work for a short ride, but one motor was twitching and the other wouldn't spin.  This happened before and it was a bad motor, so i figured it would be the same thing. I have a 12s4p, 2 vesc-x, and 2 enertion rspec ghost motors. When I connect one of the vescs to either motor the both motors work just fine.  Then I connect the other vesc to the computer, but it will not detect either motor and they will not spin even using the bldc tool using start detection.  I am bypassing the remote and using my keyboard as my remote.   When I check  real time data and check the current, the graph is dancing like crazy on both vescs, but only the one vesc will output power.  One vesc goes over 100 watts of power and the duty cycle goes past 70%.  The malfunctioning one goes up about a half a percent and negative a half a percent. I have reset the vesc settings to default, but the problem still persists.  The vescs are connected via can bus. It is a LHB build, so I have only done slight modifications to his work.  I've checked all the connections and they are tight.   Any advice would be greatly appreciated.
```

---
## \#2 Posted by: crustyxpunk Posted at: 2017-09-14T07:55:32.465Z Reads: 93

```
Have you tried to contact @longhairedboy and see what he thinks? I mean now that you have modified it, it's yours but he might have some insight into your issue.
```

---
## \#3 Posted by: Wallgreeens Posted at: 2017-09-14T22:40:14.078Z Reads: 68

```
He would probably know the answer as he is an expert in his field, but I'm pretty confident it is the vesc.
```

---
## \#4 Posted by: dg798 Posted at: 2017-09-14T22:45:15.922Z Reads: 66

```
Plug in the vesc that's not working and go to the terminal section on the top of the bldc tool and type in faults and if there is some sort of fault or problem it will show you.
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-09-15T14:43:45.020Z Reads: 52

```
check the CAN bus connections. Replace the wires and solder in new ones, then run detection and save it on each motor and see what happens afterward.
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-09-15T14:45:08.833Z Reads: 49

```
also its worth noting that my boards are 100% hackable and although it voids my warranty to do whatever you want with them, i still stick around and help out and usually provide replacement parts at my cost when needed.
```

---
