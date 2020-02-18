# I might have &ldquo;bricked&rdquo; my esc. Help?

### Replies: 44 Views: 1184

## \#1 Posted by: Flasher Posted at: 2019-05-29T15:57:55.895Z Reads: 192

```
I just started building my first diy and wanted to program my dual fsesc6.6 to make sure everything. Being a noob in this category, I think I bricked the master side. It no longer lights up. At first I had two blue lights and two green lights. Now I only have one of the two green lights. I tried with ackmaniac esctool and with vesctool and I can't seem to get it back to where it was working. Any help or actual experience with this problem would be highly appreciated.
Before![15590745065856116932150683119174|375x500](upload://wzieeymj7euPFJ85GNGsMGqn2zh.jpeg) 
After![IMG_20190529_000402383|375x500](upload://5ZmjQUV3BHtNcNpNUAyJZz5iE9n.jpeg)
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-05-29T16:14:50.189Z Reads: 178

```
Unplug everything and check if there is a short between the 3.3V rail and ground. Probe on the SWD header. If not, then all you need is an ST link and to reflash the firmware. The firmware can be found on github, I'd recommend getting a nucleo-64 board from Arrow.com and using its embedded st-link.
```

---
## \#3 Posted by: Flasher Posted at: 2019-05-29T16:31:17.301Z Reads: 176

```
Thanks for the advice. Just checked, no shorts so I guess I f'ed up XD I'm gonna look into a stlink on amazon as in Canada I'm getting screwed on shipping fees and delays. I was basically trying to figure out why it doesn't want update to 60 hw and was stuck on 46
```

---
## \#4 Posted by: Gamer43 Posted at: 2019-05-29T16:44:08.262Z Reads: 171

```
No problem. 

Also, last time I checked, Arrow offers free international shipping.
```

---
## \#5 Posted by: rolloo Posted at: 2019-05-29T18:24:00.106Z Reads: 157

```

# VESC as SWD programmer: Flash BLE modules and fix bricked VESCs
https://www.youtube.com/watch?v=PFFiVxFHDM4&feature=youtu.be&t=324

not sure if it works with FSESC
```

---
## \#6 Posted by: Flasher Posted at: 2019-05-30T02:02:13.510Z Reads: 138

```
He makes good videos but I got completely lost from the start. It felt like talking to my 8 month son and trying to understand his answers
```

---
## \#7 Posted by: Flasher Posted at: 2019-05-30T02:04:34.194Z Reads: 133

```
I'm gonna receive this tomorrow
https://www.amazon.ca/dp/B072K3Z3TL/ref=cm_sw_r_cp_apa_i_lNZ7CbAX634N3
Now its gonna be to figure out how to do it without screwing up even more :slight_smile:
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-05-30T02:21:59.977Z Reads: 130

```
@Flasher
That's not an ST-Link...... you won't be able to reprogam the MCU with that.
(The boot pins on the MCU are not broken out, so you can't use the UART DFU).

Does Arrow not offer free shipping to Canada?

https://www.arrow.com/en/products/nucleo-f070rb/stmicroelectronics 

For example, the top part of the board is an ST-Link, it's about ~$11 and Arrow should have free shipping.
```

---
## \#9 Posted by: Flasher Posted at: 2019-05-30T02:45:56.223Z Reads: 123

```
They might but I'm not willing to wait several weeks to receive it ( customs always take time) and I'm in contact with flipsky to see if it's an easy fix or a send to them for a fix. Would this work instead?
![Screenshot_20190529-224514|281x500](upload://gImuLvIKg5rOmcsaAz0vurnpQNa.jpeg)
```

---
## \#10 Posted by: Flasher Posted at: 2019-05-30T03:12:04.388Z Reads: 110

```
I bought the one from arrow. Would you be able once I get it to help me out on how to use it? It seems to be a pretty extreme piece that could allow me to make more damage than actually help
```

---
## \#11 Posted by: rolloo Posted at: 2019-05-30T03:50:13.536Z Reads: 109

```
![VESC_SWD|690x396](upload://ZQEsqNssWnuqV4Hp7Kxf8LRhD1.jpeg)
```

---
## \#12 Posted by: Blasto Posted at: 2019-05-30T04:11:24.939Z Reads: 107

```
If it doesn’t work out with your st-link, you can swing by for help (i’m in mtl)
```

---
## \#13 Posted by: Gamer43 Posted at: 2019-05-30T04:21:42.201Z Reads: 108

```
I'd be more than happy to help. The second item from amazon you posted should work as well.

You will need some male to female jumper wires.

There's only a small part at the top of the nucleo board that is needed.
```

---
## \#14 Posted by: Flasher Posted at: 2019-05-30T04:27:53.421Z Reads: 102

```
I wasn't able to cancel my first order as it's already on the way to my house so I might as well see if it can serve me in any way and then I'll send it back. Arrow estimates I'll receive theirs on the 3rd of June. Doubt it but possible. @Blasto you're prob on the FB mtl eskate page :slight_smile: look me up ti-marc
```

