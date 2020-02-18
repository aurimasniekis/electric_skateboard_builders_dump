# Trouble Updating Vesc 4.7 to newest Firmware

### Replies: 15 Views: 2474

## \#1 Posted by: shuey Posted at: 2016-03-09T14:11:38.346Z Reads: 98

```
Hello, I have a vesc 4.7 and I'm trying to update the firmware to 2.8 using a fresh ubuntu 15.1 install. I followed Vedders steps but when I get to the makeupload command, it fails everytime saying a target has deprecated and that I need to change a target. Up until this point the commands seemed to be working fine, and I think I just have to change a couple things in a config file somewhere, but i have no idea where to start. Thank you guys in advance for the input, hopefully we can get this working. I have a picture of the error in question here: http://imgur.com/QQtXPC1
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-09T15:27:33.514Z Reads: 97

```
Do you know if your VESC has a bootloader installed ?
Are you aware you can update the firmware using BLDC tool if your VESC has one installed ?
```

---
## \#3 Posted by: treenutter Posted at: 2016-03-09T15:43:57.708Z Reads: 94

```
@shuey It sounds like you're having the exact same problem I had when I [started this thread.][1]

If you need to install a bootloader, it's fairly straightforward but you need to get a STLink-V2 programmer. They're cheap, around $10-$15. Good luck!


  [1]: http://www.electric-skateboard.builders/t/vesc-installing-a-bootloader/752/33
```

---
## \#4 Posted by: shuey Posted at: 2016-03-09T16:27:21.281Z Reads: 92

```
@trbt555 I know it's supposed to, so I tried updating the firmware through the BLDC tool first, but it kept failing. My problem however does seem to be exactly like @treenutter 's though, but I won't actually be home to test it until Monday so when I get back I'll have to try playing with the pin connections some more. I actually did see your post because my pins are really weird too so I was referencing it trying to figure out my pin connections, I guess I just didn't scroll far enough to see the resolution. Thank you for the help, it seems like this is actually a really simple solution, I'll update you all when I get home on Monday.
```

---
## \#5 Posted by: treenutter Posted at: 2016-03-09T16:46:56.186Z Reads: 83

```
Awesome @shuey good luck with it!
```

---
## \#6 Posted by: shuey Posted at: 2016-03-14T21:50:57.937Z Reads: 72

```
So I've been working on this all day trying to get the VESC to work with no luck, I've double checked that the wiring is correct more times than I can count and I'm about 99% sure that isn't the issue. I've connected the vesc and I've run all the commands that I'm supposed to, but when I give the makeupload command for the bootloader I'm getting a failure. The red light on the back of the VESC is also flashing twice at a time, I'm not sure what that means, but I hope it's not bad.

All this seems A LOT like your problem @treenutter, but like I said, I've been working on this all day and I've been unable to emulate your success.

<img src="/uploads/db1493/original/2X/b/b1f8f96c9a13d25a7c9367ed01e0734164f394c5.png" width="690" height="388"> 

<img src="/uploads/db1493/original/2X/1/15427afe572d8816d92f723791792f12244e95e6.jpg" width="690" height="388">

<img src="/uploads/db1493/original/2X/f/f5c1b4d648f0dc527d8c0499a85c618a46bf37f3.jpg" width="690" height="388">
So I know the wiring is super messy, but the pinout for my st-link is here: 
http://www.st.com/st-web-ui/static/active/cn/resource/technical/document/user_manual/DM00026748.pdf on pages 12 and 13.

I have pin 19 connected to 3.3v, I have pin 20 connected to gnd, 15 to rst, 13 to data/whatever the unlabeled pin is, 9 to clk, and 7 to dio. I know this is a lot at once, but I really want to try to get this fixed and I'm hoping mine isn't part of the 4.7 flier batch which was mostly faulty.
```

---
## \#7 Posted by: treenutter Posted at: 2016-03-15T00:55:20.060Z Reads: 61

```
@shuey Nice work so far, you're getting close I'm sure of it! You're getting a low voltage error. I'm just guessing here, but why not try a different, shorter usb cable, or another USB port on your PC? Maybe there isn't enough power transferring to the VESC through the programmer? It looks like at least two of your cables are made from two different cables soldered together, check the length of those and the integrity of the soldering. Maybe there's a weak connection.

