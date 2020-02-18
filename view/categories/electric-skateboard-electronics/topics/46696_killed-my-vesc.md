# Killed my VESC :sob:

### Replies: 20 Views: 1324

## \#1 Posted by: MannyM0E Posted at: 2018-02-18T01:30:09.575Z Reads: 193

```
I plugged in a Bluetooth module onto the my vesc UART. Everything was working even the app was working for a moment, then the vesc stopped working. Any reason why ? The lights blue on the vesc, controller doesn't respond, Vesc tool don't detect it even my laptop doesn't even pick up anything when I plug it up and tried switching micro USB cables. Nothing 😭 Has anyone had this problem before ?

Using: 
DIY VESC 
Bluetooth module from MiamiEletric
Eskate app
```

---
## \#2 Posted by: SOICDIP Posted at: 2018-02-18T04:28:12.934Z Reads: 182

```
This can be tricky. 
Blue LED only means there is 3.3V, but the MCU might be the culprit. 

Notice anything burnt or shorted? Photos? 

Do you have an ST-Link?
```

---
## \#3 Posted by: MannyM0E Posted at: 2018-02-18T04:33:10.665Z Reads: 172

```
![image|375x500](upload://AmqcEly2LV6zB4BJwpVRMOxCcgy.jpg)
![image|375x500](upload://2PdwuL9MNPJ2gJ2lWMSFR1Kjqx5.jpg)
![image|375x500](upload://zgCpjw1NeRfld2i1ZgJZMBbOtex.jpg)
Posted better pictures 
 No burns or shorts that I notice.
Don't have a ST-Link. If I had one wouldnt it not work since the PC not detecting the VESC ?
```

---
## \#4 Posted by: SOICDIP Posted at: 2018-02-18T05:49:23.548Z Reads: 154

```
[quote="MannyM0E, post:3, topic:46696"]
Don’t have a ST-Link. If I had one wouldnt it not work since the PC not detecting the VESC ?
[/quote]


An ST-Link connects to the MCU's programming ports, so you can check whether the MCU is running or not.
```

---
## \#5 Posted by: MannyM0E Posted at: 2018-02-18T16:55:09.674Z Reads: 144

```
Could you tell me which st-link I need, there seems to be so many of them 

https://www.amazon.com/gp/aw/d/B072J7QKDJ/ref=mp_s_a_1_3/147-5469371-0099544?ie=UTF8&qid=1518972730&sr=8-3&pi=AC_SX236_SY340_QL65&keywords=st-link+v2&dpPl=1&dpID=41XFGkZgA8L&ref=plSrch

https://www.amazon.com/gp/aw/d/B01EE4WAC8/ref=mp_s_a_1_2?ie=UTF8&qid=1518972795&sr=8-2-spons&pi=AC_SX236_SY340_QL65&keywords=st-link+v2&psc=1

https://www.amazon.com/gp/aw/d/B01MZZ6USL/ref=mp_s_a_1_5?ie=UTF8&qid=1518972819&sr=8-5&pi=AC_SX236_SY340_QL65&keywords=st-link+v2&dpPl=1&dpID=411rmp-6xiL&ref=plSrch

https://www.amazon.com/gp/aw/d/B01N79YDJE/ref=mp_s_a_1_8?ie=UTF8&qid=1518972851&sr=8-8&pi=AC_SX236_SY340_QL65&keywords=st-link+v2&dpPl=1&dpID=41sSK8eGqfL&ref=plSrch
```

---
## \#6 Posted by: Lumaci Posted at: 2018-02-18T18:01:01.807Z Reads: 129

```
Any of them would work, but i would say get it on Ebay i paid 1 USD for mine took a week to arrive.
```

---
## \#7 Posted by: MannyM0E Posted at: 2018-02-18T18:07:30.551Z Reads: 132

```
Am I testing correct 

https://youtu.be/eEKUgpeASM8
```

---
## \#8 Posted by: MannyM0E Posted at: 2018-02-18T18:15:44.201Z Reads: 128

