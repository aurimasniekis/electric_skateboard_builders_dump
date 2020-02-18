# Are exposed motor wires coated?

### Replies: 5 Views: 401

## \#1 Posted by: chewydinosaurs Posted at: 2017-06-02T01:02:12.463Z Reads: 113

```
Alright so I needed to extend my wires coming from the motor (they're called sensor wires right?), so what I did and this may totally be my fault as I didn't know but I cut the wires coming from the motor and soldered longer leads on to them. Well this it where sh$t hits the fan, my motor kind of jumps but wont speed up or really even complete a full rotation when I give it throttle, it just sorts of jerks. So I checked all my leads and wires for continuity and they all checked out alright. What I found out was that even though my leads were soldered to the motor wires, there was no signal passing through the motor wire end. I checked this with a continuity meter and the only way for me to get the signal to pass through is if I individually connect each copper strand end from the motor wire to the wire I was extending it with. Soldering doesn't work, laying them on top of each other side by side doesn't work. SO this leads me to believe that on the exposed copper wire from the motor, there is some sort of nonconductive coating, otherwise there were be continuity through the whole wire. And this would explain why when I solder the wires and hold them together that nothing works. Do I just need a new motor at this point? I'm not sure I have the patience to really deal with this.
```

---
## \#2 Posted by: psychotiller Posted at: 2017-06-02T01:12:50.416Z Reads: 107

```
The 3 thick motor wires are called phase wires. The smaller group of wires with a plug on them are senser wires. If you have a vesc and your motor is sensored, whenever you make changes, such as soldering motor wires, you need to run motor detection again.
```

---
## \#3 Posted by: chewydinosaurs Posted at: 2017-06-02T01:41:47.327Z Reads: 99

```
Oh ok phase wires, no what I mean is that I cant even get the motor to spin at all. I only can if I individually connect the end of each strand of the copper phase wire to each strand end of the copper 'donor' wire which is extending it. It's like the exposed copper on the phase wire isn't conductive on any of it's surfaces except for the tips? Obviously I'm not about to try and connect each tip of the wire to the other wire's tips and hope they hold through hot glue since soldering doesn't do anything in this case.
```

---
## \#4 Posted by: psychotiller Posted at: 2017-06-02T02:18:22.025Z Reads: 83

```
Use flux and put the tips together. Then heat shrink them and call it a day. Take your time.
```

---
## \#5 Posted by: TranxFu Posted at: 2017-06-02T10:08:22.846Z Reads: 55

```
The phase wires which comes out of the motor can are enamel coated most of the time. There are couple videos on this board and on youtube on how to remove it. Solder it on again and reinforce with shrink tube. You might have to open up the motor which is no big deal :)
```

---
