# Vesc 3.40 to 2.18 a diyelectricskateboards vesc

### Replies: 14 Views: 626

## \#1 Posted by: Harpsaco Posted at: 2018-08-23T05:50:01.466Z Reads: 130

```
I wanna use the bldc tool but I can't use it because of the firmware. so I did my research on here but I looked at the vesc tool bootloader and I don't understand it I just keep trying to update it to the 2.18 firmware but it wont work.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-08-23T06:03:27.355Z Reads: 125

```
You need the bldc tool, not the vesc tool I guess.
It’s the old version of the service program
```

---
## \#4 Posted by: Harpsaco Posted at: 2018-08-23T15:51:26.725Z Reads: 96

```
I used the bldc tool but it said vesc to old to read update firmware
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-23T16:07:13.848Z Reads: 86

```
You get this message when you open bldc tool right? Can’t you just ignore that message by pushing ok and after flash old firmware?
```

---
## \#6 Posted by: Harpsaco Posted at: 2018-08-23T18:08:47.323Z Reads: 73

```
It won't connect to the vesc
```

---
## \#7 Posted by: Andy87 Posted at: 2018-08-23T19:49:29.787Z Reads: 62

```
Hm that’s strange.
I never downgraded a vesc.
It should be possible like upgrading too.
I think with a stl link you could fix it easily but probably you don’t have that right?
You before already changed the firmware on your vesc or it’s first time?
Could be that there is no bootloader installed, which could be a reason why it’s not functioning.
Don’t  ask me how to check if there is a bootloader or not 😅
But i‘m sure a short search in our forum will give you an easy answer too it.
```

---
## \#8 Posted by: Harpsaco Posted at: 2018-08-23T19:53:06.164Z Reads: 60

```
How do I do so 
I bought the vesc from torque boards
```

---
## \#9 Posted by: Andy87 Posted at: 2018-08-23T20:07:37.487Z Reads: 56

```
https://www.electric-skateboard.builders/t/vesc-boot-loader-installation-tutorial/32103

Didn’t read everything. But looks like for this you also need a stl link. Thought I read somewhere that it’s possible also without 🤔
```

---
## \#10 Posted by: Andy87 Posted at: 2018-08-23T20:12:14.914Z Reads: 53

```
https://www.electric-skateboard.builders/t/want-to-update-firmware-but-dont-want-to-mess-up-the-vesc/61701

There is a bootloader tap in the vesc tool.
Try to check if you have that, if no load.
Than switch to bldc tool and try again to load the old firmware
```

---
## \#11 Posted by: Harpsaco Posted at: 2018-08-23T20:33:40.263Z Reads: 52

```
Ok I'll try when i get home
```

---
## \#12 Posted by: Esk88 Posted at: 2018-12-19T03:29:21.439Z Reads: 23

```
How did this go I think I have a similar problem

@trampa @JohnnyMeduse @Deodand
```

---
## \#13 Posted by: Sn4pz Posted at: 2018-12-19T03:42:31.179Z Reads: 22

```
You're going to have to provide more information....
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2018-12-19T03:48:16.347Z Reads: 18

```
Yeah, might need more info. 

Does it connect to the PC? What is the sequence the led does when it power up?
```

---
## \#15 Posted by: Esk88 Posted at: 2018-12-19T04:07:59.995Z Reads: 17

```
Whoops let me get that for y’all
```

---
