# Firefly Esk8 Remotes Integrated PCB

### Replies: 25 Views: 1395

## \#1 Posted by: solodros Posted at: 2018-06-03T17:37:23.315Z Reads: 341

```
Thanks to Solidgeek's Firefly Remotes, which makes electric skateboards even more fun. I have a little knowledge of the electronics profession, so I designed the integrated PCB based on the schematics published by solidgeek, avoiding the cumbersome assembly of modules. It is still in the testing phase. mcu is atmega328p. The remote controller PCB is ready to use but it is not convenient enough. For example, the download of firmware cannot use USB directly, but only use another circuit board to download the firmware. When my design is complete, I will open source the schematic and PCB.
     But I have a question, solidgeek released a new remote controller schematic on his personal website, the MCU changed to atmega32u4, but the firmware of the remote controller has not changed. Can anyone tell me if he has released new firmware? This is the link https://solidgeek.dk/firefly-remote-pcb/
    If the new remote control schematic can be used, I will give up the current PCB and redesign the PCB of the new remote control schematic.
    In addition, I am now in China, so the components I use are all readily available in China. I only have time to design the PCB at night, all the speed will be very slow, please be patient
   My English is not good. This is using Google Translate. I'm very sorry.
PCB layout may not be reasonable, please make suggestions

![222|519x499](upload://uFqHmZbr9R93ugkEs2VN5lARmOx.jpg)
![555|690x489](upload://w5gtpJMf4jxZOdmKTnz0cdugw3m.jpg)![333|446x500]
(upload://uaL0QCc2teADXxBsw3Se1obLrME.jpg)
![QQ图片20180508183637|690x388](upload://jaKXTGTDLKRiGFx8u2NpRs9giYl.jpg)
```

---
## \#2 Posted by: solodros Posted at: 2018-06-08T12:54:12.964Z Reads: 289

```
If you want to make low-cost VESC4.12, I share the low-cost ESC based on vesc4, please see the link: https://github.com/Z-WX/VESC-4-derivative-
```

---
## \#3 Posted by: moon Posted at: 2018-06-08T12:59:18.702Z Reads: 286

```
People aren't looking for low cost,they are looking for high quality...
```

---
## \#4 Posted by: solodros Posted at: 2018-06-08T13:18:37.682Z Reads: 281

```
More choice
```

---
## \#5 Posted by: solodros Posted at: 2018-06-26T14:07:58.550Z Reads: 268

```
The PCB design is completed and is being sent to the factory for processing. I plan to redesign the remote to fit my PCB shape![Snipaste_2018-06-26_22-06-08|402x500](upload://7i1jwhWpa0f0lD9em2WEvRpE67R.jpg)![Snipaste_2018-06-26_22-05-53|349x462](upload://nPrBMVDu5NOxn8GJZqX5fWm5J7r.jpg)![Snipaste_2018-06-26_22-07-39|312x500](upload://mRm3Iap7yu7USMSBbc5OTQfzaPn.jpg)
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-08-19T13:42:58.980Z Reads: 212

```
Any updates ?
```

---
## \#7 Posted by: hoeksame1 Posted at: 2018-08-19T14:12:50.392Z Reads: 213

```
Going to sell the pcb???
```

---
## \#8 Posted by: solodros Posted at: 2018-08-19T14:42:17.751Z Reads: 213

```
Sorry, my friend gave me a shell similar to the boosted remote control. I designed a new remote control PCB for him and sent it to the factory.
![1|409x500](upload://8ZsuSVmhfizoqRrOxjBcPblozKw.jpg)
![QQ%E5%9B%BE%E7%89%8720180819224040|690x267](upload://fuhWrMR06gDHS2flU1QsrKIp8EZ.jpg)
```

---
## \#9 Posted by: Jc06505n Posted at: 2018-08-19T14:44:36.698Z Reads: 205

```
Nice , is this telemetry based like the firefly or a no-none sense remote ? It would be really nice to just have a reliable remote that’s not affected by interference and have a programmable multi-button and LED’s like Boosted’s
```

---
## \#10 Posted by: solodros Posted at: 2018-08-19T14:48:34.236Z Reads: 208

```
based on the firefly。
I use different 2.4G modules and they are very stable.
The LED is not used, I think there is enough OLED display information, and I try to add a button to switch acceleration and a switch to control the light.
```

---
## \#11 Posted by: hoeksame1 Posted at: 2018-08-19T14:51:42.752Z Reads: 203

```
Okay if you know the price i will buy one!
```

---
## \#12 Posted by: solodros Posted at: 2018-08-19T14:54:22.994Z Reads: 201

```
I don't plan to sell it for now, I need enough test time.
```

---
## \#13 Posted by: Jc06505n Posted at: 2018-08-19T14:55:02.125Z Reads: 201

```
[quote="solodros, post:10, topic:57686"]
and I try to add a button to switch acceleration and a switch to control the light.
[/quote]

Nice ! I’m still a strong advocate for a single momentary programmable button
```

---
## \#14 Posted by: solodros Posted at: 2018-08-19T14:56:40.741Z Reads: 197

```
Agree with your point of view
```

---
## \#15 Posted by: solodros Posted at: 2018-08-21T15:47:42.962Z Reads: 193

```
![QQ%E6%88%AA%E5%9B%BE20180821234711|304x500](upload://thlRxkjPpDl2iBVy2Gvjf9uXFVd.jpg)
```

---
## \#16 Posted by: Jc06505n Posted at: 2018-08-21T16:02:28.916Z Reads: 187

```
Nice this is that the backfire/winboard remote casing from Tao? What are you planning to do with the OLED? 

Are you planning on selling/groupbuying a complete ?
```

---
## \#17 Posted by: solodros Posted at: 2018-08-21T16:14:07.118Z Reads: 185

```
Yes, the casing is from Taobao
I will design a frame to protect and hold the OLED
There is no plan to sell it for the time being, unless I have tested it normally.
```

---
## \#18 Posted by: Battosaii Posted at: 2018-08-21T16:23:03.068Z Reads: 187

```
I've been using a Firefly for a few days now and there's a few things I'd like to change. Im not a huge fan of the long throw on the throttle.coming from a Nano x. The other thing is I wish it would stay one one fixed data I hate that it cycles from speed to battery life to distance I really don't need distance and with I could change it to MPH, maybe I can but I need to learn programming lol
```

---
## \#19 Posted by: solodros Posted at: 2018-08-21T16:25:27.741Z Reads: 178

```
HI, I made a change, switch data every 4 seconds → click the button to switch data
```

---
## \#20 Posted by: Battosaii Posted at: 2018-08-21T16:40:02.440Z Reads: 175

```
Oh nice. Is that just software? Can I upload your software on my remote?
```

---
## \#21 Posted by: solodros Posted at: 2018-08-22T12:15:36.235Z Reads: 145

```
I am busy these days, please wait a while, I will upload the firmware to github
```

---
## \#22 Posted by: solodros Posted at: 2018-08-22T13:14:36.177Z Reads: 154

```
https://github.com/Solodros/Key-switch-data
Please use, if there is any problem, please say
```

---
## \#23 Posted by: Battosaii Posted at: 2018-08-22T13:56:33.486Z Reads: 145

```
I'll try it tonight when I get home. Thank you!
```

---
## \#24 Posted by: walleywalker Posted at: 2018-09-08T15:10:51.570Z Reads: 125

```
Subscribed. This is great, can't wait for updates!
```

---
## \#25 Posted by: ElectricCoast Posted at: 2018-09-10T08:51:56.875Z Reads: 101

```
Interesting.
```

---
