# VESC noob: what&rsquo;s the (edit) capacitor for?

### Replies: 9 Views: 3640

## \#1 Posted by: trbt555 Posted at: 2015-10-29T09:20:48.525Z Reads: 210

```
Hi guys,
VESC noob here.
What is the CAPACITOR on the input wires for ? Does it come with the VESC or will I need to choose one according to my setup ? How do I choose the size of the condensator ?

Thanks,
Tom
```

---
## \#2 Posted by: onloop Posted at: 2015-10-29T10:55:34.778Z Reads: 211

```
Do you mean the Capacitor?

The VESC i make has the capacitors included. there are three of them mounted onto a small PCB. Between 1000-2000uf is ok.

What does it do? it helps supply instant burst of power to the ESC which can be a problem if the battery is to far away.

<img src='/uploads/db1493/original/1X/f17e3dc0fb10bc716e247405edc8cca671429a20.jpg'>
```

---
## \#3 Posted by: trbt555 Posted at: 2015-10-29T11:23:57.823Z Reads: 202

```
The capacitor of course. I clearly wasn't awake when I wrote this post....
```

---
## \#4 Posted by: longhairedboy Posted at: 2015-10-29T12:11:04.515Z Reads: 202

```
How short would the battery leads need to be to not require those capacitors?
```

---
## \#5 Posted by: treenutter Posted at: 2015-10-29T14:26:19.102Z Reads: 205

```
Good question @longhairedboy. I've wondered the same thing since my vesc is about 6cm from my battery series.
```

---
## \#6 Posted by: trbt555 Posted at: 2015-10-29T15:17:52.474Z Reads: 203

```
@onloop thanks for clarifying, but I was looking for a more scientific insight.

Inquisitive as I am, I've gone ahead and Googled this and read up extensively. 
Apparently the capacitor is there to smooth out ripples in the input voltage.

Some very relevant pages:

 - [Explanation of the Brushless Motor / ESC System and Capacitor Function][1]
 - [Too long battery wires will kill ESC over time: precautions, solutions & workarounds][2]
 - [ESC capacitors.  What do they do?][3]

  [1]: https://traxxas.com/forums/showthread.php?8958604-Explanation-of-the-Brushless-Motor-ESC-System-and-Capacitor-Function
  [2]: http://www.rcgroups.com/forums/showthread.php?t=952523
  [3]: http://www.rcgroups.com/forums/showthread.php?t=975333
```

---
## \#7 Posted by: longhairedboy Posted at: 2015-10-29T16:01:31.792Z Reads: 199

```
That makes a lot more sense. I'm familiar with power conditioning, and that's what it looked like to me.
```

---
## \#8 Posted by: onloop Posted at: 2015-10-30T00:06:42.270Z Reads: 193

```
Nice work @trbt555 Google is our friend... yeah i'm not the best person to explain electrickery mumbo jumbo...  18months ago i didn't even know what an ESC was..  all i know is the VESC feels amazing when riding..

I'm mostly a skateboarder!
```

---
## \#9 Posted by: Pato Posted at: 2015-10-30T06:05:09.069Z Reads: 185

```
Yeah the cap (or caps in this case) are DC link capacitors.

They act as a filter for your noisey non smooth supply (Battery, power grid). They are more necessary in AC to 'whatever' converters (where supply is AC). But still useful to make a good BLDC controller when you have long wires etc.
```

---
