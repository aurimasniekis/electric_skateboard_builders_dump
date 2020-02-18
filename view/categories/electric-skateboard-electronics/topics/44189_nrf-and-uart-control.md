# Nrf and uart control

### Replies: 8 Views: 590

## \#1 Posted by: Samuele00 Posted at: 2018-01-20T14:01:10.714Z Reads: 117

```
can someone explain to me how the nrf on vesc mode works? i would like a arduino transmitter and i have twonrf24l01 module.
 if I have to connect hm-10 I have to put vesc in uart and ppm mode?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-01-20T14:07:51.008Z Reads: 121

```
yes.

10chars
```

---
## \#3 Posted by: Deckoz Posted at: 2018-01-20T14:12:01.304Z Reads: 118

```

If you have NRF and are gonna use nunchuckcontrol you will need two ESC... Bluetooth and nunchuck nrf can't share a UART serial connection.

Your NRF -> Arduino will have to output ppm not uart if you want to use both Bluetooth and "NRF" with a ppm stream on a single vesc.

This will also mean your Arduino cannot get telemetry data... As ppm is a one way timing packet protocol, non telem.
```

---
## \#4 Posted by: Samuele00 Posted at: 2018-01-20T17:07:31.397Z Reads: 98

```
but what changes to put nrf and ppm?
```

---
## \#5 Posted by: Deckoz Posted at: 2018-01-20T17:12:18.799Z Reads: 91

```
? What do you mean?

Option 1
If you want to run UART Bluetooth module and PPM.. change it to ppm and uart on the application tab..

Option 2
You can't run UART Bluetooth and Nunchuckcontrol on the same vesc
..there's only one uart port pinned out...uart is not a bus so single device only.  You'll need two VESC to do this
```

---
## \#6 Posted by: Samuele00 Posted at: 2018-01-20T17:16:12.193Z Reads: 86

```
uart I need to see the charge battery on the app. and I would like to connect a radio control made with arduino, joystick, nrf24 but I do not know how to connect it
```

---
## \#7 Posted by: Deckoz Posted at: 2018-01-20T17:21:47.306Z Reads: 78

```
You can't do both on one esc you'll need two vesc one for Bluetooth one for uart nunchuck
```

---
## \#8 Posted by: Samuele00 Posted at: 2018-01-21T00:13:14.958Z Reads: 60

```
Ah okay thanks
```

---
