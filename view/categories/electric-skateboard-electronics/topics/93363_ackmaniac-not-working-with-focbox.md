# Ackmaniac not working with Focbox

### Replies: 18 Views: 235

## \#1 Posted by: Eskate444 Posted at: 2019-05-10T03:21:54.720Z Reads: 57

```
Hi all,

I recently upgraded my Focboxes from 2.8 to 3.56 using the vesc tool.

However the Ackmaniac app on android which i love using does not work with this firmware, do i have to rollback to get it to work or am i doing something wrong?

Firmware is 3.56 and HW is 410

Thanks
```

---
## \#2 Posted by: pookybear Posted at: 2019-05-10T03:48:54.388Z Reads: 52

```
You need to use the ackmaniac firmware.
```

---
## \#3 Posted by: Eskate444 Posted at: 2019-05-10T03:49:24.390Z Reads: 53

```
Can you link me please to it?

My original Raptor 2 firmware worked with Ackmaniac fine...
```

---
## \#4 Posted by: pookybear Posted at: 2019-05-10T03:50:11.873Z Reads: 52

```
Here you go:

https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#5 Posted by: pookybear Posted at: 2019-05-10T03:50:36.335Z Reads: 45

```
What esc are you using?
```

---
## \#6 Posted by: Eskate444 Posted at: 2019-05-10T03:50:51.980Z Reads: 44

```
Dual Focboxes
```

---
## \#7 Posted by: Jinra Posted at: 2019-05-10T03:51:44.431Z Reads: 41

```
probably the UART baud rate. Should be either 9600 or 115200. Whatever it is now change it to the other.
```

---
## \#8 Posted by: pookybear Posted at: 2019-05-10T03:51:50.073Z Reads: 41

```
Yep. Should work.
```

---
## \#9 Posted by: Eskate444 Posted at: 2019-05-10T03:52:33.113Z Reads: 41

```
I have tried both rates, none of them worked...
```

---
## \#10 Posted by: Eskate444 Posted at: 2019-05-10T03:52:55.700Z Reads: 41

```
Should i set to ppm and uart, or just uart?
```

---
## \#11 Posted by: Eskate444 Posted at: 2019-05-10T03:53:57.941Z Reads: 40

```
ACKMANIAC_ESC_TOOL_3_103

This is the latest firmware, i believe it should work if i flash as the "supported firmwares" list is lower than mine.
```

---
## \#12 Posted by: Jinra Posted at: 2019-05-10T03:54:51.946Z Reads: 40

```
that's fine
```

---
## \#13 Posted by: Eskate444 Posted at: 2019-05-10T03:56:44.869Z Reads: 40

```
Yes, finally it works, thank you guys!

I used the ackmaniac firmware.
```

---
## \#14 Posted by: pookybear Posted at: 2019-05-10T03:59:18.422Z Reads: 39

```
Some guy here was able to merge the low brake fix to the ackmaniac software. It's really good. It doesn't lock the wheels during low braking.

I'm going to see if I can find it. 

I'm using it on my vesc6.
```

---
## \#15 Posted by: Eskate444 Posted at: 2019-05-10T04:00:07.683Z Reads: 35

```
How was it done?
```

---
## \#16 Posted by: pookybear Posted at: 2019-05-10T04:01:18.513Z Reads: 37

```
Same way to flash it but hit custom and go to where you save the *.bin file.
```

---
## \#17 Posted by: pookybear Posted at: 2019-05-10T04:02:30.646Z Reads: 40

```
Here you go:

https://www.electric-skateboard.builders/t/vesc-based-controllers-brakes-locking-at-low-speed-for-larger-wheels-in-foc-possible-unity-fix/73547/155

Use it at your own risk. It's working great for me.
```

---
## \#18 Posted by: pookybear Posted at: 2019-05-10T04:03:13.924Z Reads: 38

```
Now, if it he low brake locking doesn't bother you, then keep what you have now.
```

---
