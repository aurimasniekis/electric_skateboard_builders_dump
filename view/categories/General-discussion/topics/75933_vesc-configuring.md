# Vesc configuring

### Replies: 29 Views: 501

## \#1 Posted by: y.k Posted at: 2018-11-25T07:18:55.791Z Reads: 161

```
i have a 8s2p 2600ma 5C li ion battery pack.i want to configure my vesk.
 what i fill in the Max amper and min amper blanket?
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-11-25T07:23:17.421Z Reads: 162

```
Start with 40 and -30 for battery amps and go from there 60, -50 for the motor amps.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-11-25T08:06:58.336Z Reads: 156

```
Am I calculating wrong, or his battery can only output 26a max?
```

---
## \#4 Posted by: y.k Posted at: 2018-11-26T08:18:28.220Z Reads: 138

```
 is 40 amp true for battery amx?wouldnot it damage the battery pack?
```

---
## \#5 Posted by: pat.speed Posted at: 2018-11-26T08:24:38.079Z Reads: 135

```
Yes it will, set it to 20a, -5 max for battery and about 45-60a, -50 for the motor. Start with that and see how it goes, I wouldn't increase battery max though as it will be too much for the battery
```

---
## \#6 Posted by: y.k Posted at: 2018-11-26T08:28:31.607Z Reads: 122

```
thanks bro . i will set the max at 20amp . how about -10 for the min amp?
```

---
## \#7 Posted by: y.k Posted at: 2018-11-26T08:31:31.653Z Reads: 120

```
and the batteries are LGABB41
```

---
## \#8 Posted by: pat.speed Posted at: 2018-11-26T09:17:28.357Z Reads: 121

```
In a 8s2p configuration it will be 5200mah according to the spec sheet, but only rated for 2c. Meaning your batt max would actually be more like 10a. 

Based on those values I would suggest a different battery, it might work if you limit the cells to 10a with the vesc but it won't last very long or have very much range. Your best bet is to either buy some lipos from hobbyking while they have a cyber Monday sale on or purchase a prebuilt 18650 battery from a builder here or from a prebuilt company like wowgo for example.
```

---
## \#9 Posted by: y.k Posted at: 2018-11-26T12:28:19.141Z Reads: 109

```
as you said max amp 20  and and min-5. i want to set this. is it ok from your view?
```

---
## \#10 Posted by: pat.speed Posted at: 2018-11-26T21:13:08.334Z Reads: 91

```
I don’t think it can handle 20a, I would start with 10a and see how much it sags and how hot it becomes
```

---
## \#11 Posted by: y.k Posted at: 2018-11-29T08:18:44.041Z Reads: 71

```
my battery builder told me to set it on 18. i dont know what would happen. but didnot tell about min amper. bro,is -5 good?
```

---
## \#12 Posted by: pat.speed Posted at: 2018-11-29T20:30:10.126Z Reads: 59

```
Yeah -5 is good
```

---
## \#13 Posted by: y.k Posted at: 2018-11-30T21:57:33.461Z Reads: 54

```
god bless my battery. i set it at 18 and -5 to see the result. thanks bro
```

---
## \#14 Posted by: y.k Posted at: 2018-12-08T19:06:12.417Z Reads: 55

```
hi.sorry again. i plugged in every thing and clicked on the connect part on BLDCtools program  but it says Not connected. what sould i do bro?
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-12-08T19:44:56.919Z Reads: 55

```
Make sure you are using right cable which is able to transfer data over USB.
Try plugging an android device to check the transmission of the cable
```

---
## \#16 Posted by: pat.speed Posted at: 2018-12-08T22:35:19.735Z Reads: 50

```
Yep, some cables don’t have data cables and can only charger
```

---
## \#17 Posted by: y.k Posted at: 2018-12-10T09:31:18.044Z Reads: 42

```
the cable is its fabic from Maytech company.![1544434311533-87151941|281x500](upload://mHmnW2Bb0yHarqYKa0FISSGSo5g.jpeg)
```

---
## \#18 Posted by: y.k Posted at: 2018-12-10T09:33:49.708Z Reads: 38

```
it says windows  does not recognize it? my windos is 7. sould i change my windos?
```

---
## \#19 Posted by: y.k Posted at: 2018-12-10T09:38:57.073Z Reads: 37

```
![1544434723883-2106600857|690x388](upload://hMYU6JBCPebH7zYm4lYN8unC8cN.jpeg)
```

---
## \#20 Posted by: Goonman Posted at: 2018-12-10T09:48:55.888Z Reads: 39

```
Pretty normal. You had it connected earlier? 
Unplug and plug it back in, try a different USB port, press reconnect on VESC tool make sure vesc is powered up. Wiggle connections. Use auto connect
Repeat
```

---
## \#21 Posted by: CarlCollins Posted at: 2018-12-10T09:55:18.214Z Reads: 40

```
Do this
Download and Extract: https://drive.google.com/file/d/1ei5p-xRrJsaJiyP6jYGHhD0cMyFX8eqF/view?usp=sharing
2: Right click on the unknown Device and select properties 
3: Select driver tab 
4: Click update driver
5: Choose the directory where you extracted the above file 
6: Let the Window install the driver
7: restart your PC and VESC
8: Then check if STElectronics COM port appears under Posts (COM & LPT)
```

---
## \#22 Posted by: y.k Posted at: 2018-12-10T10:11:02.797Z Reads: 36

```
i clicked on the adress and this has come up![1544436672328-87151941|690x388](upload://9w1Ff56PxItlwlBRZ63efwdoFME.jpeg)
```

---
## \#23 Posted by: CarlCollins Posted at: 2018-12-10T11:10:44.225Z Reads: 34

```
Click the down arrow on the upper right corner of the screen to download these files and then follow the instructions
```

---
## \#24 Posted by: y.k Posted at: 2018-12-11T09:56:12.625Z Reads: 30

```
i downloaded it but i think it is ziped and it cant be open![1544522213868438399716|690x388](upload://35ibz4L9M7S1f5hbEE67pjFt7Zj.jpeg)
```

---
## \#25 Posted by: CarlCollins Posted at: 2018-12-11T20:54:16.884Z Reads: 27

```
You have to unzip to a desktop or something first
(Use Extract Command)
```

---
## \#26 Posted by: y.k Posted at: 2018-12-12T08:36:27.102Z Reads: 20

```
i will do it
```

---
## \#27 Posted by: y.k Posted at: 2018-12-12T09:24:58.729Z Reads: 21

```
i unziped them but still not connected. the error is code29 of usb. i dont know what is code29. doesnot need any serial number of vesc/?
```

---
## \#28 Posted by: CarlCollins Posted at: 2018-12-12T19:30:08.255Z Reads: 16

```
Download and install team viewer and let me know your ID and Password,
I will solve it for you
```

---
## \#29 Posted by: y.k Posted at: 2018-12-13T10:25:28.313Z Reads: 11

```
i installed it.i will tell you the exact time of connecting to team viewer bro.
```

---
