# Programming vesc via Bluetooth port?

### Replies: 20 Views: 340

## \#1 Posted by: 12meterkuk Posted at: 2018-08-06T09:30:12.030Z Reads: 96

```
I know this can be done via Bluetooth directly like the trampa bt module but is there anyway to connect it to my pc from that port? My USB port broke and it took one of the solder pads with it so it’s going to be near impossible for me to fix and finding an expert to fix costs way too much. Thanks
```

---
## \#2 Posted by: Kug3lis Posted at: 2018-08-06T09:30:59.195Z Reads: 97

```
You can also get USB - UART module and just plug tx/rx and ground and program it
```

---
## \#3 Posted by: 12meterkuk Posted at: 2018-08-06T09:31:56.282Z Reads: 90

```
Ok thanks!
```

---
## \#4 Posted by: 12meterkuk Posted at: 2018-08-06T09:36:23.624Z Reads: 90

```
Only rx , tx, and ground need to be plugged in? What about 5v?
```

---
## \#5 Posted by: Kug3lis Posted at: 2018-08-06T09:43:29.536Z Reads: 87

```
5V is needed if you need to supply voltage to the device for e.g. bluetooth, but as your USB-Uart runs from usb it doesn't require power
```

---
## \#6 Posted by: 12meterkuk Posted at: 2018-08-13T13:12:41.013Z Reads: 58

```
I just got the usb to yard thing and I’ve plugged in ground rx and tx but after messing around with the switches on the pcb the most I can get is the rx and txt lights to come on but not usb. This only happens when I accidentally plugged ground to 3v3 and no lights come on any other way
```

---
## \#7 Posted by: 12meterkuk Posted at: 2018-08-13T13:32:44.605Z Reads: 55

```
@Kug3lis  it works on my Mac, all 3 lights on with only rx tx and gnd plugged , but still nothing shows on the tool,
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-08-13T13:34:18.174Z Reads: 56

```
what cable you got maybe you need drivers for it. Can you open terminal and write:

```ls -l /dev/tty.*```
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-08-13T13:35:03.275Z Reads: 56

```
![image|375x500](upload://4rg0PjmHv77yfX87NR7rOhluO77.jpg)this is what it looks like now
```

---
## \#10 Posted by: 12meterkuk Posted at: 2018-08-13T13:36:09.450Z Reads: 50

```
@Kug3lis nothing appears on the terminal when I type it. Where can I find the drivers for it?
```

---
## \#11 Posted by: Kug3lis Posted at: 2018-08-13T13:42:13.236Z Reads: 48

```
Can you open `System Information` and make screenshot of USB devices?
```

---
## \#12 Posted by: 12meterkuk Posted at: 2018-08-13T14:24:38.577Z Reads: 45

```
![image|374x500](upload://f1pGvlQi3k4Qz6mZHgXDOk3AHyS.jpg)@kug
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-08-13T14:27:38.486Z Reads: 43

```
The last one usbmodem should appear in the tool under serial port list
```

---
## \#14 Posted by: 12meterkuk Posted at: 2018-08-13T14:42:21.726Z Reads: 41

```
@Kug3lis I’ve  tried both MAC and windows and they both have the USB lights blinking now and I’ve installed the Drivers but still nothing under the serial connections
```

---
## \#15 Posted by: Kug3lis Posted at: 2018-08-13T14:45:54.744Z Reads: 37

```
Can you show me your vesc tool screen under connection tab? with the list of port select box?

Because serial port is definitely opened I see it in terminal, maybe also try to swap TX/RX
```

---
## \#16 Posted by: nuttyjeff Posted at: 2018-08-13T15:04:13.624Z Reads: 36

```
tx to rx and rx to tx pins?
```

---
## \#17 Posted by: 12meterkuk Posted at: 2018-08-13T15:12:53.941Z Reads: 36

```
@Kug3lis I swapped rx and tx with same result ... :(![image|374x500](upload://bk3DO7oN7Qj3OGsZjC3bgSQ866a.jpeg)
```

---
## \#18 Posted by: 12meterkuk Posted at: 2018-08-13T15:14:46.313Z Reads: 34

```
![image|375x500](upload://n9N56EkHNDLveZlHFVxNZHpL1By.jpg)btw what do these 3 switches do?
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-08-13T15:18:38.945Z Reads: 34

```
To tell you the thruth I don't know this adapter so can't tell you much, but I think something is bad as RX/TX should only light then there is some traffic on signals. Maybe check your wires. Also what kind of dinosaur is your VESC Tool?
```

---
## \#20 Posted by: 12meterkuk Posted at: 2018-08-13T15:20:48.574Z Reads: 34

```
Haha I didn’t bother to download the new VESC tool yet. Does that mean this Focbox is fried ?
```

---
