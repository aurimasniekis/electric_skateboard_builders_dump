# \[Help\] VESC BLDC Problem &#124; Motor acting up, twitching

### Replies: 17 Views: 1724

## \#1 Posted by: lilracerboi Posted at: 2016-07-30T20:13:44.586Z Reads: 108

```
I got my Space Cell Pro 4 in today, set everything up and went to ride it, but not even half a mile the board jitters and now the motor twitches when hitting the throttle.
This happens in BLDC, but when I switch it to FOC, it works fine. No idea what caused this as nothing in the VESC was changed.

Also, the DRV chip looks fine. Nothing burnt looking or anything.

Edit: Scratch that, FOC doesn't work either. Tried riding and motor would scream. Might need a new motor?
```

---
## \#2 Posted by: c4Lvin Posted at: 2016-07-30T20:51:09.293Z Reads: 102

```
I'm having a similar problem but not sure if it's exactly. Try unplugging and disconnecting everything and plug it back up. If you have another motor to plug it, try it there and if it works, plug it back to your original. It works for me.
```

---
## \#3 Posted by: lilracerboi Posted at: 2016-07-30T20:58:08.451Z Reads: 100

```
I've already tried unplugging and replugging everything and it still has issues. No faults show up either and I don't have another motor to test as I am the only person I know in my city who does what we do.
```

---
## \#4 Posted by: lilracerboi Posted at: 2016-07-31T00:45:54.459Z Reads: 88

```
Here is a video of my problem:

https://youtu.be/wwe-61BQpAU
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-31T00:47:59.053Z Reads: 81

```
check if you have a phase wire short in the motor. You'll probably have to open up the motor to test. Seems like a lot of people are having this issue with R-spec lately.
```

---
## \#6 Posted by: lilracerboi Posted at: 2016-07-31T00:59:41.235Z Reads: 80

```
The motor works fine on my old HobbyWing ESC, so I suspected the VESC.

It could be a combination of both though......
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-31T01:01:35.377Z Reads: 78

```
Hm weird, maybe see if there are any shorts on the VESC phase wires? or perhaps on the mosfets they're connected to?
```

---
## \#8 Posted by: lox897 Posted at: 2016-07-31T01:02:25.882Z Reads: 78

```
Sounds like a phase wire issue to me.
```

---
## \#9 Posted by: lilracerboi Posted at: 2016-07-31T02:43:51.242Z Reads: 73

```
I'm going to open it up as soon, as I get the circlips out...
```

---
## \#10 Posted by: Jinra Posted at: 2016-07-31T03:40:07.669Z Reads: 71

```
So if the phase wires are shorted you should have resistance as you try to spin the can by hand? Do you have resistance, or does it turn pretty easily? Make sure you twist the wires around while turning to see if there is a short in a certain position.
```

---
## \#11 Posted by: lilracerboi Posted at: 2016-07-31T05:15:06.131Z Reads: 62

```
That's another thing I thought about. There is no resistance when spinning the wheel freely.

Like I said, it works with my old ESC currently. When I first got the space cell earlier today, it worked, but had issues and the final moment it was working, it activated the brakes kinda hard and unusual.

I really believe it's the VESC. Something with the phase cables or mosfets.
```

---
## \#12 Posted by: Jinra Posted at: 2016-07-31T05:16:01.221Z Reads: 59

```
Maybe try re-flashing the f/w to rule that out?
```

---
## \#13 Posted by: lilracerboi Posted at: 2016-07-31T05:21:11.661Z Reads: 62

```
I'll try that tomorrow. I don't want to deal with this at the moment.
```

---
## \#14 Posted by: lospollos Posted at: 2016-10-14T20:32:42.716Z Reads: 44

```
Hey man! Did you solve this problem? I'm having the same problem right now and I would appreciate to hear if/how you solved it?
```

---
## \#15 Posted by: lilracerboi Posted at: 2016-10-14T20:38:26.609Z Reads: 44

```
Yes, I did get it resolved. 

As @Jinra stated, it was, in fact, a phase wire issue, but what threw me off was there was no resistance when spinning the motor by hand. 

All I did to fix it was take the motor apart and insulate the phase wires with some heat shrink tubing. Electrical tape also works. Just make sure to keep the insulation low profile so it won't hit against the shell.
```

---
## \#16 Posted by: lospollos Posted at: 2016-10-14T20:50:50.398Z Reads: 44

```
Alright :confused: I have glued the motor pulley to the motor shaft with red locktite because enertion failed to send me the key... I hope I will get it disassembled so I can check this.

Thanks for the help
```

---
## \#17 Posted by: lilracerboi Posted at: 2016-10-14T21:06:05.356Z Reads: 41

```
Try and hit it with a heat gun.
I had red locktite on the set screw as well as super glue to keep the pulley from sliding.
I used my heat gun to boil the super glue and loosen the locktite and it slid right out.
```

---
