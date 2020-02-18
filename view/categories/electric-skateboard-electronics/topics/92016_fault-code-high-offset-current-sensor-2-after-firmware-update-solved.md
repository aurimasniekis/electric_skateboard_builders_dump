# Fault Code: HIGH_OFFSET_CURRENT_SENSOR_2 after firmware update - SOLVED

### Replies: 29 Views: 762

## \#1 Posted by: bluegreen Posted at: 2019-04-28T02:09:41.580Z Reads: 117

```
So, maybe not too surprising but I tried these cheap VESC on ebay, which are nearly half price:
https://www.ebay.com/itm/HGLRC-Flipsky-50A-Electronic-Speed-Controller-ESC-For-Electric-Skateboard/401692035273?ssPageName=STRK%3AMEBIDX%3AIT&amp;_trksid=p2060353.m2749.l2649

And after flashing the firmware successfully the red light is flashing, the terminal fault reports:

FAULT_CODE_HIGH_OFFSET_CURRENT_SENSOR_2

My guess it is something that is out of spec on the hardware that maybe old firmwares were ok with? That is why they are on sale?

Anyways, if someone who is experienced with VESC can let me know any more test to run, or some options I might have. I tried this on both VESC I order and they both have the same problem after firmware update.

If there are on-board voltages to test or components I might be able to replace to bring it back into spec, that would be helpful. If anyone can point me in the right direction of the part of the circuit this error would involve.

You get what you pay for!
```

---
## \#2 Posted by: bluegreen Posted at: 2019-04-28T02:20:44.941Z Reads: 107

```
It appears this detection was added in version 3.55 so, yeah I guess it is a new feature!
```

---
## \#3 Posted by: bluegreen Posted at: 2019-04-28T02:36:31.756Z Reads: 103

```
Hella noob

Running motor detection clears the faults I will go into hiding now.

![ostrich%20hiding%20its%20head%20under%20sand%20to%20protect%20it%20from%20strong%20wind|468x339](upload://4vloDRj16IbZL9IMq2XQhrpKc3u.jpeg)
```

---
## \#4 Posted by: jun1208 Posted at: 2019-04-29T13:17:39.339Z Reads: 90

```
Hey bro, 

I get the same error running on BLDC mode in 3.55 using my dual 4.2 from Flipsky...

It triggers the same error every time I reboot the board so I will have to run detection all over again every time I turn on the board :frowning_face:
```

---
## \#5 Posted by: xsynatic Posted at: 2019-04-29T13:28:51.306Z Reads: 82

```
Same on 3.55 and HW 410 from Torqueboard.

Just updated from 3.54 to 3.55 not both my vescs blink and the Motor detection fails.

Can't even fnish the Motor setup.
```

---
## \#6 Posted by: jun1208 Posted at: 2019-04-29T13:37:18.980Z Reads: 78

```
Dang it...are you able to save it by downgrading the vesc fw? 
Or is it not possible?
```

---
## \#7 Posted by: xsynatic Posted at: 2019-04-29T13:37:46.550Z Reads: 76

```
I'm currently trying to research it.
```

---
## \#9 Posted by: xsynatic Posted at: 2019-04-29T14:10:00.232Z Reads: 71

```
it is possible, but for impossible to find the older Firmware.

EDIT : 
Update? I fixed it by using the VESC tool 1.08 which only supports up to 3.54.

Connected and flashed it. No the blinking is gone. Lets see if i'm able to program the VESC so i finally can drive.
```

---
## \#10 Posted by: jun1208 Posted at: 2019-04-29T15:08:49.792Z Reads: 67

```
Hope it's ok after downgrading the fw, mine runs only in foc mode...I'm keeping it in foc mode for now cos I don't wanna mess it up further...
```

---
## \#11 Posted by: xsynatic Posted at: 2019-04-29T15:23:44.501Z Reads: 64

```
Yep, so far so good. I was able to do the setup and it works. I'll keep it at 3.54 until a fix is present
```

---
## \#12 Posted by: bluegreen Posted at: 2019-04-29T16:39:42.110Z Reads: 59

```
Luckily my problem went away after motor detection and stayed away even through powerup with the recent software.
```

---
## \#13 Posted by: jun1208 Posted at: 2019-04-29T22:32:47.182Z Reads: 53

```
Great to hear that mate :slight_smile:
```

---
## \#14 Posted by: jun1208 Posted at: 2019-04-29T22:32:58.656Z Reads: 51

```
Were you in FOC or BLDC mode yea?
```

---
## \#15 Posted by: bluegreen Posted at: 2019-04-29T22:38:51.858Z Reads: 49

```
FOC, just using the wizard FOC is the default configuration.
```

