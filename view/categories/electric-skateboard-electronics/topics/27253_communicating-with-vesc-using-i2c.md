# Communicating with VESC using I2C

### Replies: 5 Views: 980

## \#1 Posted by: Mike_Lemon Posted at: 2017-07-10T16:01:01.664Z Reads: 84

```
Hello, 

I'm looking to controll a VESC through I2C with Arduino for now and I just can't find the I2C format protocol to communicate with it and or send a receive data like battery voltage and setting the power throttle. 

Does anyone has an arduino library to do that or know what is the format?

Thanks in advance for helping!
```

---
## \#2 Posted by: evoheyax Posted at: 2017-07-10T16:04:38.988Z Reads: 84

```
This is what you want:

https://github.com/RollingGecko/VescUartControl
```

---
## \#3 Posted by: Mike_Lemon Posted at: 2017-07-11T01:02:06.383Z Reads: 72

```
I said I2C not UART
```

---
## \#4 Posted by: cnd Posted at: 2019-04-21T23:22:58.714Z Reads: 30

```
Me too - did you ever figure this out?

(I tried to find it in the source code, but I2C is everywhere so I couldn't work out where to look)
```

---
## \#5 Posted by: Jamie42 Posted at: 2019-04-22T15:07:01.790Z Reads: 20

```
I want this too, but the VESC isn't capable of I2C so you would need an UART to I2C converter, probably with a microcontroller.

This would also make UART multiplexing sort of possible as multiple slaves are possible on the I2C bus.
```

---
