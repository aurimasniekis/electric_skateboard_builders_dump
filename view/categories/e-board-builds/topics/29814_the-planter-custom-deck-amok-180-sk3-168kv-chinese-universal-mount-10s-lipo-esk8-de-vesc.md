# The Planter &#124; Custom Deck &#124; Amok 180 &#124; SK3 168kv &#124; chinese universal mount &#124; 10S Lipo &#124; Esk8.de VESC

### Replies: 7 Views: 1048

## \#1 Posted by: Der6FingerJo Posted at: 2017-08-05T20:43:55.590Z Reads: 161

```
Hello everyone! 
My name is Tom and this is a showoff for my recently completed first electric longboard. 

I can only estimate the total cost to be around 700€ to 800€ with around 50 to 60 hours of work put into it.

First a pic of the finished Board:
<img src="/uploads/db1493/original/3X/c/b/cbfd54dad86f81693ec94d05335229fd8c0407b0.jpeg" width="281" height="500">

The deck is made out of 6 sheets of 3mm plywood glued together and crudely sawed out. (need to work on my woodworking skills :D)

Trucks are Amok Downhill 180mm (i believe it´s a kind of cheap brand? idk works for me though) with 12mm raisers and the wheels are 97mm Flywheel Clones called Blank Pro.

**The Drivetrain**

I use the Turnigy SK3 6374 168kv motor. Originally i wanted to go for an Alien 6374 with 10mm shaft and 130kv but that wasn´t in stock.
The SK3 already makes a rattling noises, i hate HK.
It´s powered by a Esk8.de VESC i bought right before they announced their Esk8 Controller. Man i would have liked to upgrade to that. Btw. the 3-phase connector is called MT-60.

On the SK3 sits a esk8.de 15mm pulley with 12 teeth, connected to a 48 teeth pulley on the wheel with a 325mm belt. A bit too long, 305mm would be better.

It was a lot of work to fit the wheel pulley and i was very proud that it runs that smooth. Also i fucked up mid way, that´s why it looks so janky.
https://youtu.be/_5yHybsXuuI

The threaded rods with locknuts hold everything together very well.

I mounted the motor using [this](https://www.banggood.com/Electric-Longboard-Skateboard-Motor-Mount-For-5065-5055-6374-6364-Motor-p-1157722.html?rmmds=search). Don't really recommend it as it's really hard to work with.

**The Remote**

First an foremost, credit to RollingGecko. I didn´t really copy his code but it helped me a lot to understand how to communicate with the VESC. Without his library this wouldn't have been possible.

Here´s the finished remote: (yeah someday i will make it look clean 
 :smiley:) 
<img src="/uploads/db1493/original/3X/e/e/eebcb54712df37cf87b72b5984998d1e758ba24d.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/1/e1bab72c366216b27d8a78ecebf229af4fac6abc.jpg" width="374" height="500">

So i bought a knock-off nunchuck to start experimenting, but ended up switchting the potentiometer and buttons to the original nintendo ones because the knock off's were plain crap. Inside is an Arduino Pro Mini, a HC-05 Bluetooth Module, a 1 inch OLED Screen, 2 mylipo 1s 205mah Lipos in Parallel, a 1S Lipo Charger and a Polulu 5V step. Sounds like alot but perfectly fit's in there. <img src="/uploads/db1493/original/3X/0/5/053551e48b75fcbd31f5a63e00859752f8859ccd.jpeg" width="281" height="500">

For turning it on an off i used a pair of dip switches because space reasons and a jst to connect  to 5V for charging. Batterys should last around 5 to 6 hours, 50ish mA draw.

I wrote the code myself, essentially it transmits x and y of the potentiometer as well as the buttons to the receiver and receives Voltage, Current, Speed and Capacity from the Board. Current and Capacity aren't working as of yet because i made a mistake and pulling that thing apart for programming is a pain in the butt.

Failsafe is handled by the Receiver, basically a light brake when something happens.

**The Box**

Most people i showed the board to commented on how clean it looks with the box. But there is a dark truth behind it.

It only cost 7€ and is a saucer you put beneath your planters in the garden or something. It´s called "elho Barcelona" in case someone is interested.

Inside is the VESC, an Arduino Mega with the other HC05 Bluetooth Module and 10 Lipo Cells split up in two 5S packs for charging. And a XT90 Anti Spark loop to turn it on and off.

Here it is ready to go, still a cable mess but i didn't know how long to make the Lipo leads, probably going to shorten them sometime.
<img src="/uploads/db1493/original/3X/8/a/8ac35eea38278cf9ab5b9a301531e97a318c4705.jpg" width="374" height="500">

**The Batteries**

I had 2x 4S 5000mAh and 1X 3S 5000mAh 20C from Zippy (Hobbyking) lying around. Sooooooo, very careful soldering outside was needed.
<img src="/uploads/db1493/original/3X/5/a/5a1ada770870519d3e5f77989ea8741526b51a38.jpeg" width="281" height="500">

I recommend using a very strong soldering iron with aluminum based solder to prepare the pads on the individual cells and then continue using regular solder on the wires.

In the end i had 2 (physically) flat 5S packs and i was very glad that the inner resistance didn't go up in the process.

<img src="/uploads/db1493/original/3X/f/5/f52c50d8ea1f0220622c641a6dbf674099b07228.jpg" width="374" height="500">

**The Result**

It's amazing. I don't have much experience in skating so i choose a high gearing ratio to have more power and less top speed, also because i live in a hilly area, and it plows my 105kg ass uphill no problem. Still didn't dare to go full throttle. (only cruise at 15 to 20 kmh/h)
So far i rode it for two charges in my neighbourhood and put around 25km on it. Range should be at 15km's and top speed right around 25km/h. Totally in love with this hobby now.

I hope i wrote all of this ok, not a native english speaker and i'm happy to answer any questions you guys may have!
```

