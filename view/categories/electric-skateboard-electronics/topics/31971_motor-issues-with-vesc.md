# Motor issues with vesc

### Replies: 68 Views: 1621

## \#1 Posted by: dg798 Posted at: 2017-08-31T19:31:23.249Z Reads: 100

```
When I test my motor with my computer in bldc my motor does a weird thing as shown in the video.
```

---
## \#2 Posted by: dg798 Posted at: 2017-08-31T19:33:32.343Z Reads: 95

```
Can't post video but it barely moves and makes a weird noise with the bldc tool
```

---
## \#3 Posted by: darkkevind Posted at: 2017-08-31T19:52:22.449Z Reads: 93

```
Did you do a motor detection?
```

---
## \#4 Posted by: dg798 Posted at: 2017-08-31T19:55:57.421Z Reads: 88

```
yes and it doesnt work
```

---
## \#5 Posted by: dg798 Posted at: 2017-08-31T19:56:20.573Z Reads: 86

```
it fails 
thats the video [https://goo.gl/photos/ZaVqk2wKWr4AS8B39](https://goo.gl/photos/ZaVqk2wKWr4AS8B39)
```

---
## \#6 Posted by: darkkevind Posted at: 2017-08-31T19:56:44.197Z Reads: 78

```
You need to up the A setting from 6 to 8 and try again. Keep raising the A until the detection works...
```

---
## \#7 Posted by: dg798 Posted at: 2017-08-31T20:00:33.491Z Reads: 77

```
what do you mean by a
```

---
## \#8 Posted by: darkkevind Posted at: 2017-08-31T20:01:06.051Z Reads: 76

```
If it didn't work, up the Amp number from 6... then try test again.
```

---
## \#9 Posted by: dg798 Posted at: 2017-08-31T20:02:04.194Z Reads: 79

```
8 didnt work
```

---
## \#10 Posted by: darkkevind Posted at: 2017-08-31T20:02:31.362Z Reads: 79

```
<img src="/uploads/db1493/original/3X/d/8/d8e2a3fa25256d29d0cb6a0ec8ebf9601b5e7a95.png" width="388" height="500">

Keep going up
```

---
## \#11 Posted by: dg798 Posted at: 2017-08-31T20:03:17.154Z Reads: 73

```
what do you recommend
```

---
## \#12 Posted by: dg798 Posted at: 2017-08-31T20:04:36.977Z Reads: 72

```
its already at 10 and it doesnt work still
```

---
## \#13 Posted by: Martinsp Posted at: 2017-08-31T20:04:52.940Z Reads: 71

```
Please check if you have your App disabled ("no app")
```

---
## \#14 Posted by: dg798 Posted at: 2017-08-31T20:05:48.453Z Reads: 71

```
it says current no reverse with brake
```

---
## \#15 Posted by: Martinsp Posted at: 2017-08-31T20:06:32.631Z Reads: 72

```
It is in the General sub-tab of the app config
```

---
## \#16 Posted by: dg798 Posted at: 2017-08-31T20:06:54.555Z Reads: 72

```
its on ppm
```

---
## \#17 Posted by: Martinsp Posted at: 2017-08-31T20:07:27.968Z Reads: 70

```
Set it to no app. I am sure it is the cause for your problem.
```

---
## \#18 Posted by: dg798 Posted at: 2017-08-31T20:08:10.357Z Reads: 70

```
still doesnt work
```

---
## \#19 Posted by: Martinsp Posted at: 2017-08-31T20:08:36.744Z Reads: 72

```
Did you write the configuration and reboot?
```

---
## \#20 Posted by: dg798 Posted at: 2017-08-31T20:09:23.254Z Reads: 67

```
yes and it still doesnt work
```

---
## \#21 Posted by: Martinsp Posted at: 2017-08-31T20:09:40.089Z Reads: 65

```
What motor are you using?
```

---
## \#22 Posted by: cwazy1 Posted at: 2017-08-31T20:09:41.798Z Reads: 64

```
does it work with your controller?
```

---
## \#23 Posted by: dg798 Posted at: 2017-08-31T20:10:21.396Z Reads: 65

```
6355 190 kv torque boards and i currently have no remote, just using keyboard on computer
```

---
## \#24 Posted by: dg798 Posted at: 2017-08-31T20:11:46.083Z Reads: 65

```
is it becasue i put in the wring limits and amps for the motor
and if so im using a 12s battery. what should i be doing
```

