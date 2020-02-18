# Water cooling through Vesc 5V Output

### Replies: 5 Views: 1089

## \#1 Posted by: danielogic Posted at: 2017-03-02T10:03:58.112Z Reads: 165

```
Hi everybody,

I am trying to unterstand the electronics commonly used on an esk8. So i figured out how to connect everything proper to have a "safe" circuit. 

As u know our Motor converts electrical into mechanical energy. So the "drive forces"  are continiously interacting with our electrical system. While accelerating and on steep hills these driving resistors are dominant so that we need much torque to overcome them. And we further know that torque is proportional to the drawn current. The energy losses (and so the heat) are square relatet to the current. So if we need more torque the efficiency decreases and our system could overheat. Heat in turn weakens our motor so that we have less power and less torque on demand.

I thought if someone lives in a hilly area or wants to build a mountainboard, water cooling could be interesting. Because these boards operate less often with high efficiency than boards made for flat streets. 

So now my question: is it possible to use the 5v output of the drv8302 to power a 3v motor (water pump)? Maybe controlled by a simple potentiometer to set the number of revolutions?
And if, could someone help me with the circuit? 

Thank you, I will appreciate every answer
```

---
## \#2 Posted by: Journ Posted at: 2017-03-02T11:40:52.848Z Reads: 142

```
https://www.youtube.com/results?search_query=electric+motor+cooling+system maybe some answers here^
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-03-02T11:58:45.420Z Reads: 132

```
It depends on how much amps the water pump needs at stall. Because the 5V pin on the VESC is good for 2A as far as i know. The best would be if you have a DC-DC step down from your batterys voltage to the voltage of the water pump.
Could be a interesting cooling method for EMTB.
```

---
## \#4 Posted by: hexakopter Posted at: 2017-03-02T13:49:37.413Z Reads: 108

```
[quote="Ackmaniac, post:3, topic:18443"]
Because the 5V pin on the VESC is good for 2A as far as i know.
[/quote]


The 2A value isn't correct in my opinion. The data sheet says that the DRV8302 is good for 1.5A. But don't forget that also the LDO for 3.3V and other sources uses this 5v. So for a safety reason I wouldn't go over 1A.
```

---
## \#5 Posted by: rpn314 Posted at: 2017-03-04T13:45:17.726Z Reads: 68

```
[quote="hexakopter, post:4, topic:18443"]
The 2A value isn't correct in my opinion. The data sheet says that the DRV8302 is good for 1.5A. But don't forget that also the LDO for 3.3V and other sources uses this 5v. So for a safety reason I wouldn't go over 1A.
[/quote]

Agreed. Vedder's original post cites 5V 1A, so that what I would stick to.

"5V 1A output for external electronics from the buck converter integrated on the DRV8302"
Source : http://vedder.se/2015/01/vesc-open-source-esc/
```

---
