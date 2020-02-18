# Anti-Spark Wiring Help

### Replies: 9 Views: 597

## \#1 Posted by: Emerson Posted at: 2018-03-22T19:22:46.976Z Reads: 139

```
I purchased an anti-spark from anti-spark heaven and a [power switch](https://www.amazon.com/gp/product/B071H9KXKQ/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1) a little while ago for my upcoming Icarus build.

The Problem: when I wire everything together my multi-meter reads full power regardless of the button being depressed or not and the LED glows no matter what. 

Configurations I've tried (From Anti-Spark to Switch):
Option 1:
NO -> NO
C -> C
NC -> NC
LED+ -> LED+
LED- -> LED-

Option 2 per suggestions I've seen on the forum:
NO -> NO
C -> C
No Connection between NC terminals
LED+ -> LED+
LED- -> LED-

Any suggestions?
```

---
## \#2 Posted by: Namasaki Posted at: 2018-03-24T00:35:42.696Z Reads: 116

```
Your antispark switch could be broken and stuck in the on position. 
This is very typical of antispark switches.
```

---
## \#3 Posted by: neffson Posted at: 2018-05-08T10:42:04.493Z Reads: 97

```
I have the same problem.
I've now tested it with a lower voltage battery. 14V to be exact. Works perfectly fine.
At 41V - 50V there's a spark when I connect the switch to the battery and the circuit is stuck closed.
I've tested both MOSFETs and they work as intended.
I'm thinking the problem could be the spark upon connection or maybe my BMS.

Any help would be useful.
```

---
## \#4 Posted by: Emerson Posted at: 2018-05-08T11:10:32.182Z Reads: 89

```
Total honesty here...mine was soldered backwards.  One of the labels for the polarity was written wrong on the anti-spark itself and I didn't see it at first.  Upon reversing the direction of the anti-spark it worked as intended.
```

---
## \#5 Posted by: neffson Posted at: 2018-05-08T11:26:06.301Z Reads: 88

```
In what way exactly?
```

---
## \#6 Posted by: Emerson Posted at: 2018-05-08T11:48:01.590Z Reads: 83

```
As an example, here's how it should be wired:  Battery --> (IN) Anti-Spark (Out) --> Focbox.  I had it this way...

Battery --> (OUT) Anti-Spark (IN) --> Focbox

After reversing the flow by re-soldering the correct direction for the connections mine worked fine.


![drawing_with|689x363](upload://VmLuBaaNhu7fuXwgCfBW5ixhLg.png)
```

---
## \#7 Posted by: neffson Posted at: 2018-05-08T12:06:00.589Z Reads: 75

```
Thanks for your reply!
I have mine wired the right way. 
Guess I have to keep looking for a solution.
```

---
## \#8 Posted by: neffson Posted at: 2018-05-08T14:23:33.370Z Reads: 71

```
Okay problem is solved!
Actually there never was a problem. Just a lack of patience on my end.
After pushing the button to turn off the board I have to wait about 30 seconds for my ESCs to power down.
Add another 30 seconds and the LED has faded aswell.

Hope this helps someone in the same situation.
```

---
## \#9 Posted by: Emerson Posted at: 2018-05-08T14:33:52.105Z Reads: 64

```
Glad you got it sorted!  I wondered the same thing when I first got mine working.  Have to give the caps time to drain I suppose.
```

---
