# Flipsky vesc 4.12 with hm 10 issue(ACKMANIAC-ESC Monitor)

### Replies: 20 Views: 632

## \#1 Posted by: Hoho0220 Posted at: 2018-12-21T19:20:05.337Z Reads: 141

```
Hi everyone,
I try to connect flipsky vesc by hm 10
I use the vesc monitor app
But it can not get any information
I use Anothet non flipsky vesc connect same hm 10.
It can work perfectly.
Should I change the firmware of flipsky vesc?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-21T19:26:39.748Z Reads: 138

```
Did you change the baudrate and set the vesc to ppm and uart?
```

---
## \#3 Posted by: Hoho0220 Posted at: 2018-12-21T19:31:15.898Z Reads: 131

```
No.
Do You use the flipsky with hm 10  ?
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-21T19:37:18.674Z Reads: 123

```
I have two Flipsky 6.6 and they work with bt modul.
Try to set the baudrate to 9600 and in your ppm settings change to ppm and uart than it should work
```

---
## \#5 Posted by: Hoho0220 Posted at: 2018-12-21T19:40:44.932Z Reads: 118

```
So I need use micro usb cable change the baudrate 
Right?
```

---
## \#6 Posted by: Hoho0220 Posted at: 2018-12-21T19:42:18.044Z Reads: 117

```
Do you use  ACKMANIAC-ESC Monitor?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-21T19:46:57.491Z Reads: 117

```
No I use the vesc tool, but it’s the same Menü.
Yes you need to connect your laptop to the vesc.
Go to ppm settings.
There you can change from ppm only to ppm and uart 
Than go to the uart menu and change the baudrate from 115000 or so to 9600.
Don’t forget to upload the new settings to the vesc. After that it should work.
If no, send some screenshots from your actual settings. 
There could be also rx and tx be mixed up, but that would be only second option,
Try first to change the settings.
```

---
## \#8 Posted by: adrienfeve Posted at: 2018-12-23T12:03:24.912Z Reads: 102

```
I have the same issue on my Flipsky vesc 4.12.
I already tried another bt module.
I set the baudrate to 9600.
I set the vesc to PPM + UART.
I checked the connections of TX and RX.

Still not working so I am thinking of trying Ackmaniac firmware instead of the standard 3.39 I use at the moment.

Will let you know if this works.
```

---
## \#9 Posted by: Hoho0220 Posted at: 2018-12-24T01:33:14.386Z Reads: 99

```
[quote="adrienfeve, post:8, topic:78643"]
Still not working so I am thinking of trying Ackmaniac firmware instead of the standard 3.39 I use at the moment.
[/quote]

thank you I ask arcboard team.
they said to upgrade the frimware to 3.4
```

---
## \#10 Posted by: Hoho0220 Posted at: 2018-12-24T03:24:33.696Z Reads: 93

```
Flipsky told me you need change the baudrate to 9600
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-24T06:22:39.862Z Reads: 89

```
if it´s an standard hm10 bt module it does not have anything to do with the firmware version.
who ever told you that...
```

---
## \#12 Posted by: Hoho0220 Posted at: 2018-12-24T07:41:16.744Z Reads: 89

```
https://flipsky.net/blogs/vesc-tool/having-trouble-using-flipsky-bluetooth
```

---
## \#13 Posted by: Andy87 Posted at: 2018-12-24T07:45:09.889Z Reads: 88

```
that´s a good description!
but nowhere written you need to update your vesc firmware... (as min i didn´t see)
```

---
## \#14 Posted by: Hoho0220 Posted at: 2018-12-24T07:56:57.736Z Reads: 87

```
3.38 Frimware cannot use vesc tool 0.95 need to 3.40
```

---
## \#15 Posted by: Andy87 Posted at: 2018-12-24T08:09:13.786Z Reads: 82

```
that´s right, but it has nothing to do with your bt module...
the bt module will work with any fw.
you just need the right service programm fitting to your installed fw to change the settings.
you can use an other version of vesc tool which is compatible with fw 3.38 and than it will work too.
```

---
## \#16 Posted by: Hoho0220 Posted at: 2018-12-24T08:41:06.318Z Reads: 80

```
Seem need to upgrade the ACKMANIAC firmware it will be ok
I used old vesc non-flipsky
use the vesc tool 0.95 to FW 3.4 app no information 
use the ACKMANIAC vesc tool to FW 3.101 app with information it work in good condition
```

---
## \#17 Posted by: adrienfeve Posted at: 2018-12-26T16:36:20.036Z Reads: 68

```
Thanks installed ackmaniac FW and I now have the data coming with bluetooth. So cool :)
```

---
## \#18 Posted by: buildityourself Posted at: 2019-01-08T03:33:01.998Z Reads: 56

```
Does anyone have a flipsky fsvesc and like it? Has anyone seen any consistent issues with them?
```

---
## \#19 Posted by: adrienfeve Posted at: 2019-01-09T22:09:30.235Z Reads: 54

```
It's good I have no issue with it and only paid it 50€. It now works with Bluetooth since I change the firmware to ackmaniac
```

---
## \#20 Posted by: buildityourself Posted at: 2019-01-09T23:36:16.583Z Reads: 49

```
Probably the best vesc for the money on the market, I got it, such a deal
```

---
