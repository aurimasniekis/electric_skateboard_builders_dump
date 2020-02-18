# NRF24 connection to VESC

### Replies: 14 Views: 1788

## \#1 Posted by: xilw3r Posted at: 2018-02-24T17:19:36.012Z Reads: 191

```
Hey guys,

I am not sure this is possible, but perhaps someone has already tried to connect the NRF24 RF chip directly to the VESC?

Would it be possible to have a complete control of the VESC this way? I tried searching for the answer but all i find are Vedders nunchuck variants or arduino based NRF24 remote controllers.

My plan is to make my own slightly modded version of the arduino+NRF24 for the remote and aI have another NRF24 module I want to connect directly to the VESC as a receiver.

Thanks for the help in advance! im a real damn noob in electrical pixies
```

---
## \#2 Posted by: moon Posted at: 2018-02-24T17:24:10.830Z Reads: 183

```
https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543

I don't know if this will help
```

---
## \#3 Posted by: xilw3r Posted at: 2018-02-24T18:33:43.110Z Reads: 164

```
Well... I did read through a lot of that thread, kinda hard to miss that one :) but i did not find the answer about vesc to nrf connection. 

Naturally I will be using the info there on the remote side of things though
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-02-24T18:34:31.932Z Reads: 156

```
that remote is literally based on connecting nrf to the vesc
```

---
## \#5 Posted by: Surfer Posted at: 2018-02-24T18:40:22.698Z Reads: 154

```
I believe he means to connect directly with the build in nrf on the vesc 6, seems like @solidgeek did try to find that information for the remote he is doing, even asking in the vedder forum without much success. 😕
```

---
## \#6 Posted by: xilw3r Posted at: 2018-02-24T18:41:48.582Z Reads: 152

```
Yes, I am talking about the receiver side, on the board it self
```

---
## \#7 Posted by: solidgeek Posted at: 2018-02-24T20:34:31.657Z Reads: 147

```
The issue in connecting the nRF24 module directly to the VESC is that it communicates over SPI (MOSI, MISO and SCK), and the VESC doesn't support commands in that manner. You would have to rewrite / add some code to the VESC firmware to get rid of the "SPI to UART" part (Arduino).
```

---
## \#8 Posted by: xilw3r Posted at: 2018-02-25T19:32:29.417Z Reads: 134

```
alright, i see.

I dug around a bit and found this though:

https://www.youtube.com/watch?v=PV64I1yTcsM

check around 2:00 minute mark. The NRF24 is connected directly to the UART port. Is this fellow on the forum? anyone know who this is ?
```

---
## \#9 Posted by: Janosh Posted at: 2018-04-29T23:59:35.215Z Reads: 116

```
@xilw3r

Did you make any progress so far?
I'm also looking into this, because I want to connect the Evolve R2 to the VESC.
```

---
## \#10 Posted by: xilw3r Posted at: 2018-05-06T18:40:00.114Z Reads: 101

```
I wrote an email to the guy, but no response.

You need a specific firmware on the vesc, I guess it should be available somewhere, but I definitely do not have the skills to write one, so I will just go the arduino translator way to get my stuff moving.
```

---
## \#11 Posted by: ofekp Posted at: 2018-06-08T21:08:13.329Z Reads: 91

```
For anyone else out there that might still be looking for this.

Check this out:
http://reboot.love/t/vesc-mods-for-robotics-use/107

looks like a simple code change (header define) to have the hardware SPI enabled.
Have not tested it myself but was exploring a bit (a lot) and found that, thought I'd share.
```

---
## \#12 Posted by: m.kicker Posted at: 2018-07-04T08:09:24.687Z Reads: 77

```
Hello! So did you manage to connect to the built-in nrf on the vesc ? 
I want to send data to the vesc but failed to connect over nrf with a arduino+nrf to the vesc.

I plan on modiffing the firmware on the vesc but I wanted to at least receive alive packets on the arduino.

Does anyone know how to configure the arduino to receive alive packet?

Thanks!
M
```

---
## \#13 Posted by: Wentworth Posted at: 2018-07-04T09:50:18.225Z Reads: 67

```
https://endless-sphere.com/forums/viewtopic.php?f=35&t=73812
This is what I found before. I hope it helps a little.
```

---
## \#14 Posted by: ofekp Posted at: 2018-07-05T21:43:46.297Z Reads: 55

```
Have not tried it yet, I plan to flush the firmware of the VESC with this:
`#define AS5047_USE_HW_SPI_PINS	1`
anybody tried this before?
```

---
