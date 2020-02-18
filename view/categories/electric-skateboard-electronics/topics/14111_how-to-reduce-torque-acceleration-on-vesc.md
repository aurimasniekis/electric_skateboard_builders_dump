# How to reduce torque/acceleration on VESC?

### Replies: 28 Views: 5128

## \#1 Posted by: Eckles Posted at: 2016-12-03T08:24:59.614Z Reads: 360

```
After endless hours of reading this forum and tinkering I have finally managed to get my dual motor Eboard up and running. I have limited the top speed successfully (it was insane for a beginner) but I cannot get it to accelerate slower it just goes straight to top speed and I almost fall off everytime. I have played around with "Soft RPM Limit" settings which made a tiny bit of difference but it still takes off like a rocket. I guess theres other settings im not aware of that need to be adjusted. I wanted a 12s battery for the size and torque (big hills where I live) but this is ridiculous haha so any and all help would be most welcome as im out of ideas and cant find the same issue elsewhere in the forum.

My setup is 
x2 170KV Motors 
x2 VESC (Master and slave)
12s Lithum Ion Battery

VESC Settings 
<img src="/uploads/db1493/original/3X/1/8/180135d81d96e453d084fd16c042ae607eccf485.jpg" width="689" height="281">

<img src="/uploads/db1493/original/3X/1/8/180135d81d96e453d084fd16c042ae607eccf485.jpg" width="689" height="281">
```

---
## \#2 Posted by: Hillso Posted at: 2016-12-03T09:24:00.058Z Reads: 336

```
you can limit motor amperage, but maybe then it will be not enough powerful on the hills.
maybe you can try to adjust the throttle curve http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286
```

---
## \#3 Posted by: Eckles Posted at: 2016-12-03T09:32:08.117Z Reads: 335

```
ok, ill give it a go in a little while and post my results here.
Thanks!
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-12-03T11:25:48.816Z Reads: 317

```
Post Screenshots of your settings for the motor and we can help you. More or less there are 2 parameters to control that. Motor max controls the power especially at lower speed and battery max at the higher speed and overall the total power. 
But I recommend my modded firmware, because then you could define the throttle curve to make it soft at the lower throttle range and a beast at the higher throttle range.
```

---
## \#5 Posted by: ElskerShadow Posted at: 2016-12-03T11:27:32.886Z Reads: 299

```
Guess you could go to 40A motor max at the begining. That's what I did, each 3 days going up 10 A until you reached the top. Then you will be used to the punch.
```

---
## \#6 Posted by: Eckles Posted at: 2016-12-03T11:33:55.643Z Reads: 289

```
Yes I will, I just read the other thread to figure it out and Im very impressed with what youve done. I have spent the last 5 hours in some kind of BLDC dream :laughing: staring at my computer but I wont stop until my "Pegasus" is born :grin: Ill keep you guys updated
```

---
## \#7 Posted by: Eckles Posted at: 2016-12-03T13:12:02.076Z Reads: 265

```
Ok so... I got @Ackmaniac s modded BLDC tool up and running but now I need to flash the VESCs with his firmware because Im doing this with dual motors do I jus need to flash the "Master" motor or do both of them individually?
```

---
## \#8 Posted by: Ackmaniac Posted at: 2016-12-03T13:13:26.445Z Reads: 255

```
Definitely both.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-12-03T15:01:15.170Z Reads: 252

```
12s voltage = lots of torque and fast acceleration. 
You might be able to improve your situation with a better controller. 
So, what controller are you using?
```

---
## \#10 Posted by: Eckles Posted at: 2016-12-03T15:02:11.616Z Reads: 254

```
So ive managed to things up and running again with new firmware. After downloading the Modified BLDC tool 

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286

AND downloading the firmware flash file (.bin file) from the same place. I loaded up the Modded BLDC Tool and uploaded the new firmware like so..
 <img src="/uploads/db1493/original/3X/2/c/2cfea27314ec2a2921f0ef4e4a7ecdfe6e1f31a1.jpg" width="690" height="279">

 After getting the green message  "Firmware 2.52" I repeated the process on my slave VESC. I re'entered my values again and setup up the Master slave combo anew and there we have it almost done. Now all thats left is more tinkering with the throttle curve graph <img src="/uploads/db1493/original/3X/9/e/9e85ba179af1cdfab674a7580c3c66795d51af55.png" width="690" height="289">
until I can make this 12s accelerate in a more controlled manner.
Again if someone can help with graph values it will be appreciated .......... Im going to be making a small donation to @Ackmaniacs PayPal to thank him for his work (and help) and if anyone else benefits from this you can donate via the link in his thread!
```

---
## \#11 Posted by: Eckles Posted at: 2016-12-03T15:05:09.353Z Reads: 225

```
Im using the the Winning controller and the throttle is a bit short, I would go for a Nano X but the price with shipping (to Chile) didnt really make sense.
```

---
## \#12 Posted by: Ackmaniac Posted at: 2016-12-03T15:47:29.809Z Reads: 222

