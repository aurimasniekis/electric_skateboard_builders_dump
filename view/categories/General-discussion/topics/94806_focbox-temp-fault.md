# Focbox temp fault

### Replies: 38 Views: 246

## \#1 Posted by: KaramQ Posted at: 2019-05-24T00:04:10.306Z Reads: 65

```
Using ackmaniac bldc tool version 3.103 and motor won’t run due to a temp fault read by the focbox although the motor is cold. What should I do, do I need to downgrade the version? @barajabali, @CarlCollins
```

---
## \#2 Posted by: KaramQ Posted at: 2019-05-24T05:33:40.596Z Reads: 51

```
Bump? 10jasons
```

---
## \#3 Posted by: Andy87 Posted at: 2019-05-24T05:41:04.085Z Reads: 45

```
might be your temp sensor is broken.
try to set up your motor without sensors and look if the fault still there. if no and you want to use your sensors non the less, just disconnect the temp sensor wire form the jst plug which goes to the focbox.
```

---
## \#4 Posted by: KaramQ Posted at: 2019-05-24T05:46:57.840Z Reads: 41

```
It stays after I take the motor off, it was working fine a few days ago. Also vesc tool says the firmware is too old but it’s 3.103
```

---
## \#5 Posted by: Andy87 Posted at: 2019-05-24T05:48:33.007Z Reads: 40

```
check real time data. what is the value of the temp? If it´s a fault you can´t reset, try to flash the same FW once again and hope it delete the fault.
```

---
## \#6 Posted by: KaramQ Posted at: 2019-05-24T05:48:59.074Z Reads: 38

```
It’s at 400° Celsius
```

---
## \#7 Posted by: KaramQ Posted at: 2019-05-24T05:49:49.915Z Reads: 35

```
Reuploaded firmware multiple times with no luck
```

---
## \#8 Posted by: Andy87 Posted at: 2019-05-24T05:50:49.233Z Reads: 35

```
[quote="KaramQ, post:6, topic:94806, full:true"]
It’s at 400° Celsius
[/quote]

just to get it right, it says 400 with and without sensor cable plugged?
```

---
## \#9 Posted by: KaramQ Posted at: 2019-05-24T05:51:35.793Z Reads: 33

```
plugged in and not plugged in. When motor is plugged in, motor does not heat at all
```

---
## \#10 Posted by: KaramQ Posted at: 2019-05-24T05:52:26.618Z Reads: 34

```
I’m running it in bldc at the moment as I don’t want to run sensored for the time being
```

---
## \#11 Posted by: Andy87 Posted at: 2019-05-24T05:57:09.263Z Reads: 34

```
[quote="KaramQ, post:9, topic:94806"]
plugged in and not plugged in
[/quote]

looks like there is something signal on your input port than. Unfortunately I have no idea how to check that or eliminate that.
Make sure all plins are clean (both sides of the pcb), maybe upload a not ack FW just as last try.
```

---
## \#12 Posted by: KaramQ Posted at: 2019-05-24T05:58:04.506Z Reads: 31

```
I tried with the bengiman vesc tool and no luck and as well as the enertion bldc tool
```

---
## \#13 Posted by: KaramQ Posted at: 2019-05-24T05:58:47.905Z Reads: 32

```
Maybe I uploaded the wrong firmware?
```

---
## \#14 Posted by: Andy87 Posted at: 2019-05-24T05:59:31.727Z Reads: 32

```
you can easily check that in the firmware section.
```

---
## \#15 Posted by: KaramQ Posted at: 2019-05-24T06:00:08.791Z Reads: 34

```
I did, on one tool it says up to date, then the other says the firmware is old, like wtf
```

---
## \#16 Posted by: Andy87 Posted at: 2019-05-24T06:01:14.550Z Reads: 33

```
no, go in the firmware section and look in the down left corner. there should be written which firmware is loaded. make sure it´s the one for HW4.12 and not 4.80
```

---
## \#17 Posted by: KaramQ Posted at: 2019-05-24T06:01:19.011Z Reads: 33

```
@Bobby tested it and it was running fine until I got it
```

---
## \#18 Posted by: KaramQ Posted at: 2019-05-24T06:01:41.591Z Reads: 32

