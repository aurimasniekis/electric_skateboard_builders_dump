# Under_Voltage problem Dead bms?

### Replies: 6 Views: 125

## \#1 Posted by: Zyb Posted at: 2018-09-28T17:26:59.623Z Reads: 39

```
hey guys, i get this fault with 10s @ 36V in focbox. when i apply acceleration motors spin for 1 second and then it stops and red light starts blinking couple of times and then i can apply acceleration same thing over and over again. i checked the pack voltage its around 36V up until the vesc. then i tried measuring the voltage while applying acceleration and like vesc reported voltage almost instantly drops from 36v to around 0 my multimeter cant even register the drop because it all happens too fast. im using supower bms do you guys think is dead or i should look somewhere else? my setup is like this battery - bms - vedders antispark- focbox
oh and btw when i plug in the charger led doesnt wanna go from green to red. plug reports 36v aswell so i think connection is good.
```

---
## \#2 Posted by: Lumaci Posted at: 2018-09-28T17:35:18.191Z Reads: 36

```
You could try to bypass the BMS and see.
```

---
## \#3 Posted by: Zyb Posted at: 2018-09-28T17:36:21.803Z Reads: 37

```
exactly what i was thinking gonna do that right now and see how it behaves. thanks
```

---
## \#4 Posted by: Zyb Posted at: 2018-09-28T18:14:54.145Z Reads: 34

```
every single part is ok. i just tapped on the first P group and magically everything started to work. so its basically a loose connection gonna have more info after i open the heatshrink
```

---
## \#5 Posted by: Andy87 Posted at: 2018-09-28T18:17:11.625Z Reads: 29

```
I had once similar problem.
Was the xt90 I didn’t plugged in 100%.
```

---
## \#6 Posted by: Zyb Posted at: 2018-09-28T18:35:59.383Z Reads: 26

```
Found the problem, one of the serial connections is ripped prob due to vibration. I’m lucky it didn’t catch a fire I can see how battery pcb or similar connections style would have helped in this situation. Definitely going to convert it to similar style.
```

---
