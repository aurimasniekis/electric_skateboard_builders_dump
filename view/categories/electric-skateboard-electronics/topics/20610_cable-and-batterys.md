# Cable and batterys

### Replies: 5 Views: 549

## \#1 Posted by: SanderG Posted at: 2017-04-08T14:39:41.852Z Reads: 94

```
Hi, so im building my board for the second time this time with emprovements, i need some advice on cabeling, i have 2 3s 5000mah 40C lipos. Im gonna wire them in series to get the 6s. I 3d rinted 2 cases for my board 1 for the esc and 1 for the batterys but i got this cable to go from 1 case to the other (1 case by 1 truck the other on the other side. it is 4mm2 is this good?

 <img src="/uploads/db1493/original/3X/d/6/d6c1309d1ab70a131dcde5ec0a03f45a020cb70a.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/8/28dc772a6cf1959d7f72142afc683d0b2c993aec.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/9/89fab3352860c5a6c5fd1526a15828666b79033b.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/c/bcc99db463516b38439a19d8b8181d92c7d42690.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/b/4b472141758a7c5f5734b0258c95e99b995187d1.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/d/9d71511f4bea58ebc9a2d369806198eb327e78c4.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/1/e/1e79ed4e65694d8210c741dcb6adb529a5676f73.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/9/e/9eb846453432ff84d74beda2126166237c692223.JPG" width="375" height="500">
```

---
## \#2 Posted by: jmasta Posted at: 2017-04-08T17:11:58.851Z Reads: 63

```
[quote="SanderG, post:1, topic:20610, full:true"]<img src="/uploads/db1493/original/3X/2/8/28dc772a6cf1959d7f72142afc683d0b2c993aec.JPG" width="666" height="500">
[/quote]

I would remove the black ground wire in the middle connected to pin 4. What you have works perfectly if you hook up the batteries correctly. However if you wire the XT-60s in series as 1+2, and then happen to hook up the balance leads as 2+1, you will short out a battery.  Removing one of the wires on pin4 prevents this problem. Then if it's hooked up incorrectly, the only thing that happens is your cell monitor won't turn on.  Much safer
```

---
## \#3 Posted by: SanderG Posted at: 2017-04-08T18:52:30.194Z Reads: 46

```
hi, but then it will not read out all 6 cells on my lipo alarm?
```

---
## \#4 Posted by: jmasta Posted at: 2017-04-08T20:34:17.084Z Reads: 38

```
You have them wired in series twice. Once with the 10AWG main power leads. And a second time with the ~22AWG balance leads. This redundancy does nothing for you but expose a potential risk for a nice fireworks display
```

---
## \#5 Posted by: SanderG Posted at: 2017-04-08T20:45:38.706Z Reads: 35

```
So i need to cut 1 wire? And is the 4mm2 wire good?
```

---