```
First of all i can recommend this setup for the throttle curve. For the brakes you have to find out yourself what would be nice. If you think they are to powerfull at the beginning then lower them a bit. If they are too weak then raise them a bit.

<img src="/uploads/db1493/original/3X/8/a/8a04d6c9c781e752a2bf258c36e3a57e9b2eff3d.png" width="690" height="484">

This setup reduces the power output to

12% at 25 % throttle instead of 25 %. So the power is more or less 50% compared to normal.

30% at 50 % throttle instead of 50 %. So the power is more or less 60% compared to normal.

60% at 75 % throttle instead of 75 %. So the power is more or less 80% compared to normal.

And at full throttle it is full power.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-12-03T16:11:25.475Z Reads: 201

```
I would recommend the Mini remote. 
It's a trigger 2.4 ghz and offers excellent control and dependability.
```

---
## \#14 Posted by: Eckles Posted at: 2016-12-03T16:19:54.393Z Reads: 194

```
Not sure what happened but after entering the new values my controller settings are all messed up I have also lost my dual motor config (its back to single motor) ???
```

---
## \#15 Posted by: Ackmaniac Posted at: 2016-12-03T16:23:44.391Z Reads: 189

```
Because you forgot to read the settings first before you update them. Maybe you pressed the read default accidentally.
```

---
## \#16 Posted by: Eckles Posted at: 2016-12-03T16:26:37.979Z Reads: 187

```
:open_mouth: haha.... will I need to reflash the firmware? because now I cannot get the controller to reconnect
```

---
## \#17 Posted by: Ackmaniac Posted at: 2016-12-03T16:28:06.532Z Reads: 185

```
Are you sure that you modify the settings for the master? Because if you are in the setup for the slave then you would not be able to see a ppm signal. 
If you connected the steering channel to the slave VESC to use the cruise control then you have to adjust the ppm parameters again for the slave vesc.
```

---
## \#18 Posted by: Eckles Posted at: 2016-12-03T16:34:09.902Z Reads: 186

```
no cruise control I was using "Current No Reverse With Brake" now after trying to rebind the controller I have two solid red lights (normal) but the program doesnt pick up my controller
 <img src="/uploads/db1493/original/3X/a/2/a2822305e63efef44988a2c420d36ea4e774964b.png" width="690" height="279">
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-12-03T16:35:21.507Z Reads: 185

```
Choose the right USB port on the upper right and press the connect button. You are not connected.
You can see the connection status at the lower right.

then go to the general tab in apllications and choose PPM. then write the settings and press the reboot button. After that connect again and adjust your setup for the ppm. When you write the settings then you don't need to reboot again.
```

---
## \#20 Posted by: Eckles Posted at: 2016-12-03T16:37:41.837Z Reads: 181

```
hahaha man Im sorry :blush::joy: i just panicked
```

---
## \#21 Posted by: Ackmaniac Posted at: 2016-12-03T16:41:40.081Z Reads: 177

```
And please post a screenshot of the motors BLDC tab to make sure that it looks ok.
Alos some more tips. Your board is quite powerful with the setup of batter my at 40 amps for a dual drive.

40 * 3,6 * 12 = 1728 watts
1728 watts * 2(Vescs) = 3456 watts total power output

in cruise control mode it gets a bit tricky to control that power. I recommend to try the "Watt no reverse with brake" control mode and set the max watt in the ppm setup to 1728 if you want to keep that power or maybe to 1200 watt if you want to lower it a bit but have more control.
```

---
## \#22 Posted by: Eckles Posted at: 2016-12-03T16:43:59.893Z Reads: 174

```
looks ok to me 
<img src="/uploads/db1493/original/3X/7/9/797f1f4edf59b8e75e798c29a94aee08c02e13c7.jpg" width="689" height="278">

However I need to recnfigure my Dual setup as only 1 motor runs now....and done! thanks for bearing with me
```

---
## \#23 Posted by: Ackmaniac Posted at: 2016-12-03T16:50:17.724Z Reads: 167

```
For the master you should set the checkboxes marked in red

<img src="/uploads/db1493/original/3X/e/3/e325a9ac9aeadecbd5dd9dadf031023ad674cabb.png" width="690" height="493">

And for the slave this so that they can communicate via the CAN bus

<img src="/uploads/db1493/original/3X/2/e/2e65b78c7bbe1f87452f0f517cb90b213d5fa969.png" width="690" height="499">
```

---
## \#24 Posted by: Namasaki Posted at: 2016-12-03T16:55:00.930Z Reads: 154

```
What version of BLDC tool is this ?
Where do you download it?
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-12-03T16:55:45.617Z Reads: 151

```
http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-and-individual-throttle-curve/12286
```

---
## \#26 Posted by: Eckles Posted at: 2016-12-03T17:06:41.868Z Reads: 144

```
yeah its all normal now but im going to have to lower values even more because this thing is POWERFUL however im pretty sure I can take it from here.....thanks man
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-12-03T17:12:08.880Z Reads: 141

```
Some more tips. If you want to stay with Current control then you can reduce the overall power by lowering the battery max value. In watt control you can do that by lowering the max watts in the ppm screen.
To lower the acceleration power at low speed you should lower the max motor value.
And don't forget to set the same values for master and slave.

I can recommend to use the Watt control mode because you can control the power also at higher speeds with the full throttle range. At least you should give it a try. 

Have fun
```

---
## \#28 Posted by: plasteroid Posted at: 2018-07-10T23:11:39.026Z Reads: 51

```
Thanks guys for this thread -  I'm setting up my Landsurfer and was just blown away by the torque on the first ride...  I've figured out how to make very very small adjustments on my thumb to accelerate and brake in a controlled way, but need to download the Ackmaniac build and do this.
```

---
