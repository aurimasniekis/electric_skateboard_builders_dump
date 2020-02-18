# 5V 1A output for external electronics?

### Replies: 5 Views: 1350

## \#1 Posted by: alindaniel93 Posted at: 2017-02-04T15:05:15.257Z Reads: 144

```
so on the www.vesc.net.au site where is the description of the VESC (copy and paste it down below) 
"DRV8302 MOSFET driver / buck converter / current shunt amplifier.
IRFS7530 MOEFETs (other FETs in the same package also fit).
5V 1A output for external electronics from the buck converter integrated on the DRV8302."
they say that there is allready a place where I can get power for external devices...
Can anyone show me and help me with? I don't know what and where is the buck converter...
I have 2 LiPo Hight voltage 4s batteris in series (17.40v each battery to a total of 34.80v) and I wanna put led stripes under.
I don't want to have a separate pack of battery so then I need to charge or change that too...
```

---
## \#2 Posted by: jmasta Posted at: 2017-02-04T19:23:00.582Z Reads: 129

```
The 5V source is embedded in the 3-pin servo cable that goes from your VESC to your receiver.  (This is how the receiver gets its power).  Center pin is 5V.  Pin closest to edge is ground, as marked on the board by GND.

You just need to make an adapter, or splice the 5V and GND wires to add a parallel connection for your 5V accessories.

Or buy an external BEC capable of accepting the full pack voltage. Personally I use a 12V BEC instead of tapping 5V from the VESC
```

---
## \#3 Posted by: saul Posted at: 2017-02-05T05:04:59.623Z Reads: 112

```
yes the vesc has internal 5v output at the servo and uart pins.

I would keep some saftey room so I limit my lights to about 800ma max.
the tx and system use some of this power and if you draw too much you can burn out the drv.... :frowning:

I'm putting the last touches on my light kit that has brake and ch1 control for signals or headlights 
http://www.electric-skateboard.builders/t/brake-lights-and-turn-signals-finally-for-any-esc/15888/
```

---
## \#4 Posted by: alindaniel93 Posted at: 2017-02-05T07:40:34.048Z Reads: 89

```
Ok, but I think I will put just 60 centimeters of a led stripe. Not too much. I think that this will not drain too much. And take the current from the uart so I won't mess up with the reciever. Is this way OK?
```

---
## \#5 Posted by: alindaniel93 Posted at: 2017-02-05T07:44:18.479Z Reads: 85

```
Didn't  the bec get too hot?
```

---
