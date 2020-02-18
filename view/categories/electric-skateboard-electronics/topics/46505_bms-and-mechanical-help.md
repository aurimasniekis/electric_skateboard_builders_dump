# BMS and Mechanical help

### Replies: 4 Views: 429

## \#1 Posted by: A-lone-tenno Posted at: 2018-02-15T18:19:48.529Z Reads: 65

```
Hi
I am building a 12s dual (tb) 190kv motors, 2 6s lipos. 
I have a couple problems, and I would really appreciate some help. I've been searching for an answer, but I can't seem to find a straight one. Obviously there are many ways to build a board (canbus, 2 recievers, bypass bms, not bypassing) and while Ive figured how i want to build it, I now cant find explanations on how to actually do it. but enough with the rant:
Problem 1:
![image|666x500](upload://gcZnfppyW57ThROJP6D1BpFDKOt.jpg)
I understand where the canbus wire goes, but the receiver has different sized pins, from the vesc, and i don't understand which pin connects to which, this might be common knowledge but if someone could link a picture of the connection between a nano-x receiver and a focbox, that would be great.
problem 2:
![image|666x500](upload://3cFap0frotxDtQgcf0W2zhMhUAT.jpg)
3 phase wires, connect to the vesc, and if it spins in reverse, just switch 2 and it'll work, but the vesc female is smaller (3.5 mm i think?) than the motor (5.5mm) and if someone could link a connector/converter, that would be really great, because I cant really find one, but the more serious problem is the sensor wire, the pins just aren't the same size, and I have no idea how to connect the two... if someone has a spare converter that they wants too sell, or maybe just knows the type/size of the pins because i cant find them on enertions site.
problem 3:
![image|666x500](upload://hHAPa26nOSetoPzKZup3NCkxWk6.jpg)
BMS. I've looked for wiring diagrams and explanations, but was having trouble understanding them... I understand the white wires, and am probably just gong to cut off the plastic on the battery balance wires, and i will solder them to the white wires (no problem right?), but my problem is the bms. I dont want to bypass, i want it to also discharge, so can someone please explain to me which wire goes where? 
![Screenshot (32)|690x202](upload://7mX2C9tOgU5doKQjsUJu2DyJbCj.png)
I have this photo, which might make all of problem 3 pointless, but the vescs go in the load slot, and this a discharge also scheme?
I really have done my research and if someone has links/the connectors and is willing to sell/explain that would be great. ill be in the US from the 22 till march 4th. Thank you for all the help until now, I plan on opening a build thread the second everything connects. 
Sorry for rambling...

edits: some grammar mistakes
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-15T18:24:43.751Z Reads: 56

```
1. the canbus wire DOES NOT plug into the receiver, the PPM cable plugs into the receiver 
2. adapters dont really exist, buy some connectors and solder it yourself
3. sensor cables need an adapter, search “sensor plug” and click the first result
```

---
## \#3 Posted by: A-lone-tenno Posted at: 2018-02-15T18:27:41.081Z Reads: 52

```
yeah, the canbus is between the vescs, i meant which pins connect to which from the master vesc to the receiver.
Can i just cut off the phase wire connectors on both sides and just solder the 2 together/connect an xt-90s?
```

---
## \#4 Posted by: MysticalDork Posted at: 2018-02-15T19:13:40.690Z Reads: 41

```
Regarding the RX input, have a look at this picture: http://www.electric-skateboard.builders/uploads/db1493/original/2X/a/a86bd0202f208651b56d2d4dd1cb653c379d55b8.png

You can buy bullet connectors on Amazon, Hobby King, eBay and other places to connect your phase wires. You can directly solder them, but that can be a pain in the long run.
```

---
