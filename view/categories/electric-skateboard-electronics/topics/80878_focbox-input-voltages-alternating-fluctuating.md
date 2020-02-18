# FOCBOX input voltages alternating/fluctuating

### Replies: 12 Views: 205

## \#1 Posted by: visnu777 Posted at: 2019-01-14T20:43:14.576Z Reads: 80

```
Hi there, 
i realized today that one of my two focboxes has a really bad input voltage accuracy.
Here is a quick graph showing a comparison to the other Focbox, not quite accurate since the values are just the result of  entering "volt" in the Terminal followed by arrow down plus enter :) and it took place one at a time.

![focbox_error|690x387](upload://6sNUmw2BalSSnaen14wsQ2QpgKw.png) 

What is the consequence of this? Is this a symptome of a common error, maybe loose caps? Can I still drive with it or does it need repair?

Michael
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-14T20:45:20.393Z Reads: 74

```
Maybe to tag @JohnnyMeduse he for sure can tell you what could cause it.
```

---
## \#3 Posted by: linsus Posted at: 2019-01-14T20:53:48.612Z Reads: 71

```
Check power leads for bad solders/loose contact. Thats my initial thought.
Or the Caps.
```

---
## \#4 Posted by: visnu777 Posted at: 2019-01-14T21:16:29.216Z Reads: 66

```
![1547500483499132988850265027521|375x500](upload://en4J79NMtfUVoOdIY4I1HzvlrvN.jpeg)

 it looks a bit like a bad solder joint, let's see if resoldering will work...

edit: resoldering the cap connections didnt help, now, lets see how the xt60 look underneath the shrinktube :)
```

---
## \#5 Posted by: visnu777 Posted at: 2019-01-14T21:58:05.054Z Reads: 60

```
hmm, resoldered the xt60, still not better :(
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2019-01-14T23:06:20.823Z Reads: 54

```
Are those reading from an app or the bldc tool (or vesc tool)?
```

---
## \#7 Posted by: visnu777 Posted at: 2019-01-14T23:42:42.777Z Reads: 50

```
Both. when reading from vesc tool and by metr pro.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2019-01-15T02:33:21.757Z Reads: 43

```
That is kinda weird... Maybe you could try to add some solder to the big cap.

Also, I see some solder ball near the DRV. i could be a good idea to clean the pcb a little
```

---
## \#9 Posted by: ElectricCoast Posted at: 2019-01-15T02:38:32.381Z Reads: 42

```
You could always swap the two xt connectors and see if the problem jumps to the #2 FocBox.
```

---
## \#10 Posted by: visnu777 Posted at: 2019-01-15T20:05:44.292Z Reads: 36

```
hmm, nothing is working. Since I'll send some other Focboxes to @Martinsp I just send this one along, maybe he'll find something :(
```

---
## \#11 Posted by: Martinsp Posted at: 2019-01-15T20:21:56.977Z Reads: 34

```
If it rides without problems (errors, cogging etc) it should not be a very big issue, what were you powering it with? Battery or some other power supply? You could also try to spread the pins on the XT connector to put a bit more preload there but assuming it rides without some issues that should not be the case. 
Was the measuring done under load?
```

---
## \#12 Posted by: visnu777 Posted at: 2019-01-15T20:46:34.387Z Reads: 31

```
Not for the above diagram but the voltage indicator in metr jumped rapidly when I drove. It worked but I had a bad feeling about it so I didn't drive a lot. I replaced the focbox with a fsesc 4.12, now it's working. The fsesc has no fluctuations at all, the left focbox has little but no huge spikes like in the diagram and it doesn't affect metr.
```

---
