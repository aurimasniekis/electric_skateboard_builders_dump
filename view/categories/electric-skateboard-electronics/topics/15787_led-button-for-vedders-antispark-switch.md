# Led button for Vedder&rsquo;s Antispark Switch

### Replies: 41 Views: 4626

## \#1 Posted by: karma Posted at: 2017-01-08T12:20:31.980Z Reads: 368

```
Hi I am trying to make a antispark switch (Vedders'). I would love to use a [led power button](http://www.ebay.com/itm/16mm-12V-Car-Silver-Aluminum-LED-Power-Push-Button-Metal-ON-OFF-Switch-Latching-/311438581192?hash=item48832f9dc8:g:qKUAAOSwgQ9V6Xl5&autorefresh=true) instead of a rocker. Is this possible without taking power from the vesc?
I can't seem to find what the output voltage is from the switch to the button...
```

---
## \#2 Posted by: okp Posted at: 2017-01-08T12:46:38.598Z Reads: 365

```
what about the 5V from your receiver ?
```

---
## \#3 Posted by: karma Posted at: 2017-01-08T12:59:08.689Z Reads: 358

```
I can take power from my reciever and vesc but just wanted to know if you could do it on the switch. It would be alot easier and more modularised. As an example [Miami Electric Boards](http://miamielectricboards.com/shop-1/120amp-12s-power-switch) has done it. (Though I don't think that is a Vedder Antispark Switch.
```

---
## \#4 Posted by: goldenHusky Posted at: 2017-01-08T15:05:32.355Z Reads: 347

```
[quote="karma, post:1, topic:15787"]
I would love to use a led power button instead of a rocker. Is this possible without taking power from the vesc?
[/quote]

Wanted to do the same, so I changed its schematic and implemented a voltage regulator that supplies the led of the button when the switch is on.
Pcbs and mouser parts will arrive this week (depends if the DHL custom clearance girls have a good day or not) so I'm hopefully able to show the results in a small video very soon!
```

---
## \#5 Posted by: DeathCookies Posted at: 2017-01-08T15:19:12.883Z Reads: 315

```
@goldenHusky So you have modified the vedder switch or made a complete different switch?
```

---
## \#6 Posted by: goldenHusky Posted at: 2017-01-08T15:25:39.163Z Reads: 319

```
I modified the schematic and drew the layout completely new in eagle as I'm not familiar with kicad. Dimensions of the pads and stuff might be slightly different. I also tried to make the main current path on bottom+top layer incl. vias the same or rather improve them.
```

---
## \#7 Posted by: DeathCookies Posted at: 2017-01-08T15:32:36.938Z Reads: 313

```
Just to get this topic on course again:

I have heard from some members that they just used the normal vedder switch and soldered the wires to the + and - of the led.
I have tried this approach without soldering (just holding the wires against the pins) but my led did not shine bright enough. Maybe i just needed to solder it to get a good current flow.... But some people had success.

It would be good if those people could chime in here and tell their story ;)
```

---
## \#8 Posted by: brandon Posted at: 2017-01-08T19:27:22.951Z Reads: 285

```
You could just put an led with the proper resistor on the output of the switch
```

---
## \#9 Posted by: karma Posted at: 2017-01-08T19:30:38.763Z Reads: 283

```
@DeathCookies do you mean that they solderd the led pins on the button to the power leads comming from the battery(e.g 10s - 36V) with a resistor in series?

@goldenHusky Good job man! Would love to see that in action. Will you release the files if it works? :)
```

---
## \#10 Posted by: DeathCookies Posted at: 2017-01-08T19:32:37.425Z Reads: 273

```
No. They just soldered The cables to two of the three soft switch wires.
```

---
## \#11 Posted by: karma Posted at: 2017-01-08T19:33:49.502Z Reads: 275

```
Oh okey, do you know what the supplied voltage is on those?
```

---
## \#12 Posted by: DeathCookies Posted at: 2017-01-08T19:36:20.666Z Reads: 280

```
The soft switch gets 12V from the Power supply. These 12V can be used for the LED. In my case the LED wasnt shining very bright...
```

---
## \#14 Posted by: JdogAwesome Posted at: 2017-01-08T23:11:44.447Z Reads: 287

