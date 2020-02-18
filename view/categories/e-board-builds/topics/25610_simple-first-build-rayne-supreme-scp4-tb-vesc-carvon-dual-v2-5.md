# Simple First Build &#124; Rayne Supreme &#124; SCP4 &#124; TB VESC &#124; CarvOn Dual V2.5

### Replies: 4 Views: 947

## \#1 Posted by: Flying Posted at: 2017-06-18T04:27:09.988Z Reads: 143

```
Being an owner of a Yuneec E-Go for 2 years, I knew exactly what I wanted: same long range as the E-Go, same modular approach for easy repair by me as the E-Go, and something much faster. DIY seemed to be the only choice. I called this DIY Simple because using hub motors made the assembly super easy.

The only stiff deck that I could find with a kicktail back in January was a 42.5” Rayne Supreme. It had deep concave and it was just big enough for the Enertion Space Cell Pro 4 (10S4P) Enclosure.
<img src="/uploads/db1493/original/3X/3/9/3939b39f3d59ac43a28872215518265df493fc4e.jpg" width="690" height="447">
<img src="/uploads/db1493/original/3X/c/f/cf692f86731860bc2075ec2ffae33130386fb789.jpg" width="690" height="404">
<img src="/uploads/db1493/original/3X/c/3/c300b054568906a9a6b08fd9062d2eba8229d24f.jpg" width="690" height="441">

I put a handle to the kicktail for easy dragging (and possibly as a footstop too)
<img src="/uploads/db1493/original/3X/9/7/9736cbb9dd6ca9ccf80abc7f1f198e6ef9d40f0f.jpg" width="690" height="457">

And drilled two more holes for mounting my Action Cam. Rubber bands are vital to keep the cam in position. I broke several joints before caming up with this rubber band solution. 
<img src="/uploads/db1493/original/3X/d/6/d6648e2f82615859e82213e0c70f269998c13d66.jpg" width="690" height="471">

I trimmed two inch off one kicktail to make a nose for dragging this heavy board. I didn't check how heavy it was but it was a lot more heavy than my E-Go.
<img src="/uploads/db1493/original/3X/1/1/118a462d41ff452e9b3cc22369d98fe9924075b7.jpg" width="690" height="462">

This was my simple custom grip tape, 11x45” from Restless. It's only a few dollars more expensive than standard grip tapes. 
<img src="/uploads/db1493/original/3X/b/3/b3763ad6d49e7ca145e6fd7061c15db06208da9a.jpg" width="690" height="368">

I made a XT60 to Twin XT90 power adaptor cable to match those XT90 on the VESC's from ToqueBoard.
<img src="/uploads/db1493/original/3X/4/a/4a61346579b5d221d544489f1bab8d4ca9c28bb3.jpg" width="690" height="464">

The CarvOn Dual V2.5 hub motors finally arrived in May, after a long wait of 3 months. 97mm wheels! Great for the kind of rough pavements that we have. I changed the bullet connectors to 5.5mm to match those on the VESC's.
<img src="/uploads/db1493/original/3X/8/8/881924f1a9d3eba7f13cd597293377388a1c8f04.jpg" width="690" height="442">

It was a challenge for a newbie like me to fit everything in the battery enclosure. I had two Micro USB cables laying around and I thought I could install them permanently to the enclosure. Unfortunately, VESC uses Mini USB connectors. Sugru was later used to seal the holes for the motor cables.
<img src="/uploads/db1493/original/3X/4/0/40fb25ddc81e00217b9f633ad25914a6c421b553.jpg" width="690" height="482">

The CAN Bus connector extended a few mm above the enclosure. Fortunately, the deep deck concave accommodated it. 
<img src="/uploads/db1493/original/3X/7/f/7fed008756aae69759fc60ab966651883834925c.jpg" width="690" height="450">

I heard that the Mini Remote Controller was more reliable but I bought the Nano too from TorqueBoard just to be qualified for free shipping. The Mini was put to use first as it was supposed to be more fail-safe. It's a bit bigger than the E-Go Remote Controller which I liked a lot. 
<img src="/uploads/db1493/original/3X/1/d/1d64082c5cf9d950f91a275fa595dd9f209f191c.jpg" width="682" height="500">

It seemed that there was no official location to download the BLDC Tool. I found a link in one of the posts here and it turned out to be a current version that fitted the VESC hardware and firmware. I changed only a handful of parameters. None related to ERPM was changed as I had a limited understanding of them. BLDC mode was used so that I could experience the full torque of the motors. (FOC mode that I tried 3 weeks later or yesterday was somehow not successful. My question would be posted at the end.) 

These are the screen captures:  
<img src="/uploads/db1493/original/3X/e/d/ed7cf294fcdcfb8f65fe43b991c3257c8b8f3439.jpg" width="690" height="408">
<img src="/uploads/db1493/original/3X/1/d/1dee418dbf9e4473a7455a9c314e5e7ad2072579.jpg" width="690" height="407">
<img src="/uploads/db1493/original/3X/d/a/da6ee1566ec652f5f16f6cf7148a7198a1ed79c2.jpg" width="690" height="406">
<img src="/uploads/db1493/original/3X/d/a/dae3a7aad7f3f58c245ae94a1896c39025a1f81c.jpg" width="690" height="408">
<img src="/uploads/db1493/original/3X/1/4/14cd525bb2b8455cffbf8537661a6efcd6a3691d.jpg" width="690" height="408">

The whole process of using the BLDC Tool was simple and quick even for a newbie like me. And then I was shocked! The motors ran wild after I turned the remote off. It turned out that it was because I skipped the step of binding the remote with the receiver. 

It was time to bolt the battery onto the deck. A lot of padding was needed to take care of the deep deck concave. 
<img src="/uploads/db1493/original/3X/a/3/a31dc6af1b6a8d4004e5127a79437cbd6cbbd4d1.jpg" width="690" height="414">
<img src="/uploads/db1493/original/3X/f/c/fcfa8770dfc165b47f4551f92cd4079063fb1a90.jpg" width="690" height="418">

It's time for a test ride outside.
<img src="/uploads/db1493/original/3X/8/9/89bc0beb45cf12fd1cbeae981e4d3c0cdecbf4f7.jpg" width="690" height="495">

Comparing it to my E-Go (ported to a Sector 8 deck):
<img src="/uploads/db1493/original/3X/9/f/9fb3f92404ca489ec9acee16cbcdd7ebce48ac1b.jpg" width="690" height="480">

I was pleasantly surprised that the ride with these dual hub motors was very comfortable, more than my E-Go. Noise level was lower than that of my single drive E-Go, and that the torque was well, so strong. It was a beast to my skill level! I tried hard to remember that the operation of the Mini Remote was exactly the opposite of my E-Go Remote. Things went well for 10 minutes until I needed to stop quickly near a car park exit. My muscle memory took over and did what I normally do with my E-Go Remote: pulling back the trigger quickly for braking. Fortunately, there was no car coming out. 

A few days later, I switched to the Nano Remote and did a long trip to see how fast I could possibly go at my skill level. 37km/h was achieved. Anything faster got me wobbles. The battery started at 41.7V. After roughly 20km and 100 minutes, it dropped to 37.1V. 

I made some changes with Sugru after the ride. The Nano Remote: much more easy  now to change from pushing to pulling and vice versa. 
<img src="/uploads/db1493/original/3X/7/a/7ac0a433071c48470829474b54290743aec71923.jpg" width="690" height="426">

The Power Switch: now less prone to changes when carrying. 
<img src="/uploads/db1493/original/3X/7/f/7fd6d95d988488ba7d4cbb381ce97127d5ddf327.jpg" width="690" height="499">

The Hub Motors: now less likely to cut into you with its sharp edges in an accident. As one can see, the Sugru stayed on securely even after sustaining some abuses. Also can be seen from the photo, the wheels are very soft. It's less than 100km. My E-Go wheels showed something similar only after a few hundred km. 
<img src="/uploads/db1493/original/3X/8/4/848ace553640fe4247d4af8085223500c81a1cf4.jpg" width="690" height="471">

A day or two later, I tightened my trucks and tried once again to see how fast I could go. I just could not believe it: 55km/h! I thought wind was on my back or something to make this possible. From the graph, it took 40s to get to 55km/h. My next target was to achieve maximum speed in just a few seconds. (I guess I am around 150lb.) 
<img src="/uploads/db1493/original/3X/6/8/682b98c026d1ecefb8b5451345ce9653718c2fb1.jpg" width="690" height="391">

The wheelbase was 30”, too long for tight street corner turning and I wedged both trucks. I went out for a third long ride and I got wobbles again once I reached 37km/h. 
<img src="/uploads/db1493/original/3X/f/3/f3290265ea84b98fbc0be89859e67e202081132c.jpg" width="690" height="473">

And then it was raining almost every day till today. I took the time to work on my regular longboard, changing the wheels from 70mm to 80mm. (I ride my regular in rainy days.) There was a huge improvement in comfort and control!
<img src="/uploads/db1493/original/3X/a/2/a262caca3afc4b846387d57fac51cf7167feaf7c.jpg" width="690" height="469">
<img src="/uploads/db1493/original/3X/c/a/ca026667f698e058384fa8efbb177c379bc71a9c.jpg" width="690" height="395">

So far, the motors may get warm but not hot. The battery enclosure near the VESC never get warm or hot. 

Now the negatives. Firstly, motor cables coming apart quite easily.
<img src="/uploads/db1493/original/3X/a/c/ac7e93299ed1764db95fc02e33c5934caa3174e6.jpg" width="690" height="410">

I ordered some MT60 connectors and hopefully they would work well. Secondly, the wheels seemed to be very soft. It's been at most 100km only. I am a bit worried. The E-Go wheels looked much better than this even after one thousand km. (From the spec: CarvOn are 78A and E-Go are 83A. But I could be wrong on these numbers.)
<img src="/uploads/db1493/original/3X/9/3/93b3f3e1a52a5cd593746787a4551165d2b80cbf.jpg" width="684" height="500">

Lastly, I have some questions and need your advice.
Q1. I heard that there is a bug with Max Current Ramp Step and so I entered a value of 0.004.  According to TorqueBoard, my VESC is of v4.12 Hardware and v2.18 Firmware. Is this value of 0.004 OK? 

Q2. Mini Remote Controller – Is there a way to switch the acceleration with the braking, may be by switching a couple wires inside, so that it would act just like a thumb operated remote, i.e. forward for acceleration? 

Q3. The Nano has a throttle throw of only 5mm and the board would reach max speed after I push the throttle only 3mm forward. The last 2mm is useless. For braking, nothing would happen until I pull the trigger back a couple mm. I certainly can adapt to these but can such response curves be changed? (BTW, no disconnects so far.)

Q4. FOC – I tried FOC yesterday. Measuring Lambda were mostly not successful. I found that if I turned the wheel/motor a bit to a new position, measurement could become a success and returned me a value. I used such values, “Apply”, “Apply”, and then finally “Write Configuration”. It was just as loud as BLDC (except that the speed was just a tad slower to pick up)! I was really disappointed. What was I doing wrong? Also, I set the cutoff voltages to 12 and 10 according to the TorqueBoard video. Is this really necessary? 
<img src="/uploads/db1493/original/3X/9/f/9fa26bf5ed2babe8e79159ca771f9d1b92c8f841.jpg" width="690" height="409">

Q5. Space Cell Pro 4 Voltage Display – At the beginning it showed a percentage (and L10). After a few days, it showed only voltage, which I found more useful. And then a few days later, it showed only percentage again. I have no idea what triggered the changes. Is there a way for me to set the display to show voltage permanently? 

Q6. Finally, should I use it? Should I spray it on the motors, on the electronics, and on the battery cells? Does it really work? 
<img src="/uploads/db1493/original/3X/d/d/dd189261b2e0ba381fef6085741a6936face2520.jpg" width="540" height="500">

This is it. All comments are welcome!
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-18T19:23:25.698Z Reads: 83

```
Sweet first build man, glad its fun!
```

---
## \#3 Posted by: JLabs Posted at: 2017-06-18T19:32:23.056Z Reads: 82

```
Great build and documentation, congrats :tada:
```

---
## \#4 Posted by: Flying Posted at: 2017-06-20T03:28:44.641Z Reads: 70

```
Thank you both of you!

After watching some videos saying that FOC mode could be loud with bench tests but not with loaded rides, I changed the config to FOC mode once again. After assembling everything, I noticed that the battery display was showing L3 permanently. Nothing but L3, not even a percentage. This was really frustrating to say the least.

I watched this "Space Cell Pro screen fix" video again. I noticed that there were two differences. First, Enertion had already put a pad between the BMS and Display. Second, pressing the button did not change L3 to anything else. When the button was pressed, the display changed to L3 and voltage. Pressing the button again changed the display to L3 and percentage. Pressed again gave me L3 and voltage again. It was stuck at L3. However, since the voltage display was exactly what I wanted, I added a pad between the the BMS and Display next to the button and put everything back. 
<img src="/uploads/db1493/original/3X/3/0/304d03745eb2a32dae4e8ac71b87732261dd5b05.jpg" width="678" height="500">

Since it was getting dark and it rained again, I am not testing FOC today.
```

---
