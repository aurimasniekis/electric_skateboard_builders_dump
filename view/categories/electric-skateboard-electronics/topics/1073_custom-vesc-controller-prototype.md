# Custom VESC Controller - Prototype

### Replies: 13 Views: 3485

## \#1 Posted by: vitormhenrique Posted at: 2016-01-21T16:32:18.129Z Reads: 281

```
I wanted to create a custom controller to use with my ongoing electric skateboard build. I love the BadWolf GT2B Case mod (http://www.thingiverse.com/thing:922378), but I want to get telemetry back from the VESC that I’ll use. I want to be able to check speed, battery levels, current etc. I also want to store all data on a SD card and get some performance data after each ride. 

So this is my first rudimentary prototype, I’m terrible with 3d design, I’ll ask a friend to work on the second revision, The final goal is to have the same “feel” of the BadWolf mod, but with a OLED display (**I'm FAR from that now**).

<img src="/uploads/db1493/original/2X/f/f358923e9a9467a1179e7af6b2d910abd5295147.JPG" width="375" height="500">

<img src="/uploads/db1493/original/2X/f/fc7462a0e228141346199ffe73bacfa74f93a9be.JPG" width="666" height="500">

I have a not so good experience with nRF24L01+ radios, they are great, but can be very unpredictable, so choose to use xbee radios on my controller, they are expensive but ultra-reliable.

I’m using a Teensy-lc as brain and a small lipo charger with a 500 mah internal lipo battery. Wiring everything inside was a pain… but fine in the end.

I’m still working on the code, few features that I want to put on are the ability to change acceleration speed using the LCD, changing few VESC parameters and cruise control.

I’m still deciding if I’m going to add a second microcontroller on the receiver end or put the xbee receiver on the VESC directly, Benjamin is in a whole new level of coding, so I’m still trying to understanding the UART protocol.

Second revision I'll build my own PCB, with an ATMEL microcontroller and arduino bootloader, to avoid the wiring mess and making easy if someone else wants to build it.
```

---
## \#2 Posted by: Iceni Posted at: 2016-01-21T16:40:10.134Z Reads: 270

```
Interesting project, looking forward to seeing how it turns out!
```

---
## \#3 Posted by: longhairedboy Posted at: 2016-01-21T18:50:08.390Z Reads: 261

```
holy crap. I need this.
```

---
## \#4 Posted by: trbt555 Posted at: 2016-01-21T21:14:18.693Z Reads: 255

```
Interesting.
Are you getting any data back from the VESC yet ?
```

---
## \#5 Posted by: treenutter Posted at: 2016-01-21T21:23:15.615Z Reads: 248

```
@vitormhenrique wow this is impressive! Looking forward to hearing more about your progress.
```

---
## \#6 Posted by: vitormhenrique Posted at: 2016-01-22T20:39:49.368Z Reads: 220

```
I got telemetry working yesterday, but I'm still trying to figure it out how to control the motors using the UART, for now i'm using a second microcontroller as receiver and a PPM signal to VESC.

Another problem that I found is that the joystick that I'm using is too sensitive, I'll test different ones to have a better control of the skate.
```

---
## \#7 Posted by: trbt555 Posted at: 2016-01-23T08:51:01.445Z Reads: 199

```
Would you be willing to share your code ?
I know a number of people are working in the same direction, myself included.
```

---
## \#8 Posted by: vitormhenrique Posted at: 2016-01-27T19:34:57.956Z Reads: 183

```
Sorry about the delay,

I used [this][1] code as starting point, but change the datatype back to the original and I'm implementing the other methods.

I'm currently moving to a new home so I'll not me able to work on this project for a few days, as soon as I have more time I'll share the code, schematics and 3d model.


  [1]: https://github.com/RollingGecko/VescUartControl
```

---
## \#9 Posted by: Hummie Posted at: 2016-01-27T20:15:13.664Z Reads: 175

```
Just having the battery voltage would be good enough for me.  And maybe a max speed.  So much stuff you're adding on there..you're going to get pulled over for texting and driving.
```

---
## \#10 Posted by: mason Posted at: 2016-06-14T16:21:12.521Z Reads: 157

```
hey, do you mind writing up a tutorial on how to send data from the vesc to an OLED screen? I wouldn't know how to get started on something like this.
```

---
## \#11 Posted by: Nordle Posted at: 2016-06-14T16:26:19.362Z Reads: 158

```
Hey
:point_right: [Endless-Sphere Rollinggecko](https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812) :point_left:
cheers
```

---
## \#12 Posted by: JLabs Posted at: 2016-06-29T19:42:21.279Z Reads: 137

```
Hoe so the remote coming along?
```

---
## \#13 Posted by: vitormhenrique Posted at: 2016-07-13T04:23:30.286Z Reads: 116

```
Version two is out of the oven! http://www.electric-skateboard.builders/t/ultimate-vesc-controller/6014
```

---
