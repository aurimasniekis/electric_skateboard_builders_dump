# Blown DRV8302 ? VESC not turning on

### Replies: 33 Views: 1497

## \#1 Posted by: goldrabe Posted at: 2018-02-27T12:32:24.738Z Reads: 155

```
Hi guys,
Is that a blown DRV and does it looks repairable?
VESC does not turn on anymore. I checked it with different wires. And the slave VESC still functions fine.![20180227_212422|690x388](upload://b7xDSuowD2ffExdScEc1fpz0zFx.jpg)
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-27T12:32:47.497Z Reads: 148

```
check the fault codes in bldc tool.
```

---
## \#3 Posted by: ElskerShadow Posted at: 2018-02-27T12:35:16.805Z Reads: 143

```
Type fault in the terminal after it’s plugged
```

---
## \#4 Posted by: goldrabe Posted at: 2018-02-27T12:36:54.034Z Reads: 142

```
Thanks man,
the VESC isn't connecting anymore.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-02-27T13:04:01.676Z Reads: 139

```
clean it with alcohol, there is lots of dirt around. Looks like there is solder bridging two pins on the DRV in the middle..
```

---
## \#6 Posted by: goldrabe Posted at: 2018-02-27T13:05:28.341Z Reads: 137

```
Thanks!
Will try that.
```

---
## \#7 Posted by: TarzanHBK Posted at: 2018-02-27T13:12:37.455Z Reads: 134

```
If you can´t solder on a new one, try @Martinsp or @fottaz. They both offer Vesc repairs here in the EU.
```

---
## \#8 Posted by: Martinsp Posted at: 2018-02-27T13:25:04.282Z Reads: 131

```
Yup, thank you for mentioning me @TarzanHBK 
You can check it out here 
http://electricskateboard.repair/index.php?id_product=12&controller=product
@goldrabe
```

---
## \#9 Posted by: goldrabe Posted at: 2018-02-27T13:38:53.770Z Reads: 123

```
Thanks for joining.
After a thorough cleaning i can not find any trace of damage. But the VESC still gives no sign of life. The blue light isn´t turning on. I was going over a bump when the VESC died. 
How can i troubleshoot further?
Btw. i am located in Japan, so shipping to EU is a pain.
I read so much warning about the Maytech shit...
Don´t have the money to get better ones at the moment and my board isn´t running F***ing SH*T.
```

---
## \#10 Posted by: Martinsp Posted at: 2018-02-27T13:40:59.837Z Reads: 112

```
I have not read through the thread but have you checked shorted ppwer lines to ground? The drv does not turn on if any led does not.
```

---
## \#11 Posted by: goldrabe Posted at: 2018-02-27T13:43:27.401Z Reads: 108

```
The VESC get´s hot when connected to the battery, i can not see any shorted power lines.
```

---
## \#12 Posted by: goldrabe Posted at: 2018-02-27T13:50:03.114Z Reads: 109

```
That's how the VESC looks after cleaning.![20180227_224656|690x388](upload://1VS1WlXMepG7zsqZM9HJT5bmAJq.jpg)![20180227_224549|690x388](upload://vGHQ7QXsg5FmopUOLwTEcJQ2e00.jpg)![20180227_224633|690x388](upload://qsp4JMfO8nv5JcXZ3e0UnBbWLhq.jpg)
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-02-27T13:50:53.410Z Reads: 102

```
From where you bought that VESC?
```

---
## \#14 Posted by: goldrabe Posted at: 2018-02-27T13:52:51.909Z Reads: 101

```
From Maytech in China directly.
```

---
## \#15 Posted by: banjaxxed Posted at: 2018-02-27T14:43:03.598Z Reads: 100

```
Did you use alcohol? did you give a good 'wash' with it and allow to dry properly? Looks a bit grimy still around the drv8302 chip and maybe usb too

no lights come on with power? no usb discovered on pc?
```

---
## \#16 Posted by: goldrabe Posted at: 2018-02-27T14:51:04.520Z Reads: 101

```
Yes led is not turning on no detection from usb.
I will try with more alcohol once again. 
Could the dirt be my only problem?
```

---
## \#17 Posted by: pennyboard Posted at: 2018-07-10T16:32:17.659Z Reads: 80

```
One of my Torqueboards vesc has the same issues. Doesnt turn on, no LEDs, and does not connect to my computer. It also gets hot when turned on. Did you ever figure out what the problem was @goldrabe?
```

---
## \#18 Posted by: sMATTEr Posted at: 2018-07-10T16:59:44.268Z Reads: 78

```
Try removing u401.

