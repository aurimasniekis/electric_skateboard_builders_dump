# Problems with vesc

### Replies: 60 Views: 666

## \#1 Posted by: Muffe Posted at: 2018-07-21T18:17:21.964Z Reads: 118

```
I have recently completed a build and I found the performance a bit underwhelming. I decided to optimize the vesc settings so I tried to connect my vesc to my computer. After a while i got it working so i decided to update the firmware. After this was done the board stopped working. It turns on but nothing happens and the remote controller connects. I dont get the same three blinking lights before i connect it to my computer. Right now i am basically stuck with a board that doesn't work so any help would be appreciated. Another thing to note is that when i tried to measure the L&R the board shut of after the motor made a sound, everything is fine and nothing got hot.

Edit: I have had this thread up for 12 days without any response so i would really appreciate any help possible.
```

---
## \#2 Posted by: amazingdave Posted at: 2018-08-02T14:05:00.908Z Reads: 77

```
Post screenshots of your VESC settings....
```

---
## \#3 Posted by: Andy87 Posted at: 2018-08-02T14:05:02.610Z Reads: 77

```
You load the right firmware which fit to your hardware?
```

---
## \#4 Posted by: Muffe Posted at: 2018-08-02T14:17:33.701Z Reads: 74

```
Hi, i am very new to the vesc tool. Where do i find the settings that you are after? :slight_smile:
```

---
## \#5 Posted by: Muffe Posted at: 2018-08-02T14:19:19.497Z Reads: 69

```
I have No idea, This is what it says when i read the firmware of the vesc.![Skjermbilde|690x387](upload://nMKJSbfnUHqtSLTUTmo57bjDb0K.PNG)
```

---
## \#6 Posted by: linsus Posted at: 2018-08-02T14:31:04.642Z Reads: 65

```
Do motor detection and when it doesnt go thru, go to the terminal tab and write "faults"
```

---
## \#7 Posted by: Muffe Posted at: 2018-08-02T14:47:28.358Z Reads: 64

```
how do you do motor detection. sry for being such a noob
```

---
## \#8 Posted by: Andy87 Posted at: 2018-08-02T14:47:32.161Z Reads: 61

```
Looks like you choose wrong hw😬
```

---
## \#9 Posted by: Andy87 Posted at: 2018-08-02T14:48:01.515Z Reads: 62

```
Which vesc you have? Or it’s focbox?
```

---
## \#10 Posted by: Muffe Posted at: 2018-08-02T14:48:25.743Z Reads: 65

```
i have a TB vesc 4.12
```

---
## \#11 Posted by: Andy87 Posted at: 2018-08-02T14:50:37.050Z Reads: 65

```
That should be based on hw 4.12
You choose the wrong hw version while flashing firmware 
You can see it, it’s written 48
But there should be different versions be available.
You need the one which fit to hw 4.10 4.12
```

---
## \#12 Posted by: Muffe Posted at: 2018-08-02T15:37:40.407Z Reads: 60

```
okay, thank you. I'll try that
```

---
## \#13 Posted by: Andy87 Posted at: 2018-08-02T15:43:06.527Z Reads: 60

```
In case you can’t reload your vesc you need to look here in the forum. Could be that you can load it with the bootloader and st link
```

---
## \#14 Posted by: Muffe Posted at: 2018-08-04T20:11:33.458Z Reads: 49

```
I am very sorry to interrupt you and use more of your time, but I can’t find the correct firmware. I don’t expect you to answer but it would be great.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-08-04T20:45:59.373Z Reads: 47

```
No problem.
Where you got the software from?
I mean where you downloaded the vesc tool?
On your picture you sent i can see that the right firmware not in the vesc folder.
Unfortunately I don’t know which folder it need to be (name and ending).
So, my easy way would be,
Ask here in the forum, or uninstall the vesc tool,
Go on the official vesc homepage and download again the service software.
Than open the vesc tool. Under firmware there should be not only 48, also 410,412 and some other hw should show up there.
Try this. If that‘s not functioning let me know.
I’ll have a look where to find the files.
```

---
## \#16 Posted by: Muffe Posted at: 2018-08-04T20:56:22.098Z Reads: 42

```
Wow, did not except a response, this forum is great!!!

