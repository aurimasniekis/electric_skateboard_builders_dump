# Vesc 4.12 and arduino uart

### Replies: 6 Views: 762

## \#1 Posted by: lukasilestam Posted at: 2018-08-14T23:12:42.049Z Reads: 98

```
Does anyone have a working arduino library with UART on vesc 4.12?

Currently I have connected BT module and applications on android - it works well. (9600 baud)

Now I wanted to connect through arduino ... I found something like:
https://github.com/R0b0shack/VESC-UART-Arduino

uploaded, connected LCD, baud 115200, uart + ppm and nothing ... does not download data from uart.
I use arduino Uno and vesc 4.12
```

---
## \#2 Posted by: Pedrodemio Posted at: 2018-08-15T00:35:37.904Z Reads: 86

```
What firmware are you using?
```

---
## \#3 Posted by: lukasilestam Posted at: 2018-08-15T07:32:21.227Z Reads: 72

```
Fw: 3.38
Hw: 410
```

---
## \#4 Posted by: lukasilestam Posted at: 2018-08-15T11:25:31.063Z Reads: 54

```
HW is too old?
```

---
## \#5 Posted by: Pedrodemio Posted at: 2018-08-15T12:51:45.992Z Reads: 48

```
Hardware doesn’t matter in this case

Try this one from @Pimousse

 https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/1480?u=pedrodemio
```

---
## \#6 Posted by: lukasilestam Posted at: 2018-08-15T17:23:16.839Z Reads: 45

```
Thank you!
Version VESC_FW_from_v3.34 is working :slight_smile:
```

---
