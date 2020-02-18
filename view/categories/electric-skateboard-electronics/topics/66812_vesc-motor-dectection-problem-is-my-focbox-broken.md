# Vesc motor dectection problem, is my FOCBOX broken?

### Replies: 3 Views: 162

## \#1 Posted by: MaxMalouf Posted at: 2018-09-02T06:56:44.771Z Reads: 56

```
So I have a Focbox and i was running perfectly for a month in FOC mode. As i am using ACKMANIAC's bldc tool with Bluetooth module and the vecs monitor app, I wanted to also program BLDC so i could switch between them on the go using the vesc monitor app. So as i opened up my board and went to program my motor for BLDC, I was expiriencing the exact same problems as this guy: https://youtu.be/Ng3kdIk48u8

A month ago when I was trying to program my focbox, I  had this problemb and all I did to fix the problem was writing voltage cutoffs. So i tried this and nothing worked. So I uploaded the firmware again, and tried turning it off and on, and still had no luck. But after trying to turn it on again, my reciver wasnt flashing and the fault light on my focbox was flashing. I tried to smell to see if I was getting any magic smoke, I dont think there was any, none that i could see or smell anyway. I noticed that the focbox itself was also getting a very hot while this fault light was flashing.

I typed fault into the terminal and this is what I got:![20180902_162623|375x500](upload://gGGFg3Ej3e2HY9GclM5KcdOOMeb.jpg)

I then turned it off immediately as the focbox was getting warm, I tried to set voltage cutoffs but have no luck :( 

Please, i am desperate for help! 
Thanks.
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-09-02T18:36:35.043Z Reads: 37

```
Have you tested the output of the battery? Something may have shorted there
```

---
## \#3 Posted by: MaxMalouf Posted at: 2018-09-03T00:06:46.938Z Reads: 29

```
No the battery seems perfectly fine.
```

---
