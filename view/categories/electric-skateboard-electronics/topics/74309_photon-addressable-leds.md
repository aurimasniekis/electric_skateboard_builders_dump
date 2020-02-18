# Photon Addressable LEDs

### Replies: 10 Views: 539

## \#1 Posted by: ricardo Posted at: 2018-11-11T18:13:44.986Z Reads: 169

```
Hi,

Long time lurker, first time poster here!

I've recently started converting an Evolve Carbon Gen1 to a dual motor setup (it's alive, check here: https://www.instagram.com/p/Bp_rP_kALpy/) and I would like to pimp it up with adressable LEDs, powered from the Photon remote receiver. I've read the guide in here:

http://forum.eboardshop.net/t/photon-remote-lights-info/44

but would like to know which lights did those of you that did this before me got. I'm wary of the fact that the guide recommends not to exceed the 30 LED count... :-S

Any help appreciated!

Cheers,
Ricardo
```

---
## \#2 Posted by: ricardo Posted at: 2018-11-12T11:14:32.149Z Reads: 128

```
@wajdi, anyone?

:-)
```

---
## \#3 Posted by: Mich21050 Posted at: 2018-11-12T17:01:14.697Z Reads: 110

```
WS2812B led's and if you want to install over 30 leds you need an extern power source. You can also see a photo of the according connectors. What else do you want to know? :smile:
```

---
## \#4 Posted by: ricardo Posted at: 2018-11-12T18:06:37.090Z Reads: 99

```
Thank you for your help, I just wanted to know if anyone had tried going over the 30 LED suggested limit, and have a look at any setups that used the photon receiver as a power source, just to see how good or how bad it looks...

Cheers,
Ricardo
```

---
## \#5 Posted by: Holyman92 Posted at: 2018-11-12T18:08:30.640Z Reads: 95

```
I too am interested, I'm waiting for my photon to arrive
```

---
## \#6 Posted by: Mich21050 Posted at: 2018-11-12T18:11:53.867Z Reads: 94

```
You would fry your vesc if you draw I think over 1 amp "? :smile:
```

---
## \#7 Posted by: Wajdi Posted at: 2018-11-20T04:17:29.067Z Reads: 75

```
@ricardo I would suggest to use an external power source if you want to use plenty of LEDs. 
As @Mich21050 said, WS2812B are what I have tested, 5V version.
```

---
## \#8 Posted by: DAddYE Posted at: 2018-11-20T04:27:11.104Z Reads: 70

```
Sorry for the hijack!
Hey mate! I’d like to use my photon with brake lights. Basically when I brake will turn on a couple of leds. What leds should I use in your opinion?

Thanks!!!!
```

---
## \#9 Posted by: ricardo Posted at: 2018-11-20T07:52:50.238Z Reads: 61

```
thank you for the reply, @wajdi. Do you have a link to the LEDs you tested? Or at least its specs (number of LEDs, lenght, etc)

Cheers,
Ricardo
```

---
## \#10 Posted by: Wajdi Posted at: 2018-11-21T05:12:03.734Z Reads: 47

```
After I did some more testing, and reading the WS2812B datasheet, it seems that running it at 5V while having the data pin at 3.3v causes flickering issues. 
To solve this you can connect the LED strip GND and DATA pin as in the following picture, and connect the LED strip +5v supply to the +3.3v pin.
See the 3 connections marked in red the picture.

![Pinout|690x359](upload://4BWyZeUbZFf1BvBeawgk0EgMXLb.png) 

If you are going to use about 20 leds, then you can get away without using an external power supply.
To use the reactive braking and turn signals, use 10 leds for tail light, and 10 for front( you can control the color from the remote).

Here is a quick demo I recorded :

https://www.youtube.com/watch?v=EYOW3vpIw5Y
```

---
