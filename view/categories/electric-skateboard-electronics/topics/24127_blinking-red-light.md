# Blinking red light

### Replies: 21 Views: 1358

## \#1 Posted by: ArniJoronen Posted at: 2017-05-29T16:11:54.042Z Reads: 77

```
There is a major problem in my vesc i think.
The battery is going great. The motor is also good i think.
But when i look at the bldc tool i see this.
My vesc is blinking red and this happened when I was riding on flat ground and then it just cut out. Any ideas? 
My controller (normal RC controller) also is connected but the vesc is doing everything kill my fun. also there is a problem code DRV8302
<img src="/uploads/db1493/original/3X/2/4/24ec4b6dd4674eb7a0d38cb2268567ddd0857e6d.png" width="690" height="393">
```

---
## \#2 Posted by: Blasto Posted at: 2017-05-29T16:15:30.899Z Reads: 67

```
need more details...

what is your setup, screen shots of your motor configuration tabs...
```

---
## \#4 Posted by: ArniJoronen Posted at: 2017-05-29T16:18:32.088Z Reads: 65

```
here<img src="/uploads/db1493/original/3X/6/e/6e91115b29281c70c4d3025f55f5734982ce8070.png" width="690" height="387">
```

---
## \#5 Posted by: Blasto Posted at: 2017-05-29T16:20:48.345Z Reads: 60

```
what is your setup, what type of batteries, how many cells. what type of motor.

screen shot of the BLDC tab.

did you do a motor detection?
```

---
## \#6 Posted by: ArniJoronen Posted at: 2017-05-29T16:24:24.241Z Reads: 60

```
My setup is normal space cell from raptor 1 enertion r spec (the bigger) motor 
and vesc <img src="/uploads/db1493/original/3X/3/1/318cce04ec717510afb9d2bf51f3811db234eb09.png" width="690" height="376">
```

---
## \#7 Posted by: Blasto Posted at: 2017-05-29T16:32:27.991Z Reads: 55

```
when you go in the terminal and type "faults"

what appears
```

---
## \#8 Posted by: ArniJoronen Posted at: 2017-05-29T16:34:50.705Z Reads: 55

```
<img src="/uploads/db1493/original/3X/2/a/2a1ac6d37f86144f8e9d5543959952e8854c1c50.png" width="690" height="385">
```

---
## \#9 Posted by: ArniJoronen Posted at: 2017-05-29T16:36:23.568Z Reads: 50

```
here 
kdsvlkndvl
```

---
## \#10 Posted by: Blasto Posted at: 2017-05-29T16:39:33.164Z Reads: 51

```
well seems you have a hardware problem, i'm guessing you had this problem previously and tried upgrading the firmware to see if it would go away? 

what hardware revision of the vesc do you have?
```

---
## \#11 Posted by: ArniJoronen Posted at: 2017-05-29T16:40:38.667Z Reads: 49

```
i have 4.11 and i have upgraded just to 2.18 
and no, i have not had this problem ever
```

---
## \#12 Posted by: Blasto Posted at: 2017-05-29T16:43:31.613Z Reads: 45

```
so this problem appeared after updating to 2.18?

in the BLDC tab, do a detection and hit apply, the numbers are usually rounded, i'm not sure it likes fractions
```

---
## \#13 Posted by: ArniJoronen Posted at: 2017-05-29T16:44:44.301Z Reads: 43

```
no this problem occurred while i was going somewhere
and the settings are the same as normally, have been so for 2 years
```

---
## \#14 Posted by: ArniJoronen Posted at: 2017-05-29T16:45:18.010Z Reads: 42

```
and it doesnt make a difference
```

---
## \#15 Posted by: Blasto Posted at: 2017-05-29T16:51:36.701Z Reads: 39

```
does the motor even run when you do a motor detection?
```

---
## \#16 Posted by: ArniJoronen Posted at: 2017-05-29T16:53:44.710Z Reads: 40

```
i dont know how to do that
```

---
## \#17 Posted by: ArniJoronen Posted at: 2017-05-29T16:55:59.716Z Reads: 38

```
oh it will not spin or do anything when i detect
```

---
## \#18 Posted by: chuttney1 Posted at: 2017-05-29T16:57:10.857Z Reads: 37

```
When you get the DRV8302 error. This is pretty much the death of the device.
```

---
## \#19 Posted by: Blasto Posted at: 2017-05-29T16:58:04.530Z Reads: 37

```
[quote="ArniJoronen, post:17, topic:24127, full:true"]
oh it will not spin or do anything when i detect
[/quote]

you can always fix your vesc if you send it to a DRV wrangler. but ya, your vesc is damaged
```

---
## \#20 Posted by: ArniJoronen Posted at: 2017-05-29T16:59:49.483Z Reads: 37

```
now, and ok i will kill myself now jk
```

---
## \#21 Posted by: ArniJoronen Posted at: 2017-05-29T17:00:37.557Z Reads: 35

```
thank you for all the help and if there is a possibiliti to fix this i would be happy.
```

---
## \#22 Posted by: Blasto Posted at: 2017-05-29T17:11:32.406Z Reads: 37

```
[quote="ArniJoronen, post:21, topic:24127, full:true"]
thank you for all the help and if there is a possibiliti to fix this i would be happy.
[/quote]

well there's for repairs https://www.electric-skateboard.builders/t/johnny-vesc-repair-services-now-with-soldering-tips/11267?u=blasto

but if your vesc was running strong for 2 years and then went up in smoke, I suspect some debris cause this failure.
```

---