Thanks for the help......Honestly

I’ll try your methods :smile:
```

---
## \#17 Posted by: Andy87 Posted at: 2018-08-04T21:05:30.783Z Reads: 44

```
We are all here to learn from each other😉
If you have any question than don’t worry to ask.
```

---
## \#18 Posted by: Muffe Posted at: 2018-08-04T21:11:13.062Z Reads: 47

```
okay, so i deleted the vesc tool and downloaded it again and this is what the starting screen looks like.![Skjermbilde%202|690x386](upload://nfqbjB7vFp2hqXi6YYQY07aL9o8.PNG)
```

---
## \#19 Posted by: Andy87 Posted at: 2018-08-04T21:14:32.013Z Reads: 45

```
Looks way much better
You have hw4.12 if I remember right.
So you need the firmware 410 411 412.
Last one
```

---
## \#20 Posted by: Andy87 Posted at: 2018-08-04T21:15:12.433Z Reads: 45

```
Try to flash your vesc with it again
```

---
## \#21 Posted by: Muffe Posted at: 2018-08-04T21:16:20.527Z Reads: 45

```
This is the error message that i get when i connect the vesc to my computer.![Skjermbilde%203|690x387](upload://5C7kLWYJBqC2RCZZyCCa1AOUvSq.PNG)
This is what is displayed when i am connected to the vesc.![Skjermbilde%204|690x387](upload://xsnNrYp2SPC2TYnuzQmXg3CExNn.PNG)
```

---
## \#22 Posted by: Muffe Posted at: 2018-08-04T21:16:55.669Z Reads: 42

```
what is flashing vesc?
```

---
## \#23 Posted by: Andy87 Posted at: 2018-08-04T21:18:41.937Z Reads: 43

```
Load the firmware with the right file
```

---
## \#24 Posted by: strattos Posted at: 2018-08-04T21:19:20.530Z Reads: 42

```
Updating the firmware so you can actually change parameters.
```

---
## \#25 Posted by: Muffe Posted at: 2018-08-04T21:21:45.666Z Reads: 45

```
well when i downloaded the program i only got one file.![Skjermbilde%205|690x387](upload://4ZnK1z1IywaVnQdERbgBFe2cWYn.PNG)
```

---
## \#26 Posted by: Andy87 Posted at: 2018-08-04T21:24:33.670Z Reads: 43

```
Look just connect your vesc
Open the vesc tool
Go to firmware 
Choose 410 411 412
Push the upload firmware button 
And hope that your vesc after change to the right firmware. You now have the firmware which fit to hw 48 but that’s not the right you need
```

---
## \#27 Posted by: Andy87 Posted at: 2018-08-04T21:26:41.726Z Reads: 42

```
Ok i have overseen one pic...
So it’s normal that you get this firmware too old message 
If you click ok you can upload the firmware?
Or you just see the 48 version after?
```

---
## \#28 Posted by: Muffe Posted at: 2018-08-04T21:27:38.871Z Reads: 43

```
when i click ''ok'' The firmware choices dissapear
```

---
## \#29 Posted by: Andy87 Posted at: 2018-08-04T21:34:08.766Z Reads: 43

```
Look through this thread 
https://www.electric-skateboard.builders/t/hay-i-accidentally-flashed-the-wrong-firmware-on-my-vesc-help/42928?u=andy87

I didn’t read through all of it but I think you have the same problem.
More down there should be a description how you can fix it. 
Could be that you need a st-link to get you back to the right firmware
```

---
## \#30 Posted by: Muffe Posted at: 2018-08-04T21:55:48.675Z Reads: 43

```
[quote="danielz, post:32, topic:42928, full:true"]
Flash the entire firmware bin with stlink instead of just the bootloader. Thats why i did. I got the firmware from the bldc tools program files directory. Then after i fired up vesc tool and it updated to the latest.
[/quote] 
Looks like i would need a st-link to fix it which seems taunting
```

---
## \#31 Posted by: Andy87 Posted at: 2018-08-04T22:01:31.787Z Reads: 43

```
Yes but that’s how it is.
I think this st-links not so expensive.
You could also ask here, maybe somebody will borrow or sell you one used.
```

---
## \#32 Posted by: Dariks Posted at: 2018-08-04T22:04:11.649Z Reads: 42

```
Yeah you need a st-link to fix that.
```

---
## \#33 Posted by: Dariks Posted at: 2018-08-04T22:05:29.902Z Reads: 41

```
also do not plug it in or it will blow your fuses.
```

---
## \#34 Posted by: Muffe Posted at: 2018-08-04T22:06:09.330Z Reads: 40

```
Yeah, i'll probobly send to someone.
```

---
## \#35 Posted by: Muffe Posted at: 2018-08-04T22:06:30.400Z Reads: 40

```
How do you know when fuses have been blown?
```

---
## \#36 Posted by: Dariks Posted at: 2018-08-04T22:06:59.612Z Reads: 39

```
The battery will not let you start the motor.
```

---
## \#37 Posted by: Muffe Posted at: 2018-08-04T22:10:45.031Z Reads: 39

```
Then some fuses are probably blown, You see the first thing i did after i thought i had updated the vesc with the right firmware was to plug it in and try to start it. I think i am just going to sell it to someone who has the experience and then just buy a new one.
```

---
## \#38 Posted by: Dariks Posted at: 2018-08-04T22:11:59.334Z Reads: 41

```
oh the fuses aren't on the vesc they are there to protect your battery usually in a black container made of plastic attached to the red or black wire.
```

---
## \#39 Posted by: Muffe Posted at: 2018-08-04T22:14:42.177Z Reads: 42

```
I have a tb vesc.

So the three round almost battery shaped things.
Sry for the horrific explanation
```

---
## \#40 Posted by: Dariks Posted at: 2018-08-04T22:15:55.983Z Reads: 42

```
Wait can I just see a pic of your setup? It would make it easier to explain. Make sure to show your batteries too.
```

---
## \#41 Posted by: Dariks Posted at: 2018-08-04T22:23:24.193Z Reads: 41

```
![image|500x500](upload://lpT1F2OfGmE6cOFj4qqr6VyTClN.jpg)
```

---
## \#42 Posted by: Dariks Posted at: 2018-08-04T22:24:45.139Z Reads: 41

```
looks like that you need to pull out whats inside and check if the metal is still fully attached sorta like a light bulb.
```

---
## \#43 Posted by: Muffe Posted at: 2018-08-04T22:26:26.937Z Reads: 41

```
![image|374x500](upload://oeDkbC1CTkuvTMPONoJfJZkPldO.jpg)

This is my setup
```

---
## \#44 Posted by: Muffe Posted at: 2018-08-04T22:27:20.214Z Reads: 40

```
The battery turns on and the built in USB port still works which Leeds me to believe that the battery is intact
```

---
## \#45 Posted by: Dariks Posted at: 2018-08-04T22:29:18.699Z Reads: 39

```
Ok that battery has a built in one of those so it kept it self safe. Its just the vesc.
```

---
## \#46 Posted by: Muffe Posted at: 2018-08-04T22:30:01.412Z Reads: 39

```
Ok, pm is prob only better for this
```

---
## \#47 Posted by: ThermalM16 Posted at: 2018-08-05T03:56:24.401Z Reads: 37

```
@Muffe did you get everything figured out? If not I have a gif floating around here somewhere that shows how to update a VESC with the new tool and some tips on how to set it all up
```

---
## \#48 Posted by: Andy87 Posted at: 2018-08-05T04:01:07.582Z Reads: 36

```
Don’t give up so fast😜
I don’t think that you have a serious hardware problem.
Just get a st-link and load the right firmware.
A st-link is way much cheaper than to buy a new vesc
```

---
## \#49 Posted by: danielz Posted at: 2018-08-06T23:07:20.745Z Reads: 39

```
Its easy peasy, and the stlink clones on ebay are very cheap
```

---
## \#50 Posted by: Muffe Posted at: 2018-08-07T09:40:20.545Z Reads: 38

```
I am still working on it :slight_smile:
```

---
## \#51 Posted by: Muffe Posted at: 2018-08-07T09:41:22.033Z Reads: 38

```
Yeah you’re probobly right.
```

---
## \#52 Posted by: Andy87 Posted at: 2018-08-07T09:55:32.129Z Reads: 34

```
ST-Link V2 Programming Unit Mini Metal H¨¹lle STM8 STM32 Emulator Downloader https://www.amazon.de/dp/B01F37YMJ4/ref=cm_sw_r_cp_api_i_bXwABb3932E44

2,50€ on Amazon... 😉
Give it a try. Nothing to lose.
```

---
## \#53 Posted by: Muffe Posted at: 2018-08-07T09:57:23.985Z Reads: 35

```
That seems like The best solution, is It very technical?
```

---
## \#54 Posted by: Andy87 Posted at: 2018-08-07T10:06:02.795Z Reads: 35

```
Never made. But theoretically no. Just hook up the right wires to your vesc, plug in the st link to your usb and flash your vesc via the vesc tool.
If you search here in the forum, you should find some information.
Or just ask in a new thread.
There are a lot of people who already made it.

By the way, just ordered one for me to have one in case i‘ll need one day😅
```

---
## \#55 Posted by: ThermalM16 Posted at: 2018-08-07T22:43:03.548Z Reads: 34

```
When you get it, you’ll want to download the software from the st link website and then flash your VESC with the FW provided by the VESC tool.
```

---
## \#56 Posted by: Muffe Posted at: 2018-10-21T11:28:17.802Z Reads: 26

```
hey, I am back. I have been trying to flash a new bootloader with the st-link but I am having problems. Whenever I try to upload the bootloader I get the error '' Readout protection is activated''. Does anyone know what to do, I haven't found anyone resolve this issue, can anyone help?
```

---
## \#57 Posted by: Andy87 Posted at: 2018-10-21T17:02:00.017Z Reads: 24

```
Maybe @Eboosted can help you
```

---
## \#58 Posted by: Muffe Posted at: 2018-10-21T19:51:19.681Z Reads: 26

```
Okay, i’ll ask
```

---
## \#59 Posted by: Eboosted Posted at: 2018-10-21T20:58:38.353Z Reads: 25

```
Hello:
I never heard of that message before when flashing the bootloader with a STLink, all I can see is that you wrote the incorrect firmware you should have written 4.12v instead of 48.

This has happened to me by mistake in the past and what you need to do is write the bootloader and firmware following the steps described the aforementioned post, check your VESC connections to STLink again and follow the steps slowly. 

If you already have done that I strongly suggest you get a focbox, install it and move forward, don't try to keep fixing the old one or you might get frustrated and leave the hobby forever, never experimenting such a rewarding feeling that is riding an electric sk8, just because a small piece of hardware failing on you. 

Btw, if you ever repair the tb vesc you should never use it in Foc, I saw you were measuring L&R, stick to BLDC and you will have a working board for years.
```

---
## \#60 Posted by: Muffe Posted at: 2018-10-23T13:10:32.620Z Reads: 14

```
okay, Maybe the problem is that i have another st-link, i have the authentic one. This one https://no.farnell.com/stmicroelectronics/st-link-v2/icd-programmer-for-stm8-stm32/dp/1892523
```

---
