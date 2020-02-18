# NoName &#124; Enertion R-SPEC motor &#124; Custom Mount &#124; 10S4P &#124; VESC &#124; BMS

### Replies: 8 Views: 1023

## \#1 Posted by: Bloop Posted at: 2017-06-05T19:22:36.835Z Reads: 140

```
Hello guys. Finally i'm back and so close to my final e-board.

Here are some pictures with my almost finished board. I don't think i will keep it drop through﻿ since i need some clearance for batteries and motor.

<img src="/uploads/db1493/original/3X/2/c/2c6b97540147e1b72b4d0c1f29e70145b92e7b9a.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/b/1bddcb7e5e35309a67baed2193adb7952d4e18db.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/3/63b5e9bb370741c0930589f62d96e690a3bd31e4.jpg" width="666" height="500"> 

List of components:

1. VESC
2. Enertion motor 190 kv
3. Enertion Nano X controller 
4. 10s BMS from BesTech 80A discharge with e-switch
5. Trucks, pulley and wheels also from Enertion
6. Custom battery pack from samsung 25r 18650 cells 


I've been reading post for a long time and i found some schematics that i really like and i think they are really good ( please let me know if i'm terrible wrong ).

Here are my batteries: 
<img src="/uploads/db1493/original/3X/1/f/1f4ef3a9461fefd325031fd3319e30632f775d1c.jpeg" width="333" height="250">

I want to group them into 5 * 2s4p connected with this kind of connectors 
<img src="/uploads/db1493/original/3X/4/4/44c1b6793fd8ffb2fab9eaad84c3b24ac0b99f23.jpg" width="200" height="200">

Hopefully by the end of this week i will have them welded and ready to use. The electrical circuit im thinking of something like this: 
<img src="/uploads/db1493/original/3X/2/3/237e0c0cbe204003fc6f7fb2eb12a8766b06b072.png" width="690" height="213">

Using antispark XT90. Im hoping this will be enough for protection and i wont have any problem with the bms/vesc.

And sunday i will have the motor mount finished. Here are something that i prototyped last night.
<img src="/uploads/db1493/original/3X/c/c/cc6bc1acc3c6fda43a48676853fa3b6e335e7421.png" width="690" height="349">
<img src="/uploads/db1493/original/3X/a/7/a7e986f9592d8ed475df6bd095a018e8bbb0d822.png" width="627" height="393">
<img src="/uploads/db1493/original/3X/4/b/4b1066fba40f8010f4cfd32507fcf550da0a80fa.png" width="662" height="376">


**I still have some problems that i need to figure out maybe someone here could give me a hand.**

1. Do i need anything else to protect the vesc/motor/batteries ? I will use the XT90 loop key to disconnect the vesc from the batteries while the board is charging. Anything i need to know ? i used lipo-liion batteries before but never that powerful. 

2. I really need some enclosures for battery and maybe something for vesc ? how can i protect this part from rocks or other hits? I saw lots of builds making it with an oven heating plastic and making mold etc.. i dont really think this is an option for me :\ so what else could i use any ideas would be awesome.


I will come back with more pictures when i finish more parts or when i get them together.
```

---
## \#2 Posted by: Bloop Posted at: 2017-06-08T06:22:03.483Z Reads: 100

```
As i prommised here are some pics with the battery :D


<img src="/uploads/db1493/original/3X/3/4/34d923feb0c16316ab8ca8ac67d6b06c7687eb9b.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/8/c/8c035b5e0a2cda5198745c820fdcf4f1f25bcecb.jpg" width="666" height="500">

 <img src="/uploads/db1493/original/3X/f/3/f3f92554baab5f73375cb6acd5345f9c3507bfa2.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/a/0/a0e1951be98940bbdb19ea1ebb751ac9b7e93269.jpg" width="375" height="500">

I decided to keep it as a whole pack for now i will see with next builds if ill change it.

<img src="/uploads/db1493/original/3X/1/2/122d5b260f8999923dd6f24b7ca54faad588c719.jpg" width="375" height="500">

 <img src="/uploads/db1493/original/3X/6/8/682a0c3c4e4700d94330b007c72d059bc0fe4656.jpg" width="375" height="500">
```

---
## \#3 Posted by: Bloop Posted at: 2017-06-08T06:23:38.260Z Reads: 92

```
i used awg12 cables ... now im not sure if they will be enough for this setup? 

any ideas?
```

---
## \#4 Posted by: Tuomalar Posted at: 2017-06-08T08:08:34.947Z Reads: 88

```
I thinf most of us use 10awg from battery (for some reason) and 12awg everywhere else like vescs and motor cables.
```

---
## \#5 Posted by: Bloop Posted at: 2017-06-10T19:18:03.463Z Reads: 73

```
Hey guys i have a big question here..

im using this bms 
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

And i dont get the e-switch.. i turned it on and i get 37V out of my battery and then when im turning it off it still getting me 37V ... what is that switch even doing ?

Thank you
```

---
## \#6 Posted by: mccloed Posted at: 2017-06-10T22:54:11.829Z Reads: 65

```
I noticed in your picture above that only the balance leads are connected to the BMS. Might be a dumb question but, Do you have the main leads connected to the BMS?
```

---
## \#7 Posted by: Bloop Posted at: 2017-06-11T05:27:55.402Z Reads: 59

```
@mccloed Yes i didnt update the pics yet. the black wire from battery is  connected to B- then from P- im getting another black wire to the vesc and the red wire to the loop key and into the vesc

I will update pics this week but for some reasons the e switch is doing nothing for me..
```

---
## \#8 Posted by: Bloop Posted at: 2017-06-13T21:57:44.266Z Reads: 43

```
Hi guys i just got my charger and im wondering if would be any problem that it outputs 42.8V (i measured it) i guess is not a problem for the bms right ?? Here are the bms specs

<img src="/uploads/db1493/original/3X/0/5/051ed3b7860d785f2d9dbc30c7c628d6ca8ec746.png" width="652" height="500">

And one more thing any idea if i can set up the vesc with nano X remote to go backwards when i press a button or something ? I know is possible to add the reverse but i dont want it always on.
```

---
