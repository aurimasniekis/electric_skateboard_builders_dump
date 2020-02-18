# Question BMS voltage cutoff

### Replies: 5 Views: 330

## \#1 Posted by: Deakbannok Posted at: 2018-01-08T04:47:48.907Z Reads: 68

```
Hi everyone.
I  am running discharge through my 60amp BMS. It seems that BMS will shutoff once my voltage dropped at 36v.
My pack is 10s4p and this is the BMS I use. Is anyone have the same experience with this BMS

www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

<img src="/uploads/db1493/original/3X/7/d/7dca25bbc02779215fd7b2378178d6cb583194de.jpg" width="281" height="500">

Thank you
```

---
## \#2 Posted by: L3chef Posted at: 2018-01-08T07:01:01.966Z Reads: 56

```
What esc do you have? I have the same bms without issues. Probably your battery cut off start/end settings that's the cause of this.
```

---
## \#3 Posted by: Deakbannok Posted at: 2018-01-08T07:18:01.303Z Reads: 55

```
I have torqueboard vesc. 
Is not the vesc that cutting off.
Is my BMS that cut off the power completely once it hit the 36v. because the antispark switch is cut off too.
My setup is BATTERY - BMS - Antispark - VESCs 

Are you running bypass BMS or you have it discharging through BMS on your setup?
```

---
## \#4 Posted by: L3chef Posted at: 2018-01-08T07:27:32.683Z Reads: 52

```
Check this box in bldc tool.
<img src="/uploads/db1493/original/3X/3/3/33fd35daf0678363f28085d5251e0d7212754031.jpg" width="690" height="388">

Ah missread a bit. So what does the multimeter read after the antispark switch?
And before the bms
```

---
## \#5 Posted by: Acido Posted at: 2018-01-08T12:19:18.657Z Reads: 41

```
Change your bms maybe
```

---