```
I think everyone is making this way to complex lol. On my EBoard MOSFET switch I just use two 6.8K 1W resistors in parallel to power the LED. What people don't understand is that the LED is still getting 50V (12S LiPo) it's just limiting the current to it. And because the higher the voltage the more current can flow through the resistors so you need a higher value resistor. Check out the schematic below and you can see the two resistors labelled as 4.7K but are actually supposed to be 6.8K that go to a output for the LED in my pushbutton switch.

Red and Black wires in the switch just power the LED inside the switch, black wire is connected to the drain of the MOSFET so that it only turns on when the switch is on. Red wire is connected to the two resistors. And blue and green are just the actual switch terminals, Common and Normally Open (C, NO)
<img src="/uploads/db1493/original/3X/8/8/88783be8e5927c17c82eca8aa90252314421ca11.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/d/4/d4ae9fcf0671fe87009efa66f2843fa6094f88c7.png" width="667" height="499">
```

---
## \#15 Posted by: DeathCookies Posted at: 2017-01-11T01:53:43.569Z Reads: 270

```
Maybe this is an Option:
<img src="/uploads/db1493/original/3X/9/2/9217ac836a4c6be701e7558bb4a3f0cf43def3c8.jpg" width="690" height="387">
```

---
## \#16 Posted by: TheImmortalJew Posted at: 2017-01-11T02:29:32.917Z Reads: 266

```
I was experimenting with one of my switches yesterday to try and get the LED working but no luck. I discovered the NC wire is the ground and the other two have 12V. I don't recall which wire resulted in what, but one of the positive wires made the LED light always lit when on or off...no good. The other wire made the LED light up when ON and turned off when off, but the board no longer turned on...also no good. So I don't know, I'm pretty content with no light as long as the darn thing works. :joy:
```

---
## \#17 Posted by: Eboostin Posted at: 2017-01-11T02:37:37.938Z Reads: 270

```
These are the images I found for how to wire the switch. I haven't attempted yet. Still waiting on a few parts. 

<img src="/uploads/db1493/original/3X/e/1/e14457e235845167e6ba79d799d5b20afbd719fe.jpg" width="450" height="450">

<img src="/uploads/db1493/original/3X/3/4/34f71c143b31bfdcc2cafce47882b2c04c2bba3c.jpg" width="450" height="450">

<img src="/uploads/db1493/original/3X/8/3/836df948898227a52aa21688829037393e7e6239.jpg" width="500" height="500">

<img src="/uploads/db1493/original/3X/8/b/8b3a0345fbc3ed310a216a83236b03b2805fe0a3.jpg" width="500" height="500">
```

---
## \#18 Posted by: 3sly Posted at: 2017-01-13T21:46:55.552Z Reads: 248

```
Hey quick question, I can't measure the resistance of the LED, but I assume it needs about 20mA (as most LEDs). But If I calculate this for 50V I need a 2.5k resistor. Which differs quite a bit from your value. What values did you use?

EDIT: Just found a 14.4V drill battery: the current throught he LED seemed to be 15mA, so the internal resistance is 960ohm. When using a 50V battery (12s liIon + I bump the current through the LED up to 20mA to avoid the led from dimming when the battery is depleted), I should need a 1.5k ohm resistor (1W). But how come you ended up using 6.8k?
```

---
## \#19 Posted by: JdogAwesome Posted at: 2017-01-13T22:06:07.951Z Reads: 252

```
So most LED's have a MAX current of 10-20mA but they can run fine down to just a couple mA with very little change in brightness. Using a 1.5K will work but it will seriously deplete the life of the battery and will make the resistor heat up a lot more. You could run just a mA through the LED and it would still illuminate fine.
```

---
## \#20 Posted by: 3sly Posted at: 2017-01-13T22:08:25.871Z Reads: 242