```
Will do tommarow, thanks! Gotta crash, it’s 11:00 over here
```

---
## \#19 Posted by: Andy87 Posted at: 2019-05-24T06:02:02.933Z Reads: 32

```
good luck! hope all work out well.
```

---
## \#20 Posted by: KaramQ Posted at: 2019-05-25T05:12:48.668Z Reads: 28

```
Can you show me where the 4.12 is, I can’t find it when I go to the firmware
```

---
## \#21 Posted by: KaramQ Posted at: 2019-05-25T05:13:16.090Z Reads: 28

```
It says firmware 46
```

---
## \#22 Posted by: Andy87 Posted at: 2019-05-25T07:11:05.107Z Reads: 23

```
![image|374x500](upload://9GvnkXmAjApeTyzcp8sC5XwRQei.jpeg) 

410,411,412 is the file you need.

In the red field you will see the actual version installed on the vesc if you connected.
```

---
## \#23 Posted by: KaramQ Posted at: 2019-05-25T10:43:19.310Z Reads: 19

```
It wouldn’t allow me to download it, it kept redirecting me to 46
```

---
## \#24 Posted by: Andy87 Posted at: 2019-05-25T10:48:07.509Z Reads: 19

```
Than you have the wrong fw installed properly.

If you have one vesc with the right fw you could use the newest vesc tool and flash the right fw via CAN.

If no than you will probably need an st v2 link.
```

---
## \#25 Posted by: KaramQ Posted at: 2019-05-25T10:49:07.350Z Reads: 19

```
I have no clue how that firmware was downloaded, i never even played with the firmware
```

---
## \#26 Posted by: KaramQ Posted at: 2019-05-25T10:51:46.082Z Reads: 20

```
How would I get that st v2 link
```

---
## \#27 Posted by: Andy87 Posted at: 2019-05-25T11:00:53.832Z Reads: 19

```
Amazon 8$. Just search for stl v2.

Didn’t you said it was working before when you got it from an other user? Maybe he knows how the wrong fw came on it?
```

---
## \#28 Posted by: KaramQ Posted at: 2019-05-25T11:03:42.114Z Reads: 19

```
Yeah, he told me it was working and when I came to do motor detection, it somehow downloaded the firmware unless I accidentally flashed it without knowing better. It’s all @Boardnamics fault, I asked him to run motor detection and he probably flashed 46 since he has the trampa vesc😭
```

---
## \#29 Posted by: Andy87 Posted at: 2019-05-25T11:09:43.491Z Reads: 20

```
😂 but trampa is hw6 😂 so it would be wrong either way.

You don’t have a second vesc laying around you could use to flash the right fw?
```

---
## \#30 Posted by: KaramQ Posted at: 2019-05-25T13:51:03.735Z Reads: 17

```
My second esc is fried😂
```

---
## \#31 Posted by: CarlCollins Posted at: 2019-05-25T17:00:04.280Z Reads: 13

```
I would like to assist you over teamviewer, I think I am able to solve it
```

---
## \#32 Posted by: KaramQ Posted at: 2019-05-25T17:00:56.492Z Reads: 14

```
Not sure what team viewer is
```

---
## \#33 Posted by: CarlCollins Posted at: 2019-05-25T17:01:17.647Z Reads: 13

```
It's a software which allows remote access
```

---
## \#34 Posted by: CarlCollins Posted at: 2019-05-25T17:02:45.388Z Reads: 14

```
If you are using a Windows PC then I can do it right now
```

---
## \#35 Posted by: KaramQ Posted at: 2019-05-25T17:03:09.153Z Reads: 14

```
Let me download it on my laptop
```

---
## \#36 Posted by: KaramQ Posted at: 2019-05-25T17:03:31.582Z Reads: 14

```
Windows on my laptop, my pc is currently broken
```

---
## \#37 Posted by: KaramQ Posted at: 2019-05-25T17:08:15.080Z Reads: 12

```
Downloaded it
```

---
## \#38 Posted by: KaramQ Posted at: 2019-05-25T17:10:49.543Z Reads: 10

```
I have an ID and password, I need your ID
```

---
