# Anyone found a way to program HobbyKing X-car beast 150A ESC without the card?

### Replies: 8 Views: 1247

## \#1 Posted by: murloc992 Posted at: 2018-05-12T10:53:15.405Z Reads: 111

```
Hello Esk8 people!

I was wondering if anybody found what the titles says, or maybe even reverse engineered the protocol (servo most likely) so an arduino could be used?

I am using a 6S system with a 280kV motor at 2:1 gearing and the default acceleration being on "High" means I can press the throttle even a little and see the board go to space. Without me ofcourse.

The card where I live (europe) is out of stock, and this is the main, limiting factor now. Seems like not even people around me (in RC groups) have any "supported" cards..

If anybody could assist me in reverse engineering this or even have already done so I would even pay you just to be independent from the card.
```

---
## \#2 Posted by: BooYA Posted at: 2018-05-12T11:47:39.099Z Reads: 100

```
Works with the Fvt program adapter, you can get it on banggood.
The xcar beast is actually a rebrand of ZTW esc, so you can get the software on ztw website 
Gecko USB or ProPC etc
```

---
## \#3 Posted by: BooYA Posted at: 2018-05-12T11:52:48.182Z Reads: 94

```
You could try with a USB serial adapter, like an FTDI.
Just plug both tx and rx in the servo signal. 
It may work as I know fvt esc is running a modified version of Blheli, and blheli supports communication using serial interface to USB. 
Also blheli supports arduino, so you might be able to use blheli suite software to build an arduino interface and then use it to connect the xcar
```

---
## \#4 Posted by: murloc992 Posted at: 2018-05-12T12:09:12.103Z Reads: 83

```
Hi there, I have been trying the BLHeli thing with a MEGA2560. I have connected ESC ground to GND, signal to RX0. Programmed the MEGA2560 as an interface, not the 4-way if one, just the simple one. When I try to load and cycle ESC power I get RX/TX LEDs flashing but nothing happens. If I connect same signal cable to both TX0 and RX0 using a breadboard I don't get anything at all. I guess I will need a card anyways..
```

---
## \#5 Posted by: laurnts Posted at: 2018-05-12T12:18:09.933Z Reads: 77

```
Its only 8 euro ish, safe the hassle for something else.
```

---
## \#6 Posted by: murloc992 Posted at: 2018-05-12T12:38:17.108Z Reads: 75

```
I do understand that. But waiting for a month or more because stock in Euro/UK is out sounds like a pita. :confused:
```

---
## \#7 Posted by: BooYA Posted at: 2018-05-12T21:51:49.270Z Reads: 61

```
https://m.banggood.com/fr/RC-Car-Program-Card-For-FTV-Series-Car-Brushless-ESC-USB-Link-Card-p-985974.html

I told you this one does the job I have it and the same esc works well, use the ZTW soft
```

---
## \#8 Posted by: murloc992 Posted at: 2018-05-13T21:55:07.282Z Reads: 39

```
I managed to get a card to borrow for now. Reverse engineering it using arduino seems quite impossible (arduino cannot handle the timing) so I will just program it as is and get a card later down the road. I got a ZTW LCD USB card which works perfectly fine so I am testing the max I can.. :smiley:
```

---