---
## \#25 Posted by: Martinsp Posted at: 2017-08-31T20:12:11.390Z Reads: 64

```
Try flashing the firmware to make sure. read the default configuration and start from scratch. 

Your best bet would be to try to ask @torqueboards for the configuration file that you could upload. I am sure he has them for his motor. If you are lucky someone will send you their configuration file.
```

---
## \#26 Posted by: dg798 Posted at: 2017-08-31T20:12:43.307Z Reads: 58

```
which firmware should i use
```

---
## \#27 Posted by: dg798 Posted at: 2017-08-31T20:13:19.375Z Reads: 61

```
my vesc is 4.12 and fw is 2.18
```

---
## \#28 Posted by: dg798 Posted at: 2017-08-31T20:13:51.165Z Reads: 62

```
it only gives me options for the hardware. should i do 4.12
```

---
## \#29 Posted by: cwazy1 Posted at: 2017-08-31T20:14:04.486Z Reads: 63

```
can you post exactly what your setup looks like? take some screenshots of your bldc.
```

---
## \#30 Posted by: Martinsp Posted at: 2017-08-31T20:14:48.114Z Reads: 63

```
If you are looking at the folders then yes choose 4.12 and then VESC default .bin
Make sure you did not choose wrong file because it will fry your VESC
```

---
## \#31 Posted by: dg798 Posted at: 2017-08-31T20:15:50.621Z Reads: 61

```
ok now it just rebooted by itself
```

---
## \#32 Posted by: dg798 Posted at: 2017-08-31T20:18:21.723Z Reads: 61

```
and here are some screenshots:
https://goo.gl/photos/E6kYZhNghcWCw4Vj9
```

---
## \#33 Posted by: darkkevind Posted at: 2017-08-31T20:19:43.994Z Reads: 62

```
'No App' on App Configuration...?
```

---
## \#34 Posted by: dg798 Posted at: 2017-08-31T20:20:35.730Z Reads: 64

```
thats what @Martinsp told me to do
```

---
## \#35 Posted by: MontPierre Posted at: 2017-08-31T20:21:16.306Z Reads: 62

```
What batteries do you have connected in? Just one or all of them?
```

---
## \#36 Posted by: dg798 Posted at: 2017-08-31T20:21:44.832Z Reads: 61

```
2 6s in series
```

---
## \#37 Posted by: darkkevind Posted at: 2017-08-31T20:21:46.585Z Reads: 63

```
No he was saying to check that you don't have that setting like that. Should be PPM
```

---
## \#38 Posted by: Martinsp Posted at: 2017-08-31T20:21:50.740Z Reads: 60

```
Is it just my internet being retarded or was the first link not a video? If it is not please send us a video along with what exactly your detection settings are (the three values so current mi erpm and low duty) that you used for  that video
```

---
## \#39 Posted by: dg798 Posted at: 2017-08-31T20:22:52.108Z Reads: 61

```
ok give me 10 minutes
```

---
## \#40 Posted by: cwazy1 Posted at: 2017-08-31T20:22:55.419Z Reads: 62

```
uncheck the 'send status over can' 

that is meant only for if you're running a dual motor
```

---
## \#41 Posted by: MontPierre Posted at: 2017-08-31T20:23:40.160Z Reads: 60

```
On one of the pics you just uploaded you still have 6A in detection. Make sure it is at 10a and Write conf and then reboot vesc.
```

---
## \#42 Posted by: cwazy1 Posted at: 2017-08-31T20:24:34.060Z Reads: 60

```
this won't matter because he doesnt have a remote and is just trying to turn the motor using arrow keys.
```

---
## \#43 Posted by: Martinsp Posted at: 2017-08-31T20:24:42.451Z Reads: 62

```
Oh ok it was me, sorry. Try upping the low dutycycle to say 0.08 and run detection again with the "no app" that is correct

@MontPierre The 3 values you set at motor detection are not saved in the VESC they are just for the detection therefore you dont need to write nor reboot
```

---
## \#44 Posted by: cwazy1 Posted at: 2017-08-31T20:24:54.052Z Reads: 62

```
do you have sensor wires connected? or are you running sensorless?
```

---
## \#45 Posted by: dg798 Posted at: 2017-08-31T20:25:41.010Z Reads: 59

```
sensoreless config
```

---
## \#46 Posted by: cwazy1 Posted at: 2017-08-31T20:27:42.840Z Reads: 60

```
I see that in the config, but do you have the wires plugged in?
```

