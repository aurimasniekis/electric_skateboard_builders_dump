# Hay I accidentally flashed the wrong firmware on my vesc.Help!

### Replies: 35 Views: 1566

## \#1 Posted by: Dariks Posted at: 2018-01-06T05:18:37.454Z Reads: 206

```
So I was trying to update my vesc and on one of them I wrote the wrong HW 48 instead of 4.12 its a vesc x. How can I fix this nothing burned I just can't re flash anything on it. Its a vescX 4.12
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:20:01.674Z Reads: 207

```
I think it is alright... On the new Firmware you have to select HW48

Edit: let me just check ...
```

---
## \#3 Posted by: Dariks Posted at: 2018-01-06T05:21:25.840Z Reads: 204

```
really I think something is wrong. when ever I plug it in it keeps blowing fuses. I checked the other ones and they are selected as 4.12hw
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:23:07.808Z Reads: 196

```
Which Version of the Vesc Tool are you using?
```

---
## \#5 Posted by: Dariks Posted at: 2018-01-06T05:24:26.598Z Reads: 190

```
checked the draw on a multi meter its drawing 120amps on a 10s that seems really high even my race quad doesn't draw that much
```

---
## \#6 Posted by: Dariks Posted at: 2018-01-06T05:25:21.846Z Reads: 182

```
the newest one with the wizards
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:28:27.364Z Reads: 182

```
[quote="Dariks, post:5, topic:42928"]
multi meter its drawing 120amps
[/quote]

well it could depend on the motor you have... but does the Focbox work, and which version of it you have (blue heatsink or Black heatshink)
```

---
## \#8 Posted by: Dariks Posted at: 2018-01-06T05:28:47.238Z Reads: 175

```
<img src="/uploads/db1493/original/3X/e/7/e7d843ddc559709666d89374b7842587188b0619.jpg" width="690" height="437">
```

---
## \#9 Posted by: Dariks Posted at: 2018-01-06T05:29:27.354Z Reads: 168

```
the foc box/ vescx is on 4.12 harware
```

---
## \#10 Posted by: Dariks Posted at: 2018-01-06T05:29:59.565Z Reads: 163

```
the one that works draws 40amps on the same motor
```

---
## \#11 Posted by: Dariks Posted at: 2018-01-06T05:30:25.159Z Reads: 160

```
blue heatsyncs
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:31:12.458Z Reads: 158

```
Yeah.... But there is 2 different Hardware 1.3 and 1.6, the difference goes with the heatsink color, but they are all base on the Vesc 4.12.
```

---
## \#13 Posted by: Dariks Posted at: 2018-01-06T05:31:21.543Z Reads: 152

```
It turns on and then as soon as i use the remote it blows my 60amp fuse
```

---
## \#14 Posted by: Dariks Posted at: 2018-01-06T05:32:15.008Z Reads: 152

```
it says 1.3v is that what your asking
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:33:39.760Z Reads: 152

```
Thank you. 

Are you able to run a motor detection?

and can you post some picture of it?
```

---
## \#16 Posted by: Dariks Posted at: 2018-01-06T05:34:40.530Z Reads: 153

```
Can not run anything on bldc or on the new vesc tool it says vesc too old
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:36:31.264Z Reads: 153

```
Weird... Have you tried the Old BLDC tool ?
```

---
## \#18 Posted by: Dariks Posted at: 2018-01-06T05:36:51.465Z Reads: 152

```
yep is it currupted?
```

---
## \#19 Posted by: Dariks Posted at: 2018-01-06T05:38:11.035Z Reads: 152

```
Can i send it somewhere to get it fixed or examined?
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:38:25.578Z Reads: 151

```
where are you located ?
```

---
## \#21 Posted by: Dariks Posted at: 2018-01-06T05:38:39.784Z Reads: 142

```
california USA
```

---
## \#22 Posted by: JohnnyMeduse Posted at: 2018-01-06T05:41:01.267Z Reads: 142

```
I've sent you a private message.
```

---
## \#23 Posted by: bevilacqua Posted at: 2018-01-07T00:14:20.773Z Reads: 127

```
if im not wrong you have to flash it with an ST-Link, I think it was already discussed in the main VESC/BLDC-Tool thread
```

---
## \#24 Posted by: Dariks Posted at: 2018-01-07T00:15:37.547Z Reads: 134

```
Thanks for the replay but I sent it over to johnnymeduse I think there may be more wrong then I know about.
```

---
## \#25 Posted by: PredatorBoards Posted at: 2018-01-07T00:38:58.608Z Reads: 130

```
Sounds like the bootloader is fucked. Get an ST-Link and some jumper wires.

http://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103

Here's a pretty easy guide how to do it. Good luck.
```

---
## \#26 Posted by: driver Posted at: 2018-04-23T18:07:44.454Z Reads: 101

```
Hey guys,

PLEASE HELP!

i flashed the wrong FW on my FocBox (HW 48). 
I bought the ST-Link.
Downloaded the Bootloader.
Put it on the Vesc via the ST-LINK Utility.

But, the FocBox still shows me the wrong FW:
![esc_tool|690x422](upload://4rAHO7RumNYJ6rzjcB5PQZ3qfUx.jpg)

The only option i have is the wrong HW Version.....what can i do?? :cry:
```

---
## \#27 Posted by: briman05 Posted at: 2018-04-23T18:21:50.862Z Reads: 94

```
I'm not sure you have to flash the focbox FW dont quote me but it is my understanding that they come pre tested and you shouldn't have to flash the FW
```

---
## \#28 Posted by: driver Posted at: 2018-04-23T18:54:36.162Z Reads: 93

```
i drove it for a year and wanted to update it... unfortunatly i choosed the wrong HW version
```

---
## \#29 Posted by: briman05 Posted at: 2018-04-23T19:10:43.130Z Reads: 85

```
Yeah I'm not sure how you would getting it to work try PM @JohnnyMeduse or @PredatorBoards
```

---
## \#30 Posted by: PredatorBoards Posted at: 2018-04-23T19:28:56.968Z Reads: 81

```
Click on **Show non-default firmwares** and see if you can pick out the right firmware version.
```

---
## \#31 Posted by: driver Posted at: 2018-04-24T05:24:45.721Z Reads: 69

```
Its not showing another Hardware Version..

How should it look like after i flashed the vesc with the ST-LINK?

![Unbenannt|690x427](upload://vzXOgUC5Cxm82zdRWCk5woomUNC.jpg)
```

---
## \#32 Posted by: danielz Posted at: 2018-04-24T06:11:26.859Z Reads: 68

```
Flash the entire firmware bin with stlink instead of just the bootloader. Thats why i did. I got the firmware from the bldc tools program files directory. Then after i fired up vesc tool and it updated to the latest.
```

---
## \#33 Posted by: driver Posted at: 2018-04-24T13:34:36.176Z Reads: 60

```
Thanks!
Where do i get the bin from???
```

---
## \#34 Posted by: danielz Posted at: 2018-04-24T17:41:38.723Z Reads: 55

```
I said where :laughing: i grabbed it from the bldc tool.
```

---
## \#35 Posted by: driver Posted at: 2018-04-24T20:26:03.879Z Reads: 52

```
:laughing: facepalm!
ok, but it didnt came with my version but i got from sombody.

Thanks man!
```

---