```
good tip! didn't know that. Thanks man!
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-01-13T23:46:35.727Z Reads: 242

```
Hey when I was first trying to figure out the wiring for the LED Switch I was pretty confused as well. Pretty much the + and - wires are literally just the leads for the LED inside the switch. So if you want the LED to turn on when the switch is on, you need to connect the - LED lead to, for example, the drain of the MOSFET so that when the MOSFET turns on, then the LED turns on, thats what I do in my MOSFET switch. And for the C (common) and NO (normally open) contacts, just use those as the conventional switch contacts.
```

---
## \#22 Posted by: TheImmortalJew Posted at: 2017-01-14T00:19:34.041Z Reads: 230

```
I understand that the + and - power the LED on the switch, I just didn't know where to connect those terminals to on the PCB. I found that the NC pad on the PCB is the - (MOSFET drain?) and the other two pads (C, NO) both have +12V. I tried both combinations to the LED and neither worked right. Maybe the picture DeathCookies posted above might work?
```

---
## \#23 Posted by: DeathCookies Posted at: 2017-01-14T00:21:19.186Z Reads: 243

```
Could you mark in this picture where you have attached + and - ? would be very kind
http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/5/e594848ed3834bdb62218a6d301a8aadfd2dc95a_1_624x500.jpg
```

---
## \#24 Posted by: JdogAwesome Posted at: 2017-01-14T00:44:39.021Z Reads: 238

```
I don't have access to a computer ATM, but I would attach the - of the LED to the bottom right pad, or the MOSFET drain. And the + of the LED you need to connect to the positive rail with an appropriate current limiting resistor, I would use ariund 3-4KOhm resistor.
```

---
## \#25 Posted by: JdogAwesome Posted at: 2017-01-14T00:47:06.214Z Reads: 233

```
You only want the NO teminal connected to the positive rail, or the 12S (50V) of you battery, common connects to the input for that MOSFET gates. The NC pad connects to the MOSFET source, all it does is pull the gate low so that it stays in the off state.
```

---
## \#26 Posted by: 3sly Posted at: 2017-01-28T22:02:25.214Z Reads: 227

```
Hey JdogAwesome,

I'm gonna try to modify the sparkswitch to accept led switches standard. Did I make the modifications correctly? Is that how you explained it. If I'm correct you just connected the plus or minus respectively to the in and output line.

i'm using a 0603 6k 500mW resistor. This should limit the current to 6.666mA on a 50V battery (as the internal resistance of the ledswitch is already 1500ohm).

<img src="/uploads/db1493/original/3X/d/e/de54360c95aeced5a13a5cc27bf87ec9f4cf6391.png" width="690" height="273">
```

---
## \#27 Posted by: JdogAwesome Posted at: 2017-02-01T04:29:00.217Z Reads: 213

```
Hey sorry for the late reply, yeah that should work for powering the LED. Though im curious why there are 6 terminals for the switch? You only really need 4, one for the LED+ one for - and two for the actual switch. I get the 5th terminal for the NC state to pull that gates down, but its unnecessary.
```

---
## \#28 Posted by: goldenHusky Posted at: 2017-02-01T09:49:18.078Z Reads: 207

```
[quote="JdogAwesome, post:27, topic:15787"]
but its unnecessary
[/quote]

It's not. For a safe operation it's crucial that the gates are always on a defined potential. If the gate pad is "in the air" you expose it to the enviroment with all it's interferences which most likely results to a floating voltage level on the gates that can turn your anti spark switch randomly on and off.
```

---
## \#29 Posted by: 3sly Posted at: 2017-02-01T10:28:23.868Z Reads: 202

```
6? You probably meant 5. And yes I can indeed probably combine P8 and P11. But then I'd need to put 2 cables from the LED switch into 1 JST socket and that doesn't seem very orderly.

@goldenHusky: How do you mean? Because the switch used has to always be a spdt, so it doesn't float normally. Or I might be missing your point.
```

---
## \#30 Posted by: goldenHusky Posted at: 2017-02-01T10:42:45.300Z Reads: 200

```
@3sly
 Yea, but @JdogAwesome  thinks using an spdt is unnecessary, so I tried to explain it to him.
```

---
## \#31 Posted by: 3sly Posted at: 2017-02-01T10:46:44.086Z Reads: 214

```
Ah! That explains things. This thing is good to go then, glad to hear. I''ve thrown a design on oshpark already.

To save space I'm placed the 5pin jst on the bottom and use the angled kind.

