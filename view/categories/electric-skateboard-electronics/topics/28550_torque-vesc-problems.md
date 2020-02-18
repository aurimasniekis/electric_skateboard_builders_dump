# Torque VESC problems

### Replies: 19 Views: 776

## \#1 Posted by: GrecoMan Posted at: 2017-07-25T02:04:11.598Z Reads: 114

```
Hello all, I have just gotten off of a 2 and a half hour chat with torqueboards customer service about my vesc (note: this topic is NOT meant to bash torqueboards in any way.) not working correctly. When I plug the vesc into my PC everything will boot up nicely but when I go to run the motor detection test the motor spins extremely slowly (7ish rpm) before making a sound like one of the phase wires is disconnected. I have to voltage cutoff setting correct and the torqueboards 6s2p epower pack I was using was charged to 100% that whole time. Any help is appreciated because they do not offer any sort of warranty or repair and I have already gone almost $300 over budget 😬
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2017-07-25T02:15:05.528Z Reads: 109

```
have you tried switching your cables up.. could just have the phase cables plugged wrong..
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-07-25T02:27:58.973Z Reads: 104

```
Yes I have tried that, and everything in between. After the motor detection fails the red light flashes four times, does that mean anything?
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-25T02:29:01.423Z Reads: 97

```
after you get it to flash 4 times, go to terminal and type "faults"
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-07-25T13:03:12.552Z Reads: 75

```
@Jinra ok I did and I got FAULT_CODE_NONE
```

---
## \#6 Posted by: TranxFu Posted at: 2017-07-25T13:05:55.887Z Reads: 77

```
Did you check your phase wires ? I've had this issue before and I figured that the phase wires coming from the motor were dismantled and fkd up... After resoldering it, it worked just fine
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-07-25T13:07:02.061Z Reads: 73

```
have you tried switching it off and on again? :monkey:

jokes aside; pls post a screenshot of you bldc tool motor detection.
Could be a problem there, but mostly it´s the motor which is fuckd up in some way.
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-07-25T13:07:28.391Z Reads: 69

```
so I should resolder the phase wires coming from the motor or coming from the VESC? how should I go about doing that?
```

---
## \#9 Posted by: TarzanHBK Posted at: 2017-07-25T13:09:17.423Z Reads: 66

```
hell no! you should check if they are shorted in some way and if they are, isolate them properly
If you have stiff wires, you could resolder flexwires if you want.
But mainly check if they are shorting somewhere
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-07-25T13:09:51.479Z Reads: 64

```
<img src="/uploads/db1493/original/3X/9/b/9b3facd9096e85a893575bb5eeb3d1af0cdca5d7.PNG" width="690" height="388">
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-07-25T13:10:23.052Z Reads: 58

```
oohhhhh, none of them are shorted, they are all protected with heatshrink
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-07-25T13:13:32.769Z Reads: 59

```
how long are your motor wires?
Doesn´t look like somethings wrong in your bldc.
You could try to rise the detection current up to 8A and try again.
```

---
## \#13 Posted by: GrecoMan Posted at: 2017-07-25T13:17:10.000Z Reads: 56

```
HOLY CRAP!!!! I fixed it, one of my motor mount screws was to tight :sweat_smile:
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-07-25T13:18:22.783Z Reads: 58

```
there you go!
have fun riding ;)
```

---
## \#15 Posted by: GrecoMan Posted at: 2017-07-25T13:19:13.337Z Reads: 58

```
wait, but now to motor will do the detection test but wont spin when I use the arrow keys or the remote
```

---
## \#16 Posted by: TarzanHBK Posted at: 2017-07-25T13:20:32.296Z Reads: 63

```
after detection, hit "apply" then "write configuration" (that´s what people are forgeting about all the time)
```

---
## \#17 Posted by: GrecoMan Posted at: 2017-07-25T13:21:25.939Z Reads: 64

```
yea I did that, still nothing :confused:
```

---
## \#18 Posted by: TarzanHBK Posted at: 2017-07-25T13:22:28.576Z Reads: 63

```
Do it again and reboot vesc. Otherwise you have a setting wrong
```

---
## \#19 Posted by: GrecoMan Posted at: 2019-05-27T18:28:06.100Z Reads: 18

```
Nostalgia is a bitch 😭
```

---
