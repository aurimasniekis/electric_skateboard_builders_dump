# VESC problem. motor won&rsquo;t spin

### Replies: 17 Views: 746

## \#1 Posted by: DaniRC Posted at: 2018-11-05T19:05:15.502Z Reads: 102

```
I assembled my esk8 last week and I rode for an hour withouth problem. Yesterday my friend was testing and it stopped. When he come back a phase motor wire was loose. I connected again but not response from the motor.
I have check all the conection, I've tried another motor and still no response. Also I've changed the battery for a power supply in order to check all the component so I tend to think that the problem is in the Vesc but not sure.
My Vesc is a 4.12 turnigy.
There are apparently no burnt or damage component. I can connect to PC and receive response. Light green/blue ON. No faults on terminal. Firmware updated again.
Everything seem OK but when I try to config the motor no spin nor other sound.
Any advice in how to confirm that is my VESC that is broken?


Setup:
sk3 6374 168kv
2x6s 4,5 lipo turnigy 40c
vesc 4.12 turnigy
BMS (Chinese bypassing) -> Removed to test

Screenshots of the results
Firmware
![1|690x374](upload://dr3SmkpIG5k8uG2L8HxRRhPdyKV.png) 
Motor config FOC mode results
![2|690x370](upload://fF3Z6VCJlTeSKFCt8POyDi1J8v1.png)
![5|690x370](upload://tHuCBmvHhbNoFTbDinh8G7gKOS7.png)
 ![6|690x371](upload://u55FjnW16Pdcqvx377W0h6mICYL.png) 
![7|690x371](upload://3VA8T5rfNw17eQ3l92ezuPfKFhC.png) 
Realtime data
 ![3|690x368](upload://5OhJorfiCrw874XRCmlOBtIFRlv.png) 
spinning the motor by hand
 ![4|690x370](upload://opDy1ReKOWSQOTJJNL45ThvWchx.png)
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-11-05T19:20:37.862Z Reads: 79

```
With everything plugged up and on, check to see if your fet on the vesc is getting hot. If so, its popped inside.
```

---
## \#3 Posted by: DaniRC Posted at: 2018-11-05T19:31:16.178Z Reads: 78

```
No, it's cold.
```

---
## \#4 Posted by: J0ker3366 Posted at: 2018-11-05T19:34:14.490Z Reads: 79

```
Do you have a voltmeter? If so, check voltage throughout the system. You may have a loose connection on the vesc or leads in motor came off.... Not being able to see it does leave us in the dark though.
```

---
## \#5 Posted by: Quiles Posted at: 2018-11-05T19:42:46.272Z Reads: 74

```
go on vesc terminal and type fault to check for errors
```

---
## \#6 Posted by: DaniRC Posted at: 2018-11-05T19:46:29.303Z Reads: 71

```
[quote="J0ker3366, post:4, topic:73560, full:true"]
Do you have a voltmeter? If so, check voltage throughout the system. You may have a loose connection on the vesc or leads in magnet came off… Not being able to see it does leave us in the dark though.
[/quote]
Yes, I tested in all points and everything seem correct except inside the VESC because it has the transparent insulate. I will broke to test it but the VESC indicates a correct voltage.
I've added some screenshots in the first post.

https://www.electric-skateboard.builders/t/vesc-problem-motor-wont-spin/73560/5

No faults
```

---
## \#7 Posted by: Quiles Posted at: 2018-11-05T19:47:19.698Z Reads: 67

```
thats good...no DRV fault. did you try to do motor detection again?...just for the sake of it

edit: just saw that you tried that
```

---
## \#8 Posted by: CarlCollins Posted at: 2018-11-05T22:00:52.809Z Reads: 61

```
@DaniRC
Try to reset the values to default and then give it a try.
Also check by re-flashing the fimeware on FOCBOX again
```

---
## \#9 Posted by: DaniRC Posted at: 2018-11-06T10:01:51.841Z Reads: 58

```
I did and it didn't work but I will try again with crossed fingers :relieved:
```

---
## \#10 Posted by: DaniRC Posted at: 2018-11-06T13:09:30.963Z Reads: 56

```
It think that is a DRV problem. I've broken the insulate because it had an sticker and I wan't able to see the last corner. Although I don't have any DRV fault, it seem that it is burned.
![IMG_20181106_135915|666x500](upload://f8UnfibFBQH8M8tXd6mAebWPG4v.jpeg) 
![IMG_20181106_135906|666x500](upload://nuuVL9DA0FWbyhO31h9v9mL3bie.jpeg)
```

---
## \#11 Posted by: DaniRC Posted at: 2018-11-06T20:48:24.647Z Reads: 52

```
any place to repair in Europe?
```

---
## \#12 Posted by: Mich21050 Posted at: 2018-11-06T20:49:22.810Z Reads: 52

```
@Martinsp :smile:
```

---
## \#13 Posted by: CarlCollins Posted at: 2018-11-07T00:09:39.328Z Reads: 52

```
@DaniRC These ESCs are not good. Have you tried FOCBOX?
```

---
## \#14 Posted by: DaniRC Posted at: 2018-11-07T05:44:14.983Z Reads: 50

```
No yet but I'm going to buy a new Vesc. Don't have focbox the drv issue? It cost more than double with shipping to Spain.. Three times if I include the additional warranty :cold_face:
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-11-08T02:25:23.012Z Reads: 45

```
@DaniRC Let me help you get a FOCBOX
```

---
## \#16 Posted by: DaniRC Posted at: 2018-11-08T05:57:01.352Z Reads: 40

```
Yes, try it
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-11-08T08:22:15.471Z Reads: 35

```
@DaniRC
We have reseller available, have you checked them?
https://www.electric-skateboard.builders/t/certified-focbox-suppliers/39725
```

---