[quote="pennyboard, post:17, topic:47647, full:true"]
One of my Torqueboards vesc has the same issues. Doesnt turn on, no LEDs, and does not connect to my computer. It also gets hot when turned on. Did you ever figure out what the problem was @goldrabe?
[/quote]

> Blockquote
```

---
## \#19 Posted by: pennyboard Posted at: 2018-07-10T17:47:05.670Z Reads: 73

```
I am not very familiar with VESC layout. Is u401 a component or a does it refer to something plugged into a pin on the vesc?
```

---
## \#20 Posted by: Martinsp Posted at: 2018-07-10T17:57:41.492Z Reads: 72

```
It is the small 8-legged chip, CAN chip.
```

---
## \#21 Posted by: pennyboard Posted at: 2018-07-10T18:08:54.683Z Reads: 72

```
Okay, so should I simply remove it and try to power up, or does it need replacing before the VESC will operate? (I don't use CAN at all so if it's not needed to operate I won't replace it)
```

---
## \#22 Posted by: Martinsp Posted at: 2018-07-10T18:16:26.861Z Reads: 73

```
The VESC can work without it normally except the CAN feature
```

---
## \#23 Posted by: sMATTEr Posted at: 2018-07-10T18:34:07.648Z Reads: 71

```
As Martin said, CAN chip. I've had vescs blow that chip/and shorting the vesc without the user using CAN. I have no clue why, someone smarter might have a idea :wink:
```

---
## \#24 Posted by: goldrabe Posted at: 2018-07-10T23:31:56.565Z Reads: 65

```
Yes in my case, I shorted the CAN chip with a wrong cable supplied by Maytech themselves.
Martin fixed the VESC for me, i can vouch for his service. But in the end the Maytech VESC'S were of not really good quality and I replaced them with ESCapes from @stewii which work like a charm!
```

---
## \#25 Posted by: pennyboard Posted at: 2018-07-10T23:41:24.196Z Reads: 63

```
Yeah my next vescs will ESCapes for sure. 

Did the CAN chip break the VESC, or was simply removing it sufficient to get the VESC running again. In other words am I going to need a VESC repair or can I just remove the CAN chip?
```

---
## \#26 Posted by: goldrabe Posted at: 2018-07-10T23:51:37.594Z Reads: 63

```
I was, or I am using CAN, so Martin replaced the chip for me. But if he says removal is enough to get the VESC running again then i guess it's enough. (sorry, no VESC expert here) Martin's explanation was that the broken CAN chip is shorting the VESC and that is the reason why it can not power on.
@pennyboard
```

---
## \#27 Posted by: pennyboard Posted at: 2018-07-13T01:05:07.715Z Reads: 56

```
Would someone be able to tell where the CAN chip is located on the VESC?
@sMATTEr @Martinsp
```

---
## \#28 Posted by: sMATTEr Posted at: 2018-07-13T05:33:06.960Z Reads: 52

```
![image|374x500](upload://tg6ecjgvvzPmt1nINIYY3uNuxAY.jpeg)
```

---
## \#29 Posted by: ARetardedPillow Posted at: 2018-07-13T05:39:51.838Z Reads: 50

```
Guys, the blue sticker on there says "Destory, Invalid (Does not work)"  “摧毁 无效”
![image|690x330](upload://oRrymgi9M5vo5YQSi3wMthX4En1.png)
```

---
## \#30 Posted by: Sn4pz Posted at: 2018-07-14T03:44:32.967Z Reads: 48

```
wow they had the balls to send you some bad hardware!!!

time for an email to them!
```

---
## \#31 Posted by: banjaxxed Posted at: 2018-07-14T09:49:27.580Z Reads: 44

```
My guess is that this did not come directly from maytech, probably a vendor with access to the back door of the factory 

Even with the drv cleaned up looks like a bad one, probably the can chip if gets hot under power per previous comments

![IMG_9100|281x500](upload://qfLrg1Mqj0hW1JfhN1dKL3DYsgC.PNG)![IMG_9101|281x500](upload://xM4j3R2MBVSXPHYNAdL3m9o7BAY.PNG)
```

---
## \#32 Posted by: goldrabe Posted at: 2018-07-14T09:58:14.298Z Reads: 40

```
I've ordered my VESC's directly from Maytech and they both had this sticker on it. I think it's a warranty warning like "if this seal is broken your warranty will be invalid". But when I send them messages asking for warranty repair because they supplied the wrong cable i didn't got a single answer anyway. 😂
```

---
## \#33 Posted by: banjaxxed Posted at: 2018-07-14T12:48:18.543Z Reads: 37

```
I've never seen an ESC looking like that first picture brand new, it looks like it was dragged through a field backwards
```

---
