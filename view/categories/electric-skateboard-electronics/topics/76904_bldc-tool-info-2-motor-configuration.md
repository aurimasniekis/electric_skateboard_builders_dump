# BLDC-Tool info 2 motor configuration

### Replies: 7 Views: 525

## \#1 Posted by: andrefleitao Posted at: 2018-12-03T11:31:11.803Z Reads: 68

```
Hi.

I am using the bldc_tool from Benjamin Vedder https://github.com/vedderb/bldc-tool for Linux.

I plan to have 2 VESCs connected to each other (master+slave) via CAN to have a differential robot (2 wheels + casters). I’d like to send commands and receive data via UART or CAN from the master VESC to a computer. Is this possible? If so how should i configure in the bldc_tool to have this setup?

This is what i tried:

I installed the bldc_tool and in the App configuration there is a “Send status over CAN” checkbox. There is also the App to use. UART would be the option since CAN does not appear here. Then on the side tabs there are the “Multiple ESCs over CAN” checkbox but only for ADC , PPM and Nunchuk inputs. The UART tab input only shows the Baud rate setting.
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-12-03T12:34:50.853Z Reads: 56

```
sounds like you need a DaVeGa 

https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509 

I dont know if its got memory to perma log your trips, but once you do it should just be a matter of sorting and displaying the data
```

---
## \#3 Posted by: janpom Posted at: 2018-12-03T13:07:56.536Z Reads: 47

```
What exactly are you trying to achieve? You can have the realtime data from the VESC displayed directly in the bldc_tool when you connect the VESC to your computer with a USB cable.
```

---
## \#4 Posted by: andrefleitao Posted at: 2018-12-03T15:57:38.512Z Reads: 38

```
Hi

I'd like to have a robot based on this differential drive. But would also like to configure what would be sent/receive by CAN (send speed commands but also get feedback from the odometry, motors and battery)
```

---
## \#5 Posted by: Sn4pz Posted at: 2018-12-03T16:02:33.105Z Reads: 37

```
this has already been done plenty of times, why not go the normal route and pay 8 dollars for an HM-10 module? I understand this is a builders forum but your time is valuable as well. Maybe consider using basic bluetooth and telemetry data? :P .
```

---
## \#6 Posted by: janpom Posted at: 2018-12-03T16:18:25.651Z Reads: 33

```
Maybe take a look at the [Firefly remote firmware](https://github.com/SolidGeek/nRF24-Esk8-Remote) for an example on how to control the VESC remotely and also how the retrieve the telemetry data.
```

---
## \#7 Posted by: andrefleitao Posted at: 2018-12-03T16:54:43.691Z Reads: 33

```
[quote="andrefleitao, post:4, topic:76904"]
e. But would also like to configure what would be sent/receive by CAN (send speed com
[/quote]

https://odriverobotics.com/shop/odrive-v35
something like this
```

---
