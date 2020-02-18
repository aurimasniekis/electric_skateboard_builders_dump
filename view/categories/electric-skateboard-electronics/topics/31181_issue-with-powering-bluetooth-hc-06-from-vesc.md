# Issue with powering Bluetooth HC-06 from VESC

### Replies: 6 Views: 1043

## \#1 Posted by: catalin.dragosh Posted at: 2017-08-21T19:22:55.151Z Reads: 64

```
Hi,

Has anybody encountered problems with powering a Bluetooth module (HC-06) from the VESC PPM (RC servo) pins?

I am trying to power an Arduino module with a HC-06 board attachedfrom the RC servo pins of the VESC and I can only power it if the VESC is already on when I make the connection between the VESC and the Arduino + HC-06 part. 

If I first connect the VESC and the Arduino + HC-06 and then power on the whole system, the Arduino powers on but not the HC-06.

Did anybody encounter this? Any ideas why this doesn't work?

I have also a Vedder Anti-spark switch attached. Could this affect the way the Bluetooth powers on? It seems to me that the switch from 0V to 5V is not instantaneous (at the RC servo pins), it gradually increases to 5V.

Any ideas are more then welcome.

Thanks a lot!
```

---
## \#2 Posted by: lox897 Posted at: 2017-08-21T20:21:06.338Z Reads: 53

```
Can you please show some pictures of your wiring?
```

---
## \#3 Posted by: Bataleon Posted at: 2017-08-21T21:18:30.444Z Reads: 51

```
I have never tried powering an HC-06 module from PPM. Powering from the UART header works great though.

Is there any reason why you are using the PPM header instead of UART?

<img src="/uploads/db1493/original/3X/2/d/2d981b2e23f9ea458de6f542c5235aa7dbddfd61.png" width="690" height="460">
```

---
## \#4 Posted by: lox897 Posted at: 2017-08-21T21:42:15.029Z Reads: 49

```
They both have 5v anyway, so it shouldn't matter what he uses. It would be better to use the UART because then you could have the TX & RX connected there too.
```

---
## \#5 Posted by: lox897 Posted at: 2017-08-21T21:43:39.771Z Reads: 49

```
Is your Vedder SparkSwitch attached between the battery and ESC or your VESC and the Arduino?
```

---
## \#6 Posted by: catalin.dragosh Posted at: 2017-08-22T08:31:37.813Z Reads: 39

```
There was no reason in particular to use the PPM. I just found it simple to use, but it proves to be a headache.

The Vedder SparkSwitch is connected between the batteries and the VESC. 

For now I am using one of these 2.4GHz G2TB remotes connected to the PPM (RC-servo) pins and that works fine. I've been suing it for more than 3 or 4 months.

The only problem is that the Bluetooth does not power on unless the VESC is powered on before connecting the two.

I attached a picture but it's  pretty cluttered. I hope you can understand sth of it. The batteries are connected to a BMS (blue shrink tube under VESC) and to the AntiSpark switch (blue shrink tube on top of the batteries), and then to the VESC.

<img src="/uploads/db1493/original/3X/5/9/5943931a37e20c2912edb414b94b4a658bd22ebe.jpg" width="690" height="388">

Thank you
```

---
