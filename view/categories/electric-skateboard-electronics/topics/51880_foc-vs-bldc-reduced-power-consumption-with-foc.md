# FOC Vs. BLDC - reduced power consumption with FOC?

### Replies: 5 Views: 923

## \#1 Posted by: Acidfie Posted at: 2018-04-10T21:48:25.222Z Reads: 234

```
So i just stumbled upon this:

* https://www.eetimes.com/document.asp?doc_id=1274013
* https://www.roboteq.com/index.php/applications/100-how-to/359-field-oriented-control-foc-made-ultra-simple



Can anyone make a statement about these articles?

Also, does anyone know about Direct Torque Control and if it can get omplemented?
```

---
## \#2 Posted by: Blitz Posted at: 2018-04-10T22:37:35.619Z Reads: 225

```
Maybe a simple Test, single motor 10s Bluetooth module. First in BLDC then FOC.
```

---
## \#3 Posted by: Acidfie Posted at: 2018-04-11T06:09:54.548Z Reads: 182

```
I am not going FOC in the next weeks
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2018-04-11T09:36:39.192Z Reads: 158

```
DTC is just a different flavor of vector control in relation to FOC, but is more tricky to implement, as far as I understand and is the reason why FOC is the more commonly used method.

> Although the vector control algorithm is more complicated than the Direct Torque Control (DTC), the algorithm is not needed to be calculated as frequently as the DTC algorithm. Also the current sensors need not be the best in the market. Thus the cost of the processor and other control hardware is lower making it suitable for applications where the ultimate performance of DTC is not required.

![image|690x291](upload://jlyHz9d0sWn86dLwEifxG8N7Hcz.png)
https://en.wikipedia.org/wiki/Vector_control_(motor)
```

---
## \#5 Posted by: linsus Posted at: 2018-04-11T09:55:34.267Z Reads: 134

```
Everytime BV tried to tutor me about FOC he said that the reduction of power losses in BLDC vs. FOC exist but are very small. Meaning the EFFICIENCY of FOC is higher. I interpet that into more watts are used to the motor instead of turning into heat. If this is even meassurable @ momentarly consumption in an eskate application. is very hard to tell.
```

---
