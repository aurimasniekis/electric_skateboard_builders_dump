# Vesc problem need help

### Replies: 26 Views: 1413

## \#1 Posted by: Takis Posted at: 2017-08-24T06:34:24.297Z Reads: 97

```
Hi guys , I'm having a Maytech VESC , I had connect it to pc several times but now I can't I tried different laptops a desktop pc still nothing , I've installed every possible driver for the ports for the chips for everything so it's NOT a computer issue , the vesc should have a problem , Amy ideas , the throttle works ok (which means the firmware and the settings are getting loaded ,it's been tuned to work with pulse). My question is it's probably a broken chip or sth , can I change it or any cheap and fast way to repair it ? Thaaaaaaaaaaaaanks a lot
```

---
## \#2 Posted by: Takis Posted at: 2017-08-24T06:37:09.619Z Reads: 97

```
When I plug the battery the red led flashes 3 times so I know that it loads the firmware afterwards I have that blue light on which I think is normal ! <img src="/uploads/db1493/original/3X/4/6/4652326c8a424aa33be32390f9b2de5fa0bdfdd4.jpg" width="666" height="500">
```

---
## \#3 Posted by: L3chef Posted at: 2017-08-24T06:40:36.982Z Reads: 89

```
Have you tried different usb cables?
```

---
## \#4 Posted by: Takis Posted at: 2017-08-24T06:59:21.370Z Reads: 83

```
3 different cables
```

---
## \#5 Posted by: L3chef Posted at: 2017-08-24T07:30:25.193Z Reads: 80

```
So what happens when you press connect in bldc tool?
Any error text showing ?
```

---
## \#6 Posted by: Takis Posted at: 2017-08-24T07:36:22.524Z Reads: 80

```
It cannot recognized from PC as a serial port (it finds com1 but it doesn't change no matter where I have the vesc or even if is not connected , I've tried to find where the com 1 is but no luck with that , in both 3 pc's it finds it as unknown device no matter if I install the drivers
```

---
## \#7 Posted by: rich Posted at: 2017-08-24T07:48:13.613Z Reads: 76

```
Did you connect the vesc first and after that opened BLDC Tool? Because if not, BLDC Tool doesn't recognize the proper COM port. In my case (laptop) it works on one of 3 usb ports only. BUT the first time it took about 2 minutes after plugging the vesc until the laptop started to install some drivers. I thought there is a problem but the problem was me :joy:, be patient and wait after connecting the first time, hope that helps
```

---
## \#8 Posted by: Takis Posted at: 2017-08-24T08:11:29.322Z Reads: 72

```
There is no driver issues I have test it in 3pc's I've installed every driver ! I think the problem is in the vesc and I don't know what to do I have take out the outer tube and I don't have guarantee 😢😢
```

---
## \#9 Posted by: rich Posted at: 2017-08-24T08:29:17.160Z Reads: 72

```
[quote="Takis, post:8, topic:31375"]
I have take out the outer tube and I don't have guarantee :cry::cry:
[/quote]

Guarantee? maytech? :joy::joy::joy:

[quote="Takis, post:1, topic:31375"]
I had connect it to pc several times but now I can't
[/quote]

So it was once opened with BLDC Tool and you were using the vesc already?
```

---
## \#10 Posted by: Takis Posted at: 2017-08-24T08:47:25.894Z Reads: 66

```
i was using the VESC for 2 weeks , i did something stupid once i connected the capacitors reverse and the were killed (i changed them ofc) but i tested the vesc after that and it was working . after one day the laptop i was using died , the vesc still works but i cant connect it with any pc for some reason . Will in aliexpress says garantee void if tube is removed :P .
```

---
## \#11 Posted by: rich Posted at: 2017-08-24T09:03:29.066Z Reads: 64

