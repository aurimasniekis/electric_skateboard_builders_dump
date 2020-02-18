# Antispark switches doesn&rsquo;t like long wires?

### Replies: 12 Views: 310

## \#1 Posted by: BooYA Posted at: 2018-07-05T15:38:25.730Z Reads: 128

```
Hi everyone, I was in the process of finishing my build when I went for a try of my antispark switch from @Martinsp
I first connected my focboxes to the output of the switch and making sure the button was off I connected the battery to the input. Pushed 
The button ON, everything starts, pushing again OFF and the circuit doesn't turn off.... I guess it's fried, but how? Why? 
Also, before connecting the switch to this setup I had it working great on the bench with lipos and a single esc, the wires were shorter though. 
What can I do?
Thanks for helping me :) ![20180705_172854|690x388](upload://xgE0et1DdHAl9udPakWd1feFr7S.jpg)![20180705_172800|281x500](upload://qZEK0oHMBqUUkyQXI5utFMWqOhO.jpg)![20180705_172835|281x500](upload://dV9nx9caZ97jxgx3MzWL2J7fQZe.jpg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-07-05T15:55:15.830Z Reads: 117

```
Hello, 
sorry for the trouble. This is most probably a problem with the switch. I have had to switch from making them myself to getting them made to make it quicker to meet the demand. And unfortunately a few units (so far 4 with you) have had this issue where the transistors must have been soldered on improperly. They passed QC otherwise they would not leave the factory but there is some trouble. All of that is fixed and QC increased to make sure this does not happen again. The problem is I dont have any in stock so you can decide if you want to wait for a new replacement unit to be shipped to you from the next batch or I can offer you a free repair. 

Sorry for the trouble again, let me know in how you decide.
Martin.
```

---
## \#3 Posted by: BooYA Posted at: 2018-07-05T16:03:43.275Z Reads: 112

```
Wow this is amazing customer service ! Thank you for providing a solution so quickly !
I can wait for a replacement no problem, will use a loopkey for now.
Is it difficult to repair ? I could try, I'm good at soldering. Otherwise I can send it back to you.
Thanks again Martin
```

---
## \#4 Posted by: Martinsp Posted at: 2018-07-05T16:08:14.248Z Reads: 102

```
It is not that difficult by hand. It has directFETs underneath the aluminium heatsink. They probably had a loose solderball underneath them (that is what solved the problem at the factory, using less solder paste) 

So if you want to challenge yourself you can try to replace them, you pretty much can not brake what is broken so if you want go for it.

I will mark it down and inform you when it is shipped. The pushbutton will be compatible with the new unit.
```

---
## \#5 Posted by: Silverline Posted at: 2018-07-05T18:28:13.986Z Reads: 80

```
Hallo @Martinsp
I bought your last antispark switch, last week. Do you know if there is a chance, that i have received one of the defective as well ?
```

---
## \#6 Posted by: Martinsp Posted at: 2018-07-05T18:35:49.152Z Reads: 77

```
Hi, not the whole batch is troublesome. It seems to be random not from one day but if yours is, based the previous faults, it will be obvious when you will test it like here. If it brakes I will of course replace or repair yours too.
```

---
## \#7 Posted by: Silverline Posted at: 2018-07-05T18:37:32.250Z Reads: 75

```
Can i do something before i put power on for the first time ?
```

---
## \#8 Posted by: Martinsp Posted at: 2018-07-05T19:06:25.237Z Reads: 70

```
Just obey the instructions every time you install the switch on your board, in case you lost the paper that came in the package the instructions are as a picture here http://electricskateboard.repair/index.php?id_product=36&controller=product
It is unfortunate that this happened but it is what it is, accidents happen and I will do my best to fix this for everyone who had a faulty unit as well as avoid this in the future.
```

---
## \#9 Posted by: Silverline Posted at: 2018-07-05T19:57:09.407Z Reads: 55

```
Yeah i have the instrucktions. What i mens is, can i spot the missing QC ? Or is the only way to simply just connect and try
```

---
## \#10 Posted by: Martinsp Posted at: 2018-07-05T19:59:35.413Z Reads: 54

```
You can not, it is not a visible problem. Since not only the heatsink is  covering the transistors but also the pads are underneath them so it can not be inspected visually. Just plug it in and try.
```

---
## \#11 Posted by: Silverline Posted at: 2018-07-05T20:06:21.696Z Reads: 51

```
Damn... I would loved to have sorted that out, before hitting the Streets, maybe this failure will first show up after some time :-/
```

---
## \#12 Posted by: Martinsp Posted at: 2018-07-05T20:11:10.434Z Reads: 51

```
With the nature of skateboards, there is a lot of vibrations so as long as it does not show up on your first ride when the switch will be vibrating and any loose pieces of solder short things out you will not be able to turn the board off with the switch because that is how mosfets fail, shorting input to output, luckily in this case. There is no physical connection with positive and negative so you dont have to worry about shorting your battery + and - that cant happen.
```

---
