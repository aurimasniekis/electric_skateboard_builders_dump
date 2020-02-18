# VESC Project - Bluetooth dongle error

### Replies: 10 Views: 279

## \#1 Posted by: MrDGOrman Posted at: 2019-05-20T21:04:35.607Z Reads: 85

```
Hi everyone,

I received my dongle from Trampa today. Hooked it up to my enertion focbox after switching the TX/RX wires accordingly and I get the following message when loading the app.
![vesctool|230x500](upload://qWjVW6yCm51t1Hy9UT7b63oONR1.jpeg) 

Thoughts? It connects and then a second later it disconnects
```

---
## \#2 Posted by: louwii Posted at: 2019-05-20T21:35:19.643Z Reads: 71

```
Have you tried Ackmaniac android app? Just so we know if the dongle and your phone can connect properly.
https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888

(enable bluetooth and location when connecting to your bluetooth dongle)
```

---
## \#3 Posted by: MrDGOrman Posted at: 2019-05-20T21:47:16.706Z Reads: 69

```
I got this dongle because the Ackmaniac app isn't compatible with the new version of vesc software. It appears to connect without a problem.

I'm wondering if I need to update the software to the lastest version and then try again?
```

---
## \#4 Posted by: louwii Posted at: 2019-05-20T22:52:06.540Z Reads: 61

```
We need help from @trampa here :)
```

---
## \#5 Posted by: trampa Posted at: 2019-05-21T04:30:46.860Z Reads: 52

```
Rx to Tx, Tx to Rx. Hope that will solve your matter.
```

---
## \#6 Posted by: MrDGOrman Posted at: 2019-05-21T10:26:17.867Z Reads: 31

```
I've already done that. Ive set the wires up as followed:

* VCC - 3.3v
* GND - GND
* RX - TX
* TX - RX
```

---
## \#7 Posted by: trampa Posted at: 2019-05-21T11:14:45.667Z Reads: 26

```
Did you activate UART? select PPm & UART in APP config (using USB connection to VESC-Tool)
```

---
## \#8 Posted by: MrDGOrman Posted at: 2019-05-21T11:29:24.137Z Reads: 22

```
Sorted it. My buadrate was too low. Just done a firmware update aswell and gone through all the settings. Honestly love the app!

Is there a way for me to change from Km to Miles?
```

---
## \#9 Posted by: trampa Posted at: 2019-05-21T11:30:34.543Z Reads: 22

```
Not yet, but Benjamin has that on his list.
```

---
## \#10 Posted by: MrDGOrman Posted at: 2019-05-21T11:51:57.959Z Reads: 18

```
Sweet. I'm excited. Thanks!
```

---
