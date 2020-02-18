# Motor Issue, possebly VESC?

### Replies: 11 Views: 187

## \#1 Posted by: Mathias03 Posted at: 2019-08-01T11:21:47.405Z Reads: 48

```
Hey guys! So I have a problem with my electric skateboard that I can't seem to figure out. The problem is pretty simple; the motor won't run! 
The problem started with a phase wire comming loose from the vesc joint (middle one), so i solderd it back on, and everything was all good. So i thook it for a spin, then when i jumped of a little sidewalk (15 cm max) the board stopped and would'nt run anymore. When i got  back home i opened the enclosure and found the middle phase wire half on and half off, so i soldered it back on again but still no response from the motor!

There is no red light on the vesc, i've checked for fault codes, the green light lights up when i give throttle and checked the wire connections (not opened the motor yet thought) and the motor does not spin or give any sounds what so ever. 

Any help would be much appriciated!

I am rocking a torqueboards 12s battery (old version), Enertion focboc (not dual) and a sk3 168kv motor. Havent posted a build tread yet :frowning:
```

---
## \#2 Posted by: Andy87 Posted at: 2019-08-01T13:06:19.660Z Reads: 43

```
did you do motor detection again?
did you diconnect only one phase or all 3 phases?
if you mixed them the old motor detection isnt valid anymore.
```

---
## \#4 Posted by: Mathias03 Posted at: 2019-08-04T13:57:42.105Z Reads: 30

```
Yes, I did try to run a motor detection. I dont remember what it said (could try agian if it is relevant) , but it didnt work. Oh yeah i disconnected all of the, but only one needed soldering.
```

---
## \#5 Posted by: JoelMatousek Posted at: 2019-08-04T20:31:26.112Z Reads: 29

```
Try updating firmware. That happened to me where I had a small problem and when I fixed it, nothing worked. Then I updated and it worked good as new
```

---
## \#6 Posted by: Mathias03 Posted at: 2019-08-04T21:11:27.123Z Reads: 27

```
Thanks! I’ll try that!
```

---
## \#7 Posted by: JoelMatousek Posted at: 2019-08-04T21:12:29.864Z Reads: 28

```
No problem! Just remember to do motor calibration after
```

---
## \#8 Posted by: Mathias03 Posted at: 2019-08-07T15:29:26.642Z Reads: 22

```
So I have now installed the NEW vesc tool and updated firmware. When It came to me running the motor calibration it failed (same as last time). I've not checked the phase wire connections directly on the motor yet, do you think it is worth checking?
Also is it alot of work?
```

---
## \#9 Posted by: JoelMatousek Posted at: 2019-08-07T18:01:57.895Z Reads: 20

```
I'm sorry Ive been at work, currently taking a break. Can you post a picture of the error you're getting? Also I doubt it's the motor, but you can still check the connections. Don't open the motor! That's a lot of work you don't need to do. If you touch any two leads that come out of the motor, the motor will stiffen. So hold two of the three leads together and see if it stiffens. If it doesn't, the motors bad, if it does then both of those leads have good connections. Then touch one of those two leads to the third lead and see if the motor gets stiff
```

---
## \#10 Posted by: JoelMatousek Posted at: 2019-08-07T18:03:35.991Z Reads: 19

```
If my instructions are difficult to follow, I can explain better after work in about 4 and a half hours
```

---
## \#11 Posted by: Mathias03 Posted at: 2019-08-09T20:18:48.631Z Reads: 13

```
Sorry been busy, yeah i dont really understand what you mean by stiffen? 
Also, i dont get any other error than «motor detection failed».
```

---
## \#12 Posted by: JoelMatousek Posted at: 2019-08-09T21:00:07.469Z Reads: 10

```
By stiffen I mean it gets hard to turn
```

---
