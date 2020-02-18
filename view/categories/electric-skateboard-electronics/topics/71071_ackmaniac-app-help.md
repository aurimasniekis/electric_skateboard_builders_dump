# Ackmaniac app help!

### Replies: 4 Views: 402

## \#1 Posted by: Davide Posted at: 2018-10-13T12:11:03.992Z Reads: 71

```
Hello there!
I got a Flipsky ble module, which I tried with the vesc tool for android and works fine. I've recently switched to @Ackmaniac vesc tool for pc since is the best tool so far, and I tried to connect but it isn't working, I can connect but it ain't showing any values, and if I try to set parameters the app it's giving me "esc not connected".
So I check app configuration, and it was ppm&uart, I check Baudrate and it s the default 9600 or 9800 and don't remember. So I tried the 115200, the default of VESC tool and still nothing is working.... did this issue happen to anyone else? How is it fixable?
```

---
## \#2 Posted by: Okami Posted at: 2018-10-13T13:55:41.835Z Reads: 62

```
I think some notes were left in vesc monitor app thread (scroll till end)..
https://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888/982

Havent connected my flipsky module yet but so far it looks like it might be doomed not to go with ackmaniack firmware
```

---
## \#3 Posted by: Jmding Posted at: 2018-10-13T18:01:33.081Z Reads: 50

```
Flipsky's module uses a different communication technology from what Ackmaniac's app is expecting.  It will only work with VESCTool.  To use Ackmaniac's app, use an HM10 BLE module
```

---
## \#4 Posted by: Davide Posted at: 2018-10-13T19:22:56.185Z Reads: 39

```
Thanks man, I didn't know that!!
```

---
