# Change VESC 4.12 settings without USB (port broke off) \[solved\]

### Replies: 7 Views: 875

## \#1 Posted by: Achmed20 Posted at: 2018-02-14T19:54:49.782Z Reads: 105

```
hey folks.
I know that you can flash the VESC using a st232 programmer, but can you also change the settings using the pins on the VESC using the VESC tool?

im asking because my USB port broke off and i am absolutly not able to solder these tiny pins back on.
```

---
## \#2 Posted by: bevilacqua Posted at: 2018-02-14T20:20:25.356Z Reads: 99

```
mine did too...
2 options that worked for me: 

- on a 2xVesc setup via the CAN-Bus (Click can-forward and set the correct vesc ID) 
- Via a HM-10 Bluetooth module. I use the metr.at version from @rpasichnyk witch uses the TCP-Bridge option.
```

---
## \#3 Posted by: Achmed20 Posted at: 2018-02-15T02:25:38.473Z Reads: 76

```
hmm, the slave thing might work. to bad i dont have a vesc with older firmware left :(

ive got the ackmaniac version on it so changing Amp settings or so is easy, but if i ever want to use different batteries or motor, i have a problem
```

---
## \#4 Posted by: Riako Posted at: 2018-02-15T03:09:18.076Z Reads: 72

```
Maybe Mr P ( @Pimousse :angel: ) could help you ... (not sure yet)
```

---
## \#5 Posted by: Pimousse Posted at: 2018-02-15T04:58:57.836Z Reads: 63

```
I'd say the same as @bevilacqua.

There is also a third (tricky) method :   
Use a specific BLE module, flash it with Vedder's code through STLink and use VESC Tool (linux only) wirelessly.
This is a beta and a pretty new feature.
More info here : https://vesc-project.com/node/234
```

---
## \#6 Posted by: bevilacqua Posted at: 2018-02-15T06:56:50.770Z Reads: 58

```
the vesc whose usb port you can use to connect to the other one (via CAN) does not have to be flashed with the same software.
```

---
## \#7 Posted by: Achmed20 Posted at: 2018-02-15T10:17:17.863Z Reads: 45

```
sweet. thx alot guys :)
```

---
