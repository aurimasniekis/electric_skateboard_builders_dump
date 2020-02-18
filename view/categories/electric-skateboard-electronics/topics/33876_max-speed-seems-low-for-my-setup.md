# Max speed seems low for my setup

### Replies: 19 Views: 937

## \#1 Posted by: Jdubb121212 Posted at: 2017-09-24T20:04:16.596Z Reads: 142

```
I have been riding my board for about 2 months now and love this thing however I am getting use to it and am basically full throttle everywhere I go, max speed is only 23mph (would like to be 27-30mph) calculator says I should be way faster so Im assuming I need to make some focbox adjustments (thinking about FOC mode but not sure how to setup safely) also my range seems mediocre for a 12s2p. Can you guys help me with my settings to get more juice/range/FOC setup out of this thing? 

Setup
Torqueboards 6374 190kv
focbox
Torqueboards nano remote
Torqueboards 12s2p
ebay 13t/36t pulleys 15mm belt
Torqueboards motor mount

Also will be adding another 6374 and upgrading battery to 12s4p in a couple months!<img src="/uploads/db1493/original/3X/3/8/38c5502ea2f39a90341515c4a462f0c3a359218c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/e/4eaf0659302ed01ab31f12f7d924acffd78b6dfb.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/c/3c118fbdf62a5a2f5b8e831bb0946ebe50805b05.png" width="690" height="365"><img src="/uploads/db1493/original/3X/b/0/b0180210d62c81eee1a0b46c22a90016fd581f92.png" width="690" height="365"><img src="/uploads/db1493/original/3X/9/5/95a6ba93fb22bcdf43b30209f3a9963e432fbb54.png" width="690" height="445"><img src="/uploads/db1493/original/3X/4/3/431f55087eab1088d7783a2dff3512f26d5d4403.png" width="690" height="363"><img src="/uploads/db1493/original/3X/0/2/02c8a69f0c81d51283fb6e986aa843ff0e63363e.png" width="690" height="357">
```

---
## \#2 Posted by: Silverline Posted at: 2017-09-24T20:08:06.753Z Reads: 130

```
your motor max, and batt. max, seems way to low, for a single motor setup.

All so your "Min ERPM" should be -60000 like your max ERPM, just to be shure.
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-09-24T20:11:22.254Z Reads: 129

```
What diameter are your wheels? Are you using lipo or li-ion? What C rating?
```

---
## \#4 Posted by: Jdubb121212 Posted at: 2017-09-24T20:46:17.330Z Reads: 121

```
What would you suggest for the motor and bat max? Got the Min ERPM set to -60000 now.
```

---
## \#5 Posted by: Jdubb121212 Posted at: 2017-09-24T20:49:32.651Z Reads: 120

```
Wheels are 90mm, li-ion, not sure what the c rating is.
```

---
## \#6 Posted by: Silverline Posted at: 2017-09-24T21:03:13.933Z Reads: 117

```
Depends on your specs of your battery. How many amps it can provide without overheating. But i would start trying with batt. Max at 40amp, and motor max 60amp.
```

---
## \#7 Posted by: MysticalDork Posted at: 2017-09-24T21:14:50.038Z Reads: 112

```
One limiting factor is that at full voltage, your setup would exceed 60k erpm, so the focbox will limit the maximum erpm to 60k. But you should still be getting better than 23mph. How tight is your belt?

I'd also double check your controller setup to make sure you've got full range there.
```

---
## \#8 Posted by: pat.speed Posted at: 2017-09-24T22:08:36.350Z Reads: 107

```
Yes it does seem slightly slow for that setup. In the calc it says you should hit 27mph before the Vesc limits the erpm. The only thing I can think of is if the battery can't supply enough amps to get to that speed
```

---
## \#9 Posted by: Namasaki Posted at: 2017-09-24T22:35:25.169Z Reads: 104

```
one issue I see is your gear ratio.

13/36

try 15/36 or 16/36

Also your motor max is low at 40a
Try raising your motor max to 60a or 80a
It would also help if you could raise battery max from 25a to 40a  but I dont know what your battery can handle.

Concerning speed calculators,
How can they possibly be accurate unless they factor in rider weight, wind resistance and riding conditions.
```

---
## \#10 Posted by: jmasta Posted at: 2017-09-25T01:38:58.886Z Reads: 101

```
Get a bigger motor pulley, like @Namasaki suggested

Your top speed really isn't too far off with what you'd expect from the simple calculator predictions

