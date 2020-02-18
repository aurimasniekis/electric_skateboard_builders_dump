# Vesc firmware issues

### Replies: 8 Views: 407

## \#1 Posted by: jourm Posted at: 2018-08-17T11:24:02.322Z Reads: 96

```
I have a maytech vesc 4.12 from eskating.eu that i have been using for a single drive,( 12s lipo 168kv sk3) without problems for about a year now. But now i am uppgrading to dual. I got another maytech 4.12 and another motor, tb trucks motormounts etc. I went to uppgrade the firmware on the vesc's to 3.4 using  vesctool and on the new previously unused one, everything went fine, uppgraded firmware did motor-detection and everything else.

But when I try to uppgrade the firmware on the vesc i have been using for a while (previously 2.18) the uppload seems to go ok, but a the very last second it disconnects saying "No such directory exists" or something similar. After that i cant connect to the vesc again until I turn it of and on again, at wich point it connects and still shows the old 2.18 firmware. And with the old fimware i cant change any settings in vesctool wich is a problem since i plan to connect the vesc's to eachother via canbus.

I have tried uppgrading the firmware both using vesctool and ackmaniacks vesctool but the same thing happens. If i start up the old bldc tool i can make changes, run motor detection and such but I'm scared to connect the vesc's on canbus when they are on different firmwares. 

Does anyone know why this is happening or what I could do to solve it? I guess i could try to find 2.18 fw for the other vesc and downgrade it using bldc-tool but i would much rather run them both on 3.4 fw. Is it okay to have two vesc's on different firmwares?
```

---
## \#2 Posted by: trampa Posted at: 2018-08-17T11:48:21.270Z Reads: 82

```
Your ESC probably has no bootloader installed. You need to upload the missing bootloader first. Vesc-Tool has a bootloader upload funktion in the Firmware section. 

Frank
```

---
## \#3 Posted by: briman05 Posted at: 2018-08-17T11:53:35.313Z Reads: 75

```
Where did you get your first Vesc
```

---
## \#4 Posted by: threebysix Posted at: 2018-08-18T07:05:40.811Z Reads: 56

```
Op mentioned that his first vesc was from eskating
```

---
## \#5 Posted by: briman05 Posted at: 2018-08-18T14:05:50.058Z Reads: 50

```
But some Vesc don’t have a bootloader
```

---
## \#6 Posted by: threebysix Posted at: 2018-08-18T20:40:11.877Z Reads: 45

```
True, like the flipsky's vescs
```

---
## \#7 Posted by: jourm Posted at: 2018-08-19T12:43:00.843Z Reads: 37

```
Thanks for your help, just uploaded the bootloader and everything works great now.
```

---
## \#8 Posted by: ciscotory Posted at: 2018-11-04T04:08:08.451Z Reads: 25

```
I'm facing a simelar problem with same Vesc's dual setup loangboard
did you use esc tool to upload the bootloader? if so
did you use the bootlader opton in the tool as below?!
[bootloader|584x106](upload://sH2FiUFL8aECiczgudTGhjIVTnl.jpeg) 

 was serching and reading for a while :thinking: :roll_eyes: 
 i''ve updated my vesc's using ackmaniac esc tool, from Fw 2.54 to 3.10 even thoug it's the latest updat in Fw to my knoulge, but found out fw 3.10 it wont work with controller that i got for dual can-bus connection :smile:
tried few times changing thes vese fw to 2.18 still can.

can you let me know how you did? I've might missed somthing?
```

---