```
Hmmm... I don't think it's the vesc but I'm no expert. I've read about connecting problems with newer operation sytems, I use old Windows 7 Laptop. Or you could try it with linux (don't ask me for details, I have no idea :joy: ). But when you're shure it's not the computer, it could help when you upload close up pictures of both sides of the V4.12, so experts can take a look in case there's something wrong on your pcb. One of my maytechs had a cold solder joint.
[quote="Takis, post:10, topic:31375"]
Will in aliexpress says garantee void if tube is removed :stuck_out_tongue:
[/quote]

How long the guarantee should be?
When I claimed mine at maytech I never got answer and when I claimed both faulty flier V4.12 in england I got the answer: there's no guarantee on vescs :joy:
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-08-24T09:12:34.219Z Reads: 61

```
Maybe try to connect the vesc on an other PC with the usb cable that worked before. Could be a driver issue somehow on your machine.
If the other PC is also not able to connect, focus on vesc repair or getting a new one
```

---
## \#13 Posted by: Takis Posted at: 2017-08-24T09:26:06.520Z Reads: 61

```
Buying a new one will cost time and money , im trying to find a cheap and fast solution like change some chip or something like that ;)
```

---
## \#14 Posted by: Takis Posted at: 2017-08-24T09:26:56.648Z Reads: 59

```
Thats not the best thing to hear :P :P :P  after that what did you do ?
```

---
## \#15 Posted by: rich Posted at: 2017-08-24T09:44:56.946Z Reads: 57

```
Crying for some days and ordered quality ones. I fixed the cold solder joint, both maytech's are working in sensorless BLDC mode but not in FOC what I need. If you need a quick solution I would sell one of mine for 75€ (with bootloader and bug free FW 2.18). Used them for a couple of days only. Or my Flier V4.12 for 60€ (broken hall sensor ports and temp sensors, but never had problems because they have massive heat sinks), you can PM me if you are interested. But I hope that you can fix your vesc.......
```

---
## \#16 Posted by: Takis Posted at: 2017-08-24T09:49:02.127Z Reads: 60

```
Thanks a lot man I will take it out of the box and see if there is any problem with the soldered parts in vesc , one friend told me to buy a programmer btw (if you have any tips) and I'll contact you if I need 😁Thanks a lot
```

---
## \#17 Posted by: rich Posted at: 2017-08-24T10:04:25.333Z Reads: 59

```
[quote="Takis, post:16, topic:31375"]
Thanks a lot man I will take it out of the box and see if there is any problem with the soldered parts in vesc
[/quote]

Take pictures and post it here as I did because in my case I didn't see the cold solder joint, that needs experts to watch. 

[quote="Takis, post:16, topic:31375"]
one friend told me to buy a programmer
[/quote]


But if it's the vesc a programmer won't connect, too I think.
```

---
## \#18 Posted by: Takis Posted at: 2017-08-24T10:07:11.656Z Reads: 56

```
well i study electrical engineering , i think i can find but it the current case its not that easy :P
```

---
## \#19 Posted by: onepunchboard Posted at: 2017-08-24T13:12:08.344Z Reads: 49

```
you won't get anything from maytech for sure. nor aliexpress. u can dispute them to f%%k them up. saying like fmw error and no connection. drag dispute as long as u can. this will hurt their reputaion. I'm upset they still sell these garbage dispite acknowledged issues
```

---
## \#20 Posted by: Takis Posted at: 2017-08-24T15:09:31.244Z Reads: 42

```
Here some photos from the vesc right now ! the arm chip gets really hot in seconds <img src="/uploads/db1493/original/3X/6/6/66521a67683b875223f8265886477cc226ebbc5c.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/3/d3fa25d953910b80349df89c2acdeafd644ca019.jpg" width="375" height="500">
```

---
## \#21 Posted by: Takis Posted at: 2017-08-24T15:21:01.630Z Reads: 42

```
Now for some unknown reason the vesc does not work at all and the arm chip it's burning after 5 seconds
```

---
## \#22 Posted by: Deckoz Posted at: 2017-08-24T17:11:40.586Z Reads: 38

```
probably killed the voltage regulator... or one of the diodes
```

---
## \#23 Posted by: Takis Posted at: 2017-08-24T17:20:15.555Z Reads: 39

```
One question is it worth repairing it ? I mean if it's not stm32f405(arm)  and its dvr or something else ? 😢
```

---
## \#24 Posted by: Deckoz Posted at: 2017-08-24T17:24:59.292Z Reads: 37

```
If you fried the STM32 chip, probably not unless you have an STlink to flash the bootloader after repair, as well you'll need to probe and identify all the components that are bad..
```

---
## \#25 Posted by: Takis Posted at: 2017-08-29T07:16:01.298Z Reads: 29

```
i was looking the VESC ,the transistor has some small "bubbles" and when i plug it , it gets real hot real fast :P , so i think its may be a shortcut, or just a broken transistor , does anyone faced the same problem ?
```

---
## \#26 Posted by: Takis Posted at: 2017-08-29T07:29:07.640Z Reads: 23

```
if anyone has VESC for sale (and willing to send in greece) send me working condition and price , thanks !
```

---
