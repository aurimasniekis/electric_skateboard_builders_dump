# Bluetooth module + photon remote

### Replies: 12 Views: 310

## \#1 Posted by: Flasher Posted at: 2019-06-10T22:22:19.088Z Reads: 78

```
Is it possible to plug a Bluetooth module AND the photon/proton using a fsesc dual 6.6? Thinking of buying a module but don't want to waste money if I can't even use it
```

---
## \#2 Posted by: pjotr47 Posted at: 2019-06-10T22:44:05.016Z Reads: 75

```
I don’t know if the vesc has a dual uart output. But I know here is a guy on the forum who is developing a module so that you can use multiple uart devices on one port.
```

---
## \#3 Posted by: Flasher Posted at: 2019-06-10T23:39:48.760Z Reads: 68

```
I'm using the flipsky dual6.6 it has a UART port on both master and slave sides but I would be plugging the module on the slave side. Wondering if it would allow me to use the tool on the go even though I'm plugged through the slave. Also on another point, what would the risks of interferences be since both use UART and both are sending and receiving communications
```

---
## \#4 Posted by: Flasher Posted at: 2019-06-10T23:43:36.794Z Reads: 65

```
Also, by module what do you mean? The proton panel has an extra UART port on it to allow an extra product like the photon to be used. Are you speaking of a module with a sole purpose of adding ports (ex.: Usb hub)?
```

---
## \#5 Posted by: Giba Posted at: 2019-06-12T16:43:37.586Z Reads: 39

```
I have dual vesc setup the photon remote is connected to the master UART side using Canbus fwd to vesc1 and the Bluetooth module MH10 is at the Slave UART fwd to Vesc0 on Xmatic app setting. They works only to see what's happening in my system and get all the values and save my trips but I'm not changing the modes on battery and motor amps because once I do that it somehow confuses the Photon receiver and ended up having remote won't connect to photon receiver which I won't able to control the board.
```

---
## \#6 Posted by: Giba Posted at: 2019-06-12T16:49:42.605Z Reads: 38

```
![image|230x500](upload://c9zpiOCPy92HCJdozjUt2VTqIAr.jpeg)
```

---
## \#7 Posted by: bsancken Posted at: 2019-06-12T16:56:19.055Z Reads: 30

```
This is the tread that you would want to read to learn more about UART splitter's purpose.

Basically, if you only have 1 UART port and you want to connect more than one thing, you would need something like this.

https://www.electric-skateboard.builders/t/uart-splitter-for-vesc-based-escs/94552?u=bsancken
```

---
## \#8 Posted by: Flasher Posted at: 2019-06-12T17:13:14.758Z Reads: 27

```
@Giba good to know but xmatic is iOS and I'm on Android.
@bsancken I have a dual so 2 UART ports. I'm more concerned of interferences
```

---
## \#9 Posted by: Friskies Posted at: 2019-06-12T17:22:15.241Z Reads: 30

```
[quote="Flasher, post:1, topic:96317"]
fsesc dual 6.6
[/quote]

If you have two UART ports just plug both the bluetooth and photon in and configure it in the vesc tool. It should all work together without problems as long as you have configured it correctly.
```

---
## \#10 Posted by: Flasher Posted at: 2019-06-12T17:36:29.499Z Reads: 28

```
All work don't necessarily equal not cutting out... Don't wanna wipe out at 70km/h
```

---
## \#11 Posted by: Giba Posted at: 2019-06-12T17:58:40.495Z Reads: 28

```
Try look at wireless NRF connect dongle by Trampa that might work as it runs in new Vesc mobile app by Benjamin Vedder and you can do everything on the go with that
```

---
## \#12 Posted by: Flasher Posted at: 2019-06-12T18:11:09.636Z Reads: 26

```
A friend just gave me a flipsky Bluetooth module. Would that work?
```

---
