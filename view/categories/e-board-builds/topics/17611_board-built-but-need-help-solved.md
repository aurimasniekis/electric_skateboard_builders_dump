# Board Built but Need Help -SOLVED

### Replies: 12 Views: 1010

## \#1 Posted by: dylantrygg Posted at: 2017-02-12T22:21:25.351Z Reads: 70

```
<img src="/uploads/db1493/original/3X/b/8/b8ea2053cb8639983ab3f56b2035c0983c6c6c53.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/c/6c2a392b242cfa7990be718d9e7763c3ba14d2b0.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/d/ad1a8c45c083341ee0a0cba94ed9a9ff77ed2d1e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/b/c/bc42104b1bf6368ab2224f6f958913f6a9144fac.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/c/7/c72259b248cb187bdf34b7beac61e65555d974bd.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/b/abd66b854dbabb457e3379bb7bcf6ff00e280a32.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/0/0057e7d89a4f837548cdcdab2d2608cbd0934f93.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/c/0c0d73e3cd28a36f2003ae68ac4ef21974b85f24.jpg" width="666" height="500">
-VESC-X
-Enertion 190kv Motor
-Traxxas TQi receiver/transmitter
-2 * 4s 5000mah 25c lipo

This christmas I decided to build my own electric skateboard even though it may cost me a little more than a prebuilt version. I love my build so far but I am having a few issues that I would love to get worked out. By the way, I know some of this build is a bit redneck but I was looking for short term solution. Sorry if this gets a little long, I'm just trying to explain as much as possible. 

I started out by buying the VESCX and the larger enertion motor. All my parts arrived right on christmas time except for the vescx. I decided to look into a replacement esc from a hobby store nearby so I bought a castle creations helicopter esc. This worked power wise, but the customization was terrible with castle link and it calibrated with my remote weird because it was a helicopter esc.

I tried to cancel my vescx order but they ended up sending it out anyways. I'm glad they did because I would very much recommend the vescx, and it is perfect for me.  The problem I am encountering is with power/torque. When I fully charge my two 4s batteries (so 8s in series) the board runs perfect and has great torque/speed. But after the batteries reach 95% capacity, the board loses torque and top speed. It's still rideable but very slow and takes a while to speed up. 

I'm guessing I have to get two larger batteries which will probably be what i'll end up doing. If anyone has any other ideas, that'd be awesome. 

(I'm also confused because I had an old remote from an RC car I used to race, so I decided to use that for the time being before I get another receiver. Not sure if anyone knows much about it but its a Traxxas TQi. When I put the pins into any of the channels in the receiever, it still only operates the motor from the steering input. Channel two is supposed to be the throttle trigger. Very confused.)

Any help is appreciated,
Dylan
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-12T22:27:49.655Z Reads: 57

```
Please screen shot and post your vesc settings.
```

---
## \#3 Posted by: dylantrygg Posted at: 2017-02-12T22:30:55.699Z Reads: 55

```
<img src="/uploads/db1493/original/3X/a/a/aa70acc1ec58cae90343352b30dfeb7a71728cc9.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/e/2/e2886547a1199a6a7d14df3c697c883588745b60.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/e/1/e1a6c94a6ed8056e51bee89ffb876bb6456a2fad.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/5/b57cbb814c97d245023774f40a546caca6e136d2.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/4/d41281de2fa144b5f15d64d6128ab117dce34aba.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/e/f/efafe86c8e0a9dd19920d5351f02f1dade9b9e11.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/4/4450f52142b72c11ba9087ab472e9cc45a3c9979.JPG" width="666" height="500">
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-12T22:44:32.598Z Reads: 45

```
Motor Tab:
Set your Battery cutoff start to 28.8 and your cutoff end to 27.2.
Then your board will run until the battery is empty.

PPM Tab:
you run a single drive so disable "Multiple ESCs over can"
Connect the VESC to channel 2 on the receiver and adjust your PPM pulsewith signals. (Or use my firmware mod which makes that easier.)
Read and watch here how to do it http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244?source_topic_id=17556

General Tab:
you run a single drive so disable "Send status over can"
```

---
## \#5 Posted by: dylantrygg Posted at: 2017-02-12T22:47:33.949Z Reads: 42

```
Alright I will change those. Probably a stupid question, but when you say running the battery dead, you mean running it to the safe dead level (or discharging too much) so you're not hurting the battery correct?
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-12T22:51:03.242Z Reads: 45

```
3.6V (8S * 3.6V = 28.8V) a cell for a lipo is safe as cutoff strat and 3.4V a cell as cutoff end for a lipo is safe. 
If you wnat a bit more you might alos can go to 3.5V as start and 3.3 as end.
But first i would try the settings i suggested and then measure each cell when they are empty.
if they vary already a lot then i wouldn't go lower. If they still be balanced (each cell has nearly the same voltage) then you could go a bit lower. Mine start to drift heavily below 3.4.

For a LiIon cell i recommend to use 3.0V as cutoff start and 2.8V as cutoff end a cell.
```

---
## \#7 Posted by: dylantrygg Posted at: 2017-02-12T22:52:30.186Z Reads: 43

```
Thank you so much for your help, I'll go change those values and give it a try. I'll let you know what happens!

Dylan
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-02-12T22:53:40.306Z Reads: 39

```
And once you got used to the power and feel safe then you can raise your power. You could easily go higher, but for the beginning you will be fine.
Later you can go to motor max 80 and battery max 60 for example.
```

---
## \#9 Posted by: dylantrygg Posted at: 2017-02-12T22:59:07.710Z Reads: 38

```
Okay. I've tried changing the power value before (up to 70) and I would feel no difference. Is that because I didn't change the battery max in accordance to the motor max?
```

---
## \#10 Posted by: Sander Posted at: 2017-02-12T23:10:51.881Z Reads: 39

```
[quote="dylantrygg, post:9, topic:17611"]
I've tried changing the power value before (up to 70) and I would feel no difference
[/quote]

Maybe you feel no difference because in the PPM Tab you limit the PID max EPRM to 15000?
```

---
## \#11 Posted by: dylantrygg Posted at: 2017-02-12T23:21:44.100Z Reads: 38

```
Might be true. I just edited all the values that @Ackmaniac told me to and it feels like a whole new board. I could put wings on it and fly lol. Seems like all my problems are solved. Thank you guys for all the help!

Dylan
```

---
## \#12 Posted by: Blasto Posted at: 2017-02-12T23:34:49.881Z Reads: 36

```
you should post a build thread, your build is simple and effective. A lot of people will be interested in it.
```

---
