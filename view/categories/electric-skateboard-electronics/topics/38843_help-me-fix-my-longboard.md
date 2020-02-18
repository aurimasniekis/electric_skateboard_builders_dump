# Help me fix my longboard?

### Replies: 4 Views: 497

## \#1 Posted by: Kaden Posted at: 2017-11-20T19:13:30.783Z Reads: 86

```
So I used torque boards parts in creating my build. I bought the 6374 motor with 190kv. I have three 4s batteries in series making it a 12s battery powering the board. I made a cheap enclosure so I could ride the board and make sure everything worked and wow that thing is scary fast. Easily could hit 35mph. I only could barely handle 26mph. I wanted to engineer a new enclosure that looked better and more reliable, and wanted an on and off switch. I got a chicago electric solder (cheap) and cut off the xt90 connector on my vesc and soldered in the switch setup (bought from torqueboards). In this process, I had a major spark happen when I had two wires touch and melted a connector. I thought this spark may have messed up the vesc, but after rewiring and soldering in a new connector, I got everything to turn on, and connect to my remote and everything worked. The motor however is not getting full power to it. I charged all batteries and tested them with a voltmeter and they are fully charged. Most of my numbers look good on the bldc tool when i plug in my board to it, but it will not detect my vesc. There is no fault code so i guess that is good, but the board is running like the batteries are dead. I need help with this!! I wanna ride! My guess is i need a better solder job done to make a better connection, but any ideas??????
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-11-20T20:04:01.336Z Reads: 69

```
You have one damaged a sensor on the vesc or damaged/shorted your motor
```

---
## \#3 Posted by: Kaden Posted at: 2017-11-20T20:06:51.344Z Reads: 67

```
Even though the motor will spin fairly quickly? just not full power? @Exiledd_Top
```

---
## \#4 Posted by: halifax21 Posted at: 2018-08-16T00:12:10.809Z Reads: 27

```
Check the battery cut off start and end on the vesc, the spark reset the values of the vesc, which would explain why you can’t detect the motor or have it running at full power
```

---
