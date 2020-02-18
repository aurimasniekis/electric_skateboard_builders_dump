# M Boards Dual motor esc Stuck in low power mode (solved)

### Replies: 12 Views: 124

## \#1 Posted by: Vinleei Posted at: 2020-01-14T14:53:31.904Z Reads: 36

```
The board consists of two batteries wich are seriers connected to a esc.  The esc starts up and I have no problmen connecting the esc to the controller. Howewer  the esc is beeping signaling that the board or the controller is in critically low power.This is a safe mode and it  disables the acceleration meaning that only the motor brake works. Both the batteries and the controler is fully charged. Can someone help ? I have searched the web for a while and can not find an answer. Can you program the esc ?
```

---
## \#2 Posted by: GenghisConman Posted at: 2020-01-14T17:31:19.569Z Reads: 30

```
yep, im having a similar issue. except it seems like the accelerations still works, but the power is cut wayy down. the power button also seems to blink in these times, haven't heard any beeping
```

---
## \#3 Posted by: Vinleei Posted at: 2020-01-14T18:18:09.280Z Reads: 26

```
I am going to try and change the voltage settings. Do you think that would work ?  Could be pre set for 10s
```

---
## \#4 Posted by: Vinleei Posted at: 2020-01-14T18:42:53.873Z Reads: 25

```
![bild|500x500](upload://6OpBsD9Omy6tx5pDR4qQOHShuZA.jpeg) ![bild|508x500](upload://kgj4IYK8YBTFwGzIWXkmdEd7kwc.jpeg)  ![bild|500x500](upload://a7sQ0iW4tz6p28FDCKHw231oLhh.jpeg)
```

---
## \#5 Posted by: GenghisConman Posted at: 2020-01-14T19:07:52.967Z Reads: 22

```
that might work. let me know. ive got my board with me rn, but im at the library so i cant really open it up. but if theres anything you need a second opinion on im here. I am running a 10s3p 30q. what battery are you running?
```

---
## \#6 Posted by: Vinleei Posted at: 2020-01-14T20:19:40.708Z Reads: 22

```
Im using one 3s 50c  and one 4s 50c  together 8300mah so a 7s configuration
```

---
## \#7 Posted by: Vinleei Posted at: 2020-01-14T20:25:06.021Z Reads: 22

```
do you know what the matching button does ?
```

---
## \#8 Posted by: GenghisConman Posted at: 2020-01-14T20:42:28.719Z Reads: 19

```
what button are you talking about?
```

---
## \#9 Posted by: Vinleei Posted at: 2020-01-14T20:54:48.635Z Reads: 20

```
there is a small button next to the buzzer and the development port
```

---
## \#10 Posted by: GenghisConman Posted at: 2020-01-14T20:56:12.945Z Reads: 22

```
ah, no i dont know what that does, im in a library, so i cant really open my board up. But i would think it might be some reset button
```

---
## \#11 Posted by: Vinleei Posted at: 2020-01-26T15:09:21.289Z Reads: 16

```
By ironing  the contact for 7s I was able to solve my problem. The esc is no longer set in low power mode
```

---
## \#12 Posted by: GenghisConman Posted at: 2020-01-28T22:08:35.162Z Reads: 8

```
hi, how is this done? i have 10s
```

---
