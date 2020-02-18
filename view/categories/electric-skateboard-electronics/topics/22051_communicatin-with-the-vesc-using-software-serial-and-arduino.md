# Communicatin with the VESC using software serial and arduino

### Replies: 8 Views: 1943

## \#1 Posted by: Mike_Lemon Posted at: 2017-04-30T00:27:20.627Z Reads: 120

```
Hello, 

I'm tring to get some data and control two VESCS using the UART communication and I'm struggling with and of course because I use around 3 UART busses both for the VESCS and the BL communication I cant use the hardware UART I've tried using this library:

https://github.com/RollingGecko/VescUartControl/blob/master/examples/VescUartSample/VescUartSample.ino

to do so but I keep getting errors and I'm not much into the way it approaches the user.

and I've came accros this library:

https://github.com/erwincoumans/ArduinoServoTxRx/tree/master/VescUart

which I like the programmer interface but probably doesn't include reading data off the VESC and same problem with the Software serial thing.

Does someone have an example of using one of those libraries(Or any other thing) 
To set up software serial communication along with reading and writing to the VESC?
```

---
## \#2 Posted by: lox897 Posted at: 2017-04-30T01:23:07.519Z Reads: 106

```
I use RollingGecko's library and it works fine for reading data off vesc through an OLED
```

---
## \#3 Posted by: Mike_Lemon Posted at: 2017-04-30T03:23:04.387Z Reads: 98

```
But I wanna use the code beyond that and through Software serial as well as writing data.
```

---
## \#4 Posted by: lox897 Posted at: 2017-04-30T03:34:43.813Z Reads: 95

```
What data do you want to write specifically?
```

---
## \#5 Posted by: Mike_Lemon Posted at: 2017-04-30T14:41:31.968Z Reads: 86

```
Motor dutycycle but now I figured how to use software serial with erwincoumans's library but there is no option to read data the same way trough a class.

Also is there anyway to use "Currecnt mode" like trough the UART communication with all the accelerations and breaking?
```

---
## \#6 Posted by: KTMinni Posted at: 2017-04-30T14:43:13.139Z Reads: 82

```
Have you tried setting the VESC to UART and PPM in the BLDC tool?
```

---
## \#7 Posted by: Mike_Lemon Posted at: 2017-05-01T21:22:07.809Z Reads: 75

```
Not about the vesc it's about the software I'd like simple fuction for classes to read data from the vesc as for now I can only write to it and set duty with the arduino.
```

---
## \#8 Posted by: KTMinni Posted at: 2017-05-01T21:40:20.505Z Reads: 74

```
Oh gotcha I've ran into the same issues with that.
```

---
