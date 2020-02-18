# Usb charging wiring

### Replies: 16 Views: 805

## \#1 Posted by: Vampiresquid64 Posted at: 2017-08-11T18:44:25.590Z Reads: 131

```
Nubey Electronics question here, so I have a 3 pins where a USB port for charging a battery used to be but it broke so I bought a female usb port. The one I bought has 4 pins , a + and - as well as a data + and -. When I hook it up to my voltmeter It only registers voltage when I put the positive with the positive signal wire and same with the negative. The USB charging port on the board has 3 pins (3rd one is for balancing the battery I believe) but I'm not sure which wires to hook up to where. I can send pics if needed. This is on a gt2b
```

---
## \#2 Posted by: Skitzor Posted at: 2017-08-11T18:48:52.046Z Reads: 126

```
If you know all this. Just line em up and connect it that way. Most inportant is that you keep you + + and - -
```

---
## \#3 Posted by: Vampiresquid64 Posted at: 2017-08-11T18:56:54.834Z Reads: 112

```
well the light for charging on the gt2b wont come on if its not connected to all 3 ports. iv tried all the combinations with the 2 wires I have but im not sure how to link the 2 wires to the 3 wires and make it charge correctly. maybe I need to put 2 of the wires from the controller together?
```

---
## \#4 Posted by: jammin Posted at: 2017-08-11T22:59:56.228Z Reads: 84

```
3 ports? Could you send pictures? It's hard to tell exactly what's going on here. It seems like you're confusing the USB port with an IC/mosfet, but I'm not sure.

You shouldn't need to connect the data wires (since you're only using the USB port to change).
```

---
## \#5 Posted by: Vampiresquid64 Posted at: 2017-08-11T23:26:46.621Z Reads: 72

```
<img src="/uploads/db1493/original/3X/7/9/79d02e7b6203236a0713356bae6f352e4b761833.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/b/7/b779adc7a6939ca19acc89e489589bc29e0f9690.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/2/e/2e5e2fc49b65d7137f7d34f7e50f6ea6424d318c.jpg" width="281" height="500">
```

---
## \#6 Posted by: Vampiresquid64 Posted at: 2017-08-11T23:29:13.046Z Reads: 62

```
that hotgluey mess is where the usb port used to be. hot glue is just there to make sure the connections dont short and the brown wire with the tape is just an extender
```

---
## \#7 Posted by: jammin Posted at: 2017-08-11T23:46:36.768Z Reads: 60

```
thanks for the images, but I still can't see where the 3 wires are coming from.

I see that you've intertwined your data and power lines. Shouldn't be an issue, but also not concerning.
```

---
## \#8 Posted by: Vampiresquid64 Posted at: 2017-08-11T23:47:36.387Z Reads: 58

```
the 3 wires are coming from where the 3 pins of the usb ports used to be
```

---
## \#9 Posted by: jammin Posted at: 2017-08-11T23:48:53.598Z Reads: 53

```
sorry I really want to help you but I have no idea how you're getting 3 pins from a 4 pin interface (USB).
```

---
## \#10 Posted by: Vampiresquid64 Posted at: 2017-08-11T23:50:21.769Z Reads: 52

```
oohh no, the 3 pins are from the usb port on the gt2b and the 4 wires that I wrapped together are from a usb port that I have plugged into the wall.
```

---
## \#11 Posted by: jammin Posted at: 2017-08-11T23:53:13.052Z Reads: 52

```
yes but the USB header has 4 pins, right? idk how the GT2b is getting 3 pins from that. lemme do a little bit of researching and see what I can find.

right now my best guess is that one is ground, and the other two are hot? pretty sure it's not a data pin, but hey, learning is always a process ;)
```

---
## \#12 Posted by: Vampiresquid64 Posted at: 2017-08-11T23:55:50.409Z Reads: 46

```
yeah i think ur right about a ground. hopefully I didnt buy the wrong usb connector, took like 3 weeks to get here lol
```

---
## \#13 Posted by: chinzw Posted at: 2017-08-11T23:57:33.926Z Reads: 43

```
The usb port of the gt2b is + - and signal, thats why its 3, its not really a data port.
```

---
## \#14 Posted by: jammin Posted at: 2017-08-11T23:57:59.490Z Reads: 43

```
can you send me a close-up (or could you read the PCB) of where the wires are leaving? I just realized that 3 pins probably means that it's a push button toggling the voltage. Possibly a channel 3 button? (bc the battery and PCB is intercepted by the CH3 button on the vanilla controller).
```

---
## \#15 Posted by: Vampiresquid64 Posted at: 2017-08-12T00:04:50.065Z Reads: 42

```
all it says is j4 on one side and has an arrow on the other. you can just google it if u want to see for urself
```

---
## \#16 Posted by: danyCRO Posted at: 2019-05-04T21:57:05.315Z Reads: 16

```
![20190504_205635|666x500](upload://o44pxb406OI4viHe0StjHyAPAU3.jpeg) ![20190504_200225|666x500](upload://rOhMFHOTJ0tXsHID2SCwbNNgreU.jpeg) i think I destroy mine gt2b USB. What now?
```

---
