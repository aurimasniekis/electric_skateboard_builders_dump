# Bms wiring issues

### Replies: 21 Views: 1332

## \#1 Posted by: dyingmoss Posted at: 2018-04-30T01:18:52.327Z Reads: 150

```
Hello everyone. I have been doing research and bought this all recently. Is this the correct wiring setup. Yes I know this is a crappy photo and can upload a better photo later.

![image|374x500](upload://yJuKk0iehIk1wgMRTCjU6oDftH5.jpeg)
```

---
## \#2 Posted by: Namasaki Posted at: 2018-04-30T01:55:15.038Z Reads: 137

```
Can’t tell anything by a photo. 
You need to make a diagram of your wiring so we can check it.
```

---
## \#3 Posted by: pixelsilva Posted at: 2018-04-30T02:12:09.159Z Reads: 132

```
....then I f... know jack about electric diagrams. That thing is just space science to me. Best thing for people like myself, rely on a battery expert. Don't pretend to be an Einstein. Let the experts (like @barajabali for example) handle these hook bag. :grimacing:
```

---
## \#4 Posted by: krloz Posted at: 2018-04-30T09:27:36.651Z Reads: 113

```
It's nearly impossible to follow any wire on that photo.  Try a diagram of what you think is correct and post it.  
But whatever you do. Take that away from that highly flammable rug
```

---
## \#5 Posted by: dyingmoss Posted at: 2018-04-30T13:37:07.041Z Reads: 111

```
![image|666x500](upload://bJdI22Fali2mXW5S1irpsp9af15.jpeg)![image|666x500](upload://x6Gj0azN3OqFYrlKG6davFkGmdu.jpeg)![image|666x500](upload://uONp92i0xhfsKWuU4yAo8CTSoy4.jpeg)

Is this better. 

![BMS 9s|690x388](upload://qshBYdA9HgHzKKCFSJs2iGS89cr.png)![G3P-Different Port 9S D223v1 Li-ion BesTech Power datasheet-01|353x500](upload://68rxg6LLT13tYfW4XdlkppnHqOc.jpg)

This is the diamgram I am using and this is the bms. 
@Namasaki @krloz oh and also just put it here because my workbench was to messy to spread it out.
```

---
## \#6 Posted by: krloz Posted at: 2018-04-30T13:54:38.739Z Reads: 96

```
I think your balance adapter is wrong.  Your first wire bring b- should go to the first battery first wire Erich toy have loose.  And then the last positive of the last battery would goo to the 9 balance wire. So you have to skip one wire position on all wires.  
Three part where you skip the negative of batteries 2 and 3 is ok
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-04-30T14:49:25.337Z Reads: 96

```
Also before pluggin it in for a test do ensure to do that on a safe fire resistant surface and not a hairy carpet.Also keep a metal container handy if you need to get rid quickly and a fire extinguisher too.

I see a lot of 'is this wired right?' threads on hairy carpets and I know someone's gonig to win a Darwin award sooner or later
```

---
## \#8 Posted by: dyingmoss Posted at: 2018-04-30T14:56:27.262Z Reads: 94

```
I guess I do not quite follow?
```

---
## \#9 Posted by: dyingmoss Posted at: 2018-04-30T15:17:55.172Z Reads: 91

```
What about this?
![image|571x500](upload://7gKV2BCq1JEasfG5llT9SDWTxnD.jpeg)
```

---
## \#10 Posted by: krloz Posted at: 2018-04-30T17:35:16.187Z Reads: 82

```
Can you take a picture of the bms connector for balancing.  I think I explained wrong
```

---
## \#11 Posted by: Acido Posted at: 2018-04-30T18:11:08.791Z Reads: 80

```
If you wrongly connect a bms it will just throw a small spark and thats it
Ask me how I know it
```

---
## \#12 Posted by: banjaxxed Posted at: 2018-04-30T18:40:59.585Z Reads: 76

```
If you get battery feed into the bms polarity wrong the bms will heat up very hot instantly with multiple lipos that's a possibility
```

---
## \#13 Posted by: Ethanstone Posted at: 2018-04-30T19:01:54.419Z Reads: 78

```
Hi,
I have just a had a similar problem and wondering how I should fix it. I recently hooked up a hobby king 6s BMS to my two 3s batteries in series to charge them like this like this: ![IMG_0669|375x500](upload://caGFtgNw6rEVEnNpCnrMjpiUwHq.JPG) A few minutes later it was on fire. Did I wire it wrong? Or did I get the wrong BMS? 
Here is the schematic of the BMS: ![22 PM|690x239](upload://aDhCel1fnUspoHBgA8zF2G710iP.png)
```

---
## \#14 Posted by: dyingmoss Posted at: 2018-04-30T20:51:18.596Z Reads: 75

```
I’m not currently at home, but the diagram for the bms I linked before is the bestech I have for a 9s
```

---
## \#15 Posted by: banjaxxed Posted at: 2018-04-30T20:58:44.563Z Reads: 78

```
Your pencil diagram has lots of wrong in it

If your bms has a B- & a P- this diagram should help
https://www.electric-skateboard.builders/t/help-with-charge-only-bms-wiring/5626/43

Read read read
http://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122

http://www.electric-skateboard.builders/t/two-questions-on-bms-wiring/30062/21
```

---
## \#16 Posted by: dyingmoss Posted at: 2018-04-30T21:17:18.925Z Reads: 72

```
Anything about my diagram?
```

---
## \#17 Posted by: banjaxxed Posted at: 2018-04-30T21:58:03.516Z Reads: 72

```
No anti-spark needed but lke this
http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/82?u=banjaxxed
```

---
## \#18 Posted by: Ethanstone Posted at: 2018-05-01T00:16:04.829Z Reads: 66

```
Hi,
I read the article, it was very helpful, but a few questions I have after reading them. One, it seemed in the first article that he was using the BMS to charge and discharge the batteries. Is it possible to only charge the batteries with that configuration? Two, he had seven balance ports on the BMS he had and on the BMS I had, I had only 6, do you know where the last balance cable goes? 

From what I read from the articles you suggested me is that the wiring should look like this: 
![32 PM|690x411](upload://aBU2Faeg2SpIGXNuHQ2Ti3KbNuX.jpg)
But in the diagram, there are only 3 balance cables per battery and I have 4 per battery. I know I ignore the second positive balance cable but where does the last balance cable go, the negative balance cable? If that doesn't make sense then here is a diagram: 
![IMG_0671|666x500](upload://omQithkRz5FXHa1HMnsTcxtDFWm.JPG)
```

---
## \#19 Posted by: banjaxxed Posted at: 2018-05-01T08:05:58.679Z Reads: 54

```
It goes nowhere, it's not used, a terminated wire. Ensure whatever is left cannot ground on anything
```

---
## \#20 Posted by: Ethanstone Posted at: 2018-05-01T15:16:13.827Z Reads: 49

```
Awesome. Thank you for helping helping me figure this out.
```

---
## \#21 Posted by: Ethanstone Posted at: 2018-05-01T15:45:06.461Z Reads: 46

```
Awesome. Thank you for helping me figure this out.
```

---
