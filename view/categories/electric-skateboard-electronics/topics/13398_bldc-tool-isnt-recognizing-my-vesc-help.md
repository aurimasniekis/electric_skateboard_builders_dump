# Bldc Tool isn&rsquo;t Recognizing my Vesc HELP

### Replies: 8 Views: 1457

## \#1 Posted by: Zoomy Posted at: 2016-11-21T04:25:41.544Z Reads: 131

```
Hey guys, when I plug my vesc into my computer via the usb port after hooking it up to a power supply, a motor and a receiver, the bldc tool doesn't recognize it - as in nothing pops up under the 'serial connection' tab after clicking the refresh arrow.

I've tried Uninstalling and re-installing the bldc tool, using different usb cables, using my lipos instead of a laptop power supply and plugging it into a different usb port on my computer but none of this has resolved the issue so far.

The vesc has 4.12 written on it, I got it from enertion and the bldc tool is windows version and says it supports firmwares 2.17 and 2.18.

When I hook the vesc up to batteries, a blue light comes on followed by three flashes of red.

I've gone through all of the vesc setup and connection videos, however in all of them the vesc is recognized straight away so I'm pretty sure they can't help resolve this issue.

I'm not sure if this information is enough but I hope someone can help me out because I'm dying to get this thing going!!

Thanks heaps.
```

---
## \#2 Posted by: benwong Posted at: 2016-11-21T05:18:30.824Z Reads: 119

```
com port driver installed??
```

---
## \#3 Posted by: lowGuido Posted at: 2016-11-21T06:06:27.586Z Reads: 111

```
change the com port to another one and try again. mine is usually com1 or com4.
you can check your device manager to get the correct port number.
```

---
## \#4 Posted by: benwong Posted at: 2016-11-21T06:46:38.748Z Reads: 109

```
ya, check from device manager there. 
at first, my computer cant recognize my vesc port also. 
i update the driver then works~~
```

---
## \#5 Posted by: Zoomy Posted at: 2016-11-21T07:52:10.790Z Reads: 106

```
Thanks @lowGuido @benwong!! after clicking update it tells me that "windows could not find driver software for your device" and that I should check the support section for driver software for my device.

http://support.toshiba.com/support/driversResults?freeText=88265891Q&osId=31

Are any of these what I'm looking for?
```

---
## \#6 Posted by: benwong Posted at: 2016-11-21T08:01:37.792Z Reads: 100

```
i forget what is the driver name ady. 
you need refer to your missing driver name and update manually if auto update not working.
```

---
## \#7 Posted by: Oozytoast Posted at: 2017-04-15T14:10:03.322Z Reads: 76

```
I have to same problem when I plug other things into the USB port they are recognized but not the 2 vesc's 

I have tried two different vesc's powered by two different sources with 3 different cables 

The bldc tool is blank in the com port section no options for any ports
```

---
## \#8 Posted by: Zoomy Posted at: 2017-04-16T00:19:48.930Z Reads: 66

```
I found that using a different computer worked for me.
```

---