<img src="/uploads/db1493/original/3X/f/7/f72c67d1ce595e8a998ff852d7e2f5df3a143067.png" width="690" height="256"><img src="/uploads/db1493/original/3X/d/9/d927eafcc36503af4b2b2fa08985f791df99a5cf.png" width="623" height="499"><img src="/uploads/db1493/original/3X/f/a/fa094ab84a8cc6cf3dcb6bbfcc955176813b761b.png" width="623" height="499">
```

---
## \#32 Posted by: JdogAwesome Posted at: 2017-02-01T14:20:23.453Z Reads: 186

```
No it is unnecessary as long as you have a pull down resistor. That's the entire point of a pull down lol.
```

---
## \#33 Posted by: goldenHusky Posted at: 2017-02-01T15:50:53.035Z Reads: 184

```
Yea sure, but there is no pulldown on his pcb. And most led switches are spdt anyway so a pulldown resistor would be nothing but additional cost.
```

---
## \#34 Posted by: JdogAwesome Posted at: 2017-02-01T16:17:55.945Z Reads: 190

```
I was just saying it unnecessary if you add a pull down resistor, should have been more clear about that. And I prefer having as few wires coming off the PCB to the switch as possible, so using a pull down would be simpler. And it would be "nothing but additional cost" yeah of like half a cent lol, resistors cost nothing.
```

---
## \#35 Posted by: mccloed Posted at: 2017-02-01T17:00:28.066Z Reads: 182

```
@3sly Is this in the shared projects? This is just what I've been looking for! Would really like to make some.
```

---
## \#36 Posted by: 3sly Posted at: 2017-02-01T17:33:07.488Z Reads: 187

```
Well, I'd like to make a couple first to see if it's practical and nothing is in the way. That way I can test everything before spreading it out there. I'd make a thread with some pictures of the finished product that way people would get more exited I think. Once I know they work, I'll send them out there as a shared project :smiley:

@goldenHusky @JdogAwesome
```

---
## \#37 Posted by: mccloed Posted at: 2017-02-01T19:41:47.224Z Reads: 179

```
Sounds like a plan! Thanks!
```

---
## \#38 Posted by: L3chef Posted at: 2017-08-04T18:19:26.220Z Reads: 163

```
@Eboostin Did you ever get around to try it? I'm searching for a solution and have the same on/off switch.
```

---
## \#39 Posted by: GhettoFab.rictation Posted at: 2017-12-01T05:30:42.187Z Reads: 133

```
I'm just going too hook my led up to my step down converter and hook up the switch as normal with my leads show from top to bottom nc no c and it will power on with my lights when I turn my board on<img src="/uploads/db1493/original/3X/f/a/fa9f6e8dbb441ed398c9363362c11001cd2f7a82.jpg" width="281" height="500"> <img src="/uploads/db1493/original/3X/8/4/843dca0e513733b52173f4f96646711dbddb9bbd.jpg" width="281" height="500">
```

---
## \#40 Posted by: mmaner Posted at: 2017-12-01T23:05:08.966Z Reads: 128

```
If you dont have an anti-spark switch that includes the LED driver, you can use the +5v feed from the VESC.  I've done it, completely safe.

http://www.electric-skateboard.builders/t/dropped-airless-glorrrrrrryyyyyyyy-dual-208kv-dual-focbox-10s4p-30q-ly-evo-airless-6in-wheels-on-6-shooters/36578/57?u=mmaner

<img src="/uploads/db1493/original/3X/a/7/a761e6260e63ae95bea33ccbd30141905ddd2ac1.png" width="690" height="338"> * from @Namasaki
```

---
## \#41 Posted by: GhettoFab.rictation Posted at: 2017-12-01T23:31:12.629Z Reads: 122

```
I might use my step down converter instead because I'm going to have 2 fans running on my vesc lol I thought that too but don't want to overload the vesc
```

---
## \#42 Posted by: GhettoFab.rictation Posted at: 2017-12-02T05:30:41.705Z Reads: 114

```
Anyone have any resistors soldered neatly to pcb (3.6kohm 1w) ? That will do it and if it's possible and neat I'm down
```

---
