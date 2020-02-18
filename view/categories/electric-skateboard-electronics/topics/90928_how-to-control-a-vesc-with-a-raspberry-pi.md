# How to control a VESC with a Raspberry Pi?

### Replies: 4 Views: 732

## \#1 Posted by: Schizug Posted at: 2019-04-17T21:45:29.511Z Reads: 85

```
I am trying to control a VESC in my system using a Raspberry Pi using Python. So far I have my input as a Wiimote coming into the Pi through Bluetooth and that's all sorted out, but my next hurdle is to somehow send signals to the VESC itself using the onboard GPIO pins.

I started to implement the [PyVESC](https://github.com/LiamBindle/PyVESC) library, but I'm not really sure on how to get the signals I'm sending to the actual VESC itself. I thought I would be able to use the PPM cable that comes out of the VESC, but I can't seem how to figure out if that's doing anything.

Has anyone had any experience with this before or can anyone send me in the right direction for more reading?

Thank you!
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-04-17T21:54:45.889Z Reads: 82

```
Ok, so first of all the PPM input is an input which can only handle PWM signals.\
I'm just going to assume that the PyVESC library uses the UART protocol to communicate with the vesc. So you would need to connect the according GPIO pins to the UART port of the vesc. :slight_smile:
```

---
## \#3 Posted by: Slak Posted at: 2019-04-17T22:26:24.880Z Reads: 69

```
I know you can create a PPM signal from an arduino (lib is fro servo iirc) to send to a remote receiver. Should be the same in python if you can find something like this. 

Edit after 15sec on google : \
did you even search @Schizug ? ;) --> 
https://www.raspberrypi.org/forums/viewtopic.php?t=219531

Tips : You should also search inside this topic for information (the search function of our forum has a checkbox for this) : https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/1
```

---
## \#4 Posted by: crueepy_yeti Posted at: 2019-11-01T07:19:45.260Z Reads: 21

```
Schizug, do you ever figure out how to control the vesc with a raspberry?
```

---
