# VESC 4.7 : component upgrade?

### Replies: 6 Views: 200

## \#1 Posted by: akira Posted at: 2018-08-10T08:22:18.685Z Reads: 68

```
Hello,
I am back to esk8 after a long brake. I still have two (collector) pieces : 4.7 VESC soldered by the master himself. I intend to use them with 9S battery and 190KV enertion 6355 motors.
I was wondering if I could upgrade them (beefing up some capacitors for example).

Do you have an advice ?
```

---
## \#2 Posted by: linsus Posted at: 2018-08-10T08:29:38.033Z Reads: 67

```
Does the BoM differ from VESC6? If not, then no need. Havnt been able to slay any of my hand soldered 6's so far. I have some older PCBs before production, so I know there were some small alterations. Nothing major tho
```

---
## \#3 Posted by: akira Posted at: 2018-08-10T08:56:58.009Z Reads: 58

```
I think you misread my post. 
I have the 4.7 version. I know for sure that there have been BOM modification compared to V4.12 like capacitors. Also Chaka changed some components. I was looking for advice on useful and possible mods for V4.7.
 
Compared to VESC6, many things are different, you can hardly compare them in the context of V4.7 upgrade.
```

---
## \#4 Posted by: linsus Posted at: 2018-08-10T09:08:16.405Z Reads: 52

```
Ah, by master i thought you meant BV. The early test board of vesc6 was a v4 (or maybe 5.?)something. 
I have some old 4.10-4.12 VESCs laying around. Theres one cap that is needs to be parallelled with the same value. (parallell on caps is same as plus), other then that I havnt modified them. They run ok in BLDC. FOC is bit riskier tho. Changed DRV few times.
```

---
## \#5 Posted by: akira Posted at: 2018-08-10T09:10:46.838Z Reads: 50

```
Yes I meant vedder ;-)

OK thanks, I'll dig in the forum archives to find which cap to solder in parallel. 
I will surely not run them in FOC mode. For this, I'll use a FOCBOX or a VESC6.
```

---
## \#6 Posted by: linsus Posted at: 2018-08-10T09:15:47.878Z Reads: 48

```
I blame BV tbh, he convinced me over and over that they "should" run fine in FOC. Depends a Little on what motor as well. SK3s are usually ok, but there are some motors which are prone to produce the DRV error more frequent. Impendance etc has to do with it. 


Found the post about the CAP :) its C18.
http://vedder.se/forums/viewtopic.php?f=5&t=68&hilit=Cap+solder
```

---
