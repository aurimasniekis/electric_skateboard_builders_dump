# Issue with dual vesc not working

### Replies: 18 Views: 1837

## \#1 Posted by: evoheyax Posted at: 2016-03-11T17:30:18.067Z Reads: 126

```
I finally received my space cell, so time to move forward. I soldered wires between the vesc's as specified by @onloop. my setting changes are as follows:

master: id 0
slave: id: 1, enable multi esc over can, enable send status over can

only master vescs motor spins...

This could be related to the masters servo outputting 3.2 volts instead of 5, but I want to see if there's anything else I could be doing wrong. Thank you.
```

---
## \#2 Posted by: EnertionSupport Posted at: 2016-03-11T18:10:47.798Z Reads: 125

```
The issue may be more discrete than something we can infer from your given information.

May I suggest you post a picture of your VESC's, and maybe even a couple screenshots of the BLDC tool? 

This should help us to get to the bottom of this faster.
```

---
## \#3 Posted by: trbt555 Posted at: 2016-03-11T18:18:25.719Z Reads: 117

```
You need to enable multiple vesc over can in the master, not in the slave.
The master needs to know it has to control a slave.
```

---
## \#4 Posted by: onloop Posted at: 2016-03-12T00:09:46.040Z Reads: 112

```
[quote="evoheyax, post:1, topic:1770"]
master: id 0
slave: id: 1,
[/quote]

multiple esc over can is already setup as default in firmware, all you should do is change the master ID to 1. (do nothing else) then it will work.

But if you already changed slave to 1 its now backwards.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-03-16T00:21:44.198Z Reads: 88

```
@onloop @trbt555
switching id's and enabling multiple vescs over can on master worked.

However, now I have weird behavior from your remote @onloop

When I press forward nothing happens, when I pull back to brake, it goes to full speed and stays there.

I have ppm setup on the master and no app setup on the slave vesc.

Here's my settings for master:
<img src="/uploads/db1493/original/2X/3/3431f44bc48e9892d5fee53635e08ef18c7caeb9.png" width="690" height="353">
```

---
## \#6 Posted by: onloop Posted at: 2016-03-16T00:26:52.635Z Reads: 82

```
show me your "GENERAL" tab
```

---
## \#7 Posted by: evoheyax Posted at: 2016-03-16T00:29:02.514Z Reads: 79

```
<img src="/uploads/db1493/original/2X/6/6af8a803bc80fe8809b612169100a650fec0be92.png" width="690" height="353">
```

---
## \#8 Posted by: onloop Posted at: 2016-03-16T00:30:10.393Z Reads: 75

```
did you click "read configuration"


is this your master? you should select "Send status over  CAN"
```

---
## \#9 Posted by: evoheyax Posted at: 2016-03-16T00:31:36.179Z Reads: 73

```
yes, clicked read config on the master and took that screen shot.

On the slave, I have no app selected and send status over CAN. other wise, is the same.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-03-16T00:32:45.978Z Reads: 72

```
It also stopped working with my FS-GT2, which was working before I setup the dual motors.
```

---
## \#11 Posted by: onloop Posted at: 2016-03-16T00:32:51.269Z Reads: 72

```

Maybe try selecting PPM on slave too. I can remember if it's required or not... but that's how mine are normally setup.
```

---
## \#12 Posted by: onloop Posted at: 2016-03-16T00:34:19.432Z Reads: 72

```
My advice with Dual VESC, set the BLDC tool up identical on both VESC. all settings the same. Then simply enable send status over can & multiple ESC over CAN & make sure they have different ID's
```

---
## \#13 Posted by: evoheyax Posted at: 2016-03-16T00:43:14.556Z Reads: 68

```
I double checked all settings, changed the no app to ppm, and they are now the same seting wise besides the sends status over can and enable ESC of can. Same behavior.
```

---
## \#14 Posted by: onloop Posted at: 2016-03-16T01:06:58.028Z Reads: 67

```

do both VESC work independently?
```

---
## \#15 Posted by: trbt555 Posted at: 2016-03-16T05:56:34.097Z Reads: 67

```
What are the pulsewidths you're getting when you click "display" and go to full throttle and full brake ? You can read them in the display box next to the moving blue bar.
And what is the blue bar doing ?
```

---
## \#16 Posted by: evoheyax Posted at: 2016-03-16T17:13:34.849Z Reads: 60

```
One works fine, the other has an issue with the servo power pin supplying 3.2 volts instead of 5. I bought both of them from you and this is my first time using them. Powering them with a regulated power supply.

@trbt555 Its hard to check them because it goes straight to full speed when I hit the brakes. Looking at the bar, I need to adjust the values a bit, as it goes full blue before I hit full throttle, but goes less then half way when I hit the brakes. So it need to adjust them, but I can't imagine that causing any problems. My other controller was working with the one vesc that was working, but is now not working at all. (pulse bar does not move, despite receiver lighting up)
```

---
## \#17 Posted by: trbt555 Posted at: 2016-03-16T18:30:00.341Z Reads: 59

```
So the problem with the remote only occurs when you connect the slave which had the 5v problem. Is that correct ?
```

---
## \#18 Posted by: evoheyax Posted at: 2016-03-18T20:06:58.299Z Reads: 59

```
it seems that everything had to do with the pulsewidth settings. editing the start to 1.20 and stop to 2.00 makes the controller work as it should.

Thanks for the help guys. Now, I need to find the right pulsewidth settings... 1.2 to 2 is too quick of an acceleration.
```

---
