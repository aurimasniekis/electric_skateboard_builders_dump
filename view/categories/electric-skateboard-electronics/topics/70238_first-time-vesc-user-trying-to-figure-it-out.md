# First time VESC user, trying to figure it out

### Replies: 7 Views: 281

## \#1 Posted by: danile Posted at: 2018-10-05T14:50:51.413Z Reads: 60

```
Hey guys

I've got a VESC as a gift (older version) and trying to figure it out, so far no success. 
Hope for some insight from you:

Here are the symptoms:
It is connected to battery, motor and is detected with VESC tool.
Then it says my firmware needs update.
Doing the update, all seem normal, except the red line that appears through the end (see pic).
Next time I connect it the story repeats itself, prompts for firmware update and all repeats itself.

Any ideas how to tackle this?
![vesc|250x500](upload://p0YlLJiVJyEwCODvbLAYoQHaHx9.jpeg) 
![vesc%20error|689x293](upload://zaglDRgCwGtSzlvhvyD33F8aZGQ.png) 

Thanks, 
Dani
```

---
## \#2 Posted by: Bart_Dood Posted at: 2018-10-05T16:42:59.400Z Reads: 46

```
Did you check your hardware version is the correct match for the firmware you are trying to flash? there should be a number on the board somewhere.

Once you make sure you're flashing the right firmware, do a full power off and reboot of the VESC.
```

---
## \#3 Posted by: danile Posted at: 2018-10-08T02:46:55.346Z Reads: 37

```
Mine says vesc 4.7 on the board.
Tried several options with the vesc tool, still same result.

Thank you,
Dani
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-08T04:48:36.611Z Reads: 30

```
If it’s hw 4.7 I think you need to flash this file
![image|374x500](upload://gKsTvbk31DnMsjh5jfSUNyuf71w.jpeg) 
If you did flash an other fw than your vesc now probably blocked and you need a st v2 link to upload the hexfile and firmware to make it work again
https://www.amazon.com/Aideepen-ST-Link-Programming-Emulator-Downloader/dp/B01J7N3RE6/ref=mp_s_a_1_5?ie=UTF8&qid=1538920320&sr=8-5&pi=AC_SX236_SY340_QL65&keywords=st+v2+link&dpPl=1&dpID=41u9nyzYQoL&ref=plSrch
```

---
## \#5 Posted by: danile Posted at: 2018-10-08T13:13:37.626Z Reads: 20

```
Andy, thank you. I will try this.

Can you point me to the instructions as to what to do once I have this programmer at hand?

Thanks,
Dani
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-08T13:17:33.449Z Reads: 18

```
I never made it by my own, but look through this threat
https://www.electric-skateboard.builders/t/help-with-focbox-firmware-bootloader-upgrade-vesc-tool/34810/44?u=andy87
@Eboosted wrote down everything there step by step
```

---
## \#7 Posted by: danile Posted at: 2018-10-08T13:21:31.086Z Reads: 16

```
Cool, will try it this week
Thanks again!
```

---
