# FSESC 6.6 with FW 3.40 and UART Arduino Communication

### Replies: 3 Views: 473

## \#1 Posted by: Flo Posted at: 2018-08-19T00:37:15.085Z Reads: 97

```
I am really trying hard to connect an arduino to my new FSESC 6.6 from flipsky but I do only get read errors. I am using the RollingGecko library Branch VESC6 (https://github.com/RollingGecko/VescUartControl/tree/VESC6). Did any body have the same Issue? Does the library need an update in order to work with FW 3.40? 
I already tried changing the tx and rx pin - that is not the issue...
thanks for any help
```

---
## \#2 Posted by: Blix Posted at: 2018-08-19T00:55:37.305Z Reads: 91

```
@solidgeek is already trying to fix this: https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/1528
```

---
## \#3 Posted by: AutoItKing Posted at: 2018-08-20T20:46:09.299Z Reads: 56

```
Use 3.39, it'll work.
BV made a change in 3.40 that breaks a lot of UART programs/apps.
See the link @Blix posted for more info.
```

---
