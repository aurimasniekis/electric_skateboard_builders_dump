# GT2B connection/interference problems

### Replies: 23 Views: 316

## \#1 Posted by: Michaelj1 Posted at: 2018-10-16T16:21:17.413Z Reads: 92

```
So I’ve been using a GT2B remote for almost a year now, and I’ve been having connection issues. Originally it was thought to be caused by my antenna in the remote shorting out when I did the BadWolf mod, but even after fixing that I still had small disconnects and one of them even threw me off balance and left me on the ground (I was wearing a helmet thank god). Recently, I switched over to the baby buffalo case mod, because I really like thumb control over the touchy throttle the gt2b has. It uses the steering pot/ channel on the receiver, which has a really weird failsafe. The throttle failsafe just coasts but for steering, the motors continue to move for a bit, then the master motor coasts, and then the slave motor shortly after. On top of that I usually have to reconnect the remote which I didn’t have to do before. Anyway, I tried switching out the internals and the receiver with a new GT2B to see if I have a defect, and I’m still having issues, although now it’s scarier because of the weird steering channel failsafe. Could someone help me fix this? I just want my board to work with zero disconnects if possible. Also is there any way to change the failsafe so it just coasts?
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-16T16:29:02.658Z Reads: 90

```
Did you ever adjust your failsafe?
There is a button on the receiver which with you can reset the failsafe to the center position.
Where is your receiver located? Do you have a carbonfiber encloser or placed the receiver close to power leads it can cause connection issues.
```

---
## \#3 Posted by: Michaelj1 Posted at: 2018-10-16T16:30:55.905Z Reads: 88

```
I did adjust the failsafe using the button, and I have a fiberglass enclosure. It’s in a boosted board style layout, with the VESCs and receiver in on part and the battery and on/off switch in the other
```

---
## \#4 Posted by: Michaelj1 Posted at: 2018-10-16T16:32:29.568Z Reads: 81

```
I’ll post pictures of where it is located when I get home, it’s gonna be hard to see because everything is kinda tight
```

---
## \#5 Posted by: Andy87 Posted at: 2018-10-16T16:38:07.401Z Reads: 74

```
You said you switched the internals of the remote, did you also switch the receiver?
Maybe the antenna somehow broke inside the small wire.
```

---
## \#6 Posted by: Michaelj1 Posted at: 2018-10-16T16:39:33.723Z Reads: 72

```
Yeah I switch both. The antenna is fine last time I checked, my old receiver was sticking out of the case because I wanted to see if that would help and the antenna looked kinda frayed so that’s another reason why I swapped out everything. The antenna is in the enclosure now tho
```

---
## \#7 Posted by: Michaelj1 Posted at: 2018-10-16T17:16:13.035Z Reads: 69

```
I think it’s definitely interference related to the receiver, because on my old board it works pretty well for the most part with the antenna outside of the enclosure. But I’d like it inside if possible because I don’t want to damage the antenna wire again.
```

---
## \#8 Posted by: Michaelj1 Posted at: 2018-10-16T17:16:38.580Z Reads: 66

```
Whoops I meant with my old receiver
```

---
## \#9 Posted by: Silverline Posted at: 2018-10-16T18:15:58.077Z Reads: 60

```
Do you have any faults in the terminal ? I have issues as well, but I'm in doubt if it is my Gt2b or something else. I get over current faults....
```

---
## \#10 Posted by: Michaelj1 Posted at: 2018-10-16T18:16:59.555Z Reads: 60

```
No it’s definitely my gt2b, like I said, it behaves a specific way now when’s the remote disconnects, and it’s doing exactly that every time.
```

---
## \#11 Posted by: Silverline Posted at: 2018-10-16T18:17:52.398Z Reads: 57

```
But do you have any faults in the vesc ?
```

---
## \#12 Posted by: Michaelj1 Posted at: 2018-10-16T18:19:29.069Z Reads: 57

```
Oh faults? No I haven’t had any “abs_overcurrent” faults or anything like that. I initially thought thats what it was but people on a previous thread quickly proved that it wasn’t that.
```

---
## \#13 Posted by: Michaelj1 Posted at: 2018-10-17T00:39:21.220Z Reads: 56

```
![image|374x500](upload://xZdvE0SowyfcOsCDlYPA3mq26K3.jpeg) 
Had to unplug the sensor wires so I could flip it over lol, but like I said it’s pretty compact. I don’t have the reciever glued down. Where would be the best possible place to mount it?
```

---
## \#14 Posted by: Michaelj1 Posted at: 2018-10-17T00:41:07.369Z Reads: 54

```
![image|374x500](upload://2hAiC7DFvxiOg71BWQ2CTpp6UPn.jpeg)
As you can see the power wires come in up top. The antenna was going under it, is that close enough to cause interference?!?
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2018-10-17T01:28:57.770Z Reads: 50

```
have u tried to glue your connector in. this fixed some of my connection issues.
```

---
## \#16 Posted by: Michaelj1 Posted at: 2018-10-17T13:04:11.568Z Reads: 46

```
No I haven’t! I’ll give it a shot
```

---
## \#17 Posted by: Michaelj1 Posted at: 2018-10-17T13:09:14.377Z Reads: 45

```
I have the PWM glued into the VESC, but not the receiver. However like I said, it appears to be the remote losing connection, because of the way the failsafe comes on.
```

---
## \#18 Posted by: Silverline Posted at: 2018-10-17T19:43:15.853Z Reads: 41

```
But on the bench, if you full throttle the motors, and then turn off the remote. What happen then ?
```

---
## \#19 Posted by: Michaelj1 Posted at: 2018-10-17T20:01:25.985Z Reads: 42

```
That’s how I figured out the steering channel had a weird failsafe actually. It does what I said earlier, hesitates, then the master motor goes to coast and shortly after the slave motor does
```

---
## \#20 Posted by: Michaelj1 Posted at: 2018-10-18T02:08:46.231Z Reads: 38

```
Idk I might just ditch the gt2b. Had issues again today. Anyone know if the benchwheel remote is any good?
```

---
## \#21 Posted by: trancejunkiexxl Posted at: 2018-10-18T04:55:56.884Z Reads: 35

```
It's a solid remote. I use the winningv2 mostly these days due to its compactness. The benchwheel pcb is a little larger and doesn't fit well with my enclosure. The benchwheel has less dropouts for me In areas where I know signal becomes bad, price was determining factor for me. I always do route recon before full speed
```

---
## \#22 Posted by: dareno Posted at: 2018-10-18T11:31:22.340Z Reads: 32

```
Benchwheel is the bomb my friend.  The bomb.  Remotes are the most important part of any build imo.  They're like wives and girlfriends.  If there's no trust there's nothing.  I only trust 2 atm.  Maytech and benchwheel.
```

---
## \#23 Posted by: Andy87 Posted at: 2018-10-18T12:25:41.675Z Reads: 30

```
I though first you mean two women... :joy:
```

---
