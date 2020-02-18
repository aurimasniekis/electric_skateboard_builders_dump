# Fscesc6.6 Dual canbus

### Replies: 13 Views: 285

## \#1 Posted by: Flasher Posted at: 2019-06-02T01:09:20.287Z Reads: 95

```
Anyone know how to fix canbus problems on a dual flipsky 6.6? I am unable to control my slave through the master UART port using my photon remote.
```

---
## \#2 Posted by: dareno Posted at: 2019-06-02T02:47:16.751Z Reads: 81

```
https://www.electric-skateboard.builders/t/flipsky-dual-fsesc-6-6-discussion-findings/67155/381

Probably find the answer in here or at least an expert to help.
```

---
## \#3 Posted by: Flasher Posted at: 2019-06-02T02:50:52.430Z Reads: 80

```
nice pic but not exactly what im looking to do. i want the left side to communicate with the right side. i know its supposed to do it on its own but something is preventing this. the switch for dual is toggled on already
```

---
## \#4 Posted by: dareno Posted at: 2019-06-02T02:58:19.204Z Reads: 75

```
Its a link to the thread that deals with issues and findings with the flipper 6.6 dual.  Ask in there my friend.
```

---
## \#5 Posted by: Flasher Posted at: 2019-06-02T03:00:08.875Z Reads: 71

```
i already know about that thread. i asked sofu for an answer but im also going in a new topic to make a bit more noise
```

---
## \#6 Posted by: dareno Posted at: 2019-06-02T03:05:43.014Z Reads: 68

```
Hate to say it but if they don't know in there then you may be fucked lol

Sorry couldn't be more helpful.  Keep asking and someone will chime in from a different timezone.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-06-02T06:48:15.159Z Reads: 55

```
If I remember right this problem was discussed in the thread you linked @dareno 

If it’s the version without CAN bus headers than there is a way to bridge the switch or bypass the switch to connect both sides. I remember seeing pictures where it’s marked where you can solder wires on.
```

---
## \#8 Posted by: dareno Posted at: 2019-06-02T06:54:57.241Z Reads: 54

```
You can lead a horse to water.....
```

---
## \#9 Posted by: Andy87 Posted at: 2019-06-02T06:57:12.365Z Reads: 52

```
I just checked the picture from there website. There would be a way to use dual receiver. The ports are there you just need to solder wires on the skate side.
```

---
## \#10 Posted by: Komamtb Posted at: 2019-06-02T08:08:39.351Z Reads: 45

```
Then I first set up my photon with the 6.6 dual, it kinda worked, now I have the same problem, do you get the pulsewidth to show on the vesc tool?
```

---
## \#11 Posted by: Flasher Posted at: 2019-06-02T10:36:08.644Z Reads: 35

```
I found out I had to play with the Nunchuk app for some reason. @Andy87 I thought I read thoroughly all posts in that thread  but i might have missed it. In case I need to know, did you mean splitting a 6 pin like power cables on a computer?![jpeg_1559471725399|690x412](upload://nMdwHxYsEnOLwh2HNlQKEQIKbbP.jpeg)
```

---
## \#12 Posted by: Andy87 Posted at: 2019-06-02T18:51:54.163Z Reads: 27

```
Sorry my bad. I didn’t see that you use the uart port as receiver input. The ppm port you could just y-split and remove the 5V cable on one side. With the uart i‘m not sure if it would work.

Did you try it with a ppm remote to find out if it’s an issue with the CAN connection or with the settings or uart port?
```

---
## \#13 Posted by: Flasher Posted at: 2019-06-02T19:06:46.433Z Reads: 26

```
No I didn't. I only have prebuilts (koowheel/buffalo) with onboard receivers. I went specifically for the photon remote for my first diy build
```

---