---
## \#47 Posted by: dg798 Posted at: 2017-08-31T20:28:28.788Z Reads: 59

```
which ones the 3 with the bullet connectors
```

---
## \#48 Posted by: cwazy1 Posted at: 2017-08-31T20:32:25.437Z Reads: 55

```
there should be 3 bullet connectors and then also another wire which is the sensor connector. Its a little white connector with 7 or 8 little wires connecting to it.
```

---
## \#49 Posted by: dg798 Posted at: 2017-08-31T20:33:03.114Z Reads: 54

```
no its not connected becasue im in sensoreless
```

---
## \#50 Posted by: dg798 Posted at: 2017-08-31T20:38:47.697Z Reads: 52

```
do i still need to connect that wire
```

---
## \#51 Posted by: Martinsp Posted at: 2017-08-31T20:48:18.438Z Reads: 52

```
Please program/set up your vesc based on this video tutorial. I believe Jacob is the guy that programmed the bldc tool so he knows what he is doing. 
https://youtu.be/5HLZaMcYRuY 

If you are still having problems, torque boards has a channel on YouTube and I believe he has one video of setting things up too so have a look at that.
```

---
## \#52 Posted by: dg798 Posted at: 2017-08-31T21:14:24.604Z Reads: 47

```
here is a full video of my problem:
and by the way im using 2 6s batteries in series.
https://goo.gl/photos/y6iAuCv5pQr5nbYT8
```

---
## \#53 Posted by: dg798 Posted at: 2017-08-31T21:37:49.309Z Reads: 44

```
can someone please help?
```

---
## \#54 Posted by: cwazy1 Posted at: 2017-08-31T22:20:43.144Z Reads: 44

```
uncheck any boxes that have to do with CAN 

change erpm limits to -60k and +60k and uncheck the negative torque when hitting max

Then swap some phase wires around and test again
```

---
## \#55 Posted by: dg798 Posted at: 2017-08-31T22:32:04.124Z Reads: 44

```
motor detection still fails
```

---
## \#56 Posted by: cwazy1 Posted at: 2017-08-31T22:35:33.091Z Reads: 45

```
have you tried to do it in sensored mode?
```

---
## \#57 Posted by: dg798 Posted at: 2017-08-31T22:36:53.660Z Reads: 45

```
no but do i need a special cable for that
```

---
## \#58 Posted by: dg798 Posted at: 2017-08-31T23:42:10.834Z Reads: 42

```
if that works i would buy a cable and if i dont need a special cable then what should i do
```

---
## \#59 Posted by: dg798 Posted at: 2017-09-01T16:26:51.979Z Reads: 38

```
now im getting a drv8302 error.
i heard that means that i fried something but does it have to do with anything about the motor?
```

---
## \#60 Posted by: Pedrodemio Posted at: 2017-09-01T16:36:12.779Z Reads: 36

```
Did you check the voltage limits on the main screen? Maybe your battery is above or below them
```

---
## \#61 Posted by: dg798 Posted at: 2017-09-01T16:37:38.873Z Reads: 32

```
i have a 12s battery and my cutoff start is 40 and cutoff end is 39
```

---
## \#62 Posted by: dg798 Posted at: 2017-09-01T16:39:04.973Z Reads: 32

```
and it says my vesc is at 29 degrees celsius. is that normal
```

---
## \#63 Posted by: dg798 Posted at: 2017-09-01T19:46:25.648Z Reads: 30

```
Is there anything I could do??
```

---
## \#64 Posted by: dg798 Posted at: 2017-09-10T00:33:27.531Z Reads: 29

```
just got a nwe vesc and my motor is doing this https://photos.app.goo.gl/KLdi9hF3mh4jTVXh1
listen to video
```

---
## \#65 Posted by: dg798 Posted at: 2017-09-10T13:11:34.886Z Reads: 27

```
It doesn't even spin fully it jerks and shakes a ton. Even when it took it off the motor mount it still did that.
Is there something wrong with my motor??
```

---
## \#66 Posted by: dg798 Posted at: 2017-09-10T16:48:21.825Z Reads: 26

```
Can anyone help please
```

---
## \#67 Posted by: GrecoMan Posted at: 2017-09-10T17:22:41.038Z Reads: 24

```
Loosen all your mount screws and try again
```

---
## \#68 Posted by: dg798 Posted at: 2017-09-10T19:44:29.603Z Reads: 20

```
Did already and it still didn't work
```

---
