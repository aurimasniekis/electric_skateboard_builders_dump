# How do I connect a 2-wire BMS for charging only?

### Replies: 3 Views: 879

## \#1 Posted by: motiuridentity Posted at: 2017-02-20T04:17:05.954Z Reads: 114

```
I built a 10S5P Liion battery. Bought a 10S 50A BMS that I want to use for CHARGING ONLY. I plan to have a switch that swaps the connection between BMS and VESC. I want to know how to wire the BMS since I am unsure. Here is an image:  <img src="/uploads/db1493/original/3X/a/c/ac50332de627e4d91834f409bca9eb9367f5f32a.JPG" width="674" height="500"> 

There is a B- and P-. Which wires do I connect to these?

EDIT: I already soldered the balance cables on the battery and understand how to connect them.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-02-21T03:56:26.086Z Reads: 87

```
Generally B- is going to go to the negative terminal of your battery pack and P- will go to your charging port.
```

---
## \#3 Posted by: jaykup Posted at: 2017-02-21T16:43:12.402Z Reads: 65

```
^Agree

So 3 plugs: 

**A charge/input plug** 
* Battery negative running into the BMS B- 
* Charge plug negative running into the BMS P-
* Charge plug positive direct from plug to battery

**A power/output plug** 
* positive and negative direct to the battery to supply a ESC/Motor

**A 10 pin/wire BMS plug**
```

---
