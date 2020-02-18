# Is this BMS wiring correct?

### Replies: 43 Views: 360

## \#1 Posted by: Jcullinan09 Posted at: 2018-09-28T03:27:05.482Z Reads: 83

```
Hey guys,

I'm getting really close to finishing my 10s5p battery pack with a BMS this BMS HCX-D223V1 (https://buildkitboards.com/collections/batteries/products/bestech-bms?variant=7201537687582) 

I have just about everything setup, but whenever I am trying to draw load from the battery pack I am only getting 3.0 volts. When my pack end to end simply reads 40 volts. 

I think the problem is the wiring of my BMS could an experienced battery builder verify my wiring? 
Thank you!
![39%20PM|461x500](upload://xR7UsBdEDPbqsGhYDmw6n4K78Nv.jpeg)
```

---
## \#2 Posted by: hyperIon1 Posted at: 2018-09-28T03:30:41.243Z Reads: 72

```
do you have the E-SWITCH  connected?
```

---
## \#3 Posted by: Namasaki Posted at: 2018-09-28T03:32:13.980Z Reads: 68

```
Where are de balance wires?
```

---
## \#4 Posted by: Jcullinan09 Posted at: 2018-09-28T03:32:19.570Z Reads: 70

```
@hyperIon1 I do not. Right now its just got electrical tape wrapped around it. How should I connect it?
```

---
## \#5 Posted by: Jcullinan09 Posted at: 2018-09-28T03:33:55.492Z Reads: 68

```
@Namasaki I will find an image that shows how I wired the balance wires, but would that have an effect on the voltage being drawn from the pack?
```

---
## \#6 Posted by: Namasaki Posted at: 2018-09-28T03:34:55.474Z Reads: 66

```
If you don't get the balance wires and main wires correct, you will fry the bms.
```

---
## \#7 Posted by: hyperIon1 Posted at: 2018-09-28T03:35:16.810Z Reads: 65

```
if its just two bare unstriped wires the bms should function without the switch. only if a switch is connected does the function work.
once you have it wired as you showed above and your balance leads connected, the bms should function.
and if so you should get a 40v reading at your t90
```

---
## \#8 Posted by: hyperIon1 Posted at: 2018-09-28T03:37:07.392Z Reads: 65

```
yes, disconnect the B- and connect your balance wires in order from 1-10 then reconnect B-
```

---
## \#9 Posted by: Namasaki Posted at: 2018-09-28T03:37:56.025Z Reads: 63

```
[quote="hyperIon1, post:7, topic:69423"]
only if a switch is connected does the function work.
[/quote]


That bms will not turn on unless the wires are connected to activate the built in E-switch.
The E-switch also doubles as a reset switch if the bms shuts down in protection mode so connecting a switch to the wires is necessary.
Also, per Bestech, the bms has to be turned on for charging as well as discharging.
```

---
## \#10 Posted by: hyperIon1 Posted at: 2018-09-28T03:42:18.761Z Reads: 60

```
sorry, I didn't finish what I was getting to on not needing a switch, @Namasaki is correct that the two wires need to be connected, if you are not using a switch at the bms, and you are using a vedder or luna type switch
```

---
## \#11 Posted by: Namasaki Posted at: 2018-09-28T03:47:08.772Z Reads: 61

```
From what I have seen and experienced, the Bestech E-switch is much more reliable that most external E=switches. Unless there is some new super E-switch out that I don't know about.
I've been using my Bestech's for over 2 years without a failure.
```

---
## \#12 Posted by: Jcullinan09 Posted at: 2018-09-28T03:49:50.127Z Reads: 58

```
Sorry guys I prematurely posted without having a diagram of the balance wires. 

![IMG_1382|666x500](upload://3KTJFem4xeYyQI2B97OQ1Ywe0by.jpeg)
```

---
## \#13 Posted by: hyperIon1 Posted at: 2018-09-28T03:50:17.193Z Reads: 57

```
interesting, the issue I have had lately with the e-switch is when powering up a duel esc.
even on the simple rocker switch
```

---
## \#14 Posted by: hyperIon1 Posted at: 2018-09-28T03:52:04.730Z Reads: 52

```
have you seen the push to start mostfet switch?
```

---
## \#15 Posted by: Jcullinan09 Posted at: 2018-09-28T03:53:23.706Z Reads: 47

```
Would this BMS have a push to start mosfet switch?

also,

I am getting a 40 volt reading at my T-90, however when I plug in ESC's i get no power, and only have a 3v reading.
```

---
## \#16 Posted by: hyperIon1 Posted at: 2018-09-28T03:55:45.229Z Reads: 47

```
sorry, no it wouldnt..... thats  a new external switch on the market
```

---
## \#17 Posted by: Jcullinan09 Posted at: 2018-09-28T03:56:07.325Z Reads: 47

```
After the T-90 I put an anti spark switch in https://www.amazon.com/gp/product/B07CMYPZ6Z/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1

And after load runs through it, the voltmeter says 3. Why do you think that might be?
```

---
## \#18 Posted by: hyperIon1 Posted at: 2018-09-28T04:02:38.304Z Reads: 45

```
if everything is wired correctly on the bms and you're getting 40v at t90 it should work unless your switch is bad. 
or pluged in backwards.
```

---
## \#19 Posted by: hyperIon1 Posted at: 2018-09-28T04:03:19.931Z Reads: 47

```
![54%20PM|412x380](upload://hRSxX2aww9jcqyvJM3FOt6Dk9b0.png)
```

---
## \#20 Posted by: Namasaki Posted at: 2018-09-28T04:03:20.938Z Reads: 47

```
the BMS  Built in E-switch has to be on for it to work in discharge and charge
```

