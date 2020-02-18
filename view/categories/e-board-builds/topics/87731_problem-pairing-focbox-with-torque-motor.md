# Problem pairing focbox with torque motor

### Replies: 19 Views: 268

## \#1 Posted by: Yannis Posted at: 2019-03-20T11:47:54.582Z Reads: 90

```
Hi to everyone. I am facing a problem pairing the focbox with the 6374 torque motor. The think is that I am not sure if the A, B and C cables of the sensor wire pair with the H1, H2 and H3 inputs of the focbox. Does anyone know?

Thanx
```

---
## \#2 Posted by: meesie Posted at: 2019-03-20T12:04:54.874Z Reads: 83

```
i've got a focbox and torqueboard motor, no problems at all.
what's the first indication of your problem? does the vesc tool throw any errors?
```

---
## \#3 Posted by: Yannis Posted at: 2019-03-20T12:09:45.422Z Reads: 79

```
Not at all. Did you change the wiring before pairing? Or you just plugged the sensor cable to the focbox?
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-03-20T12:21:35.182Z Reads: 76

```
I was under the impression that TB motors They are actually .5mm off. Youll need an adapter like @Battosaii said :+1:  

![image|396x265](upload://3IuIJNasdp8tjVjxCmmxWoa6oJ7.png) 

https://www.electric-skateboard.builders/t/foc-box-hall-sensor-wire-connector-type/48831/2?u=sn4pz

connector link: 
https:///collections/electrical-connectors/products/vesc-sensor-wires
```

---
## \#5 Posted by: Battosaii Posted at: 2019-03-20T12:25:25.673Z Reads: 66

```
Motor sensor wires have never been able to just plug Into a Vesc you have always needed an adapter and the Unity has not changed this. It's a fact of life.
```

---
## \#6 Posted by: Yannis Posted at: 2019-03-20T12:34:27.376Z Reads: 60

```
Thanx. Do I have to change the A C B wires to A B C in order to meet the H1 H2 and H3 inputs of the focbox or it doesn't matter?
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-03-20T12:39:59.635Z Reads: 60

```
The connectors will take care of that for you, no need to switch wires around. 

Its not important to your case, as you shouldnt be re-soldering anything, but ( some )VESC based products will actually be ok with receiving mismatched sensor wires and signals, and actually read which wire is which, allowing it to calibrate itself.
```

---
## \#8 Posted by: Yannis Posted at: 2019-03-20T12:44:03.978Z Reads: 58

```
Thanx a lot
```

---
## \#9 Posted by: Yannis Posted at: 2019-03-20T13:27:52.556Z Reads: 49

```
Also guys I have an one more question  if I may. I bought a switch button with 4 cables from chinese market. Does that goes to the focbox or to the bms?
```

---
## \#10 Posted by: L3chef Posted at: 2019-03-20T13:34:43.599Z Reads: 51

```
Can you upload a pic of the switch? There's no on/off switch on the focbox.You can either have a bms with eswitch. An antispark switch or a loopkey to turn on/off your board
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-03-20T13:36:01.944Z Reads: 49

```
Sounds like an antispark breaker type of switch, like the one that comes with @psychotiller s antisparks🤔
```

---
## \#12 Posted by: Yannis Posted at: 2019-03-20T13:38:05.615Z Reads: 48

```
Οκ guys i ll be back to you with some pictures. Appreciate your help
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-03-20T13:41:10.758Z Reads: 49

```
Please don't connect anything before sending pictures,it's ok to have more pictures rather than cramming things together
```

---
## \#14 Posted by: Yannis Posted at: 2019-03-20T16:58:03.072Z Reads: 38

```
![received_266181400979045|690x388](upload://nJ2xMTObgpIRSVIGidhhKUaUnBT.jpeg)
```

---
## \#15 Posted by: Yannis Posted at: 2019-03-20T16:58:44.788Z Reads: 37

```
![received_1073251062882142|690x388](upload://vpkA02X3HMePgJ4xkPzIW8LQROi.jpeg)
```

---
## \#16 Posted by: Yannis Posted at: 2019-03-20T16:59:40.873Z Reads: 35

```
This is the switch I was talking about
```

---
## \#17 Posted by: Sn4pz Posted at: 2019-03-20T17:00:33.821Z Reads: 37

```
Ah. the diyeboard kit uses proprietary connectors that match their ESC. it would do you good to remove the hot glue from that, buy new switches that would be compatible with the hardware you have and then screw them back in. Not to mention diyeboard buttons have failed if I remember correctly. You dont want to passively drain your entire pack to zilch.

hooray my first solution, thanks. 

Just keep bumping the topic with any more issues you might have and Ill try to keep answering lol
```

---
## \#18 Posted by: Yannis Posted at: 2019-03-20T17:04:13.532Z Reads: 34

```
Got it. Apreciate your support
```

---
## \#19 Posted by: psychotiller Posted at: 2019-03-20T17:53:02.090Z Reads: 33

```
That's not one of our switches.  Ebay?
```

---