---
## \#15 Posted by: Flasher Posted at: 2019-06-01T00:03:06.141Z Reads: 95

```
Hey I just got back from the post office. I am at a total loss with this thing...where do I plug and to what pin do I plug them in the esc![IMG_20190531_200020523|375x500](upload://o0cy8k9D9yAWVbQ4L7IbnwFvzaR.jpeg) ![IMG_20190531_200027352|666x500](upload://6aVmTtKUpX1Ykl8acN4q79QTg4j.jpeg) ?
```

---
## \#16 Posted by: Flasher Posted at: 2019-06-01T05:42:30.300Z Reads: 87

```
Managed to get it to work but now my problem has changed. I can't update the firmware on ack/vesc tool no matter what I do.it is stuck on 3.102. I tried updating to 3.103 on ack and to 3.57 on vesc and neither stayed even if it said success. Also my slave now has a blinking red light alongside the green one when booting up.
```

---
## \#17 Posted by: Pimousse Posted at: 2019-06-01T14:12:17.555Z Reads: 80

```
Perform a full chip erase.
Then flash the firmware you want.
Connect to VESC Tool et flash the bootloader through it.

Then try to upload a new FW through VESC Tool.
```

---
## \#18 Posted by: Gamer43 Posted at: 2019-06-01T19:03:12.113Z Reads: 75

```
Did you program them with ST-link utility?

You need to program a vesc6 bootloader at flash address 0x80E0000.

If you need, I can upload a short video of me doing this for one of my FSESC 6.6.
```

---
## \#19 Posted by: Flasher Posted at: 2019-06-01T19:27:34.810Z Reads: 72

```
That would be great :slight_smile:

I'm moving forward with the physical part of the build in the meanwhile![15594171560367442095420154358223|374x500](upload://QjpiQI2wcfC99ZfXJBdEAkLvyX.jpeg) ![15594171848301040376096583839583|374x500](upload://48hokdpngWn8BbAKWHC0DNIT3ek.jpeg) ![15594172066748941821636531436316|375x500](upload://ksJfK6w1xW2UIj5eAtYTx3fbTNK.jpeg)
```

---
## \#20 Posted by: Gamer43 Posted at: 2019-06-01T20:41:24.482Z Reads: 66

```
@Flasher 

https://www.youtube.com/watch?v=LFgxvkzk9JU

https://www.youtube.com/watch?v=0Wjb3rxZnts

make sure BOTH devices have power and the nucleoboard is plugged into the computer before connecting ANYTHING.

make sure that the bootloader is programmed at flash address 0x080E0000 or you WILL corrupt the firmware. 

Please let me know if you have any questions.
```

---
## \#21 Posted by: Flasher Posted at: 2019-06-01T21:08:45.397Z Reads: 63

```
i did exactly as i saw on your vid and ended up at ''firmware on connected esc is too old please update using a programmer''
```

---
## \#22 Posted by: Flasher Posted at: 2019-06-01T21:10:15.072Z Reads: 62

```
and on vesc tool i get invalid serial com 10
```

---
## \#23 Posted by: Gamer43 Posted at: 2019-06-01T21:16:55.163Z Reads: 63

```
might need to reflash the firmware as well then. Follow the exact same steps except instead of the bootloader file (which was 60_o_75.bin), select the desired firmware. You can find and download the firmware binaries here: https://github.com/vedderb/bldc/tree/master/build_all/60

Select default or default_no_hw_limits. 
**ALSO, program this at flash start address 0x08000000 (this is set by default in st-link utility when programming new firmware images, so you should not have to change the value when programming the firmware after selecting it)**
```

---
## \#24 Posted by: Flasher Posted at: 2019-06-01T21:30:24.114Z Reads: 63

```
and i am no longer able to connect to it at all. it tells me it cant find the target
```

---
## \#25 Posted by: Gamer43 Posted at: 2019-06-01T21:31:57.110Z Reads: 64

```
does the ESC still have both blue lights on? also check all the connections and restart ST-link utility.
```

---
## \#26 Posted by: Flasher Posted at: 2019-06-01T21:33:47.169Z Reads: 66

```
did all that
and still no :( also now i can no longer connect to my slave it also tells me for some reason that the firmware is too old
```

---
## \#27 Posted by: Gamer43 Posted at: 2019-06-01T21:35:46.019Z Reads: 65

```
The ESC still has both blue lights on, correct? Could you send me a picture of the connections?
```

---
## \#28 Posted by: Flasher Posted at: 2019-06-01T21:37:16.728Z Reads: 66

```
![IMG_20190601_173534556|374x500](upload://89toNEeCjVUBAeIJrWnVzuzuSsQ.jpeg) ![IMG_20190601_172050693|375x500](upload://bQ4iygCWa7f3yPzFvPNoPcF1wyF.jpeg) ![IMG_20190601_173547129|375x500](upload://qOwL71UgUqm7UYWpCgSTu4Zbt5K.jpeg) ![IMG_20190601_173603222|375x500](upload://x87RBRgM3XGF0fmlqaiX0RHWIM8.jpeg)
```

