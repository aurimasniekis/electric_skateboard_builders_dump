# VESC UART only USB

### Replies: 14 Views: 1884

## \#1 Posted by: Workaround Posted at: 2016-08-15T14:51:04.527Z Reads: 154

```
I only see data from UART when the VESC is plugged in with usb. Is this normal?
```

---
## \#2 Posted by: hugohammarstrom Posted at: 2016-08-15T16:55:34.814Z Reads: 141

```
More information is needed. For example, how are you trying to read the UART data?
```

---
## \#3 Posted by: Workaround Posted at: 2016-08-15T22:51:49.623Z Reads: 122

```
I'm using TX and RX on the VESC directly to TX and RX on my arduino uno.

Vesc pin reference
https://github.com/vedderb/bldc-hardware

I did just find out that it is not the fact I need USB connection for it to work. It has to be connected to the outer shell of the USB which is ground on the USB. I have to touch it to GND on program port or USBs ground.
```

---
## \#4 Posted by: hugohammarstrom Posted at: 2016-08-15T22:54:33.780Z Reads: 110

```
Okey so everything good, problem solved?
```

---
## \#5 Posted by: Workaround Posted at: 2016-08-15T22:58:36.217Z Reads: 101

```
No I have to have the other end plugged into my Desktop. I'm not riding with a desktop.
```

---
## \#6 Posted by: hugohammarstrom Posted at: 2016-08-15T23:00:24.113Z Reads: 98

```
Are you using the power from the VESC to power the Arduino? If not this might be your problem.
```

---
## \#7 Posted by: Workaround Posted at: 2016-08-15T23:07:40.574Z Reads: 97

```
I can't confirm if that will make it work because power comes from the USB(cause I'm checking with serial over USB) on arduino to the VESC.
```

---
## \#8 Posted by: hugohammarstrom Posted at: 2016-08-15T23:10:16.568Z Reads: 88

```
Have you connected 5v(VESC) to VIN(UNO) and GND(VESC) to GND(UNO)?
```

---
## \#9 Posted by: Workaround Posted at: 2016-08-15T23:11:36.977Z Reads: 87

```
yes. That works but my when I plug USB into arduino it turns on VESC(Which is not connected to batteries). Which means it is pulling the power form my desktops 5v USB connection that is connected to Arduino for serial monitor.
```

---
## \#10 Posted by: hugohammarstrom Posted at: 2016-08-15T23:16:15.849Z Reads: 85

```
[quote="Workaround, post:1, topic:7673, full:true"]
I only see data from UART when the VESC is plugged in with USB. Is this normal?
[/quote]

I don't see how this would work without the VESC being plugged in with USB if you don't have the battery connected to the VESC. I feel like I'm missing something in your setup?
```

---
## \#11 Posted by: Workaround Posted at: 2016-08-15T23:34:15.404Z Reads: 76

```
So I plug my Arduino into my desktop which powers up the arduino with 5v from that USB connection. Then I plug in the VESC(which has no batteries connected) 5v wire into Vin(which has 5v from the USB being connected to my desktop). Ground on VESC to arduino ground also will link to the USB connected to my Desktop.


I hope that explains this. So the VESC is being powered with 5v so it is in a red then blue alternating lights state(which means it can't power motors but still send data on TX and RX).

So the problem is that I'm checking with Serial over USB on my desktop but I can't do that because it gives the 5v to the VESC. I can't confirm it works because I need the USB connected to my desktop to confirm.
```

---
## \#12 Posted by: hugohammarstrom Posted at: 2016-08-15T23:41:26.512Z Reads: 70

```
[quote="Workaround, post:11, topic:7673"]
So the problem is that I'm checking with Serial over USB on my desktop but I can't do that because it gives the 5v to the VESC
[/quote]

I don't see why the Arduino powering the VESC with 5v would be a problem, but yet again I'm not really understanding what your problem is. Are you getting any data from the VESC?

I'm sorry for not understanding it's late where I live :sweat_smile:
```

---
## \#13 Posted by: Workaround Posted at: 2016-08-15T23:44:17.876Z Reads: 64

```
Basically I don't want two 5v connections touching. But I will continue this later
```

---
## \#14 Posted by: hugohammarstrom Posted at: 2016-08-15T23:50:13.665Z Reads: 64

```
Okey, I think I understand now, maybe... :joy: you don't want the USB to be connected at the same time as the battery is connected to the VESC. 

If this is the case it shouldn't be a problem, but don't quote me on that. I've had the VESC powered from an Arduino while powering from a battery without any mishaps.
```

---
