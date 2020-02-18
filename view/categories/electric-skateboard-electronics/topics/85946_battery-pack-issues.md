# Battery pack issues

### Replies: 8 Views: 264

## \#1 Posted by: JensSjogren Posted at: 2019-03-03T19:24:30.203Z Reads: 90

```
Hi good folks, so i just finnished building my first battery pack and connected everything to a xiaoxiang 12s BMS like shown on this picture.

![IMG-20190302-WA0011|240x500](upload://w3G3egaquhM0GWGu2QqXXW4NHdP.jpeg) 

So far so good, i get the right amount of voltage out from the XT90 connector that will go to the ESC. This BMS has a app which i was able to connect to.

![Screenshot_20190303-192631_xiaoxiang|243x500](upload://ihZdeGgS9a3PTLLDGk6JUdzo5Pc.jpeg) 

First problem i noticed was that the charger doesnt seem to charge the battery when plugged in, the LED on the charger stays green, before soldering the charging wires i used a voltmeter while the charger was connected to the port to determine the plus and minus poles on the charging port so i got the cables soldered on the right spots. 

Second problem was that when i connected the battery to my esc's they didnt start up. Which is very strange to me since i get 41.3 volts oit of the XT90. 

Here are some pictures that could be of use for anyone that may be able to locate the problem. 

![20190303_195110|374x500](upload://nynxEDIRpKpMGc5AYUqShrARgrT.jpeg) 
![20190303_195153|666x500](upload://lnffC4k8K9Qj9WyTC3sAIt6KUUL.jpeg) 
![20190303_195210|666x500](upload://5APy6Lb5pb0fcMTqG2Zx7gibk8T.jpeg) 


Any help would be greatly appriciated!
```

---
## \#2 Posted by: Benjamin899 Posted at: 2019-03-03T20:35:39.158Z Reads: 54

```
sounds rly strange. It doesn't have a E-Switch. Maybe it is still locked through the app?
```

---
## \#3 Posted by: JensSjogren Posted at: 2019-03-03T20:46:33.547Z Reads: 54

```
Not from what i can see no. That thought hit me aswell so i browsed through everything in the app but could not find anything related to either of my problems.
```

---
## \#4 Posted by: pjotr47 Posted at: 2019-03-03T20:48:40.042Z Reads: 53

```
Looks more like broken bms + I think you need a better solder iron![image|690x450](upload://2wFdLfSnKqITXQkw8LoXgDEQPDk.jpeg)
```

---
## \#5 Posted by: Therealesk8 Posted at: 2019-03-03T21:07:09.844Z Reads: 50

```
Hmmm, try to press that button: ![xiaoxiang|241x500](upload://3pi6VYH2OGKrsdbD5W5tR2utsk6.jpeg)
```

---
## \#6 Posted by: rojitor Posted at: 2019-03-03T21:08:01.289Z Reads: 48

```
The contact is poor. You soldered more on the pcb than the metal. Make the wires pass through the holes and solder both sides. Check every connection and make sure your settings at the app are ok. For example if you have set the option to balance while charging you will not notice a single volt difference for a long time
```

---
## \#7 Posted by: JensSjogren Posted at: 2019-03-03T21:34:24.116Z Reads: 44

```
may be, never soldered on circuitboards before so i didn't want to keep the iron there to long, however i'm convinced that i didn't solder on the pcb (if by that you mean the green part). nevertheless i do measure voltage both on the B- and C- aswell as on the charging port so contact should not be the reason why it wont charge. I will redo the solders and put the wires in the holes instead aswell as digging more inte the settings
```

---
## \#8 Posted by: Benjamin899 Posted at: 2019-03-03T22:25:53.728Z Reads: 42

```
good thing about soldering on a pcb is that the solder stays on the contactpatch. So you can use more solder and it will stay where it is supposed to be. As far as my expierence goes.
```

---