---
## \#29 Posted by: Gamer43 Posted at: 2019-06-01T21:41:40.874Z Reads: 61

```
Everything looks correct... maybe try unplugging the SWD connections, power cycling everything, then connecting the two back together, also restart st-link utility. 

If that doesn't work, then try connecting the NRST wire as well and see if it can connect under reset.

Also, I would highly recommend not doing this on top of batteries or other pieces of metal that can conduct.....
```

---
## \#30 Posted by: Flasher Posted at: 2019-06-01T21:44:34.522Z Reads: 59

```
ill try that last part as i already unplugged everything and restarted from scratch. even chnged the wires
```

---
## \#31 Posted by: Flasher Posted at: 2019-06-01T22:08:32.258Z Reads: 60

```
can we speak on cam (fb messenger)? im back to the problem of old firmware
```

---
## \#32 Posted by: Rc_44 Posted at: 2019-06-19T20:14:01.782Z Reads: 60

```
I'm also having this issue, but with a original Vesc 6 from Trampa. I'm making a build with two vesc 6's that was working okay until I went to update the firmware. One worked flawlessly but the other one got its power disconnected in the process. Now I'm with one Vesc functional and the other one only with the blue light on, and I can't connect to it with the usb port, which means it's probably bricked.

I bought an ST Link V2 to connect to it, but it kept giving an "could not connect to target" error even after checking the wiring many times (Gnd - Gnd, Swclk - Clk, Swdio - Io). I tried connecting the St link to the working Vesc as well but I had the same problems, so It's not an issue with the Vesc itself. 

I also tried connecting one Vesc to the other and using "SWD Prog" through the vesc tool but it also gave target errors.

I'm pretty much out of hope, but I really don't want to buy another Vesc. What am I doing wrong? Do I need to buy a Nucleo board?
```

---
## \#33 Posted by: Flasher Posted at: 2019-06-23T03:08:26.850Z Reads: 53

```
I just went straight for a nucleo board as it was recommended by @Gamer43  it revived it like it was simply a bad cold :slight_smile:
```

---
## \#34 Posted by: mattracer Posted at: 2019-08-05T06:38:04.749Z Reads: 45

```
Really Hope you find a fix! Think I have simular problems!
```

---
## \#35 Posted by: Rc_44 Posted at: 2019-08-12T00:31:24.807Z Reads: 37

```
Hi, sorry for the delay. As soon as the Nucleo Board arrived, I hooked it up with the rst pin, went into the ST Utility software and selected "Connect under reset". After that, I finally was able to upload the bootloader and the FW. Still working to this day! Thanks for the help!
```

---
## \#36 Posted by: Flasher Posted at: 2019-08-12T01:45:22.880Z Reads: 37

```
Glad I could help somewhat. Ride on
```

---
## \#37 Posted by: PartyPoison Posted at: 2019-10-12T19:16:14.384Z Reads: 25

```
i have read the thread, got the nucleo, followed the instructions/video.
run into problem!

if i dont take off the 2 black pins (st link) i can connect,
but on flashing the file, it can not read the memory.

once i take it off! it can not connect to target
```

---
## \#38 Posted by: Flasher Posted at: 2019-10-12T21:32:42.927Z Reads: 23

```
Which black pins do you mean? The 2 bridges at the top of the nucleo?
If so, it's your computer that isn't recognizing the nucleo properly. Those bridges allow you to use the internal chip on the nucleo's bottom half to test and experiment. When you remove them, it cuts the circuit and searches for the external chip you connected, in this case your esc
```

---
## \#39 Posted by: Flasher Posted at: 2019-10-12T21:34:33.778Z Reads: 22

```
Come join us on forum(dot)esk8(dot)news
I have been shadowbanned here and it's a pain just to respond to you :confused:
```

---
## \#40 Posted by: PartyPoison Posted at: 2019-10-12T21:36:07.289Z Reads: 22

```
yeah! those two bridges, so its my pc have the problem... thanks man!... im a member there to!
```

---
## \#41 Posted by: Flasher Posted at: 2019-10-12T21:37:30.338Z Reads: 22

```
What esc are we talking about here?
```

---
## \#42 Posted by: PartyPoison Posted at: 2019-10-12T21:38:01.367Z Reads: 22

```
flipsky 6 like in your vid
```

---
## \#43 Posted by: Flasher Posted at: 2019-10-12T21:39:29.026Z Reads: 22

```
Have you possibly tried another computer?
I know the process is a bitch but it would rule out user error and PC bitchery
```

---
## \#44 Posted by: PartyPoison Posted at: 2019-10-12T21:42:35.838Z Reads: 22

```
not yet... it didnt come to my mind that a pc/laptop would be a problem
```

---
