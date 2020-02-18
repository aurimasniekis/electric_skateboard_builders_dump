# How to connect - Two 5s to 10s (balance wires)

### Replies: 11 Views: 1436

## \#1 Posted by: vishal_tejwani Posted at: 2018-01-02T06:01:03.468Z Reads: 152

```
I searched on forum didn't find a perfect answer,

Can anyone help with the diagram, i have two 5lipos

Want to connect them with 10sbms 

Talking about balance wires here
```

---
## \#2 Posted by: E1Allen Posted at: 2018-01-02T06:04:29.740Z Reads: 147

```
http://www.electric-skateboard.builders/t/is-this-bms-diagram-right/21994

Search BMS lipo diagram. The answer is out there already.
```

---
## \#3 Posted by: vishal_tejwani Posted at: 2018-01-02T06:15:35.325Z Reads: 135

```
Was talking about balance wires connection, i edited the topic title now
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2018-01-02T13:42:44.498Z Reads: 119

```
Otherwise pretty straightforward, but you need to connect the bottom battery's top balance wire to top battery's bottom balance wire.
<img src="/uploads/db1493/original/3X/3/c/3cd00fe8cccf00dd393ad8063094d69f32e0e5db.png" width="512" height="500">
```

---
## \#5 Posted by: vishal_tejwani Posted at: 2018-01-02T15:31:30.738Z Reads: 107

```
Thanks that worked perfectly!<img src="/uploads/db1493/original/3X/b/e/befbb924c7f4dd08716383edb7558d6ca08480c5.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/d/adb5525a209dada2381b03f364fc603276228d97.jpg" width="374" height="500">
```

---
## \#6 Posted by: jmasta Posted at: 2018-01-02T16:25:08.502Z Reads: 98

```
The above diagram is technically correct but can cause problems.  There is no need to connect both balance leads to the center pin.  Your batteries are already wired in series through the main power leads.  If you mix up the balance leads, you are going to short out a battery

This is better:

<img src="/uploads/db1493/original/3X/7/8/782ff289069542c5a6c42c33f1c25047664e83c2.jpg" width="512" height="500">
```

---
## \#7 Posted by: vishal_tejwani Posted at: 2018-01-02T17:19:59.028Z Reads: 89

```
I did short a Balance lead just for mili sec then understood why and changed the connections.

Thanks for your help guys
```

---
## \#8 Posted by: Namasaki Posted at: 2018-01-02T22:29:14.905Z Reads: 84

```
Does your BMS use 10 or 11 balance wires. 
Most use 10 some use 11
```

---
## \#9 Posted by: vishal_tejwani Posted at: 2018-01-03T04:34:41.223Z Reads: 79

```
11 wires although Never came across a bms with 10 wires
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2018-01-03T06:19:51.533Z Reads: 77

```
I personally have used li-ion battery cell monitors that support up to 12S that you just plug the balance lead into and it shows all the cell voltages and their min and max voltages during use. In that case you need the balance lead wired as I first indicated, but as you said and I agree it is better in this case to leave the center pin just connected to just one side in case you series connect the batteries incorrectly.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-01-03T12:53:21.670Z Reads: 66

```
Bestech and Battery Supports both use 10. 
They are the 2 top brands.
```

---