<img src="/uploads/db1493/original/3X/2/c/2cd5e602a688e18af52fdc47e666e8a69d2268f8.jpg" width="603" height="500">
```

---
## \#11 Posted by: Namasaki Posted at: 2017-09-25T01:53:18.414Z Reads: 97

```
One thing I don't like about that calculator is that it doesn't apply full charge voltage.
50.4v for 12s

50.4 x 190 = 9576 rpm
9576 x 7 = 67032 erpm (over limit for vesc4)

The other thing is how do you determine the efficiency.
If you weigh 120lbs or 220lbs.  How do you translate that into an accurate value of efficiency.
```

---
## \#12 Posted by: Colson003 Posted at: 2017-09-25T02:38:50.932Z Reads: 90

```
Looking on diyelectricakateboard.com your battery max should be 30a absolute max should be 80a and motor max should be 80a <img src="/uploads/db1493/original/3X/6/4/6451d870c9db477813996de272dc178c0d7f1c34.PNG" width="281" height="500"><img src="/uploads/db1493/original/3X/f/e/fe659ad5227b0b4750dde407bdd591a3d2c3106b.PNG" width="281" height="500">
```

---
## \#13 Posted by: Namasaki Posted at: 2017-09-25T02:42:45.908Z Reads: 81

```
@Jdubb121212 
Absolute max should NEVER be set lower than 130a
Absolute max is a last resort in case soft limit strategies fail.
You really don't want absolute max to be activated because it will cause a sudden loss of power that could throw the rider off the board.
http://vedder.se/2015/01/vesc-open-source-esc/

<img src="/uploads/db1493/original/3X/5/d/5dd1499a8c520acdb96e3138e351a8c1f6e36817.png" width="642" height="263">
```

---
## \#14 Posted by: Colson003 Posted at: 2017-09-25T03:02:52.230Z Reads: 78

```
So with those specs what should the battery max be set to? 30a? Or 80a? 
I also noticed you have the regen set to 10a which the battery normally charges at 2a or 4a, don't know if that makes a huge difference but I've set mine to 4a on my torqueboards battery.

I have the 6S4P battery from them and it has identical amp ratings, 30a continuous and 80a peak. I'm now questioning how I setup mine.
```

---
## \#15 Posted by: Namasaki Posted at: 2017-09-25T03:13:42.116Z Reads: 74

```
@Jdubb121212 
[quote="Colson003, post:14, topic:33876"] 
So with those specs what should the battery max be set to? 30a? Or 80a? 
I also noticed you have the regen set to 10a which the battery normally charges at 2a or 4a, don't know if that makes a huge difference but I've set mine to 4a on my torqueboards battery.
[/quote]


In order to determine correct battery min current, we would need to know what cells are used in the battery and what their maximum charge rate is. Multiply that by 2 because it's 2p
The bms is limited to 30a continuous and 80a peak so setting battery max to 30a would be the safest solution.
If the battery has a 30a fuse, you don't want to blow that fuse while your riding because a total shut down could cause a dangerous situation.
Motor max can go as high as 80a and more motor max will increase torque especially at low speeds.
Since the system is running 12s voltage and higher voltages yield more torque as well, I would recommend raising the motor max current 10a at a time and trying it out until desired torque is achieved.
```

---
## \#16 Posted by: Colson003 Posted at: 2017-09-25T03:50:23.968Z Reads: 69

```
Looking at the 12S2P specs it's made with Samsung 30Q cells which doing some research I found to have a 15a continuous discharge and a 1.5a standard charge rate and 4.0a max charge. 
15 x 2 = 30a continuous
1.5 x 2 = 3a battery min or 4.0 x 2 = 8a battery min <img src="/uploads/db1493/original/3X/1/3/13e8341a34a7e7e16ec4841e70bdb7e84af88412.PNG" width="690" height="388">
```

---
## \#17 Posted by: Jdubb121212 Posted at: 2017-09-25T05:02:37.460Z Reads: 64

```
Thanks for the help with this, just ordered a 16t pulley and will be making the adjustments to the focbox, as well as trying out FOC.
```

---
## \#18 Posted by: Namasaki Posted at: 2017-09-25T05:18:19.195Z Reads: 62

```
I would hold off on trying FOC. Especially if your trying to increase top speed.
Better to get everything sorted out in BLDC mode and then do a lot a research before trying to mess around with FOC.
```

---
## \#19 Posted by: Jdubb121212 Posted at: 2017-09-25T05:21:15.735Z Reads: 60

```
Yeah I think thats a good idea.
```

---
