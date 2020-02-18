# VESC UART Telemetry Problems

### Replies: 5 Views: 720

## \#1 Posted by: AreaKruzer Posted at: 2017-11-21T04:59:44.508Z Reads: 73

```
Hi all,

I've been using my electric longboard for quite awhile now and want to fiddle with it.

I'm controlling my longboard on a PPM tx/rx. I am looking into having some form of telemetry from the VESC.

my VESC is 4.10 and running the latest 3.33 firmware. I've tried wiring the VESC Tx to arduino nano v3 and mega Rx and VESC Rx to Tx. I used RollingGecko's arduino library and files (including the vesc6 branch on his github), ran the setup on debug and the serial monitor was printing garbage. and don't seem to be able to be getting any values.

VESC is configured to be running PPM + UART. Can anyone advise what is the problem? Is there any way i could find out if the UART connection on my VESC is faulty ?
```

---
## \#2 Posted by: ervinelin Posted at: 2017-11-23T07:55:55.913Z Reads: 54

```
Did you find a solution to this by any chance?

My telemetry was fine until I updated to 3.33.... :frowning:
```

---
## \#3 Posted by: Der6FingerJo Posted at: 2017-11-23T08:21:01.966Z Reads: 50

```
Please take a look here, RollingGecko is trying to get some testers for the new library and any input would be appreciated!

http://www.electric-skateboard.builders/t/tester-needed-for-vescuartcontrol-with-new-interface/38476
```

---
## \#4 Posted by: RollingGecko Posted at: 2017-11-23T12:24:56.434Z Reads: 45

```
Did you try the branch v6?
```

---
## \#5 Posted by: AreaKruzer Posted at: 2017-11-23T12:47:05.234Z Reads: 42

```
I'll try the V6 branch tomorrow as the stuff is currently at my workplace.
```

---
