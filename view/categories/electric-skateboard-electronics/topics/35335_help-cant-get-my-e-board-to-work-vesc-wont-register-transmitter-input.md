# HELP! can&rsquo;t get my e-board to work, vesc won&rsquo;t register transmitter input

### Replies: 18 Views: 719

## \#1 Posted by: Ruben0811 Posted at: 2017-10-11T21:04:35.198Z Reads: 68

```
hello people of this awsome community

i have bin working on my board for a few days now and i finally overcame a few obstacle's. But now I have a final problem that i can't solve myself. the problem is that can't get my transmitter to power the moter. only when I press the keys on my keyboard the moter spins up. I have watched a lot of video's on how to configure the ''app configuration'' tab.( i used to tutorial to configure my vesc https://www.youtube.com/watch?v=17CSl1iXYE8). but when i move the trigger of my transmitter the green bar won't move. im using a [my transmitter](http://Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System)
the red light on my receiver turn on when i turn on the transmitter( i think that means it is connected cause i did bind it)
if you have any tips i would love to hear them.
thanks for reading this 

kind regards Ruben<img src="/uploads/db1493/original/3X/a/9/a986a3dfb6a68592ec35f4b8893167181fbedf73.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/8/4/84323bf52bc39b2b6194a4f9a8ebdae393f3b48a.jpg" width="690" height="388">
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-10-11T22:31:30.564Z Reads: 55

```
Have you tried all the different channels on the receiver? The vesc may be reading the steering channel, for example.
```

---
## \#3 Posted by: Ruben0811 Posted at: 2017-10-12T08:12:52.208Z Reads: 47

```
i have tried al 3 div channels yes
```

---
## \#4 Posted by: L3chef Posted at: 2017-10-12T08:15:58.474Z Reads: 45

```
Post pics on your receiver. Sound like you got pwm wire in the wrong place.
```

---
## \#5 Posted by: Ruben0811 Posted at: 2017-10-12T08:19:48.550Z Reads: 42

```
<img src="/uploads/db1493/original/3X/8/f/8ffa390f55c1fe19c48b2e9826fde2981d8112eb.jpg" width="500" height="500">
i made this ghetto servo cable myself because i got the wrong cable with my Vesc. should work tho?
```

---
## \#6 Posted by: L3chef Posted at: 2017-10-12T09:18:39.651Z Reads: 36

```
Frick that's hard to see :smile: but I think the wires are in the wrong place
```

---
## \#7 Posted by: Ruben0811 Posted at: 2017-10-12T09:26:34.780Z Reads: 35

```
https://drive.google.com/file/d/0B2QS7dKKB64zdTAyREprX0VRYzQ/view?usp=sharing hope this vid wil help
```

---
## \#8 Posted by: L3chef Posted at: 2017-10-12T09:38:35.359Z Reads: 35

```
Can't view it on my phone.
Up to you if you want to try this. But heres how i connected my aps receiver. White signal. Red + and black is ground <img src="/uploads/db1493/original/3X/8/5/8593cfd386d06c1bbd99a6760160df96eb800650.jpg" width="375" height="500">
```

---
## \#9 Posted by: Ruben0811 Posted at: 2017-10-12T09:45:32.494Z Reads: 32

```
i have it the exact same way. only mine aren't colour coded
```

---
## \#10 Posted by: L3chef Posted at: 2017-10-12T09:58:20.670Z Reads: 32

```
I don't think you have :smile:  <img src="/uploads/db1493/original/2X/6/6524598ba6aa4294b4e1a9a1eb0ec70cfd928702.png" width="690" height="265">
```

---
## \#11 Posted by: pat.speed Posted at: 2017-10-12T10:51:12.442Z Reads: 32

```
According to @L3chef your signal wire is swapped with te gnd wire
```

---
## \#12 Posted by: L3chef Posted at: 2017-10-12T10:55:32.436Z Reads: 32

```
Yep
Ten char
```

---
## \#13 Posted by: L3chef Posted at: 2017-10-12T10:58:25.231Z Reads: 29

```
And also you are feeding it 3,3v. It needs ~5v
```

---
## \#14 Posted by: Ruben0811 Posted at: 2017-10-12T11:02:17.498Z Reads: 30

```
<img src="/uploads/db1493/original/3X/e/0/e04f0698bf08205fd83d34bd727954b0af8f01f4.jpg" width="500" height="500">
This is the way i connected it al the time. But how do u know the current input is 3.3 V. Elanf how do i change it to 5 V?
```

---
## \#15 Posted by: L3chef Posted at: 2017-10-12T13:06:55.771Z Reads: 25

```
Well that's wrong. Look on the receiver you can see  -, +, and the signal symbol(just under the 2,4 ghz at the pin side) Switch ground and signal and you should be ready to go
```

---
## \#16 Posted by: Ruben0811 Posted at: 2017-10-12T14:18:48.681Z Reads: 24

```
<img src="/uploads/db1493/original/3X/b/c/bcf6c6cac022a64d4d58b586091581f00590dfa4.jpg" width="500" height="500">
The servo wires i orderd  just arrived. This should be the correct way right?  P.s thanks for help i really apriciate it. Your the best
```

---
## \#17 Posted by: L3chef Posted at: 2017-10-12T14:32:40.331Z Reads: 25

```
No that is not correct. Just turn your receiver connector 180 degrees.. 
Zoom in on the receiver so you can see what I typed
<img src="/uploads/db1493/original/3X/9/9/996d58d7c38fa53c4cd37cf36bbcf2ae38912db2.jpg" width="500" height="500">
```

---
## \#18 Posted by: Ruben0811 Posted at: 2017-10-12T15:06:46.422Z Reads: 23

```
Lol im such a dummie. This is a really stupid mistake. I always tought that that the left simbol ( on the receiver)ground was. That where im wrong. I will try it the right way tgis time and i will let u know if it works. Thanks again 😁
```

---
