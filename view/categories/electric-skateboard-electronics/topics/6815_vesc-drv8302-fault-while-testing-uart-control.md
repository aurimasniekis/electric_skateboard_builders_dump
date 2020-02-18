# VESC DRV8302 Fault while testing UART Control

### Replies: 5 Views: 755

## \#1 Posted by: Sir.Mighty Posted at: 2016-07-29T12:01:41.407Z Reads: 70

```
Hello,
I made a RX/TX from two Arduinos. The receiver Arduino was connected to the VESC through UART. I used https://github.com/RollingGecko/VescUartControl as library.
I controlled it through Nunchuk Packets. Everything worked.
But then, no movement. Connected the VESC to my PC and low and behold: FAULT_CODE_DRV8302
So I immediatly looked at the VESC if there is visible damage to the DRV chip, but nothing. Checked if it was hot, also nothing.
I'm totally confused as to what caused the FAULT_CODE_DRV8302 and I don't know what to do now. Never got to ride the board, because I had no working remote.

Its an 4.12 Enertion VESC, so you can imagine the frustration, I was waiting for it since april. The VESC worked fine after initial Motor Detection and controlling it through BLDC Tool and when I still used the Arduino connected through PPM.

The complete fault:

    Fault            : FAULT_CODE_DRV8302
    Current          : 3.1
    Current filtered : -0.2
    Voltage          : 38.39
    Duty             : 0.01
    RPM              : 0.3
    Tacho            : 5
    Cycles running   : 3
    TIM duty         : 377
    TIM val samp     : 193
    TIM current samp : 25865
    TIM top          : 51344
    Comm step        : 4
    Temperature      : 31.99

Here's also two pictures of the VESC:
http://imgur.com/a/iyza2 (imgur because they are to big/high res)
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-29T12:23:07.586Z Reads: 62

```
Try re flashing the firmware. That has fixed a few issues for some people.
```

---
## \#3 Posted by: Maxid Posted at: 2016-07-29T12:23:25.231Z Reads: 63

```
In the nunchuck pins it looks like ground is connected to the +5V pin. You are sure that is correct? Black cabling should not be used for anything but ground.
```

---
## \#4 Posted by: Sir.Mighty Posted at: 2016-07-29T12:30:48.913Z Reads: 59

```
I reflashed the firmware, still same problem.
The cables are right, triple checked before powering anything on. Used black cable because I tried a Logic3 Nunchuk first, which has red as ground and black as +3.3V, reciever of that was faulty, so I just resoldered the black cable to 5V (5V arduino), and connected the rest of the Arduino.
```

---
## \#5 Posted by: NNGG Posted at: 2016-07-29T20:40:51.608Z Reads: 43

```
What is uart control?
```

---