The clock speed error might also suggest that power isn't transferring properly, the error reports a lower clock speed than expected.

Also, where is the Cap on your VESC? I see a dean's connector but no cap? HW 4.7 uses a single capacitor between the battery and the VESC.
```

---
## \#8 Posted by: shuey Posted at: 2016-03-15T23:10:24.372Z Reads: 55

```
I've tried plugging it into a bunch of different USB ports including the 3.0 ports, and the results haven't changed, sometimes it just says flat out 0.000 volts, and I had the wires as short as I could make them thinking that would solve the problem, but I still had the same results, and the cables are longer, but it's because I took apart a female to female pin connection, so it should be a stable connection, I did that to make probing different pins easier since nothing was working. I might need to get a different ST link if it isn't providing enough power because I can't seem to get around that problem.

The cap isn't connected currently, its on the board, I was under the impression that it didn't need it when I was using the USB power.

Also do you know what the twice flashing red light on the vesc might mean? I can't seem to figure that out.
```

---
## \#9 Posted by: malik Posted at: 2016-04-11T23:57:53.285Z Reads: 45

```
In Makefile, comment the line 273 and uncomment line 274. If it does not work,  it might be Ubuntu 15. Try with Ubuntu 14. 
I am not saying your problems will be over though. I personally still cant make it work based on those advices but maybe it will be helpful to you. 
Let me know if you have solved your issue, maybe it could be helpful solving mine. (http://www.electric-skateboard.builders/t/vesc-4-12-unable-to-make-upload-the-firmware/2289)
```

---
## \#10 Posted by: shuey Posted at: 2016-04-13T14:48:50.688Z Reads: 42

```
@malik I actually solved the problem I was having, I should have followed up on here, but it turned out my ST-link was faulty, I ended up buying the same one @treenutter used and it worked fine... until my DRV died.
```

---
## \#11 Posted by: malik Posted at: 2016-04-13T16:34:11.320Z Reads: 43

```
@shuey good for you and good idea. I bought a new stlink, just waiting for the shipping. Sorry for your DRV though. 
I have a few VESCS on hand, which i had manufactured in case you would like to purchase one or two.
Cheers !
```

---
## \#12 Posted by: malik Posted at: 2016-04-13T16:38:28.134Z Reads: 42

```
By the way I have been using a Discovery board STM32F407G-DISC1 until now and the datasheet shows stlink/v2-A, dont know if that changes anything to my problem.
```

---
## \#13 Posted by: shuey Posted at: 2016-04-13T17:42:41.368Z Reads: 44

```
@malik thanks, it sucks the DRV's really seem to not like to work, luckily I have couple more vescs coming in soon, and I don't know if the stlink/v2-A really affects anything, but I'm also pretty new to playing with these boards and the hardware involved so I'm probably not the best person to ask haha. If you don't mind me asking though, how do you use the discovery boards, I keep seeing them brought up and people talking about them, but I have no idea how to use a discovery board to troubleshoot problems with the vesc, I've just been using an oscilliscope and manually probing contacts.
```

---
## \#14 Posted by: malik Posted at: 2016-04-14T11:50:31.650Z Reads: 42

```
Well I would love to ask the same question and I wish I could tell you exactly. I just bought it for the VESC, i am a total noob at it but besides uploading a firmware on the vesc, it can do much more: mp3 player, accelerometer etc. 
I am as well probably not the person to ask :smiley: 
But you can easily find on youtube some introductive videos about the Dicovery.
```

---
## \#15 Posted by: shuey Posted at: 2016-04-14T14:23:41.380Z Reads: 38

```
Haha, alright, I'll check that out
```

---
