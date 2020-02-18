# HM-10/AT-09/BT05 and VESC - no connection

### Replies: 5 Views: 241

## \#1 Posted by: kamikatze13 Posted at: 2019-07-14T12:49:56.919Z Reads: 44

```
VESC Tool Mobile v1.16;
VESC Firmware: 3.58;
VESC Hardware: 4.12, Hobbyking/Turnigy SK8-ESC

hi guys, having trouble here to get a BLE connection to the VESC with the current VESC Tool Mobile app.

The BLE module i got: https://www.ebay.de/itm/AT-09-komp-HM-10-Bluetooth-4-0-Board-BLE-Low-Energy-Modul-CC2541-CC2540-Ardu/252911950935

and here's a vid of the issue: https://www.youtube.com/watch?v=ZH3aQ94LYk0

as you can see, after one clicks "connect" in the app, the LED on the module goes solid red - only to go back to blinking.

what's causing the app to fail to connect? i triple-checked the cables (rx goes to tx and vice versa), tried 9600 as well as 115200 baud rate for UART. connecting with the BLE Scanner works fine as well.

 any ideas?

![Annotation%202019-07-14%20143942|690x82](upload://3AmgF9EfAXwIIyuQBznqJNTHmz0.png) ![Annotation%202019-07-14%20144017|690x183](upload://wqoDgiyeAf5QNkU04UNtlkJUUsr.png)
```

---
## \#2 Posted by: chris96 Posted at: 2019-07-16T11:04:06.402Z Reads: 29

```
I have the exact same problem, will report when its fixed
```

---
## \#3 Posted by: mutantbass Posted at: 2019-07-16T11:13:12.987Z Reads: 27

```
wont work. you need the proper nrf module.
```

---
## \#4 Posted by: kamikatze13 Posted at: 2019-07-16T14:29:01.662Z Reads: 23

```
so what is it with the ppl having hm10 modules working in this very forum? do they use different firmware?

also, is vesc-project.com down for just me or for everyone?
```

---
## \#5 Posted by: Supermoto Posted at: 2019-09-19T06:02:28.993Z Reads: 9

```
I have the same chip and have read countless threads with information, some going into great detail on how to change the ID in the VESC to allow different modules to work, but then others day the HM-10 works just fine. Any updates with this?
```

---
