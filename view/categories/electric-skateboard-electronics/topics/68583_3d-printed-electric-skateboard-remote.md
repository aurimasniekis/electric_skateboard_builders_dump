# 3D Printed Electric Skateboard Remote

### Replies: 14 Views: 465

## \#1 Posted by: 3Phase_Power Posted at: 2018-09-20T01:43:40.893Z Reads: 177

```
Hello, I am starting this thread to document and get feed back on my Esk8 remote. The reason I've decide to build my own remote is because in my opinion nothing on the market matches the comfortability and portability of the boosted board remote. I do not want to copy the boosted remote but rather improve on what I think is a great design. The features I want to implement are wireless charging, low cost(less then 20 dollars), single PCB solution, 600mAh battery. If you have any other features you would like to see implemented please feel free to add to the thread. My goal is to have this ready for the summer of 2019.   


Current design (MK1)
![20180919_210806|375x500](upload://uqLNFtNrs8Lwe2yPg9zaGtBsABs.jpeg) ![20180919_210801|375x500](upload://9gxRciHcxNxMN75cZt0psHtcdcV.jpeg) ![20180919_210755|375x500](upload://vdx9npet5EjLrby1qfxXqPvOm9o.jpeg) 

New design (MK2)
![20180919_213230|375x500](upload://i4ZaEZtMrk3M5fTzY9TZB0BbVmb.jpeg) ![20180919_213221|375x500](upload://g3sRbjPfCnlts8jQi4OHVtRXBJg.jpeg)
```

---
## \#2 Posted by: threebysix Posted at: 2018-09-20T02:15:03.373Z Reads: 151

```
have u considered the firefly remote @SeeTheBridges
```

---
## \#3 Posted by: Jc06505n Posted at: 2018-09-20T02:40:26.447Z Reads: 147

```
What I would like is a simple remote: 

Feels goods and won’t break upon being dropped

Have LED’s to start how basic info such as Board Battery Life , remote battery life, &  Connection status

With the most complicated thing on it Being a programmable multibutton
```

---
## \#4 Posted by: mmaner Posted at: 2018-09-20T02:46:49.196Z Reads: 138

```
Get a benchwheel remote. I have 3.  It has the basic functions, will take a beating, battery last forever.
```

---
## \#5 Posted by: Jc06505n Posted at: 2018-09-20T02:54:50.611Z Reads: 134

```
I have one but i have to order a receiver on the website.

I like it but it looks too much like a gun , and I rather not have the NYPD or some Uni guy call in a black guy flying around a piece of wood with a gun in his hands

![image|526x500](upload://29tfgxaA8S1nqZCcHt2nZSiQkOf.png)
```

---
## \#6 Posted by: mmaner Posted at: 2018-09-20T03:34:27.949Z Reads: 111

```
[quote="Jc06505n, post:5, topic:68583"]
black guy flying around a piece of wood with a gun in his hands
[/quote]

That sounds like something that happens in alabama. 

I can walk you through disassembling it and plasti-dip in orange (4-7 really light coats) fixes the gun look issue. The whole things takes less than half a day, mostly waiting on coats to dry. 

I just did this to my kids old benchwheel remote, it was scared up and ugly, now it looks brand new.
```

---
## \#7 Posted by: Socalscare Posted at: 2018-09-20T03:46:13.097Z Reads: 104

```
Following 🙂
```

---
## \#8 Posted by: 3Phase_Power Posted at: 2018-09-30T02:50:44.774Z Reads: 70

```
Update - CAD for remote body is mainly complete, next stage will be PCB development.
Current PCB component list 
-Atmega32u4 - MCU
-tp4056 - Battery Charger
-NRF24 - Data transmission
-LEDs - Battery level display
-hall effect sensor - Throttle position 
-400 to 600 mAh battey
-USB C - Charging and reprogramming 
![20180929_223643|375x500](upload://yuhjw4bHFTp8DJMDBrkVzfeZuBG.jpeg) ![20180929_223655|375x500](upload://5lBHBoRcgNhskYe7zrEmhByO3X9.jpeg)
```

---
## \#9 Posted by: StefanMe Posted at: 2018-09-30T08:43:25.865Z Reads: 60

```
I think u miss something here...  what makes the remote special when u don’t have a display to show awesome stats or smothering? This is just a remote like thousand others...
```

---
## \#10 Posted by: Jc06505n Posted at: 2018-09-30T12:00:00.872Z Reads: 55

```
Right now the only other BB like remote is the firefly , and no one has yet to make a production level feel one or at least one commercially available. Along with that , not everyone feels like using a UART port for a remote nor do some see the point of having a remote display stats while riding ( I personally don’t care , and would take either one)

So at the current moment , there is yet to be a BB-like remote without the extra display stuff out there and this guy is doing it right by adding usb-c support and sticking to led displays 

Sometimes keeping it stupid simple , is good. I for one am copping this remote next year.
```

---
## \#11 Posted by: 3Phase_Power Posted at: 2018-09-30T19:48:23.591Z Reads: 37

```
@StefanMe, this is meant to be a low cost remote ESK8 remote. Originally I wanted to add an OLED display to show things like range and battery level, but for these feature to be implemented the user must be using a VESC and at that point it would be much easier to just add bluetooth and pair it with a smartphone then trying to fiddle around with a 1 inch display on a remote.
```

---
## \#12 Posted by: 3Phase_Power Posted at: 2019-05-01T00:29:18.018Z Reads: 22

```
I haven't had much time to work on this but with summer coming I will eventually finish it this year. I have designed the PCB and updated the remote to be easier to print. The PCB should arrive in 2 weeks and I will post everything on GitHub. If there is interest I might sell a small quantity of these. I will post more updates with pictures later today with an updated feature list. 

![main|690x336](upload://gUyYPPyLmaok02sizNV7l77umS7.jpeg)
```

---
## \#13 Posted by: 3Phase_Power Posted at: 2019-05-01T22:09:42.433Z Reads: 17

```
![PIC_1|666x500](upload://xa10FgCDftbkddR9uGSmGOvk22t.jpeg) ![PIC_2|666x500](upload://ndyF7VvWfhTze60dBKMXWmfkfwa.jpeg) ![PIC_3|666x500](upload://m9wYOMuoaTYaB9dHCj9GgB0tYp5.jpeg)
```

---
## \#14 Posted by: 3Phase_Power Posted at: 2019-05-01T22:21:41.996Z Reads: 15

```
The current design features two bearings (9*5*3) which only cost 0.75 dollars and remove almost all play in the wheel. I still have to figure the LED placement that will display the remote battery level. I should be able the fit a 500mah battery (their is a lot of space left so technically the battery used can be of higher capacity) this should last for about 20 hours of operating time and a sleep time of about a 2 years (when the remote is turned off via a long press of a button the MCU goes into sleep). Currently I plan to use a Atmega328P with charging being done by USB C. The next iteration of the circuit  will feature wireless charging and the USB C port will be removed also I most likely will move to an ARM unit as the MCU. The receiver will be a similar in size to a RC remote receiver and connection to the ESC will be done via the standard servo connection. I will most likely post an update when I receive the PCB.
```

---
