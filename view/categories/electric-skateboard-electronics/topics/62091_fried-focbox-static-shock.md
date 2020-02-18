# Fried FOCbox ? static shock?

### Replies: 7 Views: 261

## \#1 Posted by: BooYA Posted at: 2018-07-17T12:29:05.894Z Reads: 93

```
Hi everyone, I just went to solder my bluetooth module to my focbox as I don't have the right connector and actually hate these connectors.
SOldered 5v, GND TX and RX on BT module, tried to plug usb to vesc tool and activate UART, but I can't connect to the FOCbox anymore ... tried different USB cables, reinstalling VCP drivers, still impossible to connect ...
Is it possible that I fried VESC by simply soldering on it ? Like static electrical shock ? I use a Weller high end soldering station and never had such an issue solderong other chips.
Would appreciate your opinion :slight_smile:
```

---
## \#2 Posted by: TarzanHBK Posted at: 2018-07-17T13:01:45.851Z Reads: 84

```
maybe you shorted the connector while soldering?
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-07-17T13:24:47.592Z Reads: 77

```
Does any LED lights up when power is connected? Also maybe you mixed pinouts?

Maybe if you still using original case it touches wires to the case and grounds it?
```

---
## \#4 Posted by: BooYA Posted at: 2018-07-17T13:27:03.482Z Reads: 75

```
okay I found the issue .... that's crazy strange
Turns out R104 ( USB data- resistor ) was reading 100M Ohms ^^ Supposed to be 22Ohms.
I guess this resistor doesn't handle heat very well :stuck_out_tongue:
To anyone having issues with USB connection, check your resistor values ( R103 and R104 )
seems to be very heat sensitive !

Have a nice day guys :slight_smile:
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-07-17T13:27:49.750Z Reads: 71

```
Nice, did you soldered directly to resistors?
```

---
## \#6 Posted by: BooYA Posted at: 2018-07-17T13:33:00.206Z Reads: 66

```
![20180717_152956|690x388](upload://khto7aI5utOwLSIS3ZjcKdCBN3K.jpg)
Soldered a USB cable this way and focbox now connects to pc flawlessly!
R104 still reads infinite resistance value xD
An hour ago all was working right through the Mini USB port haha
```

---
## \#7 Posted by: TarzanHBK Posted at: 2018-07-17T13:34:30.707Z Reads: 64

```
wait till the upload finishes before posting ;)
```

---
