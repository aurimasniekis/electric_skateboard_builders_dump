# Is it possible to test (hub) motors without ESC or battery?

### Replies: 12 Views: 721

## \#1 Posted by: Bensaida Posted at: 2018-02-22T02:27:30.786Z Reads: 84

```
title says it all.... thanks
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-02-22T02:33:05.009Z Reads: 83

```
@Bensaida Depends how thorough of a test you want to perform. If you just want to check that the windings aren't shorted and the bearings aren't sized, then yes. If you want to actually TEST the motor, as in apply power and get a feel for it's performance, then the answer is no.
```

---
## \#3 Posted by: ShutterShock Posted at: 2018-02-22T02:36:12.118Z Reads: 84

```
In order to spin a brushless motor (most of the ones we use), you need a BLDC style controller to deliver the power to the phases, or a FOC sine wave controller to deliver the power.

You cannot plug it straight into a battery, but if it was a brushed motor you could.
```

---
## \#4 Posted by: Bensaida Posted at: 2018-02-22T02:49:02.603Z Reads: 77

```
[quote="MysticalDork, post:2, topic:47105"]
Depends how thorough of a test you want to perform. If you just want to check that the windings aren’t shorted and the bearings aren’t sized, then yes
[/quote]

 how would i do that @MysticalDork
```

---
## \#5 Posted by: Apolo Posted at: 2018-02-22T03:02:14.091Z Reads: 69

```
You can check for internal resistance with a multimeter. Other than that I don't see how you can test a motor without power
```

---
## \#6 Posted by: MysticalDork Posted at: 2018-02-22T03:04:23.119Z Reads: 67

```
To test if the windings are shorted, spin the motor and see if it spins freely. Short two of the three wires, and it should become harder to turn and "cog" as it turns. Repeat with the other combinations of wires.

Then, short all three and it should be VERY hard to turn and smooth.
```

---
## \#7 Posted by: Bensaida Posted at: 2018-02-22T03:05:17.556Z Reads: 63

```
by short, do you mean i have to cut open the phase wires?
```

---
## \#8 Posted by: Apolo Posted at: 2018-02-22T03:05:49.797Z Reads: 55

```
Just touch the connectors together
```

---
## \#9 Posted by: Bensaida Posted at: 2018-02-22T03:07:59.346Z Reads: 54

```
ok thanks.
```

---
## \#10 Posted by: Bensaida Posted at: 2018-02-22T03:58:32.259Z Reads: 54

```
[quote="MysticalDork, post:6, topic:47105, full:true"]
To test if the windings are shorted, spin the motor and see if it spins freely. Shirt two of the three wires, and it should become harder to turn and “cog” as it turns. Repeat with the other combinations of wires.

Then, short all three and it should be VERY hard to turn and smooth.
[/quote]


how would i know if something is wrong? @MysticalDork
```

---
## \#11 Posted by: Namasaki Posted at: 2018-02-23T00:43:24.888Z Reads: 37

```
If the motors do not become harder to spin with 2 phase wires shorted together, then one of the wires is open or in other words, disconnected or the connector on the end of the phase wire has a cold solder joint.
If the motors do not spin freely when the phase wires are not touching, then there is a short in the motor.
```

---
## \#12 Posted by: pat.speed Posted at: 2018-02-23T01:21:53.429Z Reads: 32

```
You could also make a basic esc circuit to test it on the bench. I saw a video on yt about it, It seemed pretty simple
```

---
