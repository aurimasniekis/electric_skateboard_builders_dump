# Nunchuck and Bluetooth

### Replies: 10 Views: 1220

## \#1 Posted by: Iam319 Posted at: 2017-05-05T04:33:37.385Z Reads: 102

```
Has anyone figured out a way to use a nunchuck and bluetooth module at the same time? I want to have the option to use my phone or nunchuck to control the board while using a single vesc.
```

---
## \#2 Posted by: Print3r Posted at: 2017-05-05T07:00:57.102Z Reads: 92

```
I personally would advise against the phone for controlling your board, but a new controller that will send some stuff back to the phone is being developed here (https://www.electric-skateboard.builders/t/oled-remote-s-with-gps-bt-nrf-under-development-please-leave-suggestions/22055) else there is the closed source app that focuses on getting as much data from the VESC back to the phone for comparing stats (https://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483).
```

---
## \#3 Posted by: Iam319 Posted at: 2017-05-06T18:10:22.441Z Reads: 74

```
Any reason in particular you wouldn't use the phone?
```

---
## \#4 Posted by: Print3r Posted at: 2017-05-06T18:36:45.181Z Reads: 73

```
If a drop of water lands on your phone, the throttle could be sensed elsewhere/ not sensed at all. Accuracy with touch screens is much lower than with a joystick/ thumbstick/ trigger. If your phone falls, when you are going at speed it will get damaged, the joystick is plastic so should be fine. Holding a phone is less comfortable than holding a joystick (in my opinion).
```

---
## \#5 Posted by: rpn314 Posted at: 2017-05-06T19:14:25.198Z Reads: 70

```
[quote="Iam319, post:3, topic:22443, full:true"]
Any reason in particular you wouldn't use the phone?
[/quote]

Bluetooth is okay for things like telemetry (that don't require such precise timing and reliability), but not actually controlling an electric board. Bluetooth is simply not reliable enough of a connection protocol to use it for controlling our boards.
```

---
## \#6 Posted by: hexakopter Posted at: 2017-05-06T19:38:43.989Z Reads: 61

```
When I am not mistaken that is possible with the new VESC 6.0 but not with any older hardware.
Or two "old" VESCs connected over CAN. But you asked for a single VESC. :slight_smile:
```

---
## \#7 Posted by: Iam319 Posted at: 2017-05-06T21:05:47.760Z Reads: 58

```
If I use that app you posted the second link to, wouldn't that take up my slot for he receiver?
```

---
## \#8 Posted by: Print3r Posted at: 2017-05-07T07:04:51.818Z Reads: 56

```
You would have to check but yes I think the bluetooth module gets its data over the vesc's uart port so you would have to use a transmitter receiver combo that gives ppm signals to the vesc (rather than uart as the newer ones made especially for the vesc are doing).
```

---
## \#9 Posted by: Iam319 Posted at: 2017-05-07T15:56:19.887Z Reads: 49

```
So how would I do that?
```

---
## \#10 Posted by: rpn314 Posted at: 2017-05-17T00:03:10.909Z Reads: 37

```
[quote="Print3r, post:8, topic:22443, full:true"]
You would have to check but yes I think the bluetooth module gets its data over the vesc's uart port so you would have to use a transmitter receiver combo that gives ppm signals to the vesc (rather than uart as the newer ones made especially for the vesc are doing).
[/quote]

You are correct. All of the bluetooth modules I have seen around here connected to the VESC using UART (a communication protocol) and then transmit those signals to a device (ie phone) via bluetooth.

[quote="Iam319, post:9, topic:22443, full:true"]
So how would I do that?
[/quote]

Assuming you're asking for how you'd use a bluetooth and a controller, you just need to choose a controller that doesn't need the UART or any similar connections. Basically, you're limited to PPM ones. Search here for the GT-2B remote (sometimes written without a dash). That's pretty much the go to around here.
```

---
