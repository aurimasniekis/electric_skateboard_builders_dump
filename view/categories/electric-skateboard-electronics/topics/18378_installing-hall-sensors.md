# Installing hall sensors?

### Replies: 7 Views: 2647

## \#1 Posted by: evoheyax Posted at: 2017-02-28T18:27:12.953Z Reads: 315

```
So heres a topic I couldn't find any information about. I found 2 videos on youtube that have some oversight, but the lack details I need:

https://www.youtube.com/watch?v=hTPtMdDAs1k
https://www.youtube.com/watch?v=5BXH6GP8mPU

Maybe someone who has install hall sensors before could chime in?

I'm mostly interested in the exact placement of the sensors and the configuration of the wires into the plug for the sensor. Not really sure where to start. Maybe someone with more knowledge could chime it? It would be nice to if with the help of the community, we could build a guide for the rest of community so that others like me who have no experience with hall sensors can sensor their motors.

Thank you!
```

---
## \#2 Posted by: mccloed Posted at: 2017-02-28T18:43:32.350Z Reads: 295

```
This was a good write up on Endless-Sphere:
https://endless-sphere.com/forums/viewtopic.php?f=35&t=69959&hilit=hall+sensors

Here are the pin-outs for the standard hall sensor plug:
<img src="/uploads/db1493/original/3X/b/4/b439a4e2619a7260e9bb7e17ba3849650d0305e6.PNG" width="281" height="500">

Hope that helps! I've installed hall sensors in several motors with great success. I'll try to answer any other questions you have.
```

---
## \#3 Posted by: evoheyax Posted at: 2017-02-28T19:44:36.403Z Reads: 268

```
Thank you for your help.

What I'm confused about is my understanding was each hall sensor has a +, and -, and a control.

How far apart should they be placed? 120 degrees?
And how do I determine which one is A, B and C?
What is the temp control?
Do I combine all of the negatives and positives from the sensors together so they can connect to pin 1 and 6?

Sorry, I'm just very confused...
```

---
## \#4 Posted by: hexakopter Posted at: 2017-02-28T23:03:29.000Z Reads: 240

```
Each Hall sensor has a GND pin, a VCC (most likely 5v) and a digital output pin. You can read more abut the ATS177 for an example here: [https://www.diodes.com/assets/Datasheets/ATS177.pdf](https://www.diodes.com/assets/Datasheets/ATS177.pdf)

There are different position places.

Which one is A, B, C is detected from the VESC automatically. You can wire the three output pins to the VESC H1, H2, H3 port how you want. GND and 5v are shared for the three hall sensors.

Temp control isn't implemented in the VESC 4.x.

I used "external" hall sensors on my sk3 6374 motor for testing. You can find PCB files and 3D printing files here for an example: [http://e0designs.com/products/hall-effect-sensor-board/](http://e0designs.com/products/hall-effect-sensor-board/)
I had the problem that the PCB was so large, that it crashed to the skateboard deck when turning. But it definitely is a great upgrade.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-02-28T23:37:26.682Z Reads: 224

```
At what angle do you recommend using to space the sensors? I'm assuming that the angle changes how the sensors work...
```

---
## \#6 Posted by: mccloed Posted at: 2017-02-28T23:41:46.491Z Reads: 223

```
[quote="evoheyax, post:3, topic:18378"]
What I'm confused about is my understanding was each hall sensor has a +, and -, and a control. **Correct**
<img src="/uploads/db1493/original/3X/1/5/15e43f2e4692a27c3db7f1709769fa33c668cc4d.png" width="339" height="149">

How far apart should they be placed? 120 degrees? **This is my preference but they can also be 60 degrees(not sure if it makes a difference)** 
And how do I determine which one is A, B and C?
http://mitrocketscience.blogspot.com/2011/08/hall-effect-sensor-placement-for.html 

What is the temp control? **I do not use this, myself. I just leave the plug with no wire attached.** 
Do I combine all of the negatives and positives from the sensors together so they can connect to pin 1 and 6? **Yes. as illustrated in the diagram above.**
[/quote]
I have purchased the EO Designs kit in the beginning but as @hexakopter said it adds some girth to the motor so I decided internal was the way to go. Both the diagram and the link helped me greatly to understand hall sensors.
```

---
## \#7 Posted by: evoheyax Posted at: 2017-02-28T23:46:09.914Z Reads: 197

```
Ok, that clears up just about everything for me to try the sensors now. Thank you so much @mccloed and @hexakopter.
```

---
