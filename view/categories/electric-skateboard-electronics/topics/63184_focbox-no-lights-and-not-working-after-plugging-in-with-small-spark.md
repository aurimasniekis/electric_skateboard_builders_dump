# Focbox no lights, and not working after plugging in with small spark

### Replies: 20 Views: 624

## \#1 Posted by: 12meterkuk Posted at: 2018-07-28T23:00:12.352Z Reads: 126

```
The remote receiver still has power though, what might be the problem?
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-07-29T02:53:53.472Z Reads: 117

```
show pics of the board
```

---
## \#3 Posted by: Eboosted Posted at: 2018-07-29T03:31:03.227Z Reads: 115

```
Open it up and post a picture of both sides of the board, it only has 3 Allen bolts
```

---
## \#4 Posted by: 12meterkuk Posted at: 2018-07-29T03:46:03.089Z Reads: 110

```
![image|375x500](upload://sxKmdhctb9w9D5xw8BdwxyCOUA5.jpeg)![image|375x500](upload://pBlfN1b48Tpca812oSyq5arAAZs.jpeg)
```

---
## \#5 Posted by: dareno Posted at: 2018-07-29T07:14:10.314Z Reads: 103

```
Single drive?
```

---
## \#6 Posted by: 12meterkuk Posted at: 2018-07-29T07:30:25.688Z Reads: 103

```
dual, both not turning on
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-07-29T08:07:53.255Z Reads: 104

```
Burn mark on the diode, did you plug it in reverse polarity
```

---
## \#8 Posted by: dareno Posted at: 2018-07-29T08:37:07.356Z Reads: 101

```
are they connected with canbus?
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-07-29T09:05:26.083Z Reads: 98

```
Have you tried connecting both FOCBOXes separately to PC and re-flashed them?
```

---
## \#10 Posted by: 12meterkuk Posted at: 2018-07-29T09:40:13.814Z Reads: 92

```
yes

10cha r
```

---
## \#11 Posted by: 12meterkuk Posted at: 2018-07-29T09:40:40.798Z Reads: 92

```
i don’t know, I plugged it in after reflash it proper firmware and it wouldn’t turn on
```

---
## \#12 Posted by: 12meterkuk Posted at: 2018-07-29T09:40:47.993Z Reads: 90

```
Yes I have
```

---
## \#13 Posted by: dareno Posted at: 2018-07-29T09:46:20.610Z Reads: 93

```
My friend you are in the best hands with @CarlCollins
```

---
## \#14 Posted by: CarlCollins Posted at: 2018-07-29T10:26:16.545Z Reads: 83

```
@12meterkuk
Download and install team viewer on your MAC/Windows PC, Let me check both of your FOCBOXes
```

---
## \#15 Posted by: 12meterkuk Posted at: 2018-07-29T10:55:01.505Z Reads: 81

```
Okay, let’s do that tomorrow. I’m not home today
```

---
## \#16 Posted by: CarlCollins Posted at: 2018-07-29T10:58:57.147Z Reads: 82

```
Sure thing
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-07-29T11:05:07.606Z Reads: 82

```
If you ran canbus and 5v working and blue led not it's probably can bus ic died. 

Did you plugged only one focbox power while they were canbus connected?
```

---
## \#18 Posted by: 12meterkuk Posted at: 2018-07-29T11:18:30.487Z Reads: 81

```
I can’t remember if that was the case, what I remember is after flashing firmware and I restarted the board the Fox boxes wouldn’t turn on
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2018-07-29T16:46:16.270Z Reads: 71

```
Check this capacitor, if it is short... most likely the can transceiver is dead, so the 3,3v (NOT the 5v, that why your receiver is still powering up)

https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#20 Posted by: Rysa Posted at: 2018-10-09T04:33:24.353Z Reads: 50

```
Looks like I've found the right thread, as i'm having the exact same issue! i've tested the c25 capacitor and my multimeter does start beeping (indicating a short?). I too had a small spark inside my XT60 when plugging the FOCBOX to my battery, however all leads seem to be wired correctly and its a 42V 18650 battery pack that is at the correct voltage. When i plug my battery in i get 5v out of all 5v pins but no lights and nothing out of the 3.3v pin. Is there anything i can do to fix this, and can anyone suggest how this occurred in the first place? here are some photos of my setup...

![IMG_6764|666x500](upload://rt9NYe7yIKwCD8ndg1LZLlTrZl8.jpeg) ![IMG_3067|666x500](upload://i1GlyfYNtSpoaJZVX8FdwiioHD.jpeg) ![IMG_7295|375x500](upload://kDTh2F0U24SP1kQ3AKhctWSkU32.jpeg) 

Thanks for your time

PS. Its a Dual Motor setup
```

---