---
## \#2 Posted by: jmasta Posted at: 2017-08-06T01:59:29.472Z Reads: 109

```
Well done!!  You call it cheapo, but that's a pretty clean build!  I especially like the remote
```

---
## \#3 Posted by: Ulfberht Posted at: 2017-08-06T04:07:08.614Z Reads: 102

```
@Der6FingerJo 
I want to know more about how to build that remote!! Awesome job! I like the way you converted those Lipos into flat packs...
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-08-06T09:24:08.355Z Reads: 89

```
Well i don't want to accept how expensive it got but in the end it was totally worth it :smiley:
```

---
## \#5 Posted by: Okami Posted at: 2017-08-06T09:33:47.955Z Reads: 85

```
Nice build. I see you have implemented a lot of ideas gathered on the forum.. or who knows maybe u came up with them on your own.

The older remote does look really nice, the same as flat lipo pack and planter tray enclosure ;)
```

---
## \#6 Posted by: Der6FingerJo Posted at: 2017-08-06T09:35:10.620Z Reads: 78

```
Building the remote was relatively straight forward - cutting out all unnecesary supports in the nunchuck and fitting stuff in. Just use a original nintendo nunchuck. The potis are directly connected to analog input pins of  the arduino and the buttons are connected using the pro minis internal pullup resistors. The Oled is on A4 and A5 as these are the minis i2c pins and the power goes through the polulu for stable 5V. The Receiver is just the Mega connected tu UART of the VESC and handles PWM generation and all things failsafe.

As far as code goes, i'd like to share it if there is any interest but i wouldn't be comfortable with people actually using it since i am in no way qualified in programming to release it as something reliable.
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2017-08-06T09:38:00.893Z Reads: 75

```
Thanks, i gathered ideas from all over the net. 
Everything started with a video from GreatScott on YouTube and snowballed into more and more features. The forum was definitely a huge inspiration for drivetrain and remote design as well as using the VESC in the first place. Joop Brokkings Longboard project definitely helped a lot with the code, too.
```

---
