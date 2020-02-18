# Vesc problems connecting

### Replies: 17 Views: 4063

## \#1 Posted by: Andy12 Posted at: 2017-04-06T21:39:27.309Z Reads: 298

```
I tried to connect my Vesc to my computer using a cable. It makes that sound sating that its connected but when I go on BLDC tool, and try to connec, it says Device not Found. Does anyone out there know how to fix this.
Do I have to connect my motor to the Vesc when planning on configuring it?
Is this a Vesc problem or Computer problem?
Thanks in advance
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2017-04-06T21:42:50.167Z Reads: 297

```
Is your VESC connected to power? It needs to be.
```

---
## \#3 Posted by: Andy12 Posted at: 2017-04-06T21:43:58.270Z Reads: 290

```
it is indeed
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-04-06T21:44:40.679Z Reads: 287

```
Click the drop down in the tool and see if there are any other available COM channels?
```

---
## \#5 Posted by: Andy12 Posted at: 2017-04-06T21:45:39.812Z Reads: 275

```
tried that doesnt work
```

---
## \#6 Posted by: Andy12 Posted at: 2017-04-06T22:21:01.128Z Reads: 269

```
when i click the tool on the top it doesn't show anything its just empty. may this be where the problem is starting
```

---
## \#7 Posted by: Andy12 Posted at: 2017-04-12T03:17:52.953Z Reads: 252

```
Can anyone send me a direct download link from their computer to my computer so i can get riding asap
```

---
## \#8 Posted by: Namasaki Posted at: 2017-04-12T04:41:29.009Z Reads: 238

```
Are you on Mac or PC

PC link: https://drive.google.com/file/d/0B0o_3IlBcNTlYVNvM2djaUFZZkE/view?usp=sharing
```

---
## \#9 Posted by: HeRowe Posted at: 2017-04-13T03:44:26.881Z Reads: 233

```
Hey! I'm having the same problem... I have two VESC's that I have tried and they both won't show up on the BLDC tool. There is no Com popping up in the drop down menu. I have the VESC connected to power and it displays the blue light, then three flashing reds ones before going back to blue. I'm thinking I might try getting a different Micro-USB cable

Got my BLDC from the link above. I'm on a PC running windows 7
```

---
## \#10 Posted by: Andy12 Posted at: 2017-04-13T03:47:34.370Z Reads: 224

```
I figured it out now. You have to go into your Driver Update something(the app on pc) and go to the one that has something to do with COM. double click that and go to the drever tab and click on update driver. then itll say something in the end like COM3 or something like that. Exit BLDC tool and reopen it. it then says your COM in the tab.
```

---
## \#11 Posted by: HeRowe Posted at: 2017-04-13T03:56:57.662Z Reads: 214

```
I'm not sure that I did it right... Do I need the VESC plugged in when I run the driver update? I'm looking in my device manager under the ports section because it has the work com there.
```

---
## \#12 Posted by: Andy12 Posted at: 2017-04-13T04:00:36.976Z Reads: 204

```
yah it should be connected
```

---
## \#14 Posted by: Andy12 Posted at: 2017-04-13T04:11:26.275Z Reads: 196

```
maybe these pics will help
.<img src="/uploads/db1493/original/3X/2/5/259491417845a6107bc967fd950dc8da7da7a6fe.PNG" width="304" height="459"><img src="/uploads/db1493/original/3X/0/e/0ed7baa0a7a6c1f6faf9cade81db00d47b712d90.PNG" width="236" height="275"><img src="/uploads/db1493/original/3X/4/8/48146dca8dfa4bfcb18b2060318b2b1d39f7d729.PNG" width="455" height="146"><img src="/uploads/db1493/original/3X/d/8/d85a6ef48b3db345784d61e03414ebb5edda72b9.PNG" width="523" height="208"><img src="/uploads/db1493/original/3X/2/3/23544789c4bbf89aa0d8d8e764f9f39afb582fd8.PNG" width="436" height="455">
```

---
## \#15 Posted by: Andy12 Posted at: 2017-04-13T04:15:09.005Z Reads: 173

```
so first you connect Vesc to power and to computer. Next you open up the driver update app on pc. then you click on the ports option. double click the option there is with the COM in it.Then you open up the driver tab and click on update driver 
. click the automatic one and then the option from the ports will come up. after the update go to the BLDC tool and hopefully youll see the COM port avaliable
```

---
## \#16 Posted by: HeRowe Posted at: 2017-04-13T04:19:08.957Z Reads: 167

```
Wow thank you so much!!! I got it working! Mine was displayed under the Other Devices section.
```

---
## \#18 Posted by: michichopf Posted at: 2017-04-23T11:26:45.868Z Reads: 151

```
Hey, having the same trouble connecting the vesc to the tool at a different computer. Tried your fix. didnt work for me :(
```

---
## \#19 Posted by: TinnieSinker Posted at: 2018-04-22T06:06:09.527Z Reads: 100

```
Thanks for the help!
I was having the same problem. ended up googling and downloading drivers for "stmicroelectronics virtual com port"

now everything works fine
```

---
