# How to upgrade firmware on FOCBOX?

### Replies: 13 Views: 1418

## \#1 Posted by: Morxy49 Posted at: 2018-07-26T12:50:59.824Z Reads: 246

```
I'm not sure how I update the firmware on a FOCBOX?

How do I know what hardware version I have? 

Where can I download the firmware?
```

---
## \#2 Posted by: PartyPoison Posted at: 2018-07-26T12:51:47.942Z Reads: 246

```
Vesc tool
Connect
Firmware tab
Update
```

---
## \#3 Posted by: Morxy49 Posted at: 2018-07-26T12:53:22.184Z Reads: 240

```
Can't I use the bldc tool?
```

---
## \#4 Posted by: PartyPoison Posted at: 2018-07-26T12:56:25.726Z Reads: 239

```
Modded version (Bluetooth) 
https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116?u=partypoison
```

---
## \#5 Posted by: PartyPoison Posted at: 2018-07-26T12:58:39.876Z Reads: 227

```
Here might help!
https://www.electric-skateboard.builders/t/how-to-program-canbus-properly-video-tutorial/52606?u=partypoison
```

---
## \#6 Posted by: goldrabe Posted at: 2018-07-26T13:10:21.034Z Reads: 210

```
To update the firmware you can downloadd the latest Vesctool here.
https://vesc-project.com
From there it's pretty straight forward.
Hardware version 4.12
```

---
## \#7 Posted by: Morxy49 Posted at: 2018-07-26T13:12:21.507Z Reads: 203

```
So in other words all FOCBOXes are using hardware version 4.12? Always?
```

---
## \#8 Posted by: goldrabe Posted at: 2018-07-26T13:20:30.371Z Reads: 198

```
Sorry man, i was talking bullshit!
You only need the latest Vesctool to install the bootloader without st-link!
The Focboxes are based on the 4.12 Hardware but have some improved components.
The compatible firmware is for hardware version 4.12.
Watch the videos linked above and you will be fine.
```

---
## \#9 Posted by: Slak Posted at: 2018-07-26T15:34:11.377Z Reads: 178

```
Yes, sure you can. I'm using 2 Focbox in a dual build, running firmware 2.54 and using BLDC-Tool to configure.
```

---
## \#10 Posted by: Morxy49 Posted at: 2018-07-26T16:11:51.729Z Reads: 165

```
Okay, this seems like a good choice. Especially the remote drop out safety thingy. 
So how do I install this? With the Vesc Tool?
```

---
## \#11 Posted by: PartyPoison Posted at: 2018-07-26T16:24:45.532Z Reads: 153

```
There's a link there for you to download (its same  as vesc tool but modded)
```

---
## \#12 Posted by: Morxy49 Posted at: 2018-07-26T16:29:31.108Z Reads: 149

```
Oh okay, so Ackmaniack's mod is not a firmware, it's a tool. Am I getting this correctly?
```

---
## \#13 Posted by: PartyPoison Posted at: 2018-07-26T16:44:10.519Z Reads: 141

```
Yup! Its a tool with firm already
```

---