---
## \#16 Posted by: jun1208 Posted at: 2019-04-29T22:44:13.268Z Reads: 49

```
Alrighty, then I am in the same situation, it works fine in FOC but not BLDC :sweat_smile:
```

---
## \#17 Posted by: bluegreen Posted at: 2019-04-29T23:28:04.659Z Reads: 50

```
Oh weird, I didn't try BLDC. That is weird cuz FOC should be more difficult to do than BLDC.

And theoretically still works because I ran the motors up to speed that should be above FOC.

My guess is they have a different value resistor somewhere on the sense circuit and the value is just slightly off what it is expecting, but hasn't been an issue up until this update.
```

---
## \#18 Posted by: jun1208 Posted at: 2019-04-30T02:55:59.943Z Reads: 48

```
Probably...
Because I wasn't having any issues running BLDC on a few updates earlier too.. until the recent FW 3.55 version :-1:
```

---
## \#19 Posted by: Fatglottis Posted at: 2019-04-30T22:25:24.378Z Reads: 43

```
Thanks a lot man!
I just repaired a FOCBOX with a broken MOSFET and DRV. Flashed 3.55 and got stuck with this fault code. Never seen it before and had no idea how to fault trace.
reverted to an older sw and now wheels are spinning. :sunglasses:
```

---
## \#20 Posted by: xsynatic Posted at: 2019-04-30T23:06:46.724Z Reads: 41

```
Glad to hear that!
```

---
## \#21 Posted by: AbrownMN Posted at: 2019-05-03T18:20:10.324Z Reads: 38

```
Where did you get the 1.08 from? My buddy is setting up a brand new board and is having the same issue.
```

---
## \#22 Posted by: xsynatic Posted at: 2019-05-03T18:34:40.441Z Reads: 35

```
I still had it on my PC. I have 1.04,1.08 and 1.09.

Do you need 1.08? I can send you the file.
```

---
## \#23 Posted by: AbrownMN Posted at: 2019-05-03T18:35:52.849Z Reads: 34

```
That would be awesome! I am planning to run over there today to help him out. He seems to be having a motor detection issue, and has blinking red and blue light as described. Hoping this fixes it. 

Should I PM you my email, or do you have a host you can link from?
```

---
## \#24 Posted by: xsynatic Posted at: 2019-05-03T18:36:50.190Z Reads: 33

```
Sound like the problem i had. Just reflash the 3.54 FW with the tool and he should be set.
I was stuck on the Motor detection too.

I'll send you a PM with a host link.
```

---
## \#25 Posted by: AbrownMN Posted at: 2019-05-03T18:38:03.364Z Reads: 33

```
Thanks brotha!

I'll update this post if that solves it for others visibility.
```

---
## \#26 Posted by: xsynatic Posted at: 2019-05-03T18:44:38.919Z Reads: 33

```
PM sent.

10char
```

---
## \#27 Posted by: AbrownMN Posted at: 2019-05-03T18:58:36.446Z Reads: 32

```
That did it boys!

Thanks for the link friend. You saved my boy his sanity today.

Edit: As another note, this seems to have something to do with how you run the wizard and which button you click which is why it seems intermittent and only happening to some folks.

If you look at the GitHub Issues page a guy there describes being able to restart from scratch and get the new software/firmware to work by clicking on a different wizard button...something to consider.
```

---
## \#28 Posted by: jun1208 Posted at: 2019-05-04T11:53:35.230Z Reads: 34

```
There's an update to the vesc tool to version 1.10 with fw 3.56 that was pushed recently, changelog seems to say that they fixed the issue :+1:

 ![Screenshot_20190504-195259|250x500](upload://4VtSrENHDcrfJYnUSVza0PyG8El.jpeg)
```

---
## \#29 Posted by: AbrownMN Posted at: 2019-05-04T16:19:03.121Z Reads: 34

```
This is true. By the time I got over to his house to help out they had changed the version. It did fire up fine on 1.08 as well however.

Also, In case anyone else is having trouble with dual setups.... They need to release a new tutorial. They changed the Multiple VESC setup and the prompts no longer pop up and guide you in the same way. You have to manually write the proper ID and settings to make it recognize Master/Slave and run the motors together properly.  Took me quite some time of fiddling around with it ( being my first time with the new tool) to figure this out.

If anyone sees this and has trouble feel free to pm or reply and I can try to help out.
```

---
## \#30 Posted by: jun1208 Posted at: 2019-05-04T22:30:50.925Z Reads: 31

```
Thanks for the heads up mate! 
I'm gonna flash the new firmware later today, have a group ride this morning so don't wanna take the risk to mess up the board :smile:
```

---