```
Thanks. Probably still get from Amazon for the prime. Really trying to figure out what's wrong with the vesc fast since this is my commute for work and home.
Edit: just bought will receive on Tuesday
```

---
## \#9 Posted by: SOICDIP Posted at: 2018-02-18T18:39:05.413Z Reads: 121

```
If this is time critical, you should send the VESC for repair or get a new one. If you're not familiar with electronics, this might take a while. 

Do you have a multimeter? 

When it's plugged in, do you feel any parts heating up? You should remove the shrink wrap for troubleshooting.
```

---
## \#10 Posted by: MannyM0E Posted at: 2018-02-18T18:43:14.132Z Reads: 117

```
Don't know nothing about electronic. I do have a multimeter, posted video and pictures up but doubt I'm using it correctly. As for the repair, I contacted the site but said I'll get a email response back from 24-48 hours
```

---
## \#11 Posted by: SOICDIP Posted at: 2018-02-18T19:01:32.905Z Reads: 110

```
You can use the diode mode of the DMM to see if something is shorted, but you were poking the top of the capacitors, which are not where the leads are. 

Once you get the ST-Link, hook it up like this:

http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752

You may need a JST-PH connector as well. 

If you don't have soldering experience and a component needs to be replaced, you should send it to one of the forum's VESC repair techs.
```

---
## \#12 Posted by: MannyM0E Posted at: 2018-02-18T19:13:54.489Z Reads: 99

```
Once I get the ST-Link I'll try that out as for the JSTPH Connecter I believe it comes with one. I order the purple one in that Amazon link I posted
```

---
## \#13 Posted by: SOICDIP Posted at: 2018-02-18T19:21:07.022Z Reads: 98

```
[quote="MannyM0E, post:12, topic:46696"]
as for the JSTPH Connecter I believe it comes with one. I order the purple one in that Amazon link I posted
[/quote]

Are you sure? I don't think it comes with a JST-PH connector. 

https://www.amazon.com/gp/aw/d/B01IZWYK7I
```

---
## \#14 Posted by: MannyM0E Posted at: 2018-02-18T19:24:57.357Z Reads: 89

```
Just ordered now 😊 Thanks
```

---
## \#15 Posted by: MannyM0E Posted at: 2018-02-18T19:41:15.286Z Reads: 87

```
C25 getting a reading 
![IMG_3561|375x500](upload://uheiWoAR4mPxVG05nWCLh54WWJx.JPG)

C33 getting a reading 
![IMG_3562|375x500](upload://2Tfpo5kz4k7p2shtrwJE1sfLzOY.JPG)
```

---
## \#16 Posted by: MannyM0E Posted at: 2018-02-18T20:59:55.584Z Reads: 86

```
It's over now I killed the vesc was testing the gnd and the 5v and this spark happened 😭![image|375x500](upload://fKF3rJzrKvQRjgAvfDJAj0FYYU4.jpg)
```

---
## \#17 Posted by: Sebike Posted at: 2018-02-18T21:42:08.294Z Reads: 78

```
Sorry to see that. Stay strong, brother! 💪🐰
```

---
## \#18 Posted by: Acido Posted at: 2018-02-18T22:08:36.156Z Reads: 73

```
Dude thats mental
When I was testing my vesc i was just poking around without any worry man i wad lucky

I know how it feels when you fry this expensive piece of electronics

I basically hit myself with a sledge hammer in my head for like 50 times then I went to sell my body for a focbox
```

---
## \#19 Posted by: MannyM0E Posted at: 2018-02-18T22:21:08.955Z Reads: 72

```
@Sebike thank you, I will be sending it to someone hopefully for repairs 

@Acido, it was because I had it powered on. I also touch the capacitor just for a split sec (not on purpose) and a little sparked happened. I disconnected the vesc right away, then replug again to see if it was working (wrong move, this caused a bigger spark) and this what it ended up to be
```

---
## \#20 Posted by: moon Posted at: 2018-02-18T23:42:19.277Z Reads: 60

```
I feel so lucky now, I got an focbox for 80 euros
```

---
