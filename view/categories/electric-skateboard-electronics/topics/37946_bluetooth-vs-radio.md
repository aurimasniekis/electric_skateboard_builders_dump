# Bluetooth vs Radio

### Replies: 4 Views: 724

## \#1 Posted by: Snowi Posted at: 2017-11-10T18:26:42.016Z Reads: 120

```
So there has been lots of debate for which form of communication should be used in custom controllers. I see lots of people saying Bluetooth is better than Radio and vice versa. I just want to make a thread about this concern as there are many people don't have a set answer, and I couldn't find a very focused thread on this topic.

So what is the answer: Bluetooth or Radio?
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-11-10T20:55:04.461Z Reads: 100

```
I can only give you my experience with bluetooth and the reason why i'm switching to nrf24l01 in my next remote. I don't fully understand every aspect of the nrf yet, but i'm getting there.

Assuming you're using an Arduino, Bluetooth is simpler to hook up than NRF and at first glance easier to program as well. You just send serial commands to the module that it transmits to the other end. However, i found that Serial.print is way too slow for that application, so you have to use Seria.write. And with that comes the additional task of creating some form of protocol, which can be as hard as you want to make it i guess. 

In my current setup i have a nunchuck, arduino nano, arduino  mega and two hc05 bluetooth modules. The Arduinos each send a packet of 4 byte values to each other, the nano trasmits joystick position and buttons pressed of the nunchuck and the mega transmits Voltage, Speed, Amps and Capacity from the VESC to the nano. Even with that small amount of data i had to limit the read/write rate manually as the arduinos couldn't reliably keep up with their other tasks and the high refresh rate.
Also, i had random drop-outs during the ride that weren't recognized by the serial.available() function, which is unconvenient.
Otherwise they worked ok, after changing my 4.12 vesc to the esk8 controller the dropouts went away, might have had to do something with the power cables running too close to the bluetooth antenna.

Ok, now to the reasons i want to use nrf modules next. First, you have more control about the RF stuff, like using actual Antennas and adjusting channels and power levels. That should make the connection more robust (i hope :D ) and has more options for troubleshooting. Then there is the automated packet checking stuff that could be pretty helpful in failsafe scenarios. Also, you can just send the data as a single structure in arduino, which makes for an imo cleaner code and the transmission itself should be faster which means more transmitted data is possible. 
Wiring the module might be a bit harder because of the dedicated 3.3V regulator and the SPI interface, but that's a problem you only have to figure out once. Lastly, they don't use a serial port, which means that i can use 2 arduino nanos instead of nano/mega combination for reading vesc data and communication.

Alright that is a pretty long post and very much out of the top of my head, i hope it helps in you decision making!
```

---
## \#3 Posted by: Wajdi Posted at: 2017-11-10T21:21:14.609Z Reads: 89

```
It really all depends on your application needs. For example, BT is more suitable for smartphone devices applications, it often has short range communication, and very limited protocol control (because it is standardized). Raw BT data throughput is mostly around 0.5- 2 mbps, with a lot of overhead imposed by establishing and managing the connection. 
You may find that BT 4.0 for example has a theoretical data speed of 25Mbps, but the data is actually transferred over a WiFi (802.11) connection, while BT is only managing and establishing the connection.

On the other hand, RF such as nrf24, has far more flexibility when it comes to managing it's communication protocol. It has longer range if adjusted accordingly, and can be highly customized to your needs (Data speed, transmit power, etc..)
Therefore RF is more responsive, fast data transmission, longer range, and suitable for real-time control applications that requires a consistent/continuous link.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-11-10T21:29:32.792Z Reads: 75

```
Just wanted to add another anecdotal case.  I used hc-05 Bluetooth modules and an Android app to control my board.  Controlling a slider or while riding was precarious and the Bluetooth connection would randomly lose connection.  Been using nrf based custom controller for over a year and no major problems, when using max transmission strength the Arduino can't supply enough current so a capacitor is needed between the nrf Gnd and power if using max transmission strength but even on low transmission power it is a consistent enough connection when standing on the board for it not to be an issue.  I use a Bluetooth module for getting telemetry data with the metr app and module.


Data from metr
https://metr.at/r/rKZvg

Custom controller code
https://github.com/shusain/eskatecontroller

Updated controller design work in progress
https://cad.onshape.com/documents/50e9e32d777391df91fbe5a9/w/19598faab2182f3b574dcfaf/e/0ad21ad85976eca4fe7f88bc
```

---
