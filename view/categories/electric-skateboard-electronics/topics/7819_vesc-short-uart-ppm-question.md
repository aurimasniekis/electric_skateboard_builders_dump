# VESC short &amp; UART+PPM question

### Replies: 3 Views: 2104

## \#1 Posted by: makevoid Posted at: 2016-08-17T22:46:08.812Z Reads: 282

```
Hi, 

today I think shorted my VESC I'm not sure how ^^, I was developing a custom Arduino [application](https://github.com/makevoid/VescUartControl/blob/master/examples/VescUartSample/VescUartSample.ino) to log data over UART based off the awesome [VescUartControl](https://github.com/RollingGecko/VescUartControl) lib and sample code and save them into an SD card. This way I could load them later in a program that could make an animated graph and stick that onto a video pretty much as Vedder was doing.

Well, everything worked fine but I think I rushed some steps, on the "bench" everything was ok, I was able to connect to the VESC via UART, log all the data but I was powering the Arduino with an external power source. I currently have a 8S made from a x2 4S lipos in series, I hooked up the arduino connected to the vesc on a 4S Lipo. The Arduino was getting power correctly, I got the VESC logs but shortly (~20sec), even I was spinning the motor slowly via PPM (I had selected PPM+UART as control mode) the VESC overheated and bam, this is the current situation: 

https://youtu.be/ZHd1ekSJ9yo


<img src="/uploads/db1493/original/2X/8/8de97d72bfac4c01308864514d3a5924e9a9f40f.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/f/f6e1cd171d46d81235b8a55f237653abda13cf8a.jpg" width="375" height="500">

The VESC looks fine to the eye but **It's** definately **shorted**. I get close to 0 ohms from basically everywhere (the main battery + and -, 3.3v, 5v and gnd, rx/tx.. everywhere). When I connect power (12V 1A) after 10sec I have to disconnect it because the main chip (not the DRV) and the usb port get very hot very quickly. I'm no VESC expert but I know basics of electronics and soldering and if you can point me to what test to do and if it's just a simple component to check and replace I can manage that, otherwise my best option is to send it to the repair guy in germany. Btw this vesc is from esk8.de.


<img src="/uploads/db1493/original/2X/5/5e78753f779cd1d7e6712ee698be73b84babe7a0.jpeg" width="499" height="499">

This is how I connected VESC to Arduino via UART to Arduino TX/RX. The question is (other than what failed and how should I fix this):

Can I use both PPM and UART at the same time? Or is that that attempt to mix the two that made the VESC fail?

Maybe it failed because the Arduino provided too much current on the TX/RX-UART pins because was powered with ~16V (4S)? Should I try on another VESC but with a step down converter for powering the Arduino to make it 8V so it's safer? Or it was because I did something else stupid like inverting the PPM cable on the receiver (I think it was all alright but I may have f**ed up that and that's the only reason that comes into my mind). 

Thanks in advance for your help.
```

---
## \#2 Posted by: aliounembaye Posted at: 2017-05-13T08:42:17.100Z Reads: 155

```
Did you find a solution?
```

---
## \#3 Posted by: makevoid Posted at: 2017-05-13T08:59:35.570Z Reads: 149

```
Yes, I didn't have a common ground : / that was my error.

Also now that there are 3! logging solutions that rely just on a self powered (UART only) Bluetooth module I just use those, they have a lot of extra features. It's great to see this much development in such a short time.

If I'll play with arduino (maybe Intel Edison) in the future and I'll probably get a bec/buck down converter or a dedicated battery for the arduino, a bit more on the safe side  ;)
```

---
