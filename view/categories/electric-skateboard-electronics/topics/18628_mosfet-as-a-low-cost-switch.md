# Mosfet as a low cost switch?

### Replies: 11 Views: 1293

## \#1 Posted by: anoop54 Posted at: 2017-03-06T05:28:06.128Z Reads: 109

```
Hey I was wondering why no one has used a mosfet plus voltage divider to create a low cost switch? Im not 100% on how non ideal mosfets work so Im most likely wrong if so can anyone explain why? My plan was to use a voltage divider or buck converter to get the VGs required for saturation. Then put a simple low voltage switch at the Vgs. 

The reason I am uncertain of this is Im not sure how the mosfet will affect the behavior of the esc, since it'll be adding a small voltage drop in the circuit. 

http://www.jameco.com/z/FQP50N06-Fairchild-Semiconductor-Transistor-MOSFET-N-Channel-60-Volt-50-Amp-3-Pin-3-Tab-TO-220-Rail_785590.html
```

---
## \#2 Posted by: Maxid Posted at: 2017-03-06T05:51:09.543Z Reads: 101

```
The Vedder Anti Spark is a MOSFET switch...
```

---
## \#3 Posted by: anoop54 Posted at: 2017-03-06T10:13:45.557Z Reads: 79

```
No need to be sassy I just got into electric boards so i have no clue what that is
```

---
## \#4 Posted by: Maxid Posted at: 2017-03-06T10:24:14.429Z Reads: 75

```
My post was not meant to be sassy but simply informative. No need for me to write an essay on something that can be described in one sentence. All you needed to know is the term "Vedder anti spark" to get you going in the right direction and find all the information you'll need.
```

---
## \#5 Posted by: lowGuido Posted at: 2017-03-06T11:12:09.810Z Reads: 68

```
[quote="anoop54, post:1, topic:18628"]
Hey I was wondering why no one has used a mosfet plus voltage divider to create a low cost switch?
[/quote]

I'm pretty sure almost everyone does use a MOSFET switch.
```

---
## \#6 Posted by: IsTalo Posted at: 2017-03-06T20:34:42.143Z Reads: 47

```
Look at this 
http://www.electric-skateboard.builders/t/eboard-mosfet-switch/5738?u=istalo
```

---
## \#7 Posted by: anoop54 Posted at: 2017-03-06T20:44:49.639Z Reads: 44

```
People we're using circuit breakers and relays, so i thought maybe something was wrong with using a mosfet. Thank you!
```

---
## \#8 Posted by: anoop54 Posted at: 2017-03-06T20:45:04.974Z Reads: 45

```
I understand! Thanks man appreciate it
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-03-06T22:08:50.163Z Reads: 37

```
Hey @anoop54 just read through your thread and that's a  great question. As you may be aware there are a lot of people selling MOSFET switches (including me) but none of them are really under $30 and that's for a good reason, it's a pain in the ass. By that I mean that pretty much all the people who sell the switches build and solder them there selves and, it's not easy as I've learned. They really only cost, at least for me, ~$15 in components, but the testing and soldering and the time it takes is the reason there expensive. You could for much less build your own switch, but most people don't want to do that because they don't know how or don't trust themselves to do so.

Moving on, about your idea of using a voltage divider or regulator to drive the ~10V VGS of most FET's. First of all, there's no need to use a voltage divider for the insanely small amount of current the VGS requires to be saturated. Next is why not to use a voltage divider as I use to do. The main reason is that the voltage output changes with the change in the source voltage, by that I mean if your using a divider to get 10V at 24V(6S) when someone is then using like 50V(12S) the output will be totally different and could destroy the FET. What I recommend you do is use a 12V Zener diode like I use to get a constant 12V for the VGS, no matter the input voltage (as long as it's above 12V obviously). And then about the switch on the VGS, well that's exactly what most people do including me lol. 

Anyways I hope that cleared up your confusion on the topic and if you've got any more questions, let me know!

P.S. I use 12V for the VGS because I like to keep it a little above 10V to make sure the FET is fully saturated, and usually FET's have a max VGS of 20V.
```

---
## \#10 Posted by: lowGuido Posted at: 2017-03-06T22:09:32.630Z Reads: 36

```
there are a few different options. circuit breakers and loop keys are cheaper than MOSFETS, but most people like the MOSFET switches
```

---
## \#11 Posted by: JdogAwesome Posted at: 2017-03-06T22:11:27.981Z Reads: 33

```
Oh and also the MOSFET you linked is complete trash lol, at least for this application. Oh and also the "current rating" of a MOSFET means jack shit FYI. Like the leads of a TO-220 package FET will melt at like 70A so yeah.
```

---
