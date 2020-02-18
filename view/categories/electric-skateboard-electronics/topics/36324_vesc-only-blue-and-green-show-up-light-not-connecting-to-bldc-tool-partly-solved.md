# VEsc only blue and green show up light not connecting to bldc tool/Partly solved

### Replies: 37 Views: 1513

## \#1 Posted by: vishal_tejwani Posted at: 2017-10-24T04:57:31.604Z Reads: 95

```
Any one can help where to check for drv error also it is only showing blue and green light what does that mean , i know my drv is blown but where to check in bldc that "drv error"...
```

---
## \#2 Posted by: vishal_tejwani Posted at: 2017-10-24T05:00:58.102Z Reads: 94

```
<img src="/uploads/db1493/original/3X/0/2/02f8b4a26134e16d74bc2bc49f78a831acbd42eb.jpg" width="374" height="500">
```

---
## \#3 Posted by: L3chef Posted at: 2017-10-24T05:01:02.819Z Reads: 91

```
Try in bldc tool / terminal and type in faults
```

---
## \#4 Posted by: vishal_tejwani Posted at: 2017-10-24T05:01:54.581Z Reads: 91

```
My vesc isnt connecting with computer
```

---
## \#5 Posted by: vishal_tejwani Posted at: 2017-10-24T05:05:17.026Z Reads: 89

```
Its showing no firmware read response
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-10-24T05:05:22.515Z Reads: 88

```
Try another USB cable Some USB cables only supply power, and don't have the extra data wires.
```

---
## \#7 Posted by: vishal_tejwani Posted at: 2017-10-24T05:05:46.877Z Reads: 88

```
Mine is from ardunio nano, it is a data cable for sure
```

---
## \#8 Posted by: vishal_tejwani Posted at: 2017-10-24T05:06:29.796Z Reads: 85

```
It is data cable
```

---
## \#9 Posted by: vishal_tejwani Posted at: 2017-10-24T05:06:43.761Z Reads: 84

```
Showing no firmware read response
```

---
## \#10 Posted by: L3chef Posted at: 2017-10-24T05:07:10.091Z Reads: 84

```
I had similar issues when I shorted the canbus. Maybe @JohnnyMeduse can help you
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-10-24T05:09:32.940Z Reads: 82

```
Also it might be worth installing some usb drivers for the STM32, just in case.
```

---
## \#12 Posted by: vishal_tejwani Posted at: 2017-10-24T05:10:21.022Z Reads: 80

```
I was actually thinking that , will try now
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-10-24T05:11:18.438Z Reads: 78

```
http://www.st.com/en/development-tools/stsw-stm32102.html
```

---
## \#14 Posted by: vishal_tejwani Posted at: 2017-10-24T05:22:18.684Z Reads: 72

```
installed drivers still shows no firmware read response
```

---
## \#15 Posted by: vishal_tejwani Posted at: 2017-10-24T05:26:09.231Z Reads: 71

```
installed drivers still same issue
```

---
## \#16 Posted by: vishal_tejwani Posted at: 2017-10-24T05:26:32.204Z Reads: 73

```
why are the blue light and green leds on vesc for?
```

---
## \#17 Posted by: vishal_tejwani Posted at: 2017-10-24T05:30:05.993Z Reads: 73

```
It worked , i typed faults it shows fault code none
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-10-24T05:31:07.187Z Reads: 74

```
Blue is power, dim green means it's running correctly. Bright green means it's outputting to the motor. Red means errors, three red flashes means DRV error specifically.
```

---
## \#19 Posted by: vishal_tejwani Posted at: 2017-10-24T05:32:15.247Z Reads: 74

```
no such thing , its showing no faults since startup
```

---
## \#20 Posted by: vishal_tejwani Posted at: 2017-10-24T05:33:09.958Z Reads: 76

```
there is no red led is flashing, there is dim green light, but there is hole in drv for sure
```

---
## \#21 Posted by: vishal_tejwani Posted at: 2017-10-24T05:34:00.618Z Reads: 73

```
there is no flashing of red led there is no drv error when i type faults in terminal
```

---
## \#22 Posted by: b264 Posted at: 2017-10-24T05:34:34.854Z Reads: 72

```
[quote="vishal_tejwani, post:20, topic:36324"]
hole in drv
[/quote]

What do you mean hole in drv?  Like, a physical hole and black charring?
```

---
## \#23 Posted by: MysticalDork Posted at: 2017-10-24T05:34:49.900Z Reads: 72

```
is it in the corner?
```

---
## \#24 Posted by: vishal_tejwani Posted at: 2017-10-24T05:35:01.055Z Reads: 72

```
black small point like
```

---
## \#25 Posted by: vishal_tejwani Posted at: 2017-10-24T05:35:26.696Z Reads: 71

```
yes...it is in corner
```

---
## \#26 Posted by: MysticalDork Posted at: 2017-10-24T05:35:52.221Z Reads: 71

```
like this? http://www.electric-skateboard.builders/uploads/db1493/original/3X/9/7/9751367e0c9e4b692171abd43c3a7e2a9874b3c4.jpg
```

---
## \#27 Posted by: vishal_tejwani Posted at: 2017-10-24T05:36:42.687Z Reads: 71

```
no no, i know that much of electronics, when ic gets blown tht type of thing
```

---
## \#28 Posted by: MysticalDork Posted at: 2017-10-24T05:38:00.221Z Reads: 72

```
just checking :P Sounds like you may have a blown drv. Seems like your main options are either get it replaced or get a new vesc.
```

---
## \#29 Posted by: vishal_tejwani Posted at: 2017-10-24T05:38:15.635Z Reads: 72

```
<img src="/uploads/db1493/original/3X/a/3/a3692c1be63e9f46d0c54508089df55245eb1852.jpg" width="666" height="500">
```

---
## \#30 Posted by: vishal_tejwani Posted at: 2017-10-24T05:38:36.803Z Reads: 71

```
but why i am not getting drv error and red flash of leds
```

---
## \#31 Posted by: MysticalDork Posted at: 2017-10-24T05:39:23.337Z Reads: 70

```
it's possible that it's so completely fried that it can't give an error.
```

---
## \#32 Posted by: vishal_tejwani Posted at: 2017-10-24T05:40:08.659Z Reads: 69

```
soo if i replace drv would it solve?
```

---
## \#33 Posted by: vishal_tejwani Posted at: 2017-10-24T05:40:39.878Z Reads: 66

```
soo if i replace drv would it solve??
```

---
## \#34 Posted by: MysticalDork Posted at: 2017-10-24T05:41:56.783Z Reads: 66

```
There's a pretty good chance that's the case. There's always a possibility that something else may be damaged or fried as well, but the DRV is definitely a first step. 

Do you have access to a hot air rework station?
```

---
## \#35 Posted by: b264 Posted at: 2017-10-24T05:42:49.939Z Reads: 68

```
You let the magic smoke out!  If you get the magic smoke back and put it back in the drv it will work again
```

---
## \#36 Posted by: vishal_tejwani Posted at: 2017-10-24T05:59:31.862Z Reads: 67

```
yes, i connected my remote as i hit ful throttle green led just lights up
```

---
## \#37 Posted by: vishal_tejwani Posted at: 2017-10-24T06:42:35.342Z Reads: 64

```
i cannot detect motor, but stll no error of drv
```

---