---
## \#21 Posted by: Jcullinan09 Posted at: 2018-09-28T04:04:05.478Z Reads: 42

```
I don't think the switch is bad/faulty because once I connect the pack to the ESC's. Not even the ESC's will turn on.
```

---
## \#22 Posted by: hyperIon1 Posted at: 2018-09-28T04:04:56.473Z Reads: 43

```
did you connect the  e switch
```

---
## \#23 Posted by: Jcullinan09 Posted at: 2018-09-28T04:06:15.642Z Reads: 44

```
Nothing is connected to the e-switch on the BMS. should there be two switches?

These wires are loose ![10%20PM|667x500](upload://4rMK0NpmA7P66nHS5KU1XdnqXo2.png)
```

---
## \#24 Posted by: Namasaki Posted at: 2018-09-28T04:07:49.257Z Reads: 41

```
The bms e-switch is not optional
```

---
## \#25 Posted by: Jcullinan09 Posted at: 2018-09-28T04:08:25.874Z Reads: 41

```
How or where do I connect these wires?
```

---
## \#26 Posted by: Namasaki Posted at: 2018-09-28T04:09:12.938Z Reads: 38

```
connect them to a 2 pole 12v automotive on/off switch
use that switch to turn the bms on/off  and to reset it from protection shut down.
```

---
## \#27 Posted by: Jcullinan09 Posted at: 2018-09-28T04:11:28.475Z Reads: 42

```
So I will have two on/off switches one for the BMS, and one for the anti-spark switch? That doesnt seem right?
```

---
## \#28 Posted by: hyperIon1 Posted at: 2018-09-28T04:11:45.091Z Reads: 44

```
you can put a rocker type switch like @Namasaki uses, or bypass by wiring together because you have an external one. 
the bms has a reset function time-delayed if it is tripped so the options are to have the function on/ off with switch or always on wired together. if you just spent 60$ on a luna switch use it
```

---
## \#29 Posted by: Namasaki Posted at: 2018-09-28T04:12:12.282Z Reads: 42

```
You don't need an external anti-spark switch with this bms.
```

---
## \#30 Posted by: hyperIon1 Posted at: 2018-09-28T04:12:58.478Z Reads: 39

```
no one said you did, but he bought one for the pretty led light
```

---
## \#31 Posted by: Jcullinan09 Posted at: 2018-09-28T04:13:42.668Z Reads: 37

```
Lol, well I already spent $60 bucks on it. 
So could I simply just solder the BMS on/off switch? and rely on the anti-spark for my on/off.
```

---
## \#32 Posted by: Namasaki Posted at: 2018-09-28T04:13:55.658Z Reads: 31

```
It's is possible to have a lighted switch with the built in E-switch.

The problem with external E-switches is they are prone to failure from excessive heat cause by the high current passing through them.
```

---
## \#33 Posted by: hyperIon1 Posted at: 2018-09-28T04:14:47.108Z Reads: 34

```
if you use a pushbutton latching 5pin and supply power for led off esc
```

---
## \#34 Posted by: Namasaki Posted at: 2018-09-28T04:15:59.105Z Reads: 33

```
[quote="Jcullinan09, post:31, topic:69423"]
Lol, well I already spent $60 bucks on it.
[/quote]


If I was in your shoes, I would sell it and use the one in the bms.
```

---
## \#35 Posted by: hyperIon1 Posted at: 2018-09-28T04:16:46.144Z Reads: 34

```
true for the old style 2-4 mosfet anti spark switches.  the biggest problem was finding fuses
now they are coming along with improvements
```

---
## \#36 Posted by: Jcullinan09 Posted at: 2018-09-28T04:17:24.577Z Reads: 31

```
I'll probably sell it then. 

But I'm still confused. Can I simply put a two pole, on/off switch to connect the BMS e-switch?
```

---
## \#37 Posted by: Namasaki Posted at: 2018-09-28T04:18:04.681Z Reads: 32

```
[quote="Jcullinan09, post:36, topic:69423"]
But I’m still confused. Can I simply put a two pole, on/off switch to connect the BMS e-switch?
[/quote]


Yes, just a 12v 2 pole on/off switch. 
You can get them at the local auto parts store on online.
```

---
## \#38 Posted by: hyperIon1 Posted at: 2018-09-28T04:18:07.062Z Reads: 34

```
yes, that will do
```

---
## \#39 Posted by: Jcullinan09 Posted at: 2018-09-28T04:20:03.279Z Reads: 37

```
Well sick. Thanks guys. 

I also bought a battery capacity tester to measure voltage, Correct me if I'm wrong, but I could connect that anywhere in the hot wires leaving to the ESC? 
https://www.amazon.com/gp/product/B01LQ7MT4K/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1
```

---
## \#40 Posted by: hyperIon1 Posted at: 2018-09-28T04:21:17.837Z Reads: 35

```
yes anywhere past the e switch because that's an a always-on led
```

---
## \#41 Posted by: Jcullinan09 Posted at: 2018-09-28T04:22:35.138Z Reads: 32

```
Thanks a bunch @hyperIon1 and @Namasaki!
```

---
## \#42 Posted by: Namasaki Posted at: 2018-09-28T04:24:58.665Z Reads: 32

```
Note that you will have to set that meter for your particular number of cells in series to get an accurate percentage.

Personally, I prefer a voltage meter to a percentage meter.
```

---
## \#43 Posted by: Jcullinan09 Posted at: 2018-09-28T04:26:23.590Z Reads: 30

```
Yep, I know. I'll need to set the meter for 10S. But Idk I kinda prefer the percentage display, just comes down to personal preference I guess.
```

---
