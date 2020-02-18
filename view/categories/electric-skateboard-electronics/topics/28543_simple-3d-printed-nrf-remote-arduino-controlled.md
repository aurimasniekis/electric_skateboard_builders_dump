# Simple 3D-printed NRF remote - Arduino controlled

### Replies: 2217 Views: 88429

## \#1 Posted by: solidgeek Posted at: 2017-07-25T00:14:46.497Z Reads: 2383

```
This summer I finished my second electric skateboard, and instead of using the usual Nunchuck remote I thought I would try to make my own. I am currently studying to become an electronics engineer, and recently bought a 3D-printer, so I thought it could be a fun summer project.

I have seen quite a lot of interesting remote builds on this forum, however many seems to me to be very complicated or an exaggeration with too many expensive components. I have always loved the simplicity of the Boosted Board remote, and therefor been trying to make something just like that - however powered by an Arduino.

This is the design I came up with :wink: :wink:  

<img src="/uploads/db1493/original/3X/9/d/9d5a0512ee2074855dc86ce3d8914af18764f550.jpg" width="690" height="359">

The remote consists of quite a few components, including an Arduino Nano, a NRF24 transmitter and a 3,7V 400mAh LiPo battery etc. You can find a list of all the components I used here:

https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit?usp=sharing.

The 3D-model is done and the STL-files can be found on my Thingiverse page in a few days - I have to make sure everything is fitting nicely before you guys waste perfectly good plastic :slight_smile: 

As you might see from the shopping list I use a linar Hall-effect sensor and two magnets to replace the more common potentiometer. The datasheet for SS495A says ”Ratiometric Linear sensors have a ratiometric output voltage, set by the supply voltage. It varies in proportion to the strength of the magnetic field”. By placing the sensor between two magnets (one north and one south) and moving the magnets over the sensor we get a nice throttle value.

<img src="/uploads/db1493/original/3X/c/1/c1a1e905e63e3b04ea91f5b1bdbf1b7a94f2e354.jpg" width="690" height="359">

 I have been using my second prototype for more than 20km now and it feels very stable, however it has it flaws. I am therefore currently building a new prototype (the third). IMAGES :smile:!! 

<img src="/uploads/db1493/original/3X/0/9/098b125636f94961a59c1956c71730c002770bc8.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/f/f/ff4e1b2856499119da5783951d10894bdea719d1.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/0/5/05acdbe9e905f498c09f390cc643a61e2b950533.jpg" width="690" height="388">

I would like to hear your thoughts and suggestions :slight_smile:!!  I will keep you guys posted with images and updates the next few days.
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-07-25T00:17:08.079Z Reads: 1967

```
That thing looks amazing!! Are you planning on selling or putting out a guide on how to build it?
```

---
## \#3 Posted by: JLabs Posted at: 2017-07-25T00:20:39.349Z Reads: 1939

```
Looks good, mad props!
```

---
## \#4 Posted by: solidgeek Posted at: 2017-07-25T00:34:01.239Z Reads: 1916

```
@GrecoMan most likely the last. I have been taking alot of pictures, so I could easily put a guide together if you like :slight_smile:

@JLabs Thanks! :wink:
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-07-25T01:21:41.641Z Reads: 1849

```
I would love it if you could put out a build guide
```

---
## \#6 Posted by: wafflejock Posted at: 2017-07-25T01:29:21.005Z Reads: 1790

```
Nice there was a recent post asking about good remotes posted my own similar incarnation there, should add yours to the list there for potential options (mine is still alpha quality at best, but been using it for over a year)
```

---
## \#7 Posted by: Cobber Posted at: 2017-07-25T01:45:19.464Z Reads: 1705

```
Dude! 
I like the alternative tech on the trigger :sunglasses:
```

---
## \#8 Posted by: High-roller Posted at: 2017-07-25T04:53:33.677Z Reads: 1672

```
Same here, it's about time we saw a remote design that can use both trigger and thumb configurations!
Would you consider doing a gt2b mod version of this?
```

---
## \#9 Posted by: DevoCut Posted at: 2017-07-25T05:09:28.916Z Reads: 1635

```
Really like the design, What printer are you using? your prints came out perfect!
```

---
## \#10 Posted by: baxter Posted at: 2017-07-25T10:57:47.945Z Reads: 1606

```
Looks great!  Would love to hear/see more about your design!
```

---
## \#11 Posted by: solidgeek Posted at: 2017-07-25T19:28:38.414Z Reads: 1685

```
First of all thanks for all the nice comments, I am very glad you like my work :slight_smile:! I am currently working on some schematics and finishing up the third prototype.

@GrecoMan I will make a guide for you guys as soon as I get to finish the newest version - final parts are 3D-printing at the moment ;-) !

@wafflejock Yeah I have just checked out your design! I like the simplicity of your remote, I could fit a whole lot of electronics in that beast! My design is much more compact, with no or little room for extra electronics :wink:

@Cobber @High-roller Glad you like! I will be posting a video of the trigger and throttle mechanism in the bottom of this post! I am afraid I don't own a gt2b remote, and I am not sure if the electronics will fit - so probably not! And doesn't there already exist a ton of great enclosures for gt2b remotes?

@DevoCut Thanks! I am using the european version of the CR-10 called Afinibot A31. It's basicly the same printer, however with a few improvements.

@baxter Thanks! I will keep you updated on the progress :slight_smile:

Here is a video and some pictures:

https://www.youtube.com/watch?v=yeIccUWoDQA

<img src="/uploads/db1493/original/3X/c/1/c1cb8cd9e07aa41d7176a106fff114450992d4e0.jpg" width="375" height="500"> 

<img src="/uploads/db1493/original/3X/e/e/eef4b07967a943713604e8e9b20b069268c0b0da.jpg" width="690" height="388">
```

---
## \#12 Posted by: markyoe Posted at: 2017-07-25T19:31:12.194Z Reads: 1515

```
Dude that is amazing! I'd totally print and build one if you have the time to come out with a guide. Is that an LCD to show battery level?
```

---
## \#13 Posted by: solidgeek Posted at: 2017-07-25T19:39:21.887Z Reads: 1505

```
Thanks :smile: Would be awesome to see it being made and used by you guys! It is a itzy bitzy OLED LCD (128x32px) to show battery level, signal strenght etc. Could be programmed to show basicly everything - even VESC data by using the UART library made by RollingGecko (https://github.com/RollingGecko/VescUartControl).
```

---
## \#14 Posted by: wafflejock Posted at: 2017-07-25T19:46:43.917Z Reads: 1492

```
Yeah beautifully done on your design and thread here definitely inspiring me to want to redo mine but need to put it on the backlog pile of things to do for now, maybe I'll get around to it in a few weeks.  I considered doing the linear hall sensor idea too so cool to see someone who actually implemented it.  I went with the potentiometer and trigger route because it's basically what I had previously and just took the same concept for my own controller.

Definitely big but I was putting a mess of wires and big boost converter and nonsense in there but have since figured out how to get it down to a small stack of PCBs, those NRF modules you're using are super compact though that's awesome.  I'm pretty sure you don't need the boost circuit if you get the 8MHz pro mini boards they run on 3.3V so they're pretty much good using the LiPo power directly into the RAW pin and getting regulated down to 3.3V for most of the life of the LiPo (speed grades section in the ATMEGA328P shows it at 10MHz with less voltage so should be good) in my own testing has been pretty stable without the boost.  Only issue I have is when the battery is really low in the remote it doesn't read the top end in the ADC as high as it should so the throttle signal is sending lower/sluggish speed but kind of good because lets me know I need to juice up the remote.  Awesome thing is all these parts use almost no power either way so the battery lasts forever.
```

---
## \#15 Posted by: solidgeek Posted at: 2017-07-25T19:59:33.321Z Reads: 1419

```
Thanks I really appreciate your kind words :slight_smile:! The potentiometer is a great solution, however I couldn't find a way to make it small enough to fit in my remote. Also the Hall sensor setup is quite solid, because there are no mechanical wear on the throttle. I have been thinking of using the 3.3V Arduino, however the Hall Sensor makes this impossible as it requires at least 4,5V to operate optimal. 

There are probably some Hall Sensors of the same type that works at 3.3V however I had already ordered mine :) And as you mention yourself, when the battery voltage drops below 3.3V the reference voltage will drop, so will need some kind of undervoltage circuit that prevents that - the easy solution a Boost converter :stuck_out_tongue: ! They come in very small sizes and cost no more than 5$.
```

---
## \#16 Posted by: wafflejock Posted at: 2017-07-25T20:02:55.758Z Reads: 1423

```
Gotcha yeah had the afterthought that some of the other components here might need higher voltage.  Regarding the cut off think it can probably be done with a zener diode too but I'm not entirely sure so far I haven't really had a problem since most of the time the voltage level is far above what's needed anyhow (4.2V-3.6V is where it's at a majority of the charge).  Yeah the boost converter I had was variable and big will have to check out the ones you used here too looks super compact, I don't think I need it but good to be aware of what's out there for future stuff anyhow.
```

---
## \#17 Posted by: JLabs Posted at: 2017-07-25T20:07:13.014Z Reads: 1441

```
I would check out the WeMos TP5410 board. Its a lipo protection, charger, and boost converter all in one. 

https://youtu.be/aND0j2Y2IkM
```

---
## \#18 Posted by: Silverline Posted at: 2017-07-25T20:17:51.209Z Reads: 1417

```
Pretty awesome project. 

I'm flying racing drones, and have recently upgraded my gimballs in my remote to hall sensors. It feels so much better and so much more precise now. So seeing your project makes me wanna start my 3d printer now 😃
How much do it cost in parts to build this nice remote, with LCD ?
```

---
## \#19 Posted by: solidgeek Posted at: 2017-07-25T20:43:32.989Z Reads: 1423

```
@JLabs That is pretty neat! However I don't like that its a shield :( I like better the one from Sparkfun https://www.sparkfun.com/products/11231 - however the price is quite higher :P 

@Silverline Thanks! Yeah Hall Sensors are great :P! I have made a "shopping list" with the prices in Google Sheets, and the price for the remote is roughly 34$ (not including 3D-printed parts).

https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit#gid=0
```

---
## \#20 Posted by: Maxid Posted at: 2017-07-25T20:46:08.877Z Reads: 1386

```
please get me those files :smiley:
I want to first print it to see if I like it and then order the parts if so.
```

---
## \#21 Posted by: MontPierre Posted at: 2017-07-25T21:13:59.137Z Reads: 1285

```
Very cool project @solidgeek ! 

Is there any code for receiver and remote?
```

---
## \#22 Posted by: solidgeek Posted at: 2017-07-25T21:24:55.841Z Reads: 1276

```
@Maxid I am currently making a few improvements on the 3D-model (testing it out tonight), I will release the files on thingiverse tomorrow :wink: Looking forward to hear your opinion on the printed version! 

@MontPierre Yeah for sure, however it is still some very basic Arduino code, with only a few hours of work. Anyways I will release the prototype code tomorrow as well :) Maybe you guys can help me improve it ;)
```

---
## \#23 Posted by: wafflejock Posted at: 2017-07-25T21:40:58.583Z Reads: 1235

```
Yeah would like to see the code as well, have a couple of things I ran into that I can probably add as a PR to your code for some fail-safes if you don't have them in there already.
```

---
## \#24 Posted by: Silverline Posted at: 2017-07-25T21:43:57.892Z Reads: 1216

```
Cool thanks @solidgeek

Btw. Where are you from 😃 ?
```

---
## \#25 Posted by: markyoe Posted at: 2017-07-25T21:45:06.653Z Reads: 1188

```
Woohoo I'm so printing this out when you post it so that I can see/feel the formfactor.
```

---
## \#26 Posted by: solidgeek Posted at: 2017-07-25T22:20:51.556Z Reads: 1223

```
@wafflejock Looking forward to your PR :D 

@Silverline No problem, I am from Denmark!

@markyoe Looking forward to see the result ;)
```

---
## \#27 Posted by: solidgeek Posted at: 2017-07-27T00:13:23.586Z Reads: 1274

```
Hey guys, I didn't have much time to work on the remote today, however all parts seems to fit so I can't see no reason not to release the STL-files :slight_smile:

https://www.thingiverse.com/thing:2454391

Looking forward to hear your opinions :smile:
```

---
## \#28 Posted by: JLabs Posted at: 2017-07-27T04:42:55.652Z Reads: 1271

```
I'm up to no good :laughing:
<img src="/uploads/db1493/original/3X/2/6/26c3655eec8acba7ca10159593e58091cc76d317.jpg" width="375" height="500">
```

---
## \#29 Posted by: benwong Posted at: 2017-07-27T06:16:31.406Z Reads: 1209

```
@solidgeek  awesome design of the remote, i notice you missing a module in the shopping list? 
the dead man switch/trigger. which module are you using?
```

---
## \#30 Posted by: solidgeek Posted at: 2017-07-27T10:45:59.099Z Reads: 1201

```
Thanks! Yeah I see I forget the trigger button :slight_smile: Its called a 12mm tactile switch: http://www.ebay.com/itm/20PCS-TC-1212T-12x12x7-3-mm-Tact-Tactile-Push-Button-Momentary-PCB-Switch-/281438642731?epid=1546197021&hash=item41870ce22b:g:DfEAAOSwVFlUFCr4

I will add it to the parts list - thanks!
```

---
## \#31 Posted by: MontPierre Posted at: 2017-07-27T11:07:11.675Z Reads: 1181

```
How does it feel in hand @JLabs ?
```

---
## \#32 Posted by: benwong Posted at: 2017-07-27T14:23:37.286Z Reads: 1194

```
Going to order all the parts. Waiting for the programme guide. Haha.
```

---
## \#33 Posted by: wmj259 Posted at: 2017-07-27T15:34:22.149Z Reads: 1218

```
Same, this is a much better compact design versus a original GT2B. Can't wait.
```

---
## \#34 Posted by: solidgeek Posted at: 2017-07-28T10:35:54.715Z Reads: 1251

```
I am almost finished with the newest version of the remote, including the software! I will post a link to github later today with the source code :smile:

For now you will have to make due with a video and a image of the wiring :slight_smile:

https://youtu.be/IgEk8VuB40Y

<img src="/uploads/db1493/original/3X/b/5/b50376c731d49d196a82543890e996f9fd22fb33.jpg" width="429" height="500">
```

---
## \#35 Posted by: NAF Posted at: 2017-07-28T10:42:41.841Z Reads: 1176

```
Pure awesomeness !!  What kind of information would we we able to display ??
```

---
## \#36 Posted by: wmj259 Posted at: 2017-07-28T14:42:53.604Z Reads: 1180

```
Im digging the remote. Can't wait, also, is the code available? I had a semester for java coding on arduinos, maybe I can help out.
```

---
## \#37 Posted by: benwong Posted at: 2017-07-28T15:01:10.176Z Reads: 1172

```
o no, this abit hard for me, i no idea about the writing code. 
any simple way to do that?
```

---
## \#38 Posted by: MontPierre Posted at: 2017-07-28T15:22:29.144Z Reads: 1174

```
It will be very easy, You will have to connect arduino to your computer via USB, open up Arduino app ( free), copy and paste code into it and click upload. More or or less this is it. There are plenty videos on youtube on how to upload code to arduino, Dead easy :)
```

---
## \#39 Posted by: oyta Posted at: 2017-07-28T22:48:29.018Z Reads: 1166

```
@solidgeek Love it! I eager to order the parts! 

* The power module: This one from Adafruit is a bit cheaper: https://www.adafruit.com/product/1944 Could it work and does it fit?
* One features suggestion - adding a hole or something to the enclosure to add connect a leash.
* Would this work with the new VESC 6 that has NRF built in?
```

---
## \#40 Posted by: JLabs Posted at: 2017-07-28T23:14:12.098Z Reads: 1154

```
Feals great! I want to make it work now! 👍
```

---
## \#41 Posted by: markyoe Posted at: 2017-07-28T23:15:23.395Z Reads: 1093

```
I second @oyta 's leash suggestion...
```

---
## \#42 Posted by: solidgeek Posted at: 2017-07-28T23:54:36.958Z Reads: 1185

```
@NAF Glad you like it ;) Well at the moment only data from the remote, fx the remotes battery level etc.

@wmj259 Yeah I have made a github repository https://github.com/MrSolidGeek/NRF24-Esk8-Remote

@benwong I think the hardest part is to assemple everything correctly - without shorting anything!  The rest should be easy enough :slight_smile:

@oyta I am not sure if the module from Adafruit would be a very good choice, as it has a normal USB plug for charging something external. I like your idea of a hole to connect a leash, I will try to implement it in the next version!
Regarding the built in NRF in the VESC 6, unfortunately there are no documetation on how to establish a connection to the it, and I can't get an solid answer from the VESC team yet... So at the moment you will have to use a receiver with UART or PPM :slight_smile:

@JLabs Glad to hear it :slight_smile: I am almost done with the software to the remote, however I am having some problems with the transmission part... I can't seem to establish a connection between the receiver and the remote at the moment. I believe the NRF24 module I am using might be defect or I might accidentally shorted it :confused: I will have to try another one tomorrow - hopefully its just the bad chinese quality thats given me a lesson :wink:  

<img src="/uploads/db1493/original/3X/9/8/98e9ccae142749b43104c24f88cb7843ec558ead.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/f/d/fd51aa0fb1b5f0e7cda25045f908a7e5b94e294d.jpg" width="690" height="388">
```

---
## \#43 Posted by: wafflejock Posted at: 2017-07-29T00:05:45.941Z Reads: 1127

```
Looks awesome, regarding the nrf modules make sure you aren't feeding more than 3.3V into the VCC and use them in low power mode unless you tack a capacitor on there, I fried at least 3 of them by accidentally feeding 5V into them, they work for a few minutes on 5V but will fry out eventually.

---

You do have one of the fail safes in there already for the timeout but you might want to check out elapsedMillis it makes keeping track of that a little easier.

On the **receiver** side would check to see what happens if you remove the MISO pin from the NRF to the arduino, when I did that it was still reading available on the receiver side but the arduino would read the data as 255 which then got sent to the ESC as full throttle (basically I'm pretty sure the pin floated high, it did this while bench testing as well).
```

---
## \#44 Posted by: solidgeek Posted at: 2017-07-29T00:16:35.256Z Reads: 1094

```
Thanks! I just tried changing RF24_PA_HIGH to RF24_PA_LOW and it started working, however only making a connection every second or third try. My older prototype did not have these problems, I will have to dig into this. I think it must be some kind of power issue - even though I already have added a 47uF cap on the NRF24 module. 

Thanks for the advice I will try it out :)
```

---
## \#45 Posted by: Pantologist Posted at: 2017-07-29T01:46:14.990Z Reads: 1076

```
[quote="solidgeek, post:42, topic:28543"]
am not sure if the module from Adafruit would be a very good choice, as it has a normal USB plug for charging something external
[/quote]

You don't have to install the USB port. You can use the 5V and GND as the output connections instead.
```

---
## \#46 Posted by: wmj259 Posted at: 2017-07-29T19:58:43.787Z Reads: 1060

```
Heads up: they don't ship the springs to the US.
```

---
## \#47 Posted by: markyoe Posted at: 2017-07-29T20:51:39.189Z Reads: 1096

```


<img src="/uploads/db1493/original/3X/6/2/620c61b7507479f414d568277da2fac5452db507.jpg" width="375" height="500">
```

---
## \#48 Posted by: Snowi Posted at: 2017-07-31T01:25:37.630Z Reads: 1056

```
What software did you use to create your controller?
```

---
## \#49 Posted by: wmj259 Posted at: 2017-07-31T03:22:01.910Z Reads: 1099

```
Also another heads up for the nrf antenna. They seemed to be defective so the seller told me this.
 <img src="/uploads/db1493/original/3X/f/c/fc11dc8140168ec9b11e43b5073ddac649b6cad1.png" width="281" height="500">
<img src="/uploads/db1493/original/3X/a/4/a46e7ef456118345def9076fcf773e5b33e73899.png" width="281" height="500">
```

---
## \#50 Posted by: MontPierre Posted at: 2017-07-31T08:43:16.318Z Reads: 1055

```
Thanks for heads up, I was just going to order it haha;) maybe that's why @solidgeek had slight issues with them.
```

---
## \#51 Posted by: solidgeek Posted at: 2017-07-31T16:03:52.914Z Reads: 1057

```
@wmj259 Well if thats the case... I found another seller on Aliexpress - I have replaced the link in the parts list and bought a few myself to test. 

@MontPierre Slight issues? My head is gonna explode... I can't seem to get a stable connection with the current nRF24 modules. It is very sensitive, and the range is no more than 1.5 meters. I am thinking of pulling out the nRF24 module from my old remote, and use it instead, as that module surely did work. However I still have to find a good supplier of nRF24 modules. I am waiting for the ones from Aliexpress.

It seems that nRF24 modules from china mostly are crap :tired_face:
```

---
## \#52 Posted by: JdogAwesome Posted at: 2017-07-31T17:53:03.528Z Reads: 1009

```
Looks like an awesome remote, might try it out myself if my Bad Wolf starts having problems. I'm curious though as to why you used the NRF module over something like an ESP that can also serve as the MCU so you can ditch the Arduino.
```

---
## \#53 Posted by: wafflejock Posted at: 2017-07-31T20:43:00.866Z Reads: 1037

```
I've asked others about this too but haven't seen much about doing ad-hoc with the ESP chips since they're usually used on wifi (at least from what I've seen on the youtubes).  I do think a single board with the radio and mcu would be ideal I basically made a PCB that just connects the two boards but it's a fat sandwich compared to baking all the smd components onto a single board.  Problem is the cost to get the chips and assembly done is high unless you're making a bazillion of them (at least a few thousand) so it's hard to justify doing a total custom board, @Sander did a custom nrf board design but costs are way higher for small batches.

---

Pretty sure the way the ad-hoc works with the ESP chips is the same as the particle photon boards where one has to be setup to be an access point and the other one connects to it https://community.particle.io/t/multi-device-talking-possible/13373/7 
Honestly not sure if this is better or worse than the "burst-packet" technology the nrf modules use for point to point communication but feels sort of like shoehorning it with the ESP chips if you're making a mobile access point (on the plus side I suppose multiple devices could connect to it but that must have overhead to it).
```

---
## \#54 Posted by: wafflejock Posted at: 2017-07-31T20:44:51.758Z Reads: 1035

```
About the range in a clear line of site you'll get about 3-4 meters of connection before it loses it completely on low power mode, if you add the capacitor on the gnd and vcc and jack up the power to max with the chips I have can broadcast at least a half a block away.

---

Definitely one of those components that is notorious for being cloned, honestly didn't check the stamp with a magnifying lens or anything to see if it was genuine but haven't really had problems outside of my own errors.

These are the ones I've been using:

https://www.amazon.com/gp/product/B00O9O868G/ref=oh_aui_search_detailpage?ie=UTF8&psc=1
```

---
## \#55 Posted by: solidgeek Posted at: 2017-08-01T00:27:31.349Z Reads: 1040

```
I finally got it working! The problem wasn't the actual transmission, but instead the auto-acknowledgement. The remote uses the auto-ack feature of the nRF24 to know if the transmission was a succes or not, however I had not taken into consideration that a transmission could be succesfull even though the auto-ack wasn't recieved probably.

And it seems that the nRF24 modules weren't to blame, but instead the poor quality of my Arduino Nanos 3.3V output. Apparently the clones that are being sold on Ebay etc. comes with a very poor 3.3V regulator, that causes a lot of electronic noise - some worse than others. The noise/voltage ripples can make signal distorted and therefore not getting to the remote.  

I solved this by adding a 220uF cap on the 3.3V rail, and adding a 47uF on the nRF24 modules (soldered it directly to the pins). This however didn't solve the issue completly, I had to make some software changes on the receiver, and now the remote works perfectly with a distance of +8 meters.

I will update the software on githup tonight and finish the schematics as soon as I can :slight_smile: 

https://github.com/MrSolidGeek/NRF24-Esk8-Remote

@JdogAwesome Thanks :-) ! I have choosen to use nRF24 module, because they are power efficient, and easy to get and use. The idea of the remote, was that anyone with a little DIY-skills should be able to make one by themself, and therefore I believe that an Arduino and the nRF24 modules are a perfect match :slight_smile:
```

---
## \#56 Posted by: Snowi Posted at: 2017-08-01T23:49:46.210Z Reads: 973

```
Why go through this trouble with the NRF when you can use bluetooth module? Isn't it much simpler?
```

---
## \#57 Posted by: wafflejock Posted at: 2017-08-01T23:54:48.257Z Reads: 1006

```
No not really the pairing is also a pita typically and the hc-05 or hc-06 chips are still more than the nrf chips.  I used one and controlled from an app on my phone but would recommend against it.  With a controller instead of phone as controller it might be better but still don't see the advantage over the nrf chips.

---

Also I use Bluetooth for headphones and Android is crappy enough at A2DP or whatever it's using that I don't really trust all the extra noise that will make (maybe unjustified fear but there nonetheless)
```

---
## \#58 Posted by: solidgeek Posted at: 2017-08-02T00:19:39.465Z Reads: 998

```
@Snowi Bluetooth was also my first thought! However I read many places that Bluetooth 2.0 (HC-05 etc) aren't that reliable to use for critical applications such as Esk8 at high speeds in crowded cities - your life is at stake :cold_sweat:. In addition, Bluetooth doesn't really have any advantages, except that it is (in my experience) easier to work with. Maybe a newer version of Bluetooth (3.0, 4.0) would be more reliable in the future? For the moment I think nRF24 will do :stuck_out_tongue:

@wafflejock I agree
```

---
## \#59 Posted by: solidgeek Posted at: 2017-08-02T12:10:26.874Z Reads: 992

```
I just found this PCB, with a built-in charger and boost converter! Seems very nice, and fits perfectly (with extra room) next to the battery in the remote. It does not have a built-in over-discharge protection, however, the battery I am using has - so no problem. 

https://www.aliexpress.com/item/6W-5V-UPS-mobile-power-Diy-Board-Charger-Step-up-DC-DC-Converter-Module-for-3/32790658678.html

This seems a lot easier than using two different modules, it would make the assembly process much easier at least :slight_smile:
```

---
## \#60 Posted by: TranxFu Posted at: 2017-08-02T12:18:07.369Z Reads: 967

```
Are you planning any design changes in the near future :) ? Just wanted a heads up if you do and before I start printing it.
```

---
## \#61 Posted by: solidgeek Posted at: 2017-08-02T12:20:45.418Z Reads: 878

```
Yes I am planning to make a hole for leash attachment, and adding a 3D-model for the receiver too :slight_smile: If you don't need leash, well there will be no changes to the remote design at the moment :slight_smile:
```

---
## \#62 Posted by: TranxFu Posted at: 2017-08-02T12:22:49.953Z Reads: 858

```
Thanks mate ! I'll be waiting on that leash hole then haha. Are you going to finalize the BOM and a step by step guide anytime soon ?
```

---
## \#63 Posted by: solidgeek Posted at: 2017-08-02T12:29:24.574Z Reads: 873

```
Yes I am :) I am currently working on a wiki/guide on github, I hope that will do ;) maybe I will make an instructables later.
```

---
## \#64 Posted by: kyo Posted at: 2017-08-02T12:30:21.796Z Reads: 901

```
how about this one. it has micro usb interface.

https://www.aliexpress.com/item/5PCS-TP4056-5V-1A-Mini-Micro-Interface-USB-Lithium-Battery-Charging-Board-DIY-Charger-Module/32671926086.html?spm=2114.search0302.4.14.WtRwTM
```

---
## \#65 Posted by: solidgeek Posted at: 2017-08-02T12:34:59.151Z Reads: 944

```
It's basically the same I used in my current remote build, however it is only a charger nothing more (you will need a boost converter board too). The micro USB has to be removed anyway, as the charging port is placed next to the switch, and it can't fit attached to the board. 

<img src="/uploads/db1493/original/3X/a/0/a074607909dab12e33369623edb60e87d56685a0.PNG" width="445" height="500">
```

---
## \#66 Posted by: kyo Posted at: 2017-08-02T12:38:02.993Z Reads: 895

```
ok, thanks.
```

---
## \#67 Posted by: solidgeek Posted at: 2017-08-02T12:50:17.097Z Reads: 908

```
I just found another one which fits (with over-discharge protection). I will order a few of both boards and test them out as soon as they arrive (usually two weeks). 

Charger and boost module (over discharge protection): $3,79
https://www.aliexpress.com/item/2-in-1-Boost-Charger-Module-DC-DC-Step-Up-Converter-DC-2-5V-3V-3/32690709065.html

Charger and boost module (no over discharge protection): $3,18
https://www.aliexpress.com/item/6W-5V-UPS-mobile-power-Diy-Board-Charger-Step-up-DC-DC-Converter-Module-for-3/32790658678.html
```

---
## \#68 Posted by: Silverline Posted at: 2017-08-02T12:57:50.563Z Reads: 868

```
Håber du poster dit projekt i FB gruppen, når du er i mål :-) Jeg vil i hvertfald bygge din remote, men venter med at bestille noget, til du har låst dit på de forskellige komponenter :-)
```

---
## \#69 Posted by: solidgeek Posted at: 2017-08-02T13:54:35.486Z Reads: 843

```
Helt sikkert, glæder mig til at høre jeres mening :D !
```

---
## \#70 Posted by: wmj259 Posted at: 2017-08-02T15:52:33.026Z Reads: 857

```
Are these necessary from what was originally on the parts list? Or they are better features? I already got the stuff from the parts list shipped, but it's gonna be stuff in the shipping for two weeks.
```

---
## \#71 Posted by: solidgeek Posted at: 2017-08-02T21:44:48.458Z Reads: 886

```
No these are only to simplify the assembly process. The remote needs a lipo charger, and a boost converter (on the parts list) I just found a board that could do both :) However, I just realized that using one board probably isn't a better solution because you wouldn't be able to put a switch between the charger and the boost converter. 

Maybe I should design a custom PCB... Another day :P
```

---
## \#72 Posted by: solidgeek Posted at: 2017-08-03T19:23:55.593Z Reads: 903

```
So I was testing out my remote today and had what felt like a few loss of connection (no acceleration, no braking). I began debugging the connection and found that it worked perfectly. The problem wasn't the transmitting part, but the trigger button. It seems that the tactile button I am using has a "dead-zone" after it "clicks". 

https://www.youtube.com/watch?v=mYTaYsBsJ4w

I will have to make some adjustments to the trigger part, so the button doesn't release accidentally.
```

---
## \#73 Posted by: bmcm Posted at: 2017-08-03T20:10:21.994Z Reads: 867

```
This isn't the first time I've seen a hall sensor used over a pot, but why? What are the pros/cons of using a hall sensor vs a pot?
```

---
## \#74 Posted by: Silverline Posted at: 2017-08-03T20:20:26.631Z Reads: 852

```
More precision and resolution. Over time, the mechanical pot will wear down and get imprecise and introduce jitter. In princip a hall sensor will last forever, since its magnetism and the parts is not tuching each other.

This is a hall sensor gimball for a Rc remote. I did this upgrade to my own Taranis, and the feeling was a night/day experience. He explains it very well : https://www.youtube.com/watch?v=h5oI6is-0CE
```

---
## \#75 Posted by: bmcm Posted at: 2017-08-03T20:43:14.116Z Reads: 822

```
I guess that makes sense, esp considering pots are mostly used for when you only adjust it maybe several times a day (volume control, etc), not many times a minute. Now I'm starting to wonder how all sorts of things work - throttle pedals in cars, etc :slight_smile:
```

---
## \#76 Posted by: Maxid Posted at: 2017-08-03T22:29:57.427Z Reads: 829

```
To be fair though: potentiometers have been used in rc remotes since forever (just look at the all time favourite here: the gt2b) and have been holding up quite well. 
Hall sensors are more sophisticated though and I guess the only downside is that they might be more expensive than a traditional potentiometer design.
```

---
## \#77 Posted by: solidgeek Posted at: 2017-08-03T22:55:28.515Z Reads: 836

```
Well, I don't know much about the pros/cons of using a Hall Effect sensor, except that a Hall sensor is very small and has no mechanical friction. Basically I choose to use a Hall sensor, simply because I couldn't find any high-quality potentiometer that I could fit inside the remote. And well... A Hall sensor seems a little more high tech :wink:
```

---
## \#78 Posted by: lrdesigns Posted at: 2017-08-03T23:55:10.512Z Reads: 814

```
Also no effected by water, which is why I want to put one in my GT2B. Anyone know of a drop in replacement for the pot?
```

---
## \#79 Posted by: wafflejock Posted at: 2017-08-04T01:26:16.923Z Reads: 825

```
Believe magnets typically weaken over time especially if they are heated and or shocked from impact but everything is subjective to damage if you hit it hard enough.  The hall sensor may also be affected by other magnets such as those used in wallet if it was in an inopportune place.  Up sides have already mostly been pointed out, no friction from the sensor itself so free to use any sort of spring or other mechanism to create the feel you want.
```

---
## \#80 Posted by: MontPierre Posted at: 2017-08-04T10:03:52.355Z Reads: 828

```
@solidgeek please post link to PayPal or something similar for donations once your project is finished.  I'm sure a lot of us ( including myself ) would love to send your few € for all your hard work ! 👍🏻
```

---
## \#81 Posted by: Nordle Posted at: 2017-08-04T10:20:26.987Z Reads: 738

```
Love this project! Why not use arduino with integrated nrf module? Could safe a lot trouble from what i read, no experience actually.
```

---
## \#82 Posted by: oyta Posted at: 2017-08-04T21:26:05.975Z Reads: 784

```
[quote="solidgeek, post:42, topic:28543"]
Regarding the built in NRF in the VESC 6, unfortunately there are no documetation on how to establish a connection to the it, and I can't get an solid answer from the VESC team yet... So at the moment you will have to use a receiver with UART or PPM :slight_smile:
[/quote]

Are you on the VESC-project forums? I asked a question there now. I'll see what the answer is. However I guess it is something like Vedder's Nunchuck FW code on Github. See the links at http://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588?u=oyta
```

---
## \#83 Posted by: saul Posted at: 2017-08-04T22:21:24.426Z Reads: 781

```
yea I switched to hall sensors also. its just more fun to play with magnets.
 but yea no mechanical friction or wear. less noise. in theory more precise. 
and tiny.
```

---
## \#84 Posted by: solidgeek Posted at: 2017-08-04T22:59:44.531Z Reads: 846

```
@MontPierre Thanks mate, I will think about it :-) ! 

@Nordle I am glad you like my work! Regarding your proposal... Do they exist? :open_mouth: If they indeed do, well it would be interesting to try it out! I am thinking about making a custom PCB with a few solder points (easy assembly), a socket for an Arduino Nano (or mini) and use a Low Dropout Regulator to make a stable 3.3V for the nRF24 module. I believe this would be much better than the 3.3V supplied by the Arduino, and eliminate any power related issues :) 

@oyta Yes I am, I have asked a few questions in there myself. The only information I got was that I could find what I needed in the source code for the VESC nunchuck. However, the source code isn't documented AT ALL, with no or only a few code comments - not easy for a DIY-guy as myself :stuck_out_tongue: I would be much interested in what you find out!

@saul Gotta love those magnets ;)

<img src="/uploads/db1493/original/3X/2/5/256b7968e25996430faa929e117eba8e4b94ea31.jpg" width="571" height="500">
```

---
## \#85 Posted by: saul Posted at: 2017-08-05T03:25:55.447Z Reads: 845

```
[quote="solidgeek, post:84, topic:28543"]
Do they exist? :open_mouth: If they indeed do, well it would be interesting to try it out! I am thinking about making a custom PCB with a few solder points (easy assembly), a socket for an Arduino Nano (or mini) and use a Low Dropout Regulator to make a stable 3.3V for the nRF24 module. I believe this would be much better than the 3.3V supplied by the Arduino, and eliminate any power related issues :slight_smile:
[/quote]

They do but not really so I made my own. :nerd:
I started with a nano clone for easy debugging with usb.

this version uses atmega328p pu.  ftdi breakout, and regular nrf, 3.v3 ldo mcp 1700. 3x pwm out, 2x analog in.

the new version has 4 pwm, irq interupt, 1 analog pot, 1 hall sensor analog. + i2c out for oled.
you're welcome to use my hardware.  

<img src="/uploads/db1493/original/3X/1/9/1983f61a00edc6a6db4f7b6f81c294c4742f8d39.jpg" width="690" height="387">
<img src="/uploads/db1493/original/3X/5/4/5409514027bfe33d22d01401d90fe503cbb3c5ef.jpg" width="690" height="387">
```

---
## \#86 Posted by: solidgeek Posted at: 2017-08-06T10:05:39.518Z Reads: 830

```
Looks good! However I don't think I am going to use a atmega328p. I would rather use a Pro mini, because it is small and a little easier to reprogram :slight_smile: I made and ordereder a PCB yesterday

<img src="/uploads/db1493/original/3X/d/c/dca0775099b78afe35bccdf4338166b5bf221365.PNG" width="253" height="500">

I have added a LDO voltage regulator (5v to 3.3V) and some caps for the nRF24, and used the footprint for a pro mini (clone). I think it will help keep all the wiring more simple.

I have ordered some cheap Micro switches (12*6*5mm) they should arrive tomorrow, I hope I can replace the tactile button with one of them.
 <img src="/uploads/db1493/original/3X/f/0/f0cc4ff98cbfc9d0840a81b5e67bf2ed753d2729.jpg" width="500" height="500">
```

---
## \#87 Posted by: MontPierre Posted at: 2017-08-06T14:19:58.673Z Reads: 817

```
@solidgeek I just came across a exway board - and its remote .... Check it out. Similarities are amazing :) I don't think board is out as of yet.

https://www.exwayboard.com

https://www.exwayboard.com/public/img/exway_section4_img_con.png

https://www.youtube.com/watch?v=-qkyYZPCwBw&feature=youtu.be&t=4m47s 

https://youtu.be/d6VJSZsKN0Y?t=2m47s
```

---
## \#88 Posted by: NAF Posted at: 2017-08-06T14:55:37.124Z Reads: 800

```
This exway brand is a ghost company of Stary boards and this remote is just a clone of stary boards remote.

<img src="/uploads/db1493/original/3X/6/5/6555c4a92cadb2b885df0fb96b4254e581a89f9a.JPG" width="275" height="183">
```

---
## \#89 Posted by: MontPierre Posted at: 2017-08-06T14:57:56.385Z Reads: 800

```
Cool! This explains a lot.
```

---
## \#90 Posted by: solidgeek Posted at: 2017-08-07T01:16:22.436Z Reads: 811

```
I have made a new version of the shell tonight, with room for a wrist strap and changed the design so that there are no need for bolts inside to hold the trigger button etc.

<img src="/uploads/db1493/original/3X/3/8/384beafd4dfb4a8282991e6750a83c3561e889b1.PNG" width="690" height="426">

Going to test everything out tomorrow :-)
```

---
## \#91 Posted by: solidgeek Posted at: 2017-08-07T01:18:47.102Z Reads: 799

```
That remote looks nice ;) I like their OLED interface, maybe I am going to steal some of those graphics :sunny:
```

---
## \#92 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-07T06:31:09.760Z Reads: 780

```
Please upload the new version to thingiverse! I'd like to print it :)
```

---
## \#93 Posted by: MontPierre Posted at: 2017-08-07T06:36:30.707Z Reads: 774

```
You're not copying - you're being inspired by their graphics 😂 Now repeat after me 🤣
```

---
## \#94 Posted by: solidgeek Posted at: 2017-08-07T11:59:41.859Z Reads: 784

```
@UniqueSnowflakeN27 I am currently printing top and bottom (roughly 5 hours), I will upload the new version if everything fits correctly :slight_smile:

@MontPierre As my old school teacher always told us "copy and paste - no time to waste" ;)   :sweat_smile:
```

---
## \#95 Posted by: wmj259 Posted at: 2017-08-09T00:52:12.564Z Reads: 800

```
If anyone needs buttons hit me up, just pay for postage and ill send a few your way.
<img src="/uploads/db1493/original/3X/0/3/03aa4bc7ba62a7012faff62e7a0cb5c05900a878.jpg" width="690" height="388">

Boost converter came in its really really small :grin:
```

---
## \#96 Posted by: solidgeek Posted at: 2017-08-09T10:19:42.235Z Reads: 783

```
Looks nice! I am very interesting to see if your buttons have the same "deadzone" as the ones I got from a local shop here in Denmark. Its a little anoying as I have to press my trigger a little extra after it says "click" to activate the trigger :weary: I am still working on a solution :sunny:
```

---
## \#97 Posted by: solidgeek Posted at: 2017-08-09T23:26:08.489Z Reads: 799

```
Just finished the newest version of the remote, with no need for inside bolts, room for a wrist strap and some minor changes that should improve the overall quality of the remote.

I have been trying to solve the "dead zone" issue with the tactile buttons, however, I have not found a solution. Instead, I have bought some new buttons (12,6mm micro switches) and made room for them, which works much better. However, the previous tactile buttons should still fit perfectly.

<img src="/uploads/db1493/original/3X/1/e/1ebea97dcb9a4b24fa93c3a9fa3b40a2899d88d1.jpg" width="427" height="500">

Will be releasing/updating my Thingiverse project tomorrow, so you guys can try out the design :-) 

Thanks for the support!
```

---
## \#98 Posted by: wmj259 Posted at: 2017-08-09T23:40:43.751Z Reads: 774

```
Received the arduino nano came in today.
```

---
## \#99 Posted by: solidgeek Posted at: 2017-08-11T01:22:48.202Z Reads: 811

```
I just realized that the lipo battery shouldn't be charged with more than 1C (or 400mA), and the charger TP4056 normally is programmed to output 1A (1000mA) by setting the R_prog resistor to 1,2kOhm. To keep the battery well charged, and safe I recommend changing the resistor to a 5kOhm, which would limit the charge current to 250mA.

<img src="/uploads/db1493/original/3X/1/d/1dff3b56bd5e3b15b16a2a2a04335058ef20bddf.PNG" width="653" height="500"> 

I have released the newest (and maybe final?) version of the 3D-model on Thingiverse. It should be mostly plug-n-play, you will only need a spring and six M3 16mm bolts :-) 

https://www.thingiverse.com/thing:2454391

I am planning to make a few prototypes for you guys (fully assembled and tested) if anyone is interested :slight_smile: !
```

---
## \#100 Posted by: markyoe Posted at: 2017-08-11T04:32:36.199Z Reads: 776

```
I'd totally be interested in a prototype! I'd compensate you for it, of course. This is an awesome project.
```

---
## \#101 Posted by: wmj259 Posted at: 2017-08-11T06:15:17.639Z Reads: 727

```
I'd be interested as well, and compensate like above.
```

---
## \#102 Posted by: Silverline Posted at: 2017-08-11T06:31:21.089Z Reads: 719

```
But i dont like that tactile buttom. I could just bypass right ?
```

---
## \#103 Posted by: High-roller Posted at: 2017-08-11T08:14:40.876Z Reads: 715

```
I might be up for a prototype if you're offering! With proper compensation to you of course...
```

---
## \#104 Posted by: navgor Posted at: 2017-08-11T10:19:35.642Z Reads: 701

```
I'd be up for a prototype too. :)
```

---
## \#105 Posted by: zeah Posted at: 2017-08-11T12:54:23.553Z Reads: 694

```
I'd be up for one as well and I will make a donation for your excellent work!!:+1:
```

---
## \#106 Posted by: Neilfenstein Posted at: 2017-08-11T13:00:17.317Z Reads: 711

```
I'd be up for a prototype and will compensate as required.
I spent some time teaching myself 3D modelling and bought an arduino starter kit to do something very similar to you but you beat me to it with something way better than I could have managed.
```

---
## \#107 Posted by: solidgeek Posted at: 2017-08-11T13:56:24.983Z Reads: 750

```
@markyoe Sounds good, I added you to the list :slight_smile: And thanks man!

@wmj259 Nice, you are added :slight_smile:

@Silverline Sure thing, however, it's a good safety feature! If you are very creative, you could program it to other things, such as turn on lights etc. :P Are you up for one?

@High-roller Sounds good, I have added you to the list :-)

@navgor Thanks, you are on the list too!

@zeah Sounds good, and thanks mate! I have added you to the list

@Neilfenstein I am glad you like my work! You too are added to the list :P   

Where are you all from, because I am only planning to ship to Europe? I am in touch with a guy from the USA, who could produce and ship the prototypes inland. I will begin to find good suppliers for the needed items - it would be nice if I could find a good European supplier (any ideas?). I believe the price for remote and receiver excluding shipping (EU) would be around 50€ :blush:
 
Thanks for the support, looks like I should begin to produce 7-8 prototypes :sunny:
```

---
## \#108 Posted by: Silverline Posted at: 2017-08-11T14:07:49.612Z Reads: 716

```
Yes i am thanks 
What about you @DK-Odense 
We are both from Denmark 😃
```

---
## \#109 Posted by: High-roller Posted at: 2017-08-11T14:08:45.150Z Reads: 694

```
No chance of getting it to Israel somehow?
```

---
## \#110 Posted by: Neilfenstein Posted at: 2017-08-11T14:16:51.260Z Reads: 703

```
Awesome!

I am in the U.K. I hope that will be ok. I can pay any additional for shipping if necessary. 

Thanks.
```

---
## \#111 Posted by: DK-Odense Posted at: 2017-08-11T14:19:27.072Z Reads: 691

```
I am up for one 👍 Count me in @solidgeek
```

---
## \#112 Posted by: navgor Posted at: 2017-08-11T14:42:27.806Z Reads: 700

```
[quote="solidgeek, post:107, topic:28543"]
Where are you all from, because I am only planning to ship to Europe?
[/quote]


Thanks mate! London, UK here.
```

---
## \#113 Posted by: solidgeek Posted at: 2017-08-11T14:59:52.150Z Reads: 687

```
@High-roller I am sure we can find a solution :-)

@Neilfenstein UK is just fine!

@DK-Odense Sounds good ;)!

@navgor Great!
```

---
## \#114 Posted by: High-roller Posted at: 2017-08-11T15:29:32.012Z Reads: 668

```
Thanks man! Actually, if you send it to the US before September, that might work for me. Otherwise we can figure something out. 
Do you have an idea of what the price will be for the remote?
```

---
## \#115 Posted by: Jammeslu Posted at: 2017-08-11T16:08:01.446Z Reads: 655

```
Im from sweden mate
```

---
## \#116 Posted by: wmj259 Posted at: 2017-08-11T16:08:12.653Z Reads: 657

```
I'm also in the US
```

---
## \#117 Posted by: markyoe Posted at: 2017-08-11T18:18:27.155Z Reads: 661

```
I'm in the US also, but I'm open to paying for shipping across the pond.
```

---
## \#118 Posted by: tueboard Posted at: 2017-08-11T19:02:18.301Z Reads: 663

```
Im interested too :) (spain, Europe)
```

---
## \#119 Posted by: solidgeek Posted at: 2017-08-11T19:49:07.334Z Reads: 743

```
I am in a dialog with @JLabs about making prototypes for you guys in the US :-) 

@tueboard that makes 7 prototypes for Europe :P 

**Europe:** DK-Odense, Neilfenstein, navgor, Silverline, Jammeslu,  zeah, tueboard 
**US:** markyoe, wmj259,  High-roller (maybe) 

Did I forget anyone?

I just found an Arduino Nano V3 with a dedicated 3.3V regulator and a micro USB. This seems promising, as it easily could power the nRF24 and all the other electronics, without an external dedicated 3.3V regulator (still needs a 5V boost converter).

https://www.aliexpress.com/item/Nano-V3-ATmega328-CH340G-Micro-USB-Pin-headers-NOT-soldered-Compatible-for-Arduino-Nano-V3-0/32664577152.html

I am going to order 20 of these :smile:
```

---
## \#120 Posted by: NAF Posted at: 2017-08-11T20:33:14.992Z Reads: 760

```
@solidgeek This remote is awesome..but can you add some simple functionality for the OLED and pull some basic info from the vesc like remote from STARY BOARD ?  ..all we need is SPEED . BATTERY . and RANGE ...that would be enough. 

<img src="/uploads/db1493/original/3X/d/a/dae4cd7f1cb930fc1b0c8b43823d80152af172ef.png" width="179" height="473"><img src="/uploads/db1493/original/3X/c/4/c40e064acd87f66edaea7926f1e170a288892d18.png" width="663" height="363">
```

---
## \#121 Posted by: Silverline Posted at: 2017-08-11T20:36:40.700Z Reads: 718

```
Speed, battery and range / distance that would be so cool. And yes, that`s all we need.... :-)
```

---
## \#122 Posted by: zeah Posted at: 2017-08-11T21:39:39.972Z Reads: 707

```
Thanks @solidgeek! I´m in Portugal btw
```

---
## \#123 Posted by: Snowi Posted at: 2017-08-12T04:07:01.249Z Reads: 715

```
Are you going to do a YouTube tutorial on how you made and assembled everything, including programming?
```

---
## \#124 Posted by: wafflejock Posted at: 2017-08-12T04:10:47.326Z Reads: 736

```
Not sure if he will but programming the arduino nano is dead simple you just download his repository open the .ino file (arduino project file) and write to USB.  Since he's using the nrf modules he's probably using one of the RF24 libraries too so you'd need to download and extract that to your libraries folder and maybe one for the display as well... actually now that I'm writing this up a YouTube video would probably be a good idea ;)

Beyond getting the libraries though you basically load up the ino project file and hook up the nano via USB to a computer then select the port and board type in the arduino interface (drop down menus) and then hit a button to compile the code and upload it to the board.

I did a general walk through including the programming steps here for my own remote but only wrote it up and you can skip over all the physical assembly and FTDI stuff, the arduino IDE stuff will be the same though just his code instead of mine:

https://github.com/shusain/eskatecontroller

---

Actually not sure if the hall sensor requires the manual calibration and setting like mine either I imagine that is the same too though since it depends on how powerful your magnet is and exactly where it ends up at the top and bottom end.
```

---
## \#125 Posted by: solidgeek Posted at: 2017-08-12T15:01:57.962Z Reads: 712

```
Yes I most certainly can :smile: The only reason why I haven't is that I am using my VESCs UART port for the Metr.at bluetooth module. I will try to add it tonight :slight_smile: 

@Silverline I am not sure about distance, I would have to calculate that by the values the VESC outputs. I will look into it :-)
```

---
## \#126 Posted by: MontPierre Posted at: 2017-08-12T19:21:06.660Z Reads: 691

```
Guys, as I don't have 3D printer - would you know approx cost of printing it in UK? I've heard of printing Hubs. Can you give me a rough estimate on how much it would cost me to have it done it one of the hubs ?
```

---
## \#127 Posted by: solidgeek Posted at: 2017-08-12T19:26:18.122Z Reads: 670

```
You can easily check it yourself, if you upload the STL models to https://www.3dhubs.com/ and find a local hub :-)
```

---
## \#128 Posted by: MontPierre Posted at: 2017-08-12T19:32:21.409Z Reads: 665

```
On it ! Thanks!
```

---
## \#129 Posted by: solidgeek Posted at: 2017-08-12T19:52:14.502Z Reads: 658

```
Let me know what you find out :-) 3Dhubs normally are very cheap, at least in Denmark :P
```

---
## \#130 Posted by: MontPierre Posted at: 2017-08-12T20:16:16.232Z Reads: 664

```
Ok - anything between £18 and £30 in pla/Abs. Any tips on print resolution and type of material and printer ?
```

---
## \#131 Posted by: solidgeek Posted at: 2017-08-12T20:20:42.934Z Reads: 656

```
I do not know about what printer to choose (I am using a CR-10/Afinibot A31), however, I use a resolution of about 150 microns (0,15m per layer). I have printed all parts in PLA, however, it would probably be better in ABS (or something with similar strength).
```

---
## \#132 Posted by: Silverline Posted at: 2017-08-12T20:23:34.298Z Reads: 645

```
Bliver din STL fil ændret mere nu ? Ellers kunne jeg nemlig godt finde på lige at printe den for sjov 😃
```

---
## \#133 Posted by: wafflejock Posted at: 2017-08-12T20:53:34.925Z Reads: 649

```
Would suggest using ABS, PLA is good for getting the shape of something perfect (not much warping right off the printer) but doesn't really hold up over time (very brittle and prone to crack easily also gets worn down by relatively low temperatures).
```

---
## \#134 Posted by: MontPierre Posted at: 2017-08-12T22:22:45.498Z Reads: 614

```
I'll go ahead with ABS the - perhaps 100 microns? And then sand it down for smoother finish?
```

---
## \#135 Posted by: wafflejock Posted at: 2017-08-12T22:42:38.484Z Reads: 654

```
Yup a little sanding works really well you can also look into making an acetone "vapor bath".  If you put ABS into a container that has a cloth soaked in acetone in it (not touching the model) the acetone will evaporate in the container and the bit of it that reacts with the outside will "melt" the layer lines, you just need to be careful not to leave it in there for too long or with too much acetone (just soaking a paper towel is pretty safe just check it every hour leave it outside or somewhere well ventilated so you don't get a build up of acetone in a place it could explode).  It's a bit more dangerous than just sanding (though you also don't want to breath bits of plastic) but has a great result on ABS (doesn't work on PLA but sanding works well there).

Look into the acetone vapor bath option on the net and will find more details you also don't want to really touch the model right after it's been in the acetone vapor since it will remain "melted" for a while so you need to take it out without bending it or take the acetone cloth out and let the acetone vapor out of the container and give the model some time to sit (maybe an hour the acetone will evaporate pretty quickly).
```

---
## \#136 Posted by: solidgeek Posted at: 2017-08-13T01:22:27.777Z Reads: 666

```
@Silverline Altså jeg kan ikke love, at der ikke er noget der bliver ændret i fremtiden - men jeg er tilfreds med designet på nuværende tidspunkt :P Kunne være fedt hvis du gad, altid godt at høre andres mening når de får den i hånden!

@wafflejock I have used carbon infused PLA for the bottom part, and I am going to print the prototypes in that PLA as well. Don't you think that would be durable enough?  

@MontPierre Looking forward to seeing the results!  

I have done some testing with the UART library today and found that the VESC 6 has changed a bit, regarding the UART communication. Because of that, I don't have a means of testing how my remote works with a VESC 4. However, I did manage to pull basic data from the VESC 6, such as input voltage, used amps, regen etc. Until I get my hands on a VESC 4 I am not going to be able to test the remote completely :-) 

I will start working on displaying the data on the OLED display in next week! Pictures will be coming :O
```

---
## \#137 Posted by: wafflejock Posted at: 2017-08-13T01:33:14.638Z Reads: 713

```
Nice yeah I mean for prototypes it is going to be good enough initially I just wouldn't expect long term durability out of them.  I printed risers out of PLA that are going to go under a lot more impacts and stress typically and they eventually crumbled but held up for a decent amount of time considering the material properties (over a month of regular riding which was more than I expected really, think they were 25% infill and about .5" thick).

About Carbon infused PLA I haven't used that but have heard it works well, there's also the annealing process that is supposed to help a lot with overall part strength:

https://www.youtube.com/watch?v=CZX8eHC7fws

For the most part ideally the controller isn't going through too much but occasionally I end up tossing mine or smashing it into the ground.  After a year of love, and a few bails, it has started to show some age (granted my printer was in bad shape when I made it in the first place so layer adhesion wasn't great to start).  My guess is if your printer nozzle is clean and everything is extruding and sticking well then they'll be tough enough especially with the carbon infused filament (I've also heard carbon infused and metal infused filaments can cause the hot end nozzle to wear down more quickly so watch out for that or use a hardened steel nozzle).

---

ABS just tends to be a bit more "mushy" and impact resistant so it's less likely to crack and more likely to bend a little bit in most cases, Nylon is more extreme where it will flex a lot and won't really ever crack, down side is it's really hard to print with if you're making anything large.  I printed my x-carriage out of nylon and it's no bigger than this controller and it came out well but warping and stopping water absorption is a battle with Nylon.

---

Really if you plan to make a lot of these I'd look at using your PLA to make a mold out of silicone then pour the parts.  The initial investment in silicone is somewhat high (and there is a little learning curve) but once you have a mold you can use it for 50 parts or more and each part takes about 10-15 minutes to cure (and you can easily color the plastics or choose harder/softer plastics).  This gets rid of the layer adhesion problem, you just make one nice model out of PLA and sand it down and use it as the original to make a mold then can make them pretty easily at will (just need an area you can mix up the chemicals and clean up easily).  I'm in the process of doing this with my own enclosure parts but am working on 3D printing parts of the mold box too since silicone is so darn expensive and the battery boxes are pretty big and lots of empty space.

If you want to try it out this is a sample kit of the silicone and plastic it is probably enough silicone to make the molds for all the parts for your controller if you get everything right the first time around:

https://www.amazon.com/Smooth-Silicone-Smooth-Cast-Plastic-Compound/dp/B01D9BUSI0/ref=sr_1_1?ie=UTF8&qid=1502589500&sr=8-1-spons&keywords=oomoo+300&psc=1&smid=A19NVE4G6SOT2C

If not maybe one to try and one to get it right if you're like me :slight_smile:

The time and effort with a mold is up front and you get a lot more parts a lot quicker in the long run.
```

---
## \#138 Posted by: Fatglottis Posted at: 2017-08-13T08:28:04.340Z Reads: 689

```
Hi! Nice build.. i like it a lot :slight_smile:

I'm also running an arduino based remote with code from RollingGecko. I like to share what hardware I'm using.
For lipo chargin/protection and 5V boost (all in the same PCB). Never had any problem with it.
http://www.ebay.com/itm/2PCS-5V-Battery-Charge-Discharge-Protection-Integration-Board-Boost-Voltage-/201708017533

I did not see how you turned on/off the remote but I'm using a soft switch board for this. I can then power up/down the remote using on of the push buttons on the remote.. holding it pushed for a long time. (instead of using an on/off switch).
http://www.ebay.com/itm/3V-12V-Solid-State-Switch-Control-Module-Power-Soft-Start-Switch-PCB-for-DSO-068-/141768160000?hash=item21020a7300:g:l60AAOSwTapV7P5M

My plan was to integrate a small display as well but the form factor of the wii nunchuck im using is not optimal for this.
I do have all the data send from the VECSs to the already.. I just need a way to visualize it. At the moment I'm using a vibrator with different patterns to signal low battery etc. :D
```

---
## \#139 Posted by: MontPierre Posted at: 2017-08-13T10:22:58.490Z Reads: 633

```
@Fatglottis This is turning into awesome project! Thanks for sharing you're knowledge and experience! I'll try to see if I can come up with nice 8bit graphics for the remote battery status and etc.
```

---
## \#140 Posted by: solidgeek Posted at: 2017-08-13T13:12:03.859Z Reads: 657

```
Hi! Thanks for sharing :slight_smile:

I have been looking at the exact same model for battery charging and boost, however, there were a few things I didn't like about it. First of all, I needed something thin, not any higher than 5-6mm. Secondly, I needed a way to turn of the boost converter while the battery still was connected to the charging circuit, otherwise, I would not be able to charge the battery, while the whole circuit was turned off. How did you solve this?

The TP4056 board is also current-limited (0-1000mA depending on R_prog), which I think is a nice feature to have, so you do not charge your battery with too high of a current. Charging a 400mA battery with 1A could kill or even worse make the battery explode at some point :O

I like your idea with the solid state switch, however, I think the PCB takes up more space than I got the room for at the moment. However, it opens the possibility to use a normal push button (small tactile switch), which I quite like.

I would like to see your software sometime if you are willing to share :-) !
```

---
## \#141 Posted by: mikenyc Posted at: 2017-08-13T16:06:03.034Z Reads: 586

```
Hey I’d like to get one as well. Shipping to the United States!

Question: what would it take for this to be able to power on the board?
```

---
## \#142 Posted by: solidgeek Posted at: 2017-08-13T16:09:51.541Z Reads: 606

```
Great! I will add you to the list :-) 

Regarding your question... The receiver would have to be powered in some way all the time, and being able to turn on/off some kind of soft switch (such as a vedder antispark). It's something that I don't have any plans for :P
```

---
## \#143 Posted by: Fatglottis Posted at: 2017-08-13T16:28:54.801Z Reads: 684

```
[quote="solidgeek, post:140, topic:28543"]
I needed a way to turn of the boost converter while the battery still was connected to the charging circuit, otherwise, I would not be able to charge the battery, while the whole circuit was turned off. How did you solve this?
[/quote]

Why can't you charge the battery with the boost active? Is it the design of that circuit that doesn't allow it?

The booster circuit I'm using can charge the battery while boosting. In fact my design requires the nunchuck to be ON while charging so I don't have that problem.

1. push nunchuck button 
Solid state switch sensor input will be grounded and the switch will supply battery voltage to the booster circuit. 
2. The booster circuit will feed the arduino with 5V. 
	There is a feed back from the arduino to the solid state switch. The solid state switch need 3-5V on this feedback to remain active... if not... it will turn off.
When the solid state switch board is activated, it is possible to charge the battery using the USB input on the boost/charging board. Its charging an empty 400mAh lipo with 700mA. Maybe not optimal but its good enough for me.

If the solid state switch is not active, the battery is not connected to the circuit and i cannot charge. The charging/boost board would just indicate "fully charged"
In addition, I have implemented a couple of safety/ timeout features and there might be some pull up/down resistors at some places that I have not mentioned. I don't remember all the details in my head right now and my phone with all the documentation got lost :(  
Maybe this is all confusing but here is quick drawing and the mess inside the nunchuck :smiley: 

<img src="/uploads/db1493/original/3X/6/5/6550a72bb13234bf12b46a36dfc8641698716765.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/3/0/30cc8975580625b0e7d1fcad049dc179c0257937.jpg" width="629" height="500">

I can send you the code for the nunchuck and the board :)
/Simon
```

---
## \#144 Posted by: solidgeek Posted at: 2017-08-13T16:38:31.079Z Reads: 648

```
Nice build, I did make a Nunchuck remote just like that a year back, however, it was a lot messier than yours :joy: It's not easy to fit all that wire and electronics in such a small case! 

[quote="Fatglottis, post:143, topic:28543"]
If the solid state switch is not active, the battery is not connected to the circuit and i cannot charge. The charging/boost board would just indicate "fully charged"
[/quote]

That's exactly why I choose to use two different boards. I can charge my remote without having to turn it on, and the boost circuit will only draw current if the remote is turned on. A boost circuit uses a very small amount of current while connected - even though no current is drawn from it. 

I would like to see your code thanks :-)
```

---
## \#145 Posted by: Silverline Posted at: 2017-08-13T17:32:24.962Z Reads: 655

```
Just test printed

<img src="/uploads/db1493/original/3X/2/2/22112bed3b1456e95bf02dd532d02c2a5d85bbd8.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/7/275ffa0dfe73843a0d12cbc0fa78f055b61ac788.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/4/44bbae32783b88501d022461b3f487e68be850be.jpg" width="690" height="388">


I have to say that I still think it would be much cooler, to use the button as a "toggle switch" for various info pages on the screen. I dont get the "safety trigger thing"
To toggle between, batt level, speed, and distance would just be awesome :slight_smile:
I know that @DK-Odense thinks the same, he saw the remote today btw.  But it's your call, and your project. 
I´m looking forward to build this thing.... :slight_smile:
```

---
## \#146 Posted by: solidgeek Posted at: 2017-08-13T17:40:16.576Z Reads: 623

```
Looks amazing! Love the red color :P How did everything fit? 

I know a few of you guys don't love the safety trigger :(  ... and that's why I am making it possible to change between three settings for the trigger: Killswitch, Cruise control and the option to use it as a toggle switch for screen :-) 

I am working on a settings menu, and saving the settings on the EEPROM! This is also needed to change wheel diameter, cell count and motor poles (used to calculate speed, distance etc.)

EDIT: Love the rubber band, why didn't I ever think of that!!!
```

---
## \#147 Posted by: Silverline Posted at: 2017-08-13T17:44:42.560Z Reads: 625

```
Now we are talking :heart_eyes::sunglasses:

I had to file a little bit in the throttle and trigger hole, for a not so tight fit. But other than that, no problems. I think i`m gonna try printing the throttle wheel in tpu, to se if i will get me a little better grip feeling.

The rubber band is just temporary, so i could try it out :slight_smile: I dont think it would work nice in the long run :-)
I had some springs from an old gimball (RC remote) but it was to short....

Btw. I`m using the Metr app. at the moment on my VESC, and with the wheel diameter, cell count etc. dialed in,  it just works freaking awesome, i would love to have these features on my remote :-)
```

---
## \#148 Posted by: solidgeek Posted at: 2017-08-14T19:54:13.392Z Reads: 648

```
I found a nice way to enter the settings on the remote with only the throttle wheel. To enter the settings menu, you will have to give full throttle in 5 seconds, without clicking the trigger. However this only works, if the trigger is programmed to be used as a "kill switch". Otherwise, I would not have a way to differentiate between full throttle and "enter settings". To fix this, I would need a way to enter the settings, without using the throttle wheel, f.x. an extra button somewhere. 

It should be quite easy to add a small tactile switch to the top shell by simply drilling a hole, and gluing the switch in. 

https://www.youtube.com/watch?v=wRKT_dVo7CA

I have added VESC real-time data, however, I am having problems calculating the speed based on the ERPM. Does anyone have an idea of how the calculation should be made? I have tried RollingGeckos approach, but it doesn't seem to work very well.
```

---
## \#149 Posted by: lox897 Posted at: 2017-08-14T20:27:10.737Z Reads: 629

```
First, you must convert ERPM to RPM: 
RPM = ERPM / 7
Km/hr = radius (in metres) × RPM × 0.10472
```

---
## \#150 Posted by: Neilfenstein Posted at: 2017-08-14T20:38:00.578Z Reads: 615

```
Hi, that looks absolutely awesome. 

I was wondering if the trigger is set to cruise control or screen toggle could you not hold the trigger then push throttle for 5secs. It would save adding an extra button. 

I was wondering if we could help with development and improvements when we get the prototypes but you've got it all in hand and then some. 

Thanks for all your effort.
```

---
## \#151 Posted by: zeah Posted at: 2017-08-14T21:41:32.103Z Reads: 600

```
Thats really awesome!! Great work!! :clap::clap::clap:
```

---
## \#152 Posted by: solidgeek Posted at: 2017-08-14T22:22:03.932Z Reads: 629

```
@lox897 Thanks, but I believe I got a breakthrough. However, nothing like the calculation you came with :smile: . Why would you divide ERPM with 7 to get RPM? As far as I understand the VESC counts 1 ERPM for each back-emp it measures. So to calculate the RPM of the motor I believe it should be: 

> RPM = (ERPM) / (motorpoles * 3) 

So if I had a motor with 14 poles, the **RPM** of the motor could be calculated by dividing **ERPM** with 42. To calculate the speed from **RPM** is quite simple from there, that is if you know the gearing **ratio** and wheel diameter.

> Speed = (RPM * ratio * d * pi * 60) / 1000000

The wheel diameter **d** is in millimeters and **RPM** in minutes^-1. I then multiply with 60 to convert minutes to hours and lastly divide with 1000000 to get the result in km (1km = 1000000mm).  What do you think about my calculations, am I wrong?

@Neilfenstein thanks man :slight_smile: ! Yeah, I thought about that option too, but I believe it is too risky (could easily be activated while driving). However, instead of adding a new button I found another solution. My idea is that when the remote turns on it checks whether or not the trigger is active. If the trigger is active the settings menu are loaded, and if not it simply turns on normally. This way you can only access the settings if you restart the remote - do you think that's a problem?  

@zeah Thanks! I am glad you like it :-)
```

---
## \#153 Posted by: lox897 Posted at: 2017-08-14T22:38:26.212Z Reads: 601

```
I'm pretty sure you divide the ERPM by the number of pole pairs in the motor. Just copied it off @evoheyax 's thread so maybe he can input some advice
```

---
## \#154 Posted by: solidgeek Posted at: 2017-08-15T00:51:45.588Z Reads: 628

```
@lox897 Hmm I don't know, maybe the ERPM is different on a VESC 6? I am getting pretty accurate results with my current model at the moment. Would like to hear what @evoheyax thinks :-) 

I have updated the display a little further, with some "wifi" icons indicating the signal. I am pretty much pleased with the looks of it :smile:

<img src="/uploads/db1493/original/3X/d/9/d9b6f7e26ac882541211ba313de215b687b95d07.jpg" width="317" height="500">
```

---
## \#155 Posted by: oyta Posted at: 2017-08-15T06:57:42.225Z Reads: 600

```
My understanding is as follows:

The RPM is 
    RPM = ERPM / (_Number of motor poles_ / 2 )

Then multiply it with the gear ratio and circumference of the wheel and you will get the speed.

See one of Vedder's blog posts about designing the drive train: http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/ Note: he is referring to a maximum ERPM which is not valid for the VESC 6.
```

---
## \#156 Posted by: NAF Posted at: 2017-08-15T07:44:25.288Z Reads: 590

```
Yesss ..!! this is just awesome ...@solidgeek please count me in for testing. I am in Poland. I'd love to put my hands on this . By the way do you need some help with the graphics ?? I'd love to help with some custom designed icons I think it would look better instead of WIFI icon.

And by the way how is the signal ? is it reliable ? did you had any losses when riding in the city ?
```

---
## \#157 Posted by: lox897 Posted at: 2017-08-15T09:05:15.642Z Reads: 571

```
That's exactly what I said... Most motors have 14 poles so the number of pole pairs for mine was 7.
```

---
## \#158 Posted by: Maxid Posted at: 2017-08-15T09:15:42.827Z Reads: 583

```
I have sent the files to my printer guy - but will only get them back next week :cry:
In the meantime I was thinking about buying the rest of the parts.
@solidgeek: It would probably be easier if you could send me the required parts when you order them in bulk anyway.
Would that be possible (living in Germany btw)?
```

---
## \#159 Posted by: solidgeek Posted at: 2017-08-15T11:52:32.155Z Reads: 603

```
@oyta I don't really think Vedder is mentioning the ERPM to RPM conversion in the post? However, I think you are right. My calculation only worked because I calculated the gear ratio wrong. I calculated the ratio by dividing the wheel pulley with motor pulley, which makes no sense if I want to find the speed of the wheel. It should be the other way around: **ratio** = motor-pulley / wheel-pulley.

> RPM = (ERPM) / (motorpoles / 2) 

The speed can then be calculated in the same way as before

> Speed = (RPM * ratio * d * pi * 60) / 1000000

I just updated the remote software, and the speed seems to be precise :D !

@lox897 Yep :-) I would still like to know how the VESC measures the ERPM to clarify why the RPM is calculated like so :sunny:  

@Maxid That is a long wait time :open_mouth: !  Sure thing, no problem. I am still looking for good quality surpliers (mostly from China), so it probably takes around 3 weeks until I got all parts ready to ship.
```

---
## \#160 Posted by: Maxid Posted at: 2017-08-15T11:53:45.206Z Reads: 578

```
He is on vacation this week - that's why. Otherwise this would be done by tomorrow. But since it is the printer at work I am not complaining if I have to wait a little ;)
```

---
## \#161 Posted by: solidgeek Posted at: 2017-08-15T12:27:43.552Z Reads: 541

```
Thanks man! I have added you to the ever growing list of beta testers :P  I would love some help with the graphics, I have been drawing everything on paper (and manually created the bit strings) until I found that GIMP can export the right bit-string (called XBM) from a black/white image. 

The "connection/wifi" icon has three stages: No connection, connected and transmitting. It has to be within 24x32 px (width x height). Would love to see what you could come up with :slight_smile:
```

---
## \#162 Posted by: oyta Posted at: 2017-08-15T13:22:44.789Z Reads: 565

```
[quote="solidgeek, post:159, topic:28543"]
I don't really think Vedder is mentioning the ERPM to RPM conversion in the post?
[/quote]
He is not setting it up directly, but it is what he says in the following sentence:
[quote]
In my experience, these losses start to get significant around 60k electrical RPM, which for a 14-pole motor is about 8570 mechanical rpm
[/quote]
So I think you are on the right track now 😊😊

@lox897: Yes, true. Should be right.
```

---
## \#163 Posted by: evoheyax Posted at: 2017-08-15T15:31:58.576Z Reads: 560

```
sorry it took me so long...

Basically, 

erpm = rpm * # of pole pairs 

or... 

erpm = rpm * (# of magnets / 2)

Either works. I know this to be correct, as I use this formula for my app, VESC Status, and I have used them recently for calculating kv. (kv = max rpm/batt voltage, and in this case, your working with erpm, so it has to be converted). Everything is accurate with these formulas.
```

---
## \#164 Posted by: evoheyax Posted at: 2017-08-15T15:34:33.203Z Reads: 568

```
Since your doing speed, you'll need users to be able to input their wheel diameter and the number of pole pairs in their motor. Most are 7, but some of 14 or 12. Just a thought to keep in mind. The last photo looks great!
```

---
## \#165 Posted by: MontPierre Posted at: 2017-08-15T18:20:58.935Z Reads: 592

```
Parts parts lol 

<img src="/uploads/db1493/original/3X/6/2/6212cd336cbd4ecd08d99ef2a954d52859238689.JPG" width="666" height="500">
```

---
## \#166 Posted by: wmj259 Posted at: 2017-08-15T18:34:05.268Z Reads: 578

```
Another update if you didn't read closely, magnets come by X1 piece.  I thought it came in like x10+.
```

---
## \#167 Posted by: MontPierre Posted at: 2017-08-15T18:54:26.092Z Reads: 561

```
Well I found 10x, I don't mind having spares ;)
```

---
## \#168 Posted by: NAF Posted at: 2017-08-15T19:08:26.645Z Reads: 550

```
@solidgeek can you tell me whats the total screen size of the display ?? pixels x pixels size ?  I want to try some different graphics. Also what format ? GIF ? PNG ? JPG ?
```

---
## \#169 Posted by: Maxid Posted at: 2017-08-15T19:09:25.694Z Reads: 557

```
Format should be:
[quote="solidgeek, post:161, topic:28543"]
bit-string (called XBM)
[/quote]

I think
```

---
## \#170 Posted by: NAF Posted at: 2017-08-15T19:10:15.951Z Reads: 550

```
[quote="Maxid, post:169, topic:28543"]
XBM
[/quote]

OK got it. Do you know what's the total screen size in pixels ?
```

---
## \#171 Posted by: Maxid Posted at: 2017-08-15T19:11:41.267Z Reads: 546

```
He mentioned it further up:
[quote="solidgeek, post:13, topic:28543"]
OLED LCD (128x32px)
[/quote]
```

---
## \#172 Posted by: solidgeek Posted at: 2017-08-15T19:29:02.331Z Reads: 583

```
Okay thank you :-)! I have already added the option to enter wheel diameter and number of motor poles (magnets). The calculation of speed and distance is now working. 

I am calculating the distance based on the tachometer value, would you mind checking if my calculation are correct? (poles are equal to the number of magnets).

_ratio = motor-pulley / wheel-pulley_

_distance = ((tachometer / (3 * poles)) * ratio * d * 3,14159) / 1000000_

<img src="/uploads/db1493/original/3X/5/c/5ca1f70133a2b636fc4d7166f1405168ad0eaf3b.PNG" width="449" height="155">

Or simplified to a constant multiplied with the changing tacho-value

<img src="/uploads/db1493/original/3X/0/5/059f9767a75336c68513498fbad57f48e9a9a3ab.PNG" width="504" height="129">
```

---
## \#173 Posted by: MontPierre Posted at: 2017-08-15T19:31:09.663Z Reads: 575

```
Also graphics need to be in 8bit mode up to 128x32 size or smaller like icons for example - black and white only and saved as .bmp file which he can later convert to hex/C array.

https://youtu.be/cURh2-dTuI0?t=1m54s
```

---
## \#174 Posted by: solidgeek Posted at: 2017-08-15T19:31:50.738Z Reads: 577

```
@NAF I see @Maxid was faster than me :P You can see how the screen looks in this video:

https://youtu.be/ik0lJ54-LWc

@MontPierre Excatly :slight_smile:
```

---
## \#175 Posted by: MontPierre Posted at: 2017-08-15T19:33:31.813Z Reads: 561

```
Would spinning of the motor in the air add milage ?
```

---
## \#176 Posted by: NAF Posted at: 2017-08-15T19:36:52.452Z Reads: 552

```
Thanks guys !! I got everything !
```

---
## \#177 Posted by: solidgeek Posted at: 2017-08-15T19:39:18.422Z Reads: 559

```
@MontPierre Yeah no way around that  :wink:

@NAF Looking forward to see what you come up with :smile:
```

---
## \#178 Posted by: lox897 Posted at: 2017-08-15T20:24:32.575Z Reads: 593

```
If you need help designing the graphics hit me up because I've done it before. Hopefully you're using Windows, or if you want to convert it to a hex array you'll have to run the program on wine or a VM.

<img src="/uploads/db1493/original/3X/9/e/9e6e17cdca60c516862315b90e77b4e2786f6c28.JPG" width="375" height="500">
```

---
## \#179 Posted by: MontPierre Posted at: 2017-08-15T21:35:37.889Z Reads: 572

```
Can't get my screen to work, maybe it's defective. Voltage is on vcin pin ( 5V) and I think i connected it correctly - a5 and a4 pins on Nano. Got the libraries, everything compiles and uploads. Nothing on the screeen. I'll wait for more screens to arrive and try again :)
```

---
## \#180 Posted by: solidgeek Posted at: 2017-08-15T21:42:34.855Z Reads: 573

```
Maybe you connected the I2C wrong? This is how it has to go:

SDA = Pin A4
SCL = Pin A5

If this isn't working you could try using an I2C-scanner (I think Arduino comes with a sketch for this by default).
```

---
## \#181 Posted by: MontPierre Posted at: 2017-08-15T21:45:51.392Z Reads: 516

```
Yeah I tried ic2 scanner - I get unknown error and then 0x and few values .... ic2 was connected correctly.
```

---
## \#182 Posted by: solidgeek Posted at: 2017-08-15T21:56:54.298Z Reads: 524

```
Well if the I2C scanner doesn't work, I think you are right. The screen probably is defective :/ I will try to run an I2C scanner on a spare OLED display I have, to see if it can find that :-)

EDIT: My spare works just fine, tried to use the I2C scanner and got the address: I2C device found at address 0x3C. Yours are probably defective :/ ! How you used good wire, and checked if there a signal through all four cables (with a multimeter)?
```

---
## \#183 Posted by: MontPierre Posted at: 2017-08-15T22:24:30.328Z Reads: 527

```
Ive check and had voltage on one out of two wires ( SDA I think) . I wasn't to precise with multimeter there might have been voltage on second one but anyway I have up ;) in couple of weeks I'll get a new oleds ;) no worries. Or might order one from eBay for double the price of China import ;)
```

---
## \#184 Posted by: Ackmaniac Posted at: 2017-08-15T22:35:57.477Z Reads: 526

```
speedDevider = magnets / 2 * wheelPulley / motorPulley / (wheelSize * 3.14159265359 / 1000) * 60 / 3.6;
distanceFactor = (wheelSizeInMM / 1000) * 3.14159265359 / (wheelPulley / motorPulley) / magnets / 3;

speedInKm = ERPM  / speedDevider
speedInMi = ERPM  / (speedDevider * 1.609344)
distanceInMeter = tachometerAbs * distanceFactor
distanceInKm = tachometerAbs * distanceFactor / 1000
distanceInMiles = tachometerAbs * distanceFactor / 1609.344
```

---
## \#185 Posted by: solidgeek Posted at: 2017-08-15T22:53:51.395Z Reads: 514

```
Thanks @Ackmaniac! I am curious if you got all the parenthesis right? Could you write them in some kind of math program, to better visualize the equations? Where does the 3.6 come from? :D
```

---
## \#186 Posted by: Ackmaniac Posted at: 2017-08-15T22:55:07.029Z Reads: 515

```
for calculation from meter per second to km per hour
1hour = 3600 seconds
```

---
## \#187 Posted by: solidgeek Posted at: 2017-08-16T00:43:48.306Z Reads: 551

```
Ohh okay, I think it's a very nice, but however very complicated equation you got - how did you deduce it :P ? I tried your equation, and it gives the exact same value as mine. So it seems that there are two solutions to the same problem - nice ;)! Good to have something to choose between. 

<img src="/uploads/db1493/original/3X/6/5/65a186e4da5f3dbd352f9ece370910442fc6f1ba.PNG" width="690" height="185">

Your method to calculate distance works great too, however, I think I prefer my own. Feels a little simpler to me.  

<img src="/uploads/db1493/original/3X/8/e/8ed371d0dd6ba684dd552eb1ebb902ba5d612ef7.PNG" width="690" height="240">

Thanks for the input :slight_smile:
```

---
## \#188 Posted by: Kookaburra Posted at: 2017-08-16T06:05:08.647Z Reads: 517

```
Did a Little bit of mathematical reformulation and can confirm that both Solutions are interchangable...except of the tens potency ;) 

Btw. take my application as a potential tester. Mechatronic Engineer from Germany with 3D Printer and programming experience.
```

---
## \#189 Posted by: Ackmaniac Posted at: 2017-08-16T10:10:42.776Z Reads: 510

```
Another issue you will come across is that BLDC gives you correct tachoAbs and FOC not (10% - 15% off) with the standard 2.18 firmware. In my firmware mod 2.54 this issue is fixed.
```

---
## \#190 Posted by: NAF Posted at: 2017-08-16T10:47:10.628Z Reads: 504

```
I am going to post a few concept screens I did this morning. I have redesigned pretty much everything :) So I hope you don't mind.
```

---
## \#191 Posted by: Ackmaniac Posted at: 2017-08-16T11:02:56.206Z Reads: 537

```
I just had a look at your throttle calculation and it isn't correct. Problem is that when the center position isn't exactly in between the max and min analog readings it will overshoot the min or max and underestimate the other side.
Means you will loose throttle range in one direction and wont be able to have full output in the other direction.

e.g. center is at 500, max at 600 and min at 300 then you calculate the offset as 50 ( 500 - ((600 + 300) / 2) )
when the throttle input is now 500 = center then you get 127.5 as output which is correct
but when you have a throttle input of 600 = max you get 212.5 as output which isn't 255
same for 300 = min as input which results in -42.5 and not 0

Long story short. If your analog readings detect bullshit only one time (for example when the remote passed another magnet) your remote becomes dangerous. And if you switch on the remote and have it at full brake while you switch it on your board will run off ones you release the brake because you detect the center position at startup.

I leave you with that homework
```

---
## \#192 Posted by: NAF Posted at: 2017-08-16T11:11:35.156Z Reads: 507

```
[quote="Ackmaniac, post:191, topic:28543"]
Long story short. If your analog readings detect bullshit only one time (for example when the remote passed another magnet) your remote becomes dangerous.
[/quote]

That's some serious stuff :confused:
```

---
## \#193 Posted by: Fatglottis Posted at: 2017-08-16T12:24:17.608Z Reads: 527

```
Ackmaniac has good feedback!

The quality of the throttle sent to the vesc is cruisal. I have learned it the hard way through the development phase of my board haha!

In my nunchuck design, I have added an accFactor to the analog readings from the throttle. I can thereby cycle through different accFactors while I'm driving.. and thereby get different acceleration profiles. I find it more secure to be able to cruise around with low torque and only use the boards full potential in areas where I can handle it.

simple example of equation:
Throttle sent to VESCs = 127  +  (Y_axis - 127)/accFactor.   (where Y_axis = 255 at full throttle)

Increasing the accFactor will decrease the amount of throttle that can be sent to the VESCs, still being able to use the whole throttle range of the nunchuck. 

I also do not allow throttle unless the wheels are spinning for extra safety. This means no start from stand still but I always push away anyway.

Right now I try to figure out how to handle a situation of signal loss or corrupt data. Not sure how I want it yet.. it all depends on how i ride the board when the data loss occurs. Sending zero throttle to the VESCs during a loss at constant speed is okay but NOT during acceleration.. That is scary :O. 

I will create a smooth ramp down of the throttle at that point... and if there is data again.. not allow full power immediately since I wont be ready for it. 
It will be amazing :slight_smile:
```

---
## \#194 Posted by: Ackmaniac Posted at: 2017-08-16T12:46:19.043Z Reads: 497

```
Well,
if you only allow throttle when the board is rolling then that will make it more dangerous.
For example the remote want's to go full throttle because of a problem you only will find out when you stand already on the board. 
Throttle ramping makes it on the one side safer but on the other side also less safe. Because if you need to make a full brake you loose meters until it ramped down. And i like a direct throttle instead of a softened throttle. But that is personal preference.
And ramping is already included in the nunchuk software of the VESC. Mostly i disable it.

Actually that makes me think about to improve the failsafe of the VESC itself. There a slow ramping would make a lot of sense. But sadly the PPM users will not benefit from it because the receiver sends a default signal when the connection is lost. Only when the receiver also dies it would work. And a slow ramping back to the actual throttle if the connection is back after a timeout. Fuck that idea is great and it will prevent a couple of broken bones and brains.

Time to earn some more karma points :innocent:
```

---
## \#195 Posted by: solidgeek Posted at: 2017-08-16T13:43:10.820Z Reads: 521

```
[quote="Ackmaniac, post:191, topic:28543"]
Long story short. If your analog readings detect bullshit only one time (for example when the remote passed another magnet) your remote becomes dangerous.
[/quote]

I am not sure that I agree. When the remote boots, it gets an average reading for the Hall sensor in its center position. This value will always be the center. However, the placement of the Hall sensor and the quality of magnets will, of course, make the min and max value different from remote to remote. This means that the value from center to max isn't necessarily the same as from center to minimum. Therefore I calculate the offset value, which is used to keep the throttle value at 127 (in neutral position) even though the max and min don't span over the same. 

Sure if you get a much higher max value than the minimum value, the braking resolution would be lower, however, you will still be able to do a full brake (<0) and release the throttle to the neutral position (127). The only thing affected would be the max throttle value (because I minus the offset). I have done this because I think it is more important to be able to do a full brake and get a neutral value of 127 in the center position. It's not a perfect solution, however, if you got a better way I would love to hear it :-) 

I agree that constantly updating the min and max value, could be problematic if you entered a very powerful magnetic field (however the max value would never be over 1023). Maybe I should instead make a calibration option, so the min and max are remembered in the settings - and doesn't update while using the remote. Regarding the calibration at startup, what else would you propose? It isn't that hard to not use the throttle while the remote is turning on :-)
```

---
## \#196 Posted by: Ackmaniac Posted at: 2017-08-16T13:47:27.212Z Reads: 512

```
The same issue is in your code for braking. So if the center is at 500 and the max 800 and min 400 then at 400 you only get a value of 63,75 and not 0. So the brake would be only roughly at half.
And at switch on it is easy to accidentely touch the throttle and when you release it the board goes flying.

To gain some more karma points you should give this a try

    if(hallMeasurement >= hallCenter){
        hallSpeed = constrain(map(hallMeasurement, hallCenter, hallTop, 127, 255), 127, 255);
    }else{
        hallSpeed = constrain(map(hallMeasurement, hallBottom, hallCenter, 0, 127), 0, 127);
    }

and set fixed values for center, max and min. And make them changable with a calibration via the menu
```

---
## \#197 Posted by: Norrmalm Posted at: 2017-08-16T14:02:20.444Z Reads: 486

```
Hi! Awesome work! I'd like to be a beta tester too if possible. I have a spare VESC 4 you could loan if you still need one for testing (I'm in Sweden).
```

---
## \#198 Posted by: Fatglottis Posted at: 2017-08-16T14:04:03.049Z Reads: 527

```
[quote="Ackmaniac, post:194, topic:28543"]
if you only allow throttle when the board is rolling then that will make it more dangerous.
For example the remote want's to go full throttle because of a problem you only will find out when you stand already on the board
[/quote]
No worries, I'm able to test the board from standstill if I want. Just pulling the stick to the right during startup will allowing throttle at standstill ;). I just want to avoid the following scenarios: 
* Racing the board away into the traffic like a RC car without me.
* Spinning the motors accidentally while carrying, destroying my jacket

[quote="Ackmaniac, post:194, topic:28543"]
Throttle ramping makes it on the one side safer but on the other side also less safe. Because if you need to make a full brake you loose meters until it ramped down.
[/quote]
Let's say you have a loss at zero throttle (or a little brake), then it would be nice with a ramp. I already have it and it is smooth. It makes you first realize something is wrong and then more and more braking force is applied. You stop quick enough and if not, then you have lowered the speed enough to jump off without falling to the ground

[quote="Ackmaniac, post:194, topic:28543"]
And i like a direct throttle instead of a softened throttle. But that is personal preference.
[/quote]
I don't mean the throttle to be softened like turbo delay. I just make the board weaker so that if I throttle to hard by accident, I won't fly off :slight_smile:

In the scenario when you are throttling its harder to have a good fail safe.
In earlier design I had lots of communication issues (bad soldering) so I increased the amount of time a loss could be allowed. I then kept the throttle at the last successful received data. This is not a good solution since tapping short on the throttle and having a loss at the same time would cause the board to fly away when you don't expect it.

In a scenario with a loss at low speed and high throttle, I would make the positive throttle decrease before breaking. Too quick change of torque is what makes me flying

In a scenario with a loss at close to max speed, I think the throttle could decrease faster since less positive torque would be applied to hold the current speed. Better to slowly apply breaking force.. its less likely you need to panic brake when running at full speed.
```

---
## \#199 Posted by: solidgeek Posted at: 2017-08-16T18:52:57.736Z Reads: 479

```
Thanks @Ackmaniac, and of course you are right! I just never had any issues, probably because my Hall Sensor sits firmly in the middle :slight_smile: ! I will try to implement your code as soon as I get it tested - and I am working on a calibration menu for fixed min, max and center values :-) 

Thanks for the example!

@Norrmalm I think we got room for a couple more :P ! I have added you to the list!
```

---
## \#200 Posted by: MontPierre Posted at: 2017-08-16T19:23:41.304Z Reads: 487

```
Is the part list up to date ? I know you have been looking into boost + overcharge board instead of boost only.  have ordered most of the parts already, just making sure nothing has changed in the meantime. 

I'm hardcore - I'll wire it up and solder myself haha! 💪🏻🤣no need for prototype 😂

Would you have wiring schematics somewhere to share ? Otherwise I'll be happy to trace wires on the pictures of the build. I rather keep same wiring as you so I don't have to change pins in the code. 

Btw are you making custom pcb to connect all parts together rather than using wires?
```

---
## \#201 Posted by: solidgeek Posted at: 2017-08-16T21:31:41.416Z Reads: 480

```
The part list should be up to date, however, for the prototypes, I will be using a different boost converter (a little smaller) and an Arduino Nano with a dedicated 3.3V voltage regulator. This is because the standard Arduino Nano really can't deliver more than 25mA at a stable 3.3V (comes from the serial to USB chip), and the nRF24 modules with PA and LNA can use up to 45mA (depending on the settings). You could just add a big ass capacitor on the 3.3V rail, however, it's a more reliable solution to use a dedicated 3.3V regulator/power supply. 

This is the Nano I will be using: https://www.aliexpress.com/item/Nano-V3-ATmega328-CH340G-Micro-USB-Pin-headers-NOT-soldered-Compatible-for-Arduino-Nano-V3-0/32664577152.html

And this is the boost converter: http://www.hobbytronics.co.uk/u1v10f5-5v-regulator

I had plans about making a PCB mainly for making the soldering process easier, however, I haven't even received a notice about them being shipped yet... Sooo let us see :smiley: Also the PCB I ordered where made for the Pro Mini, and I think I will stick with the Nano because of its easy to use USB connector. 

@NAF Are we going to see your concept screens or what? ;) :smiley:
```

---
## \#202 Posted by: MontPierre Posted at: 2017-08-16T21:53:46.713Z Reads: 480

```
Cool!

I've ordered this V3 Nano:

https://www.ebay.co.uk/itm/161784434085 

It looks different to yours but I think specs are the same... same chip and Micro controller... am I right? 

I'll see if boost covcerter with over charge protection will fit inside ;)
```

---
## \#203 Posted by: solidgeek Posted at: 2017-08-16T22:00:48.642Z Reads: 488

```
Well, it is the same chip and micro controller, however not exactly the same board. The one I linked got a dedicated 3.3V voltage regulator, and a micro USB. The Arduino Nano (clone or not) doesn't have this, only a 3.3V output from the serial to USB chip. You could buy a dedicated 3.3V regulator f.x the LD1117-3.3 or a small bulk converter to achieve the same.

I think it is important that the nRF24 can draw as much current as it needs.

What boost converter with charge protection are you talking about? :D
```

---
## \#204 Posted by: MontPierre Posted at: 2017-08-16T22:12:10.317Z Reads: 494

```
I think that's one of your links - with charge protection 
http://s.aliexpress.com/b6vYfAze
```

---
## \#205 Posted by: solidgeek Posted at: 2017-08-17T00:09:46.502Z Reads: 524

```
I am sorry but I wrote that this module didn't work. They are "falsely" advertised as a boost and charger module, however, they only work as charger and boost converter WHEN an input voltage is applied. If you look at the traces of the PCB the battery is ONLY connected to the charger circuit. This means the battery voltage doesn't get boosted, only the input voltage.

Weeeell you could make it work by using a two position on/on switch, and some soldering (not tested!).

<img src="/uploads/db1493/original/3X/d/8/d8a1a545108a4b7a03d9c333d555c0b5c45c0b02.PNG" width="637" height="378">

This however, would make it impossible to charge the remote, while it is turned on.
```

---
## \#206 Posted by: lox897 Posted at: 2017-08-17T00:16:13.960Z Reads: 506

```
You sure you got the I2C address right? A lot of the time I didn't have anything displaying on my OLEDs and it was simply errors in the code.
```

---
## \#207 Posted by: solidgeek Posted at: 2017-08-17T00:59:50.803Z Reads: 494

```
Also you could try to change the U8G2_SSD1306_128X32_UNIVISION_1_HW_I2C in the sketch to U8G2_SSD1305_128X32_NONAME_F_4W_HW_SPI. Maybe your OLED is different from mine (I got mine from a local supplier).
```

---
## \#208 Posted by: MontPierre Posted at: 2017-08-17T07:56:46.419Z Reads: 489

```
@lox897 I have tried to get ic2 address but no luck. 

@solidgeek possibly I have different oled screen, I'll try to change the settings in the code.
```

---
## \#209 Posted by: lox897 Posted at: 2017-08-17T10:16:29.622Z Reads: 465

```
There's an Arduino script that scans connected I2C devices. You could try that. Can you send a few pictures of your OLED code parts and wiring?
```

---
## \#210 Posted by: MontPierre Posted at: 2017-08-17T11:03:50.131Z Reads: 468

```
I have tried the script- got "unknown error  0x"as one of the posts above. I'll take pictures later on as I'm at work now :/
```

---
## \#211 Posted by: lox897 Posted at: 2017-08-17T13:23:16.015Z Reads: 478

```
I believe the usual address for clone displays is 0x3f or 0x3c
```

---
## \#212 Posted by: NAF Posted at: 2017-08-18T08:03:26.096Z Reads: 514

```
@solidgeek

Ok so here is my take on the menu. We have very small screen so what I suggest is we need to make the menu easy to ready while riding the board. At a quick glimpse everything is big enough to read. The only Icon that I kept on all of the screens is the remote SIGNAL icon. 

1.The small bar on the left with tiny dot -indicates where we are in the menu. 
2.First icon on the left is the icon of the category we are in.
3.Than we have clear potentiometer for each of the category.
4. The last thing are the big numbers easy to read. 

<img src="/uploads/db1493/original/3X/4/c/4cfaeb2cb6c71d3a5a619203f4ac223fca2799d6.jpg" width="400" height="300">
```

---
## \#213 Posted by: solidgeek Posted at: 2017-08-18T10:20:30.457Z Reads: 487

```
@NAF Amazing job dude! It looks very professional and modern, I like it! I will try to implement it the best I can today. 

I am ordering the rest of the parts today (just found some good suppliers). I hope to have the first batch (10 pieces) of prototypes ready in the beginning of September :slight_smile:
```

---
## \#214 Posted by: NAF Posted at: 2017-08-18T19:33:13.362Z Reads: 474

```
@solidgeek - thanks dude ! I can prepare all the icons ..and cut them out for you and save them as BMP files ..question is how do we use the numbers ? Do you want me to cut them out from 1 to 10 ..like 1 . 2. 3. 4 and so on ? 

Anyway ..I'd love to design the rest of the menus ..but what I am thinking is that people who want complex infos they use IPHONE or ANDROID apps where they get a lot of data ..but with this small remote it would be cool to only have the basic screens and get rid of unnecessary screens. What other screens could I prepare ?
```

---
## \#215 Posted by: solidgeek Posted at: 2017-08-18T20:21:31.145Z Reads: 470

```
I would love the icons, however the rest I can make myself with software :-) The numbers I just print by using a bigger font - no problem! I am not sure if we need more screens, maybe something with amps drawn / current motor amp?

If you got some idea for the settings menu, I would love to see them too!
```

---
## \#216 Posted by: NAF Posted at: 2017-08-18T20:22:58.574Z Reads: 455

```
Settings !! That's a good idea ..and true ..amps would be useful too.
I will do both of them.
```

---
## \#217 Posted by: solidgeek Posted at: 2017-08-18T20:24:33.347Z Reads: 469

```
Sounds great, I will begin to implement the menus now :slight_smile:

Btw I can see that your icons aren't only black and white. Some of the pixels are in between (gray). The icons can't have gray, as the display can't show half light at a specific pixel.
```

---
## \#218 Posted by: NAF Posted at: 2017-08-18T20:26:16.691Z Reads: 472

```
I know but don't pay attention to that ..final version will have only white ..no grays. It's just a quick sketch.
```

---
## \#219 Posted by: solidgeek Posted at: 2017-08-18T20:40:12.493Z Reads: 493

```
Okay cool, I just had a thought. I think it is crucial that one can see the throttle value at all times. So maybe instead of the battery and the nice distance icon, we simply put the same speedometer that is on the speed page? :slight_smile:  

In this way you will always know how much throttle you are giving, and still being able to distinguish between the different pages.
```

---
## \#220 Posted by: NAF Posted at: 2017-08-18T20:55:27.647Z Reads: 479

```
Hmm...ok let me think about it. I think I have nice idea for that. I'll come back tomorrow with something.
```

---
## \#221 Posted by: lox897 Posted at: 2017-08-18T21:15:33.531Z Reads: 450

```
Did you already mention if you are using the Adafruit or U8GLIB? Pretty sure Adafruit's has a higher refresh rate but it might be the other way around. It's also much easier to set a variable for a travelled distance and print it on the screen IMO.
```

---
## \#222 Posted by: solidgeek Posted at: 2017-08-18T21:19:35.748Z Reads: 461

```
I use the U8G2 library. I like it because I can control everything, and it doesn't take up as much space as the Adafruit library :slight_smile: I agree that the Adafruit library is easy to use, and maybe the refresh rate is better? However the refresh rate is more than enough - so I will stick with U8G2 :P
```

---
## \#223 Posted by: wafflejock Posted at: 2017-08-18T21:36:43.298Z Reads: 475

```
But can it play crysis?
```

---
## \#224 Posted by: solidgeek Posted at: 2017-08-18T21:39:40.216Z Reads: 506

```
It's preinstalled. 

<img src="/uploads/db1493/original/3X/4/4/44070fbd9acd07b904e8a95b73426132c7719106.jpg" width="500" height="365">
```

---
## \#225 Posted by: solidgeek Posted at: 2017-08-18T22:22:50.874Z Reads: 508

```
Just tried something myself, with a new speedometer bar, and removed the icons to make space for a miniature battery indicator (for the remote). I like how it came out what do you think? :slight_smile: 

<img src="/uploads/db1493/original/3X/a/6/a619a10f42bbdae4b6f591fe4e5af059d6df12c2.png" width="400" height="400">

The throttle bar under the text "Distance" begins from left then accelerating, and from right then braking, while the sticks increase in height according to the value.
```

---
## \#226 Posted by: MontPierre Posted at: 2017-08-18T22:47:23.478Z Reads: 513

```
@solidgeek Looks wicked !! Simple and slick!

What about connection icon being smaller, to free up a space for voltage meter ? I think voltage meter in the corner would very useful. The connection icon can be:

Small empty circle for no connection
Small filled circle for establishedconnection 
Blinking empty Circe for "connecting" ? If there is such state in the code... ;)

Just an idea. Keeping eye on Voltage as we all know is very important in eks8 ;)

Edit:

One more idea- small vibrator to alert on low remote battery ( 15-20%) ? This way we could perhaps free up more space on screen ;)  or use it for let's say other alerts : low voltage on the board, faults from vers (not sure if possible) etc. 

Here is one after quick google. Tiny but with more research there could be smaller ones ;)


https://shop.pimoroni.com/products/vibrating-mini-motor-disc?utm_medium=cpc&utm_source=googlepla&variant=1038384249&gclid=EAIaIQobChMI882A7e7h1QIV5p3tCh17AAMKEAQYASABEgKdVfD_BwE
```

---
## \#227 Posted by: MontPierre Posted at: 2017-08-18T23:08:30.599Z Reads: 485

```
Ohhh btw, will remote work fine with @Ackmaniac watt mode in terms of displaying values from vesc?
```

---
## \#228 Posted by: solidgeek Posted at: 2017-08-19T00:00:19.461Z Reads: 491

```
The voltage will be displayed on the battery page, so I am not sure if it is necessary to show the voltage on every page? Currently, there are three pages:

* Speed
* Distance
* Battery

The remote will loop through these pages every 3 seconds or so unless you set the trigger as "Data toggle" then it will shift every time you press the trigger.

I have no idea how @Ackmaniac watt mode works, I have never used it. But it could probably be added at some point :slight_smile:
```

---
## \#229 Posted by: chinzw Posted at: 2017-08-19T07:29:28.878Z Reads: 478

```
@solidgeek 
I think this project would really benefit from the Adafruit M0 Proto (https://www.adafruit.com/product/2772)
Its smaller than a nano and comes with integrated lipo charger/booster and usb.
I have a few, ill try to modify your remote to fit the m0 and an nRF24L01+
```

---
## \#230 Posted by: MontPierre Posted at: 2017-08-19T13:24:14.732Z Reads: 473

```
Give it a try! He's throttle curve works amazingly together with watt mode. I don't think I'll ever go back to any other firmware. Smooth throttle control! 

@Ackmaniac could you tell if your firmware would work well with this remote ?
```

---
## \#231 Posted by: solidgeek Posted at: 2017-08-19T13:46:07.160Z Reads: 471

```
Well if the firmware works with a standard PWM signal and doesn't change the tachometerAbs value then it should work just fine :-)
```

---
## \#232 Posted by: solidgeek Posted at: 2017-08-19T14:09:33.334Z Reads: 498

```
The Adafruit Feather are awesome, however as far as I understand they operate at 3.3V. The only thing using 3.3V in the remote is the nRF24 module, while the OLED and Hall Effect sensor requires 5V. The OLED could be supplied by a separate 5V boost converter, however, the Hall Effect sensors max output would be too high for a 3.3V logic, so a voltage divider would be necessary. It should, however, be possible to find a Hall Effect sensor working at 3.3V. 

The Adafruit Feather could surely be a cool substitute of the Nano, TP4056 and boost circuit. I am looking forward to see your modifications :slight_smile:
```

---
## \#233 Posted by: chinzw Posted at: 2017-08-19T17:44:32.615Z Reads: 477

```
@solidgeek, the hall effect sensor works fine with a 3.3v source, it's out of spec but works fine and it's ratiometric so it's output is proportional to the input. Adding a tiny 5v step up would be very easy for the screen
```

---
## \#234 Posted by: solidgeek Posted at: 2017-08-19T22:28:11.318Z Reads: 501

```
Well you are probably right, however, I am sure there is a reason why the min voltage is 4.5V. The output might be unstable or unable to detect the same min and max values, and I don't think that's an option then driving 40km/h on a skateboard. Using the Hall sensor out of specs only adds another way to face the asphalt :grimacing:

I think a better solution would be to find a Hall Sensor that is working correctly (within it's specs) at 3.3V, or simply find a way to supply it with 5V :-)
```

---
## \#235 Posted by: Maxid Posted at: 2017-08-24T12:14:00.510Z Reads: 517

```
<img src="/uploads/db1493/original/3X/a/1/a1af688a6deefe18ad3cde7f6d00cc0d9ca732e2.jpg" width="375" height="500">
Let's do this

A couple of thoughts: a sort of lip on the sides would be good to have so that the halves fit together without a wobble even when not screwed together.
Also I'd prefer screws with nuts on the opposite side instead of cutting a thread in the plastic - that would make reopening a lot easier.
```

---
## \#236 Posted by: chinzw Posted at: 2017-08-25T17:42:40.469Z Reads: 492

```
I ordered a few sensors (TI DRV5053 variants with different sensing ranges) these are 2.5-38v input and 0-2v output so well within spec. Ill try and print a case this weekend and give it a try! I ordered a oled screen as well, 3.3v operating voltage as well :slight_smile:

OLED consumes ~20ma
NRF consumes ~15ma
And the proto m0 can provide 500ma regulated 3.3v, i think this might work very nicely
```

---
## \#237 Posted by: wafflejock Posted at: 2017-08-25T18:27:20.523Z Reads: 493

```
Regarding the screws can also just put a retaining nut into the plastic so you don't need to have screws on one side and nuts on the other, just boolean/extrude/cut out a cube slightly bigger than the nut from the cylinder of plastic the screw goes into.  Can also widen out the holes themselves in that case and let the screws freely drop through the holes until they get to the retaining nut did this with my remote and it worked well I only have 1 screw on mine though so it can be swiveled open pretty easily which is good for tweaking things and charging since I didn't put a charge circuit in the last one I did think you could get away with just 2 screws for closing the case though especially with a lip added.
```

---
## \#238 Posted by: wafflejock Posted at: 2017-08-25T18:30:52.610Z Reads: 501

```
I have almost the same guts in my controller except minus the OLED and using a 800 mAh battery it lasts incredibly long, have left it on by accident overnight a few times and was still pretty well charged, your numbers are pretty accurate, the nrf chip plus arduino for me was consuming between 18-20mA.  Actually speaking of leaving it on overnight not sure if that's in the code already but might be good to add in some stuff about excessively long times without input to just shut off the radio at least (not sure what you could do in terms of lowering power consumption of the arduino too but it's pretty negligible itself anyhow).
```

---
## \#239 Posted by: Maxid Posted at: 2017-08-25T18:42:50.583Z Reads: 488

```
Well there is an interrupt based sleep on arduinos:
https://playground.arduino.cc/Learning/ArduinoSleepCode

not sure if the nano can actually benefit from this.
```

---
## \#240 Posted by: MontPierre Posted at: 2017-08-25T18:47:22.144Z Reads: 483

```
@solidgeek  BTW guys, would you know if there is option for implementing a long press of a button to switch on and off the remote ? Most of today's devices have this as standard and I think it would be better than the actual switch. I think it would be more hardware based than code based. Any thoughts ?
```

---
## \#241 Posted by: wafflejock Posted at: 2017-08-25T19:08:00.194Z Reads: 481

```
Have some examples of devices that use long press to turn on and off?  Only things I can think of is phones or tablets really but in the case of shutdown it's a long press to activate the shutdown confirmation screen.  On startup they will use a short press to show battery charging or life and long press to turn on but in that case they must be using some power to run a timer and then I imagine they are using a FET to actually open or close power to the main cpu/mcu (I'm speculating here).

Only thing I can find that would do this without keeping the arduino itself powered up to monitor the button press seems pretty big: http://www.ebay.com/bhp/time-delay-switch

Doing the going to sleep part based on a delayed button press from the arduino itself wouldn't be too hard but actually shutting off and then doing the startup without some clock running won't really work as far as I can tell.
```

---
## \#242 Posted by: chinzw Posted at: 2017-08-25T19:09:33.338Z Reads: 497

```
This can be done, but its not the most efficient way. Of the top of my head, this should work:
<img src="/uploads/db1493/original/3X/7/b/7be117c4ce9029564c77a07740f8066fbcfe754c.jpg" width="500" height="347">

The switch turns the transistor, which powers the arduino, the arduino sets A01 high, which overrides the switch and keeps power flowing.
For shutdown just need to set A01 low, which can be done by connecting the switch to one of the arduino inputs and reading its value.
```

---
## \#243 Posted by: MontPierre Posted at: 2017-08-25T19:24:56.834Z Reads: 490

```
My maytech remote has a button for on and off - longpress. And it works amazingly. If maytech can do it, I'm sure @solidgeek can 😜.

I googled it and as you mentioned it might be fets.
```

---
## \#244 Posted by: wafflejock Posted at: 2017-08-25T19:33:57.998Z Reads: 511

```
Don't turn it on take it APAAAART :)

---

http://www.eevblog.com/images/shirts/TakeItApart-20.jpg

---

http://easy-electronics4u.blogspot.com/2012/02/simple-dc-timer-using-mosfet-onoff.html

^^ Think this is similar to what @chinzw sketched up above but doesn't include the arduino part but pretty sure that would just be controlling one of the "switches" using a BJT maybe... really in any case I think this is a fair amount of extra complexity if you aren't baking all the stuff onto a single PCB.  Would be interested to see pictures of the guts of the controller that does this though.
```

---
## \#245 Posted by: MontPierre Posted at: 2017-08-25T19:51:37.074Z Reads: 510

```
Haha!

Well I found its guts here 

https://hiveminer.com/Tags/maytech

One one of the pics you can see in upper left corner on the board the momentary switch- it turns it on and off.


<img src="/uploads/db1493/original/3X/3/2/32ea77f8654e80c34710dcbfab5783191206a3a4.JPG" width="500" height="500">

Actually pics of the guts might be slightly different to current model. Mine doesn't have side switch like on above pic here ( which I think originally was to switch remote on and off). I might take mine apart to see how it looks now.
```

---
## \#246 Posted by: wafflejock Posted at: 2017-08-25T20:03:36.629Z Reads: 492

```
Hmm yeah hard to see what that momentary button is hooked to but I don't see any NE555 timer ICs on there either so I would guess they're using something akin to the circuit in the previous post.  I haven't really used surface mount FETs or BJTs only the through hole kinds but they have 3 legs so think some of those small black packages on the board with 3 pins could be one or the other (could also be voltage regulators or other things).... some details on identifying components here:

https://electronics.stackexchange.com/questions/176756/how-to-identify-smd-devices-from-the-codes-on-top-of-the-component

Can usually zoom in with a phone or better camera and take a picture to be able to actually read the labels, sometimes need to get the angle to get light bouncing off it or wipe off the components to get rid of any grime.
```

---
## \#247 Posted by: MontPierre Posted at: 2017-08-25T20:40:48.368Z Reads: 467

```
I will undress my remote and get some pics. You're right, if there is no custom pcb then it will be too complicated. @solidgeek was looking into making one but I think it would be for later Versions if anything  ;)
```

---
## \#248 Posted by: chinzw Posted at: 2017-08-25T20:42:34.466Z Reads: 469

```
If im not mistaken, that circuit you posted wont stay on tough. It looks like its just a capacitor bleeding timer, but it wont stay on indefinitely or off indefinitely.
```

---
## \#249 Posted by: Fatglottis Posted at: 2017-08-26T11:22:13.085Z Reads: 486

```
As I mentioned earlier in post 138. This is what I am using and it works perfectly for button hold on/off! The board is the size of a finger nail  :)

http://www.ebay.com/itm/3V-12V-Solid-State-Switch-Control-Module-Power-Soft-Start-Switch-PCB-for-DSO-068-/141768160000?hash=item21020a7300:g:l60AAOSwTapV7P5M
```

---
## \#250 Posted by: MontPierre Posted at: 2017-08-26T11:50:36.437Z Reads: 474

```
Amezballs! Sorry I missed your earlier post. I shall look into this!
```

---
## \#251 Posted by: solidgeek Posted at: 2017-08-28T14:52:31.271Z Reads: 494

```
Sorry for the late answers guys, I have been sick for the last four days :grimacing:

@Maxid Looks good! Great idea with the lip thing, I will definitely try to add that to the 3D model. Regarding the nuts, I don't think it is necessary. I have been assembling and dissembling my remote (with threads in the plastic) +20 times, and it still works great. Sure it takes a little time to reopen the remote, however no more than a minute (about 10 seconds per bolt?). Maybe adding the lip I could remove 2-3 bolts from the design, making it much easier to reopen.

@chinzw Great! I am looking forward to seeing the result :slight_smile: However sampling from a 0-2v output from an Arduino running on 5V (or even 3.3V) would mean a much lower resolution, does the m0 has a higher resolution ADC?

@MontPierre Regarding the soft switch, I think it's a nice idea, however, I think it takes up to much space in the current version. Maybe it could be added in the future. I am planning on making a custom PCB for all the electronics, some time in the far future :P 

**Update regarding the beta version**: I am beginning to receive all the parts, however, some (many) things probably got stuck in customs (or bad weather) so I expect at least a week more before everything arrives :slight_smile: . Meanwhile, I will make my 3D-printer do some work :sunny:
```

---
## \#252 Posted by: chinzw Posted at: 2017-08-28T16:43:18.850Z Reads: 458

```
@solidgeek i didn't have time this weekend, but ill get to it this week. The proto m0 has a 12bit ADC, on 3.3v thats 0.81mv resolution, it should be plenty :slight_smile:
```

---
## \#253 Posted by: chinzw Posted at: 2017-08-29T05:12:56.503Z Reads: 456

```
@solidgeek hey dude, i was just checking the thingiverse files, is there any chance to get a source? i rather not have to work with stls
```

---
## \#254 Posted by: pshaw Posted at: 2017-08-30T04:38:49.346Z Reads: 440

```
I can't tell but is this the same exact size as the boosted remote? How does the total wheel travel compare?
```

---
## \#255 Posted by: wafflejock Posted at: 2017-08-30T17:07:07.107Z Reads: 444

```
I was busy writing books in the thread when you posted this thanks for sharing again interesting little doohickey.
```

---
## \#256 Posted by: Jammeslu Posted at: 2017-09-03T13:11:27.298Z Reads: 440

```
How is it going?
```

---
## \#257 Posted by: Clonkex Posted at: 2017-09-06T04:03:28.119Z Reads: 460

```
This is an awesome thread. I finally know how I'm going to build my remote. Maybe I'll even look into how to control OLED displays with Arduinos :P
```

---
## \#258 Posted by: solidgeek Posted at: 2017-09-06T20:26:12.164Z Reads: 483

```
Hi all, sorry for the missing updates! I just started my third semester at the university, so I have been very busy. I have been updating my GitHub wiki with some schematics and information regarding the remote. It's not finished yet, but I think I will be able to finish everything this weekend.

You can find the schematics here: https://github.com/MrSolidGeek/nRF24-Esk8-Remote/wiki under the subpage "Electronics". 

Regarding the beta remotes, I am still waiting for a few components :P Why does everything has to come with the slow boat from China...
```

---
## \#259 Posted by: chinzw Posted at: 2017-09-06T20:42:14.120Z Reads: 472

```
@solidgeek any chance i can get fusion files or some other editable file that's not an stl?
```

---
## \#260 Posted by: MontPierre Posted at: 2017-09-06T20:53:14.676Z Reads: 483

```
@chinzw I'm with you! I would like to add a button and etc.
```

---
## \#261 Posted by: solidgeek Posted at: 2017-09-07T22:05:15.685Z Reads: 492

```
@chinzw and @MontPierre I do not plan to release the original files just yet because they are a giant mess (and not entirely finished). I will try to finish the design completely this weekend, maybe then. Sorry :) 

I just received a lot of items for the prototypes today :smiley: Only waiting for the batteries now! :smiley: 

<img src="/uploads/db1493/original/3X/f/2/f2031164598de61ffec64cf8c8863caf1a5cef16.jpg" width="690" height="483">
```

---
## \#262 Posted by: danielz Posted at: 2017-09-07T22:54:37.973Z Reads: 480

```
Remove those handles from the bed clips, they vibrate so much, took me 2 weeks to realize myself :slight_smile:
```

---
## \#263 Posted by: Jammeslu Posted at: 2017-09-08T06:04:37.610Z Reads: 469

```
Is there a way to make the remote feel smoother and more premium exept sandpapper ?
```

---
## \#264 Posted by: ACIN Posted at: 2017-09-08T06:37:15.632Z Reads: 468

```
Yes: acetone vapor smoothing, using better filament, using different colors for different parts and especially changing print settings (acceleration, speed, temperature, layer thickness, nozzle size, tightening printer joints etc.).
Much more you can do just google it.
```

---
## \#265 Posted by: solidgeek Posted at: 2017-09-08T09:27:46.466Z Reads: 463

```
@Jammeslu Its all about finding the right settings for your 3D-printer. I own a Creality CR10 (a low budget printer) and my prints look more premium than most I have seen printed on much more expensive machines. I use a layer height of 150 microns (0.150mm) and a layer width of 0,4mm for almost every print. 

As @ACIN mentions there are many ways to improve the look of the print. As an example, if you are using ABS as filament a acetone vapor bath would remove most of the layer lines.
```

---
## \#266 Posted by: chinzw Posted at: 2017-09-08T16:45:22.724Z Reads: 450

```
@Jammeslu CA glue works wonders too.
```

---
## \#267 Posted by: MontPierre Posted at: 2017-09-08T18:55:19.086Z Reads: 443

```
I might try at some point resin :sunglasses: It would look so cool!
```

---
## \#268 Posted by: wafflejock Posted at: 2017-09-09T17:00:03.331Z Reads: 452

```
.1mm parts will be pretty close to smooth already and like others said acetone bath for abs or with pla just use sandpaper and can use spray paint after sandpaper to help fill in any remaining layer lines
```

---
## \#269 Posted by: Johan_R Posted at: 2017-09-12T12:15:25.695Z Reads: 470

```
@solidgeek Just found this awesome awesome build, and instantly fell in love. Arduinos is totally new to me, but i will give it at try. Is it possible to become one of "late" beta tester, or is it possible to buy the 3d printed parts from you? I think i am up to the soldering and assembly my self. Btw. i am also from Denmark (Aarhus)

Again, SICK build!
```

---
## \#270 Posted by: MontPierre Posted at: 2017-09-12T12:50:38.610Z Reads: 498

```
Just got my print delivered ;) nothing pretty as I'll be changing design to accommodate soft switch  button and etc 

<img src="/uploads/db1493/original/3X/7/2/728a2fb68e659647cfcc0f7103df215011335b4b.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/1/a14bdb61fd0296f6ba0b36c7d461951459851eb7.JPG" width="375" height="500">
```

---
## \#271 Posted by: navgor Posted at: 2017-09-12T13:50:43.966Z Reads: 474

```
I've got a Formlabs Form2 Resin SLA printer - I can do a run of these parts using 'Tough' ABS (like) resin. It won't be as strong as real ABS but it's close. Resin is expensive so each print would be £30-40. It would be injection moulding quality however. Anyone interested? Can ship internationally too.
```

---
## \#272 Posted by: MontPierre Posted at: 2017-09-12T14:18:32.487Z Reads: 476

```
@navgor I would be interested ! For sure Outer shell and perhaps thumb wheel. I'll leave interior parts and PLA ;) it should make it even cheaper ;)

What colours resin do you have and are you from UK? 

I also would like to add a space for button and get ride of the LED holes ;) awaiting @solidgeek to clean up the files ;)
```

---
## \#273 Posted by: Jammeslu Posted at: 2017-09-12T15:42:26.982Z Reads: 469

```
not that educated about 3dprinting but isn't it possible to print the trigger and thumbwheel is some kind of rubbermaterial? for better grip etc
```

---
## \#274 Posted by: navgor Posted at: 2017-09-12T15:56:37.928Z Reads: 488

```
Great. Well if 5+ people want the parts I'll order up the resin.

The tough resin is only available in a translucent light blue colour. See video:
https://youtu.be/R2yh1YnZUCk?t=26

I also have loads of white and a little but of grey left. I think i'm out of black right now.

@Jammeslu it is possible to print using a flexible / rubbery resin for the trigger and thumbwheel in resin. If there is interest I could also do a run of rubber parts.
```

---
## \#275 Posted by: meissnerl Posted at: 2017-09-12T16:39:59.239Z Reads: 460

```
I would be interested in the rubber thumbwheel, my PLA one is not that good...
```

---
## \#276 Posted by: MontPierre Posted at: 2017-09-12T16:47:24.178Z Reads: 467

```
I think black or grey would be better. Not only in terms of colour but also it will be cheaper and product doesn't have to be uber tough INMO.

As for thumbwheel I was thinking Colorfabb nGen Flex - not too flexy not too hard... But thats a different printer right?
```

---
## \#277 Posted by: navgor Posted at: 2017-09-12T17:12:24.494Z Reads: 457

```
The black is quite brittle, I doubt it would take a fall. I can print one in white which has the same strength as black and do some tests.
```

---
## \#278 Posted by: navgor Posted at: 2017-09-12T17:13:36.683Z Reads: 455

```
Yea, the form2 is resin based. uses a UV laser to cure a liquid resin. I have standard FDM printer too.
```

---
## \#279 Posted by: MontPierre Posted at: 2017-09-12T17:18:08.713Z Reads: 445

```
@navgor  Ohhh then I might order thumb wheel from someone on 3D hubs in UK. Are you in UK?
```

---
## \#280 Posted by: solidgeek Posted at: 2017-09-12T23:26:44.022Z Reads: 475

```
Just got a letter from customs, the LiPo batteries are on their way to me! A few days and I will be able to assemble 10-12 remotes :-)  Yeah! 

@Johan_R Hey! Thanks for the kind words. I would love to ship you the components, and 3D-printed parts, however I only got spare parts for all the beta builds (at the moment). I will add you to my list, and notify you when I got the parts ready for you (I am thinking about creating a small webshop selling the remote and kits :P ). I you are interested, I could ship you the 3D-printed parts and the components I got in stock (bolts, switches, micro USBs etc.), and you could buy the rest yourself :slight_smile: 

@MontPierre Looks awesome mate! Can't wait to see your final version :smile:

@navgor That would be so cool!!  I am currently testing a slightly modified 3D-model (only enclosure modification) with three bolts instead of six. I would wait with the expensive model until I release the modified version :slight_smile:
```

---
## \#281 Posted by: navgor Posted at: 2017-09-12T23:36:27.233Z Reads: 426

```
Yea I'm in London but can ship globally for pretty cheap (non-tracked though). You?
```

---
## \#282 Posted by: navgor Posted at: 2017-09-12T23:38:10.274Z Reads: 440

```
[quote="solidgeek, post:280, topic:28543"]
That would be so cool!!  I am currently testing a slightly modified 3D-model (only enclosure modification) with three bolts instead of six. I would wait with the expensive model until I release the modified version :slight_smile:
[/quote]


Cool, let me know and I'll do a few runs. I can probably get 6 or so full prints out of a resin tank.
```

---
## \#283 Posted by: landonkun Posted at: 2017-09-13T00:39:51.091Z Reads: 445

```
I've been following this thread while on a work trip and am finally back and exited to try this out!

I JUST printed a test print with my very first 3D printer and it went well :slight_smile:

@solidgeek I may have missed it somewhere in this thread, but do you have any tips on ideal settings for this particular print (infill, etc)? I'll be using PLA for now, until I buy/experiment with other filaments.
```

---
## \#284 Posted by: MontPierre Posted at: 2017-09-13T07:55:09.617Z Reads: 423

```
@navgor London too baby! Amazing! Well let's keep in touch ;) 

Are you planning to put you're own remote By yourself or would you rather buy assembled one?
```

---
## \#285 Posted by: navgor Posted at: 2017-09-13T09:41:41.075Z Reads: 414

```
Nice one! I'm East London, (London Fields), you nearby? Yea I'll be printing my own. Shall I let you know when I do a do a run for you as well?
```

---
## \#286 Posted by: MontPierre Posted at: 2017-09-13T09:58:20.132Z Reads: 416

```
Sure ! I'm south - Brixton. 

As I mentioned- I'll hold off until I have final design and files, otherwise printing few times will make it very expensive DIY remote hahha;) but would love to see how this resin print look in real life. Do you have all parts? I have some ordered in bulk so I can sell few off to you, you'll save on shipping and etc.
```

---
## \#287 Posted by: navgor Posted at: 2017-09-13T10:12:39.607Z Reads: 422

```
I have the Arduino, OLED and charger/boost circuit.Yea I'll buy the rest of the parts off you if you have them all.
```

---
## \#288 Posted by: Martijn Posted at: 2017-09-13T19:27:50.704Z Reads: 428

```
Oke... I'm following this thread for some time now. @solidgeek you have made an awesome remote sir! I'm definitely want one.
I'm also like the idea from @MontPierre to get ride of the leds or replace them with buttons. This makes the remote more stealthy as esk8 are illegal in the Netherlands. So I don't want raise suspicion with the police with bright shiny leds ;-)

I'm in!
```

---
## \#289 Posted by: Genius2017 Posted at: 2017-09-14T03:49:13.360Z Reads: 431

```
Hello @SolidGeek, what program are you using to layout your new pcb? Just joined the thread and love the design you have so far. Looking to build my skateboard this year if time permits.
```

---
## \#290 Posted by: Nordle Posted at: 2017-09-14T06:34:33.627Z Reads: 449

```
Hey @solidgeek, awesome work! You may could help me with some easy answers^^
-The receiver part consists of just a nrf chip, no arduino? And how is that wired to vesc? Would be a nice additive in your github.
-OLED is 0.91inch - 128x32pixels?
-The switch on ''D4'' is it for cruise control?
-And i assume instead of the hall sensor i can use a pot? They do the same from what i understand.
 
And if you have some parts left or a set let me know, i buy yours then instead of ordering;)

Cheers!
```

---
## \#291 Posted by: Necromenz Posted at: 2017-09-16T19:50:58.141Z Reads: 440

```
Hi! Awesome work! I'd like to be a beta tester too if possible. Iam from germany and I have a dual VESC 6 Mountainboard.
```

---
## \#292 Posted by: wafflejock Posted at: 2017-09-16T20:02:53.419Z Reads: 486

```
It's difficult to find a potentiometer that doesn't have a long threaded shaft for mounting it in and therefore is pretty big.  Basically I've found the ones for guitars and other audio equipment (beware linear vs tapered http://www.resistorguide.com/potentiometer-taper/ ) or the very small surface mount ones that are hard to attach to a trigger or wheel.  The advantage with the hall sensor is there is no extra resistance from the knob itself and it's easier to make it fit in a compact design, I'm currently redoing my own design here with a trigger control and using a pot but because of the size of the potentiometer I need it to stick out of the side or make the remote thick.

Regarding electronics for this project there is an arduino nano involved for reading the values and passing the data along to the nrf chip to transmit to the receiver.  I believe the nrf chips can be reprogrammed directly but pretty sure there is no ADC to read the sensor/knob position so still need some other MCU.  There are other boards like the ESP8266 with a MCU and transceiver on one board but they are made to work on wifi and likely have more latency without doing extra work to change the default protocols.

Anyhow for parts for this project it's linked above:
https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit#gid=0

http://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/19

---

Still working tweaks of a new version here (very blocky right now but just getting dimensions on the guts worked out and can push things out afterwards to smooth it out) https://cad.onshape.com/documents/50e9e32d777391df91fbe5a9/w/19598faab2182f3b574dcfaf/e/52a747c0c2e141ee735a22b8
```

---
## \#294 Posted by: wafflejock Posted at: 2017-09-16T20:15:21.614Z Reads: 493

```
https://github.com/MrSolidGeek/nRF24-Esk8-Remote/blob/master/receiver/receiver.ino#L21

https://github.com/MrSolidGeek/nRF24-Esk8-Remote/blob/master/receiver/receiver.ino#L64

^^ is writing the data to Digital Pin 5 so the receiver signal wire should go to digital pin 5 the arduino can get power through vin (goes through votlage regulator) or if you trust the BEC then can go into the 5V if it supplies regulated 5V well.

I also have more explanation of setting things up and wiring on my github:
https://github.com/shusain/eskatecontroller

Believe @solidgeek mentioned doing a video at some point to explain the build/programming that's probably the best way to communicate all this for people who aren't already familiar with arduino or the nrf chips.
```

---
## \#295 Posted by: Nordle Posted at: 2017-09-20T08:35:29.683Z Reads: 454

```
[quote="Nordle, post:81, topic:28543, full:true"]
Love this project! Why not use arduino with integrated nrf module? Could safe a lot trouble from what i read, no experience actually.
[/quote]

[quote="solidgeek, post:84, topic:28543"]
@Nordle I am glad you like my work! Regarding your proposal... Do they exist? :open_mouth: If they indeed do, well it would be interesting to try it out! I am thinking about making a custom PCB with a few solder points (easy assembly), a socket for an Arduino Nano (or mini) and use a Low Dropout Regulator to make a stable 3.3V for the nRF24 module. I believe this would be much better than the 3.3V supplied by the Arduino, and eliminate any power related issues :slight_smile:
[/quote]

i Think i found one, could it work?
https://www.aliexpress.com/item/V3-Wireless-module-NodeMcu-4M-bytes-Lua-WIFI-Internet-of-Things-development-board-based-ESP8266-esp/32647542733.html?spm=2114.33020108.13.9.95WBOB&scm=1007.12851.33061.0
..need to find one without headers now
```

---
## \#296 Posted by: MichoFPV Posted at: 2017-09-20T09:29:48.929Z Reads: 429

```
NodeMCU is not Arduino, but you can program it in Arduino IDE with right libraries. The code is running on ESP8266 itself. Also I wouldn't worry about headers, you can easily desolder them or just cut them with pliers.
```

---
## \#297 Posted by: chinzw Posted at: 2017-09-20T17:59:35.279Z Reads: 449

```
Adfruit makes Feathers with NRF52 BLE already integrated, you can comunicate nrf52 with nrf24.
https://www.adafruit.com/product/3406

This would solve, charging, lipo and nrf all in one.
```

---
## \#298 Posted by: Jammeslu Posted at: 2017-09-20T18:16:54.665Z Reads: 427

```
whats status on betas?
```

---
## \#299 Posted by: solidgeek Posted at: 2017-09-20T19:00:43.924Z Reads: 477

```
@landonkun Well I got a few tips printing the remote casing :-) I have written something about it on my Github page: https://github.com/MrSolidGeek/nRF24-Esk8-Remote/wiki/1.-Housing-and-mechanism

@Martijn Well I have been thinking about removing the LEDS for quite some time, they are the remnants of the first remove I designed without an OLED. All information is displayed on the OLED, so maybe I should just get rid of the LEDS :slight_smile: What do you guys think? 

@Genius2017 I use Eagle mostly, however, more recently I began learning Altium (pretty heavy program - and not free) :-) 


@Nordle Thanks mate! The receiver part consists of an Arduino and the nRF24. However, it should be possible to connect an nRF24 module directly to a VESC. However, I have not tested it yet - seems rather complicated. The switch is used as a "kill switch" as standard but will be changeable through the interface. (I can see that your answer has already been answered - thanks, guys :slight_smile:) 

@Necromenz I do not have the spare parts at the moment to make you a beta... But I will add you to the list for the next batch :P  

@Jammeslu Status on betas is that I got all the parts in house, with the exception of some JST connectors for the receiver - does anyone know where I can get those? China isn't a option, to long delivery time! I need a week or two to finish the remotes as I only get to work on them in the weekends - I study (and live) a few hours away from my workshop...  I hope to make the first test unit this weekend, and if it goes well I assemble the rest :slight_smile:
```

---
## \#300 Posted by: Clonkex Posted at: 2017-09-20T23:07:33.634Z Reads: 470

```
Wow that wiki information is fantastic! Keep it up! :smile:

I think the LEDs are unnecessary if you've got a screen.

I buy JST connectors from eBay. Just filter by whatever country you're in, like so:

<img src="/uploads/db1493/original/3X/0/7/07dd260059fd9d7bdf49c46b4f12c4c636fbc207.png" width="271" height="185">
```

---
## \#301 Posted by: chinzw Posted at: 2017-09-20T23:08:34.814Z Reads: 453

```
@solidgeek where are you? if you're in the US/Canada use digikey, 8$ overnight shipping.
```

---
## \#302 Posted by: Necromenz Posted at: 2017-09-22T10:36:13.861Z Reads: 430

```
@ solidgeek
Thx for the anwser.No Problem i can wait and i hope i can help at the next batch. :slight_smile:
```

---
## \#303 Posted by: Martijn Posted at: 2017-09-22T12:27:16.693Z Reads: 433

```
Well I think the Led's are unnecessary if everything is presented on the screen.
@solidgeek Count me in for the next batch :+1:
```

---
## \#304 Posted by: Samuele00 Posted at: 2017-09-22T13:00:13.621Z Reads: 430

```

sorry, does anyone have the libraries and codes used to program the receiver and transmitter? is it easy to program everything? I want to build a glove-shaped transmitter
```

---
## \#305 Posted by: Clonkex Posted at: 2017-09-22T13:05:27.189Z Reads: 425

```
Do you know how to program? If not, programming it will not be easy.
```

---
## \#306 Posted by: Samuele00 Posted at: 2017-09-22T14:38:30.916Z Reads: 425

```
I`m at the basic level
```

---
## \#307 Posted by: solidgeek Posted at: 2017-09-22T22:17:52.910Z Reads: 445

```
I have been looking at a way to implement PPM cruise control. Any suggestions on that topic @wafflejock? I can only think of two ways to accomplish this.

**First method:** Setting speed value to current Hall-reading, if the trigger is pressed. 

This way you can only cruise if you first use the throttle first, and the speed will not be constant if the load changes (assuming one is using current control). 

**Second method:** Calculating a PPM value based on the eRPM (or current), if the trigger is pressed.

This way you will always be able to cruise by holding the trigger, however, it could be very dangerous if the PPM value isn't calculated correctly. Any thoughts on this would be appreciated. How do you accomplish this with your watt control @Ackmaniac.
```

---
## \#308 Posted by: Genius2017 Posted at: 2017-09-27T16:47:20.422Z Reads: 458

```
Looking at the Transmitter Sketch Code if anyone is interested in seeing the graphics images being displayed on the OLED, GIMP allows you to take an XBM file with the Char values and load the images into GIMP for viewing. I did this for "static unsigned char u8g_logo_bits[] ", "static unsigned char wifi_bits[]",static unsigned char wifi_nosignal_bits[],static unsigned char wifi_transmitting_bits[]. I will attach a screenshot for those. At least it gives you an idea of what some of the values mean to those who are not good at programming or so. Still waiting for my hardware to arrive from China to finish my remote. Other then that messing around with the code to get a feel for things. <img src="/uploads/db1493/original/3X/2/0/206339301f176e4e2c95238fa730dcfb8436208f.JPG" width="690" height="472">
```

---
## \#309 Posted by: BoostedBuilder Posted at: 2017-09-27T21:05:31.268Z Reads: 465

```
Hi @solidgeek, I love your work with the remote design! I've been following this thread for quite a while now but just don't remember if anyone talked about the questions I have so in advance, sorry if you have already answered these:

Why don't you consider putting a bigger OLED screen? Would it fit? 

Why are you using a hall sensor for the dead man's switch when you can just you a button like this:
<img src="/uploads/db1493/original/3X/b/1/b18718bb169546e281b0958c81d7f797eb80e2db.JPG" width="375" height="500">

Have you considered a button for changing mode, and what's shown on the OLED. 

Thanks for your effort on trying to help the community!!
```

---
## \#310 Posted by: Jammeslu Posted at: 2017-09-27T21:09:08.392Z Reads: 448

```
Another question. 
Are you trying to implement the new features people requested and implement that inte betas or are you building and realizing betas soon and then upgrading firmware etc
```

---
## \#311 Posted by: chinzw Posted at: 2017-09-27T21:14:30.760Z Reads: 448

```
He's not using a hall sensor for the switch, its just a normal 4 pin switch.
```

---
## \#312 Posted by: landonkun Posted at: 2017-10-01T04:53:38.029Z Reads: 460

```
Does anyone know if these receivers will also work?

http://www.ebay.com/itm/6-x-2-4-GHz-Wireless-Transceiver-Module-NRF24L01-/182551182042

I don't know much about this stuff, but I can solder it all together if I know what to buy :slight_smile:
```

---
## \#313 Posted by: vishal_tejwani Posted at: 2017-10-01T20:05:53.510Z Reads: 457

```
Can you make a complete diy video, not all can get the remote at same time, it would be very helpful. 

You are already working on beta remotes while making that you can shoot some clips , I can edit them for you
```

---
## \#314 Posted by: solidgeek Posted at: 2017-10-01T21:43:59.797Z Reads: 475

```
@landonkun they should work, however I would highly recommend using the ones I have been using instead :slight_smile: check out my part list.

 @vishal_tejwani I will try to make a video while producing the betas. I am almost done with the first, and I Hope to be done with all beta before next week :smile:

<img src="/uploads/db1493/original/3X/5/5/55c1796476e8cd947c9b6e567a29439e2ac2679f.jpg" width="690" height="388">

  <img src="/uploads/db1493/original/3X/0/7/07ec82976ddad29b84c27ecd5832bbf703879620.jpg" width="281" height="500">
```

---
## \#315 Posted by: Maxid Posted at: 2017-10-01T22:26:04.847Z Reads: 441

```
I see you added a lip to the case :thumbsup:
:heart_eyes:
```

---
## \#316 Posted by: landonkun Posted at: 2017-10-02T04:01:33.927Z Reads: 450

```
I've purchased double of all the parts, so assuming everything works when they arrive (in probably 2-3 months because China shipping to Canada is terrible), I might be able to build one extra controller to sell to someone at cost (if anyone wants).
```

---
## \#317 Posted by: esk8guy Posted at: 2017-10-02T04:04:51.765Z Reads: 445

```
what do I need to make the receiver for the board?
```

---
## \#318 Posted by: vishal_tejwani Posted at: 2017-10-02T04:41:07.530Z Reads: 439

```
How much time will it take to make video? Both reciver and transmitter. You said the same in lastmonth too😅
```

---
## \#319 Posted by: vishal_tejwani Posted at: 2017-10-02T05:39:41.414Z Reads: 449

```
I understood how to make remote read your github page,but didn't understand the reciver part.

Also uts the codeongithubthe most updated version?
```

---
## \#320 Posted by: Genius2017 Posted at: 2017-10-06T01:13:28.465Z Reads: 471

```
Here is an interesting design of a remote I found on AliExpress.<img src="/uploads/db1493/original/3X/8/6/86271f7a6dfa293f847cd17b0c917d0abc65dbd8.jpg" width="281" height="500">
```

---
## \#321 Posted by: Genius2017 Posted at: 2017-10-06T01:16:15.034Z Reads: 460

```
Maybe a design of this sort could be made for a skateboard remote. Replace the buttons with a small insert of a display of some kind. Thinking about getting one and take it apart to see what I could come up with. What does everyone else think?
```

---
## \#322 Posted by: esk8guy Posted at: 2017-10-06T01:17:36.111Z Reads: 444

```
if you’re you’re going to take it apart anyways just 3d print it
```

---
## \#323 Posted by: solidgeek Posted at: 2017-10-08T19:30:09.502Z Reads: 480

```
@esk8guy You will need an Arduino, a nRF24 module and maybe a capacitor (220uF) for input voltage stabilization. 

@vishal_tejwani I will try to make the video this week, however I am a very busy person - and I am doing this in my spare time :slight_smile:

The code on github is not the newest version, I have made quite some changes recently. I will update the code as soon as I finish the betas. 

@Maxid the lip works great, its a very nice addition to the design :D
```

---
## \#324 Posted by: solidgeek Posted at: 2017-10-09T21:37:24.314Z Reads: 496

```
Today I finished the first beta remote, using all the new parts and changes made so far. Here is what I have learned:

-  Using the Arduino with a dedicated 3.3V regulator gives a higher range.  

- A capacitor is no longer needed on the 3.3V output to support the current demand.

- The nRF24 module is sensitive to noise from nearby wires and coils. The right position (and or shielding) is essential for reliable communication. 

- It takes roughly 3 hours to assemble a remote, at least the first one (hopefully I can speed up the process - lol :smile:) 

I have been updating the 3D-models and made a new assemply-file: 

 <img src="/uploads/db1493/original/3X/f/9/f9b9fea3e4ce53888af51bd23db845069efeb17a.png" width="616" height="500">

What do you think of the name :smile: ?
```

---
## \#325 Posted by: Nordle Posted at: 2017-10-09T21:50:27.144Z Reads: 469

```
[quote="solidgeek, post:324, topic:28543"]
What do you think of the name :smile: ?
[/quote]
i like, all we need now is a foolproof tutorial how to set one up;)
```

---
## \#326 Posted by: Genius2017 Posted at: 2017-10-10T01:37:43.204Z Reads: 464

```
@solidgeek nice. Another name(s) could be OrangeLeaf remote, ArdEsk Remote, EskLeaf Remote, SpeedSkate Remote, EMJ remote.
```

---
## \#327 Posted by: NAF Posted at: 2017-10-10T07:44:55.669Z Reads: 455

```
Awesome name !! @solidgeek ..can't wait !!
```

---
## \#328 Posted by: vinividivici Posted at: 2017-10-10T12:38:32.710Z Reads: 470

```
Good work and nice name ;-) 

Will you be selling these sometime in the near future or is it just meant as a hobbyist do it yourself project?


Got my Raptor 2 a while back, but the nano-x is lacking in some aspects. Would definitely be nice to be able to read the board battery % off the controller instead of checking bellow the board how much juice you have left.

Your design is :thumbsup: and you got a customer once you get out of the beta stage ;-).
```

---
## \#329 Posted by: Genius2017 Posted at: 2017-10-10T19:11:35.316Z Reads: 484

```
Just putting my remote together after getting my parts in and i thought i would share a few things for those who are interested of a few things i did to my remote. Please let me know what you think. Happy building.<img src="/uploads/db1493/original/3X/d/a/da91af579472d88717a816fc66329631e3252a3f.JPG" width="690" height="392"><img src="/uploads/db1493/original/3X/8/c/8c4d55ff76959e387e7c7e5da26113ca87915a89.JPG" width="690" height="394">
```

---
## \#330 Posted by: MontPierre Posted at: 2017-10-10T20:16:42.513Z Reads: 469

```
@Genius2017 Cool! Thanks for update! I’ve got all my parts, just looking for some spare time to put it together. I also ordered micro limit switch ( for another project) so I’ll give it a try! 

I’m also planing to add soft switch option to power on and off remote with long press of a button ( need to come up with convenient place for it ) instead of slide switch at the bottom of the remote.
```

---
## \#331 Posted by: Clonkex Posted at: 2017-10-10T21:34:27.588Z Reads: 497

```
I freakin love the name! The instant I saw it I thought it was perfect. Think I'm going to start buying up some of the parts for it and 3D print one myself :smiley: 

@MontPierre Why replace the slide switch though? Long-press power buttons are way more annoying.
```

---
## \#332 Posted by: solidgeek Posted at: 2017-10-10T22:30:50.695Z Reads: 502

```
@Nordle glad you like it! I will be assembling a remote tomorrow - and hopefully get some nice pictures for the tutorial :) 

@Genius2017 Cool names, but I think I prefer Firefly Remote  :P 

@NAF Thanks mate!

@vinividivici Thanks! I really appreciate your kind words - it keeps me going :wink: I am planning to sell kits and maybe fully assembled remotes in the future yes! However the fully assembled remote will need a custom PCB - otherwise, the assembly process will take to much of my time :P   

@Genius2017 Awesome dude! Thanks for sharing - I think I will be adding the small holes in the 3D-model :slight_smile:

@Clonkex Glad you like it, I think the name suits the remote quite well too! I got some displays and most basic parts in stock if you need something (bolts, springs, micro USB etc.).
```

---
## \#333 Posted by: bsancken Posted at: 2017-10-10T22:37:12.543Z Reads: 482

```
When it gets closer to being done I'll defitely sign up for a kit/final parts list! I'd love to put something like this together.

What are the chances of putting the screen somewhere more readable? I'm not sure where that would be, but just throwin it out there!
```

---
## \#334 Posted by: Genius2017 Posted at: 2017-10-10T23:49:55.479Z Reads: 473

```
Sorry about the first picture with the holes added for the magnets. When I did my PowerPoint I copied over another text box. I will upload tomorrow with the correct headings.
```

---
## \#335 Posted by: Genius2017 Posted at: 2017-10-10T23:53:25.049Z Reads: 460

```
@solidgeek thanks. You know what would be cool is at the top of the remote to have a small LED for a light in case you want to look for your keys the remote with let's say three clicks of a button will turn on the LED light and if in the sourcecode it will time out after a few seconds or so so it won't drain the battery. Great option for those who hit the trails at nigh time. Would be a cool feature. What you think?
```

---
## \#336 Posted by: Jorand Posted at: 2017-10-11T00:26:18.536Z Reads: 455

```
@solidgeek I love your project, thanks for sharing it. 
I plan to make one and I found a new version of the NRF24L01 with IPEX connector, it allows me to stick the antenna out of my esk8 case for the receiver.
I will share my progress :)

https://fr.aliexpress.com/item/1PC-New-Arrival-100mW-AS01-SPIPX-nRF24L01-wireless-pa-lna-2-4g-wifi-module-Wireless-Transmission/32819372747.html
```

---
## \#337 Posted by: Clonkex Posted at: 2017-10-11T00:38:40.559Z Reads: 456

```
That's called a torch. You should buy one.

:P
```

---
## \#338 Posted by: Genius2017 Posted at: 2017-10-11T01:27:06.354Z Reads: 473

```
Here is the updated pic with the correct text boxes. Sorry for the mistake. Did this at work and should have proof read before saving. Enjoy.<img src="/uploads/db1493/original/3X/6/1/610bf65252a5113fc1f4b494258aa9b71fbdc959.JPG" width="690" height="392">
```

---
## \#339 Posted by: Genius2017 Posted at: 2017-10-11T01:29:52.314Z Reads: 462

```
@MontPierre Soft switch would be a great idea. let me know what you use for the switch if you find one that fits please post the link.
```

---
## \#340 Posted by: Genius2017 Posted at: 2017-10-11T01:48:54.904Z Reads: 477

```
I'm going to buy a small white LED and see if its possible to make it fit near the trigger switch or so. Playing around with some cool ideas. Love the remote @solidgeek.<img src="/uploads/db1493/original/3X/0/b/0b8e5ee398e033c7b05177671cb7757bcbb6bdf0.JPG" width="690" height="393">
```

---
## \#341 Posted by: boards Posted at: 2017-10-11T03:15:15.734Z Reads: 474

```
My NRF nunchuck has been sticking lately even though I bought a legitimate nintendo nunchuck :(.

Considering making one of these when I have time. I have a little experience getting arduino -> vesc nrf working too.
```

---
## \#342 Posted by: MontPierre Posted at: 2017-10-11T07:27:21.721Z Reads: 476

```
Has anyone had a problem with spring being very tight? Mine is made of  0.49 mm thick wire. Throttle really bounces back hard when released and it’s a work out to move the wheel forward and backwards. Perhaps it will loosen up with time, I guess I’m yoused too my Maytech remote with thumb throttle too much - it is softer ( 1 axis joystick).

Also - @solidgeek any chance to easily disable deadman switch in the code ? Just to have as an Option, as I think my hand will have spasms after a while ;)
```

---
## \#343 Posted by: Sander Posted at: 2017-10-11T07:59:12.887Z Reads: 471

```
If another guy has electric skateboard and  has the same remote won't it cycle between the two remotes because the signal has most likely the same pipe? When I was testing that thing happened to me, if someone had the same address etc...
```

---
## \#344 Posted by: Genius2017 Posted at: 2017-10-11T13:34:03.029Z Reads: 492

```
@Sander  Nordic's Explanation of Pipe Address(s).

We recommend using at least 32bits address, preferably 40bits address. The reason we don't recommend using a shorter address is that the nRF device might demodulate random noise on the air which might match with the correct address. Using a long address avoids this problem.

For instance with a 16bit address and 1mbit speed, the chance is that random noise hits the correct address about every 65ms. Statistically with a 32bit address hits the correct address every 70 minutes.

We recommend enabling 16bit CRC, this ensures that the received payload is correct. Both the address field and payload must be equal to the CRC checksum. All bits must be correct otherwise the packet is discarded.

Here are some guidelines when choosing an address:

A. The address made by (5, 4, or 3) equal bytes (0x00 or 0xFF) is not recommended because it usually makes the packet-error-rate increase.

B. Addresses where the level shifts only one time (i.e. 0x000FFFFFFF) can often be detected in noise giving a false detection, which again may give raised packet-error-rate.

C. First byte of the address should not start with 0x55.. or 0xAA.. as this can be interpreted as part of a preamble, causing an address mismatch for the rest of the address.

Quick summary:

Use at least 32bit address and enable 16bit CRC.
Avoid addresses that start with 0x00, 0x55, 0xAA and 0xFF.

openWritingPipe
Open a pipe for writing. Addresses are 40-bit hex values, e.g.:

openWritingPipe(0xF0F0F0F0F0);
Parameters:

address: The 40-bit address of the pipe to open. This can be any value whatsoever, as long as you are the only one writing to it and only one other radio is listening to it. Coordinate these pipe addresses amongst nodes on the network.
openReadingPipe
Open a pipe for reading.

Warning: all 5 reading pipes should share the first 32 bits. Only the least significant byte should be unique, e.g.

openReadingPipe(0xF0F0F0F0AA);
openReadingPipe(0xF0F0F0F066);
Parameters:

number: Which pipe# to open, 1-5.
address: The 40-bit address of the pipe to open.

So from the code in Github for Solidgeeks Controller:

	Transmitter (Transmitter.ino)

	const uint64_t pipe = 0xE8E8F0F0E1LL;

	Receiver (Receiver.ino)

	const uint64_t pipe = 0xE8E8F0F0E1LL;

Change the address to whatever you want to make it but follow the notes, rules above. Recompile your code and upload to your Ardunio Device
and you should now have a different address then someone elese's controller. Of course what is in the Github is going to be the same for every controller
until you change it to something different.

I will post the link to Nordic and look at Appendix A for detailed information about "Pipelines"
[https://www.sparkfun.com/datasheets/Components/SMD/nRF24L01Pluss_Preliminary_Product_Specification_v1_0.pdf](https://www.sparkfun.com/datasheets/Components/SMD/nRF24L01Pluss_Preliminary_Product_Specification_v1_0.pdf)
Hope this helps.
```

---
## \#345 Posted by: Genius2017 Posted at: 2017-10-13T01:49:28.469Z Reads: 459

```
@solidgeek looks like @Wajdi took your recommendation of using orange for his top piece for his design of his new remote.

  <img src="/uploads/db1493/original/3X/d/8/d87b60d07a03e7b98776b695ef1cd3228f91ef7f.jpg" width="375" height="262">
```

---
## \#346 Posted by: Wajdi Posted at: 2017-10-13T01:54:07.219Z Reads: 459

```
Nice work! I like the name you gave it! I gotta find a name for mine as well :smile:
```

---
## \#347 Posted by: Genius2017 Posted at: 2017-10-13T13:38:41.657Z Reads: 467

```
@solidgeek <img src="/uploads/db1493/original/3X/9/3/935da26af012f281ec1cf9377ee24a60358906f4.JPG" width="656" height="500">
```

---
## \#348 Posted by: DjamboBuksne Posted at: 2017-10-13T21:12:19.930Z Reads: 482

```
<img src="/uploads/db1493/original/3X/d/f/df5ed30385f70cbbaac87a8100213900ba052c4a.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/1/d11028f3dd8fe8ca6c37d3c7abf001f65d3c1562.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/9/e/9e5225d1571507db8122217e94a6c3bfd431d561.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/2/c2ee1ba2076bd60463935329f285e306c6d30499.jpg" width="375" height="500">

Done printing my remote! How do i wire up the arduino that is going to the esc?
```

---
## \#349 Posted by: Clonkex Posted at: 2017-10-13T22:39:56.347Z Reads: 452

```
I like the Firefly SolidGeek text at the bottom, but I'm not sure about the weird icon at the top.
```

---
## \#350 Posted by: Genius2017 Posted at: 2017-10-13T23:53:27.521Z Reads: 451

```
@Clonkex Suppose to be like a Firefly/dragon fly mix.
```

---
## \#351 Posted by: Jammeslu Posted at: 2017-10-14T16:14:38.490Z Reads: 451

```
I would  rather have a minimalistic logo inly instead of logo and text swell
```

---
## \#352 Posted by: Mozillum Posted at: 2017-10-15T00:40:30.713Z Reads: 457

```
Hi @solidgeek ! Im trying to find which on/off switch you are using? Itˋs not on the partslist😬
```

---
## \#353 Posted by: solidgeek Posted at: 2017-10-15T13:38:36.124Z Reads: 476

```
@Wajdi Thanks! I love your work mate, it looks amazing :-)

I have been thinking of adding a logo of some kind, however, it's hard to find the right print-settings to make it work. I think it looks awesome, but I am not sure if I can print it ... Will try it out tomorrow :-)

<img src="/uploads/db1493/original/3X/3/d/3d175c9a45adba6b5b793992130610435e6ec4c6.png" width="490" height="500">

@DjamboBuksne looks great! The receiver nRF24 is wired the same as the remote. The Arduino should be connected to the VESC in this manner:

TX → RX
RX → TX
5V → 5V
GND → GND
D5 → PPM

You will have to unplug the receiver from VESC while uploading firmware because the serial port (TX, RX) is connected directly to VESC. I also recommend adding a big capacitor (220uF will do) on the 5V rail, to ensure a stable 5V output to the Arduino. I will have a tutorial ready in the following week.

@Mozillum oh I see, well the switch I got from a local store. Its a 13mm Slide switch but any in that size should work just fine. I am able to find a lot of 10mm, however the 12-13mm is hard to come by. Does anyone know of a good supplier?
```

---
## \#354 Posted by: GrecoMan Posted at: 2017-10-15T13:51:18.981Z Reads: 457

```
You got a donation link?  For those of us that cant afford the remote but would still love to support you lol.  Looks amazing!
```

---
## \#355 Posted by: Genius2017 Posted at: 2017-10-16T16:53:47.378Z Reads: 470

```
For those who may be struggling with good, not so good or loss of communication with the NRF's please read below. Link will be at the end.<img src="/uploads/db1493/original/3X/d/2/d282bebab74ab46561f96a656911003d67d19426.JPG" width="690" height="398"><img src="/uploads/db1493/original/3X/1/8/1807c0d4b242a7c358fd48e5ccbbcb5df5c3b3d9.JPG" width="690" height="393">[https://hackaday.io/project/12123-electric-longboard/log/40963-nrf2401-power-capacitor-experiment](https://hackaday.io/project/12123-electric-longboard/log/40963-nrf2401-power-capacitor-experiment)
```

---
## \#356 Posted by: Genius2017 Posted at: 2017-10-16T17:01:13.882Z Reads: 447

```
@solidgeek looks like you changed the throttle. I see there is more that extends to help for a better grip when going forward or reverse. Looks good. When do you think the drawings will be uploaded with the new changes with the beta's, etc?
```

---
## \#357 Posted by: ervinelin Posted at: 2017-10-17T03:30:14.916Z Reads: 448

```
This is such an awesome project.. I have already put all the necessary parts in my cart but before I make the order I wanted to ask a few things.

1. Can one remote control two different boards? Like how in RC radios you can have two models but share the same remote.

2. If my buddy also builds one, will we be able to ride together without interference? I've read the whole thread plus the wiki but there isn't much mention about how to bind the remote to the receiver.

Thanks a lot and I look forward to building my own!
```

---
## \#358 Posted by: Clonkex Posted at: 2017-10-17T04:19:47.895Z Reads: 449

```
1. With some code changes you could, but you'd also need to add a physical switch or button to the controller to set which "pipe" to use in the code.
2. You don't "pair" per se. You'd need to change the "pipe" addresses in the code of the controller AND receiver, and I'd recommend anyone that uses this controller should do that, otherwise they may skate near someone else with this controller (who also hasn't changed their pipe addresses) and things would go wrong.
```

---
## \#359 Posted by: ervinelin Posted at: 2017-10-17T04:35:20.655Z Reads: 447

```
Thanks!

I suppose I can code it in somehow, enter the menu and then swap from one model/board to another. This will be super useful so I don't have to build another remote for another board, which I currently need to do with my GT2B unless I keep rebinding when I swap boards.

Good point about not using the default the pipe address! 

I'll put down an order and hope everything goes according to plan!
```

---
## \#360 Posted by: DjamboBuksne Posted at: 2017-10-17T08:16:06.826Z Reads: 458

```
Oh ok thanks! Is there any way to use it with the esc? I don't need all of that data, I just want to make it work.

Can i connect it like this;
5v to 5v
gnd to gnd 
D5 to signal

Will it work?
```

---
## \#361 Posted by: DjamboBuksne Posted at: 2017-10-17T08:20:00.240Z Reads: 468

```
https://www.thingiverse.com/thing:2454391

There you have "tip designer" option
```

---
## \#362 Posted by: Johan_R Posted at: 2017-10-17T08:49:15.073Z Reads: 448

```
@solidgeek A quick question: Have you any experience with the SS495A from Aliexpress? Or would you recommend to stick with the "well known" from Honeywell ?
```

---
## \#363 Posted by: DjamboBuksne Posted at: 2017-10-17T10:14:15.395Z Reads: 449

```
http://www.ebay.com/itm/2PCS-SS495A-95A-High-Precision-Analog-Linear-Hall-Sensor-Magnetic-Sensor-TO-92S/191160281622?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649 

I ordered it from here and everything is okay. 1 dollar for 2pcs!
```

---
## \#364 Posted by: solidgeek Posted at: 2017-10-17T21:45:08.481Z Reads: 445

```
@GrecoMan Thanks man! I just created a Paypal.me page, I am very glad you think so highly of my work :) 

Donation link: https://www.paypal.me/solidgeek

@Genius2017 Thanks for the information, could be helpful. It seems that the most important factor here is to maintain a good 3.3V supply, by removing noise and supplying enough current. I will upload the the new throttle STL (and keeping the old) tomorrow if it works as expected :slight_smile: 

@ervinelin Thanks I am glad you like it :slight_smile: 1. Yes, however it doesn't support multiple addresses, so you would have to use the same pipe for both receivers - and only use one at the time. 2. As long as you change the pipe (which I recommend regardless) there should be no problem. 

@DjamboBuksne Yes the remote works fine without the UART data, however you will not be able to see speed, distance and board voltage :slight_smile: The remote should work with any standard ESC on the market.

@Johan_R I have no experience with SS495A from Aliexpress. However, they probably work just fine!

Thanks for all the interest and support guys, it means a lot. I'm truly sorry that I am not able to put in more hours finishing the betas and perfecting the remote, but my work and study (electronic engineer) take up most of my time at the moment :frowning: Looking forward to see you guys improve upon my work :slight_smile:
```

---
## \#365 Posted by: ervinelin Posted at: 2017-10-17T23:53:35.788Z Reads: 436

```
@solidgeek I haven't looked at the code yet but I assume you would assign a pipe address on the controller and another on the receiver making sure that they are the same address.

If so can't you have a switch or some method to toggle between two pipe addresses on the controller?

Schematically,
If button pressed 
(Pipe address = receiver 1 address)
Else
(Pipe address = receiver 2 address)

Of cos one board at a time will work too but just isn't the most ideal.
```

---
## \#366 Posted by: egzplicit Posted at: 2017-10-19T14:06:06.063Z Reads: 435

```
What you could do is a routine where both the receiver and transmitter use the same default pipe value at the beginning. Then the receiver could generate a new pipe value and send it to the transmitter (via the default pipe) and wait for a confirmation. Once the confirmation arrives, they both switch to the newly generated pipe and that way you don't have issues when multiple remotes are in the area. Unless this process happens at the same time on multiple devices... in that case you could cross pair them by accident.
```

---
## \#367 Posted by: Clonkex Posted at: 2017-10-19T21:30:37.941Z Reads: 424

```
@ervinelin Yep you could definitely do that.

@egzplicit I reckon that's a great idea. You could even have a menu option on the controller that allowed you to generate a new pipe address. To make it faster and more reliable you could have it store the random pipe address in EEPROM after the first startup (so you could start up your remote at the same time as other people after the first time). Pretty easy to do, too. Gogo @solidgeek, do it!
```

---
## \#368 Posted by: Jammeslu Posted at: 2017-10-19T21:39:25.439Z Reads: 417

```
Great Idea but just let betas out first before improvemts and a v2 maybe
```

---
## \#369 Posted by: Clonkex Posted at: 2017-10-19T21:47:45.030Z Reads: 426

```
The problem is that letting the betas go out with a hardcoded pipe address could cause lots of problems. We're not suggesting a feature, we're suggesting a bugfix. If these remotes turn out to be popular the likelihood of skating near someone else with another of these remotes could be high.
```

---
## \#370 Posted by: solidgeek Posted at: 2017-10-20T21:34:11.601Z Reads: 464

```
@egzplicit Great idea!

@Clonkex I am already on it ;) I only need to do some minor changes to the settings menu and adding some data to the auto-acknowledgment response, and I will have a working example. I believe this is a critical update to perform before finishing the betas :slight_smile:  <img src="/uploads/db1493/original/3X/f/7/f7b1e5a5a49b545d9ff96364f0b41d3fec2a2245.PNG" width="690" height="445"> 

I just got my first donation, thank you so much its very appreciated :slight_smile:
```

---
## \#371 Posted by: chinzw Posted at: 2017-10-20T22:39:44.325Z Reads: 429

```
@solidgeek i dont think i've asked this, but you've added ppm to the receiver right? So that it can be used with any esc?
```

---
## \#372 Posted by: Clonkex Posted at: 2017-10-20T22:40:42.313Z Reads: 414

```
Well yeah, that's how the VESC works as well. That's the only way for a receiver to work unless you make your own custom ESC :P
```

---
## \#373 Posted by: solidgeek Posted at: 2017-10-20T22:41:38.840Z Reads: 410

```
@chinzw Yeah it should work with any standard ESC :-)
```

---
## \#374 Posted by: Clonkex Posted at: 2017-10-20T22:44:35.943Z Reads: 415

```
Fantastic! I'm so glad you agree about that! It shouldn't be super difficult to do either.

It's surprisingly uncommon to see another person who's experience in CAD, programming AND electronics. It's really awesome! Fellow jacks-of-all-trades unite!
```

---
## \#375 Posted by: banjaxxed Posted at: 2017-10-20T22:48:15.360Z Reads: 411

```
This is amazing I'd like to try making one or two, can you link to the replacement resistors and caps on alibaba as well?

Secondly is there a problem with making a cart just on alibaba? Component quality maybes 

Thirdly is a larger oled screen a possibility?
```

---
## \#376 Posted by: chinzw Posted at: 2017-10-20T22:52:33.751Z Reads: 404

```
@Clonkex not really, vesc has uart, which is used by this remote to get data, and can also be used to control the vesc.
```

---
## \#377 Posted by: solidgeek Posted at: 2017-10-20T23:04:43.153Z Reads: 426

```
@Clonkex I agree, it's not a big change :-) Maybe you are right, I just try to learn myself everything I need to do a specific task - and it helps a lot that the task itself is exciting! ... Jacks-of-all-trades that's a new one :D

@banjaxxed Well you just need a single 220uF cap for the 5V input on the receiver side, and the replacement resistor (for the charger) is a 5kOhm SMD (1603/0603) resistor, however, if you never soldered SMD I recommend just getting an ordinary through-hole resistor. No need to buy this on alibaba or aliexpress, just find a local shop :slight_smile: 

A larger OLED screen is not possible at the moment, as the whole GUI is designed around the 128x32 px display.

@chinzw It will be possible to change between three modes: PPM only, PPM and UART and  UART only. The PPM mode will be used to run any ESC :slight_smile:
```

---
## \#378 Posted by: banjaxxed Posted at: 2017-10-21T14:58:56.872Z Reads: 421

```
makes sense now, thank you

I've started the slow boat, maybe will have one working for xmas, I hope :slight_smile:
```

---
## \#379 Posted by: mptrs Posted at: 2017-10-22T08:26:46.853Z Reads: 453

```
Been following this one for a while and it looks great. Will print and build it soon.

And a small tip will be send soon as well.
```

---
## \#380 Posted by: banjaxxed Posted at: 2017-10-22T08:40:13.485Z Reads: 460

```
I'm almost certain there wasn't a poo stl in the combination I merged
<img src="/uploads/db1493/original/3X/0/3/0319b5486cf0039674d42ab7c6c756e9ce43ba70.JPG" width="666" height="500">
```

---
## \#381 Posted by: High-roller Posted at: 2017-10-22T09:01:15.387Z Reads: 448

```
You... printed a potato...?
```

---
## \#382 Posted by: banjaxxed Posted at: 2017-10-22T09:02:24.031Z Reads: 458

```
I'm Irish, we find it more ergonomic if `<item> ` is potato-shaped

Try again - ABS 101% scale with brim
<img src="/uploads/db1493/original/3X/8/7/87e60430a54a884fa54a98a5a2e78ce0cb335df0.JPG" width="666" height="500">

**edit:** both top and bottom shell pieces are the  same direction and impossible to close against each other, so you will have to mirror one of them, then flip, JFI

Also you may need to build the Mr Happy Face...I mean throttle with support.

It just occured to me and maybe this is a 3D newbie duh, any lefties out there can use that mirror-flip proceedure to make a left handed remote!
```

---
## \#383 Posted by: High-roller Posted at: 2017-10-22T09:04:51.715Z Reads: 447

```
Supposedly they also make great batteries.
<img src="/uploads/db1493/original/3X/5/8/584945c0784afbace9e3472201695726cebe3b57.jpg" width="300" height="168">
```

---
## \#384 Posted by: banjaxxed Posted at: 2017-10-22T09:05:41.470Z Reads: 447

```
Self charging remote? Kickstarter!
```

---
## \#385 Posted by: solidgeek Posted at: 2017-10-23T21:27:47.405Z Reads: 440

```
@mptrs Thanks mate, I'm glad you like it! 

@banjaxxed What a mess, haha :P Second attempt looks good, did I forget to mirror the top? Thanks for notifying me - I will add it to my ever-growing to-do list :-)! If you mirror the remote to make a lefthanded version, the display will not be placed in the right way (the screen itself is not in the center on the board).
```

---
## \#386 Posted by: banjaxxed Posted at: 2017-10-23T22:23:01.392Z Reads: 433

```
I twigged that I think I made a leftie, the screen is on my right hand palm side I should have mirrored and flipped the other case side instead!

I'll notch it up to a learning curve also made a very nice active cooling addition to my dual extruder so expecting even better results but might use nylon instead of ABS 👌
```

---
## \#387 Posted by: Clonkex Posted at: 2017-10-23T22:29:51.202Z Reads: 411

```
Why not print it in PLA? Way easier and well and truly strong enough for a hand-held remote.
```

---
## \#388 Posted by: banjaxxed Posted at: 2017-10-23T22:30:56.925Z Reads: 407

```
I had the Abs ready to roll the pla on the other roll I'm not happy with
```

---
## \#389 Posted by: Clonkex Posted at: 2017-10-23T22:50:42.018Z Reads: 402

```
Fair enough :thumbsup:
```

---
## \#390 Posted by: Tathers Posted at: 2017-10-24T02:26:25.764Z Reads: 401

```
@solidgeek any ETA on when the ESC/VESC end of the github will be updated?
```

---
## \#391 Posted by: egzplicit Posted at: 2017-10-24T08:33:12.547Z Reads: 435

```
@solidgeek @Clonkex glad you like my idea. Just another suggestion, if you decide to store the pipe address on the eeprom. If by accident one receiver pairs with another remote during startup, and you store the pipes, then the two will be forever paired. Also if somebody loses their remote / changes the receiver, there will be no way to pair them.

However, if you still want to store the pipes, I would suggest another bit of code that monitors the pairing process in the setup. After a long timeout (for example 1 or 2 minutes), if it can't pair, both the remote and receiver should erase the pipe address from the eeprom and reset it to the default one. This way if a cross pair happens or somebody replaces their remote/receiver, they can still pair the two. Just turn both on and leave them on for a while, then the timeout occurs and the default pipe is used again.

@solidgeek I'm interested in a beta unit as well, is there more room for one? (I'm in London, UK). I'm a software engineer and could help contributing to the codebase with a couple of PRs. I can source most of the electronics and put it together myself, getting a good 3D printed enclosure is the hardest part. If there is more room, I'd be interested in one beta remote to help with the coding and debugging/testing.

Thanks!
```

---
## \#392 Posted by: solidgeek Posted at: 2017-10-24T19:27:14.994Z Reads: 436

```
@Tathers I have been working on the newest version with pairing and unique nRF24 addresses. I got a few hours left of coding for sure, however, I think I will be ready to release this weekend :slight_smile:

 @egzplicit I like your ideas :P I have been thinking about the same problem for quite some time now. I am not sure that a timeout is the best solution. This is because you could easily forget to turn off your remote and having the remote using the default pipe next day without you knowing. Another option, I think would be better is to make a pairing procedure, and adding a little tactile button on the receiver to enable this. In this way, you can pair your remote and receiver, and save the pipe to both EEPROMs. In pairing mode, the receiver will listen on the default address, while waiting for a new pipe sent by the remote. This way you can always repair, and chances for pairing with a wrong remote is second to none. What do you think of this?

@egzplicit  I am sorry I have already promised more than I am able to produce at the moment. I would love to get you one... I could surely use some fellow engineering support. If you want I can definitely print all parts for you, and maybe sell you some of the modules (I got some of them in spare). 

Thanks for your support :slight_smile:
```

---
## \#393 Posted by: Clonkex Posted at: 2017-10-24T21:32:01.330Z Reads: 391

```
@solidgeek That's exactly what I was thinking, a small push button on the receiver for pairing mode. +1
```

---
## \#394 Posted by: egzplicit Posted at: 2017-10-25T08:38:02.219Z Reads: 410

```
@solidgeek thanks! For some reason i though the restriction is not having a button on the receiver. This is why I tried to come with a solution without any other physical components. The timeout would work without the switch but yes, if you decide to have one, your solution is much better. 

A temporary switch will work nicely: press it them turn on the board and the setup() routine will see it being pressed and the receiver will enter pairing mode on the default pipe. Then put the remote into pairing mode as well (via the menu) and the process starts.

That's ok about the betas, the 3d printed parts are the hardest for me so if you can help me with those it would be great. I can buy most of the components, however, if you have some extra parts, I don't mind buying from you and save some time (shipping from china takes forever). I'll PM you.
```

---
## \#395 Posted by: ervinelin Posted at: 2017-10-26T01:28:25.321Z Reads: 407

```
Awesome work with finding ways to deal with the pairing!

While I wait for the latest code, I wanted to start 3D printing the enclosure, however I noticed that there was a "newer version" with the knob on the thumbwheel, has that version been uploaded to thingyverse yet?

If that was the only change made then I can probably adjust the model myself but I wasn't sure if there were other updates.

One other question I had was, if I am running dual VESCs, I assume I need to use the CAN bus between the two so that I will be able to read data from both simultaneously?
```

---
## \#396 Posted by: Mozillum Posted at: 2017-11-02T11:21:17.458Z Reads: 401

```
Any updates on the complete tutorial @solidgeek? :grinning:
```

---
## \#397 Posted by: karatektus Posted at: 2017-11-03T21:18:23.699Z Reads: 415

```
Is there a specific reason, why you dont use the nrf24 module with the trace antenna? its way cheaper :D
[link](https://de.aliexpress.com/item/Free-shipping-SMD-NRF24L01-wireless-data-transmission-module-Mini-NRF24L01-wireless-module/32642004648.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10344_10345_10547_10342_10343_10340_10341_10548_10193_10194_10541_10304_10307_10060_10302_10155_10154_10056_10055_10539_10537_10536_10059_10534_10533_100031_10103_10102_10142_10107_10320_10321_10322_10084_10083_10177_10180_10312_10313_10314_10184_10319_10550_10073_10551_10552_10553_10554_10186_10557,searchweb201603_25,ppcSwitch_4&btsid=1618bfc4-bf6b-4a6f-99c2-6e845988f2c0&algo_expid=dac20527-7959-44b7-b8f7-2c3011f22b3f-2&algo_pvid=dac20527-7959-44b7-b8f7-2c3011f22b3f)
```

---
## \#398 Posted by: banjaxxed Posted at: 2017-11-03T21:33:12.532Z Reads: 424

```
The thumb wheel does have a knobbed profile on thingiverse
```

---
## \#399 Posted by: karatektus Posted at: 2017-11-04T18:12:58.366Z Reads: 442

```
Had a little go at modifying at least the main screen to a larger oled. can anyone edit the stl? :D<img src="/uploads/db1493/original/3X/0/6/06ab3e25aea272439c32c81d4ad6a588a0f6fa31.jpg" width="375" height="500">
```

---
## \#400 Posted by: karatektus Posted at: 2017-11-05T12:05:20.421Z Reads: 427

```
Hmmmm I just noticed. 
The display takes up pretty much all of the looptime. so displaying more increases the looptime. (150ms in my case) Thats just too much for such a time critical application. 
I was thinking about a second arduino in the remote just to drive the display? Either that or a 32bit micro controller like this one: [ali link](https://de.aliexpress.com/item/Teeny-3-1-Teensy-3-2-Teensy-2-0-USB-Keyboard-Mouse-Teensy-AVR-experiment-board/32804448852.html?ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10344_10345_10547_10342_10343_10340_10341_10548_10193_10194_10541_10304_10307_10060_10302_10155_10154_10056_10055_10539_10537_10536_10059_10534_10533_100031_10103_10102_10142_10107_10320_10321_10322_10084_10083_10177_10180_10312_10313_10314_10184_10319_10550_10073_10551_10552_10553_10554_10186_10557,searchweb201603_17,ppcSwitch_4&btsid=f300b23e-fac2-4212-861f-8477f785b19c&algo_expid=69fb52d5-9129-4c7d-b6e1-c8765c7f9786-3&algo_pvid=69fb52d5-9129-4c7d-b6e1-c8765c7f9786) (which is way more expensive)

 thoughts?
```

---
## \#401 Posted by: vishal_tejwani Posted at: 2017-11-05T12:26:41.240Z Reads: 419

```
Use atmega 328 which is compact for such things, if possible go for attiny85 i think there is some way for it to.work with nrf
```

---
## \#402 Posted by: solidgeek Posted at: 2017-11-05T20:35:19.184Z Reads: 416

```
Hey, sorry for the late answer, I've been busy at work and school. I am currently working on a big update for the software - to be released soon I hope (lol).

@egzplicit Actually I am not even sure if the button is necessary, I believe I can make it work by transmitting a struct with a updateSettings variable in it or something like that :-) To be continued... 

@ervinelin I am positive the newest version is online at Thingiverse :-) Regarding the dual VESC setup, you won't be able to read data from both at the same time - the remote only needs one data source. If you connect your two VESCs by CAN bus, I think everything should work just fine.

@Mozillum I am currently looking for a way to borrow a good camera / video-recorder. However that is it, sorry :(  

@karatektus I use the module with a ceramic antenna because it is more stable (mainly because of the PA/LNA). I am sure you can use a normal nRF24 module ;) And nice work modifying the display :D However I am not sure if it is even possible to fit that display inside the remote? It looks kinda big. Regarding the delay caused by the display, I have been planning to optimize that part heavily. Any ideas regarding that? Without adding another microprocessor ;)
```

---
## \#403 Posted by: karatektus Posted at: 2017-11-05T20:58:57.711Z Reads: 436

```
well the first thing would be to remove all the backgroundelements from the loop. no need to redraw the text everytime. no ideas otherwise. im a webdeveloper. resources arent normally a problem for me :D
i guess id just use a different arduino. ill order it and give it a shot. i wouldnt really mind the extra $10.
Edit: Thinking about it for another five minutes: You should only draw a new number if necessary (if it differs from the old value) but that wouldnt help much when you break or accelerate hard. which is when its the most critical ^^

The bigger display should just fit could you remove the little ledge in there and increase the height of the cutout to twice the current height? if you are too busy im gonne bodge it together with openscad or something :D

<img src="/uploads/db1493/original/3X/e/6/e60c28dc21140681ba76dc5f0b02a5d9042530ee.jpg" width="666" height="500">

(its maybe a little tight but you can easily shave a little from the pcb off ^^ )
```

---
## \#404 Posted by: ervinelin Posted at: 2017-11-06T02:46:46.654Z Reads: 413

```
Awesome, I was planning to put this together tomorrow on my day off. Already got 90% of the parts in and 3D printed all the necessary files (my 3D printer is very bad for small objects though, so having problems fitting everything nice and snug).  You are right about the wheel with the knob, it's in Thingiverse already, my bad.

I am assuming I can just run the current code and I can update it as and when you have uploaded the new version.
```

---
## \#405 Posted by: DjamboBuksne Posted at: 2017-11-06T13:19:50.523Z Reads: 393

```
Can you  send me the code for larger 64*128 display? Please!!
```

---
## \#406 Posted by: DjamboBuksne Posted at: 2017-11-06T13:21:37.589Z Reads: 391

```
I will try to redesign the top to fit the larger display...
```

---
## \#407 Posted by: karatektus Posted at: 2017-11-06T15:27:50.263Z Reads: 389

```
ill rework it a little so it doesnt break compatibility with smaller displays and create a fork tonight.
(Edit - maybe not all tonight its kind of a lot of work :D)
```

---
## \#408 Posted by: DjamboBuksne Posted at: 2017-11-06T16:19:02.704Z Reads: 389

```
Is it complicated or just a lot of work? Myb I can help... I have a longboard without a remote but i have all of the parts for this remote, just larger display
```

---
## \#409 Posted by: karatektus Posted at: 2017-11-06T16:21:45.620Z Reads: 398

```
[quote="DjamboBuksne, post:408, topic:28543"]
just a lot of work? Myb I can help... I have a longboard without a remote but i have all of the parts for this remote, just larger display
[/quote]

if you just quickly need the code i can send it to you no problem.
```

---
## \#410 Posted by: DjamboBuksne Posted at: 2017-11-06T16:29:29.100Z Reads: 380

```
Yes please.
```

---
## \#411 Posted by: DjamboBuksne Posted at: 2017-11-06T22:43:51.179Z Reads: 385

```
Can you upload it to the google drive or something and then post the link?
```

---
## \#412 Posted by: karatektus Posted at: 2017-11-06T23:23:33.399Z Reads: 398

```
Really sorry - I was busy!
here you go: https://github.com/karatektus/nRF24-Esk8-Remote

keep in mind that performance is poor and it needs optimizations
```

---
## \#413 Posted by: DjamboBuksne Posted at: 2017-11-06T23:33:40.868Z Reads: 424

```
Thank you so much! I will try to redesign the remote to fit that larger screen<img src="/uploads/db1493/original/3X/2/9/2929173439e92f8932bef7e68d95aaa4dca17315.jpg" width="375" height="500">...
```

---
## \#414 Posted by: ervinelin Posted at: 2017-11-07T09:54:02.619Z Reads: 426

```
So I spent the whole afternoon building this.. boy that's a lot of tiny wires!!! Had a lot of fun building this but it's not easy especially when my printer spits our very rough prints.

<img src="/uploads/db1493/original/3X/6/6/662748f32f13d54786860e59f617b919fb7194be.JPG" width="601" height="500">

I THINK it's working but I haven't built the receiver yet so I have no idea if this is working.

<img src="/uploads/db1493/original/3X/6/1/61f9c1b1b8aed5ffd4d1852896b30617d56ebe9f.JPG" width="690" height="349">

I see that when I press the trigger and move the throttle a little bar moves up and down (not the full range) but that's all I got it to do...

Is there something I need to do to further set it up, calibrate, etc?

Thanks again!
```

---
## \#415 Posted by: solidgeek Posted at: 2017-11-07T11:09:03.496Z Reads: 414

```
Looks good! Its a lot of fun to build :-D You can enter and change settings by holding the trigger while turning on the remote. In the settings you can change the hall min, max and center values, to match your magnets and print. If you activated debug (in software) and open up serial monitor, I believe it should print out the hall sensor values. This way you can calibrate the remote. I am adding a function for this in the next big software update :smile:
```

---
## \#416 Posted by: HighMasterGogo Posted at: 2017-11-07T11:47:41.457Z Reads: 402

```
Bought all the items from your BOM and I'm printing the parts tonight; thanks for creating such an awesome remote @solidgeek!
```

---
## \#417 Posted by: ervinelin Posted at: 2017-11-07T13:54:26.659Z Reads: 411

```
Hm... So I pressed the trigger and turned on the remote. It shows remote settings then goes into a single page called Trigger.

Pressing the trigger just shifts the zero left and right. Wheel does nothing. No other options available. 

What am I missing? Or do I need to connect to the receiver for this to work?

Lastly. I assume the connection between Arduino and NRF module for the receiver is the same as the transmitter?

Thanks again...
```

---
## \#418 Posted by: solidgeek Posted at: 2017-11-07T16:59:11.786Z Reads: 425

```
@HighMasterGogo Glad you like it mate :-) Looking forward to see your build!

@ervinelin At least you entered the settings! Clicking the trigger enters and exits the selected setting, while the throttle is used to select and change setting values. So if the throttle doesn't change anything, something is wrong :P I got a few ideas.

1. **The polarity isn't opposite**. Check the polarity of the magnets, they have to be opposite (one being north and the other being south). If they aren't opposite, drill a small hole beneath each magnet and push them out.

2. **Magnets are weak / min and max are to high**. By default, the min and max values are 0 and 1023. To change the settings on the remote the input has to be _input = maxHallValue - 50 = 973_ or _input = minHallValue + 50 = 50_. 
If your magnets are a bit weaker than mine, the hall sensor will output a smaller value (voltage), and therefore not high enough to change settings. To check this, enable debug and plug-in a USB for debugging through Serial monitor :slight_smile: I have just added a debug-message for the Hall sensor value to the transmitter software - so remember to use the newest version on Github

<img src="/uploads/db1493/original/3X/7/2/72ee624ccb7357ebc04ec6182609133cacca052b.png" width="690" height="231">

You just have to uncomment #define DEBUG, and read the output in Serial monitor. Let me know :-)

<img src="/uploads/db1493/original/3X/5/0/507d0054fed2d24ca0099a2ab9c7dbdfc6bdee11.png" width="600" height="449">
```

---
## \#419 Posted by: ervinelin Posted at: 2017-11-07T17:14:53.154Z Reads: 408

```
[quote="solidgeek, post:418, topic:28543"]
maxHallValue
[/quote]

AH I was wondering why I couldn't see the hall sensor value in the serial monitor!

Okay it looks like magnets are too weak, I'm getting 350-700 at the extremes.

I don't see where I can adjust this in the code manually though.

EDIT: Okay I think I got it...
```

---
## \#420 Posted by: ervinelin Posted at: 2017-11-07T17:37:03.015Z Reads: 402

```
Okay I managed to calibrate the thumb wheel.

Now one slight problem I noticed is that the trigger is always set to "kill switch" mode, I've gone into the settings and changed it from 0 to 3 (kill switch to data toggle) but it remains as "kill switch".

The bigger problem is I can't get the transmitter to connect to the receiver... :frowning:

I double checked the connections, made sure the pipe addresses were the same as well. Still nothing, serial monitor shows "Failed Transmission".

Any ideas?
```

---
## \#421 Posted by: tueboard Posted at: 2017-11-08T00:06:08.722Z Reads: 419

```
anyone found another source to buy the Hall-Effect sensor (SS495A) ? shipping to spain is crazy expensive 20€

this one can work?
http://www.ebay.es/itm/1Pcs-Ss495a1-Ss495a-Capteur-A-Letat-Solide-Nouvelle-Ic-M/162656960806?hash=item25df1c4126:g:vzYAAOSwZr9ZquZO
```

---
## \#422 Posted by: ervinelin Posted at: 2017-11-08T05:07:41.531Z Reads: 412

```
I got mine here... 

5pcs/lot SS495A1 95A TO-92 high-precision Hall sensor SS495A screen 95A new original
 http://s.aliexpress.com/UzQJJ73U 
(from AliExpress Android)
```

---
## \#423 Posted by: banjaxxed Posted at: 2017-11-08T10:06:27.234Z Reads: 415

```
It ain't easy bro
<img src="/uploads/db1493/original/3X/b/7/b723995b96f82decbe56002913c2d5d29b6dedab.JPG" width="375" height="500">
```

---
## \#424 Posted by: HighMasterGogo Posted at: 2017-11-08T10:26:44.973Z Reads: 426

```
Yes it is! :grin:

<img src="/uploads/db1493/original/3X/5/0/505d6749c73bc554304d622686256ee9deada012.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/a/0/a00ec2ebaf200b9806f033be2094e8581440d161.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/5/6/567c1e75849b52fe1992a47636ae51fbddd542cb.jpg" width="666" height="500">

Sorry @banjaxxed, probably not what you want to hear! It looks like you've got some skipped steps there. Did you print from your PC over USB or an SD card? I had skipped layers when I tried to print from my PC. 

Super impressed with the model. It's very well planned out and modeled.
```

---
## \#425 Posted by: banjaxxed Posted at: 2017-11-08T11:31:11.500Z Reads: 401

```
Heh no I use astroprint loaded up with x3g files created with slicer I adjusted the flow to increase since my printer seems not to like pla, I think it hit off some layer during the night and popped over some belt teeth hence the stepping effect, I'm adjusting to fix that have managed a decent print in abs
```

---
## \#426 Posted by: HighMasterGogo Posted at: 2017-11-08T11:40:02.665Z Reads: 395

```
Cool, sounds like you're on the case. Make sure you post it up when you get a successful print.
```

---
## \#427 Posted by: Clonkex Posted at: 2017-11-08T12:07:59.900Z Reads: 383

```
Wow yours is really nicely printed! Looks good, show us the finished product when you get that far :D
```

---
## \#428 Posted by: HighMasterGogo Posted at: 2017-11-08T12:19:22.785Z Reads: 375

```
Thanks @Clonkex! I'm really amazed with the model, props to @solidgeek. The two sides slot together perfectly!
```

---
## \#429 Posted by: karatektus Posted at: 2017-11-08T13:51:27.918Z Reads: 388

```
[quote="banjaxxed, post:425, topic:28543"]
reated with slicer I adjusted the flow to increase since my printer seems not to like pla, I think it hit off some layer during the night and popped over some belt teeth hence the stepping effect, I'm adjusting to fix that have managed a dec
[/quote]

I had skipped steps becaus one of my motor drivers got to hot and failsaved.adding pc fan on top solved the problem (or decreasing the motor current and therefore printspeed)
```

---
## \#430 Posted by: banjaxxed Posted at: 2017-11-08T14:00:09.115Z Reads: 405

```
I have a dual with twin fans and a third as a blower onto the nossle openings, I've added a 1mm plate of glass fibre this morning...no more hairspray 🤣

This is great @solidgeek thanks

Trying again with a light blue abs but just realised I used the same stl as last time, so I will have two for the leftorium
```

---
## \#431 Posted by: mptrs Posted at: 2017-11-08T16:06:57.115Z Reads: 425

```
Finishing up one part in yellow to make it look like I'm just holding a banana :smile: 
Forgot to set it to 50% infill, but don't think 20% will be a problem.
Now to order me some electronics and build this fine looking remote.

Donation done!

<img src="/uploads/db1493/original/3X/d/e/dea5b7f0e36442a472692619fdfe697aeb17bcfa.JPG" width="375" height="500">

_Printer under extruded one layer and I broke it hehe, let's print again and hope my printer doesn't fail now._
```

---
## \#432 Posted by: HighMasterGogo Posted at: 2017-11-08T16:29:54.144Z Reads: 394

```
Wow a proper Prusa i3! They are lovely machines. Mine is a custom i3 clone.
```

---
## \#433 Posted by: solidgeek Posted at: 2017-11-08T21:28:54.622Z Reads: 414

```
@ervinelin Well okay... That's some very low values, however, it shouldn't be a problem as long as the min and max values are set correctly :-) The Trigger options aren't used in the software just yet, I hope to include it in the next update. Regarding the transmitter, it's hard to tell however here is a few things to remember:

1. The receiver needs **5V directly on the 5V rail** or 7-12V on the VCC rail. If you supply 5V to the VCC it will drop beneath the 3.3V regulator min-voltage-input - and not be able to supply the right amount of voltage.  

2. I recommend adding a **220uF cap on the receiver 5V rail**

3. The nRF24-module should be connected **to 3.3V**

4. **Shield the module from the wires underneath**. Wrap some aluminum foil around the wires going under the nRF24-module.

5. Try **shielding the nRF24-module**. First, wrap some isolating material (plastic or shrink wrap) around the module. On top of the isolating material, add a layer of aluminum foil around the module - remember to keep the antenna free. This helps remove electromagnetic noise from the wires beneath and around the module, which in some cases causes problems.

5. Double check the wires and the connections, it should work :P

Let me know.

@banjaxxed try printing one part at the time ;-) 

@HighMasterGogo Looks beautifull! I am glad you like the model - it took some hours to make :P Thanks

@mptrs Looks good mate! The 20% shouldn't be a problem, however the LEDs will probably shine through ;) ... Thanks, but I don't see any donation, you sure :dizzy_face: ?
```

---
## \#434 Posted by: Jammeslu Posted at: 2017-11-08T21:32:11.350Z Reads: 389

```
not to stress but when can we expect to assembly video to be made?
```

---
## \#435 Posted by: mptrs Posted at: 2017-11-08T21:38:16.332Z Reads: 383

```
Did it via the paypal.me, but it's still on being processed.

Printing it again tomorrow in translucent blue, so everything will be visible hehe. Can't get the yellow to print cleanly.
```

---
## \#436 Posted by: solidgeek Posted at: 2017-11-09T07:22:55.886Z Reads: 391

```
@Jammeslu Probably not gonna make a video, but a guide for all steps is in my mind. 

@ervinelin I just realised that I have changed the CE and CS pins on the receiver, at some point. If you wired the nRF24 receiver the same as the transmitter, that will for sure cause problems. 

I have updated the receiver code, hope it helps :P 

<img src="/uploads/db1493/original/3X/2/a/2a319d94cdd8d8cdf00acbbb0fb70a93d2bc5951.png" width="690" height="90">

Try the new software out first!! :P
```

---
## \#437 Posted by: ervinelin Posted at: 2017-11-09T17:39:44.822Z Reads: 406

```
Thanks @solidgeek!

But here's the thing, the diagram in your wiki showed pins 9 and 10 connected, not 7 and 8...

So I actually swapped the code back to 9 and 10 and FINALLY I got the transmitter to talk to the receiver!!!

I checked with the VESC app to see if there was a signal and indeed there was!

Now the next problem. The signal is very very very sketchy, one second it's there, the next it is not. I have yet to shield the NRF modules but I am surprised the signal is so bad.

Also, the min and max pulsewidth as seen in the VESC app are wildly off what I used to have, what used to be 1 and 2 is now something like 0.8 and 0.9. Is this normal?

Thanks again, really stoked that at least I got some movement... just for some reason it's a really really sketchy signal, I'll try shielding next.
```

---
## \#438 Posted by: solidgeek Posted at: 2017-11-09T18:54:06.192Z Reads: 395

```
Haha okay, well I am a big mess  :smile: I will edit the schematic, the pins should be the same, it makes more sense. 

Regarding the sketchy signal, it is probably power or noise related. How are you supplying power to the receiver? It's important to add a big capacitor on the 5V rail if you are powering the Arduino from a VESC. If it's a noise issue, try to take out the transmitter module, and move it away from the remote. If this helps, you could try shield the wires or nRF24-module. 

The 0.8 and 0.9 pulse width seems weird, however, I am not sure because I have never tested the remote on a VESC 4 (please provide a picture). 

Most issues are fixed by adding some capacitors or shielding the transmitter. A few pictures of your setup, with wiring etc. would help me fix your issue :-)

EDIT: The problem may be that I have fucked up the pins in software. In transmitter.ino I have written _RF24 radio(7, 8);_ however according to my schematics, it should be pin 9 and 10. I will change both the transmitter code AND receiver code to use pin 9 as CE and pin 10 as CS. Maybe this helps :P
```

---
## \#439 Posted by: mptrs Posted at: 2017-11-09T22:12:47.528Z Reads: 378

```
Just a heads up, but 0.20mm worked best for me. Slic3r had some trouble with 0.15mm. Now I got one side 0.15mm 50% and the other 0.20mm and I think 20% but could be 50% as well. Not sure my OCD can handle this hehe.

As for the design I have to give you mad probs, it fits together perfectly! Now I'll wait for the 11th to order the things from Ali cause there is discount on some of the items. (yeah I'm Dutch hehe)
```

---
## \#440 Posted by: karatektus Posted at: 2017-11-10T10:17:02.854Z Reads: 377

```
Any progress on this? :)
```

---
## \#441 Posted by: ervinelin Posted at: 2017-11-10T18:39:03.832Z Reads: 417

```
Progress!

So I shielded both transmitter and receiver NRF modules with copper tape and that seemed to work. When connected I can get a few meters away before I lose connection (good enough for esk8).

Now the problems:

* Noisy PWM signal - PWM signal seems awfully noisy, I'm still getting that strange pulse width range (now it's about 0.4 - 0.9) and the throttle position doesn't seem consistent all the time. However I suspect it's my magnets, I have better ones coming in so hopefully that will help.

* Receiver needs reboot to connect - Receiver does not connect when I turn on the board, but connects almost instantly when I reboot the ardunio via on-board reset button - I suspect this might be a timing issue between when it's powered on and when it looks for the signal to bind to the transmitter?

* No UART data - This really is the only reason why I built this controller, but I'm getting nothing, I assume in the remote settings UART should be set to 1(0 didn't work either), then in VESC I set it to PPM & UART. I then connect Tx on the arduino to Rx on the VESC and vice versa. Anyone know exactly which pins are these on both the VESC and Arduino? Also does this work for every VESC out there? I'm using the Hobbyking VESC.

Thanks again for the help!
Erv.
```

---
## \#442 Posted by: chinzw Posted at: 2017-11-10T19:00:17.583Z Reads: 401

```
Check the baud rate on the VESC matches the one on the receiver, otherwise it wont be able to read the uart data.
```

---
## \#443 Posted by: ervinelin Posted at: 2017-11-10T19:14:25.696Z Reads: 418

```
In the receiver Arduino code it looks like it's set to 115200, so I already set this in VESC but no go.

On a more positive note... <img src="/uploads/db1493/original/3X/e/0/e0e1d1391205a4b3ba8f26848d19a6fe8f9f12e0.jpg" width="281" height="500">
```

---
## \#444 Posted by: mptrs Posted at: 2017-11-11T10:11:19.260Z Reads: 400

```
Everything ordered! And now we wait.

Don't forget guys it's singles day, so nice discounts on aliexpress
```

---
## \#445 Posted by: solidgeek Posted at: 2017-11-11T23:04:08.000Z Reads: 402

```
Good to hear you got some progress :slight_smile: Well I got +20 meters of range with my remote, so you are probably doing something wrong :P

Let's see. You got a noisy PWM signal, and low range. I am 95% sure its a power issue. How is you receiver connected to your VESC? It's crucial that the receiver is connected to 5V and GND, with a big ass capacitor on the 5V rail. The VESC (or any ESC) doesn't have a very stable 5V output, and it isn't capable of supplying huge current pikes. The 220uF or higher helps with that. And it is important to remember that the 5V from VESC should go to the 5V pin on the Arduino, not the VCC pin. 

Regarding the UART, which library are you using? 

I will need some pictures of your wiring / and or setup to better help you :-) And some pictures of your VESC would be great too :P
```

---
## \#446 Posted by: Snowi Posted at: 2017-11-12T00:30:55.122Z Reads: 392

```
Can this be used on DIYelectricskateboard's vesc? If so, what are the connections I need and which ports do I connect them to?
```

---
## \#447 Posted by: ervinelin Posted at: 2017-11-12T00:40:15.278Z Reads: 432

```
Hi again,

Actually a few meters was through a wall, furniture and such, I never bothered to test any further than 6m out in the open.

Power for receiver is via VESC signal cable, 220uF installed and buffering across the Arduino 5v and ground not VCC.

Actually on riding it I don't sense the noise at all, it seems nice and smooth so for now I will leave it as it is.

As for pairing, any idea why sometimes I need to reset the receiver to get a lock? Quite irritating when the receiver is hidden inside the enclosure.

I am using the rollinggecko library and this was installed and flashed to the ardunios, but was I supposed to flash this somehow to the VESC as well?

I will send a picture over but not at home these few days. Will do so when I can.

Thanks again..

EDIT: Huston, we have telemetry... <img src="/uploads/db1493/original/3X/b/8/b8803b5e0a69c2034be7ed3b14761255a461c92d.jpg" width="281" height="500">

Turns out I was using the right tx and Rx pins originally then I swapped them out before changing the baud rate... Now all seems good awaiting more testing
```

---
## \#448 Posted by: mptrs Posted at: 2017-11-12T11:48:34.317Z Reads: 414

```
@solidgeek I mirrored everything to make it a lefty remote. I know the text on the screen might be upside down, but that's no problem for now.

But are there code changes needed for the hall sensor? If so can you let me know where so I can change them in the fork I made on github. Or a setting might be nice, that way the screen layout can be changed as well.

When I build the remote and receiver I want to take a closer look at the code anyways, to see if I can help. Might be able to document my build proces, at least I'll try.
```

---
## \#449 Posted by: escu_12 Posted at: 2017-11-12T15:26:12.871Z Reads: 412

```
a question, in the receiver, what is the schematics?
```

---
## \#450 Posted by: ervinelin Posted at: 2017-11-12T16:31:12.365Z Reads: 442

```
So I just came back from a 5km ride to test the remote. I am happy to say that it didn't have a single dropout. Telemetry worked perfectly as well.

<img src="/uploads/db1493/original/3X/2/a/2a3bd5ccfba5339c53d73246eee66f2d810ad3c5.jpg" width="281" height="500">

For those who want to wire up the receiver, the NRF module wires up exactly the same as in the schematic on the wiki for the transmitter. Then add in a 220uF cap to 5v in and ground, pwm signal to D5 and vesc uart pins to the tx and Rx.

For me I draw 5v from the VESC servo lead.

Took some photos of the second receiver I wired up for reference to anyone who's interested.

<img src="/uploads/db1493/original/3X/8/4/84d6b19ba4881b07f5f8274633403c937933c729.jpg" width="281" height="500">
I used some hotglue to hold the delicate 30awg cables together

<img src="/uploads/db1493/original/3X/e/6/e6ff4309f9d4792c68ff0d3691af825bd7123ab8.jpg" width="281" height="500">
Shielding with copper tape

<img src="/uploads/db1493/original/3X/5/0/500bbc4ac0abcc295a68ea3cefe2f4f36bf2f814.jpg" width="690" height="388">
Heat shrunk both into one compact package.

For some weird unknown reason, the last step has solved the problem of occasionally not being able to connect on a cold boot and requiring a hard reset on the receiver.

Can't wait for the new firmware to add more bells and whistles.
```

---
## \#451 Posted by: Snowi Posted at: 2017-11-12T19:00:23.651Z Reads: 403

```
Anyone else got a place to buy 20mm springs that ship to the US? The one on the google sheets cannot ship to the US. :/
```

---
## \#452 Posted by: solidgeek Posted at: 2017-11-12T19:01:01.570Z Reads: 424

```
@Snowi Yes they should work with most VESCs, however I haven't tested one myself :-) The receiver needs only 3 pins (5V, GND and PPM) - however can also be connected to UART (RX, TX), to retrieve data such as speed and battery voltage.  

@mptrs The changes I made lately on Github is important, I recommend you change them too - you should be able to see the changes on Github yourself :-) ? However a big software update is coming soon, so stay tuned :wink: 

@ervinelin I am so glad you got it working! It looks amazing, thanks for sharing your process - I am sure it will help a lot in the future :D Love your compact receiver, I will probably make a 3D-model for the receiver in the near future. 

Hopefully I am able to finish the new firmware by next week :slight_smile:
```

---
## \#453 Posted by: solidgeek Posted at: 2017-11-12T19:08:46.710Z Reads: 403

```
I am sure you can find an US supplier :-) They are called "Extension springs", I found a local shop with some, and they have a length of 20mm, a width of 5.5mm and a wire width of 0.5mm: https://www.conradelektronik.dk/?websale8=conrad-dk&pi=889250
```

---
## \#454 Posted by: mptrs Posted at: 2017-11-12T21:16:38.059Z Reads: 401

```
These should work: https://www.aliexpress.com/item/20PCS-0-5-x-4mm-0-5mm-Tension-spring-with-a-hook-extension-spring-length-15mm/32801604704.html
I've ordered them for this build.

@solidgeek pulling in all changes to your repo by pull request :)
```

---
## \#455 Posted by: MontPierre Posted at: 2017-11-13T14:23:15.917Z Reads: 392

```
@ervinelin thanks for detailed post. How’s throttle range working for you? I have my model printed and all parts but throttle range seems very limited and the spring action is a little too hard for me to push. I got same spring as in the spreadsheet, maybe I need to loosen it up a bit.
```

---
## \#456 Posted by: Migro Posted at: 2017-11-13T20:32:29.788Z Reads: 416

```
Hi guys i saw some one use the other nrf module but would it work like the one you have in the spreadsheet? (already have a few). <img src="/uploads/db1493/original/3X/1/e/1ed47c48bb48fee76fbc4c9cc9fc3e89fdb823ae.png" width="200" height="200">

And was the hall sensors from aliexpress okay? if anyone used those? 
Keep up the good work @solidgeek :slight_smile:
```

---
## \#457 Posted by: Tig3rch3n Posted at: 2017-11-13T23:33:35.542Z Reads: 425

```
Hey Guys, first entry inhere, sort of a silent reader before...

Okay, the Case is Printed already :stuck_out_tongue: <img src="/uploads/db1493/original/3X/2/4/24728f483a5143694a472be52a655291cb219ddf.jpg" width="690" height="388">
All Aliexpress Parts are bought and on the way, the rest is sourced locally :slight_smile:

But I have a question.
Since the Arduino has so many leftover Pinouts free to use. I thought about adding a Light System and a bell somehow.
On the Receiver side there is no Problem attaching a W2812B as Front/Back/Ground facing Floodlight and a SAB0600 based Bell sound with a small speaker.

But on the  Remote ... There is no leftover buttons or switches to use as trigger to enable the additional features :stuck_out_tongue:
I think I'll just cut some buttons on the backside but I wait until the rest is working.

Any Ideas to solve those remarks?

Cheers
```

---
## \#458 Posted by: ervinelin Posted at: 2017-11-14T01:24:33.327Z Reads: 409

```
I had to calibrate the throttle via both the remote as well as the VESC PPM tab via BLDC tool to get an acceptable range. I do think something isn't quite right though, it's much too narrow by default.

My spring is temporary and its super loose now, sometimes so much so that it doesn't jump back to neutral! I'm waiting for my springs from aliexpress.. taking FOREVER...

@Migro Yes I used the aliexpress hall sensors but as per my comment above I am getting quite a narrow range of readings, not sure if it's due to the sensor or the magnets (magnets are now 5pcs of 1mm as opposed to a single 5mm. Again waiting for aliexpress shipment...

On a side note, I kind of prefer an index finger trigger over the thumb wheel, I originally wanted to redesign the casing for this but then I realised I had an unsed mini 2.4ghz remote lying around. So I've started to hack it to fit all the electronics (less the hall sensor). Should work, everything fits after some dremel work. Will update once I have a result.
```

---
## \#459 Posted by: karatektus Posted at: 2017-11-14T13:57:20.098Z Reads: 401

```
[quote="Tig3rch3n, post:457, topic:28543"]
Any Ideas to solve those remarks?
[/quote]

yeah i was missing some buttons too. But since the firmware really isnt that complicated i was like: "yeah once my parts are here ill just bool some holes for buttons in the top shell and map those to lights and stuff."
I am still boardless so im not in a rush ^^
```

---
## \#460 Posted by: MontPierre Posted at: 2017-11-14T14:36:21.087Z Reads: 396

```
@karatektus  I’m planing to add a button for soft switch on and off , so you can hold it for programmed amount of time to power on or off the remote. I’m not a fan of rocker switch.

Since there are gpios available on the arduino in remote you could add buttons for different functions. 

I’m having a trouble finding small enough caps for the button. All I found are standard large ish ones which will take a lot of space on this tiny remote. Also would be good to have them recessed so they are harder to press by mistake. This would involve redesign of enclosure a bit, perhaps @solidgeek could help? I’m not sure how to go about it.
```

---
## \#461 Posted by: karatektus Posted at: 2017-11-14T14:50:53.015Z Reads: 413

```
[quote="MontPierre, post:460, topic:28543"]
I’m having a trouble finding small enough caps for the button
[/quote]

just dont use caps at all? since they are not buttons you will use while riding, id just mount those on the shell so the button pokes through:[link](https://de.aliexpress.com/item/Free-Shipping-Bzx84-b51-215-dioda-Zener-51-V-250-MW-SOT23-BZX84-B51-100-pcs/32575164814.html?ws_ab_test=searchweb0_0,searchweb201602_2_10152_10065_10151_10068_10344_10345_10547_10342_10343_10340_10341_10548_10193_10194_10541_10304_10307_10060_10302_10155_10154_10056_10055_10539_10537_10059_10534_10533_100031_10103_10102_5680020_10142_10107_10320_10321_10322_10562_10084_10083_10177_10180_10312_10313_10184_10314_10319_10073_10186_10557,searchweb201603_25,ppcSwitch_5&btsid=fc9e1c68-f42e-4a6e-84f3-68045a9a1bbb&algo_expid=c59c0e1d-6e69-4c37-a214-05c963c55a25-7&algo_pvid=c59c0e1d-6e69-4c37-a214-05c963c55a25&rmStoreLevelAB=0)
```

---
## \#462 Posted by: MontPierre Posted at: 2017-11-14T18:24:08.232Z Reads: 416

```
[quote="karatektus, post:461, topic:28543"]
id just mount those on the shell so the button pokes through:link
[/quote]

Ohhh but I want to make it pretty ! Something like this but obviously smaller buttons. I guess this might be hard to achieve. Perhaps someone here has any tips? 

<img src="/uploads/db1493/original/3X/4/b/4bb8eb30bf3daa1109ca381eef0ec3b3de884f07.jpeg" width="225" height="225">
```

---
## \#463 Posted by: Migro Posted at: 2017-11-14T18:29:00.125Z Reads: 412

```
@MontPierre The ones in the picture is only the arrow array. The colored ones are 2-axis potentiometers. Like one a wii or something. 
It is possible to find button caps for the ones karatekus linked. 
Just go on ebay and search for momentary buttons or toggle if you want a toggle button.
```

---
## \#464 Posted by: Tig3rch3n Posted at: 2017-11-14T18:46:45.090Z Reads: 397

```
Maybe some really small "Capped SMD Buttons"?Like those [1](https://de.aliexpress.com/item/1000PCS-6X6X7-3MM-4PIN-SMT-Square-Top-Button-Tactile-Button-Tact-Button-Momentary-Mini-Key-button/32803774561.html?ws_ab_test=searchweb0_0,searchweb201602_4_10152_10065_10151_10068_10344_10345_10547_10342_10343_10340_10341_10548_10193_10194_10541_10304_10307_10060_10302_10155_10154_10056_10055_10539_10537_10059_10534_10533_100031_10103_10102_10142_10107_10320_10321_10322_10562_10084_10083_10177_10180_10312_10313_10184_10314_10319_10073_10186_10557,searchweb201603_25,ppcSwitch_5&btsid=fce325c8-9d0a-47f0-affc-161989917ec4&algo_expid=59e90f3b-a34c-49ca-8ee7-8ea6635a464a-1&algo_pvid=59e90f3b-a34c-49ca-8ee7-8ea6635a464a&rmStoreLevelAB=0) or [2](https://de.aliexpress.com/item/140pcs-lot-12-12-7-3mm-DIP-Tactile-Push-Button-with-colorful-Cap-and-transparent-Cover/32789018264.html)?
```

---
## \#465 Posted by: Ricco Posted at: 2017-11-14T18:51:11.885Z Reads: 396

```
Try having a look through the caps on [digikey](https://www.digikey.com/products/en/switches/accessories-caps/210). Or if you are printing the case yourself, why not try designing some caps and print those out too.
```

---
## \#466 Posted by: MontPierre Posted at: 2017-11-14T21:45:39.290Z Reads: 388

```
I’ll have a look there. If I had a source file of the enclosure it would be much easier to edit ;)
```

---
## \#467 Posted by: Ricco Posted at: 2017-11-14T23:32:00.604Z Reads: 385

```
True. Though,  you could still drill a hole for the button and just design the cap to fit tht hole
```

---
## \#468 Posted by: MontPierre Posted at: 2017-11-15T00:22:41.903Z Reads: 396

```
Yes but I would need to need to mount switch just below it, so a change in design is needed anyway, might just design hole myself plus a socket for the switch, to hold it in place....
```

---
## \#469 Posted by: banjaxxed Posted at: 2017-11-15T20:11:18.622Z Reads: 426

```
PETG 100% infill bottom shell, 50% top, abs trigger, wheel and spring parts<img src="/uploads/db1493/original/3X/3/9/39be53cd1857b6d6c666e6b76d0f73aba0bc8ed2.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/5/5/5565acacdb72340e918f732fe80db1a48973d036.JPG" width="375" height="500">
```

---
## \#470 Posted by: Becker33 Posted at: 2017-11-15T20:42:45.500Z Reads: 414

```
What settings would you advise using if you have a dual motor setup? (just waiting on a final part before building it!)
```

---
## \#471 Posted by: ervinelin Posted at: 2017-11-15T23:20:00.500Z Reads: 432

```
As I mentioned previously, I prefer an index finger trigger as opposed to a thumb wheel throttle.

So I hacked a mini 2.4ghz remote I had lying around and replaced the internals with the same parts as the remote here (less the hall sensor, I used the remote potentiometer instead, I am also trying a smaller pololu step up instead of the one listed, just hope it can provide enough current).

Here's my progress thus far... Everything fits after some creative dremelling.  I am left with the nrf module but that shouldn't be a problem as well.

<img src="/uploads/db1493/original/3X/d/6/d62d99309f84e5d0df1b3f92392680539f7c4985.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/9/9/9916505f3f80c6f3e1b033495bf60e74609620b1.jpg" width="281" height="500"> 
Arduino sits on the battery (not shown here)

<img src="/uploads/db1493/original/3X/b/a/ba21cddd17064b6db6e70bcd571657fb336e570b.jpg" width="281" height="500">

Will update more when it's done and I have field tested it.
```

---
## \#472 Posted by: karatektus Posted at: 2017-11-16T15:11:51.305Z Reads: 405

```
[this](https://www.sparkfun.com/products/10063) would be awesome. You would be totally independent of any actual driving control. can anyone design a socket for that? guess ill order some.
```

---
## \#473 Posted by: ervinelin Posted at: 2017-11-16T18:33:50.630Z Reads: 430

```
I managed to finish up the mini remote hack, here are some images of the completed product.

<img src="/uploads/db1493/original/3X/c/5/c58aba47e67d14935bcb689c6e39dab79a5a7beb.jpg" width="281" height="500">
NRF module fits behind the battery compartment

<img src="/uploads/db1493/original/3X/0/a/0acf51a300664b28afa98e034020ce5f3e6c646a.jpg" width="281" height="500">
Arduino sits on top of the battery 

<img src="/uploads/db1493/original/3X/c/3/c3cfcc166d19d74d87baf282827a98f7874b3042.jpg" width="281" height="500">
USB charging port

<img src="/uploads/db1493/original/3X/3/8/382ba99dbe2d50d70ff2345c1c128d48976c816f.jpg" width="281" height="500">
Used instamorph to close up the holes then drilled a new one to fit a single button which replaces the trigger button in the solidgeeks remote. Technically you can add more buttons here too.

Took me a while to get the throttle range calibrated and synced up with vesc but it works nonetheless. Telemetry is coming in as expected and range is more than enough for esk8.
```

---
## \#474 Posted by: Bensaida Posted at: 2017-11-16T20:17:19.195Z Reads: 397

```
Id be down to buy one from somebody here
```

---
## \#475 Posted by: korryh Posted at: 2017-11-16T22:46:11.472Z Reads: 395

```
I would buy either version as long as it has the safety push button/pull trigger then throttle.  My little likes to pull the throttle when I am not looking so any kind of "do this then that" mechanism is awesome.
```

---
## \#476 Posted by: ervinelin Posted at: 2017-11-16T23:04:14.251Z Reads: 385

```
I actually coded it out so I don't need the safety or dead man's switch to throttle up.

For me i make it a habit to turn off the transmitter when I am not actually riding.
```

---
## \#477 Posted by: ervinelin Posted at: 2017-11-18T00:06:26.891Z Reads: 382

```
Field tested, works as expected, 8km ride with no dropouts.

One tip, don't get distracted by reading the telemetry data and losing your focus on the road ahead.... :)
```

---
## \#478 Posted by: MontPierre Posted at: 2017-11-18T14:25:14.793Z Reads: 383

```
@ervinelin could you share that bit of code ?  I also don’t need deadman switch . Thanks
```

---
## \#479 Posted by: ervinelin Posted at: 2017-11-18T17:27:23.971Z Reads: 393

```
There's a piece of the code which reads:

    if (triggerActive())
    {
      throttle = throttle;
    } else
    {
      // 127 is the middle position - no throttle and no brake/reverse
      throttle = 127;
    }

that basically means you need to the trigger for the thumbwheel to act as throttle, otherwise it's just neutral.

I replaced that piece of the code with just throttle = throttle;

Please test on bench after changing the code!!!
```

---
## \#480 Posted by: ervinelin Posted at: 2017-11-18T17:40:58.894Z Reads: 384

```
I am still getting a strange pairing problem...

I sometimes need to power cycle the board's receiver in order to get a pair, once that pairing is done, I can turn on and off the transmitter without any problems.

But if I turn off the board again, I might lose paring and I need to repeat the power cycling till I get it again.

Any ideas? I suspect it's something in the code somewhere.
```

---
## \#481 Posted by: Jorand Posted at: 2017-11-18T18:41:43.778Z Reads: 400

```
Hi everyone, 
I started making some code changes for my needs. I discuss with @solidgeek about improvement for the code. If it can interest some of you waiting for the new version of the software, I posted my changes on github.

https://github.com/Jorand/nRF24-Esk8-Remote

What I added so far

* Add UART option (saved in EEPROM) in the receiver for sending throttle value and make this option editable from the settings of the remote
* Set Radio channel to 108 (Above most WiFi frequencies) to avoid interference
* Improve the management of the dead zone and add it in remote settings (very useful for joystick user)
* Add reverse throttle setting in the remote
* Make Trigger Mode setting "Killswitch" and "data toggle" working
* Fix battery voltage (I do not know if you have this problem too ...)
```

---
## \#482 Posted by: ervinelin Posted at: 2017-11-19T09:58:20.127Z Reads: 370

```
This is awesome.. Can I know what the UART option does?
```

---
## \#483 Posted by: Jorand Posted at: 2017-11-19T11:40:18.750Z Reads: 378

```
This option allows you to choose between PPM and UART to send the throttle value to your VESC. In my case I plugged my receiver only on the UART instead of PPM. 
And this option is programmable from the remote. If on the remote you change the setting "UART data" your choice is sent to the receiver, that changes the setting and save it in his memory.
```

---
## \#484 Posted by: ervinelin Posted at: 2017-11-19T12:50:00.263Z Reads: 374

```
That's awesome. Didn't even know this is possible.

What advantage does it have other than just having less wires?
```

---
## \#485 Posted by: Jorand Posted at: 2017-11-19T19:14:40.096Z Reads: 382

```
It's digital and you can send other informations if you need. It is already uart that the receiver get the data from the VESC, I find it easier for me and it's a good option to have I think :)

Edited: I looked at the library "VescUartControl" and it seems that it is also possible to have a crusing control mode. I'll try to look at it more ;)
```

---
## \#486 Posted by: ervinelin Posted at: 2017-11-23T07:40:58.943Z Reads: 379

```
Hi @Jorand, I finally managed to find time to try your firmware but I couldn't get the remote to work, nothing on OLED, nothing on serial monitor...

Did I miss a step?

Rolling back to  my other firmware was fine...
```

---
## \#487 Posted by: ervinelin Posted at: 2017-11-23T07:52:36.693Z Reads: 391

```
Oh no... I updated my VESC to FW 3.33 and now my telemetry doesn't work anymore...

Any ideas?
```

---
## \#488 Posted by: Jorand Posted at: 2017-11-24T11:49:59.565Z Reads: 439

```
I finally took the time to finish my remote and I'm very happy with the result ! I changes a little bit the placement of the components because i use a [700mah batterie](http://www.epropulsionsystems.eu/lipo-20c/141-batterie-lipo-1s-700.html) and this [AS01 SPIPX nRF24L01](https://fr.aliexpress.com/item/1PC-New-Arrival-100mW-AS01-SPIPX-nRF24L01-wireless-pa-lna-2-4g-wifi-module-Wireless-Transmission/32819372747.html) module.

I also connected the two data wire from the micro usb charging port to the arduino micro usb. That way I can reprogram it without having to open the remote ;) (I use the plug of a USB cable that I opened).

I can wait to finish the receiver and give it a try !!

@solidgeek There is an best position of the hall sensor to have the best resolution ? and it seems that the screws to close the remote are no longer M4x12 ?

<img src="/uploads/db1493/original/3X/d/4/d43542fd60bf4bf2011d80a6cf427f6efb4fd3b8.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/7/976e626d29d3b2eb4abfb9d52c69ba4e03506562.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/f/9/f960c8c8d94564466e372f42681a1c930483a8b6.jpg" width="666" height="500">

@ervinelin Sorry, it seems that I forgot to pull the last modifications made by @solidgeek will look at what I forgot. Thanks for giving a try :)
```

---
## \#489 Posted by: Der6FingerJo Posted at: 2017-11-24T11:55:35.650Z Reads: 422

```
Here's a thread for your problem, the developer of the VESC library is currently testing things.

http://www.electric-skateboard.builders/t/tester-needed-for-vescuartcontrol-with-new-interface/38476
```

---
## \#490 Posted by: Jorand Posted at: 2017-11-25T01:27:56.945Z Reads: 411

```
I did 18 km tonight to test the remote and it was so nice ! Super smooth and safe. I also tested the cruse control mode that i added today… is perfect :)

I updated my [code](https://github.com/Jorand/nRF24-Esk8-Remote). With the cruse control (Trigger Mode `1`) only working with UART yet. Enjoy !
```

---
## \#491 Posted by: TranxFu Posted at: 2017-11-26T11:00:29.437Z Reads: 404

```
Is there an updated component list/BoM ?

I'd be printing this today and would like to source the parts. But am worried that some are outdated or better ones have been found.
```

---
## \#492 Posted by: Jammeslu Posted at: 2017-11-27T22:45:22.971Z Reads: 395

```
I need this remote assp, since I was one of the beta testers I wounder if anyone of you managers to make one fully functional and would be willing go build one and send me in EU please DM
```

---
## \#493 Posted by: ervinelin Posted at: 2017-11-29T16:36:59.016Z Reads: 391

```
I tried this, unfortunately doesn't work...

Distance seems to have something but the numbers are garbled, nothing else works as it should, rolled back again to FW2.18...
```

---
## \#494 Posted by: niktwo17 Posted at: 2017-11-29T19:43:04.065Z Reads: 399

```
@solidgeek
Is it possible to get the inventor files for the remote? already built one(great design) but id like to change some details(different screen and buttons)
```

---
## \#495 Posted by: HighMasterGogo Posted at: 2017-12-05T09:57:49.010Z Reads: 426

```
Finally got the remote fully built and working last night.

I did have to solder a 10k ohm resistor from the RX to GND on the transmitter nano as it wouldn't fully power on without hitting the reset button. Apparently this is a common thing with Arduinos.

I'll be constructing the receiver nano tonight. Exciting! Thanks again @solidgeek!

<img src="/uploads/db1493/original/3X/7/a/7a90bfa418cee1ef7d013b153357cc29c6252cf9.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/5/8/5879744a664201024c41e449b97784b5ee63792d.jpg" width="666" height="500">
```

---
## \#496 Posted by: mmaner Posted at: 2017-12-05T16:36:38.779Z Reads: 409

```
If you decide to build and sell these as a completed device, I think you could make some big money.  I'd be up for a couple myself.
```

---
## \#497 Posted by: BoostedBuilder Posted at: 2017-12-05T21:27:57.268Z Reads: 404

```
[quote="mmaner, post:496, topic:28543"]
I'd be up for a couple myself.
[/quote]


Same here!
```

---
## \#498 Posted by: HighMasterGogo Posted at: 2017-12-05T22:55:01.178Z Reads: 390

```
OK so I got everything wired up for a transmit and receive test but I can only get the transmitter to successfully connect if I power it via the nano's micro USB port. I've took multimeter readings whilst powered off battery and USB and I can't see any issues. I'm wondering if the need to have a resistor between RX and GND is a clue to bigger issues? I removed it to test but no difference (other than now having to press the reset button on the nano when powering from the battery - as mentioned in my last post). Any ideas?
```

---
## \#499 Posted by: banjaxxed Posted at: 2017-12-05T23:01:38.799Z Reads: 382

```
Still waiting on innards here
☘️
```

---
## \#500 Posted by: Clonkex Posted at: 2017-12-05T23:03:30.790Z Reads: 392

```
I'd suggest checking all your solder joints first.
```

---
## \#501 Posted by: Blacksheep Posted at: 2017-12-05T23:11:32.271Z Reads: 401

```
Yes me too
```

---
## \#502 Posted by: HighMasterGogo Posted at: 2017-12-05T23:24:14.210Z Reads: 384

```
Thanks guys, def a weak joint or lack of shielding as with the parts pulled apart, I get a reliable connection. Thanks!
```

---
## \#503 Posted by: HighMasterGogo Posted at: 2017-12-07T21:44:04.735Z Reads: 390

```
Right, so, remote now gives a very reliable connection but the pulsewidth display in BLDC tool is terrible, it seems like the receiver is only getting a position report every so often. Certainly not smooth. Is this likely to be a shileding issue at the receiver end?

I'm stating to thing these nRF24 modules I have aren't great (built in, very small antenna).
```

---
## \#504 Posted by: ervinelin Posted at: 2017-12-08T09:00:37.984Z Reads: 391

```
The pulsewidth display in my BLDC tool also doesn't look as "clean" as I think it should.

However, in real world riding it works just fine.

My only gripe is that I can't get the entire throw of the trigger to spread across the entire throttle band, meaning to say I hit 100% throttle when I am only at maybe half of the max throw.

Already tried to calibrate as much as I could, didn't seem to help.
```

---
## \#505 Posted by: HighMasterGogo Posted at: 2017-12-08T09:20:25.716Z Reads: 391

```
I have an issue with my temporary RC car remote where the brake travel is much less than the throttle. This means the neutral position doesn't sit at 50% no matter how much I trim. This meant I'd have to sacrifice some throttle or brake in order for the motor not to spin or have brakes applied at neutral position.

I used this, awesome, extended firmware from @Ackmaniac http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116

It has an awesome little wizard (very much like the old windows game controller calibrator) that sorts your controls out in no time. You can also manually set the neutral position.

I'm wondering if it may help you out?
```

---
## \#506 Posted by: banjaxxed Posted at: 2017-12-08T11:25:24.947Z Reads: 379

```
Pretty much the problem with the nano/winning, is that bench or in use?
```

---
## \#508 Posted by: Genius2017 Posted at: 2017-12-09T04:14:06.086Z Reads: 377

```
Sorry hit the wrong button on my phone.
```

---
## \#509 Posted by: escu_12 Posted at: 2017-12-09T18:45:34.120Z Reads: 380

```
ok and tried many times, and with different codes even those of example and do not communicate the two nrf24

I do not know what's going on

all conections is okey and revised lot of times
```

---
## \#510 Posted by: escu_12 Posted at: 2017-12-09T18:58:54.439Z Reads: 381

```
okey i'm fixed with a capacitor in two arduinos
```

---
## \#511 Posted by: ervinelin Posted at: 2017-12-11T07:26:18.044Z Reads: 388

```
In use it seems fine, would be better if the control was finer but I've gone many kilometers with it as it is... So "don't fix what isn't broken"
```

---
## \#512 Posted by: escu_12 Posted at: 2017-12-11T13:19:05.702Z Reads: 402

```
again it does not work, the capacitor was temporary, but it does not work, they do not communicate

I do not know what to do

what libraries have you used?
```

---
## \#513 Posted by: PredatorBoards Posted at: 2017-12-13T06:24:31.891Z Reads: 416

```
I have a proposition...
<img src="/uploads/db1493/original/3X/7/1/712c2844dd2c7578f304e12d6edb904d7ca1acdf.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/2/6265275098c43ba585ed64b555c7ee87f053ea84.JPG" width="375" height="500">

We currently use these remotes on the Banshee. Damn solid construction and a pretty much mechanical imitation of the Boosted remote. What's stopping me from releasing these to the DIY market is the fact that the manufacturer doesn't want to make new circuitry for pairing with a standard RX/TX receiver.

I'm thinking of just selling this remote as a standalone and letting y'all figure out the electronics bit.

For those who have a 3D printer and want the pulsewidth display, then by all means go with the current firefly design. However I'm interested in figuring out a slightly less complicated approach for those looking for a half decent thumb throttle remote for their DIYs.
```

---
## \#514 Posted by: pjotr47 Posted at: 2017-12-13T13:15:00.377Z Reads: 389

```
I like the imitation of the boosted board remote. I maybe want one remote to disassemble and try to fit al the components of the lcd remote in it. What would be the price?
```

---
## \#515 Posted by: PredatorBoards Posted at: 2017-12-13T17:15:25.694Z Reads: 390

```
For early tinkerers who think they can help jumpstart this 'hack'... let's say 20$. Should be enough to cover the costs and shipping, though I may charge extra depending on how things pan out with the manufacturer.

I think that's a pretty reasonable price, given the magnets + spring + battery is already more than 10$
```

---
## \#516 Posted by: HighMasterGogo Posted at: 2017-12-13T20:09:45.223Z Reads: 386

```
Hey @solidgeek, did you ever have an issue monitoring the serial on the transmitter when it's fully wired up? My nano isn't even recognised by my computer if it's completely wired up. After a little googling, I have to disconnect pin 13 and then the nano connects great. The problem with this is that pin 13 is used by the nRF24 module and so I can't debug my transmission issues. Any ideas?
```

---
## \#517 Posted by: Clonkex Posted at: 2017-12-13T22:27:22.182Z Reads: 390

```
Is that USD? I only ask because you've put the $ sign on the wrong side of the number so I feel like you're not from the US.

EDIT: Don't mind me, your profile says you're in California.
```

---
## \#518 Posted by: PredatorBoards Posted at: 2017-12-14T00:27:27.603Z Reads: 395

```
I'm about as American as you get.
```

---
## \#519 Posted by: landonkun Posted at: 2017-12-14T02:51:16.602Z Reads: 396

```
[quote="PredatorBoards, post:518, topic:28543"]
I'm about as 'Murican as you get.
[/quote]

Fixed that for you ;)
```

---
## \#520 Posted by: nikoli280 Posted at: 2017-12-16T14:55:10.386Z Reads: 389

```
Can someone send a schematic for how the receiver is setup. I know the Arduino and module is like in the remote. But how are they connected to the VESC?
```

---
## \#521 Posted by: Jammeslu Posted at: 2017-12-16T16:14:47.366Z Reads: 392

```
Has anyone succesfully made the remote fully working no problem?
```

---
## \#522 Posted by: SORRENTINO Posted at: 2017-12-18T16:26:03.336Z Reads: 377

```
Are you selling this remote for $20 still for use that want to hack it?
```

---
## \#523 Posted by: PredatorBoards Posted at: 2017-12-19T18:29:19.106Z Reads: 372

```
Yeah still am. I currently don't have time to make a listing on my website since it's damn finals week for my Uni. However you can PM me and PayPal if you want.
```

---
## \#524 Posted by: wafflejock Posted at: 2017-12-19T22:35:55.616Z Reads: 377

```
Avoiding the electronics and selling the rest of the assembly as a kit is probably a good way to go.  I looked into doing this like a year ago or so when I was working on my own nrf based remote too but think even *if* the boards are FCC certified any electronics device sold in the US or most places in the EU will need more further certification since it's a "radiator" (a friend has told me anything with a coil in it they design and plan to manufacture goes through FCC certification, adafruit has some good write ups on what is allowed in terms of hobbyists building their own though).

https://www.sparkfun.com/tutorials/398
```

---
## \#525 Posted by: SORRENTINO Posted at: 2017-12-19T22:56:00.484Z Reads: 375

```
 I don't think any 5.8, 2.4, or 1.3ghz vtxs or receivers go through any FCC certification sold at numerous hobby shops across the US. I could be wrong tho. I know fatshark does offer 1 vtx that is FCC approved but I don't think the rest are FCC approved. I wonder how they get away with that?
```

---
## \#526 Posted by: solidgeek Posted at: 2017-12-20T23:29:28.430Z Reads: 387

```
Hi guys, I am sorry that I have been inactive the last few weeks, I had to finish my university project :-) I appreciate all the interest in my project, however, I do not have the time to answer all your questions at the moment. 

I will work on some better documentation and a new software update after Christmas. 

In the meanwhile, I wish you all a Merry Christmas! :christmas_tree:
```

---
## \#527 Posted by: SORRENTINO Posted at: 2017-12-21T16:48:34.607Z Reads: 384

```
pm'd you!

10char
```

---
## \#528 Posted by: dokraphael Posted at: 2017-12-28T11:07:16.992Z Reads: 388

```
Go it assembled
Thanks a lot that was a lot of fun.
Now I need to make the board :slight_smile: 

<img src="/uploads/db1493/original/3X/0/b/0b26042bdb5012eca8d9ddf4dffe513fa11f5d4a.jpg" width="690" height="457">
```

---
## \#529 Posted by: GrecoMan Posted at: 2017-12-28T14:08:07.875Z Reads: 379

```
hmmm...  do I print at 0.005 res or 0.01 :imp:

decisions decisions

7 hours solid abs at .005 res :astonished:
```

---
## \#530 Posted by: GrecoMan Posted at: 2017-12-28T17:05:16.952Z Reads: 368

```
anyone order more than they needed and is in the us? i just don’t really wanna wait for it to come from china
```

---
## \#531 Posted by: NAF Posted at: 2017-12-29T14:51:01.003Z Reads: 360

```
I got the same question ..anyone from Europe with some more parts.
```

---
## \#532 Posted by: SORRENTINO Posted at: 2017-12-29T20:24:11.473Z Reads: 359

```
@PredatorBoards SENT YOU PM MY DUDE! NEED THAT REMOTE :grinning:
```

---
## \#533 Posted by: MontPierre Posted at: 2017-12-29T20:56:35.469Z Reads: 362

```
@NAF

 Where are you from, UK 🇬🇧 here ? I might have some spares -  micro usb, magnet, hall sensor, NRF, perhaps arduino as well.  PM please.
```

---
## \#534 Posted by: GrecoMan Posted at: 2017-12-30T00:47:48.429Z Reads: 361

```
[quote="GrecoMan, post:530, topic:28543, full:true"]
anyone order more than they needed and is in the us? i just don’t really wanna wait for it to come from china
[/quote]

please?  I cant imagine nobody bought extras
```

---
## \#535 Posted by: Sk8Board Posted at: 2017-12-30T01:05:19.409Z Reads: 351

```
That's a mighty small resolution if you want it to be smooth to the touch, you could print at a higher resolution and acetone smooth them.
```

---
## \#536 Posted by: GrecoMan Posted at: 2017-12-30T01:06:13.726Z Reads: 342

```
think i’ll print at tiny res, then just sand and paint. saves me the time of setting up an acetone bath
```

---
## \#537 Posted by: Sk8Board Posted at: 2017-12-30T01:07:45.415Z Reads: 349

```
You don't need an acetone bath, just a mist or acetone in a towel, but whatever works the best.
```

---
## \#538 Posted by: GrecoMan Posted at: 2017-12-30T01:08:34.869Z Reads: 367

```
oh really? every time i’ve done it ive just used a bath.
```

---
## \#539 Posted by: Sk8Board Posted at: 2017-12-30T01:17:38.466Z Reads: 385

```
I've used paper towels with some decently sized parts. It's really just the surface that needs to be smoothed. You could also put spackle to smooth it out, but that is a lot of work. Acetone will probably be best. Here's a video of acetone mist paper towel should work, just wash off the piece after because the acetone will continue to melt the plastic. 

https://youtube.com/watch?v=6xFUNFG-UKE
```

---
## \#540 Posted by: Maralc Posted at: 2017-12-30T03:29:32.749Z Reads: 381

```
Hi All
I tried to search on the thread but could not find.
Is anyone manufacturing this remote and selling it ready to go? I am really interested.
```

---
## \#541 Posted by: Sk8Board Posted at: 2017-12-30T03:37:43.628Z Reads: 371

```
@PredatorBoards might still be selling. Even if not, it will still be a fun build.
```

---
## \#542 Posted by: PredatorBoards Posted at: 2017-12-30T03:49:06.329Z Reads: 365

```
For now I'm selling 'replacement remotes' for our Banshee. These replacement remotes are Boosted remote replicas. If you buy them, you'd be buying them for the enclosure and nothing else. You will have to fab the electronics yourself.

Edit: Another problem is that I can  only begin selling if there is enough interest to group buy several at a time. Otherwise the cost to ship a single remote out of China is expensive.
```

---
## \#543 Posted by: MontPierre Posted at: 2017-12-30T14:06:02.855Z Reads: 356

```
[quote="GrecoMan, post:534, topic:28543"]
please?  I cant imagine nobody bought extras
[/quote]

Pm please, here are you from ?
```

---
## \#544 Posted by: GrecoMan Posted at: 2017-12-30T14:06:25.070Z Reads: 351

```
US. that’s the problem 😉
```

---
## \#545 Posted by: MontPierre Posted at: 2017-12-30T14:28:31.067Z Reads: 352

```
Ohhhh yeah ...... I was hoping for EU at most, sorry bud !
```

---
## \#546 Posted by: GrecoMan Posted at: 2017-12-30T14:30:55.416Z Reads: 350

```
depending on shipping costs it could possibly be a bit cheaper since some of the items would ship together :thinking:
```

---
## \#547 Posted by: wmj259 Posted at: 2017-12-30T16:37:52.093Z Reads: 352

```
Just wondering if the design other then the 3d printed controller changed from earlier in this thread.
```

---
## \#548 Posted by: Boesila Posted at: 2017-12-31T13:19:07.360Z Reads: 361

```
Hi guys, 
before a tell my question I like to thanks everybody who contribute to this remote. Great job! :smiley:

I'm almost finish with my build of the remote but unfortunately I ordered the wrong NRF Module. Instead of the recommended one I ordered this one: https://www.aliexpress.com/item/CORE51822-BLE4-0-Bluetooth-2-4-GHz-Wireless-Module-NRF51822-Communication-Board-RF-Controller-2-3/32673748670.html
I has the same chip, so it should work... if I would know how to connect it. I'm sure here is somebody who i able to tell me which pins I should use. I cannot find the labels like CE, CS, SCK, MOSI, MISO... 

Thanks in advance :+1:
```

---
## \#549 Posted by: niktwo17 Posted at: 2017-12-31T16:16:01.635Z Reads: 367

```
I dont think it has the same chip. It uses bluetooth instead of 2,4Ghz
Im not sure youll find anyone who is using this chip as bluetooth is not known to be reliable which is crucial for esk8 remotes.
You will probably be better of buying nrf24l01 modules instead of messing with those(this chip doesnt support i2C or SPI either)
```

---
## \#550 Posted by: Hummie Posted at: 2018-01-05T22:31:59.315Z Reads: 359

```
hows the boosted replica and where can it be gotten?  i'd like any good thumb remote really but don't want to get into the complication of making this Arduino one.  I assume this Arduino one is expensive and a lot of time in making
```

---
## \#551 Posted by: solidgeek Posted at: 2018-01-05T23:16:11.603Z Reads: 359

```
Actually it is quite inexpensive, however, you are right about it's a time-consuming build :smile: Hopefully I will be able to produce and sell some in the near future :slight_smile:
```

---
## \#552 Posted by: pjotr47 Posted at: 2018-01-08T18:12:39.671Z Reads: 344

```
With what program is the housing designed?
```

---
## \#553 Posted by: NAF Posted at: 2018-01-08T18:16:57.885Z Reads: 343

```
@solidgeek Come on solidgeek !! I wanna buy one !!
```

---
## \#554 Posted by: solidgeek Posted at: 2018-01-08T19:30:51.945Z Reads: 340

```
@pjotr47 I made it in Autodesk Inventor, however, I am currently learning to use Onshape, and that's a very nice program too :slight_smile:

@NAF My final exam is on Friday, afterward I finally got time to finish the remotes! Looking forward :P
```

---
## \#555 Posted by: Jammeslu Posted at: 2018-01-08T19:40:45.647Z Reads: 342

```
Could you just take a quick check at  you pm I have to plan haha
```

---
## \#556 Posted by: SeeTheBridges Posted at: 2018-01-10T07:06:33.093Z Reads: 343

```
What parts are you looking to get?

EDIT: Also, @solidgeek will you be making a tutorial for building the remotes at some point? I'm waiting for the last parts of my prints to finish, and I was thinking of doing a short 2-3 part series about it. I might wait though if you have plans for a comprehensive guide or plan on updating the current documentation for it.
```

---
## \#558 Posted by: Zyb Posted at: 2018-01-11T13:55:40.899Z Reads: 353

```
hey guys looking forward to build this remote soon. do you think this hall sensor will work ? https://www.aliexpress.com/item/5pcs-lot-SS495A1-95A-TO-92-high-precision-Hall-sensor-SS495A-screen-95A-new-original/32699635518.html?spm=a2g0s.9042311.0.0.FZd8KP
```

---
## \#559 Posted by: Snowi Posted at: 2018-01-17T05:49:11.906Z Reads: 358

```
anyone got the finished schematic? especially someone who finished and has a working controller
```

---
## \#560 Posted by: Howardzinn Posted at: 2018-01-17T13:05:45.546Z Reads: 364

```
Hello, 
can anyone tell me if this connection is usable? I do not want to burn my VESC because of BEC :frowning:

Thanks a lot 4 reply ![RZZ|690x316](upload://qkn6rzaYdSMSLmFZg8Sh31PTzxN.png)
```

---
## \#561 Posted by: Pimousse Posted at: 2018-01-17T14:49:44.810Z Reads: 360

```
Arduino Nano Tx level is 5V.
You need a voltage divider to lower the signal to 3,3V (VESC's logic level).
BTW, why don't you use 5V from VESC for supplying the Nano ?
Is that nRF24 chip that much powerful ?

Creating a ground loop is not a good idea.
```

---
## \#562 Posted by: Pedrodemio Posted at: 2018-01-17T16:25:51.525Z Reads: 351

```
@Pimousse  Are you sure of that? I always connected TX/RX directly and it worked for more than a year, but I always had problems sending VESC data to the arduino, sometimes it worked others it wouldn’t, maybe that’s it?

If I recall I saw a lot of people connecting directly also
```

---
## \#563 Posted by: Snowi Posted at: 2018-01-17T17:12:23.325Z Reads: 345

```
what program or website did u use to make that schematic?
```

---
## \#564 Posted by: solidgeek Posted at: 2018-01-17T17:36:44.607Z Reads: 332

```
@Howardzinn It looks good to me. 

@Pimousse It's true that the VESC logic is 3.3V, however I remember reading someplace that it is 5V tolerant. Of course, it would be best to use a voltage divider or a level converter to be sure.  I would love some more thoughts on this.

@Snowi Its made in Inkscape
```

---
## \#565 Posted by: Howardzinn Posted at: 2018-01-17T18:45:09.928Z Reads: 333

```
@Pimousse It's the thing i've be afraid of. But in this topic "http://www.electric-skateboard.builders/t/focbox-hm-10-bluetooth-do-i-need-resistors/27093" dont use nothing
@Snowi  yes it's Inkscape but honestly I was a little lazy and adjusted the scheme from solidgeek
@solidgeek thanks a lot for your reply, remote and all the energy you've spent <3
```

---
## \#566 Posted by: Pimousse Posted at: 2018-01-17T18:52:29.112Z Reads: 333

```
I've read STM datasheet long time ago and as far as I remember, It wasn't sure that tx/rx pin are 5V tolerant.
So I always use voltage divider on all of my Arduino stuff for communicating with VESC (1k and 2,2k).
Works great like this.
See my latest update here : http://www.electric-skateboard.builders/t/pircac-trampa-holypro-35-2x-overion-130-kv-10s10ah-2x-vesc6/32408/7?u=pimousse
```

---
## \#567 Posted by: Pedrodemio Posted at: 2018-01-17T20:13:18.603Z Reads: 335

```
Thanks, I will take a look and probably will implement the divider on the board I’m current working, the think is, the divider does nothing when the STM sends the 3,3V to the arduino, for this we would need an level shift ic
```

---
## \#568 Posted by: Pimousse Posted at: 2018-01-17T22:43:56.315Z Reads: 335

```
3.3v for the Arduino Rx is high enough even at 115200 bauds ;)
No need of extra chip.
```

---
## \#569 Posted by: SeeTheBridges Posted at: 2018-01-17T22:55:22.801Z Reads: 338

```
Hmm, I can't seem to get my OLED display to show anything. The one on the parts list doesn't have the same pinout as on the schematic... Mine has GND VCC **SCK** and SDA. An I2C scanner I ran detects the display still, but its just not working? Any help?
```

---
## \#570 Posted by: Jamy Posted at: 2018-01-17T23:01:12.718Z Reads: 330

```
Make sure it's connected when the arduino starts up. If you connect it afterwards it might not work.
```

---
## \#571 Posted by: SeeTheBridges Posted at: 2018-01-17T23:07:30.922Z Reads: 324

```
Everything is already soldered to the board. Im just not getting anything
```

---
## \#572 Posted by: solidgeek Posted at: 2018-01-17T23:21:14.424Z Reads: 328

```
@SeeTheBridges SCL is a typing error on my side, it should be SCK :P  If you have connected it in the same manner as on the schematic, it should work. It's possible that the display is broken they are quite fragile. Otherwise, I would check the connections. It should be as follows:

GND → GND
VCC → 5V
SCK → A5
SDA → A4
```

---
## \#573 Posted by: SeeTheBridges Posted at: 2018-01-18T00:02:55.303Z Reads: 321

```
well fuck. I guess I broken mine 😓
```

---
## \#574 Posted by: Snowi Posted at: 2018-01-18T01:24:27.482Z Reads: 322

```
anyone need limit switches or trigger switches? i got a lot extra because i bought in bulk. if you need any, i only charge a dollar + shipping, compared to being $3
```

---
## \#575 Posted by: SeeTheBridges Posted at: 2018-01-18T02:53:55.976Z Reads: 332

```
I finally got it working, but now the display is just hanging on Esk8 remote...any advice?

EDIT: My 3V3 was shorting to my D13. Missed a bit of solder on the back. Got a mostly working remote now. I can't seem to cycle through the settings if I try to go into the remote settings though...
```

---
## \#576 Posted by: Howardzinn Posted at: 2018-01-18T09:29:15.473Z Reads: 335

```
This may solve the problem with RX/TX 5V logic. But need to try and measure (im waiting to the module) :penguin:! any advice or comments? ![RZZ_2|690x280](upload://HXMJCY8kBcXEi1wJJYr4Q0zYmU.png)
```

---
## \#577 Posted by: Zyb Posted at: 2018-01-18T10:11:49.509Z Reads: 332

```
Just a quick googling, I found out it’s a common problem with arduinos in other applications too. If that’s A solution to the problem I found a cheap and small board just for that. https://www.proto-pic.co.uk/4-channel-i2c-safe-bi-directional-logic-level-converter-bss138.html
```

---
## \#578 Posted by: Howardzinn Posted at: 2018-01-18T10:16:07.542Z Reads: 323

```
@Zyb Yes! It's what i looked at. https://www.aliexpress.com/item/IIC-I2C-Logic-Level-Converter-Bi-Directional-Module-5V-to-3-3V-For-Arduino/32589088559.html?spm=a2g0s.9042311.0.0.mcoGbR I have no experience with BSS138 so its need to do some measure. but looks legit
```

---
## \#579 Posted by: Zyb Posted at: 2018-01-18T10:19:16.096Z Reads: 315

```
People in the comments are explaining exactly the same problem so it’s worth giving a shot.
```

---
## \#580 Posted by: Pimousse Posted at: 2018-01-18T10:21:44.816Z Reads: 318

```
About VESC PPM, why don't you use UART comm for driving the VESC ?
VescUartControl library has functions for that (VescUartSetCurrent & VescUartSetCurrentBrake).

;)
```

---
## \#581 Posted by: Der6FingerJo Posted at: 2018-01-18T11:03:28.467Z Reads: 309

```
Without modifying the library you can only get it to work on one VESC, the slave won't do the same thing as the one connected to the Arduino. You would need to send a special "transmit this also over can" byte when setting the current which isn't implemented and I don't really know how to do it.
```

---
## \#582 Posted by: solidgeek Posted at: 2018-01-18T15:07:45.347Z Reads: 326

```
@SeeTheBridges Great! Well, it's probably an issue with your magnets or the placement of your hall-sensor. If the magnets aren't strong enough, the hall sensor will not return a high or low enough value. You have to tweak the min and max hall sensor values. I am adding a Hall sensor calibration function in the newest software update, which should be ready by Monday :slight_smile:  

Otherwise if you can't wait, you will have to go to the function **controlSettingsMenu()** and change the value 150 to a higher value (try with 250).

@Howardzinn that's a good idea!
```

---
## \#583 Posted by: Zyb Posted at: 2018-01-19T14:03:59.240Z Reads: 336

```
@Howardzinn hanks for the link i just made an order, they are much cheaper than the ones I found from Uk :slight_smile:

complete arduino noob here. i installed 3 extra libraries and when i verify/compile the transmitter code i get some red colored message i guess its a warning saying: 

D:\Documents\Arduino\libraries\VescUartControl-master\VescUart.cpp: In function 'int PackSendPayload(uint8_t*, int)':

D:\Documents\Arduino\libraries\VescUartControl-master\VescUart.cpp:139:21: warning: converting to non-pointer type 'uint8_t {aka unsigned char}' from NULL [-Wconversion-null]

  messageSend[count] = NULL;

does it look like theres problem? thanks for any help i have no idea whats going on :slight_smile:

edit: when i open the transmitter.ino file and verify it for the first time it always gives me that warning but second verify comes out clean.. weird. i guess its allright.
```

---
## \#584 Posted by: Migro Posted at: 2018-01-19T20:24:34.730Z Reads: 351

```
![image|375x500](upload://z2crXIIz8QcStj8suPmKeFAdqkF.jpg)

It could just be my printer that causes the problem as you can see the curved sides is bad but my question is about the micro usb? Was it suposed to be all the way down into the bottom shell? 

And also one other question is what this should be connected to? what pin is that? ![image|322x76](upload://31So0PQp9S3OR3JL9OftVRTDFcw.png)
```

---
## \#585 Posted by: Zyb Posted at: 2018-01-19T21:54:15.338Z Reads: 333

```
im wondering about that pin too :confused:
```

---
## \#586 Posted by: Migro Posted at: 2018-01-19T22:01:16.246Z Reads: 336

```
Do you have the problem with the micro usb?
```

---
## \#587 Posted by: solidgeek Posted at: 2018-01-19T22:27:57.306Z Reads: 349

```
Well that doesn't look right at all. The micro USB should fit.

![20180119_232238|281x500](upload://lSgzoefWi2weizIlY8Bt9hxoP2N.jpg)

Regarding the batteryMeasurePin, if you look at the code its used to measure the remote's battery voltage, and is defined as "const int batteryMeasurePin = A2;". It's connected to pin A2.
```

---
## \#588 Posted by: SeeTheBridges Posted at: 2018-01-19T22:34:01.900Z Reads: 333

```
ohhhhhhhh. shit. That wasn't on the schematic... Im in the middle of a build guide and the fact that I completely missed that is gonna be HELLA unfortunate 😅
```

---
## \#589 Posted by: Migro Posted at: 2018-01-19T22:41:21.665Z Reads: 346

```
Okay thanks. I guess my printer thats sucks at the moment... :sweat_smile:
Nothing else to do than try prin a new one tomorrow.
What have you done to get the microswitch wired and mounted @solidgeek ?
 ![image|375x500](upload://drE1sygaDUpMr5PsQ0Y7nNtTftU.jpg)
```

---
## \#590 Posted by: solidgeek Posted at: 2018-01-19T23:25:32.930Z Reads: 344

```
@SeeTheBridges Haha sorry for that! But wow, I am glad you would take your time to share your experience and help out. I know the documentation lacks a lot, so I appreciate it a lot :slight_smile:  

@Migro I bent the legs up toward the top, press them against a flat table or something :-) 

![20180120_002237|281x500](upload://1TIVYcd3HFBhW9HQRqxggFCxswN.jpg)
```

---
## \#591 Posted by: Migro Posted at: 2018-01-19T23:41:38.258Z Reads: 333

```
Thanks. Now i just need to fix my print and make the reciever. And ofcourse wait for the weather... :grinning:
Keep up the work :slight_smile:
```

---
## \#592 Posted by: Migro Posted at: 2018-01-20T13:30:48.417Z Reads: 342

```
Once again i seek ur help. Do i need to change something in the code or am i doing something wrong? 
https://youtu.be/G3uAmgSiQZ0

As you can see i cant change settings (maybe doing something wrong) but saw one of your videos where i think im doing the same. Im not getting the full motion of the wheel at the moment.
```

---
## \#593 Posted by: solidgeek Posted at: 2018-01-20T14:53:04.215Z Reads: 338

```
You got the exact same problem as @SeeTheBridges, and it should be fixed in the new update I am releasing tomorrow :-) The problem is that the magnets are not as strong as the ones I have bought, and therefore not giving the same hall sensor reading. If you want a quick fix go to the function **controlSettingsMenu()** and change the value 150 to a higher value (try with 300).
```

---
## \#594 Posted by: Migro Posted at: 2018-01-20T16:23:52.224Z Reads: 327

```
Okay thanks seemed to do the job. :slight_smile: Figured out how to use the settings but dont know what everything does.
```

---
## \#595 Posted by: Snowi Posted at: 2018-01-20T18:23:58.910Z Reads: 322

```
How would I connect the VESC to the arduino? Can anyone send me a picture of their exact wiring setup from connecting the VESC to the arduino.

Thanks.
```

---
## \#596 Posted by: Snowi Posted at: 2018-01-20T19:49:28.904Z Reads: 320

```
Also anyone who lives in the US got extra 5mm magnets that I can have? Kinda at a time crunch rn and I would love to get the magnets soon. Willing to buy them.
```

---
## \#597 Posted by: solidgeek Posted at: 2018-01-20T22:40:45.376Z Reads: 335

```
I bought these from Amazon: https://www.amazon.co.uk/gp/product/B0038A4MKI however not sure if you can find anything like it on the international Amazon. 

Regarding connecting VESC to Arduino, if I remember correctly the connections should be as follows: 

Arduino  - VESC
GND → GND
5V → 5V
RX → TX
TX → RX (you could add a voltage divider here)
PIN 5 → PPM
```

---
## \#598 Posted by: Snowi Posted at: 2018-01-21T03:12:48.841Z Reads: 333

```
I have also been looking at hall sensors. Can I use this hall sensor? If not, why?

https://www.amazon.com/A3144-A3144E-OH3144E-Effect-Sensor/dp/B00ATNJH20/ref=zg_bs_306929011_1?_encoding=UTF8&psc=1&refRID=NYCKM46V6XEBW3KR8XD1
```

---
## \#599 Posted by: SeeTheBridges Posted at: 2018-01-21T04:24:33.695Z Reads: 327

```
@solidgeek Have you changed the size of the bolt holes since you started working on the firefly? The bolts on the parts list didn't end up fitting into my enclosure at all. I had to expand the screw holes to make some of them work. It feels like the bolts needed to go down around maybe an M2.5 size screw...
```

---
## \#600 Posted by: Clonkex Posted at: 2018-01-21T04:37:04.274Z Reads: 329

```
Check that your printer is printing the hole sizes accurately. It's very common for holes to print much smaller than they should be.
```

---
## \#601 Posted by: SeeTheBridges Posted at: 2018-01-21T04:39:02.137Z Reads: 337

```
I'd love to check that, buuuttttt I'm using school printers. And I have no idea how to check. They're makerbot V3s?
```

---
## \#602 Posted by: Snowi Posted at: 2018-01-21T05:33:44.357Z Reads: 344

```
where are these ground wires supposed to connect to? i am new to electronics so please pardon my incompetencies.

![image|690x407](upload://9Tl5cig3WCsZGxSdEzEOWc6WjPL.png)
```

---
## \#603 Posted by: Clonkex Posted at: 2018-01-21T05:36:17.353Z Reads: 335

```
Just measure the holes?
```

---
## \#604 Posted by: Clonkex Posted at: 2018-01-21T05:37:07.592Z Reads: 330

```
To ground. Negative.

Honestly (without trying to be mean) if you don't know what GND means I doubt your ability to make an esk8 :/
```

---
## \#605 Posted by: SeeTheBridges Posted at: 2018-01-21T05:49:11.520Z Reads: 326

```
Oh you literally meant to measure them 😅 I thought maybe you meant there was a way to check how the slicer setup the makerbot file or something
```

---
## \#606 Posted by: Clonkex Posted at: 2018-01-21T05:54:39.087Z Reads: 327

```
Oh lol, nah I always just go with the easiest possible option. Grabbing a ruler works, so that's what I do. There's probably other more advanced and more accurate ways but who needs that for this kind of project :P
```

---
## \#607 Posted by: Zyb Posted at: 2018-01-21T10:00:52.574Z Reads: 349

```
Its aliveee :smile:![image|375x500](upload://9nrTbIcYEFDTb4cCFgAGmO35C3H.jpg)
god damn cat5 cable is so stiff i wish had some silicone wires laying around :frowning: 

@solidgeek status leds still relevant? I don’t have led holes on my copy :confused:
```

---
## \#608 Posted by: solidgeek Posted at: 2018-01-21T14:43:29.708Z Reads: 343

```
@Snowi I am not sure the A3144 would work. The Hall sensor needs to have a "ratiometric output voltage", which means that the output voltage changes according to the magnetic field. Try searching on "Linear Hall-Effect Sensor" should give you something to choose from. 

@SeeTheBridges The holes are meant to be tapped, therefore the holes are 2.5mm instead of 3 so you are able to cut threads. I understand now that most people don't have tapping equipment to do so, I will probably update the model to have 3mm holes instead. 

@Snowi All that GND wires is connected, it is just a simple way to show it. 

@Zyb Looks good! Well the status LEDs are gone, simply because the OLED display shows all the relevant information :-)
```

---
## \#609 Posted by: Achmed20 Posted at: 2018-01-21T18:30:36.290Z Reads: 336

```
parts ordered. in 30-50 days we know more :)
should be enough for 5 remotes. also, i wanted to play arround with a few other designs. i want something with trigger and a bigger screen.

PS: thanks for all the effort :slight_smile:
```

---
## \#610 Posted by: SeeTheBridges Posted at: 2018-01-22T01:05:52.567Z Reads: 340

```
So Ive been reading up a shit ton to learn all about how VESCs and voltages and everything work... In general, you shouldn't need a step-down circuit for the TX and RX pins coming from the Arduino because those are 5V tolerant pins on the STM32F4 CPU that runs VESCs... SO, no need to worry about that. I can cross that off the list of things I was gonna potentially have to cover.
```

---
## \#611 Posted by: solidgeek Posted at: 2018-01-22T16:23:55.098Z Reads: 332

```
@SeeTheBridges Actually I tried to use a voltage divider with my remote today, just to give it a try. And all my UART communication stopped working. I used a 1k and 2k resistor, maybe the values were too high? Anyway if the pins are 5V tolerant, there are no need :slight_smile:

I had announced that I would be releasing a new software update today, but I have been having some issues to implement cruise control with RollingGeckos library. I found this library instead: https://github.com/bastianraschke/ESP8266VESC which has many more features, like setting the RPM value with UART. This I believe can be used to implement cruise control. Any thoughts on this? :D

EDIT: Just realised that RollingGecko has been working on another branch, that has the features I need: https://github.com/RollingGecko/VescUartControl/tree/imartinezl-master
```

---
## \#612 Posted by: Snowi Posted at: 2018-01-22T17:21:40.415Z Reads: 327

```
Anyone got an extra spring and micro switch they got? Or maybe even got extra magnets. I know most people bought a bulk of them so I would assume that they got no other use for them. I would love to get them off your hands. I am willing to pay for shipping and any other costs.
```

---
## \#613 Posted by: SeeTheBridges Posted at: 2018-01-23T01:08:55.894Z Reads: 329

```
Hmmm, well personally I'm not looking for cruise control. that sounds a little dangerous to me personally.

@Snowi where are you located? I've got spare springs and switches.
```

---
## \#614 Posted by: Snowi Posted at: 2018-01-23T01:51:35.042Z Reads: 316

```
I live in Las Vegas, NV. I can PM you the exact address and other info.
```

---
## \#615 Posted by: Pimousse Posted at: 2018-01-23T10:00:50.009Z Reads: 322

```
I checked the reference manual again crossing with the pin definition of UART port and your right.
So I was wrong, thanks for having pointed that !

@solidgeek : Strange. I use boards with 1k and 2.2k as voltage divider and it works fine.
What baudrate do you use ?
```

---
## \#616 Posted by: bimmer Posted at: 2018-01-23T11:19:22.401Z Reads: 324

```
Vesc 6 has nrf anyway this would be compatible?
```

---
## \#617 Posted by: solidgeek Posted at: 2018-01-23T21:06:31.214Z Reads: 336

```
@SeeTheBridges Well I like to be able to cruise at a certain speed, it's nice on long trips :-)

@Pimousse Yeah I was puzzled by it too, it should have worked. I use 115200, do you think that should affect anything?

@bimmer Yeah the VESC 6 got a build-in nRF24 antenna, however, I have not been able to figure out how to use it yet, and Benjamin isn't of much help :frowning:  VESCs, in general, are so very complicated and - very undocumented.
```

---
## \#618 Posted by: Pimousse Posted at: 2018-01-24T10:37:03.067Z Reads: 342

```
When I use a simple Arduino powered by the VESC itself without other GND sharing, the comm. works flawlessly with the voltage divider even at 115200 bauds.

Now the point is that I'm using several devices connected to each other and it creates a mess with the GND.

![IMG_20171211_105223|666x500](upload://gj0hmTHTHnbMBipbzPDIrJOA6rz.jpg)

I resolved issues by removing GND connection between VESC and Arduino and between Rx and Arduino.
So no more loop, the GND is now shared through UBEC only.
However, I can't go above 9600 bauds otherwise I loose the comm.
Don't know why.
I still have a lost packet time by time, but It's only for monitoring purpose so it doesn't really matter.

About nRF, Benjamin designed it to be compatible with his nRF controller. 
Check the corresponding github repo, you'll find more details about nRF comm.
Anyway, I'm agree : there's freaking NO documentation although the VESC Project is meant to be a wide Open Source project...
I asked at the begin of the beta program to allow disabling the nRF module (thus avoiding to pollute with undesired RF on the same band as the bluetooth), but Trampa refused.
I'm still convinced that it really doesn't help metr.at module to have a steady connection. :neutral_face:
```

---
## \#619 Posted by: Snowi Posted at: 2018-01-24T17:45:48.868Z Reads: 329

```
I was wondering if this booster works. It goes from 3V to 5V so I assume it would work. It just uses USB, but I could exchange that with micro USB. 

https://www.ebay.com/itm/122482998236
```

---
## \#620 Posted by: SeeTheBridges Posted at: 2018-01-24T18:01:42.084Z Reads: 341

```
Hmm, I got my receiver all wired up, and it powers on. But for some reason I'm having that reset issue where the remote won't connect unless I press the reset button on the receiver. The other guy in the thread with the issue got lucky and it sorted itself out 😤 so thats no help

EDIT: Hmmm, If I turn my board on an off a couple times, the receiver fixes itself. No idea what to do to make it a proper fix, but I'm just gonna hit the power button a bunch until it cooperates 🤷‍♀️
How would I calibrate my remote without firmware 2.0?
```

---
## \#621 Posted by: solidgeek Posted at: 2018-01-24T23:53:26.292Z Reads: 329

```
Do you experience the same issue while the receiver is powered from USB and disconnected from VESC? And have you added a capacitor on the receiver 5v input? A few pictures of your wirering and setup would be nice :slight_smile:
```

---
## \#622 Posted by: solidgeek Posted at: 2018-01-24T23:54:44.634Z Reads: 323

```
It would work, but remember to make sure that it fits inside :slight_smile:
```

---
## \#623 Posted by: solidgeek Posted at: 2018-01-25T00:02:46.263Z Reads: 335

```
Removing that GND between the Arduino and VESC seems very dangerous, unless of course the Arduino gets GND through UBEC. Why have you connected Arduino receiver with UBEC? I would remove the ground connection between UBEC and Arduino, and keep the one between VESC and Arduino.
```

---
## \#624 Posted by: SeeTheBridges Posted at: 2018-01-25T00:48:48.831Z Reads: 321

```
Yeah, it happens on USB too. Is there a way to verify on the serial monitor that the signal from the remote is going through to the receiver?
```

---
## \#625 Posted by: Snowi Posted at: 2018-01-25T02:45:46.831Z Reads: 339

```
what would you prefer: (sorry for spam but i just found a couple options i can do)
https://www.amazon.com/DROK-Converter-Voltage-Regulator-Portable/dp/B00BZJ1DEC/ref=sr_1_11?ie=UTF8&qid=1516847439&sr=8-11&keywords=3v+to+5v+boost+converter

https://www.ebay.com/itm/122482998236
```

---
## \#626 Posted by: Pimousse Posted at: 2018-01-25T05:19:42.446Z Reads: 320

```
Yes, the UBEC shares the GND. If only I could use VESC power, of course I won't use a UBEC, but Îm powering a lot of ws2812.
The total consumption is a bit high for the 2A 5V regulator built in the VESC.
```

---
## \#627 Posted by: ervinelin Posted at: 2018-01-25T14:12:32.998Z Reads: 318

```
I still have the same problem.. need to power cycle a few times to get it connected.. sometimes it fires up on the first try, sometimes not...

Only good thing is once the receiver is connected, I can turn off the remote and turn it on again without the same problem.

No other solution for now... Hoping the new firmware will resolve this.
```

---
## \#628 Posted by: SeeTheBridges Posted at: 2018-01-25T19:55:09.175Z Reads: 312

```
Hmm, so I finally got my remote and receiver mostly working. Still having the power issues, but right now I'm more concerned with another issue. The Receiver is outputting to PWM with a MASSIVE min and max values. My maytech VESCs freeze anytime the timings go above 1ms annoyingly enough. I managed to fix it by going into the transmitter code and changing some values in the calculateThrottlePosition portion of the code. By lowering the maxHallValue and raising the minHallValue, I got my PWM signals between .3 and .9ms. with that little change, the Firefly is compatible with the Pulse Echo board after 1 little recalibration 🤗
```

---
## \#629 Posted by: dg798 Posted at: 2018-01-28T03:03:38.343Z Reads: 300

```
been reading this thread for a while and looked at the github page.
@solidgeek do you know when part 3 of the tutorial on the home page is coming out.
```

---
## \#630 Posted by: dg798 Posted at: 2018-01-28T03:16:17.424Z Reads: 302

```
also does anyone have any or all parts that wants to sell them to me. im in the US
```

---
## \#631 Posted by: dg798 Posted at: 2018-01-28T13:50:14.980Z Reads: 297

```
Anyone have s fully functioning tested remote that they want to trade for a brand new nano x?
```

---
## \#632 Posted by: Jammeslu Posted at: 2018-01-28T13:54:39.195Z Reads: 297

```
not to be rude by any means but isn't that like an downgrade ?
```

---
## \#633 Posted by: dg798 Posted at: 2018-01-28T13:55:17.345Z Reads: 299

```
Not really for me.
I really like this remote and it’s functionality.
```

---
## \#634 Posted by: Jammeslu Posted at: 2018-01-28T13:59:00.673Z Reads: 301

```
yeah I mean for th gut that trades with you
```

---
## \#635 Posted by: dg798 Posted at: 2018-01-28T14:00:18.639Z Reads: 302

```
It depends on who u ask. Someone may want a smaller remote that’s a more simple design.
Just put out there just in case. Not trying to rip anyone off.
```

---
## \#636 Posted by: UniqueSnowflakeN27 Posted at: 2018-01-29T20:16:18.015Z Reads: 296

```
Is anyone selling completes of this remote? I'd love to buy one from you @solidgeek :) I'm in Sweden so shipping wouldn't be that bad!
```

---
## \#637 Posted by: Jammeslu Posted at: 2018-01-29T20:17:19.259Z Reads: 295

```
jag har första beta, om din fixas snabbt kan han skicka i samma paket till oss @UniqueSnowflakeN27
```

---
## \#638 Posted by: UniqueSnowflakeN27 Posted at: 2018-01-29T20:19:51.057Z Reads: 290

```
Det har vart najs! Men annars går det säkert att posta det i ett kuvert med 2st frimärken(14kr), eftersom att den inte väger så värst mycket :slight_smile:
```

---
## \#639 Posted by: dg798 Posted at: 2018-01-29T23:35:52.684Z Reads: 304

```
I was also wondering if anyone is selling any completes. Didn’t quite understand @Jammeslu, and @UniqueSnowflakeN27 LOL
```

---
## \#640 Posted by: dg798 Posted at: 2018-01-29T23:39:44.792Z Reads: 311

```
I would take a beta as well.
```

---
## \#641 Posted by: Snowi Posted at: 2018-01-30T00:08:22.332Z Reads: 335

```
I was wondering why we need a charger board and a boost converter board. Aren't there many other boards thats can do both?

EDIT: like i found a board like this, and it seems like it works. although i may be wrong.

https://www.amazon.com/gp/product/B071RG4YWM/ref=ox_sc_sfl_title_2?ie=UTF8&psc=1&smid=A1N6DLY3NQK2VM
```

---
## \#642 Posted by: SeeTheBridges Posted at: 2018-01-30T01:25:21.742Z Reads: 322

```
That's just a charger/protection circuit. It doesnt boost the voltage to 5V.
```

---
## \#643 Posted by: chinzw Posted at: 2018-01-30T19:15:18.259Z Reads: 327

```
There's the adafruit feather that comes with everything in one simple package. BMS, Boost and Arduino.
```

---
## \#644 Posted by: dg798 Posted at: 2018-01-30T23:40:33.475Z Reads: 321

```
I was just on their website and found this awesome module https://www.adafruit.com/product/3458.
It says you can buy one of their 3.7v 500 mah batteries and it already had a connector to plug in the battery and is compatible with a USB for charging. This is the best of all worlds!!
```

---
## \#645 Posted by: dg798 Posted at: 2018-01-30T23:41:12.057Z Reads: 297

```
Great idea @chinzw
```

---
## \#646 Posted by: chinzw Posted at: 2018-01-30T23:53:47.034Z Reads: 299

```
Im using their Proto M0, but its almost the same thing. Just make sure you buy the 3.3v hall sensors. Im using these sensors:
DRV5053OAQLPGM
DRV5053PAQLPGM

They are the same sensor, just different sensing ranges.
```

---
## \#647 Posted by: dg798 Posted at: 2018-01-31T00:08:13.629Z Reads: 303

```
Also can I use a 500 mah battery or does it have to be 400 mah
```

---
## \#648 Posted by: dg798 Posted at: 2018-01-31T00:08:34.712Z Reads: 299

```
Also do you have a link for this sensors, never mind found.
```

---
## \#649 Posted by: chinzw Posted at: 2018-01-31T01:38:37.460Z Reads: 302

```
You can use any mah battery you want, the bigger the better, just make sure it fits in the case.
```

---
## \#650 Posted by: dg798 Posted at: 2018-01-31T01:41:22.347Z Reads: 300

```
Also do I need a special PA LNA NRF24L01 module.
I’m trying to get everything from the us and this is one thing I can’t seem o find for less than $20
```

---
## \#651 Posted by: Snowi Posted at: 2018-01-31T04:17:48.454Z Reads: 301

```
Is anyone interested in buying magnets from me? 5x5mm obv but I bought bulk of those magnets so I can ship it to anyone in US. Just pay for shipping.
```

---
## \#652 Posted by: stormboard1 Posted at: 2018-01-31T07:07:48.782Z Reads: 297

```
anyone selling completes in eu?
```

---
## \#653 Posted by: Pedrodemio Posted at: 2018-01-31T23:40:31.459Z Reads: 290

```
@solidgeek where do I find the power switch? The remote that i made uses the same as your, but I pulled it out of some old toy or something and it gone bad

No matter where I search or they never have something this small or it’s out of stock, maybe I’m using the wrong nomenclature for this type of switch
```

---
## \#654 Posted by: chinzw Posted at: 2018-02-01T00:44:34.078Z Reads: 288

```
Just get a spst switch from any electronics store.
```

---
## \#655 Posted by: dg798 Posted at: 2018-02-01T00:45:28.696Z Reads: 284

```
can i use this adafruit module https://www.adafruit.com/product/3406 so i only have too get one nrf24 module for reciever?
```

---
## \#656 Posted by: Pedrodemio Posted at: 2018-02-01T00:48:36.535Z Reads: 285

```
thanks, but the normal switches are too big, maybe in this remote the larger switches are used, in mine its about half of an H-H switch
```

---
## \#657 Posted by: chinzw Posted at: 2018-02-01T00:52:31.569Z Reads: 282

```
They're called mini slide switches.
```

---
## \#658 Posted by: Pedrodemio Posted at: 2018-02-01T01:22:16.419Z Reads: 289

```
Thanks, exactly this one https://www.pololu.com/product/1408

I will see if i can find locally
```

---
## \#659 Posted by: dg798 Posted at: 2018-02-01T02:09:13.365Z Reads: 301

```
anyone have any micro switches willing to give to me and i pay postage. im in the US
```

---
## \#660 Posted by: dg798 Posted at: 2018-02-01T02:48:28.429Z Reads: 318

```
![image|375x500](upload://jRiU6JjsXwpXzEnXDMhdL3kbdDR.jpg)
Can I connect this to arduino and use it as ppm and then use a separate uart cable
```

---
## \#661 Posted by: chinzw Posted at: 2018-02-01T19:31:29.634Z Reads: 305

```
No, that wont work
```

---
## \#662 Posted by: dg798 Posted at: 2018-02-01T19:39:34.316Z Reads: 304

```
do I connect the uart and ppm to arduino or just uart?
```

---
## \#663 Posted by: dg798 Posted at: 2018-02-01T19:39:54.851Z Reads: 300

```
Also where can I get a uart cable? Do I need any resistors between arduino and vesc?
```

---
## \#664 Posted by: Seikeau Posted at: 2018-02-01T21:57:47.529Z Reads: 294

```
Would it be possible with this remote to program the receiver to switch modes on the VESC like you can with some other bluetooth apps (e.g. Ackmaniac)?
```

---
## \#665 Posted by: Jamy Posted at: 2018-02-01T22:02:07.572Z Reads: 293

```
Technically, yea
```

---
## \#666 Posted by: dg798 Posted at: 2018-02-01T23:51:36.551Z Reads: 292

```
Let’s say for now I only wanted to use ppm and not uart, how would I wire that with the arduino and can I?
```

---
## \#667 Posted by: solidgeek Posted at: 2018-02-02T00:42:33.281Z Reads: 300

```
I would recommend buying Adafruit Feather 328P if you consider using one of their boards. The Feathers run at 3.3V so you will have to find another Hall sensor, as the one I use has a min voltage of 4.5V.

Wirering the receiver Arduino to PPM is easy. Connect pin 5 on Arduino to PPM, and of course, 5V to 5V and GND to GND.
```

---
## \#668 Posted by: dg798 Posted at: 2018-02-02T01:31:59.570Z Reads: 295

```
So I looked at the 328p but it doesn’t have a built in nfr24 module
```

---
## \#669 Posted by: dg798 Posted at: 2018-02-02T01:34:21.689Z Reads: 302

```
This is the hall sensor I’m getting. Will it work with the arduino that I want to get?
```

---
## \#670 Posted by: dg798 Posted at: 2018-02-02T01:37:29.965Z Reads: 320

```
Is this what I’m looking for?
![image|281x499](upload://prElN2mVff4TtxC3gTnwaObgDph.jpeg)

Also do I need to get magnets? If so where do they go exactly?
```

---
## \#671 Posted by: dg798 Posted at: 2018-02-02T13:56:33.638Z Reads: 290

```
If I wanted to do uart as well where can I find a uart cable or something like that?
```

---
## \#672 Posted by: amitbt69 Posted at: 2018-02-03T10:20:40.411Z Reads: 296

```
hi Predatorboards
I would like one remote. 
can you ship to Tel Aviv?
```

---
## \#673 Posted by: Fabian287 Posted at: 2018-02-03T10:59:47.818Z Reads: 308

```
@solidgeek can you add a Option to use a 128x64 oled. I think its more reliable. 

Fabian
```

---
## \#674 Posted by: ervinelin Posted at: 2018-02-05T09:12:19.421Z Reads: 334

```
So I've gotten many many kilometers in using my hacked mini remote (see above https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/471?u=ervinelin). I'm still waiting for solidgeek's latest firmware upgrade but in the meanwhile I'll stick to the older version which has worked well for me. 

In the meantime, I wanted to make it easier replicate build this remote without all that dremeling and with less need for 1001 wires running all over the place.

So the only way was to DIY a PCB for all the parts and to design a new enclosure for it. Again my personal preference is a trigger throttle over a thumb wheel, so my design is catered for that. It's also meant to be ambidextrous, so you can use it in either hand (OLED needs to be flipped either digitally or physically.. still not sure if it's possile). It's still work in progress but I've got all the parts and the PCB should reach me soon.

Here's some images of my progress thus far:

![DIY_Remote_Massing|649x499](upload://oObGsKWdQgZrkYtDT4pY08cILkv.JPG)
3D model showing where the stacked custom PCB will go

![IMG20180202222940|690x388](upload://wpYfRdUJGk17B9gQZnHz5gSqc6T.jpg)
For the trigger, I'm using a skate bearing. Not 100% necessary but I thought it's an interesting touch

![IMG20180204125943|281x500](upload://tZk09EJQsO1Flr6CnlOtbmW1knU.jpg)
Here's a terrible unfinished print of the remote (my printer really sucks) but you can get an idea of how big it is

You can see the cutout for the OLED on the top instead of the side (ambidextrous), below that is the mode switch then the power switch. Under the middle finger is a dead man's switch to prevent accidental throttling up when the remote is not held in the hand (necessary feature after I busted my finger getting caught in the gears because I accidentally hit the trigger).

If it works out well I'll release the PCB files and STLs... wish me luck!
```

---
## \#675 Posted by: Twinsen Posted at: 2018-02-05T09:56:19.471Z Reads: 305

```
@ervinelin I'm interested for sure. Coming from RC, I prefer the trigger as opposed to thumb throttle.
```

---
## \#676 Posted by: Hiorth Posted at: 2018-02-05T16:15:19.787Z Reads: 314

```
hello all!, I have not been very active on this forum yet, but I think I will build a Eskate soon😊
Here I made a **waterproof** remote casing, if anyone is interested.
I know it is a bit big, but it is to make it stay afloat in water. 

the Files are on thingieverse  
https://www.thingiverse.com/thing:2781808
more info and link to Efoilbilders can be found on thingiverse. 
.
```

---
## \#677 Posted by: Jammeslu Posted at: 2018-02-05T16:23:28.710Z Reads: 309

```
Not many will need a remote to float in water because most of us rides on land
```

---
## \#678 Posted by: solidgeek Posted at: 2018-02-05T21:44:36.265Z Reads: 303

```
Nice work! I like your design very much, and the idea of adding a bearing to the throttle is very interesting :D Regarding the PCB wouldn't you still need a boost and charger board, or is it integrated on the bottom of the PCB? 

I have also been working on a custom PCB for the remote for a while now, with all needed parts (atmega, regulators etc), however I still have a lot to do and learn about PCB design :)
```

---
## \#679 Posted by: ervinelin Posted at: 2018-02-06T01:58:39.852Z Reads: 314

```
@Twinsen I know what you mean, I always find thumbwheels very unnatural to operate.

@solidgeek  It's 2 PCBs stacked on top of each other, the DC booster, Lipo charger and NRF module go onto the bottom PCB (not seen in the image I shared).

![DIY-Remote-PCB-Top (1)|238x358](upload://r5VN2TrFE8GJcP79QRwZdBgSaOc.png)
Here's the top PCB, some of the pins connect to the bottom PCB (NRF and Batt pins)

![DIY-Remote-PCB-Bottom|238x358](upload://aK6y4tSX1mTxnNEdt43lDS0Nv3S.png)
Here's the bottom PCB which holds the DC boost, lipo charger, 10k resistor and 220uF cap, the NRF module is soldered to the back (pins running down the right).

The PCB just reached my post office, awaiting for it to be delivered to my home. I should be able to get it by the end of the week.

For those interested, I used EasyEDA for this, drew the schematic but I had to customise the board layout as they did not have most of the parts in the library.

I'm a total noob at this, and this is my very first DIY PCB so I'm keeping my fingers crossed that it turns out well. I could have saved a lot more space by compressing all the components into a custom board with inbuilt regulators and such but I have no skill to do something like this, so it's just off the shelf components which then get soldered to the PCB.

As for the enclosure design, the trigger works well, nice and smooth because of the bearing (still some friction due to spring arm and all). However I ran into some issues with the buttons, will need some adjustments to make sure they work well and don't get stuck.
```

---
## \#680 Posted by: ju_mpe_r Posted at: 2018-02-06T02:39:33.277Z Reads: 288

```
A-WE-SO-ME! :+1::smiley:
waiting for release!
```

---
## \#681 Posted by: ervinelin Posted at: 2018-02-06T03:32:41.314Z Reads: 301

```
For all those interested I compiled a list of things to buy, all from Aliexpress so it's just easier to track everything. Some smaller items like caps, resistors, screws I just got them from the local hardware shop.

https://docs.google.com/spreadsheets/d/1vXR9ce0m25Ap6XxzlymFo_pfpIeT2RAqWCypW-a-Jes/edit?usp=sharing

Do note that I have personally ordered these items and they work for me, your mileage might vary. Also some sellers are much faster at shipping than others.
```

---
## \#682 Posted by: Pimousse Posted at: 2018-02-06T08:30:46.689Z Reads: 294

```
Glad to see another people using easyeda ! :grinning: 
For sure it misses a lot of component.
But it's a collaborative tool, so you can create your own component, they will be shared with other users ;)
You can also use components of other people.

Did you use the EasyEDA "fabrication output" ?
I used it for a batch of 10x little PCBs. Very cheap (10$ shipped) and pretty good quality.
```

---
## \#683 Posted by: ervinelin Posted at: 2018-02-06T08:52:14.963Z Reads: 312

```
That's exactly what I did, designed and fabricated using EasyEDA.

PCBs are cheap as chips, was very surprised. They were also shipped out pretty quickly, less than a week from time or ordering.

BTW, I also created a receiver board PCB, will be easy as pie to wire up the NRF module now as compared to before when I needed 7 or 8 tiny wires between the module and the arduino!

![DIY-Remote-Receiver|146x339](upload://kC6NFzB1jHDONk7orTthapVVWEj.png)
```

---
## \#684 Posted by: Zyb Posted at: 2018-02-06T16:00:57.540Z Reads: 312

```
For those of electronics noobs like me normal size 5k resistor works just fine no need for smd. My cheap multimeter reads 200mA while charging a random 18650 battery. ![image|463x500](upload://tKgsw91Bu0Co2ImrwhjK7fFUec4.jpeg)
```

---
## \#685 Posted by: LunarKim Posted at: 2018-02-06T16:24:31.613Z Reads: 295

```
It is perfect of neatness!!!
```

---
## \#686 Posted by: Nandox7 Posted at: 2018-02-06T16:26:58.932Z Reads: 292

```
Is there any place other than thingiverse on on tho get the remote parts?
I see some with place for the LED's and other changes that I can't find in the thingiver list.

Cheers!
```

---
## \#687 Posted by: dg798 Posted at: 2018-02-06T18:01:45.682Z Reads: 281

```
You could always drill carefully and make the hole yourself
```

---
## \#688 Posted by: solidgeek Posted at: 2018-02-06T18:18:17.588Z Reads: 287

```
The LEDs are no longer supported, as everything is displayed on the display :-)
```

---
## \#689 Posted by: MatwoSvK Posted at: 2018-02-07T14:47:23.822Z Reads: 281

```
Hi guys is there someone who are willing to Print the parts for me and send them to me , only USA 
i paid ofc. Thank you
```

---
## \#690 Posted by: dg798 Posted at: 2018-02-07T17:46:00.865Z Reads: 293

```
Where exactly do the magnets and the hall sensor go in the housing?
Also I don’t understand the wiring for sv on the hall sensor and sv on oled. Where do they go exactly?
```

---
## \#691 Posted by: Migro Posted at: 2018-02-07T17:54:54.355Z Reads: 311

```
![27787189_10213711159647681_1267103884_o|375x500](upload://nHYjMfnaTlsQIY1KUqQCTlWU06J.jpg)![27781879_10213711159847686_768254049_n|375x500](upload://y6mMnGeJplKZhRVCL7IvfmIrlTq.jpg)

Magnets into the holes ind the throttle 3d print and in the buttom deres at slot for the hall sensor
```

---
## \#692 Posted by: dg798 Posted at: 2018-02-07T17:56:25.690Z Reads: 294

```
Wow thanks a lot man. Do u know exactly how the wiring goes for the oled sv and the hall sensor sv
```

---
## \#693 Posted by: Migro Posted at: 2018-02-07T17:56:55.316Z Reads: 300

```
Do you mean 5v? 
![image|690x407](upload://1Xh7rw2114h80WLd8O0FdYrhlWu.png)
```

---
## \#694 Posted by: dg798 Posted at: 2018-02-07T17:57:29.123Z Reads: 289

```
Yes do I splice the hall sensor 5v into the oled 5v?
```

---
## \#695 Posted by: Migro Posted at: 2018-02-07T17:58:25.161Z Reads: 287

```
Basically just all 5v needs to be connected from the boost converter output
```

---
## \#696 Posted by: dg798 Posted at: 2018-02-07T17:59:57.672Z Reads: 284

```
All the 5v wires go into the 5v pinout?
```

---
## \#697 Posted by: Migro Posted at: 2018-02-07T18:02:32.537Z Reads: 298

```
![image|690x488](upload://7ljIECaUNk1x9YpXaCayArs2q5d.png)
The 5v from the boost converter needs to go into the arduinos 5v and all the other 5v's. 
Use the method you finds the easiest. I think i took a wire from boost moduels vout to 5v on arduino and all the other 5v to the 5v arduino :slight_smile:
```

---
## \#698 Posted by: dg798 Posted at: 2018-02-07T18:03:52.975Z Reads: 277

```
Got it, one more question, all the grounds I don’t need right? I don’t need to put any of them in the gnd of the arduino right?
```

---
## \#699 Posted by: Migro Posted at: 2018-02-07T18:06:42.313Z Reads: 276

```
You do yea. Otherwise your not finishing the loop. The ground needs to be connected just like 5v but all grounds together.
```

---
## \#700 Posted by: dg798 Posted at: 2018-02-07T18:08:08.767Z Reads: 273

```
Meaning all grounds to the same pinout? Also can I connect the switch to a6 instead of d4?
```

---
## \#701 Posted by: Migro Posted at: 2018-02-07T18:11:38.149Z Reads: 282

```
Aslong as the arduino i reciving ground from the boost connector it dosent really matter which of the ground outlets you use on the arduino
```

---
## \#702 Posted by: dg798 Posted at: 2018-02-07T18:12:35.473Z Reads: 277

```
What about the grounds from all the other things? They can all go to the same ground on the arduino?
```

---
## \#703 Posted by: Migro Posted at: 2018-02-07T18:14:28.384Z Reads: 292

```
![Fixed|690x259](upload://tU2OQYbISySubNigJflMUDitQ9n.png)
Correct i tried to put this together not as beautiful as the original 2. But maybe easier for some
```

---
## \#704 Posted by: dg798 Posted at: 2018-02-07T18:15:41.976Z Reads: 277

```
Ok great amazing now I understand. Can I put the switch to a6 instead of d4?
```

---
## \#705 Posted by: Migro Posted at: 2018-02-07T18:16:40.966Z Reads: 270

```
Think you mean d instead of a. But the problem by doing that is then you need to change something in the code
```

---
## \#706 Posted by: dg798 Posted at: 2018-02-07T18:18:07.885Z Reads: 264

```
No I mean a6.
If I find the code that defines d4 I can just put in a6 instead no?
```

---
## \#707 Posted by: Migro Posted at: 2018-02-07T18:20:01.499Z Reads: 259

```
I actually dont  know the answer for this. im not that good at coding. But i know that the a ports is analog ports and they are different to the d (digital) ports. If it is possible i do not know :confused: :slight_smile:
```

---
## \#708 Posted by: dg798 Posted at: 2018-02-07T18:21:08.802Z Reads: 257

```
Ok thanks anyways for all ur help. Really appreciate it. If anyone knows the answer please let me know.
```

---
## \#709 Posted by: Migro Posted at: 2018-02-07T18:22:17.539Z Reads: 258

```
No problem, glad to help :slight_smile:
```

---
## \#710 Posted by: dg798 Posted at: 2018-02-07T18:23:03.336Z Reads: 262

```
The reason why I’m asking about the d4 is because I’m getting the adafruit feather nrf52 module which doesn’t have any d
```

---
## \#711 Posted by: Migro Posted at: 2018-02-07T18:27:10.967Z Reads: 261

```
Ahh i see. Theres probably some clever minds here to answer that question :slight_smile:
```

---
## \#712 Posted by: SeeTheBridges Posted at: 2018-02-07T18:59:58.403Z Reads: 275

```
Pretty sure someone was saying that bluetooth isn't a great protocol to use for these remotes because of possible interference from everything around you. The NRF52 uses Bluetooth LE, but I think the same problem still persists...
```

---
## \#713 Posted by: dg798 Posted at: 2018-02-07T19:42:20.159Z Reads: 283

```
It does but it also is compatible with nrf modules
```

---
## \#714 Posted by: Deakbannok Posted at: 2018-02-07T21:45:09.139Z Reads: 298

```
It takes 2 months to get all the things I need. It takes 2 hours to build.

The trigger switch was little pain to get them fit right.
![20180207_215319|690x388](upload://eZvw0HPCvRnqXZQhNZWCkqpBG6o.jpg)
```

---
## \#715 Posted by: Migro Posted at: 2018-02-07T22:56:38.890Z Reads: 291

```
@Deakbannok  Did you make it leftie?
```

---
## \#716 Posted by: dg798 Posted at: 2018-02-07T23:01:40.444Z Reads: 282

```
Anyone have an answer to my question
```

---
## \#717 Posted by: Deakbannok Posted at: 2018-02-07T23:15:35.553Z Reads: 283

```
yesi am goofy
```

---
## \#718 Posted by: Migro Posted at: 2018-02-07T23:52:22.946Z Reads: 282

```
Did you just flip the stl files? if so did the display still fit?
```

---
## \#719 Posted by: SeeTheBridges Posted at: 2018-02-08T01:53:03.013Z Reads: 300

```
So I've been staring at the pinout for the feather, and honestly, unless you're prepared to be going through all of solid geeks code and making the necessary changes yourself, you'd be better off not trying to use a feather. you'll need to redefine pretty much every pin used. 

https://cdn-learn.adafruit.com/assets/assets/000/046/248/original/microcontrollers_Feather_NRF52_Pinout_v1.2-1.png?1504885794

Although... on the other hand this may simplify the whole design since this has an integrated lipo charger as well... hmmm...
```

---
## \#720 Posted by: dg798 Posted at: 2018-02-08T02:03:05.085Z Reads: 289

```
i would actually only have to redefine anything that goes to a d pin as the feather has a0-a7 already.
```

---
## \#721 Posted by: dg798 Posted at: 2018-02-08T02:17:50.839Z Reads: 282

```
i mean do i need a digital output pin for the micro switch?
```

---
## \#722 Posted by: dg798 Posted at: 2018-02-08T02:23:46.626Z Reads: 278

```
@solidgeek any input on this topic??
```

---
## \#723 Posted by: SeeTheBridges Posted at: 2018-02-08T02:26:28.115Z Reads: 272

```
Wait why wouldn't you just use a digital pin for the switch?
```

---
## \#724 Posted by: dg798 Posted at: 2018-02-08T02:27:46.107Z Reads: 264

```
there is no digital pin on the feather
```

---
## \#725 Posted by: SeeTheBridges Posted at: 2018-02-08T02:28:59.935Z Reads: 264

```
What are all those Purple labeled pins then?
```

---
## \#726 Posted by: dg798 Posted at: 2018-02-08T02:31:22.087Z Reads: 258

```
if you saw the pic it said the purple/green ones were ide
```

---
## \#727 Posted by: SeeTheBridges Posted at: 2018-02-08T02:32:23.978Z Reads: 258

```
Yeah, does that mean the rest are not addressable?
```

---
## \#728 Posted by: dg798 Posted at: 2018-02-08T02:33:51.255Z Reads: 260

```
to be honest, im not sure. since though i only need to wire up the oled and micro switch and hall sensor. all of them go to analog pins except for the microswitch. thats the pin in question
```

---
## \#729 Posted by: dg798 Posted at: 2018-02-08T02:37:18.467Z Reads: 259

```
actually its only 2 pins that are ide. the key on the diagram doesnt show what purple is.
hmm....
```

---
## \#730 Posted by: SeeTheBridges Posted at: 2018-02-08T02:38:49.751Z Reads: 261

```
Yeah... Im pretty sure the rest are addressable as digital pins? It wouldn't make sense for them not to be. It even says you can set most of them to PWM too so they HAVE to be addressable somehow.
```

---
## \#731 Posted by: dg798 Posted at: 2018-02-08T02:39:20.163Z Reads: 264

```
alright then we solved the problem. thanks a million man.
cant wait to start ordering.
```

---
## \#732 Posted by: chinzw Posted at: 2018-02-08T04:32:30.299Z Reads: 263

```
Onboard nrf, lipo charger, booster. Its a much more elegant solution.
```

---
## \#733 Posted by: bimmer Posted at: 2018-02-08T05:02:04.613Z Reads: 261

```
So will this work with a vesc-6?
```

---
## \#734 Posted by: Deakbannok Posted at: 2018-02-08T06:37:27.742Z Reads: 261

```
Yes I mirrored the STL on all the parts and the display is still fit perfect. I will do the right hand for my friend later.
```

---
## \#735 Posted by: SeeTheBridges Posted at: 2018-02-08T07:23:58.929Z Reads: 258

```
Quite elegant, but no booster on this board. Everything is at 3.3v
```

---
## \#736 Posted by: solidgeek Posted at: 2018-02-08T10:15:06.064Z Reads: 283

```
@dg798 As I mentioned earlier I recommend using the Adafruit Feather 328P, as this has the same pins as an Arduino Nano. The NRF54 version is NOT compatible with my software at all, as this module is using Bluetooth.

The feather 328P should be compatible with all software and hardware, except that you will need a 3.3V Hall sensor instead.   

EDIT: The Adafruit Feather M0 Basic Proto should also work

@bimmer Actually I got a VESC 6, and as long as you use the right library from RollingGecko it works just fine.
```

---
## \#737 Posted by: ervinelin Posted at: 2018-02-08T11:11:43.764Z Reads: 310

```
PCBs are in!!! Made some small mistakes but doesn't affect functionality....

Unfortunately I misjudged how thick the stack becomes when I use headers... So I had to get creative to flatten the stack to fit.

![IMG20180208165007|281x500](upload://h0EdFZuQ5ieO5MGW9NMpVOuZuME.jpg)
Bare PCBs

![IMG20180208173904|690x388](upload://bv8M3BjLnVeP0vCgrF0k1BhHz5H.jpg)
So much easier to solder than 1001 wires!!

![IMG20180208173918|690x388](upload://xyVZbepzrYpImf8pr8CBXjdZ00t.jpg)
NRF module is at the bottom

![IMG-20180208-WA0036|281x500](upload://6QUNlNKqnt5F2sX2rkjC78fStNr.jpeg)
Pin headers made the stack too thick

![IMG20180208183442|690x388](upload://3waXl4ibAx6OxmjsXEZeiHcLNmq.jpg)
Had to get creative with the soldering to flatten the stack

![IMG20180208183548|690x388](upload://bEL1M69Dpp1FIz2Tbzo2pakYPQT.jpg)
I should have flipped the Arduino so the usb doesn't get blocked by the lipo... Sigh...

Now if my 3D printer could just cooperate with me that would be great...
```

---
## \#738 Posted by: LunarKim Posted at: 2018-02-08T11:16:28.881Z Reads: 291

```
It is completely neat and compact.
```

---
## \#739 Posted by: Migro Posted at: 2018-02-08T11:41:19.893Z Reads: 292

```
That looks amazing. They did the same thing on my bms from bestech ![image|187x250](upload://ozIBkHxpXFYkOQ9zO9xgtPtIAc0.jpg)

Whats your reason for the lipy battery you choose?
```

---
## \#740 Posted by: dg798 Posted at: 2018-02-08T12:24:40.764Z Reads: 286

```
I know it says that but I looked at the Nordic website for the chip and it says it’s on air compatible with an nrf24l module
```

---
## \#741 Posted by: dg798 Posted at: 2018-02-08T12:25:45.049Z Reads: 283

```
Also the 328p and Proto M0 doesn’t have any d pins either if I’m not mistaken
```

---
## \#742 Posted by: ervinelin Posted at: 2018-02-08T12:38:31.030Z Reads: 283

```
Ah so I am not so creative after all with my soldering!!

As for lipo... It's what I had lying around, also it fits, can easily buy more of the exact same size if I wanted, plus it has higher capacity so you can go without charging for a long time...

Only problem is you gotta solder direct to the lipo...
```

---
## \#743 Posted by: Migro Posted at: 2018-02-08T12:52:53.414Z Reads: 301

```
@ervinelin i see. 

![image|375x500](upload://apSrY7lY1nrhipcqBnnznEFEton.jpg)
![image|375x500](upload://tkSJ19XqjZ7jo3LkKw4JQe9W3Ku.jpg)
Can anyone explain why something gets so hot that it melts the plastic?  
I think it is when i charge but not sure. The middle divider also bend. The charge module was melted into the plastic as you can see in second picture it left a mark from one of the corners. :confused:
```

---
## \#744 Posted by: ervinelin Posted at: 2018-02-08T13:20:11.852Z Reads: 280

```
My charge module got super hot and basically fried when i accidentally reversed the polarity of the lipo
```

---
## \#745 Posted by: solidgeek Posted at: 2018-02-08T13:50:57.564Z Reads: 283

```
Did you remember to change the Rprog to a 5kOhm instead of the standard 1,2kOhm? The 1,2kOhms resistor set the max charge current of 1A, which is way too much. A resistor value of 5kOhm limits the current to 250mA.
```

---
## \#746 Posted by: dg798 Posted at: 2018-02-08T13:57:07.848Z Reads: 279

```
@chinzw, I know that you use the proto M0.
Would you mind making a diagram of how to wire the oled, micro switch, hall sensor, and nrf module for me please?
I really don’t want to blow anything up lol!
```

---
## \#747 Posted by: dg798 Posted at: 2018-02-08T14:03:20.777Z Reads: 273

```
And also @solidgeek, I don’t see how the pins on the 328p are the same as the nano?
```

---
## \#748 Posted by: Migro Posted at: 2018-02-08T14:23:26.398Z Reads: 273

```
I did not, i dont have these small resistors. But i may have made another wiring mistake which is only when charging..
```

---
## \#749 Posted by: ervinelin Posted at: 2018-02-08T14:40:25.445Z Reads: 274

```
This would have caused the lipo to overheat... Not the charger I think.
```

---
## \#750 Posted by: ervinelin Posted at: 2018-02-08T14:41:45.157Z Reads: 302

```
Soldered up a receiver board... Nice and neat

![IMG20180208223040|281x500](upload://tpJkYnOnxaGJ6EGw9Wr7mmPYjdN.jpg)

![IMG20180208223042|281x500](upload://aagMLzP5M2RtMZghAlbDYvwmgCU.jpg)

But I accidentally stripped one of the solder pads... Sigh so had to jumper it via a wire instead.. should still work I hope..
```

---
## \#751 Posted by: navgor Posted at: 2018-02-08T15:35:24.475Z Reads: 290

```
Which BMS model is that? Do you recommend it? I'm in the market for a 60+ amp 12s BMS.
```

---
## \#752 Posted by: navgor Posted at: 2018-02-08T15:39:26.736Z Reads: 312

```
If anyone wants some high quality 3D prints I can do a small run of SLA 'Tough' resin on my Formlabs Form2. 

I just printed some abec pulleys and they came out fantastic and dramatically stronger than the standard resins which are brittle.

The 'Tough' resin is apparently as strong as ABS.

![IMG_0108|375x500](upload://cl6SUWzPqYAaSHuFqUAm76RTNrM.jpg)![IMG_0106|375x500](upload://zfXoG8KlAIYi6zI5aKoiMCkGrhA.jpg)![IMG_0111|375x500](upload://8fYIgftfrFQFrjogpQxW2zVWZaj.jpg)![IMG_0110|666x500](upload://gUaLmZmusgT1rfVri1VNp0QfTJg.jpg)![IMG_0109|375x500](upload://okW3T6fUnLDbWSZGjLBvpycIsOi.jpg)![IMG_0107|375x500](upload://cv3mOIrdmE7ioxTGaE5pPaV08Am.jpg)
```

---
## \#753 Posted by: Surfer Posted at: 2018-02-08T15:47:06.537Z Reads: 299

```
Wow that's awesome! Maybe you want to print the remote? Is just the last part what I need.
Well and 3d printer also need 😁
```

---
## \#754 Posted by: navgor Posted at: 2018-02-08T17:18:14.258Z Reads: 306

```
I've been getting a few PM's about prints. I'm based in London, UK but can ship globally for cheaply though my business ([e-bikes for those interested](http://www.analogmotion.co.uk)). This resin is absurdly expensive compared to filament but I did some quick calculations and I can print a full remote for £34 shipped to uk or 57usd shipped anywhere in the world.

PM me if you want one and I'll send PayPal details. I've already done a few prints for other forum members.
```

---
## \#755 Posted by: dg798 Posted at: 2018-02-08T17:54:10.743Z Reads: 292

```
Can I use this nrf module: https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F222469277836
```

---
## \#756 Posted by: Migro Posted at: 2018-02-08T17:55:19.063Z Reads: 286

```
thats the one im using cause i had em laying around
```

---
## \#757 Posted by: dg798 Posted at: 2018-02-08T17:55:38.626Z Reads: 286

```
Have u had any break ups or connection issues?
```

---
## \#758 Posted by: dg798 Posted at: 2018-02-08T17:59:24.715Z Reads: 286

```
Because also that one isn’t pa lna
```

---
## \#759 Posted by: Migro Posted at: 2018-02-08T18:00:33.125Z Reads: 287

```
havent made the reciever yet, so i dont know yet. Still waiting for a connector cable.
```

---
## \#760 Posted by: dg798 Posted at: 2018-02-08T18:01:10.641Z Reads: 291

```
How would I wire that module. I didn’t see any labels for the pins in any of the pictures on eBay
```

---
## \#761 Posted by: Migro Posted at: 2018-02-08T18:02:21.684Z Reads: 301

```
![image|690x320](upload://3mxfn7RwhUfP9Jgm5ZmAsHkcYNs.jpg)
```

---
## \#762 Posted by: dg798 Posted at: 2018-02-08T18:02:56.762Z Reads: 292

```
Great thanks!!
```

---
## \#763 Posted by: dg798 Posted at: 2018-02-08T18:04:43.465Z Reads: 290

```
On the arduino that I’m getting it only has 2 3.3v outputs. I found a hall sensor that can work at 3v and so can the oled but I still need another rail for the nrf module. Can I solder the oled and sensor both to the same 3.3v rail?
```

---
## \#764 Posted by: dg798 Posted at: 2018-02-08T18:06:51.379Z Reads: 269

```
And I don’t need to wire any of the boost converters and what not becaus I have a built charger on it.
```

---
## \#765 Posted by: Migro Posted at: 2018-02-08T18:10:38.089Z Reads: 273

```
Yea you should be able to just wire to the same one. Im pretty sure it just depends on the amp draw or something and i dont think your exceeding that on the 3.3v outputs. So if the hall sensor and display is able to do 3.3v i dont see why not.
```

---
## \#766 Posted by: dg798 Posted at: 2018-02-08T18:11:10.444Z Reads: 276

```
Ok thanks again!
😃
```

---
## \#767 Posted by: mmaner Posted at: 2018-02-08T20:42:38.535Z Reads: 273

```
So...who's gonna me and sell me one of these?
```

---
## \#768 Posted by: SeeTheBridges Posted at: 2018-02-08T22:24:03.950Z Reads: 279

```
Currently working on that ;)
```

---
## \#769 Posted by: dg798 Posted at: 2018-02-09T02:33:06.414Z Reads: 273

```
anyone want to make a diagram to wire this up with an adafruit protoM0. its a bit different then a regular nano.
i just dont want to blow anything up
```

---
## \#770 Posted by: MatwoSvK Posted at: 2018-02-09T05:42:26.557Z Reads: 271

```
@solidgeek or anyone else ?
One thing, how you connect receiver to Vesc ? cause in your  github Wiki still missing part 3 Receiver electronic.
```

---
## \#771 Posted by: Der6FingerJo Posted at: 2018-02-09T06:43:14.828Z Reads: 279

```
[quote="dg798, post:763, topic:28543, full:true"]
On the arduino that I’m getting it only has 2 3.3v outputs. I found a hall sensor that can work at 3v and so can the oled but I still need another rail for the nrf module. Can I solder the oled and sensor both to the same 3.3v rail?
[/quote]

You might want to use a small capacitor on the nrf if you use all the peripherals on the 3.3V rail of the arduino. (around 100-500µF)
With a somewhat bigger capacitor my arduino nano can even reliably drive a nrf24 pna module.
```

---
## \#772 Posted by: Migro Posted at: 2018-02-09T07:12:29.127Z Reads: 292

```
Its mentioned earlier here
[quote="solidgeek, post:353, topic:28543"]
The receiver nRF24 is wired the same as the remote. The Arduino should be connected to the VESC in this manner:

TX → RX

RX → TX

5V → 5V

GND → GND

D5 → PPM
[/quote]
```

---
## \#773 Posted by: Boesila Posted at: 2018-02-09T10:27:44.715Z Reads: 305

```
Hi all, 

to which Pin exactly should i connect D5 at the VESC6? Do you mean SERVO at the PPM port? 
Thanks in advance 

![image|307x500](upload://6w1Or2odwdCCKhdbSmhEraQnisj.png)
```

---
## \#774 Posted by: ervinelin Posted at: 2018-02-09T17:04:30.069Z Reads: 295

```
Servo (ppm), 5v and ground go to the receiver, along with Tx and Rx from the comms port.
```

---
## \#775 Posted by: ervinelin Posted at: 2018-02-09T17:06:58.318Z Reads: 306

```
Need some final adjustments to the 3D model but I am almost there!!

![IMG20180210010129|690x388](upload://pgM64LwMqQFy8tFL6ZTxVixZ3el.jpg)

The skate bearing trigger makes it really smooth and the buttons I think should work just fine... Now just need one final set of adjustments and I will be good to wire everything up!
```

---
## \#776 Posted by: dg798 Posted at: 2018-02-11T01:08:05.390Z Reads: 298

```
alright, having parts 3d printed as i type and ordering all parts tonight!!
```

---
## \#777 Posted by: dg798 Posted at: 2018-02-11T01:14:10.745Z Reads: 300

```
just a question, will all this fit in the housing?
https://www.ebay.com/itm/262877977774
https://www.ebay.com/itm/222469277836
https://www.ebay.com/itm/142301748870
https://www.ebay.com/itm/202178620339

and of course the 502535 battery.
```

---
## \#778 Posted by: dg798 Posted at: 2018-02-11T01:32:48.394Z Reads: 272

```
and this magnet?  https://www.ebay.com/itm/161903088944
and this hall sensor?https://www.mouser.com/ProductDetail/595-DRV5053OAQLPGM
```

---
## \#779 Posted by: HighMasterGogo Posted at: 2018-02-11T12:08:00.346Z Reads: 290

```
I have the remote working really well. But I think my hall sensor may not be ideal.

If I quickly push or pull the thumb wheel to either extremity I get almost no acknowledgement in the PPM display in BLDC tool but If I I use my finger to manually restrict th  total sweep, I get perfect results no matter how slow of fast I operate the wheel.

It seems like, at the extremity of the wheel, the hall sensor is sending some crazy value.

However, in serial monitor I get a top value of 830, a bottom value of 110 and a middle value of 490. Also, the scale on the remote's LCD dimply is perfect. This makes me think it's a receiver issue?

Any ideas?
```

---
## \#780 Posted by: ron Posted at: 2018-02-11T13:27:04.756Z Reads: 300

```
Finally I finished the remote.

I am using a 500mAh Battery which fits perfectly into the battery place...

One question tho. I can enter the remote settings by holding down the Trigger button while turning on the remote, but I can not switch the menues by using the thumb wheel. It only shows the Trigger Menu and thats it. Is there any magic to it to browse the settings of the remote?

![DSC03635|333x500](upload://acWZffMN76EkoHPkh1rFQ3zddeP.JPG)
```

---
## \#781 Posted by: Migro Posted at: 2018-02-11T14:48:32.726Z Reads: 286

```
You need to change some variables in the code but cant remember which. Solidgeek said he would update IT so it should Work without changing anything in the code. But i Guess he is busy.
```

---
## \#782 Posted by: HighMasterGogo Posted at: 2018-02-11T17:38:13.683Z Reads: 285

```
Thanks, Migro. Do you know which variables?
```

---
## \#783 Posted by: moon Posted at: 2018-02-11T18:52:28.293Z Reads: 284

```
What's the difference between the two remotes?
```

---
## \#784 Posted by: ervinelin Posted at: 2018-02-11T19:32:42.212Z Reads: 278

```
Obviously one is a thumb wheel the other is a trigger mechanism. Electronics inside is almost identical.

Maybe I should start another thread so as not to confuse people...
```

---
## \#785 Posted by: moon Posted at: 2018-02-11T19:53:28.096Z Reads: 279

```
Yeah sorry for the dumb question, just that there's 800 replies to the thread and I thought something changed with the design
```

---
## \#786 Posted by: moon Posted at: 2018-02-11T19:56:18.559Z Reads: 273

```
For the springs, I have found 0.5x5x20mm is this fine?
```

---
## \#787 Posted by: Migro Posted at: 2018-02-11T22:00:27.378Z Reads: 282

```
@HighMasterGogo this is what he said earlier. I can't remember what i needed to change mine to, but i didn't get i all right. I just hope his next update should fix this.  

[quote="solidgeek, post:582, topic:28543"]
@SeeTheBridges Great! Well, it’s probably an issue with your magnets or the placement of your hall-sensor. If 


the magnets aren’t strong enough, the hall sensor will not return a high or low enough value. You have to tweak the min and max hall sensor values. I am adding a Hall sensor calibration function in the newest software update, which should be ready by Monday :slight_smile:

Otherwise if you can’t wait, you will have to go to the function controlSettingsMenu() and change the value 150 to a higher value (try with 250).
[/quote]


Aand for you @moon on the very top of this thread theres a link to a spreadsheet where all the parts is, if they match the dimensions he got it is probably fine. The link to the [spreadsheet](https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit#gid=0) ;)
```

---
## \#788 Posted by: moon Posted at: 2018-02-11T22:38:37.941Z Reads: 273

```
It says I need 2x

nRF24 module
Arduino Nano

Is this right?
```

---
## \#789 Posted by: dg798 Posted at: 2018-02-11T22:41:03.530Z Reads: 260

```
Yes one nano for transmitter and one for receiver. On nrf24 for transmitter and one for reciver.
```

---
## \#790 Posted by: moon Posted at: 2018-02-11T22:55:24.124Z Reads: 268

```
Oh makes sense :slight_smile:

Thanks
```

---
## \#791 Posted by: dg798 Posted at: 2018-02-11T23:03:27.203Z Reads: 259

```
Sure
10 charc
```

---
## \#792 Posted by: ervinelin Posted at: 2018-02-12T00:43:48.542Z Reads: 261

```
I actually use the same remote for two boards... So you need as many NRF modules as you need receivers.
```

---
## \#793 Posted by: dg798 Posted at: 2018-02-12T01:20:21.623Z Reads: 255

```
well said :smile:
```

---
## \#794 Posted by: dg798 Posted at: 2018-02-12T02:17:35.531Z Reads: 261

```
can someone tell me if all the parts i posted a few posts above will fit in the housing??
```

---
## \#795 Posted by: Deakbannok Posted at: 2018-02-12T03:59:23.731Z Reads: 263

```
If you can get a read from the controller and the value is showing perfectly then most likely is the the reciever. Hook up the receiver to computer and see what kind of transmit values the receiver is acquiring
```

---
## \#796 Posted by: SeeTheBridges Posted at: 2018-02-12T06:35:40.195Z Reads: 259

```
I changed my controlSettingsMenu() to 350 to get it working.
```

---
## \#797 Posted by: Achmed20 Posted at: 2018-02-12T08:45:28.579Z Reads: 268

```
nice!
i wanted to go this route as well because i dont realy like thumb triggers and also ebcause i wante4d a bigger screen.

but first im going to build the original :)
```

---
## \#798 Posted by: HighMasterGogo Posted at: 2018-02-12T09:05:31.058Z Reads: 261

```
Thanks everyone for your help.

I see there are two "150" values in the controlSettingsMenu, I assume I'd be wise to change both?

@Deakbannok, how do I get the receiver to print the values? To my knowledge there isn't serial output? I suppose I could code it to print to serial but I'm not great with code.
```

---
## \#799 Posted by: SeeTheBridges Posted at: 2018-02-12T17:04:14.808Z Reads: 268

```
Yeah. I changed both of mine to 350. And as for getting the receiver to spit out to serial monitor, just uncomment the "#define debug" at the top of the the code.
EDIT: Just kidding. the receiver doesn't have any debug code. thats only on the transmitter
```

---
## \#800 Posted by: Deakbannok Posted at: 2018-02-12T19:29:18.749Z Reads: 293

```
https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development

Here is his latest update v2

Go on setting and set your minimum; center; max throttle. There you will see your throttle position dedication.

With this v2. He added the reset pin and and LED pin to the receiver between pin 4 and 6.

I use the latest library version VESC 6 from
https://github.com/RollingGecko/VescUartControl/tree/VESC6

If you get error (**SERIALIO**) or cannot get a read from VESC v4.10 you need to update this to your receiver file

#define SERIALIO Serial
**void setup(){**
SetSerialPort(&SERIALIO);
SERIALIO.begin(115200);
 
For folks with Arduino Nano V3 with VESC 4.10 >
```

---
## \#801 Posted by: Migro Posted at: 2018-02-12T19:45:04.610Z Reads: 274

```
But the problem is that if you dont change the variables in the code your self you wont be able to change anything in the settings of the remote. Solidgeek said that he would fix this in the next update.
```

---
## \#802 Posted by: HighMasterGogo Posted at: 2018-02-12T21:32:53.560Z Reads: 279

```
thanks will give it a go
```

---
## \#803 Posted by: Deakbannok Posted at: 2018-02-12T21:45:02.059Z Reads: 294

```
Also someone please confirm this.

By default analog input to PPM from pin 5 to VESC is between 0 - 255 min/max

When I have tested on VESC Tools log *digitally.
The input from Receiver to VESC is cut off  when a full throttle and full break applied.

If I have low the analog input down to between 45-200 min/max. There is no cut off at all.

VESC V4.10 v3.3 Torqureboard
Arduino Nano V3
```

---
## \#804 Posted by: ervinelin Posted at: 2018-02-13T01:48:01.169Z Reads: 310

```
Partial success!

![IMG20180213011757|281x500](upload://ttiahTTQXmCOlTZZ0IgJCUnTBKe.jpg)
Internal wiring quite nicely routed compared to original version.

![IMG20180213020519|281x500](upload://jhWm7uYFbNwqWZFqcyR2gJ741oi.jpg)
OLED display position is very ergonomic now.. just one glance down and you can read it clearly

![IMG20180213020502|281x500](upload://u6Wgo3tCHQvrs4CFBGghkqfZPwx.jpg)
Deadman's switch is right under the middle finger. Hold the remote and it activates. I also adjusted the code so this only limits thorttle not brakes, realised after my first ride that I want brakes to be available all the time regardless of Deadman switch position... Good for those panicked moments!

First test ride was not good, several small issues one of which being the remote needs several hard resets to fire up, I suspect the capacitor is problematic. Will try another cap.

Also my receiver for some reason cuts out when the board is jolted... Very risky.. Suspect it's a loose connector somewhere...

![IMG20180213113011|281x500](upload://iAyB3GjTAX1CVbvbiQLzb6CXiUu.jpg)
Can't wait to upgrade to @solidgeek new firmware
```

---
## \#805 Posted by: SeanHacker Posted at: 2018-02-13T01:52:25.428Z Reads: 283

```
I want this. Good job dude!
```

---
## \#806 Posted by: dg798 Posted at: 2018-02-13T01:57:38.127Z Reads: 286

```
looks great man.
hopefully someone can sell me a complete soon!!:slight_smile:
```

---
## \#807 Posted by: ervinelin Posted at: 2018-02-13T04:02:13.243Z Reads: 287

```
For me I had to do two things, the first was to calibrate the remote. So you go in and adjust the midpoint as well as the ends based on the serial output.

After this I had to adjust the PPM limits within the VESC software (using older version)
```

---
## \#808 Posted by: Zyb Posted at: 2018-02-13T10:36:28.379Z Reads: 299

```
![image|375x500](upload://y40XAdw0nAClR1USWqOhL7uWl1y.jpg)

Doesn’t look pretty but it looks operational :slight_smile: 
Last night I left it for charging and after that when I tried to turn it on it was like dead no lights or anything. I checked the booster it had voltage so up until arduino everything was fine. Then I unplugged the usb(I power the arduino thru it’s usb socket) and tried another source of power again nothing. Then assembled it the way it was and it started to work again. Has anyone encountered this situation?
```

---
## \#809 Posted by: ervinelin Posted at: 2018-02-13T19:00:27.993Z Reads: 284

```
So I managed to resolve some problems, my remote now powers on as per normal after I removed the 220uF cap.

However, somewhere along the way I am no longer receiving telemetry data. I've tried using an older rx and remote and even swapping to another deck.

I checked baudrates, tx, rx pins, everything I could think of but I just cannot seem to get telemetry data back again..

Totally bummed... any ideas?
```

---
## \#810 Posted by: ron Posted at: 2018-02-13T19:01:02.087Z Reads: 276

```
This sounds like a Bad Wire Connection after the power switch..

Please check if the 5v pin of the Arduino measures 5v after turning your remote on in its current state.
```

---
## \#811 Posted by: Zyb Posted at: 2018-02-13T19:13:33.991Z Reads: 291

```
Will do thanks, it works ok for now I ll measure 5v output if it fails again. In the meantime wiring my receiver and adding this logic level converter to Tx/rx channels. I dunno if it’s going to work tho.![image|375x500](upload://pWCkH9Opi2Mjxv9KOzNnKAUcQfG.jpg)
```

---
## \#812 Posted by: Deakbannok Posted at: 2018-02-13T20:11:42.839Z Reads: 280

```
Did you upload a new version to the receiver?
reset your on receiver EEPROM see that will do if not then you might have the same problem I had earlier.
```

---
## \#813 Posted by: Zyb Posted at: 2018-02-13T20:59:56.584Z Reads: 284

```
![image|375x500](upload://qbitwpjZyV7haJf2ihl9a9Knqph.jpg)

Just finished the receiver. Is there any way to check if it’s working or not without connecting it to the vesc? When I power up the transmitter and the receiver, wireless icon on the screen becomes solid. Is that a good indication that there’s connection?
```

---
## \#814 Posted by: Migro Posted at: 2018-02-13T21:03:16.471Z Reads: 271

```
Havent finished mine yet, but im assuming that thats a good sign. I would say it is paired when it becomes solid. 

I've got at question to some code geniuses what should i change if i need to different remotes for 2 boards. I would assume you need to different "addresses" or something.
```

---
## \#815 Posted by: moon Posted at: 2018-02-13T21:04:52.140Z Reads: 266

```
I am thinking about ordering a bunch off stuff from Taobao, what AWG wire have people used?
```

---
## \#816 Posted by: Zyb Posted at: 2018-02-13T21:15:05.748Z Reads: 273

```
thanks for the input :slight_smile:

@moon
my transmitter battery came with some cheap 30awg wires. if the required current can flow from those cables i would assume 30 awg silicone wires are ok. i used them for signals and some 26 awg for power but i dont think 26 is necessary tho im not expert just my opinion.
```

---
## \#817 Posted by: Jamy Posted at: 2018-02-13T21:22:18.869Z Reads: 274

```
@Zyb yes, if it's not connected it'll be flashing.

@Migro You'd want to edit the pipe ID in both the [receiver code](https://github.com/SolidGeek/nRF24-Esk8-Remote/blob/master/receiver/receiver.ino#L14) and the [transmitter code](https://github.com/SolidGeek/nRF24-Esk8-Remote/blob/master/transmitter/transmitter.ino#L126).
You can generate a valid new pipe id [on this website](https://www.randomlists.com/string) (it has to be hexadecimal). On that site, enter base: 16, length: 10 and amount: 1.
Then you just need to add 0x in front and LL at the back.

(So if the site gives you `6188F15ED0` you want to add 0x in front and LL at the back so it becomes `0x6188F15ED0LL`)

Edit: I'm also maybe thinking of writing some code to auto pair on first boot. (And then maybe multiple boards in the config menu :D)
```

---
## \#818 Posted by: Migro Posted at: 2018-02-13T21:26:59.263Z Reads: 277

```
Amazing just what i needed :slight_smile: 
And thanks for the indepth explanation. 

The autor pair feature actually sounds quite cool :slight_smile:
```

---
## \#819 Posted by: Deakbannok Posted at: 2018-02-13T21:59:03.750Z Reads: 290

```
Here is my controller.
 I have the cruise control running and option to switch safety on and off. fixing the flow on the receiver and controller. also I will to short down the codes.
Arduino Nano capacity is only 30720 btyes

![20180213_224323|690x388](upload://t3sb8FdN5rnsRHqSQ3xT0SgNqjK.jpg)
```

---
## \#820 Posted by: chinzw Posted at: 2018-02-13T22:11:47.772Z Reads: 279

```
I just got the new adafruit nrf52 modules delivered, so ill be building with those.
@solidgeek any way i can get my hand on something more editable than a stl?
```

---
## \#821 Posted by: dg798 Posted at: 2018-02-13T23:39:23.192Z Reads: 275

```
@chinzw, do the nrf52 modules fit in the housing?
```

---
## \#822 Posted by: dg798 Posted at: 2018-02-13T23:40:13.821Z Reads: 269

```
Also once you are done with the wiring and everything works, would you mind opting a diagram for that module as that’s the one I would like to buy.
```

---
## \#823 Posted by: moon Posted at: 2018-02-14T01:12:22.057Z Reads: 268

```
How come the LED's and the power switch are missing from  the BOM?
```

---
## \#824 Posted by: moon Posted at: 2018-02-14T01:13:05.295Z Reads: 264

```
I assume not since he is asking for editable files
```

---
## \#825 Posted by: Migro Posted at: 2018-02-14T01:20:02.588Z Reads: 265

```
He removed the led's because everything is on the display know. 


Can anyone tell me how to get perfect throttle min and max and center in the remote settings?
```

---
## \#826 Posted by: chinzw Posted at: 2018-02-14T01:27:33.951Z Reads: 264

```
they do fit, but the usb port and some other things wont line up properly
```

---
## \#827 Posted by: dg798 Posted at: 2018-02-14T01:33:56.624Z Reads: 256

```
Are u updating the remote to fit? If so when you do can you pos the new version for those modules?
Also can you post a diagram of the wiring as it’s diferent than the nano?
```

---
## \#828 Posted by: chinzw Posted at: 2018-02-14T01:35:40.426Z Reads: 255

```
I'll be working on this probably this weekend
```

---
## \#829 Posted by: dg798 Posted at: 2018-02-14T01:38:43.267Z Reads: 257

```
Alright cool, let me know how it goes!
```

---
## \#830 Posted by: dg798 Posted at: 2018-02-14T02:40:48.546Z Reads: 260

```
anyone know of a diagram/breadboard maker like fritzing that i can use online. i cant really download anything because i have a chromebook.
```

---
## \#831 Posted by: ervinelin Posted at: 2018-02-14T05:44:35.805Z Reads: 267

```
I was wondering if you managed to get this to work (with telemetry)?

EDIT: your later post shows an image in which it looks like you did!

In that case what problem did you encounter?
```

---
## \#832 Posted by: ervinelin Posted at: 2018-02-14T05:59:17.946Z Reads: 268

```
Easyeda. That's how I made my custom PCBs above
```

---
## \#833 Posted by: Deakbannok Posted at: 2018-02-14T08:15:46.475Z Reads: 281

```
I did a recode on them.

First. Delete all the UART liibrary and install the newest UART VESC6.
Open the Receiver.ino

First you must add
#define SERIALIO Serial

Then next add set serial port next to begin
 
SetSerialPort(&SERIALIO);
SERIALIO.begin(115200);

You can only use one serial port. So if you have declared Serial.begin(); You must disable it by //
```

---
## \#834 Posted by: dg798 Posted at: 2018-02-14T13:51:10.368Z Reads: 277

```
They don’t have a way to wire arduino modules as a diagram type. Not looking for a PCB, I want to see a diagram.
```

---
## \#835 Posted by: Migro Posted at: 2018-02-14T18:07:41.972Z Reads: 290

```
Made half of the reciver just missing the cables with connector for the vesc. 
So made myself at lille box for it. Still got the opportunity to reach the mini usb. 
![image|375x500](upload://9SfmtMEDMLqWUHqoTJF7GjMFHg0.jpg)

Hole for the uart and ppm wires. 
![image|375x500](upload://i17VfmACOnJySzCxAFbtIzlmrLv.jpg)

Can anyone tell me how to calibrate the remote?
```

---
## \#836 Posted by: ervinelin Posted at: 2018-02-14T22:50:53.462Z Reads: 282

```
You mean a schematic like this??

![IMG_20180215_065023|690x347](upload://jmHdpEbV5WEOrUncWYRJxRjgk.jpg)
EasyEda can do that just fine...
```

---
## \#837 Posted by: dg798 Posted at: 2018-02-14T23:33:35.974Z Reads: 271

```
I know but they don’t have a nrf52 module in their components list
```

---
## \#838 Posted by: ervinelin Posted at: 2018-02-15T00:49:12.595Z Reads: 267

```
Draw your own? Find user contributions?
```

---
## \#839 Posted by: dg798 Posted at: 2018-02-15T01:10:21.592Z Reads: 271

```
i also want to know how to figure out the pinning for the nrf52 as its not the same pinout as the nano
```

---
## \#840 Posted by: chinzw Posted at: 2018-02-15T01:48:38.994Z Reads: 265

```
You can look at the bluefruit api for the pinouts probably
```

---
## \#841 Posted by: dg798 Posted at: 2018-02-15T01:52:14.798Z Reads: 263

```
i did and here is what i came up with:https://drive.google.com/file/d/0B-o4mV1-aV4jV1BtUHJnZGsxb2lBby1zY0o0R2VIT3RmYU93/view?usp=sharing

i will probably have to update the code though right?
```

---
## \#842 Posted by: chinzw Posted at: 2018-02-15T01:53:37.531Z Reads: 262

```
dont know, i cant see that
```

---
## \#843 Posted by: dg798 Posted at: 2018-02-15T01:55:29.921Z Reads: 265

```
basically all i did was wire the oled and hall sensor to the same analog pins as the nano and the one wire from the micro switch to P0.15 instead of D4 becasue the nrf52 doesnt have the D4.
```

---
## \#844 Posted by: dg798 Posted at: 2018-02-15T02:00:33.681Z Reads: 263

```
would i have to edit the code for the nrf24 module or do i keep it for communication becasue its built in so im not connecting an nrf24 to any pins?
```

---
## \#845 Posted by: chinzw Posted at: 2018-02-15T02:12:17.691Z Reads: 256

```
ill have more info when i actually start building these, until then you're on your own im afraid
```

---
## \#846 Posted by: dg798 Posted at: 2018-02-15T02:26:50.167Z Reads: 257

```
Alrighty then good luck
```

---
## \#847 Posted by: Achmed20 Posted at: 2018-02-15T02:30:49.359Z Reads: 271

```
did anyone have any luck finding 3V hall sensors?
so far i only found the [A1120](https://www.allegromicro.com/de-DE/Products/Magnetic-Digital-Position-Sensor-ICs/Hall-Effect-Unipolar-Switches/A1120-1-2-5.aspx). 

just asking cause i was planing to use the [328p feather](https://www.adafruit.com/product/3458) which brings pretty much everything with it (charger, battery connector and voltageregulater) but the TO-92 only starts working at 3.7V which wont be enough with a lipo
```

---
## \#848 Posted by: dg798 Posted at: 2018-02-15T02:31:54.596Z Reads: 270

```
The DRV ones from TI
```

---
## \#849 Posted by: dg798 Posted at: 2018-02-15T02:35:26.110Z Reads: 281

```
Forgot the full name, it’s a long product number
```

---
## \#850 Posted by: Achmed20 Posted at: 2018-02-15T02:36:54.535Z Reads: 291

```
those seem to be SMD only!?

http://www.ti.com/graphics/folders/partimages/DRV5053.jpg
```

---
## \#851 Posted by: chinzw Posted at: 2018-02-15T02:41:36.517Z Reads: 285

```
There's a ton. Here's the ones im using:

https://www.digikey.ca/product-detail/en/texas-instruments/DRV5053OAQLPGM/296-40059-1-ND/5177936
```

---
## \#852 Posted by: dg798 Posted at: 2018-02-15T02:43:46.134Z Reads: 286

```
@chinzw has the one i was talking about.
```

---
## \#853 Posted by: ervinelin Posted at: 2018-02-15T04:29:39.961Z Reads: 300

```
I edited the code to allow me to easily swap between decks.

![IMG20180215113931|281x500](upload://z3a20ldzjMjQxtR8SqkZPAGuV5S.jpg)

Update: I finally managed to get telemetry to work after fiddling for a long time... Just need to make sure to use the new rollinggecko library and make sure my edited code worked.
```

---
## \#854 Posted by: Deakbannok Posted at: 2018-02-15T12:16:36.716Z Reads: 287

```
I am using the newest VESC Tools.
Been play around with the PPM settings and Pulselength.
The throttle cannot surpass the below 46 and 202 or the ESC will cut off. I am not sure why
```

---
## \#855 Posted by: Achmed20 Posted at: 2018-02-15T12:40:26.069Z Reads: 290

```
[quote="chinzw, post:851, topic:28543"]
There’s a ton. Here’s the ones im using:
[/quote]
well here in germany / europe that seems to be different.
i found a few 2.4V switch types, but liniar analog ones... thats a whole different story. shipping costs me whopping 20€ from the digikey (and other sites) :unamused:

well i orderd them now, but if anyone knows a good site in europe / germany where you can find this type of stuff without paying a fortune on shipping costs, i'd be grateful
```

---
## \#856 Posted by: Krazyaklo Posted at: 2018-02-15T14:41:39.327Z Reads: 293

```
Hello folks, is there a way to use this reciever and wire it to something like an rc car esc to test its function with a the remote?also can it be made useable on something like a Chinese hub motor board? What would the process be? Much appreciated in advanced.  ![20180215_093822|281x500](upload://hwjTLJx9YHvD93KLKz1DmjXhaQE.jpg)
```

---
## \#857 Posted by: monter_man Posted at: 2018-02-15T15:08:02.545Z Reads: 274

```
I bought those SMD from Texas instruments,  solder tiny wires to legs and just fill up the gap with epoxy glue below, as the legs breaks easily.  Otherwise, detection is very good even from a bit far.
```

---
## \#858 Posted by: monter_man Posted at: 2018-02-15T15:11:43.123Z Reads: 271

```
BTW could you share your code? For feather.
I have the feather proto m0, but could not make it work because the libraries are all different, and I'm not good with arduino.  It would be great if you could do a quick error up of what libraries to use and your code.   Thanks!
```

---
## \#859 Posted by: ervinelin Posted at: 2018-02-15T17:02:50.058Z Reads: 266

```
If you have a regular rc servo you can wire the ppm signal to test it. Although usually I just test with my board directly...

Chinese escs have their Rx inbuilt, so unless you have some creative hacking it's not going to be possible. Even if you do get the ppm signal in there would be no telemetry data as the telemetry data is dependent on a vesc.
```

---
## \#860 Posted by: Achmed20 Posted at: 2018-02-15T17:35:55.301Z Reads: 265

```
i will once all parts have arrived and i got it working. 
still missing the magnets, nrf modules and the hallsensors
```

---
## \#861 Posted by: dg798 Posted at: 2018-02-15T17:53:42.937Z Reads: 286

```
Just get the nrf52 modules from adafruit and then u just need 1 nrf24 module for the receiver.
```

---
## \#862 Posted by: Achmed20 Posted at: 2018-02-15T18:27:11.301Z Reads: 296

```
looks like you have to figure out your problem for yourself :(
i have the feather 328p and its working flawlessly

![20180215_192342|666x499](upload://3nzVgljVekRTr1ZE7KogQrM3vRq.jpg)
```

---
## \#863 Posted by: Achmed20 Posted at: 2018-02-15T18:37:02.936Z Reads: 296

```
are those compatible?
it totaly reads like the nrf52 is bluetooth only
```

---
## \#864 Posted by: Krazyaklo Posted at: 2018-02-15T21:22:07.932Z Reads: 294

```
Ah, alright, thank you for your responce. i was considering the maytech kit which uses an external radio and reciever, but even to i guess it's not worth it.  My idea was to start on that type of board with wome good hub motors then eventually upgrade to dual vescs.  I was hoping to use this firefly remote throughout this all.. Im done building the remote part.  Sad.  Well if anyone has any ideas it would be much appreciated.
```

---
## \#865 Posted by: chinzw Posted at: 2018-02-15T22:44:49.855Z Reads: 291

```
nrf52 is BLE and RF, you can even connect nrf52 to nrf24

https://devzone.nordicsemi.com/f/nordic-q-a/13878/any-advice-for-nrf52832-to-nrf24l01-communication
```

---
## \#866 Posted by: MontPierre Posted at: 2018-02-15T23:39:54.962Z Reads: 302

```
Just FYI enertion is working on new remote ;) hopefully that’s not old news.

https://instagram.com/p/BfKwz6GHJkN/ 

Would anyone know what are they using as a throttle?
```

---
## \#867 Posted by: dg798 Posted at: 2018-02-15T23:42:07.491Z Reads: 298

```
The only problem would be that the pinout is different, but that’s all.
```

---
## \#868 Posted by: moon Posted at: 2018-02-16T00:05:16.515Z Reads: 293

```
Cool, but so many good opensource remotes on the forum too
```

---
## \#869 Posted by: Deakbannok Posted at: 2018-02-16T00:16:26.938Z Reads: 292

```
It calls Potentiometer.
10k will work with Arduino Nano controller. It work flowlessly with this code too. I have not get time to do a 3D knob for it yet.
```

---
## \#870 Posted by: ervinelin Posted at: 2018-02-16T05:35:13.712Z Reads: 286

```
Yes it looks like a pot. I used one in my hacked mini remote with this code.
```

---
## \#871 Posted by: Jc06505n Posted at: 2018-02-16T05:36:49.845Z Reads: 283

```
[Looks like someone beat you to cruise control](https://github.com/deakbannok/Arduino-Nano-Controller/blob/master/README.md) @RollingGecko
```

---
## \#872 Posted by: chinzw Posted at: 2018-02-16T08:17:28.955Z Reads: 283

```
Seems like none of the protos are supported by u8glib.
I tried the M0 and the nrf52, but no luck, i might need to fork your code to make the changes for these platforms.
```

---
## \#873 Posted by: MontPierre Posted at: 2018-02-16T10:26:47.393Z Reads: 287

```
I thought it was potentiometer - I actually bought a joystick myself - same as Xbox has - but they are very chubby :/  - this one above looks very slim and sexy haha :) If someone had a link to it I would be very grateful!
```

---
## \#874 Posted by: SimosMCmuffin Posted at: 2018-02-16T14:03:07.554Z Reads: 301

```
Found the mystery component, it was not a plain potentiometer, trimmer or an encoder, but sort of specialized potentiometer (you can actually see the Bourns Inc logo on the picture too):
![image|200x200](upload://3i6bqg1tFDLJ6KKrR2smaRH1sjC.jpg)
https://www.digikey.fi/product-detail/en/bourns-inc/3382G-1-503G/3382G-1-503GCT-ND/2080240

I looked for it as a detective challenge for myself :grin:

EDIT: It is basically a potentiometer without a shaft, that can freely spin around continuously, although only the angle between 0-330 degrees, will give a resistive output, as the wiper travels around. Between 330-360 degrees it will most likely come to a gap in the resistive surface, which means the output will float in the area.
```

---
## \#875 Posted by: MontPierre Posted at: 2018-02-16T14:13:35.461Z Reads: 281

```

Amazing find! Thanks, man! Looks like they will have a shaft bent at 90 degrees to have it working as a thumb control or trigger style ... Super flat, perfect for slim remote :)
```

---
## \#876 Posted by: Twinsen Posted at: 2018-02-16T15:36:05.696Z Reads: 292

```
If anyone else is looking for cheap 3v3 hall sensors, I bought these. They should be fine.
https://www.aliexpress.com/item/10-pcs-Hall-Element-49E-OH49E-SS49E-Linear-Hall-Switch/1903819684.html

I did some limited testing though.
```

---
## \#877 Posted by: ervinelin Posted at: 2018-02-16T16:42:19.038Z Reads: 305

```
Guys.. I solved the problem of my Rx not booting up and requiring a reset all the time!

Initially I used a 220uF cap like what solidgeek recommended but that didn't work, and I knew it was a 5V noise issue as it doesn't happen when I don't power it via the VESC.

So I put an LC filter on the 5V input (it's something I had lying around from my miniquad flying days) and voila! Problem solved!!!

![ca5646bc-d26f-4be5-939b-c082372491f2|690x387](upload://pHsrvQdMRk0AYvlAR1oxXhFjpmO.jpg)

Super happy now... everything seems to work like it should!
```

---
## \#878 Posted by: Deakbannok Posted at: 2018-02-17T04:52:53.521Z Reads: 289

```
I am new to github have you guys tried my code yet?
```

---
## \#879 Posted by: Jc06505n Posted at: 2018-02-17T13:43:01.312Z Reads: 280

```
Not yet, did you change any coded or just added on? Have you tried making a pull request?
```

---
## \#880 Posted by: Achmed20 Posted at: 2018-02-17T14:24:07.374Z Reads: 286

```
do a pull request!
on the original repo, go to "new pull request" and on the top youll find a link "compare across forks".
ther you should be able to select your fork and create a pull request from that one.
```

---
## \#881 Posted by: Achmed20 Posted at: 2018-02-17T14:29:43.298Z Reads: 304

```
still 3 parts missing. hall sensors, NRF modules and the battery. 
but so far, its a breeze to work with the feather 328p. no extra charger or voltage regulator needed, which leaves room for improvement.

![20180217_151322|375x500](upload://tgGrQRk6DE8qczmFqItz7hEgNsd.jpg)
![20180217_151351|666x499](upload://fcQpTUbRDLuO2BiOPS2a3R52VJj.jpg)

thx alot @solidgeek ! i always wanted to do a arduino project,  but so far, lacked the ideas for one :)
```

---
## \#882 Posted by: Tot_Designs Posted at: 2018-02-17T14:57:46.271Z Reads: 287

```
looks cool!
```

---
## \#883 Posted by: solidgeek Posted at: 2018-02-17T16:45:23.294Z Reads: 296

```
@ervinelin Looking forward to seeing your finished remote!  I love your design, I would like to make one myself at some point :D And nice to know that a LC filter fixes those bad power supplies! 

@Deakbannok I have been having that issue with max PPM too, not sure why it happens either. Would have been nice if you either did a pull request or forked my repository :slight_smile: 

EDIT: Been looking through your repository, and will be implementing some of your changes in the new update, nice work! 

@Achmed20 Look good mate! Nice to know that the Feather 328p can replace most of the electronics! Leaves room for a bigger battery :P
```

---
## \#884 Posted by: chinzw Posted at: 2018-02-17T19:28:10.649Z Reads: 303

```
I started working on porting everything to nrf52 last night. Its a completely different architecture, so most of the code has to change. Since i don't have the time nor need for vesc data and fancy menus, it stripped everything down to the bare minimum.
Redid the ui with arduino gfx (u8glib doesnt work on nrf52). Now im starting to work on the radio side of things.

![IMG_20180217_111722|666x500](upload://4FTrYvo0gzPdnhLJkAxxRfSfaXD.jpg)
```

---
## \#885 Posted by: Achmed20 Posted at: 2018-02-17T20:17:04.388Z Reads: 289

```
i'll receive my nrf52 next week. at some point i will probably join you on your quest ;)
but first i want to finisha few other htings
```

---
## \#886 Posted by: dg798 Posted at: 2018-02-18T00:07:13.672Z Reads: 279

```
If I was to use just ppm, would I need to change code?
```

---
## \#887 Posted by: chinzw Posted at: 2018-02-18T01:07:57.825Z Reads: 275

```
On the nrf52 yes
```

---
## \#888 Posted by: dg798 Posted at: 2018-02-18T01:08:54.201Z Reads: 286

```
do you know what to change?
```

---
## \#889 Posted by: Achmed20 Posted at: 2018-02-18T01:13:45.493Z Reads: 291

```
pretty m,uch everything ^^
just go with the buylist from solidgeek, his development branch supports "PPM" only mode

@chinzw
did you have a chance to play arround with the switch yet (the kill/cruise control one) ?
the documentation stated somewhere that the Pins dont support "INPUT_PULLUP" which means you have to add resistors manualy to the switches manualy. not sure if this is correct though
```

---
## \#890 Posted by: dg798 Posted at: 2018-02-18T01:15:44.795Z Reads: 276

```
oh ok
10 charc
```

---
## \#891 Posted by: chinzw Posted at: 2018-02-18T03:23:51.023Z Reads: 278

```
Yeah, as far as i can tell there's no pullups, but thats just a resistor to vcc, super simple, or you can reverse the logic too.
I havent yet played with the trigger as i dont really use one anyways.
```

---
## \#892 Posted by: ervinelin Posted at: 2018-02-18T03:39:50.771Z Reads: 297

```
@solidgeek I am almost 100% done with my remote design, already took it out for a test ride and everything worked as it should.

I will upload the STLs to thingiverse and provide a build guide soon (lots of work to do one).

I will also upload the eagle files somewhere for the PCB design.

As for the code I adjusted your original a fair bit to accommodate for my own requirements (second button, deck choices, dead man switch, etc) but I dropped the latest round of changes because I didn't find them necessary for my use (e.g. pipe address generation, Rx settings, etc)

In this case should I do a fork or a pull on GitHub? Sorry I have never contributed anything on GitHub so I have no idea exactly how it works.

Thanks again for the awesome project...
```

---
## \#893 Posted by: ervinelin Posted at: 2018-02-18T09:16:01.864Z Reads: 304

```
Silly me... I thought I had to physically turn the OLED 180 deg to make the remote left hand friendly. Turns out all I needed was a change in the code.

Now my remote is effectively ambidextrous! ![IMG20180218171411|690x388](upload://rSWHAwNy2liwnuGFXBBYopStX5O.jpg)
```

---
## \#894 Posted by: Deakbannok Posted at: 2018-02-18T17:03:31.575Z Reads: 296

```
@solidgeek I am new to github thing so I will do tonight.

I there were alot of changed and not just adding. I will delete and creating the repository again
```

---
## \#895 Posted by: SeeTheBridges Posted at: 2018-02-18T17:07:55.258Z Reads: 286

```
What did you have to change to make it lefty?
```

---
## \#896 Posted by: ervinelin Posted at: 2018-02-18T17:14:50.364Z Reads: 286

```
Just swap one line of the code which deals with the OLED setup one of which is for the rotation... Ug82 something R0 vs R2. Sorry forgot the exact code, not at my PC now...
```

---
## \#897 Posted by: nikoli280 Posted at: 2018-02-18T18:28:05.998Z Reads: 292

```
Hi everyone i am in i tight spot. I can not get further. My remote is finished but there is not signal between the receiver and transmitter. I have talked to Emil (Solidgeek) about it. If you have some advice for me to try please say so.

At the moment i have.

- Checked for short (nothing came up)
- Changed Dupont wires for silicone wire
- Reuploaded the arduino code to both TX and RX

The remote shows Display and i can navigate around the display without problem. So both display, power system, and hall sensor works.
```

---
## \#898 Posted by: wafflejock Posted at: 2018-02-18T23:04:04.661Z Reads: 281

```
Should be able to use the radio library to have it print details about the connections might help for debugging purposed to write out those details to the serial port and copy/paste them here make.
```

---
## \#899 Posted by: solidgeek Posted at: 2018-02-18T23:44:38.168Z Reads: 287

```
@ervinelin Sounds good! Well I think a fork would be best, since your changes probably won't be backward compatible :-)  I am looking forward to seeing your complete build, it got some interesting features! I am a little curious to know what you use the top button for!

@Deakbannok Okay no problem mate, this is also my first time using Github for realz. Looking forward to seeing your fork!

@wafflejock Yeah we tried that, shows everything correctly. I am maybe thinking a defective nrf24 module @nikoli280.
```

---
## \#900 Posted by: ervinelin Posted at: 2018-02-19T00:16:08.420Z Reads: 292

```
@solidgeek remote is completed already, just did a 15km ride last night without much incident. I did have an instance which I couldn't start the board again after stopping on a slope... Not sure what that was need to check.

As for the top button, it's meant the mode switch. Meant to swap between displays (instead of the display rotating every 4 secs). Also used to access the menu. The front one acts only as a dead man switch.

@nikoli280 make sure pipe addresses are correct on both ends. Make sure in your code the radio is set to the correct pins (9 & 10 for me, not 7 & 8).  Lastly try hitting the reset button on the Rx after it powers up, see if that works.
```

---
## \#901 Posted by: Scoo_B_SK8 Posted at: 2018-02-19T03:43:14.375Z Reads: 284

```
I Just got the 100th like on thingiverse for this project!

props  @solidgeek


EDIT: Whoa...Where did all  the balloons and streamers come from?:stuck_out_tongue_winking_eye:
```

---
## \#902 Posted by: Boesila Posted at: 2018-02-19T07:47:58.324Z Reads: 287

```
Hey guys, 

my remote is finish jet and on a small test ride it was great! :star_struck: THANKS!
But I really miss the function to change the driving direction (forward / backwards), like it is possible with the nunchuck remote from BV. Do you @solidgeek  think it is possible to add this feature? For example if the motor(s) stands still you hit two times or three times the dead man switch and than the motor(s) spins in the reverse direction when you push the throttle forwards. 
I know you can choose different modes in the VESC tool ( "current" vs. "current with reverse"). But I don't like that the motors spins backwards when you just want to break in the "current with reverse" mode.

Hopefully you understand what I'm trying to explain :thinking:

Have a nice ride!:sunglasses:
```

---
## \#903 Posted by: Achmed20 Posted at: 2018-02-19T16:55:16.075Z Reads: 280

```
that should be UART controls which he will be working on sooner or later. at least its on his roadmap :)
```

---
## \#904 Posted by: Scoo_B_SK8 Posted at: 2018-02-19T18:08:21.461Z Reads: 282

```
@nikoli280 I second @solidgeek's diagnosis of bad nrf24 if you've already check pipe #'s and wiring as @ervinelin mentioned.

Side note: with the popularity of this remote I would definitely suggest using a unique "pipe #" so when you go to "meet ups"  or "events" like http://www.electric-skateboard.builders/t/2018-electric-skateboard-convention-esk8con2018/18866/1 ,  you won't have 20+ people controlling your board.
```

---
## \#905 Posted by: nikoli280 Posted at: 2018-02-19T18:23:48.301Z Reads: 295

```
I have tested with no better result. I have talked to Solidgeek and he will look at it. Lucky we live in the same small country.
```

---
## \#906 Posted by: Migro Posted at: 2018-02-19T18:35:48.826Z Reads: 312

```
Could be the nrf24 module as you can see in my batch of modules one is odd. 
This could just be that the third is using another chip or something that dosent require the other compoments. Havent tested the odd one yet. 
![image|375x500](upload://mFXnThcphz4axVEzPEezleK8hvm.jpg)
```

---
## \#907 Posted by: Scoo_B_SK8 Posted at: 2018-02-19T18:59:06.545Z Reads: 292

```
The arduino nano DOES NOT have a good 3v source for running nrf24.
```

---
## \#908 Posted by: bsancken Posted at: 2018-02-19T19:22:39.618Z Reads: 295

```
Hey is there a definite list of everything that needs to be ordered? I started looking at the top of the thread and found the [linked sheets doc](https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit#gid=0), but I didn't know if this has been updated as better components were found or not.

I'm planning on looking at building @ervinelin version but I'd assume that they are mostly the same parts. Just looking for your know working config. I can modify the code to suit my additions.

Thanks
Bsancken
```

---
## \#909 Posted by: Surfer Posted at: 2018-02-19T19:38:20.751Z Reads: 288

```
Good point! Already have the Arduino, there is a solution for that?
Thanks in advance
```

---
## \#910 Posted by: chinzw Posted at: 2018-02-19T19:42:03.363Z Reads: 286

```
A capacitor between vcc and gnd will smooth out the crappy power
```

---
## \#911 Posted by: Surfer Posted at: 2018-02-19T19:45:22.220Z Reads: 288

```
Thanks for the quick reply, because my lack of knowledge, capacitor is a electrolytic condensator? Mind you to give the values of this component, I will try to find it.
```

---
## \#912 Posted by: chinzw Posted at: 2018-02-19T19:46:46.292Z Reads: 280

```
Just use a 220uf cap and you should be golden.
```

---
## \#913 Posted by: solidgeek Posted at: 2018-02-19T22:57:17.217Z Reads: 299

```
@ervinelin Awesome! Sounds weird, did you check your VESCs error log? 

@Scoo_B_SK8 Thanks mate :P 

@Boesila I have been looking into the possibility to add a reverse function, however, I am not yet sure how to implement it. It will not be added to the next release :-)   

@Scoo_B_SK8 I have added a function to generate a unique address for each remote in the newest beta-build. Will be releasing the code soon! 

@bsancken I believe the sheets document is updated with the newest parts.

@Surfer As long as you add a capacitor or use the Arduino Nano I recommend (with builtin 3.3V voltage regulator) it should not be a problem
```

---
## \#914 Posted by: moon Posted at: 2018-02-19T23:14:28.318Z Reads: 283

```
I think Nano V3 ATmega328 is out of stock on aliexpress
```

---
## \#915 Posted by: Jc06505n Posted at: 2018-02-19T23:37:09.822Z Reads: 288

```
I thought the remote can go reverse simply by letting go and triggering back via VESC-TOOL settings. Unless you mean a reverse function similar to pressing a button like the Winning V2?
```

---
## \#916 Posted by: chinzw Posted at: 2018-02-19T23:45:57.749Z Reads: 281

```
@solidgeek any chance of getting source files for the remote case? I'm about to start remodeling it, i rather i didn't have to.
```

---
## \#917 Posted by: Jamy Posted at: 2018-02-20T01:10:20.473Z Reads: 272

```
Bleh, I've been trying to make this amazing thing for like months. But I can't solder for crap :P
```

---
## \#918 Posted by: moon Posted at: 2018-02-20T01:14:49.234Z Reads: 273

```
Join the club, but all it takes is correct techniques and certain equipment from the youtube videos I have seen
```

---
## \#919 Posted by: chinzw Posted at: 2018-02-20T21:34:20.075Z Reads: 270

```
Just a good soldering iron, lead solder and flux, thats it
```

---
## \#920 Posted by: Scoo_B_SK8 Posted at: 2018-02-20T21:40:26.305Z Reads: 271

```
the right "tip" makes all difference
```

---
## \#921 Posted by: Jamy Posted at: 2018-02-20T21:51:40.947Z Reads: 268

```
I think I need better wires, and a heat controlled soldering iron. But I'm not able to get a new soldering iron atm
```

---
## \#922 Posted by: Clonkex Posted at: 2018-02-20T21:59:29.416Z Reads: 271

```
Honestly I've tried using flux and it's never made it any easier. Plain old 60/40 rosin core solder and a 350-400° iron is all you need in most cases.
```

---
## \#923 Posted by: chinzw Posted at: 2018-02-20T22:33:45.250Z Reads: 270

```
Depends on the flux you're usin, rosin core is filled with rosin flux, that's why it solders nicely.
```

---
## \#924 Posted by: Achmed20 Posted at: 2018-02-20T22:35:32.674Z Reads: 263

```
in my epxerience its neither the tip, nor the sodler nor flux, 
its usualy just a cheap ass soldering iron with way to low Watts.
```

---
## \#925 Posted by: Clonkex Posted at: 2018-02-20T22:48:38.814Z Reads: 276

```
[quote="chinzw, post:923, topic:28543"]
rosin core is filled with rosin flux, that’s why it solders nicely
[/quote]

I know :)

10char
```

---
## \#926 Posted by: Surfer Posted at: 2018-02-21T11:05:34.226Z Reads: 288

```
Jamy if you want, as soon I finish mine and it works, I can make one for you.
For the old times!
```

---
## \#928 Posted by: Migro Posted at: 2018-02-21T17:06:02.971Z Reads: 300

```
Okay im a little unsure about my vesc and the reciever wiring so is this correct? 
![Reciever|688x499](upload://ly2HYTisxuYhN8jfsHfIVTHDw3l.jpg)
```

---
## \#930 Posted by: ervinelin Posted at: 2018-02-21T17:37:30.087Z Reads: 295

```
Some updates on my progress...

https://www.thingiverse.com/thing:2800544 - STLs have been uploaded!
https://youtu.be/gQl7mLMAiAs - I also uploaded a quick youtube video showing the functions of the remote

Give me some time to fix the eagle files...

As for the troubleshooting of the remote here's what I've been trying:
1. I went from a 5x5mm magnet to a 5x8mm magnet, this effectively removed the weird deadzone I was having in my remote
2. Not all LC filters are the same, I tried another larger LC filter and it didn't work for me, not sure why
3. I need to check why the remote seems to be self draining its battery, I might have accidentally left it on but I need to double check.
3. I just updated my dual motor loaded truncated tesseract, it rides awesome with the new remote!
```

---
## \#931 Posted by: ervinelin Posted at: 2018-02-21T17:38:15.064Z Reads: 272

```
I get 5v and ground from the PPM line, tx and rx from the UART.

Although where you draw 5v shouldn't matter...
```

---
## \#932 Posted by: Migro Posted at: 2018-02-21T17:47:20.239Z Reads: 273

```
Did you just cut the ppm off or did you solder on some extra wires?
```

---
## \#933 Posted by: ervinelin Posted at: 2018-02-21T17:52:23.416Z Reads: 278

```
Why would I cut the PPM off? 

PPM, 5v and ground in one servo wire goes to the receiver.

If you are asking about the connection to the receiver, I have on receiver which has a servo lead soldered to it, another has pins, either way it can be easily disconnected from the VESC PPM wire.
```

---
## \#934 Posted by: Migro Posted at: 2018-02-21T17:59:26.264Z Reads: 272

```
Genius! 
Forgot i had those. And they dont come out?
```

---
## \#935 Posted by: Migro Posted at: 2018-02-21T18:38:01.815Z Reads: 277

```
I connected the reciever to the vesc and powered on the board. But for some reason the vesc didnt turn on. The bec or ppm cables or what they are called got alittle hot. I turned the board off and connected the old remote and it works fine. 
Any ideas?
```

---
## \#936 Posted by: ervinelin Posted at: 2018-02-21T22:57:01.312Z Reads: 283

```
Wires got hot??? Likely you connected something wrongly. Share a clear picture of your connection. Hopefully you didn't fry anything...
```

---
## \#937 Posted by: Clonkex Posted at: 2018-02-21T22:59:11.442Z Reads: 283

```
If wires are getting hot, something is very wrong!
```

---
## \#938 Posted by: Migro Posted at: 2018-02-22T07:28:00.560Z Reads: 292

```
I dont really have a picture at the moment, will take one later. 
Im pretty sure i did it like this: 
![image|304x273](upload://mKxoILq8LnJb81u6fxtCJUnxRTx.png)

But im going to double check when i get home.
```

---
## \#939 Posted by: dg798 Posted at: 2018-02-22T12:38:40.307Z Reads: 278

```
Are u using the regular arduino nano?
```

---
## \#940 Posted by: Migro Posted at: 2018-02-22T14:14:57.082Z Reads: 275

```
I guess yea?
```

---
## \#941 Posted by: ZackoryCramer Posted at: 2018-02-23T05:40:37.865Z Reads: 285

```
Hey there! :ghost::smiley:
I know there is a RPM counter in the Vesc bldc measure struct but it doesn't seems to be very precise and accurate especially with the magnets pole count. I was thinking maybe we can use the voltage going into the motor and the kv, gear, wheels dia. to calculate the speed. Is this something you guys are aware of? What do you think of my idea. :lying_face:
```

---
## \#942 Posted by: Migro Posted at: 2018-02-23T07:39:12.294Z Reads: 307

```
![PPM billede|552x500](upload://7k5LKpHnnXVv7rgQXzERtraHdEy.png)![NRF24|666x500](upload://pcigKTkHydFHBEJ6dx9WyoMIjJY.jpg)![NRF24 til arduino|666x500](upload://b3MN31klpp9uRXoDEsKAmFbOsDn.jpg)

Sorry for the late pictures, but my main computer decided to stop working so had to fix that. 
I cant seem to find whats wrong. with the reciever. And could'nt get it out from my little box. But i tried to show the wires and so with these pictures.
```

---
## \#943 Posted by: ervinelin Posted at: 2018-02-23T09:02:49.920Z Reads: 285

```
Got a feeling you mixed up the connection between the Arduino and vesc because the wires are the same colour.. so your ppm connected to v+
```

---
## \#944 Posted by: Migro Posted at: 2018-02-23T09:23:01.740Z Reads: 282

```
The v+ is red and the ppm is orange ish. But im going to check anyways :slight_smile:
```

---
## \#945 Posted by: Scoo_B_SK8 Posted at: 2018-02-23T13:19:16.538Z Reads: 287

```
be sure to use some kind of flux, as it draws solder and will give you better looking/functioning solder points

id' try again on
nano - D12
nrf - 5v,CSN

also i dont see a CAP present since using arduino nano.
```

---
## \#946 Posted by: Migro Posted at: 2018-02-24T15:16:37.689Z Reads: 276

```
What kind of cap?
Most of them is soldered on the other side tho. But worth a try :slight_smile:
```

---
## \#947 Posted by: solidgeek Posted at: 2018-02-24T20:40:21.531Z Reads: 275

```
Well you could use motor KV, gearing etc. to calculate the speed, however, the speed would be a theoretical speed and not the actual speed. This would only work if no load is applied I believe. Actually, the eRPM counter is more than enough and does the job very precise (at least the VESC 6) :slight_smile:
```

---
## \#948 Posted by: solidgeek Posted at: 2018-02-24T20:46:17.820Z Reads: 277

```
@Deakbannok I have lately been thinking about the issue regarding acceleration turning of while giving max or minimum throttle. At the moment the receiver uses standard PWM signal to generate the throttle signale, however shouldn't the signal be a PPM signal? I remember something about a "Servo" library which are able to generate a true PPM signal. I will give this a try, and return my findings :slight_smile:
```

---
## \#949 Posted by: Clonkex Posted at: 2018-02-24T23:12:57.360Z Reads: 300

```
As far as I'm aware, receiver signal is actually PWM. I don't know why people call it PPM. The position is not modulated, only the width. The correct way to generate a receiver signal is something like this (I made my own Arduino/NRF controller/receiver setup some time ago and this is part of my code):

    #include <Servo.h>

    Servo esc;

    void setup() {
      esc.attach(9);
    }

    void loop() {
      receiveFromController();
      int val = map(throttle, 0, 1023, 900, 2100);
      esc.writeMicroseconds(val);
    }

This post is quite useful (and I relied on it heavily when designing some code for @MysticalDork to control some LED headlights from a receiver signal): https://ryanboland.com/blog/reading-rc-receiver-values/
```

---
## \#950 Posted by: Deakbannok Posted at: 2018-02-25T03:58:43.715Z Reads: 284

```
Is 180 degree but you have to compromising the negative output numbers  min/max of Hall sensor. I am not super confident if that is right. But no worry I have fixed and added adjustable options to your code awhile ago.
 You will see it soon
Right now I am looking on this glitchy RF24 code. Try to understand the limitation and how this thing works.

I am new to this program stuffs so it will take awhile for me to catch up.
My work is piling up in the office so I hardly get time to continue working on your code except the weekend. I took a week off from work to Spain last week and tested there. Had a good running so far.. but here are a few safety concerns i have found and added to the code.
I will try to push out as soon as i have tested myself that everything is working correct before let the public try it out
```

---
## \#951 Posted by: ju_mpe_r Posted at: 2018-02-26T12:34:04.510Z Reads: 284

```
[quote="ervinelin, post:930, topic:28543"]
I went from a 5x5mm magnet to a 5x8mm magnet, this effectively removed the weird deadzone I was having in my remote
[/quote]

Hi, Ervinelin!
What exactly kind of magnet do you use? Like this one?
aliexpress.com/item/50pcs-8mmx5mm-Strong-Round-Cylinder-Magnets-8x5-mm-Rare-Earth-Neodymium-N52-Permanent-Magnet-Powerful-Magnet/32789112260.html 
I'm asking because link in your BOM is on 5x5mm magnet.
```

---
## \#952 Posted by: ervinelin Posted at: 2018-02-26T13:17:58.075Z Reads: 291

```
I ordered this, U-JOVAN 20pcs N35 5 x 8 mm Mini Strong Round Cylinder Neodymium Magnets Disc Rare Earth Manget 5*8mm
http://s.aliexpress.com/7vAVRbQN?fromSns=Gmail 
(from AliExpress Android) but it's not here yet.

In the meanwhile I stacked my 5x5 with 3pcs of 1mm magnets to get 5x8mm.
```

---
## \#953 Posted by: Zyb Posted at: 2018-02-26T13:54:19.551Z Reads: 286

```
is it possible to build yours without the custom pcb? good job btw
```

---
## \#954 Posted by: ervinelin Posted at: 2018-02-26T15:43:45.723Z Reads: 295

```
I think so, might be a little tricky keeping everything together but I suppose it should be doable.
```

---
## \#955 Posted by: ervinelin Posted at: 2018-02-26T16:16:12.386Z Reads: 301

```
I forked SolidGeek's Github page, all available files for my trigger style remote are now available including the PCB files (I believe you can order it yourself from EasyEDA with the links).

https://github.com/ModMiniMan/nRF24-Esk8-Remote
```

---
## \#956 Posted by: Zyb Posted at: 2018-02-26T18:31:06.061Z Reads: 297

```
as soon as i confirm my remote is working im gonna try your version too. pcbs cost $12 + shipping 
thanks for the contribution i feel like trigger style is better for me because original case is somewhat ucomfortable for small hands. holding down the trigger and braking at the same time is somewhat difficult
```

---
## \#957 Posted by: Poselings1981 Posted at: 2018-02-26T18:40:08.561Z Reads: 289

```
come back with updates when you would have some, i'm pretty interested. 
As well interested in [buying steroids online](https://www.athletespharmacy.to).  Any update would be much appreciated.
```

---
## \#958 Posted by: Boesila Posted at: 2018-02-27T10:23:27.933Z Reads: 322

```
Hi guys,

another feature requeset... 
I like do switch on / off the lights of my board with the help of this remote. My idea was to add an extra point in the setting menu, where you can select light on or off. I tried to implement this in the code from @solidgeek but I'm an absolutely newbie in arduino programming. So I didn't master it. 

_At the **transmitter** I added / changed this:_

**1.**
struct settings {
  byte triggerMode;
  ...  
  **int lightValue;**
};


**2.** 
const byte numOfSettings = 12;

String settingPages[numOfSettings][2] = {
  {"Trigger",         ""},
  ...
  **{"Light",  		  ""}**
};

**3.**
int settingRules[numOfSettings][3] {
  {0, 0, 3}, // 0 Killswitch, 1 cruise & 2 data toggle
  ...
 **{1, 0, 1}, // On or Off**
};

**3.**
int getSettingValue(int index) {
  int value;
  switch (index) {
    case 0: value = remoteSettings.triggerMode;     break;
   ...
	**case 11: value = remoteSettings.lightValue;  	break;**

**4.**
void setSettingValue(int index, int value) {
  switch (index) {
    case 0: remoteSettings.triggerMode = value;     break;
    ...
	**case 11: remoteSettings.lightValue = value; 	break;**
  }

**5.**
void transmitToVesc() {
  // Transmit once every 50 millisecond
  if (millis() - lastTransmission >= 50) {
lastTransmission = millis();    
    radio.write(&lightValue, sizeof(lightValue));
    boolean sendSuccess = false;
    // Transmit the speed value (0-255).
    sendSuccess = radio.write(&throttle, sizeof(throttle));
    **radio.write(&lightValue, sizeof(lightValue));**...



*And at the **receiver** I added / changed this:*

**1.**
int motorSpeed = 127;
int timeoutMax = 500;
int speedPin = 5;
**int lightPin = 7;**
**int lightValue;**

**2.**
pinMode(speedPin, OUTPUT);
  analogWrite(speedPin, motorSpeed);
  **pinMode(lightPin, OUTPUT);**

**3.**
void loop() {
  ...
   getVescData();
  // If transmission is available
  if (radio.available())
  {
...
**radio.read(&lightValue, sizeof(lightValue));**
**if (lightValue==1){**
**digitalWrite(lightPin, HIGH);**
**}**
**else {**
**digitalWrite(lightPin, LOW);**
**}**...



Compiling and upload to the arduinos works. However this code does not work in a proper way, unfortunately. I guess I made something wrong because the transmission of lightValue does not work. Could some please help me? I guess it is an easy task but I just to inexperienced. 

THX in advance
```

---
## \#959 Posted by: Clonkex Posted at: 2018-02-27T10:59:32.272Z Reads: 272

```
Try using the `</>` button so your code is actually readable ;)
```

---
## \#960 Posted by: Boesila Posted at: 2018-02-27T13:01:32.541Z Reads: 308

```
Okay, here is the full code in the right format: 

**TRANSMITTER:**

    #include <U8g2lib.h>
    #include <Wire.h>
    #include <SPI.h>
    #include <EEPROM.h>
    #include "RF24.h"
    #include "VescUart.h"

    // #define DEBUG

    #ifdef DEBUG
      #define DEBUG_PRINT(x)  Serial.println (x)
      #include "printf.h"
    #else
      #define DEBUG_PRINT(x)
    #endif

    int lightValue;

    // Defining the type of display used (128x32)
    U8G2_SSD1306_128X32_UNIVISION_1_HW_I2C u8g2(U8G2_R0, U8X8_PIN_NONE);

    static unsigned char logo_bits[] = { 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x7e, 0x00, 0x80, 0x3c,     0x01, 0xe0, 0x00, 0x07, 0x70, 0x18, 0x0e, 0x30, 0x18, 0x0c, 0x98, 0x99, 0x19, 0x80, 0xff, 0x01, 0x04, 0xc3, 0x20, 0x0c, 0x99, 0x30, 0xec, 0xa5, 0x37, 0xec, 0xa5, 0x37, 0x0c, 0x99, 0x30, 0x04, 0xc3, 0x20, 0x80, 0xff, 0x01, 0x98, 0x99, 0x19, 0x30, 0x18, 0x0c, 0x70, 0x18, 0x0e, 0xe0, 0x00, 0x07, 0x80, 0x3c, 0x01, 0x00, 0x7e,     0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00 };

    static unsigned char signal_transmitting_bits[] = {
      0x18, 0x00, 0x0c, 0x00, 0xc6, 0x00, 0x66, 0x00, 0x23, 0x06, 0x33, 0x0f,
      0x33, 0x0f, 0x23, 0x06, 0x66, 0x00, 0xc6, 0x00, 0x0c, 0x00, 0x18, 0x00
    };

    static unsigned char signal_connected_bits[] = {
      0x18, 0x00, 0x0c, 0x00, 0xc6, 0x00, 0x66, 0x00, 0x23, 0x06, 0x33, 0x09,
      0x33, 0x09, 0x23, 0x06, 0x66, 0x00, 0xc6, 0x00, 0x0c, 0x00, 0x18, 0x00
    };

    static unsigned char signal_noconnection_bits[] = {
     0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x06, 0x00, 0x09,
      0x00, 0x09, 0x00, 0x06, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00
    };

    // Defining struct to hold UART data.
    struct vescValues {
      float ampHours;
      float inpVoltage;
      long rpm;
      long tachometerAbs;
    };

    // Defining struct to hold stats 
    struct stats {
      float maxSpeed;
      long maxRpm;
      float minVoltage;
      float maxVoltage;
    };

    // Defining struct to hold setting values while remote is turned on.
    struct settings {
      byte triggerMode;
      byte batteryType;
      byte batteryCells;
      byte motorPoles;
      byte motorPulley;
      byte wheelPulley;
      byte wheelDiameter;
      bool useUart;
      int minHallValue;
      int centerHallValue;
      int maxHallValue;
      int lightValue;
    };

    // Defining variables for speed and distance calculation
    float gearRatio;
    float ratioRpmSpeed;
    float ratioPulseDistance;

    byte currentSetting = 0;
    const byte numOfSettings = 12;

    String settingPages[numOfSettings][2] = {
      {"Trigger",         ""},
      {"Battery type",    ""},
      {"Battery cells",   "S"},
      {"Motor poles",     ""},
      {"Motor pulley",    "T"},
      {"Wheel pulley",    "T"},
      {"Wheel diameter",  "mm"},
      {"UART data",       ""},
      {"Throttle min",    ""},
      {"Throttle center", ""},
      {"Throttle max",    ""},
      {"Light",           ""}
    };

    // Setting rules format: default, min, max.
    int settingRules[numOfSettings][3] {
      {0, 0, 3}, // 0 Killswitch, 1 cruise & 2 data toggle
      {0, 0, 1}, // 0 Li-ion & 1 LiPo
      {10, 0, 12},
      {14, 0, 250},
      {15, 0, 250},
      {40, 0, 250},
      {83, 0, 250},
      {1, 0, 1}, // Yes or no
      {0, 0, 1023},
      {512, 0, 1023},
      {1023, 0, 1023},
      {1, 0, 1} // on or off
    };

    struct vescValues data;
    struct settings remoteSettings;

    // Pin defination
    const byte triggerPin = 4;
    const int chargeMeasurePin = A1;
    const int batteryMeasurePin = A2;
    const int hallSensorPin = A3;

    // Battery monitering
    const float minVoltage = 3.2;
    const float maxVoltage = 4.1;
    const float refVoltage = 5.0; // Set to 4.5V if you are testing connected to USB, otherwise 5V (or the supply         voltage)

    // Defining variables for Hall Effect throttle.
    short hallMeasurement, throttle;
    byte hallCenterMargin = 4;

    // Defining variables for NRF24 communication
    bool connected = false;
    short failCount;
    const uint64_t pipe = 0xE8E8F0F0E1LL; // If you change the pipe, you will need to update it on the receiver         to.
    unsigned long lastTransmission;

    // Defining variables for OLED display
    char displayBuffer[20];
    String displayString;
    short displayData = 0;
    unsigned long lastSignalBlink;
    unsigned long lastDataRotation;

    // Instantiating RF24 object for NRF24 communication
    RF24 radio(9, 10);

    // Defining variables for Settings menu
    bool changeSettings = false;
    bool changeSelectedSetting = false;

    bool settingsLoopFlag = false;
    bool settingsChangeFlag = false;
    bool settingsChangeValueFlag = false;


    void setup() {
      // setDefaultEEPROMSettings(); // Call this function if you want to reset settings
  
      #ifdef DEBUG
        Serial.begin(9600);
      #endif
  
      loadEEPROMSettings();

      pinMode(triggerPin, INPUT_PULLUP);
      pinMode(hallSensorPin, INPUT);
      pinMode(batteryMeasurePin, INPUT);

      u8g2.begin();

      drawStartScreen();

      if (triggerActive()) {
        changeSettings = true;
        drawTitleScreen("Remote Settings");
      }

      // Start radio communication
      radio.begin();
      radio.setPALevel(RF24_PA_MAX);
      radio.enableAckPayload();
      radio.enableDynamicPayloads();
      radio.openWritingPipe(pipe);

      #ifdef DEBUG
        printf_begin();
        radio.printDetails();
      #endif
    }

    void loop() {
  
      calculateThrottlePosition();
    
      if (changeSettings == true) {
            // Use throttle and trigger to change settings
        controlSettingsMenu();
      }
      else
      {
        // Use throttle and trigger to drive motors
        if (triggerActive())
        {
          throttle = throttle;
        }
        else
        {
          // 127 is the middle position - no throttle and no brake/reverse
          throttle = 127;
        }
        // Transmit to receiver
        transmitToVesc();
      }

      // Call function to update display and LED
      updateMainDisplay();
    }

    void controlSettingsMenu() {
      if (triggerActive()) {
        if (settingsChangeFlag == false) {

          // Save settings to EEPROM
          if (changeSelectedSetting == true) {
            updateEEPROMSettings();
          }

          changeSelectedSetting = !changeSelectedSetting;
          settingsChangeFlag = true;
        }
      } else {
        settingsChangeFlag = false;
      }

      if (hallMeasurement >= (remoteSettings.maxHallValue - 150) && settingsLoopFlag == false) {
        // Up
        if (changeSelectedSetting == true) {
          int val = getSettingValue(currentSetting) + 1;

          if (inRange(val, settingRules[currentSetting][1], settingRules[currentSetting][2])) {
            setSettingValue(currentSetting, val);
            settingsLoopFlag = true;
          }
        } else {
          if (currentSetting != 0) {
            currentSetting--;
            settingsLoopFlag = true;
          }
        }
      }
          else if (hallMeasurement <= (remoteSettings.minHallValue + 150) && settingsLoopFlag == false) {
        // Down
        if (changeSelectedSetting == true) {
          int val = getSettingValue(currentSetting) - 1;

          if (inRange(val, settingRules[currentSetting][1], settingRules[currentSetting][2])) {
            setSettingValue(currentSetting, val);
            settingsLoopFlag = true;
         }
        } else {
          if (currentSetting < (numOfSettings - 1)) {
            currentSetting++;
            settingsLoopFlag = true;
          }
        }
      } else if (inRange(hallMeasurement, remoteSettings.centerHallValue - 50, remoteSettings.centerHallValue + 50)) {
        settingsLoopFlag = false;
      }
    }

    void drawSettingNumber() {
      // Position on OLED
      int x = 2; int y = 10;

      // Draw current setting number box
      u8g2.drawRFrame(x + 102, y - 10, 22, 32, 4);

      // Draw current setting number
      displayString = (String)(currentSetting + 1);
      displayString.toCharArray(displayBuffer, displayString.length() + 1);

      u8g2.setFont(u8g2_font_profont22_tn);
      u8g2.drawStr(x + 108, 22, displayBuffer);
    }

    void drawSettingsMenu() {
      // Position on OLED
      int x = 0; int y = 10;

      // Draw setting title
      displayString = settingPages[currentSetting][0];
      displayString.toCharArray(displayBuffer, displayString.length() + 1);

      u8g2.setFont(u8g2_font_profont12_tr);
      u8g2.drawStr(x, y, displayBuffer);

      int val = getSettingValue(currentSetting);

      displayString = (String)val + "" + settingPages[currentSetting][1];
      displayString.toCharArray(displayBuffer, displayString.length() + 1);
      u8g2.setFont(u8g2_font_10x20_tr  );

      if (changeSelectedSetting == true) {
        u8g2.drawStr(x + 10, y + 20, displayBuffer);
      } else {
        u8g2.drawStr(x, y + 20, displayBuffer);
      }
    }

    void setDefaultEEPROMSettings() {
      for (int i = 0; i < numOfSettings; i++) {
        setSettingValue(i, settingRules[i][0]);
     }

      updateEEPROMSettings();
    }

    void loadEEPROMSettings() {
      // Load settings from EEPROM to custom struct
      EEPROM.get(0, remoteSettings);

      bool rewriteSettings = false;

          // Loop through all settings to check if everything is fine
      for (int i = 0; i < numOfSettings; i++) {
        int val = getSettingValue(i);

        if (! inRange(val, settingRules[i][1], settingRules[i][2])) {
          // Setting is damaged or never written. Rewrite default.
          rewriteSettings = true;
          setSettingValue(i, settingRules[i][0]);
        }
      }

      if (rewriteSettings == true) {
        updateEEPROMSettings();
      } else {
        // Calculate constants
        calculateRatios();
      }
    }

    // Write settings to the EEPROM then exiting settings menu.
    void updateEEPROMSettings() {
      EEPROM.put(0, remoteSettings);
      calculateRatios();
    }

    // Update values used to calculate speed and distance travelled.
    void calculateRatios() {
      gearRatio = (float)remoteSettings.motorPulley / (float)remoteSettings.wheelPulley;

      ratioRpmSpeed = (gearRatio * 60 * (float)remoteSettings.wheelDiameter * 3.14156) /     (((float)remoteSettings.motorPoles / 2) * 1000000); // ERPM to Km/h

      ratioPulseDistance = (gearRatio * (float)remoteSettings.wheelDiameter * 3.14156) /             
    (((float)remoteSettings.motorPoles * 3) * 1000000); // Pulses to km travelled
    }

    // Get settings value by index (usefull when iterating through settings).
    int getSettingValue(int index) {
      int value;
      switch (index) {
        case 0: value = remoteSettings.triggerMode;     break;
        case 1: value = remoteSettings.batteryType;     break;
        case 2: value = remoteSettings.batteryCells;    break;
        case 3: value = remoteSettings.motorPoles;      break;
        case 4: value = remoteSettings.motorPulley;     break;
        case 5: value = remoteSettings.wheelPulley;     break;
        case 6: value = remoteSettings.wheelDiameter;   break;
        case 7: value = remoteSettings.useUart;         break;
        case 8: value = remoteSettings.minHallValue;    break;
        case 9: value = remoteSettings.centerHallValue; break;
        case 10: value = remoteSettings.maxHallValue;   break;
      }
      return value;
    }

    // Set a value of a specific setting by index.
    void setSettingValue(int index, int value) {
      switch (index) {
        case 0: remoteSettings.triggerMode = value;     break;
        case 1: remoteSettings.batteryType = value;     break;
        case 2: remoteSettings.batteryCells = value;    break;
        case 3: remoteSettings.motorPoles = value;      break;
        case 4: remoteSettings.motorPulley = value;     break;
        case 5: remoteSettings.wheelPulley = value;     break;
        case 6: remoteSettings.wheelDiameter = value;   break;
        case 7: remoteSettings.useUart = value;         break;
        case 8: remoteSettings.minHallValue = value;    break;
        case 9: remoteSettings.centerHallValue = value; break;
        case 10: remoteSettings.maxHallValue = value;   break;
      }
    }

    // Check if an integer is within a min and max value
    bool inRange(int val, int minimum, int maximum) {
      return ((minimum <= val) && (val <= maximum));
    }

    // Return true if trigger is activated, false otherwice
    boolean triggerActive() {
      if (digitalRead(triggerPin) == LOW)
        return true;
      else
        return false;
    }

    // Function used to transmit the throttle value, and receive the VESC realtime data.
    void transmitToVesc() {
      // Transmit once every 50 millisecond
      if (millis() - lastTransmission >= 50) {

        lastTransmission = millis();

        boolean sendSuccess = false;
        // Transmit the speed value (0-255).
        sendSuccess = radio.write(&throttle, sizeof(throttle));

        radio.write(&lightValue, sizeof(lightValue));

        // Listen for an acknowledgement reponse (return of VESC data).
        while (radio.isAckPayloadAvailable()) {
          radio.read(&data, sizeof(data));
      
        }

        if (sendSuccess == true)
        {
          // Transmission was a succes
          failCount = 0;
          sendSuccess = false;

          DEBUG_PRINT("Transmission succes");
        } else {
          // Transmission was not a succes
          failCount++;

          DEBUG_PRINT("Failed transmission");
        }

        // If lost more than 5 transmissions, we can assume that connection is lost.
        if (failCount < 5) {
         connected = true;
        } else {
          connected = false;
        }
      }
    }

    void calculateThrottlePosition() {
      // Hall sensor reading can be noisy, lets make an average reading.
      int total = 0;
      for (int i = 0; i < 10; i++) {
        total += analogRead(hallSensorPin);
      }
      hallMeasurement = total / 10;

      DEBUG_PRINT( (String)hallMeasurement );
  
      if (hallMeasurement >= remoteSettings.centerHallValue) {
        throttle = constrain(map(hallMeasurement, remoteSettings.centerHallValue,     remoteSettings.maxHallValue, 127, 255), 127, 255);
      } else {
    throttle = constrain(map(hallMeasurement, remoteSettings.minHallValue, remoteSettings.centerHallValue, 0, 127), 0, 127);
      }

      // removeing center noise
      if (abs(throttle - 127) < hallCenterMargin) {
        throttle = 127;
      }
    }
    
    // Function used to indicate the remotes battery level.
    int batteryLevel() {
      float voltage = batteryVoltage();

      if (voltage <= minVoltage) {
        return 0;
      } else if (voltage >= maxVoltage) {
        return 100;
      } else {
        return (voltage - minVoltage) * 100 / (maxVoltage - minVoltage);
      }
    }

    // Function to calculate and return the remotes battery voltage.
    float batteryVoltage() {
      float batteryVoltage = 0.0;
      int total = 0;

      for (int i = 0; i < 10; i++) {
        total += analogRead(batteryMeasurePin);
      }

      batteryVoltage = (refVoltage / 1024.0) * ((float)total / 10.0);
    
      return batteryVoltage;
    }

    void updateMainDisplay() {

      u8g2.firstPage();
      do {

        if (changeSettings == true) {
          drawSettingsMenu();
          drawSettingNumber();
        } else {
          drawThrottle();
          rawPage();
          drawBatteryLevel();
          drawSignal();
        }

      } while ( u8g2.nextPage() );
    }

    void drawStartScreen() {
      u8g2.firstPage();
      do {
        u8g2.drawXBM( 4, 4, 24, 24, logo_bits);

        displayString = "Esk8 remote";
        displayString.toCharArray(displayBuffer, 12);
        u8g2.setFont(u8g2_font_helvR10_tr  );
        u8g2.drawStr(34, 22, displayBuffer);
      } while ( u8g2.nextPage() );
      delay(1500);
    }

    void drawTitleScreen(String title) {
      u8g2.firstPage();
      do {
        title.toCharArray(displayBuffer, 20);
        u8g2.setFont(u8g2_font_helvR10_tr  );
        u8g2.drawStr(12, 20, displayBuffer);
      } while ( u8g2.nextPage() );
      delay(1500);
    }

    void drawPage() {
      int decimals;
      float value;
      String suffix;
      String prefix;

      int first, last;

      int x = 0;
      int y = 16;

      // Rotate the realtime data each 4s.
      if ((millis() - lastDataRotation) >= 4000) {

        lastDataRotation = millis();
        displayData++;

        if (displayData > 2) {
          displayData = 0;
        }
      }

      switch (displayData) {
        case 0:
          value = ratioRpmSpeed * data.rpm;
         suffix = "KMH";
         prefix = "SPEED";
          decimals = 1;
          break;
        case 1:
          value = ratioPulseDistance * data.tachometerAbs;
          suffix = "KM";
          prefix = "DISTANCE";
          decimals = 2;
         break;
        case 2:
          value = data.inpVoltage;
          suffix = "V";
          prefix = "BATTERY";
          decimals = 1;
         break;
      }

      // Display prefix (title)
      displayString = prefix;
      displayString.toCharArray(displayBuffer, 10);
      u8g2.setFont(u8g2_font_profont12_tr);
      u8g2.drawStr(x, y - 1, displayBuffer);

      // Split up the float value: a number, b decimals.
      first = abs(floor(value));
      last = value * pow(10, 3) - first * pow(10, 3);

      // Add leading zero
      if (first <= 9) {
        displayString = "0" + (String)first;
      } else {
        displayString = (String)first;
      }

      // Display numbers
      displayString.toCharArray(displayBuffer, 10);
      u8g2.setFont(u8g2_font_logisoso22_tn );
      u8g2.drawStr(x + 55, y + 13, displayBuffer);

      // Display decimals
      displayString = "." + (String)last;
      displayString.toCharArray(displayBuffer, decimals + 2);
      u8g2.setFont(u8g2_font_profont12_tr);
      u8g2.drawStr(x + 86, y - 1, displayBuffer);

      // Display suffix
      displayString = suffix;
      displayString.toCharArray(displayBuffer, 10);
      u8g2.setFont(u8g2_font_profont12_tr);
      u8g2.drawStr(x + 86 + 2, y + 13, displayBuffer);

    }

    void drawThrottle() {
      int x = 0;
      int y = 18;

      // Draw throttle
      u8g2.drawHLine(x, y, 52);
      u8g2.drawVLine(x, y, 10);
      u8g2.drawVLine(x + 52, y, 10);
      u8g2.drawHLine(x, y + 10, 5);
      u8g2.drawHLine(x + 52 - 4, y + 10, 5);

      if (throttle >= 127) {
        int width = map(throttle, 127, 255, 0, 49);

        for (int i = 0; i < width; i++) {
          //if( (i % 2) == 0){
          u8g2.drawVLine(x + i + 2, y + 2, 7);
          //}
        }
      } else {
        int width = map(throttle, 0, 126, 49, 0);
        for (int i = 0; i < width; i++) {
          //if( (i % 2) == 0){
          u8g2.drawVLine(x + 50 - i, y + 2, 7);
          //}
        }

      }
    }

    bool signalBlink = false;

    void drawSignal() {
      // Position on OLED
      int x = 114; int y = 17;

      if (connected == true) {
        if (triggerActive()) {
          u8g2.drawXBM(x, y, 12, 12, signal_transmitting_bits);
        } else {
          u8g2.drawXBM(x, y, 12, 12, signal_connected_bits);
        }
      } else {
        if (millis() - lastSignalBlink > 500) {
          signalBlink = !signalBlink;
          lastSignalBlink = millis();
        }

        if (signalBlink == true) {
          u8g2.drawXBM(x, y, 12, 12, signal_connected_bits);
        } else {
          u8g2.drawXBM(x, y, 12, 12, signal_noconnection_bits);
        }
      }
    }

    void drawBatteryLevel() {
      int level = batteryLevel();

      // Position on OLED
      int x = 108; int y = 4;

      u8g2.drawFrame(x + 2, y, 18, 9);
      u8g2.drawBox(x, y + 2, 2, 5);

      for (int i = 0; i < 5; i++) {
        int p = round((100 / 5) * i);
        if (p <= level)
        {
          u8g2.drawBox(x + 4 + (3 * i), y + 2, 2, 5);
        }
      }
    }



**and RECEIVER:**


    #include <SPI.h>
    #include <nRF24L01.h>
    #include "RF24.h"
    #include "VescUart.h"

    #define SERIALO
    #define SERIALIO Serial

    struct vescValues {
      float ampHours;
      float inpVoltage;
      long rpm;
      long tachometerAbs;
    };

    RF24 radio(9, 10);
    const uint64_t pipe = 0xE8E8F0F0E1LL;

    bool recievedData = false;
    uint32_t lastTimeReceived = 0;

    int motorSpeed = 127;
    int timeoutMax = 500;
    int speedPin = 5;
    int lightPin = 7;
    int lightValue;

    struct bldcMeasure measuredValues;

    struct vescValues data;
    unsigned long lastDataCheck;

    void setup() {
      SERIALIO.begin(115200);

      radio.begin();
      radio.enableAckPayload();
      radio.enableDynamicPayloads();
      radio.openReadingPipe(1, pipe);
      radio.startListening();

      pinMode(speedPin, OUTPUT);
      analogWrite(speedPin, motorSpeed);
      pinMode(lightPin, OUTPUT);
    }

    void loop() {
  
   
      getVescData();
      // If transmission is available
      if (radio.available())
      {
        // The next time a transmission is received on pipe, the data in gotByte will be sent back in the                     acknowledgement (this could later be changed to data from VESC!)
        radio.writeAckPayload(pipe, &data, sizeof(data));

        // Read the actual message
        radio.read(&motorSpeed, sizeof(motorSpeed));   
        recievedData = true;

        radio.read(&lightValue, sizeof(lightValue));
    
        if (lightValue==1){
          digitalWrite(lightPin, HIGH);
        }
        else {
          digitalWrite(lightPin, LOW);
        }
      }

      if (recievedData == true)
      {
        // A speed is received from the transmitter (remote).

        lastTimeReceived = millis();
        recievedData = false;

        // Write the PWM signal to the ESC (0-255).
        analogWrite(speedPin, motorSpeed);
      }
      else if ((millis() - lastTimeReceived) > timeoutMax)
      {
        // No speed is received within the timeout limit.
        motorSpeed = 127;
        analogWrite(speedPin, motorSpeed);
      }
    }

    void getVescData() {

      if (millis() - lastDataCheck >= 250) {

        lastDataCheck = millis();

        // Only transmit what we need
        if (VescUartGetValue(measuredValues)) {
          data.ampHours = measuredValues.ampHours;
          data.inpVoltage = measuredValues.inpVoltage;
          data.rpm = measuredValues.rpm;
          data.tachometerAbs = measuredValues.tachometerAbs;
        } else {
          data.ampHours = 0.0;
          data.inpVoltage = 0.0;
          data.rpm = 0;
          data.tachometerAbs = 0;
        }
      }
    }
```

---
## \#962 Posted by: Boesila Posted at: 2018-02-27T14:01:27.780Z Reads: 273

```
Thanks for that hint... unfortunately there isn't such a mod :-(
```

---
## \#963 Posted by: solidgeek Posted at: 2018-02-27T22:02:36.480Z Reads: 290

```
I believe the problem in your code is that the receiver never knows if its a lightValue or a throttle value it receives. I would add both throttle and lightvalue to a struct, and then transmit that whole struct. In this way you only have to do one radio.write(&package, sizeof(package)). 

    struct transmit {
      int throttle;
      bool light;
    } package;

And then of course save the lightValue to the struct before transmitting it:

    package.throttle = throttle;
    package.light = lightValue;

    sendSuccess = radio.write(&package, sizeof(package));
```

---
## \#964 Posted by: Migro Posted at: 2018-02-28T11:53:15.604Z Reads: 276

```
Cap? what cap? And where should it be?
```

---
## \#965 Posted by: Boesila Posted at: 2018-02-28T14:23:38.734Z Reads: 288

```
THANKS!

What should I write in the receiver code?
This does not work :-(

     radio.read(&package, sizeof(package));
    if (lightValue==1){
      digitalWrite(lightPin, HIGH);
    }
    else {
      digitalWrite(lightPin, LOW);
    }
```

---
## \#966 Posted by: Scoo_B_SK8 Posted at: 2018-02-28T15:08:49.563Z Reads: 292

```
https://arduino-info.wikispaces.com/Nrf24L01-2.4GHz-HowTo  <== nice colorful write up (although it appears site is closing soon).

"Solder a 100nF ceramic cap across the gnd and 3.3v pins direct on the nrf24l01+ modules!Some have used a 1uF to 10uF capacitor."

SIDE NOTE; on any remote style used, be sure you have the right corresponding "nrf24 library" and change the OG pipe#.
```

---
## \#967 Posted by: Migro Posted at: 2018-02-28T15:15:40.415Z Reads: 284

```
Okay thanks. This could cause my connection failure after 30sec - 1 min? 

And i'm going to change the pipe when its all up and working. Wouldn't like to run into one with similar pile address :wink:
```

---
## \#968 Posted by: Mathieu Posted at: 2018-02-28T19:31:48.535Z Reads: 308

```
Would this work with the VESC 4?
```

---
## \#969 Posted by: solidgeek Posted at: 2018-02-28T19:42:30.586Z Reads: 318

```
@Boesila You have to learn a little more about C-programming that's for sure :P 

You have to define the struct in the top of the receiver code as well (don't know if you remembered), and then you should be able to read the content of the struct like so:

    // Saves the data in the struct     
    radio.read(&package, sizeof(package));

    // Reads data from struct
    if(package.light == 1){
      ...
    }

@Mathieu Yes it works with VESC 4 as long as you use the right library from RollingGecko :slight_smile:
```

---
## \#970 Posted by: ervinelin Posted at: 2018-03-01T09:08:44.899Z Reads: 295

```
Out of curiosity, how are you doing up the lights? Relay from the receiver? Then how are the lights powered? 

I ask because I too wanted to do something like this but I couldn't figure out how to safely relay 10S down to something the LEDs might need...
```

---
## \#971 Posted by: moon Posted at: 2018-03-01T16:16:22.851Z Reads: 304

```
[quote="navgor, post:754, topic:28543"]
I can print a full remote for £34 shipped to uk or 57usd shipped anywhere in the world.
[/quote]

Good price, but surely people would only need the shell printed for SLA?
```

---
## \#972 Posted by: Boesila Posted at: 2018-03-01T19:17:40.959Z Reads: 301

```
You need a DC-DC converter (called BEC)... I bought this one:
https://de.aliexpress.com/item/DC-DC-Buck-Converter-KIT-Adjustable-Power-Supply-DC-DC-Step-Down-Adapter-3A-LM2596HVS-LM2596HV/32803672846.html

It didn't arrived jet, so I can not say if its working or not
```

---
## \#973 Posted by: ervinelin Posted at: 2018-03-01T23:09:28.853Z Reads: 301

```
And a relay to turn on the converter?
```

---
## \#974 Posted by: Jammeslu Posted at: 2018-03-02T07:07:01.572Z Reads: 303

```
@solidgeek. How is beta going?
```

---
## \#975 Posted by: Boesila Posted at: 2018-03-02T16:53:48.874Z Reads: 309

```
That's the plan 😊
```

---
## \#977 Posted by: lambievu0916 Posted at: 2018-03-05T06:52:12.509Z Reads: 301

```
I wanna start building this but there isnt a schematic that i can find, has anyone successfully built this yet?
```

---
## \#978 Posted by: ervinelin Posted at: 2018-03-05T13:08:36.491Z Reads: 302

```
Yes myself and several others here I believe. You will need to sift through info on this page as well as solidgeeks wiki page to build it.
```

---
## \#979 Posted by: webst Posted at: 2018-03-05T13:21:09.994Z Reads: 310

```
Please summarize this topic when you decide to build it. For now there are 971 replies with an estimated read time of 107 minutes.
```

---
## \#980 Posted by: Deakbannok Posted at: 2018-03-05T15:40:59.097Z Reads: 321

```
Here is video of the cruise control on a dry run.
It runs different when is loaded.
I have forked the code on github you may find it under the development source.
https://youtu.be/zXkidgwjiIU
```

---
## \#981 Posted by: ervinelin Posted at: 2018-03-05T16:50:07.010Z Reads: 318

```
I have written a build guide for my version of the remote, available here:

https://github.com/ModMiniMan/nRF24-Esk8-Remote/wiki

I have also started another thread on my version of the remote so as not to confuse people reading this post.

https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231
```

---
## \#982 Posted by: Becker33 Posted at: 2018-03-06T22:58:05.146Z Reads: 302

```
It would be really useful if someone could update the Wiki page to be more comprehensive and beginner friendly? I know it's easier said than done but it would allow many more to make and test the remote! If not the wiki page then maybe a shared document? @solidgeek I really like the way @ervinelin wrote the guide to his version of the remote :slight_smile:
```

---
## \#983 Posted by: SeeTheBridges Posted at: 2018-03-07T01:54:41.856Z Reads: 293

```
I've been working on a video build guide for the last few months, so something till be going up by the end of the month! I just got my firefly back from the Pulse team bc they wanted to test it out while they were repairing my board. I can finally film my intros and outros now that I have it back
```

---
## \#984 Posted by: Becker33 Posted at: 2018-03-07T07:31:56.372Z Reads: 291

```
Perfect! Can't wait to see it
```

---
## \#985 Posted by: solidgeek Posted at: 2018-03-08T17:17:08.419Z Reads: 299

```
I just want to thank you for your code snippet using the Servo library. This works much better than standard PWM from the Arduino. The throttle no longer cuts off at max or minimum throttle, which is very nice... I can't believe I didn't get this fixed a lot earlier, hopefully, no one has been injured while maxing out the throttle! 

I have included this in the newest update to the development branch on my GitHub page.  By using the new update the VESC has to remap the PPM pulse lengths via the VESC tool - however shouldn't be a issue :slight_smile:
```

---
## \#986 Posted by: Clonkex Posted at: 2018-03-08T21:56:33.642Z Reads: 292

```
Honestly I'm quite surprised the standard PWM worked at all, but I'm glad it's more reliable now :D
```

---
## \#987 Posted by: Deakbannok Posted at: 2018-03-09T01:51:13.604Z Reads: 294

```
Is done ;D![20180309_020335|690x388](upload://8D33M5rQwgDfdqgy1qPoCYbUDoC.jpg)
```

---
## \#988 Posted by: xype Posted at: 2018-03-09T20:54:24.401Z Reads: 282

```
@solidgeek Do you think this switch would be a good fit? 
http://swechtrading.se/zencart/index.php?main_page=product_info&cPath=188_34&products_id=531
```

---
## \#989 Posted by: solidgeek Posted at: 2018-03-09T23:23:49.688Z Reads: 278

```
I think it should fit just about right :-)
```

---
## \#990 Posted by: junwoo091400 Posted at: 2018-03-10T11:52:08.342Z Reads: 277

```
Thank you for the design. I am currently designing a pcb for this remote. But realized it would be much easier to size the pcb(since currently it is a tight fit) if i had design files. Can you share actual modifiable non-mesh file? I hope it is compatible with Fusion360
```

---
## \#991 Posted by: Snowi Posted at: 2018-03-10T19:13:46.840Z Reads: 279

```
I got extra parts I could sell to you guys, if you need them. I live in the US, so its quick delivery to those of you guys that live in US, so if you want to start working on this, you can. All you gotta do is 3d print them.

I got:

3 * Arduino Nanos w/o Pins
10 * TP4056 Charging Modules (don’t know if you can use that tho but lmk)
10 * NRF24L01
5 * 5 meters of 30 AWG Wires (each of color of red, blue, yellow, white, and black)
20 * 5x5mm magnets
1 * SS495A Hall Sensor
2 * OLED Screen (They fit the ones on the remote control)
1 * 3.7V 500 mAh battery (fits in remote control)

If you are interested, please let me know. Trying to get rid of these things
```

---
## \#992 Posted by: Jcullinan09 Posted at: 2018-03-10T22:47:46.387Z Reads: 267

```
@Snowi I just finished reading this entire thread from the very beginning, and I would indeed buy all of these parts off of you! A question before, though is, are these all the parts necessary that are on the excel spreadsheet? Oh and by the way I am in USA, Minnesota.
```

---
## \#993 Posted by: ron Posted at: 2018-03-11T00:32:20.282Z Reads: 261

```
Is it possible to use a Smartphone with APP through BT Connection to track Telemetry data with this remote simultaneously somehow?

NRF24 and BT would use both UART . Can I conect only the TX from the VESC to the BT module in parallel?
```

---
## \#994 Posted by: solidgeek Posted at: 2018-03-11T00:48:45.791Z Reads: 266

```
Unfortunately no, the UART port cannot be shared as far as I know. However, if you run a dual setup I guess you could add the BT module to one VESC and the receiver to the other, and then connect them by CAN-bus.
```

---
## \#995 Posted by: Snowi Posted at: 2018-03-11T03:50:02.471Z Reads: 266

```
Yeah, every part is used on the spreadsheet. All you need is to 3d print the controller and screws.
```

---
## \#996 Posted by: Zyb Posted at: 2018-03-11T16:08:04.430Z Reads: 278

```
i was able to make a connection, both receiver and transmitter works but theres one problem. whenever i powerup my vesc receiver does not respond i need to press reset button once and after that theres no problem. this happens everytime and its unusable this way. i tried to power it from another 5v source but same thing, i needed to press reset again. anyone encountered this problem? oh also this problem doesnt occur when i power it from its usb socket.

@solidgeek
im trying to upload your latest receiver build. had no issue with transmitter uploading but receiver gives this error code:
receiver:124: error: 'SetSerialPort' was not declared in this scope

   SetSerialPort(&Serial);

am i missing something? Thanks

OK i found where i did the mistake. For the latest version you need vesc6 rollinggecko library while master version goes along with master version of rollinggecko. compiled and uploaded successfully but they dont have communication while master version connects almost instantly when transmitter and reciever has power. just to be sure i rolled back to master version and everything works fine. any ideas?
```

---
## \#997 Posted by: Deakbannok Posted at: 2018-03-11T21:19:53.183Z Reads: 275

```
you must declare the serial of setserialport first

#define SERIALIO Serial
// add this to the header

void setup(){
  // Open serial VESC data
  //Setup UART port
  SetSerialPort(&SERIALIO);
  SERIALIO.begin(115200);
```

---
## \#998 Posted by: Zyb Posted at: 2018-03-11T21:21:20.356Z Reads: 270

```
that problem vanished as soon as i used the vesc 6 rollinggecko library or is it related to the connection issue that i have ?

on a side note: Rx led on receiver used to blink constantly but it does not blink at all when latest build is installed
```

---
## \#999 Posted by: Jcullinan09 Posted at: 2018-03-11T21:35:30.179Z Reads: 267

```
I have a question regarding which SS495A hall sensor to use? Will they both work the same?

Link 1: https://www.mouser.com/ProductDetail/Honeywell/SS495A/?qs=%2ffq2y7sSKcKEzWT94S3drA==

or

Link 2: https://www.digikey.ca/product-detail/en/texas-instruments/DRV5053OAQLPGM/296-40059-1-ND/5177936
```

---
## \#1000 Posted by: Snowi Posted at: 2018-03-11T21:53:52.514Z Reads: 264

```
The first one, but shipping will cost like $10 for that small item. I got an extra one, I'll sell you one for like $4 bucks.

There are different hall sensors but make sure its SS495A
```

---
## \#1001 Posted by: Apolo Posted at: 2018-03-13T01:56:26.238Z Reads: 253

```
How's the travel on the wheel? Really looking for something with far travel to get more control
```

---
## \#1002 Posted by: SeeTheBridges Posted at: 2018-03-13T14:25:56.053Z Reads: 259

```
Yeah, I tried flashing the dev branch last night and I couldn't get it to work at all. Hope it all gets sorted soon :( this whole receiver not connecting on first power on properly is getting quite annoying. I'm tempted to just wire a switch under my deck to reset the Arduino manually without needing to take the whole enclosure off
```

---
## \#1003 Posted by: Snowi Posted at: 2018-03-13T16:09:42.052Z Reads: 282

```
I got extra parts I could sell to you guys, if you need them. I live in the US, so its quick delivery to those of you guys that live in US, so if you want to start working on this, you can. All you gotta do is 3d print them.

I got:

* 3 * Arduino Nanos w/o Pins

* 10 * TP4056 Charging Modules (don’t know if you can use that tho but lmk)

* 10 * NRF24L01

*  ̶5̶ ̶*̶ ̶5̶ ̶m̶e̶t̶e̶r̶s̶ ̶o̶f̶ ̶3̶0̶ ̶A̶W̶G̶ ̶W̶i̶r̶e̶s̶ ̶(̶e̶a̶c̶h̶ ̶o̶f̶ ̶c̶o̶l̶o̶r̶ ̶o̶f̶ ̶r̶e̶d̶,̶ ̶b̶l̶u̶e̶,̶ ̶y̶e̶l̶l̶o̶w̶,̶ ̶w̶h̶i̶t̶e̶,̶ ̶a̶n̶d̶ ̶b̶l̶a̶c̶k̶)̶ **(SOLD)**

* 20 * 5x5mm magnets

* 1 * SS495A Hall Sensor

* 2 * OLED Screen (They fit the ones on the remote control)

* 1 * 3.7V 500 mAh battery (fits in remote control)

If you are interested, please let me know. Trying to get rid of these things

EDIT: sold the wires but still got a lot of parts left for you guys!!!
```

---
## \#1004 Posted by: Deakbannok Posted at: 2018-03-13T20:59:46.683Z Reads: 266

```
Try the master branch. see if you can get your tx and rx connected. 

NO ? check your wiring connection on your RF24.
YES ? You can continue flash the dev branch. You need to clear out the EEPROM on both tx and rx
```

---
## \#1005 Posted by: SeeTheBridges Posted at: 2018-03-13T21:05:30.800Z Reads: 258

```
I can use the master branch fine, but I've never been able to get telemetry with TX and RX working. I'm thinking that's just due to the ackmaniacs firmware the Pulse uses at this point tho
```

---
## \#1006 Posted by: Mtnmuse Posted at: 2018-03-13T21:44:48.438Z Reads: 262

```
Hi @Snowi, just started to read this, this guide looks like gold ! Sounds like you have everything to build another remote? 

How far are along are you?  Did it work lol? I'd love to buy some of your spares. Please let me know.
```

---
## \#1007 Posted by: escu_12 Posted at: 2018-03-13T22:08:00.815Z Reads: 264

```
i have a problem allways reply failed transmission in debug mode and normal mode not connect never connect and the example getting started works fine

what happends?
```

---
## \#1008 Posted by: solidgeek Posted at: 2018-03-13T22:17:43.490Z Reads: 277

```
I am pretty sure the problem with your receiver is a power issue, especially because it works powered by USB :-) You could try to add a few different bypass capacitors on the receivers power line, to filter out any noise or maybe add an LC filter as one suggested. Are you using a standard Arduino Nano, or the one I recommend? 

If you are trying out my development branch, and you have a VESC 4 you will have to use this branch of RollingGeckos library: 
https://github.com/RollingGecko/VescUartControl/tree/imartinezl-master

If you have a VESC 6 this is the branch to use:
https://github.com/RollingGecko/VescUartControl/tree/VESC6

Hope it helps
```

---
## \#1009 Posted by: ron Posted at: 2018-03-14T00:05:46.734Z Reads: 251

```
Did someone tested the NRF Remote in a Dual VESC Setup (ackmaniacs Firmware) with Bluetooth module connected simultaneously to a Smartphone to get Telemetry data tracked/captured?
```

---
## \#1010 Posted by: Deakbannok Posted at: 2018-03-14T00:08:19.028Z Reads: 252

```
If you have Dual VESC setup. You can connect BLT to your Slave VESC and CAN  to the Master VESC.
```

---
## \#1011 Posted by: SeeTheBridges Posted at: 2018-03-14T00:08:44.256Z Reads: 249

```
So the Pulse Echo matches this description and I have been trying for so long to no avail to get both working. Honestly, I can't get any telemetry from my Firefly but the included BT module works fine.
```

---
## \#1012 Posted by: Deakbannok Posted at: 2018-03-14T00:23:50.965Z Reads: 248

```
If you can get the TX and RX but no telemetry.
You need go into the setting of Controller and select PPM and switch back PPM/UART again. Is if that will fix.

That because rxSettings.controlMode is == 0; so you might not getting a read back.
if ( rxSettings.controlMode != 0 ) {
        getUartData();
        radio.writeAckPayload(1, &returnData, sizeof(returnData));
}
```

---
## \#1013 Posted by: SeeTheBridges Posted at: 2018-03-14T01:27:25.731Z Reads: 249

```
So a low pass filter should fix this power issue... Have any thoughts on maybe using this one? I figure the nano can't pull more than 5V 1A right? Space is currently a HUGE premium for me in the Echo enclosure

http://www.myrcmart.com/lc-filter-super-micro-for-micro-multirotor-14s-1a-current-02g-p-11036.html
```

---
## \#1014 Posted by: Snowi Posted at: 2018-03-14T05:53:09.969Z Reads: 249

```
Hey man, I just sold the wires, but i got all the rest of the parts. I even got some 3d printed stuff you can use if you want.
```

---
## \#1015 Posted by: Zyb Posted at: 2018-03-14T14:35:04.598Z Reads: 253

```
Thanks for the reply, I was thinking to use usb cable as my power and attach the capacitor to it but I ll try the LC filter like @ervinelin did. 
@SeeTheBridges  routing a reset button just feels like poor mans solution to the problem. Need something proper and refined. I’m sure lc filter or powering from usb socket will work. I’m powering transmitter from usb socket and works without a problem, not using the 5V line.
```

---
## \#1016 Posted by: SeeTheBridges Posted at: 2018-03-14T16:54:53.933Z Reads: 256

```
So I was talking to deakbannok on discord last night and he helped me get my telemetry working on his separate fork! 🤗🤗 (Turns out I wasn't making sufficient contact to the VESC UART terminals 😅) he also told me that the power issues might just be down to low quality capacitors. I did a bunch of research last night when he suggested looking specifically for low ESR caps instead of using an LC filter, and the first person drone racing community has done a TON of real world comparison testing between them already. What I learned was that low ESR caps are preferable, but an LC filter is better than a cheap capacitor. 

SO, I'm gonnna say the wiki should be ammended to include a line about making sure to find a high quality name brand low ESR cap since it should be cheaper than even the micro LC filter that I ordered last night. Due to space constraints though, I may use the micro filter instead tho since it appears to be TINY compared to the caps I do I have right now
```

---
## \#1017 Posted by: ervinelin Posted at: 2018-03-15T03:35:36.068Z Reads: 249

```
So it's not just me!! 

It's a real pain, just yesterday night I spent HOURS trying to figure out why I need to do the same on my transmitter after I replaced some parts on it... It needs a hard reset in order to get going.

Same thing for my receivers, but receiver problem seem to have been resolved by doing 2 things. 1 - Include and LC filter, 2 - Place the receiver as far away from the main power lines as possible.

Googling this symptom has found that there might be a solution by soldering a capacitor between the reset and ground pins on the arduino. I'll try and see if it works.
```

---
## \#1018 Posted by: Clonkex Posted at: 2018-03-15T04:13:32.913Z Reads: 251

```
I've got my own custom-designed remote that also uses Arduinos + NRF modules and by coincidence happens to be basically identical to @solidgeek's system. I'm having some odd issues where it begins to lose connection (or rather, the signal gets weaker) the longer I ride, to the point (usually after 30 minutes or so) where simply holding the remote above waist height is enough to break the connection. I tested leaving the board and remote switched on for a couple of hours and they still functioned perfectly, so I decided it must be something to do with heat (based on some other very non-scientific experiments it _seems_ to be related specifically to Focbox heat). I have a 220uf cap on the power from the Focbox but none between the chinese clone Arduino and the NRF module, so that's what I'll try next. I also hadn't realised that low-ESR caps existed and I never considered that my cap my be very low quality, just being a cheap chinese one.

I'm really confused how it could be heat related though, especially on the receiver. Maybe the Arduino's power regulator is really bad and gets worse as it gets hotter? That seems weird to me but maybe it's normal.

Either way I'm very interested in this thread since it's basically helping me solve my custom remote's issues :P
```

---
## \#1019 Posted by: Mich21050 Posted at: 2018-03-15T17:38:54.956Z Reads: 244

```
Hi, I´m selling a full kit to build the remote. I would offer the following parts:
2 * magnets (5mm)
Boost converter
Lipo charger
3.7V battery
OLED display
2 * Arduino Nano
2 * nRF24L01 (one already soldered)
Hall sensor
Micro USB
Power switch
Spring
Limit switch
all 3D printed Parts

Price: 40€ plus shipping 
If anyone is interested just send me a PM :smile:
```

---
## \#1020 Posted by: SeeTheBridges Posted at: 2018-03-15T18:39:41.793Z Reads: 239

```
Just wired up my micro LC filter annnndddd it didn't work. Maybe a bigger one is necessary? these micro ones are rated for 16V1A, but I guess that's not enough. I tried it both by itself and with my 220uF capacitor wried before it. Maybe the cap needs to come AFTER the LC filter? idk.

EDIT: Tried putting the cap on the output of the LC filter too. Still didn't fix the issue. Honestly I'm not sure what else to try
```

---
## \#1021 Posted by: Zyb Posted at: 2018-03-15T18:58:02.929Z Reads: 240

```
Did you try connecting directly to 5v line without lc filter or a cap? See if it works that way at least you will know if they have any effect or not. Last resort would be connecting via usb socket. When I get home I ll try it. Taking the insulation off around the plug makes it super small and viable.
```

---
## \#1022 Posted by: SeeTheBridges Posted at: 2018-03-15T18:59:03.194Z Reads: 241

```
I haven't tried that yet because I was under the assumption the cap was recommended since it just doesn't work without it?
```

---
## \#1023 Posted by: Zyb Posted at: 2018-03-15T19:02:49.670Z Reads: 249

```
It was added to eliminate signal issues. It should work without a cap
```

---
## \#1024 Posted by: Jc06505n Posted at: 2018-03-15T19:03:42.099Z Reads: 246

```
According to @Cncninja the 

[quote="Cncninja, post:39, topic:48231"]
capacitor to help stabilize voltage on the 5v rx input.
[/quote]
```

---
## \#1025 Posted by: SeeTheBridges Posted at: 2018-03-15T19:04:29.886Z Reads: 242

```
If it's not working with a cap to stabilize it, I doubt it'll work without too :frowning:

EDIT, is there maybe a VESC related setting that could be causing an issue somewhere?
```

---
## \#1026 Posted by: Zyb Posted at: 2018-03-15T19:07:09.526Z Reads: 243

```
Post #55 explains it. Assuming it is only for more stable connection it should at least work without it. Because in our situation arduino just plays dead. That’s whole another problem.
```

---
## \#1027 Posted by: SeeTheBridges Posted at: 2018-03-15T19:17:54.363Z Reads: 239

```
Playing dead is a good way to put it lol yeah running it with nothing didn't fix it either. surprise surprise.
```

---
## \#1028 Posted by: Zyb Posted at: 2018-03-15T19:25:27.472Z Reads: 229

```
Lol well usb power is the only thing left to try 😁
```

---
## \#1029 Posted by: SeeTheBridges Posted at: 2018-03-15T19:26:15.219Z Reads: 223

```
How would I even do that? I'm gonna try pulling VCC from UART next bc why not
```

---
## \#1030 Posted by: Nandox7 Posted at: 2018-03-15T19:28:11.943Z Reads: 234

```
Checking in case has even had the same problem.

Got 3 OLED's  for this, two out of the three can't make them work.
Tried all  found codes and example and nothing.
Using eh arduino i2c scanner for both's he find them at their address 0x03c 
but they never work. :|

Anyone had similar problem?
```

---
## \#1031 Posted by: SeeTheBridges Posted at: 2018-03-15T19:29:06.188Z Reads: 223

```
I had an OLED inexplicably die. Apparently they're just really sensitive
```

---
## \#1032 Posted by: Nandox7 Posted at: 2018-03-15T19:30:50.700Z Reads: 228

```
I've used the 168x64 for other projects and they can take some abuse.
But seems like that is the answer... those things just go bad quite easily.
```

---
## \#1033 Posted by: SeeTheBridges Posted at: 2018-03-15T19:49:56.886Z Reads: 237

```
So I spliced the power lead to just behind the micro USB port to feed it power there, and still doesn't boot up properly. I tried it with power from both PPM and UART. I'm at a lost rn. I don't understand why it won't start up properly
```

---
## \#1034 Posted by: Zyb Posted at: 2018-03-15T20:13:35.840Z Reads: 235

```
Damn I was hoping for usb to solve this issue :/
```

---
## \#1035 Posted by: Zyb Posted at: 2018-03-15T20:23:15.728Z Reads: 238

```
Take a look at here, seems like they have the same problem https://forum.arduino.cc/index.php?topic=256771.0
```

---
## \#1036 Posted by: SeeTheBridges Posted at: 2018-03-15T20:43:55.415Z Reads: 239

```
Looks like post #37 has a solution: https://forum.arduino.cc/index.php?topic=256771.msg2359179#msg2359179

a 10uF cap and 470 ohm resistor in series form the reset pin to ground
```

---
## \#1037 Posted by: Zyb Posted at: 2018-03-15T20:58:38.184Z Reads: 236

```
Fingers crossed for the method
```

---
## \#1038 Posted by: SeeTheBridges Posted at: 2018-03-15T21:02:28.306Z Reads: 235

```
damn, the electrical engineering parts room just closed :( I'll have to wait till tomorrow to buy those parts to try it
```

---
## \#1039 Posted by: Zyb Posted at: 2018-03-15T21:06:30.042Z Reads: 239

```
just hope it works, as soon I get back home I need to try those possible solutions :)
```

---
## \#1040 Posted by: SeeTheBridges Posted at: 2018-03-16T03:24:23.662Z Reads: 257

```
So I was bored and I may have found a solution that someone needs to tell me is a bad idea. But bridging the RST and GND pins with my cheap 220uF cap, I get proper startup on some example sketches all of the time. I've also got the LC filter wired up to keep some of the noise on the power lines at bay. Can someone tell me why this is a bad idea? 😂 I've ordered a bunch of low ESR caps, but I'm curious if this is a viable option too.

"The benefit of a capacitor between RESET and Gnd is that it will keep the chip in reset mode for a brief period - and hence help with any contact bounce on the power supply."
http://www.societyofrobots.com/robotforum/index.php?topic=3903.0
```

---
## \#1041 Posted by: ervinelin Posted at: 2018-03-16T10:58:46.908Z Reads: 255

```
That was what I was planning to do as well...

Edit: tried it on my remote... Works!! I used a 100uF 10V cap soldered directly to the pins...

![IMG20180316215112|690x388](upload://jnrBtO7H5EwXvXuj3X71Rjy2de0.jpg)
```

---
## \#1042 Posted by: ervinelin Posted at: 2018-03-16T16:21:46.813Z Reads: 253

```
Just to add on in case you guys don't read my other thread...

I added an LC filter and a large 1000uF cap to the receiver 5V supply. LC filter smooths out the noise, cap prevents brownouts. The latter I was getting when I tried to ride slowly upslope, I would lose connection (and brakes!!!) and it wouldn't come back till I stopped for a few seconds.
```

---
## \#1043 Posted by: SeeTheBridges Posted at: 2018-03-16T19:54:41.730Z Reads: 259

```
Hmmmm that's good to know. I'm at my Electrical engineering stockroom right now trying out different capacitors to bridge the Reset and GND pins with. I had success with some .022uF ceramic caps that are absolutely TINY and perfect for size constrained areas like my enclosure. These were the specific ones I plan on using. 

https://www.digikey.com/product-detail/en/kemet/C320C223K1R5TA/399-4284-ND/818060

I'm gonna leave my LC filter on the power line too and probably put the 22ouF cap on it just in case after hearing about that.
```

---
## \#1044 Posted by: Seikeau Posted at: 2018-03-16T20:27:16.103Z Reads: 247

```
Where are you shipping from (or 'what are the costs of shipping to the Netherlands')? Also, what material and color did you print?
```

---
## \#1046 Posted by: Mich21050 Posted at: 2018-03-16T20:50:23.925Z Reads: 247

```
I´m shipping from Austria (shipping would cost about 3€) :smiley:  Its printed in pla and the colour is black. :smiley:
```

---
## \#1047 Posted by: ervinelin Posted at: 2018-03-16T22:49:44.497Z Reads: 252

```
Gotta try and see if a lower uF cap will work. Online it seems mostly 100 to 220uF is used for this.
```

---
## \#1048 Posted by: SeeTheBridges Posted at: 2018-03-16T22:53:44.446Z Reads: 255

```
The .022 uF ceramic cap works perfectly. It's absolutely TINY and out of the way. now I've just gotta fix my remote connection issues again :(
```

---
## \#1049 Posted by: ervinelin Posted at: 2018-03-17T01:15:51.251Z Reads: 244

```
Good to know something so tiny works!

What connection issues are you facing?
```

---
## \#1050 Posted by: SeeTheBridges Posted at: 2018-03-17T02:14:48.185Z Reads: 244

```
Running @Deakbannok's code, the main control screen freezes up if I turn on safety mode (deadman switch). If I leave the safety off, the remote continues to function fine. Everything is working almost perfectly too which is the annoying part. I know the Hall sensor and trigger are working properly because if I boot straight into the remote settings, I have no problems. I'm beginning to think maybe my voltage regulator might be an issue?
```

---
## \#1051 Posted by: ervinelin Posted at: 2018-03-17T04:51:08.673Z Reads: 236

```
Likely a code issue... Or maybe you wired the switch wrongly?
```

---
## \#1052 Posted by: SeeTheBridges Posted at: 2018-03-17T04:54:08.709Z Reads: 244

```
I'm thinking it must be one of my wirings. the code worked perfectly for a while and now just doesn't work as expected anymore

EDIT: Deak called it. One of my Ground pins wasn't soldered well enough. I think I have a fully working Firefly now,,, Will be finalizing the first part of my video build guide if that's the case.

EDIT2: just kidding. Still having problem with it
```

---
## \#1053 Posted by: Zyb Posted at: 2018-03-17T13:10:20.852Z Reads: 244

```
50v 0.68uF relatively small cap solved my requiring to reset on every boot issue. soldered it directly between rst and gnd pins.
```

---
## \#1054 Posted by: Deakbannok Posted at: 2018-03-17T20:05:51.950Z Reads: 247

```
I donno what is he talking about.... he iz crasy. i have nothing to do with anything on here 😆

problem you guys having is similar.. Please check your wiring and use a basic master branch code.
You need a get a low ers capacitors.

we are working on a PID cruise control. hope to finalize before summer.

you will have an awesome DIY controller.

I have 4 controllers that I have built and are free giving free of charge. Mainly for the local riders in Paris and a few places in Europe I would hand them out for free.
```

---
## \#1055 Posted by: Surfer Posted at: 2018-03-17T21:30:48.960Z Reads: 232

```
Thanks buddy, this looks like a real community. I am already given with your code. :)
```

---
## \#1056 Posted by: Snowi Posted at: 2018-03-17T21:46:02.129Z Reads: 257

```
Hey guys these extra parts are still up for grabs... I'll sell them all for $80. You can of course buy one or few parts.

I got:

3 * Arduino Nanos w/o Pins

10 * TP4056 Charging Modules (don’t know if you can use that tho but lmk)

10 * NRF24L01

̶5̶ ̶*̶ ̶5̶ ̶m̶e̶t̶e̶r̶s̶ ̶o̶f̶ ̶3̶0̶ ̶A̶W̶G̶ ̶W̶i̶r̶e̶s̶ ̶(̶e̶a̶c̶h̶ ̶o̶f̶ ̶c̶o̶l̶o̶r̶ ̶o̶f̶ ̶r̶e̶d̶,̶ ̶b̶l̶u̶e̶,̶ ̶y̶e̶l̶l̶o̶w̶,̶ ̶w̶h̶i̶t̶e̶,̶ ̶a̶n̶d̶ ̶b̶l̶a̶c̶k̶)̶ (SOLD)

20 * 5x5mm magnets

1 * SS495A Hall Sensor

2 * OLED Screen (They fit the ones on the remote control)

1 * 3.7V 500 mAh battery (fits in remote control)

If you are interested, please let me know. Trying to get rid of these things
```

---
## \#1057 Posted by: Shippo Posted at: 2018-03-18T08:50:09.535Z Reads: 258

```
![IMG_3993|500x500](upload://gG9wNB1cCPyaAYK44FboAa583np.JPG)

Finally! I spent all day to build, and I'm so happy with this diy remote😍 thank you @solidgeek
Now I'm going to buy VESCs. Does anyone know will Torque Board's VESC work with this remote? Will the "vescuart.h" library only work with vesc 6 (using real time data)? 
Thanks
```

---
## \#1058 Posted by: Mich21050 Posted at: 2018-03-18T12:21:08.273Z Reads: 258

```
Hi, I´m selling a full kit to build the remote. I would offer the following parts:
2 * magnets (5mm)
Boost converter
Lipo charger
3.7V battery
OLED display
2 * Arduino Nano
2 * nRF24L01 (one already soldered)
Hall sensor
Micro USB
Power switch
Spring
Limit switch
all 3D printed Parts

Price: 40€ plus shipping
If anyone is interested just send me a PM  :smile:
```

---
## \#1059 Posted by: Deakbannok Posted at: 2018-03-18T20:31:06.679Z Reads: 256

```
i have both torque and enertion. they all work fine
```

---
## \#1060 Posted by: Shippo Posted at: 2018-03-18T22:22:19.380Z Reads: 252

```
@Deakbannok Thanks for the information!
```

---
## \#1061 Posted by: SeeTheBridges Posted at: 2018-03-21T01:04:33.461Z Reads: 249

```
Ok, short update. I killed my receiver but it's ok because I built another one. The small ceramic capacitor along with the cheap 220uF electrolytic capacitor and an LC filter have made my new receiver functional from immediate power on. I'm building a second remote and I have some low ESR caps to test still, but I'm pretty confident that a small cap between reset and ground will fix any freezing issues people are having.
```

---
## \#1062 Posted by: ervinelin Posted at: 2018-03-21T05:41:03.138Z Reads: 251

```
It works for me too but I cannot upload a sketch u less I unsolder the cap connected to reset pin...
```

---
## \#1063 Posted by: SeeTheBridges Posted at: 2018-03-21T05:44:24.086Z Reads: 246

```
hmmm... I was able to upload code just fine... are you using a larger electrolytic cap?I think the really small one I'm using doesn't alter the reset timing enough for it to be a problem but maybe a bigger cap delays the reset too long to upload code?
```

---
## \#1064 Posted by: ervinelin Posted at: 2018-03-21T05:55:18.088Z Reads: 244

```
I tried a smaller cap. Didn't work. Went back to 100uF. What are you using?
```

---
## \#1065 Posted by: solidgeek Posted at: 2018-03-21T06:34:55.638Z Reads: 249

```
You have to be carefull putting a big capacitor between reset and GND.  When you turn off the arduino the cap will still be charged and the energi stored have no other way to discharge than to run into the arduino. This could fry the arduino. To limit the discharge current you could add a resistor in series with the cap.
```

---
## \#1066 Posted by: SeeTheBridges Posted at: 2018-03-21T06:35:21.321Z Reads: 253

```
I posted them earlier:
https://www.digikey.com/product-detail/en/kemet/C320C223K1R5TA/399-4284-ND/818060

It's a .022uF ceramic cap. how much smaller did you try? I tried a pF cap in the parts room but that didn't work for me
```

---
## \#1067 Posted by: ervinelin Posted at: 2018-03-21T07:45:41.421Z Reads: 254

```
I forgot what it was that I tried... I will try to hunt down what you have and report back..
```

---
## \#1068 Posted by: ervinelin Posted at: 2018-03-22T11:08:43.968Z Reads: 251

```
0.22uF cap didn't work for me.. had to go back to the big fat 100uF... :frowning:
```

---
## \#1069 Posted by: Deakbannok Posted at: 2018-03-22T11:25:04.510Z Reads: 244

```
I am not sure what is the backdraft for that cap to reset and ground thing.

Just sure you are wearing a protective gears. We are not responsible for any type of injury on here. By the default, the setup and code are fine. Both tested by me and others I have handled
```

---
## \#1070 Posted by: Zyb Posted at: 2018-03-22T11:27:59.117Z Reads: 257

```
![image|375x500](upload://3H4yJ8QPteeAcBLCBW3nUY6oybq.jpg)
This one worked for me. It’s 0.68 one of the cheapest ones
```

---
## \#1071 Posted by: Zyb Posted at: 2018-03-22T11:34:33.840Z Reads: 265

```
Is this one of the low ESR caps you guys were talking about? If it is I’m gonna give it a go on 5v line and see what happens.![image|375x500](upload://8HWWN4OXMPIwLy9uctDWYM3XSl3.jpg)
```

---
## \#1072 Posted by: webst Posted at: 2018-03-22T14:05:15.923Z Reads: 259

```
https://www.youtube.com/watch?v=WytU5uj78-4
```

---
## \#1073 Posted by: SeeTheBridges Posted at: 2018-03-22T18:49:15.554Z Reads: 262

```
By default there is obviously still some type of issue in the design! There's multiple of us that have this power issue, and while I can't speak for everyone else, I'm using all of the recommended parts on the list. That reset cap is the only thing that seems to have worked and so far as I can tell, it's doing no harm.
```

---
## \#1074 Posted by: Zyb Posted at: 2018-03-22T18:59:43.279Z Reads: 257

```
you mentioned you killed your receiver earlier, did it happen because of the the cap between reset and GND?
```

---
## \#1075 Posted by: SeeTheBridges Posted at: 2018-03-22T19:15:28.483Z Reads: 261

```
I don't believe that's what caused it. I was altering the squared shape of the Nano to better fit inside my enclosure and I think I hit a PCB trace and permanently shorted something else. Got my hands on a multimeter and several of my digital and analog read pins are shorted to ground at ~1.2V when they should be less than 200mV on a proper working Arduino. The microprocessor just starts immediately heating up and burns to the touch. if it turns out it was the cap and my second receiver dies I'll let you all know
```

---
## \#1076 Posted by: Deakbannok Posted at: 2018-03-22T20:36:27.670Z Reads: 268

```
If you are having issue with center noises. drill the thumb
![20180321_003634|281x500](upload://daZnEfhyCyWtDFXxpdSbxrr9I0.jpg)
```

---
## \#1077 Posted by: SeeTheBridges Posted at: 2018-03-22T23:00:38.693Z Reads: 262

```
The center noise isn't my main concern right now. I'm worried about this power issue and the ceramic cap potentially killing another arduino
```

---
## \#1078 Posted by: Snowi Posted at: 2018-03-24T15:38:37.570Z Reads: 264

```
Still got these parts for sale. PM me. Dont need to be bought as a whole but I am trying to give this away so im doing a large discount if all bought together.

I got:

3 * Arduino Nanos w/o Pins

10 * TP4056 Charging Modules (don’t know if you can use that tho but lmk)

10 * NRF24L01

20 * 5x5mm magnets

1 * SS495A Hall Sensor

2 * OLED Screen (They fit the ones on the remote control)

1 * 3.7V 500 mAh battery (fits in remote control)
```

---
## \#1079 Posted by: Mich21050 Posted at: 2018-03-24T19:28:22.010Z Reads: 268

```
Hi, I´m selling a full kit to build the remote. I would offer the following parts:
2 * magnets (5mm)
Boost converter
Lipo charger
3.7V battery
OLED display
2 * Arduino Nano
2 * nRF24L01 (one already soldered)
Hall sensor
Micro USB
Power switch
Spring
Limit switch
all 3D printed Parts

Price: 40€ plus shipping
If anyone is interested just send me a PM  :smile:
```

---
## \#1080 Posted by: SeeTheBridges Posted at: 2018-03-24T20:46:37.150Z Reads: 263

```
Well, it's not gonna be much help for those of you trying to assemble your remotes right now, but for those of you interested in the idea, Part 1 of my tutorial is up. It goes over all of the preparation worth you'll need to do before you can start assembling/ordering your parts.
https://youtu.be/N032HqxeymA
```

---
## \#1081 Posted by: landonkun Posted at: 2018-03-25T05:32:19.498Z Reads: 259

```
Nice! I saw this earlier today. I'm a bit of an electronics noob myself, so I've been putting off building my own after I saw some issues people were having and adding capacitors and whatnot. I figured I'd wait for a tutorial like this before I got started. I have all the other parts though, and I just need to order some more filament for my printer :slight_smile:
```

---
## \#1082 Posted by: Apolo Posted at: 2018-03-26T00:54:01.031Z Reads: 265

```
did PETG
![18|375x500](upload://kHAvFzqLRWl2QPatgXBaGMybDrp.jpeg)
```

---
## \#1083 Posted by: Kit Posted at: 2018-03-26T23:31:26.833Z Reads: 240

```
I want to print the case but I have to use 3DHubs - should I model this in mm, cm, or in?
```

---
## \#1084 Posted by: Apolo Posted at: 2018-03-26T23:36:40.808Z Reads: 247

```
mm. I Can print a set for you for $18 shipped by friday
```

---
## \#1085 Posted by: Shagrat Posted at: 2018-03-28T10:27:04.775Z Reads: 252

```
guys, but what about the spreadsheets and electronics for the reciever? and can someone summarize if there still is some problems or if they have been fixed wich is the fix? I've read all te post twice but still having serious dubts
thanks a lot
```

---
## \#1086 Posted by: adrianlee Posted at: 2018-03-28T12:48:01.273Z Reads: 257

```
For receiver you just need arduino nano and the same 2.4ghz transceiver module as in the remote
```

---
## \#1087 Posted by: SeeTheBridges Posted at: 2018-03-28T14:13:23.540Z Reads: 256

```
For some people, the receiver currently has an issue where the arduino will freeze as soon as you turn it on. When you press the reset button, it fixes itself. Myself and Ervinelin have been attempting to fix the need to press the reset button every time you turn a board on. I've had success with a small ceramic capacitor but apparently it's not a consistent fix. There's another potential fix that I haven't tested yet but that I have the components for. That being low ESR electrolytic capacitors. Basically, it's a crap shoot right now. It either just works for you, or you're fighting with it to initialize properly.
```

---
## \#1088 Posted by: Zyb Posted at: 2018-03-28T14:15:31.932Z Reads: 243

```
What happened with capacitor fix? Did it fail at some point?
```

---
## \#1089 Posted by: webst Posted at: 2018-03-28T14:27:21.329Z Reads: 245

```
[quote="Zyb, post:1088, topic:28543, full:true"]
What happened with capacitor fix? Did it fail at some point?
[/quote]

Try reading the post above yours.
```

---
## \#1090 Posted by: Zyb Posted at: 2018-03-28T14:52:36.952Z Reads: 250

```
I can read only below
```

---
## \#1091 Posted by: Zyb Posted at: 2018-03-28T14:56:06.482Z Reads: 254

```
Did you try another cap? My 0.68uf seems to work fine for now

interesting fact, i had a spare new arduino nano, uploaded ino file and fired it up using 220uf cap  on 5v line and it seems to work on every boot because rx light flashes rapidly. now im confused.
```

---
## \#1092 Posted by: SeeTheBridges Posted at: 2018-03-28T15:41:12.146Z Reads: 255

```
I broke my Pulse Echo again and it's been raining so I haven't had the chance to field test. Just testing it in my room has been working fine though
```

---
## \#1093 Posted by: mlp Posted at: 2018-03-28T16:52:17.224Z Reads: 246

```
Could a Microcontroller Supervisory Circuit be a more stable fix?
Check out pitrs33’s posts on the Arduino Due forum. 

Forum: https://forum.arduino.cc/index.php?topic=256771.30

PDF: http://ww1.microchip.com/downloads/en/DeviceDoc/11184d.pdf
```

---
## \#1094 Posted by: Zyb Posted at: 2018-03-28T18:21:12.584Z Reads: 249

```
from datasheet ''Holds microcontroller in reset until supply voltage
reaches stable operating level'' looks like just what we need. 
this is also a good reference for Low ESR caps https://docs.google.com/spreadsheets/d/14M4Z0GPJp3u7L3bmYBizHm3Leg0XOCmAWQOx_wEgEng/edit#gid=1538665578
```

---
## \#1095 Posted by: SeeTheBridges Posted at: 2018-03-28T18:24:14.096Z Reads: 249

```
My only issue with it is cost. That transistor is 46c it looks like.
https://www.digikey.com/product-detail/en/microchip-technology/MCP120T-300I-TT/MCP120T-300I-TTCT-ND/275287

The small ceramic cap that's working for me so far is ~8c.
```

---
## \#1096 Posted by: Zyb Posted at: 2018-03-28T18:27:59.794Z Reads: 261

```
this guy in the forum is talking about the possible damage to reset switch over time and how to get around it. 

''My solution might be better then directly connecting a 10 µF ceramic or tantalum capacitor to the reset switch. That will damage the switch over time and is a risk for the clamp diodes in the microcontrollers.

I connected a 10 µF electrolytic capacitor (ceramic or tantalum should also work) with a 470 Ohm resistor in series between the reset pin and ground. This will delay the startup of the SAM by around 150 ms, as you can see below. The current through the reset switch (and maybe other parts) is limited to 7 mA by the resistor, so nothing can be damaged.''
```

---
## \#1097 Posted by: mmaner Posted at: 2018-03-28T19:07:58.330Z Reads: 254

```
Is anyone building these and selling them yet?
```

---
## \#1098 Posted by: SeeTheBridges Posted at: 2018-03-28T19:32:57.673Z Reads: 256

```
I've got a box of parts for a short run of 10 remote/receiver pairs to sell, but I'm not gonna start that run until I have my receiver issues ironed out.
```

---
## \#1099 Posted by: Twinsen Posted at: 2018-03-28T20:58:24.127Z Reads: 263

```
I made my own remix based on solidgeek’s code and ervinelin’s 3D files, with my own simplified schematic.

I posted about it here: https://www.electric-skateboard.builders/t/twinsens-3d-printed-nrf-remote/50482

At the moment it no longer sends VESC telemetry since I have no way to test it, but maybe someone can look at putting it in. It should be quite trivial except for the fact that I managed to fill the entire program memory :D
```

---
## \#1100 Posted by: DjamboBuksne Posted at: 2018-04-02T13:13:17.402Z Reads: 255

```
Where can I cat the latest software and wireing diagrams?
```

---
## \#1101 Posted by: Zyb Posted at: 2018-04-02T14:16:29.665Z Reads: 261

```
im building a new receiver and did some unscientific test. uploaded the .ino file to arduino and fired it up 10 times in a row using 5v-GND line and booted up without a problem. then i introduced the wireless module and tried to boot it up from the same power source using the same pins and never booted correctly, needing a reset everytime. i got my hands on a low ESR cap going to connect it and see what happens.
```

---
## \#1102 Posted by: DjamboBuksne Posted at: 2018-04-02T14:43:05.489Z Reads: 271

```
Done!

![20180402_164022|666x500](upload://5xH0f7sSquj26ZsO1hAHzdikvBO.jpg)


![20180402_164032(0)|666x500](upload://haYRyIJTdA2yNEqXxDzc5Ath0Yl.jpg)
```

---
## \#1103 Posted by: DjamboBuksne Posted at: 2018-04-03T08:35:06.890Z Reads: 263

```
When I accelerate or brake, the line on the display is a bit laggy.
```

---
## \#1104 Posted by: DjamboBuksne Posted at: 2018-04-03T08:36:15.341Z Reads: 259

```
I can do that if @solidgeek is okay with it
```

---
## \#1105 Posted by: webst Posted at: 2018-04-03T08:38:00.974Z Reads: 256

```
The secret is not to accelerate or brake!
```

---
## \#1106 Posted by: Deakbannok Posted at: 2018-04-05T01:07:53.980Z Reads: 265

```
Another tip for everyone
Get a small JST connectors is less soldering work you have to do and is more easier to disconnect the wires and swap components. 

http://i65.tinypic.com/2j3jsk9.jpg
```

---
## \#1107 Posted by: Zyb Posted at: 2018-04-05T16:40:40.642Z Reads: 262

```
i found this part in aliexpress its practically a combination of tp4056 and 5v boost converter board. it also has a place for power key. size wise its 4mm longer than tp4056 rest is around the same.
https://www.aliexpress.com/item/DC-5V-2-1A-USP-Mobile-Power-Diy-Board-4-2V-Charge-Discharger-boost-battery-protection/32824032545.html?spm=2114.search0204.3.1.6ef04383PGgppp&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10151_10065_10344_10068_5722815_10342_10343_10340_5722915_10341_5722615_10697_10696_10084_10083_10618_10304_10307_10302_5722715_10059_10534_308_100031_10103_441_10624_10623_10622_5722515_10621_10620,searchweb201603_25,ppcSwitch_7_ppcChannel&algo_expid=61870233-7824-404c-82e5-bc8a93e01893-0&algo_pvid=61870233-7824-404c-82e5-bc8a93e01893&priceBeautifyAB=0
![jpg_640x640|500x500](upload://wuI8Gc4fIYyQiLQVaXszKzPcdU8.jpg)
```

---
## \#1108 Posted by: PI3RR3 Posted at: 2018-04-05T18:43:06.592Z Reads: 257

```
Hey this thing is awesome. I have 2 Bluefruit Feather nRF52 boards and I want to use them as remote/receiver.
You're build is very impressive !! I have a couple of questions if you don't mind:
* what is the remote battery and how long does it last?
* how reliable is the communication between your remote and your receiver?
* do you think bluefruit feather can do the job ?
* And do you have a schematic of the circuit ?
thanks in advance !!
```

---
## \#1109 Posted by: chinzw Posted at: 2018-04-05T20:00:53.104Z Reads: 241

```
Im reimplementing an nrf52 version of this, using bluetooth instead of RF as RF on the nrf52 is quite hard to implement and not supported in the libraries.
```

---
## \#1110 Posted by: PI3RR3 Posted at: 2018-04-05T20:05:42.290Z Reads: 240

```
I don't mind having to write some extra code. I know the bluefruit library can handle UART communication through BLE so it should be ok. 

Can you share what you have if you manage to make it work ?
```

---
## \#1111 Posted by: chinzw Posted at: 2018-04-05T20:12:29.358Z Reads: 238

```
All the libs are different as the processor is in the nrf52 module. I had to rewrte all the ui code and im designing a much simpler version of the code for my use, no fancy stuff, just pwm and nothing else.
```

---
## \#1112 Posted by: wafflejock Posted at: 2018-04-05T20:18:21.356Z Reads: 235

```
Can see in the first pic it's a 400mAh battery he's using.  I have my own DIY variant arduino 8Mhz/nrf24l01 based  uses around 20mA typically from what I've seen (using 800mAh in mine... it has more free space).  Have left it on over night and still had charge when I realized I had left it on.  Regarding 'bluefruit' or any other development board it should be fine the only thing going on here that is 'computationally expensive' is running the display (other work is read the position of knob or hall sensor and pass along info to wireless radio to handle sending it out)
```

---
## \#1113 Posted by: PI3RR3 Posted at: 2018-04-05T20:19:50.414Z Reads: 234

```
By the way, why is the hall sensor for? What does it do? Why is it needed?
```

---
## \#1114 Posted by: webst Posted at: 2018-04-05T20:20:17.545Z Reads: 232

```
It acts as contactless potentiometer
```

---
## \#1115 Posted by: PI3RR3 Posted at: 2018-04-05T20:46:49.364Z Reads: 238

```
can you elaborate on that? what is the role?
```

---
## \#1116 Posted by: wafflejock Posted at: 2018-04-05T20:54:09.826Z Reads: 246

```
A hall sensor tells you essentially how close a magnet is if you put a magnet in the wheel or on whatever part is moving towards/away from the hall sensor you can read that value (much like reading the value of a potentiometer turning).  It is the 'input' that the MCU will read for position of the trigger/wheel.

There are some hall sensors that have a "schmitt trigger" so they only signal when a magnet passes some threshold (good for things like a door that might bounce up and down as it closes so you only want to call it 'closed' when one threshold is met and only want to call it 'open' when another is met but want it to ignore any bouncing while closing).  What you'd want in this case is a linear hall effect sensor so you can see the variable output based on the variable distance of the magnet instead of just a full on or full off type of signal.
```

---
## \#1117 Posted by: PI3RR3 Posted at: 2018-04-05T21:04:29.461Z Reads: 234

```
Thanks for these precisions, so the hall sensor is for the input (acceleration/decelaration) ?
```

---
## \#1118 Posted by: wafflejock Posted at: 2018-04-05T21:07:25.334Z Reads: 237

```
yup ultimately that signal gets read by something in the controller (MCU of some sort) and passed along to the transmitter circuitry/chips which broadcasts over an antenna then the receiver on the board connected to the ESC gets that signal and passes it along to the ESC which ultimately controls the throttle.
```

---
## \#1119 Posted by: Jcullinan09 Posted at: 2018-04-05T23:46:20.225Z Reads: 231

```
Can we pin the actual schematic for this build somewhere at the top, I literally cant find it.
```

---
## \#1120 Posted by: Clonkex Posted at: 2018-04-06T00:00:50.243Z Reads: 238

```
[quote="Jcullinan09, post:1119, topic:28543"]
I literally cant find it.
[/quote]

Come on, there's only >1000 messages.... ;P
```

---
## \#1121 Posted by: Jcullinan09 Posted at: 2018-04-06T00:20:25.512Z Reads: 241

```
I know it exists because I have seen the one legit schematic but I cant remember what post it was UGHHH
```

---
## \#1122 Posted by: Zyb Posted at: 2018-04-06T00:23:18.069Z Reads: 237

```
its all in the first post no need to dig https://github.com/SolidGeek/nRF24-Esk8-Remote/wiki/2.-Electronics

just ignore the status led part, rest is correct.
```

---
## \#1123 Posted by: Jcullinan09 Posted at: 2018-04-06T00:48:15.549Z Reads: 233

```
Thanks @Zyb
```

---
## \#1124 Posted by: deltazeta Posted at: 2018-04-06T05:26:59.121Z Reads: 236

```
I know there has been mention of this working with vesc 6, but I wanted to clarify if that meant this will work with the nrf chip built on the vesc 6, or if it will still need a separate receiver?
```

---
## \#1125 Posted by: Clonkex Posted at: 2018-04-06T05:34:03.399Z Reads: 240

```
It needs a separate receiver. If it used the NRF receiver on the VESC you'd have to upload a custom firmware, and I don't know of any hardware that is able to make use of the built in NRF receiver.
```

---
## \#1126 Posted by: deltazeta Posted at: 2018-04-06T05:52:58.790Z Reads: 244

```
that's a shame, what's the nrf even used for then? there's an nrf tab in the vesc tool.
```

---
## \#1127 Posted by: Clonkex Posted at: 2018-04-06T06:09:37.505Z Reads: 247

```
I think currently nothing. I might be wrong but as far as I'm aware it's just there for potential future uses but currently does nothing.
```

---
## \#1128 Posted by: Migro Posted at: 2018-04-06T06:31:45.458Z Reads: 259

```
I've stitched the two pics together some where up there. But here it is:![image|690x259](upload://8SJWG7FjylVFYNKaJrMEWjq0BXM.png)

But people has started to put on a small cap somewhere havent really been looking into that part yet. But someone would probably be able to help you with that.
```

---
## \#1129 Posted by: solidgeek Posted at: 2018-04-06T07:04:31.255Z Reads: 266

```
I am currently making New documentation for the remote, here is a better schematic: 

https://solidgeek.dk/wp-content/uploads/2018/03/schematic-4.png
```

---
## \#1130 Posted by: moon Posted at: 2018-04-07T15:26:20.375Z Reads: 266

```
![IMG_20180407_162359|375x500](upload://4WnOX0nfUiYWVSkmL2FOjiBlkcp.jpg)![IMG_20180407_162432|375x500](upload://57F0HBbFV7GfFd9BJJlwRuivibb.jpg)
```

---
## \#1131 Posted by: Charles_Chan Posted at: 2018-04-08T14:10:35.910Z Reads: 249

```
Is anyone know why the signal of receiver send is 20ms one cycle?
```

---
## \#1132 Posted by: wafflejock Posted at: 2018-04-08T14:19:44.944Z Reads: 254

```
Seems it's somewhat arbitrary but is the value baked into the servo library https://forum.arduino.cc/index.php?topic=107964.0
```

---
## \#1133 Posted by: Shippo Posted at: 2018-04-08T19:22:22.862Z Reads: 274

```
Hi, @solidgeek thanks for your sharing and I really love your remote. I'm using 12s2p battery and Torque VESC. Currently I can connect the remote and the receiver, but in the BLDC tool the pulsewidth is very unstable, everytime I roll the throttle to max and min, the value shows in the BLDC tool is different and delay, depends how fast I roll the throttle. I can not get the real time data dispalyed on the remote as well. Here's some pics and how I wired the receiver. I chose " PPM and UART " in BLDC tool.
![IMG_4236|666x500](upload://eSDCr0dtAY0MMyD8RIXuylDTNpj.JPG)![IMG_4235|666x500](upload://qXPz3E70oiwcnLpwNM3kvuOJles.JPG)![IMG_4237|666x500](upload://34b7Ox0ciwbffI1TfhVYV6TG0kK.JPG)!
[IMG_4240|666x500](upload://7Fu8i0ecD584lTazjccepLdGxkj.JPG)!
![IMG_4240|666x500](upload://7Fu8i0ecD584lTazjccepLdGxkj.JPG)
![IMG_4239|666x500](upload://uO08NpC7MHxPrOfYNwcupXLyLKZ.JPG)

I paralleled connected 330uf cap between 5v and GND, also between 3.3v and GND on NRF24L01 (100uf and 4.7uf).
There's an error message when I uploaded the code using RollingGecko's vestuart.h library, although I was able to upload it successfully. 
![擷取|690x442](upload://tlRQoUJ7Yv3fTYchXTC7rFr1ZRL.JPG)
Could you tell me any possibilities that may cause the pulsewidth problem?
By the way, the pattern of battery level on the remote keeps changing with the throttle all the time.
```

---
## \#1134 Posted by: Deakbannok Posted at: 2018-04-08T20:25:25.430Z Reads: 256

```
Use the latest version
https://github.com/RollingGecko/VescUartControl/tree/VESC6
```

---
## \#1135 Posted by: deltazeta Posted at: 2018-04-08T20:28:02.921Z Reads: 252

```
Have you guys encountered SERIALIO not declared in the arduino ide? I've got the nrf24 library and rollinggecko's vescuartcontrol for vesc6.
```

---
## \#1136 Posted by: Deakbannok Posted at: 2018-04-08T20:51:05.032Z Reads: 259

```
![Untitled|690x388](upload://AapZdHBdWoxj2SuLt7Cci9aFGJU.jpg)
```

---
## \#1137 Posted by: solidgeek Posted at: 2018-04-08T20:52:25.077Z Reads: 252

```
Glad you like the remote! Which version of the software are you using? I recommend you try my newest development branch on github, includes lot if bug fixes
```

---
## \#1138 Posted by: deltazeta Posted at: 2018-04-08T20:55:03.284Z Reads: 241

```
cmon man, I did that, I just wanted to know how people specifically dealt with it for this use case. Especially if you actually tried that yourself and saw relevant posts were from 2016 and anything more recent is just code.
```

---
## \#1139 Posted by: Shippo Posted at: 2018-04-08T20:57:54.994Z Reads: 242

```
Hi, I used this one and uploaded it successfully. But still showed an error message in the picture I posted. Don't know if that affects anything.
```

---
## \#1140 Posted by: Deakbannok Posted at: 2018-04-08T21:01:52.474Z Reads: 248

```
@deltazeta :) Yes but is fixable

@Shippo Use the codes under the development branch.
```

---
## \#1141 Posted by: deltazeta Posted at: 2018-04-08T21:06:00.955Z Reads: 244

```
that's why i'm asking??? I don't know what your point is, you could have just replied with how you solved it.
```

---
## \#1142 Posted by: Shippo Posted at: 2018-04-08T21:12:33.346Z Reads: 255

```
Thanks for your reply. Is this one the latest version?
https://github.com/SolidGeek/nRF24-Esk8-Remote

Do I have to set anything in the remote setting to show up the real time data?
I selected  "PPM and UART " in BLDC tool and let anything else default. Is that correct?
I was thinking the receiver can't receive the data instantly cause the max pulse width shows in the BLDC tool are really different everytime. I'm not sure how I can fix that. 
Thank you.
```

---
## \#1143 Posted by: Shippo Posted at: 2018-04-08T21:20:28.950Z Reads: 251

```
Are you talking about this one?
https://github.com/RollingGecko/ArduBoardControler

Thanks.
```

---
## \#1144 Posted by: deltazeta Posted at: 2018-04-08T21:26:40.812Z Reads: 254

```
i think they're talking about this one:
https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development
```

---
## \#1145 Posted by: Deakbannok Posted at: 2018-04-08T21:48:01.409Z Reads: 247

```
@deltazeta Yes that is the one. the latest update
```

---
## \#1146 Posted by: thetechtrader Posted at: 2018-04-09T16:29:16.126Z Reads: 249

```
Hey guys, what is your experience with remote controls still working if the receiver is in an aluminum case under the board? do you still get a signal or does that cause issues VS receiver in waterproof plastic container?
```

---
## \#1147 Posted by: Jcullinan09 Posted at: 2018-04-13T22:35:34.460Z Reads: 244

```
Im late to making one of these builds, but holy shit is the nrf module hard to solder. How did you guys manage to solder that thing. Im using 30AWG wire and its still a bitch.:sweat_smile:
```

---
## \#1148 Posted by: Deakbannok Posted at: 2018-04-14T15:19:11.658Z Reads: 256

```
steady  hands and a clean tip hotiron. nrf is not that bad.. try soldering wires to micro usb :slight_smile: 

![20180414_171504|281x500](upload://y9AqzIme7LNNWsjBMxP8mEYJnIW.jpg)
```

---
## \#1149 Posted by: GrecoMan Posted at: 2018-04-14T20:59:49.368Z Reads: 239

```
i soldered 22awg to one of those fuckers once
```

---
## \#1150 Posted by: Tathers Posted at: 2018-04-15T04:02:38.216Z Reads: 251

```
![image|375x500](upload://6lBaEiBq3VEl4LVMEXpbpM8tmvB.jpeg)
```

---
## \#1151 Posted by: landonkun Posted at: 2018-04-15T08:29:10.463Z Reads: 241

```
Ooo, do I spy an Eva-themed remote? ;)
```

---
## \#1152 Posted by: Tathers Posted at: 2018-04-15T08:40:10.681Z Reads: 243

```
To go along with my "01" board ;)
```

---
## \#1153 Posted by: Jcullinan09 Posted at: 2018-04-16T00:59:12.252Z Reads: 246

```
Does anybody have a guide that I could follow on how to put the arduino code onto the nano chip? I'm somewhat lost, and keep getting the following error message. I have included RollingGeckos .zip library.![03 PM|690x372](upload://zhaEOke3A2rKq2so3Kf0PKqBhKH.png)
```

---
## \#1154 Posted by: deltazeta Posted at: 2018-04-16T01:06:02.112Z Reads: 231

```
I'm not really aware of any guides per se, but you're gonna want to change the board type to Arduino Nano. The ide thinks you're using an Arduino Uno instead.
```

---
## \#1155 Posted by: Jcullinan09 Posted at: 2018-04-16T01:15:32.543Z Reads: 240

```
I played around with it and managed to adjust the ide to Arduino Nano. But man that compiling error still exists. Do you think there is some kind of Compiler I need to download in addition to the ide? 
I appreciate the help. ![37 PM|690x122](upload://uVcksHEbzsRWTdPnUziRJLyuZ4O.png)
```

---
## \#1156 Posted by: deltazeta Posted at: 2018-04-16T01:23:33.977Z Reads: 227

```
Besides libraries, the ide has everything you need to build for the nano.

The error message is somewhere in there. Expand the output area so you can see it. Probably missing a library or something is my guess.
```

---
## \#1157 Posted by: Jcullinan09 Posted at: 2018-04-16T01:28:05.023Z Reads: 234

```
Aha! You are correct, it was indeed missing a directory..? Should I try and start from scratch or is this a simple thing I missed including somewhere.
![22 PM|690x86](upload://eQxCBGwbgG0xu7bjd4Ifz98xa12.png)
```

---
## \#1158 Posted by: Jcullinan09 Posted at: 2018-04-16T01:56:13.658Z Reads: 233

```
Yeah so I re-downloaded everyting including: the arduino ide, Both rollingGecko's .zip library, and Solidgeeks ino, and I have the same fatal error... 

I'm sorry for being a noob, with the noobiest software such as arduino's but I do not know what I am doing wrong.
```

---
## \#1159 Posted by: Scoo_B_SK8 Posted at: 2018-04-16T03:59:29.824Z Reads: 235

```
you need to download/install that library "U8g2lib"

further more check to see if nano has Ch340 on bottomside this would mean its a china clone(ebay) and would need to download/install the "ch340 driver"

could also try and just run the "blink" script on the nano and see if onboard led blinks. if it blinks your all good, if not do the above ch340
```

---
## \#1160 Posted by: Jcullinan09 Posted at: 2018-04-16T04:06:03.903Z Reads: 235

```
Hey, Thank you for responding. I do not know where to get that specific library. Is it as simple as googling it from the internet? 

I also do not see the print Ch340 on the bottom of the nano, and I'm not quite sure how to run a blink script, but when I connect the micro USB to the nano it does blink. 

Any thoughts?
```

---
## \#1161 Posted by: Scoo_B_SK8 Posted at: 2018-04-16T04:18:03.672Z Reads: 238

```
3 ways ...

1) in Arduino IDE
>Sketch (tab)
   >include library (tab)
      >Manage libraries
            -use filter/search bar "u8g2lib"
            -click on it and hit install

2) google,download .zip file and...
in Arduino IDE
>Sketch (tab)
   >include library (tab)
     -add .ZIP library (tab)
     - follow to where you downloaded it to

3) google,download .zip file and copy & paste to arduino libraries folder


always good practice to restart IDE after install
```

---
## \#1162 Posted by: Jcullinan09 Posted at: 2018-04-16T04:19:37.191Z Reads: 219

```
I am going to work now! Thank you so much!
```

---
## \#1163 Posted by: Jcullinan09 Posted at: 2018-04-16T05:11:46.327Z Reads: 229

```
Okay I got to a point where I believe I have downloaded all the necessary libraries. Now when I tried to upload the code, I think my computer and the board cannot talk to one another as I have been stopped at this pop-up.

Could "COM1" be something that my mac needs to know about the serial address in order for the nano and mac to shake hands?

![27 AM|690x85](upload://5bZPPtEg9dkpqFPs7axtf59J3LT.png)

I'm sorry I'm having to trouble this forum with questions, but I haven't found answers or a guide on how to set this up elsewhere.
```

---
## \#1164 Posted by: Zyb Posted at: 2018-04-16T10:55:23.578Z Reads: 228

```
i had the same problem after updating some files which poped up in arduino ide software. dont click on that ''update boards..'' message. now i cant use my main computer for this reason. i installed everything fresh on my old laptop and it works fine. so my suggestion would be to try another computer and dont update anything except for the library updates.
```

---
## \#1165 Posted by: Scoo_B_SK8 Posted at: 2018-04-16T12:10:51.002Z Reads: 228

```
in Arduino IDE 
-tools tab
-port tab

select "COM" (in your case looks like COM1)
```

---
## \#1166 Posted by: Jcullinan09 Posted at: 2018-04-16T22:57:12.031Z Reads: 233

```
I see what you are suggesting.

How do I find the "COM" or "COM1" in the IDE if it doesn't show up after selecting tools tab > port tab > 

So far it just shows me a list of previous bluetooth devices I've connected my Mac to.
```

---
## \#1167 Posted by: Scoo_B_SK8 Posted at: 2018-04-16T23:37:18.611Z Reads: 243

```
https://www.youtube.com/watch?v=Ix4t-_RZ7NI



be sure YOU @Jcullinan09  get the MAC driver version
```

---
## \#1168 Posted by: Jcullinan09 Posted at: 2018-04-17T02:01:35.673Z Reads: 247

```
Well that fixed the port problem. Now it tried to sync 10 times, and failed.

Do you know what this command window prompt means?  ![53 PM|690x325](upload://cE8Sz2zcrkqVO1CsmPuxxBcHPRx.png)
```

---
## \#1169 Posted by: Scoo_B_SK8 Posted at: 2018-04-17T04:11:38.575Z Reads: 237

```
you sure you have "nano" selected under >boards

EDIT: you sure you want to build a remote?... might be less trouble/time/$ for you to just purchase one.
```

---
## \#1170 Posted by: Deakbannok Posted at: 2018-04-17T13:07:04.840Z Reads: 228

```
How many of you here already for a crash test PID cruise control? I need a feedback. Solidgeek came up with the formula for PID. we just need a right formula numbers of PID l.
```

---
## \#1171 Posted by: Jcullinan09 Posted at: 2018-04-17T13:08:40.034Z Reads: 234

```
Yeah, I did everything we talked through, and the steps followed in this forum.

I do want to build one! Coding is just not my strong-suit (clearly).

EDIT: I wouldn't need help if somebody else had already put a guide or steps on how to do this, however nobody has. But if you don't want to help me, and want me to struggle to learn how to do this, I will. I appreciate your help so far.
```

---
## \#1172 Posted by: Scoo_B_SK8 Posted at: 2018-04-17T15:53:03.115Z Reads: 221

```
all good.  just keep pluggin away at it, any "error messages" you get just type that into "GOOGLE", should get some hits.  I'm not fluent with MAC/OS, but the IDE should be the same.
```

---
## \#1173 Posted by: PeterMcKane Posted at: 2018-04-18T01:17:53.874Z Reads: 215

```
Is anyone selling a finished remote?
```

---
## \#1174 Posted by: Tathers Posted at: 2018-04-18T02:40:31.551Z Reads: 218

```
@SeeTheBridges is in the process of making multiple but I'm not too sure when he's selling.
```

---
## \#1175 Posted by: solidgeek Posted at: 2018-04-18T21:30:46.706Z Reads: 231

```
For those of you who have a startup problem with the receiver, have you thought about making a startup delay with a 555 timer circuit? The startup problem is caused by voltage spikes coming from the VESC, so to delay the startup of the receiver should fix this. 

Give this a look: http://www.learningaboutelectronics.com/Articles/555-timer-delay-before-turn-on-circuit.php 

I will try this out myself soon.

@Deakbannok I have abandoned the PID cruise control, the sampling rate just isn't fast enough, and tweaking the numbers don't seem to do the trick. The "UART only" mode, however, works great with cruise control, since it utilizes the VESCs internal PID control.
```

---
## \#1176 Posted by: Pedrodemio Posted at: 2018-04-18T23:57:24.073Z Reads: 226

```
I had some similar problem on my old board using arduino, first I had to make an RC filter on the 5V line, but the turn on problem I solved by just adding delay as the first thing on the setup, 8 seconds did the trick back them
```

---
## \#1177 Posted by: deltazeta Posted at: 2018-04-19T00:00:22.368Z Reads: 232

```
Does this mean cruise control is coming soon :grinning:
```

---
## \#1178 Posted by: SeeTheBridges Posted at: 2018-04-19T02:28:20.989Z Reads: 232

```
I've been riding with my tiny cap for a couple weeks now and its still running fine... I think this may be the fix we needed. A 555 Timer could work for people without huge space constraints though?
```

---
## \#1179 Posted by: ervinelin Posted at: 2018-04-19T05:38:18.587Z Reads: 227

```
I run an LC filter + 1000uF cap on the 5V line, that helps with the startup problem.

In addition to that, I add a 220uF cap between the reset and ground pins, that solves all problems with having to do a hard reset to get the Rx (or Tx) going.

Not sure if the cap is the best idea but so far it works.
```

---
## \#1180 Posted by: deltazeta Posted at: 2018-04-19T17:37:38.034Z Reads: 218

```
Anyone got some extra parts? The spring, power switch, magnets, and hall sensor are stuck in customs sorting and I'm not sure I'll even get those parts.
```

---
## \#1181 Posted by: Deakbannok Posted at: 2018-04-20T10:36:13.554Z Reads: 235

```
@solidgeek Oversaw that problem. I added 
if (UartUpdated){
    err = ((returnData.rpm)-rpm_set);
    err_T+=err;
    throttle_adjustment = ((Kp*err) + (Ki*err_T) + (Kd*(err - err_P)));
    err_P = err;
  }
Just to cal when there is a new simple udpated. Is still slow but it working out little smoother.
Also and added the band zone between 15 range. So you dont get a jump throttle when the adjustment and throttle is  15 or less different.

Just need more tester.
If anyone is interesting testing this Cruise Controller.?
```

---
## \#1182 Posted by: Deakbannok Posted at: 2018-04-20T22:59:41.151Z Reads: 234

```
is been out for awhile :wink: we r testing them.
```

---
## \#1183 Posted by: Tig3rch3n Posted at: 2018-04-23T12:30:44.959Z Reads: 245

```
@solidgeek
Finally I got all parts and tossed them together on Saturday :slight_smile:
I took the pictures before I updated to the latest dev build.
But as I stepped through the diff, I noticed a additional Pin going to the Arduino called "chargeMeasurePin = A1;"
What was It intended for originally? And will it be reused or did you canceled that idea?

![20|690x388](upload://7cfql2XVqiDQO0HmevTtauteg53.jpg)![30|690x388](upload://koz0w5RDq0sI6Zx1sSJ2kLpbQX4.jpg)
```

---
## \#1184 Posted by: solidgeek Posted at: 2018-04-23T22:54:28.580Z Reads: 239

```
Looks good! The pin was planned to monitor if a charger is connected. This way I could show a big battery and procentage on the display while charging, however I choose not to as it seemed unnessecary as it would only work while the remote is turned on.
```

---
## \#1185 Posted by: HighMasterGogo Posted at: 2018-04-24T08:53:27.455Z Reads: 251

```
Finally got my remote working pretty much perfectly! The development branch basically fixed all the issues I was having with the hall sensor range/not registering the extremities. Thanks @solidgeek!

![IMG_1308|375x500](upload://h9NI1575uBdCRIBV0aDFTMsXIpU.jpg)

Just one question, apologies if it's been asked before, I did do a search but nothing came up; I can only set a maximum of 12 under motor poles but I believe mine has 14. Any ideas? Apologies if this is a dumb question!
```

---
## \#1186 Posted by: solidgeek Posted at: 2018-04-24T22:27:48.022Z Reads: 255

```
@HighMasterGogo Glad to see you got it working :-) ! Not a dump question at all. It seems that I have forgotten to change the maximum number of poles. Thanks for noticing!  I have updated the development branch again, and you should now be able to set a maximum of 250 poles (after reuploading the firmware).

Now to something a little more exiting! I have been working on a custom PCB for the receiver, to eliminate any receiver-related issues. It utilizes the Atmega32u4 as the microcontroller and a Pololu 300mA Buck converter to step down the unstable 5V to a better regulated 3.3V. So far I got a working prototype (still need to do a lot of testing), and I am planning to sell the receiver to anyone who is interested. 

 ![20180425_000810|281x500](upload://AjKZgX1nr2tYG5eDgxswNBt9PmV.jpg)

What do you think? :-)
```

---
## \#1187 Posted by: Surfer Posted at: 2018-04-25T05:51:44.895Z Reads: 235

```
I will want 2 receivers! 😁
```

---
## \#1188 Posted by: Tig3rch3n Posted at: 2018-04-25T10:21:42.590Z Reads: 240

```
I'll be in for 2-3 kits :slight_smile:
Got a Reflowoven here so i'll do the SMD stuff my selfe :stuck_out_tongue:

If You want I can help you assemble the boards, i'm living in Berlin, shouldn't be to long away from your place.
```

---
## \#1189 Posted by: SuperBen Posted at: 2018-04-25T15:07:19.396Z Reads: 241

```
If anyone has a complete kit (3d printed parts can be missing, I can always use 3dhubs for that) for sale I would definitely be interested. I wanna start ordering parts but if someone out there already did all the work and can send it all in one comfy package it would make my life much easier hahaha
```

---
## \#1190 Posted by: Tig3rch3n Posted at: 2018-04-25T20:46:05.979Z Reads: 245

```
Where are you from?
I'm from Berlin, Germany

I have 1 Display, 2 Arduino, 2 RF Chips, 8 Magnets, 2 Hall Sensors, 3 LiPo Charger, 15+ Microswitches, 10+ USB Micro Ports

So you need 1xBoost DC-DC Converter, 1x LiPo, Wire
```

---
## \#1191 Posted by: mrplaygood Posted at: 2018-04-25T21:13:25.776Z Reads: 246

```
I‘m in for 1 or 2 receivers. Just realized that my 3.3V Adafruit feather can‘t read the 5V UART of the VESC. That‘s why I have no readings on my remote :confused:
```

---
## \#1192 Posted by: Zyb Posted at: 2018-04-25T21:17:46.893Z Reads: 253

```
theres a part made just for that https://www.sparkfun.com/products/12009
```

---
## \#1193 Posted by: SuperBen Posted at: 2018-04-25T22:34:26.359Z Reads: 258

```
I'm located n California, USA :frowning:
```

---
## \#1194 Posted by: SeeTheBridges Posted at: 2018-04-26T00:39:35.944Z Reads: 260

```
Just gonna drop this here because I've been editing it all day to get it out before finals week 😴
https://youtu.be/OM7yJRaTvMQ
```

---
## \#1195 Posted by: mrplaygood Posted at: 2018-04-26T05:39:43.817Z Reads: 251

```
Thank you very much! Forgot about this possibility.
```

---
## \#1196 Posted by: webst Posted at: 2018-04-26T07:08:49.912Z Reads: 251

```
[quote="mrplaygood, post:1191, topic:28543"]
Just realized that my 3.3V Adafruit feather can‘t read the 5V UART of the VESC. That‘s why I have no readings on my remote :confused:
[/quote]

Let us know if it’s alive after receiving 5V on 3.3V inputs
```

---
## \#1197 Posted by: Deakbannok Posted at: 2018-04-26T07:16:32.457Z Reads: 238

```
On the UART connection. You have 3.3v and 5v pin.
```

---
## \#1198 Posted by: ervinelin Posted at: 2018-04-26T07:47:34.548Z Reads: 232

```
Please also sell just the populated PCB without the casing!

Also what's that HUGE cap for
```

---
## \#1199 Posted by: mrplaygood Posted at: 2018-04-26T08:08:05.878Z Reads: 230

```
The receiver works great but it does not send back the data of the VESC.
```

---
## \#1200 Posted by: mrplaygood Posted at: 2018-04-26T08:27:40.444Z Reads: 231

```
That‘s true but only for the power output. The logic is still 5V
```

---
## \#1201 Posted by: SuperBen Posted at: 2018-04-26T14:38:36.317Z Reads: 219

```
Nice glad you posted the second Part. Both of these segments were easy to follow and explained really well
```

---
## \#1202 Posted by: Tig3rch3n Posted at: 2018-04-26T20:13:56.150Z Reads: 231

```
Wuhu, first time Motor running via the Remote signals ;)
Can anyone post there Vesc settings for the remote?
And somehow I dont get Telemetry :(
```

---
## \#1203 Posted by: Deakbannok Posted at: 2018-04-26T22:53:21.197Z Reads: 229

```
@everyone  if you dont get the reading telemetry. check in the line 174: and remove that IF off for good
```

---
## \#1204 Posted by: Tig3rch3n Posted at: 2018-04-27T10:05:27.241Z Reads: 241

```
I'm not sure what you are talking about :frowning:
The latest Dev Build is:

Receiver
>172 	/* Begin listen for transmission */
>173 	while (radio.available() && !recievedData)
>174 	{
>175 		// Read and store the received package
>176 		radio.read( &remPackage, sizeof(remPackage) );
>177 		DEBUG_PRINT( "New package: '" + String(remPackage.type) + "-" + String(remPackage.throttle) + "-" + String(remPackage.trigger) + "'" );
>178     delay(10); 
>179     
>180 		if( remPackage.type <= 2 ){
>181 			timeoutTimer = millis();
>182 			recievedData = true;
>183 		}
>184 	}
>185 	/* End listen for transmission */

the only if that i can see is Line 180, so
>180 		if( remPackage.type <= 2 ){
turns into
>180 		( remPackage.type <= 2 ){

right?
```

---
## \#1205 Posted by: mrplaygood Posted at: 2018-04-27T13:14:13.696Z Reads: 227

```
OK, I think the problem is caused by my receiver board. I'm using an Adafruit feather m0 board which does not only not work with the second Serial but apparently it also does not have EEPROM so I can't use the new firmware. So right now it still works as a normal receiver with ppm to control the board but it does not work with other features. So before I buy a new board, how's about the boards from @solidgeek ? I would definitely buy one. But if it will take you some time maybe I buy an Arduino board first.
```

---
## \#1206 Posted by: Deakbannok Posted at: 2018-04-27T13:42:04.633Z Reads: 238

```
Under Development branch code.

>      if ( rxSettings.controlMode != 0 ) {
>         getUartData();
>         radio.writeAckPayload(1, &returnData, sizeof(returnData));
>       }

To...

 >  getUartData();
 >   radio.writeAckPayload(1, &returnData, sizeof(returnData));
```

---
## \#1207 Posted by: Becker33 Posted at: 2018-04-27T19:40:47.687Z Reads: 236

```
I'm considering building mine with a QI wireless charging receiver inside if it will fit. Something like this perhaps?

[Receiver module](https://www.amazon.co.uk/iPhone-Receiver-CHOETECH-Wireless-Charging/dp/B01L1WOKD8/ref=sr_1_2?s=electronics&ie=UTF8&qid=1524857719&sr=1-2&keywords=small+qi+receiver)

Any preconceptions?! :slight_smile:
```

---
## \#1208 Posted by: wafflejock Posted at: 2018-04-27T20:18:28.520Z Reads: 233

```
Think Qi charging is overkill for the remote they don't drain much power by themselves (mine doesn't have an oled but can't imagine that is taking much power and is only on when the controller is powered).  I literally hadn't used mine for a couple of months and it's still sitting at like 4V (1S battery) and when I am using it it runs about 20mA continuous current so with a 800mAh battery (or even smaller) you get a ton of on time too.  All that said don't see any reason it couldn't work.
```

---
## \#1209 Posted by: wafflejock Posted at: 2018-04-27T20:22:20.549Z Reads: 246

```
The NRF chip needs to occasionally draw far more amperage than the regulated power on a typical arduino can handle so it's recommended to have a capacitor to help maintain consistent voltage when there are moments of high current draw I'm pretty sure.... I did my own based on the nrf chip/breakout and the instructions I followed explain it further:

https://arduino-info.wikispaces.com/Nrf24L01-2.4GHz-HowTo

Guess is same deal here.
```

---
## \#1210 Posted by: Deakbannok Posted at: 2018-04-28T09:19:39.498Z Reads: 256

```
![20180428_020856|281x500](upload://ve8nEnL4GhgxbVJcPJXOnnidnrx.jpg)

Use JST a small connection wired them together. It is easier to swap the case or changing parts.
```

---
## \#1211 Posted by: MatwoSvK Posted at: 2018-04-29T01:37:04.060Z Reads: 248

```
Hi i just make my controler but i have a problem with get into settings , maybe cause when i even put magnet on hall sensor from one side is going all the way to max but from different polarity is missing like little piece of that bar, i try changing the numbers from 255 to even 200 but no difference , can anyone help me hot to change it to get into settings , and also when i plug turn both receiver and transmiter on display i still see is not connected , and i duno how to do it , if i need set something in vesc but i thing it should connect just when it turn on, i have these nrf24 https://www.aliexpress.com/item/SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in-stock-fast/32367254718.html?spm=a2g0s.9042311.0.0.otfQzv
thank you for any help.
```

---
## \#1212 Posted by: solidgeek Posted at: 2018-04-29T12:21:11.033Z Reads: 240

```
Which Hall sensor do you use?
```

---
## \#1213 Posted by: MatwoSvK Posted at: 2018-04-29T13:14:13.396Z Reads: 246

```
This one
https://www.aliexpress.com/item/SS495A-TO92-in-stock-can-pay/32624267215.html?spm=a2g0s.9042311.0.0.otfQzv&dp=2d0e8adaa6c308ba4ae590b2bd83e3ed&af=137322&cv=47843&afref=&mall_affr=pr3&aff_platform=aaf&cpt=1525007633418&sk=VnYZvQVf&aff_trace_key=ddd1b71dfa244dd1974cfd899607513b-1525007633418-00162-VnYZvQVf&terminal_id=dbd2ea436f8b460687ce1f15110655d0

but i mesure Voltage , in one polarity have 5V and another have around 90 mVolts
and middle without magnet have 2.550 V
```

---
## \#1214 Posted by: Deakbannok Posted at: 2018-04-29T14:37:01.538Z Reads: 240

```
Try to switching the mag around see you can get both polarity reading.
Check the wiring and use the code under development branch not master.
```

---
## \#1215 Posted by: MatwoSvK Posted at: 2018-04-29T15:00:42.333Z Reads: 244

```
i get readings of both but on one is going to full and on different polarity not going to full bar on display. So i cant get into settings
```

---
## \#1216 Posted by: Deakbannok Posted at: 2018-04-29T17:49:26.447Z Reads: 250

```
ah is common. is your hall sensor aligning right on the mags? ur mag aint strong enough. you need to drill through the mag holder on your thumb throttle and push the mags closer to the hall sensor.

modify the code to go into setting.. and calibrate your value from there.

if you have more question how to do join the discord.
```

---
## \#1217 Posted by: MatwoSvK Posted at: 2018-04-29T18:46:17.634Z Reads: 243

```
yea mag is not strong enough or hall sensor is bad, i talking about putting magnet right on top of hall sensor , not in remote wheel and is still not enough to get into settings so i need to change code ,but i dunno how.
```

---
## \#1218 Posted by: solidgeek Posted at: 2018-04-29T21:03:25.705Z Reads: 242

```
You dont need to change anything in the code. Use the development branch (on github) instead of the master, as it works much better. To enter the settings you need to hold the trigger (killswitch) while restarting the remote, then use the hall sensor (throttle) to navigate the settings menu.
```

---
## \#1219 Posted by: MatwoSvK Posted at: 2018-04-30T01:45:25.862Z Reads: 242

```
thank you, throttle working now ,
but i still have problem with connection to receiver , 
i see flashing connection logo all the time,
is there something how to pair remote to receiver, or i need set something in vesc tool, but i thing it should be connected even without vesc.
```

---
## \#1220 Posted by: Zyb Posted at: 2018-04-30T09:57:00.869Z Reads: 244

```
i had the same problem in the past, the one in the development branch didnt work for me so i switched to master version and connection was flawless and yes it should connect without vesc. i would suggest try master and development versions (uploading both receiver and transmitter) see if you get a connection. if not check your connections to the nano.
also i would like add i had very different experiences with the same nrf module. some work ok with great range some work intermittently. it could be my soldering job or lack of experience but if you search in google you will find similar problems.
```

---
## \#1221 Posted by: Deakbannok Posted at: 2018-04-30T17:52:29.738Z Reads: 256

```
![20180428_160220|281x500](upload://eGGHZahjHwcsrxusInOUnJtYjQm.jpg)

Here is my complete built unit.
```

---
## \#1222 Posted by: karatekidfpv Posted at: 2018-05-02T17:07:29.198Z Reads: 241

```
Is anybody willing to sell units?
```

---
## \#1223 Posted by: SeeTheBridges Posted at: 2018-05-02T18:18:50.123Z Reads: 239

```
I'll be selling a run of 10 remotes after finals week is over. I'll post details sometime next week once I'm moved out and back home
```

---
## \#1224 Posted by: karatekidfpv Posted at: 2018-05-03T05:58:01.724Z Reads: 248

```
Sweet, add me to the queue please and good luck with finals.
```

---
## \#1225 Posted by: Howardzinn Posted at: 2018-05-03T22:42:45.210Z Reads: 264

```
Hello guys. 
I need some help from your side. :frowning:
 I read the whole topic and found no solution

This is my remote from SolidGeek
![IMG_20180504_002508|375x500](upload://qjS8mxpTBvd5MC8OjqNPQxOeM9f.jpg)

and this is my reciever with VESC-X
 ![IMG_20180504_002422|666x500](upload://aObGlzhn8g8jBgrC51jBBsuZZOQ.jpg)

what I am doing wrong when I can not make any communication? 

This is my reciever connect
![IMG_20180504_002430|690x289](upload://s7ipJzpudaxYSui7Gg9RwwuSlf4.jpg)

and in the end this is my VESC settings (UART set to 115200 baud)
 ![1 |690x202](upload://2QYipgu0PqMUK5BHlpeQFag6KTZ.jpg)

some ideas? I tried to change the modules, add cap's or use newest version (transmitter+reciever) and did not help :penguin:
```

---
## \#1226 Posted by: Deakbannok Posted at: 2018-05-04T07:01:48.908Z Reads: 247

```
dang son.. @solidgeek u did this? 😆

Did you get no connection between TX RX or no link between RX to VESC? check you PM.
```

---
## \#1227 Posted by: Seikeau Posted at: 2018-05-04T07:24:02.402Z Reads: 243

```
I don't have much experience with this at all, but from the picture it seems you have connected RX where the FocBox says TX and vice versa.
```

---
## \#1228 Posted by: Howardzinn Posted at: 2018-05-04T07:42:47.549Z Reads: 250

```
@Deakbannok  Honestly it's not really from him but kind of intellectual property is really his :smile:
I have no link between Tx Rx and measuring don't tell me literally nothing :frowning: 

Now im trying to make some basic code to check VESC 

@Seikeau it's all right i think, where VESC say Tx (Transmit signal) you need to read it with arduino Rx (Receive signal)
```

---
## \#1229 Posted by: solodros Posted at: 2018-05-04T08:21:38.273Z Reads: 255

```
![QQ图片20180504161749|690x388](upload://A0Ag4okEF3m61OfrKJpKNHMPyIr.jpg)![IMG_20180504_154315|690x388](upload://6BI5oIJAmfxx1KQSOlCm2PxFbuz.jpg)
I tried to integrate the remote control module to a PCB, but the first boot OLED will be chaotic, it needs to disconnect many times to normal display. Can you help me?
```

---
## \#1230 Posted by: Howardzinn Posted at: 2018-05-04T08:40:20.467Z Reads: 251

```
@solodros Try to desolde the cap
```

---
## \#1231 Posted by: solidgeek Posted at: 2018-05-04T08:43:38.326Z Reads: 259

```
@Howardzinn You need to have the RX and TX connected, otherwise, you will not be getting any data. However the remote should connect to the receiver right away if you have soldered everything correctly, and uploaded the newest firmware.

@Deakbannok No my work is a little more organized :P

![img_20180314_181103750-2|690x388](upload://oTUSVy9sbwEKK94vFZR2OPhSNRp.jpg)

@solodros Did you remember to add pull-up resistors on the I2C line?
```

---
## \#1232 Posted by: Howardzinn Posted at: 2018-05-04T08:59:23.210Z Reads: 256

```
@solidgeek it's good point! I will try to measure the signals when connected RX TX. Thanks alot 

BTW the remote is many times desolder :smile: it will looks better i promise!
```

---
## \#1233 Posted by: solodros Posted at: 2018-05-04T09:09:29.720Z Reads: 261

```
![1|524x500](upload://xu2VWRf1EYrIzeycCchMs7HboFm.jpg)
This is the driving circuit of OLED. I doubt it is power supply. I plan to replace IC with IC of 5V1A and 3V3-800MA.
```

---
## \#1234 Posted by: solodros Posted at: 2018-05-04T09:12:10.771Z Reads: 243

```
[quote="Howardzinn, post:1230, topic:28543"]
Try to desolde the cap
[/quote]

My friend also made it, but he did not have these problems. I tried your advice.
```

---
## \#1235 Posted by: northern Posted at: 2018-05-06T04:23:49.541Z Reads: 238

```
Hey guys, I finally got around to building a remote but I'm having trouble with it freezing at start up. I have played around with commenting out lines to narrow down the source. Currently I am able to get it to boot by changing line 471 in the transmitToReceiver function from:
if ( radio.write( &remPackage, sizeof(remPackage) ) )
to:
if ( true )
I can't figure out how to solve this so any help would be great!
```

---
## \#1236 Posted by: Deakbannok Posted at: 2018-05-06T08:09:03.208Z Reads: 236

```
You dont want to chnange that line 471. that is what TX writing to RX.
freezing up like no starting screen?
```

---
## \#1237 Posted by: northern Posted at: 2018-05-06T15:01:14.711Z Reads: 238

```
Right, I was just trying to isolate what was causing the crash and it looks like any write command will do it. I can get the starting screen to load but it will lock up before the program draws the running screen on both yours and SolidGeek's software. I can also get into settings just fine but changing certain values will cause it to crash as well.

I also have tried different versions of the RF24 library without success.
```

---
## \#1238 Posted by: xilw3r Posted at: 2018-05-06T20:55:02.196Z Reads: 248

```
@solidgeek Hey man, are you using the newest VESC firmware from VESC tool? Which is, I suppose 3.xx ? I think I read that you are using a vesc 6, do you know if I can use RollingGecko's library with the newest 3.xx firmware and a 4.12 vesc ? 

I am planning to use Gecko's ArduBoardController in a simplified version, mainly just because your code looks really hard to understand for a non prgrammer like me. I will use no screen and only a single potentiometer, so I think GEcko's code wil be easier to adapt, or do you htink otherwise?

On the other hand I think @lox897 had a simmilar idea to use ArduBoardController codes but he ran into issues. https://www.electric-skateboard.builders/t/ultimate-vesc-controller-with-oled/21922/152 

Ok, so basically do you think a monkey like me could edit your code to run with a pot without much hassle :) ?

Edit: I also was considering to use @wafflejock 's code, but it seems to not use UART, but PWM instead? So, I am unsure if it can be used with a vesc at all..

Cheers
```

---
## \#1239 Posted by: wafflejock Posted at: 2018-05-06T21:14:09.769Z Reads: 262

```
Just to clarify mine does work with a vesc but the code runs on an Arduino pro mini that relays the radio signals on both sides and reads the potentiometer on the control side and writes out to a pin (pretty sure I used d5) to send signal to the vesc just like any other receiver (on the receiver side).  I used the 8MHz 3.3V to avoid low voltage issues with either the controller lipo or VESC BEC, the 8Mhz variant will work down to about 3.5V

![IMG_20180506_192027|666x500](upload://i0r9Qz4d6kzBN0QmnB55q9GEQF6.jpg)
```

---
## \#1240 Posted by: Scoo_B_SK8 Posted at: 2018-05-07T03:06:01.273Z Reads: 257

```
@wafflejock was about to ask if anyone had tried using the smaller “arduino pro mini” which is smaller in size compared to “nano”, even a step further I have 5 “arduino pro mini 3v” which has a solid 3v for nrf24 module... since everyone only buys in bulk around here was gonna do a run of 5 remotes.  My Nano build worked just fine, just wanted to experiment a bit, I’ve also sat on this pro mini 3v build for months...
Cases are made of;
-PETG 
-ABS
-PLA
-Hemp PLA

![image|375x500](upload://wHiSJHirPLd0TxjxeXSQe3CoNJS.jpeg)
```

---
## \#1241 Posted by: Deakbannok Posted at: 2018-05-07T06:24:02.951Z Reads: 244

```
use a basic master branch. see if your problem still existing.
```

---
## \#1242 Posted by: xilw3r Posted at: 2018-05-07T07:11:23.052Z Reads: 249

```


I dont see a problem adjusting your code to go with an Arduino nano for my purposes. So one question remains, in the vesc/bldc tool you set up the control through the PPM ? because I am either blind or vesc tool does not have a PWM control tab. Did not check the older bldc tool though.

I should probably just shut up and try doing something already :) . I would still primarily try to adapt old Gecko's code and see what happens.
```

---
## \#1243 Posted by: Charles_Chan Posted at: 2018-05-07T10:06:13.181Z Reads: 261

```
Hi Everyone 

After installed newest library, I still have the problem with real time data delay on the OLED display. Is there something wrong I made it? Can you help to share how to solve it? thanks

The link on below are the library that I used, and the ESC I used is VESC4. After installed the library, I roll the throttle to max and min, the value shows on OLED are delay every time.
https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development
https://github.com/RollingGecko/VescUartControl

Thanks
```

---
## \#1244 Posted by: wafflejock Posted at: 2018-05-07T13:46:12.390Z Reads: 262

```
Yeah it says ppm in the vesc interface but seems to work fine with pwm signal, I check it with one of those cheap jbtek oscilloscopes and looks like varying pulse width to me but after calibration works as intended.  Side note too just had my remote start drifting on values it was sending recently and seems to have been from a loose connection to the potentiometer in the remote so just something to look out for (behavior being you see data coming into the receiver but it doesn't line up with the trigger position).  Ideally would want it to pull the pin down to gnd so at worst it sends a brake signal instead of ever floating high and sending a full throttle signal.  Anyhow just saying make sure whatever code or setup you go with you test the hell out or everything with regard to pulling individual wires and seeing the behavior in case any connections between the nrf and Arduino or the Arduino and potentiometer or between Arduino and esc come loose, make sure your fail-safes work appropriately.

---

Also just to add I made some small adjustments to my code for carrying two data points and used basically the same hardware to replace a radio for my RC car with steering control and a regular hobby esc and it also works fine using the servo library for handling sending out the pulses.
```

---
## \#1245 Posted by: solodros Posted at: 2018-05-08T10:37:18.718Z Reads: 256

```
Finally, it worked properly![QQ图片20180508183637|690x388](upload://jaKXTGTDLKRiGFx8u2NpRs9giYl.jpg)
```

---
## \#1246 Posted by: northern Posted at: 2018-05-08T16:23:01.899Z Reads: 251

```
Still the same on the master branch
```

---
## \#1247 Posted by: mrplaygood Posted at: 2018-05-08T16:33:59.354Z Reads: 258

```
I've got a question. Since I still don't get the VESC readings sent to my Remote I have no clue anymore. Do I need the "old" BLDC Tool or can I also use the "new" VESC Tool?

I'm running a VESC 4.12 with Firmware 3.38. __Edit:__ Oh yeah, and I have tried the master and developer branch.

I would be really pleased if someone could help me. I guess it is a pretty dumb failure I did here but I don't see it :smiley:
```

---
## \#1248 Posted by: Howardzinn Posted at: 2018-05-08T17:15:51.140Z Reads: 274

```
I have same problems too :smiley:  

Try to load some simply program to try the comm like:

> #include <SPI.h>
> #include <nRF24L01.h>
> #include <RF24.h>
> RF24 radio(9, 10);
> const byte address[6] = "00001";
> void setup() {
>   radio.begin();
>   radio.openWritingPipe(address);
>   radio.setPALevel(RF24_PA_MIN);
>   radio.stopListening();
> }
> void loop() {
>   const char text[] = "Hello eBoard";
>   radio.write(&text, sizeof(text));
>   delay(1000);
> }

for **transmitter** (remote) and: 
> #include <SPI.h>
> #include <nRF24L01.h>
> #include <RF24.h>
> RF24 radio(9, 10); 
> const byte address[6] = "00001";
> void setup() {
>   Serial.begin(9600);
>   radio.begin();
>   radio.openReadingPipe(0, address);
>   radio.setPALevel(RF24_PA_MIN);
>   radio.startListening();
> }
> void loop() {
>   if (radio.available()) {
>     char text[32] = "";
>     radio.read(&text, sizeof(text));
>     Serial.println(text);
>   }
> }

to **reciever** 

but honestly I have problems too and can not come to them (try different modules etc.)

Edit: Now im buying these modules https://www.aliexpress.com/item/SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in-stock-fast/32367254718.html with ceramic antenna and maybe it will work propertly
```

---
## \#1249 Posted by: xilw3r Posted at: 2018-05-09T19:11:14.000Z Reads: 246

```
Has anyone seen this compiling error while using @RollingGecko 's library ?

C:\Users\Asus\Documents\Arduino\libraries\VescUartControl-VESC6\VescUart.cpp: In function 'int PackSendPayload(uint8_t*, int, int)':

C:\Users\Asus\Documents\Arduino\libraries\VescUartControl-VESC6\VescUart.cpp:188:21: warning: converting to non-pointer type 'uint8_t {aka unsigned char}' from NULL [-Wconversion-null]

  messageSend[count] = NULL;
```

---
## \#1250 Posted by: Deakbannok Posted at: 2018-05-10T09:04:53.160Z Reads: 242

```
@northern @Howardzinn You have no connection between your remote TX to receiver RX?
@mrplaygood  Make sure you have selected PPM and UART in the setting.
```

---
## \#1251 Posted by: Howardzinn Posted at: 2018-05-10T09:31:38.518Z Reads: 247

```
@Deakbannok Unfortunately, I do not have any connections between modules (remote+reciever). I tried other nrf modules but without result. When I try to upload a simple code to test the connectivity between nrf modules everything works and I send messages to each other (see 1239 post).
After uploading codes from SolidGeek, no communication takes place. :-( (tested on all Branch and with different version of library)

I have the newest focbox (VESC 4)
from my side i tried everything i can, last thing  what i can do is to buy module with ceramic antenna
```

---
## \#1252 Posted by: mrplaygood Posted at: 2018-05-10T11:00:45.940Z Reads: 239

```
Yeah, I already set everything up. PPM and Uart on the vesc with 115200 Baudrate and PPM on the Remote with the same Baudrate. I have really no clue. 
Is it easy to „break“ the UART Port on the Vesc? Maybe I did this unknowingly (if this is a word :smiley: ) 

Thank you for your help!
```

---
## \#1253 Posted by: northern Posted at: 2018-05-10T15:04:23.539Z Reads: 236

```
@Howardzinn @mrplaygood My issue turned out to be a faulty RF module, I actually had two bad ones. I could get the sample code to work but they would lock up when you threw a lot of data at them. Try a new nrf24 module or a different supplier.
```

---
## \#1254 Posted by: Howardzinn Posted at: 2018-05-10T15:56:06.863Z Reads: 236

```
@northern really? 
That would be a great news! I just ordered modules with a ceramic antenna.
If it works, it's great. Because my basic communication worked, I did not deal with the functionality of the modules.


Thank you very much :penguin:
```

---
## \#1255 Posted by: Zyb Posted at: 2018-05-10T17:07:34.823Z Reads: 248

```
In my experience those nrf modules with ceramic antennas are super unreliable. You may have a perfectly working one or semi working one. I have ditched all of these and gone with an external antenna one. Just waiting for it I hope it’s a better one. Just before giving up on your current module try a 10-20uf cap. solder it between 3.3v and ground pins. See if it makes a difference. Because according to some tests I found, those nrf modules can dip to 2.7v while working because the 3v3 line appears to be goin up and down with power demand.
I’m going to try to make it work by soldering 3 caps in parallel 100nf, 10uf, 100uf these are all goin in between 3v3 and gnd pins. And may be one 220uf to 5v line.
```

---
## \#1257 Posted by: Howardzinn Posted at: 2018-05-11T12:17:18.707Z Reads: 256

```
You are right, soldering capacitors softens the voltage drops. But it can be the main problem with making communication between modules. 
I have the 220uF between 5V and GND due to unstable voltage from VESC

and I will definitely try a small capacitor on the nrf module, but surely (sadly) it will not be a major problem :frowning:
```

---
## \#1258 Posted by: ervinelin Posted at: 2018-05-11T14:07:29.597Z Reads: 259

```
So I heard you like external antennas...

https://youtu.be/b6dGFBtb3PI
```

---
## \#1259 Posted by: Deakbannok Posted at: 2018-05-11T20:47:11.115Z Reads: 253

```
I use 100uf. it runs smoothly
```

---
## \#1260 Posted by: DougM Posted at: 2018-05-12T01:04:08.215Z Reads: 259

```
I have probably a dumb question.  I ordered up some of the parts for this build, and amongst them was the recommended Nano V3, but I can't get my Arduino environment to flash the sample Blink program via USB.  Do I need to do anything special?

Settings:
Board = Arduino Nano
Serial Port = (the port it showed up on)
Programmer = AVRISP mkII (the default)

Thanks
```

---
## \#1261 Posted by: SeeTheBridges Posted at: 2018-05-12T01:55:06.111Z Reads: 248

```
Do you have everything up to date? If so, you need to change the processor to "ATmega328p (Old Bootloader)" Otherwise the code won't upload
```

---
## \#1262 Posted by: DougM Posted at: 2018-05-12T03:27:15.178Z Reads: 247

```
@SeeTheBridges that worked!  Thanks so much.
```

---
## \#1263 Posted by: ggalisky Posted at: 2018-05-12T17:18:31.967Z Reads: 244

```
If I wanted to print and sell the parts for these remotes is there any interest? My 3D printers are sitting with no print jobs currently.
```

---
## \#1264 Posted by: chris.hunt Posted at: 2018-05-13T20:23:12.137Z Reads: 236

```
I'd be interested, have you built one of these already?
```

---
## \#1265 Posted by: ggalisky Posted at: 2018-05-13T20:31:05.602Z Reads: 243

```
Not yet, after I finish finals I plan on ordering the parts. However, my main printer has about 3000 hours of printing parts under its belt, so I do not think these parts would be too tough to print.
```

---
## \#1266 Posted by: chris.hunt Posted at: 2018-05-13T20:32:04.832Z Reads: 251

```
Gotcha, I'm planning my build and deciding between this a Modded GT2B remote or a Enertion Nano X
```

---
## \#1267 Posted by: ggalisky Posted at: 2018-05-13T22:08:40.816Z Reads: 255

```
I have the nano X, and it is very bare bones, it gets the job done and that its. I want some more data when I ride, mostly about battery voltage, I already know when I am going to fast lol
```

---
## \#1268 Posted by: Wentworth Posted at: 2018-05-15T11:21:12.446Z Reads: 265

```
I want to know what is configured on VESC TOOL.Who can tell me？And my signal connection seems not very stable, sometimes transmitter will get stuck.Is it wrong for me to use the wrong way？
```

---
## \#1269 Posted by: solidgeek Posted at: 2018-05-15T19:24:42.787Z Reads: 279

```
I have been putting together a tutorial on how to assemble the remote and receiver. I have tried to add as much information about the build, and included a lot of the fixes you guys have found :slight_smile:

It can be found here: https://solidgeek.dk/docs/firefly-remote/getting-started/

Also, I just received a bunch of PCBs for the receiver I have been working on. Now I got a fully functional PCB for the receiver - I will announce when they are ready to ship :-) 

![20180515_205507|690x388](upload://yGOTXSArYykxgQz3kLbx2w4MnOv.jpg)

... with external antenna :smirk:
```

---
## \#1270 Posted by: clistpdx Posted at: 2018-05-15T19:53:24.200Z Reads: 268

```
Wow, that's a great walkthrough! Thanks for putting it together. Now, do I have the guts to try to make this myself?....
```

---
## \#1271 Posted by: mrplaygood Posted at: 2018-05-15T20:19:41.066Z Reads: 253

```
So when can I order the sender/receiver? Sorry but I‘m very interessted and thrilled :smiley:
```

---
## \#1272 Posted by: Wentworth Posted at: 2018-05-16T08:24:21.877Z Reads: 245

```
I see that there are words such as "Motor pole" and "Motor pulley" in the program. Can this controller be used in belt driven skateboards? If I want to use it on the hub motor, do I need to change these parameters?
```

---
## \#1273 Posted by: Maxid Posted at: 2018-05-16T10:13:30.704Z Reads: 242

```
Not sure if this ever came up but did you guys ever think about switching to an ESP8266 as brain AND wireless module? I just got a NodeMCU for a work project and man this thing is awesome. Super tiny (much much smaller than a Nano) and even more powerful (80Mhz compared to the Nano's 16). Plus it is Arduino IDE compatible.
```

---
## \#1274 Posted by: mrplaygood Posted at: 2018-05-16T11:47:57.098Z Reads: 246

```
I‘m totally with you! Also it‘s cheaper and you can access the ESP8266 with the Remote and your Smartphone. So you could change Settings on your phone and use your remote mainly as ... a remote ;)
I have 2 Adafruit Feather with this chipset and I will try it out but I‘m no developer by any means.

Otherwise the ESP32 would be interessting to as it provides BLE and WiFi. Its even faster (if this is important) and it supports mesh capabilities which would enable much more features.
```

---
## \#1275 Posted by: webst Posted at: 2018-05-16T17:26:27.223Z Reads: 246

```
Up there somewhere I suggested ready esp32 based module with built in oled and liion charger but implementation is yet to be done. Shouldn’t be that hard as you can program it using arduino ide but so it may only seem.
```

---
## \#1276 Posted by: mrplaygood Posted at: 2018-05-16T17:38:01.744Z Reads: 255

```
Yeah, ESP32 can be programmed using Arduino but BLE implementation is pretty bad right now (or ar least last time I checked a few months ago)
I wouldn‘t even need a fully Oled remote. Boosted Board styled LEDs for a rough battery astimate would be enough for me. If I could connect my phone for further information and settings, I would already be happy :wink:
```

---
## \#1277 Posted by: chinzw Posted at: 2018-05-16T17:40:11.957Z Reads: 257

```
I have a port for nrf52 and working on a port to nrf51, both very good and stable modules. I prefer the nrf51 as it uses atmega 32u instead of the nordic shared cpu.
```

---
## \#1278 Posted by: webst Posted at: 2018-05-16T17:41:18.745Z Reads: 249

```
Wifi is pretty stable though. Have you seen metr.at module? Maybe it is all you need for now?
```

---
## \#1279 Posted by: mrplaygood Posted at: 2018-05-16T17:44:50.088Z Reads: 247

```
I ordered the (pretty expensive) bluetooth module for the metr app. That‘s what I will use but much more because my receiver doesn‘t really work. So I hope this build and especially @solidgeek s remote and receiverboard will be ready soon :slight_smile:
```

---
## \#1280 Posted by: Kit Posted at: 2018-05-16T23:42:10.362Z Reads: 250

```
This is awesome man, great work! I am excited for the announcement!
```

---
## \#1281 Posted by: wafflejock Posted at: 2018-05-17T00:00:00.409Z Reads: 256

```
I did a Bluetooth based receiver and used a phone app for a bit of testing but found the connection or pairing could drop out too easily and didn't recover quickly like the nrf chips can so I abandoned that entirely.  Personally decided to just go with a simple remote and using metr for collecting data on the go or changing "modes".  It works out pretty well and the remote remains a dumb and simple remote only responsible for transmitting control data (and failing safe when necessary).  Good thing about the lower clock rate mcu on the Arduino is it's very light on power consumption and if you don't have a lot of display or serial processing going on 8MHz is plenty fast to keep a consistent signal going.

From what I gathered with the esp modules there is some more overhead to maintaining the connection and can have other latency issues but I've not worked with them myself so can't really pass on my own judgement.
```

---
## \#1282 Posted by: wafflejock Posted at: 2018-05-17T00:11:19.901Z Reads: 240

```
Also to whoever is having problems with the nrf chips make sure you're only using 3.3V on the power input, the other SPI pins are 5V tolerant but with too high input voltage (on VDD) they will work for a brief period and burn out.  The capacitors right on the power and gnd on the nrf chips have helped me out as well.  On board antenna works to about 30-40ft in my experience the external power amplified antennas can go as far as I can see, over a city block.
```

---
## \#1283 Posted by: Wentworth Posted at: 2018-05-18T08:35:54.203Z Reads: 246

```
The lights of my receiver have been flashing, I have the correct connection mode, and the power supply voltage of nRF24L01 is 3.3 volts. I wonder why there is no successful communication. Can you give me some advice?
```

---
## \#1284 Posted by: Wentworth Posted at: 2018-05-18T10:38:22.065Z Reads: 271

```
There are other things I can't understand. Why do you want throttle less than 512 instead of 1023? According to your understanding, in one cycle, the pulse should not exceed 1.5ms, so can't we move forward? Since my transmitter and receiver are unable to communicate, I will wait until I have a good communication.![捕获|580x331](upload://hOWeG3tCIhF9j531nKfhDnraeIL.PNG)
```

---
## \#1285 Posted by: SeeTheBridges Posted at: 2018-05-19T00:49:54.971Z Reads: 277

```
Just gonna casually drop this here... Awesome to see your text guide coming together Solidgeek!
https://youtu.be/sCWVJGpMXQc
```

---
## \#1286 Posted by: Kit Posted at: 2018-05-19T05:15:12.744Z Reads: 275

```
Great guide man, are you going to do a batch run of some of these fireflies?
```

---
## \#1287 Posted by: Deakbannok Posted at: 2018-05-19T08:53:28.026Z Reads: 272

```
I will do a run test on nodeMCU. 80mhz  seems to be a perfect option for a RX.  ☺
```

---
## \#1288 Posted by: Wentworth Posted at: 2018-05-22T08:24:06.111Z Reads: 265

```
I don't seem to be able to show some parameters such as speed, and the setting on VESC TOOL is PPM and UART, and the receiver is the same as the schematic connection. Who can tell me how to do it? Maybe I am stupid. I can not understand the real usage of the reset button on the receiver, because there is a reset button on the Arduino.
```

---
## \#1289 Posted by: Zyb Posted at: 2018-05-22T09:16:15.817Z Reads: 270

```
did you set the correct baud rate in vesc tool? it should be 115200 if i remember correctly
```

---
## \#1290 Posted by: Wentworth Posted at: 2018-05-23T05:46:46.940Z Reads: 258

```
Of course, my baud rate is 115200
```

---
## \#1291 Posted by: Wentworth Posted at: 2018-05-23T05:52:52.051Z Reads: 259

```
You gave me the program, I could not connect, so I changed the nRF24L01 communication program, now I can connect, but can not receive speed, distance parameters. Is it because I changed the communication program?
```

---
## \#1292 Posted by: Wentworth Posted at: 2018-05-23T09:06:42.268Z Reads: 254

```
Oh, my God, I finally see the data, but how can I achieve the unique value? If it happens to be the same, will there be any interference?I do not understand the function of receiver reset button now.
```

---
## \#1293 Posted by: webst Posted at: 2018-05-23T14:11:10.927Z Reads: 265

```
[quote="Wentworth, post:1292, topic:28543"]
how can I achieve the unique value?
[/quote]
Put your cat on a keyboard
```

---
## \#1294 Posted by: sterlinggray4 Posted at: 2018-05-23T19:07:59.774Z Reads: 272

```
So I have been working all week to put together this awesome remote and I have both the receiver and the transmitter working and programmed but no matter what I do I cannot get them to connect since Monday. I have read this whole thread at least three times but haven't gotten the recievers to talk to each other today. I am using the nrf24 with a breakout board for power regulation and today I finally managed to see them connected but I don't know what I did besides leave them alone for a while. I also noticed that while they were connected the transmitter nrf was very hot and now I cannot get them to connect at all. Any advice here?
```

---
## \#1295 Posted by: SeeTheBridges Posted at: 2018-05-24T03:05:30.074Z Reads: 264

```
For those of you that have been interested in buying a complete Firefly, my thread is live: http://www.electric-skateboard.builders/t/for-sale-firefly-esk8-remotes/56558
```

---
## \#1296 Posted by: moon Posted at: 2018-05-24T10:16:02.451Z Reads: 259

```
Anyone have a 500mah lipo 3.7v?
```

---
## \#1297 Posted by: ACIN Posted at: 2018-05-26T00:35:56.264Z Reads: 261

```
Also looking for the lipo. If anyone in Europe bought a bunch and would sell one I'd be super happy.
```

---
## \#1298 Posted by: ACIN Posted at: 2018-05-26T03:23:29.098Z Reads: 264

```
Anyway I have made a [quick collection of the links I used](https://docs.google.com/spreadsheets/d/1UZk5K47U4A1RXhF5OQmYIX7wVK7k5NMdyN3NUXQifMw/edit?usp=sharing) instead of aliexpress (ebay and amazon mostly) to achieve sub 7 day delivery on all parts (except the damn battery :( ) for my fellow central european builders who just can't wait to get started.
```

---
## \#1299 Posted by: adrianlee Posted at: 2018-06-01T09:45:13.663Z Reads: 250

```
Anyone had problems with OLEDs? I think these SSD1306s have logic level max voltage of 3.3v, and it when usb powered (about4.5v) but mine stopped working after 5v regulator spiked over 5.5.v. 
No one needed to use logic level shifters?

@solidgeek thanks for the designs man, I have used without oled with some random airplane esc and it works smooth :ok_hand:
```

---
## \#1300 Posted by: Zyb Posted at: 2018-06-01T18:47:39.003Z Reads: 260

```
i have found some weird issue. when i quickly flip the wheel either to braking or acceleration side vesc basicly does nothing as if the movement never happened tho its visible in the oled that input has given. im talking very fast movement like flicking to braking side in under a second. can you guys test this? i tested it with 2 remotes they all do the same. im not sure if this is a huge deal as if you do that while on the board sudden %100 braking will prob make me fall off of it.
```

---
## \#1301 Posted by: ervinelin Posted at: 2018-06-02T09:23:42.580Z Reads: 261

```
See here for the solution... (works for my remote, needs to be ported to solidgeeks if proven to work)

https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/153?u=ervinelin
```

---
## \#1302 Posted by: Zyb Posted at: 2018-06-02T16:47:16.119Z Reads: 251

```
that fixed it along with another problem for me. acceleration and brakes are butter smooth now. you can actually use @ervinelin's code in firefly remote but you will be stuck with only speed value as his version uses a button to shuffle around the vesc data.
```

---
## \#1303 Posted by: SeeTheBridges Posted at: 2018-06-02T19:11:39.916Z Reads: 246

```
I highly recommend just using the development branch of Solidgeeks code if you want rotating VESC data like the current master branch. The dev branch works perfectly and is what I've been shipping my remotes with.
```

---
## \#1304 Posted by: ervinelin Posted at: 2018-06-03T00:47:31.129Z Reads: 250

```
He is right, the developmental branch uses the servo library as well.

Looks like he cleaned up lots of other stuff too... Will go look when I have the time.
```

---
## \#1305 Posted by: willumpie82 Posted at: 2018-06-04T06:39:24.924Z Reads: 261

```
I have build one of these remotes as well, its great! thanks @solidgeek, but i run in to trouble with the receiver, it sends `servo esc.writemiliseconds(1000~2000)`, but my VESC 4.12 did not like the output, the autodetection rate was 1700~2000. I changed it to `esc.write(0~180)` now the full range is properly detected in VESC-tool.

Other than that i also added a blinking battery when charging. for ADC input I used the 2x 20k divider as suggested by the schematics on the website of @solidgeek, I had to change the voltage reading to x 2 

another tip, add (or the schematic of-) a soft power button (e.g. [Adafruit push-button](https://www.adafruit.com/product/1400) solid state switch), I ordered this breakout and going to add it to my build, I'll add a remote timeout to the code (soft switch off pin of the breakout)
```

---
## \#1306 Posted by: clistpdx Posted at: 2018-06-05T21:18:09.197Z Reads: 263

```
[quote="solidgeek, post:1269, topic:28543"]
It can be found here: [https://solidgeek.dk/docs/firefly-remote/getting-started/ ](https://solidgeek.dk/docs/firefly-remote/getting-started/)
[/quote]

@solidgeek Is there a final portion missing from your guide in the 'receiver' section? It covers attaching the Nano to the NRF, but I don't see any description of what to do w/ the LED, switch, and power filtering board:
https://solidgeek.dk/docs/firefly-remote/receiver/electronics/
```

---
## \#1307 Posted by: willumpie82 Posted at: 2018-06-06T06:57:28.526Z Reads: 269

```
If i read the source code correctly, the switch is for resetting the address, "kind a pairing mode?" on pin 4, the other side if the switch to ground (pinMode = INPUT_PULLUP)  
the LED is a status led, pin 13, other end of the LED with a resistor to GND (missing in the schematics?)
https://solidgeek.dk/wp-content/uploads/2018/03/reciever-schematic.png

by the way, I integrated the softpower switch, and also included a sleep to power off function to the code, when de board is not connected it will shut the remote off in ~30sec

![IMG_20180605_213153|666x500](upload://81CZn7381lAd6SYnKD46b9OviGN.jpg)
```

---
## \#1308 Posted by: clistpdx Posted at: 2018-06-07T05:26:35.918Z Reads: 256

```
Does anyone have a good US source to find the 20mm tension spring needed for this build? The suggested ebay source in @solidgeek's spreadsheet doesn't ship to the US. I've found these alternatives on aliexpress, but I'd hate to spend $10 when I only need 1 spring:
[$10 for 10](https://www.aliexpress.com/item/20PCS-0-7-x-4mm-0-7mm-Tension-spring-with-a-hook-extension-spring-length-20mm/32803559040.html?spm=2114.search0104.3.116.11d8751bHdGATX&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10151_10065_10344_10068_10130_5722815_10324_10342_10547_10325_10343_10546_10340_5722915_10548_10341_10545_5722615_10696_10084_10083_10618_10307_5722715_10059_100031_10103_10624_10623_10622_5722515_10621_10620,searchweb201603_11,ppcSwitch_5&algo_expid=516816c9-94cb-4354-ab9f-e3750aa69e41-17&algo_pvid=516816c9-94cb-4354-ab9f-e3750aa69e41&transAbTest=ae803_1&priceBeautifyAB=0)
[$18 for 50](https://www.aliexpress.com/item/Extension-spring-stainless-steel-wire-0-4mm-OD-4mm-L-20mm-spring-x50/32828531720.html?spm=2114.search0104.3.26.16ab2fd71Oqbjc&ws_ab_test=searchweb0_0,searchweb201602_4_10152_10151_10065_10344_10068_10130_5722815_10324_10342_10547_10325_10343_10546_10340_5722915_10548_10341_10545_5722615_10696_10084_10083_10618_10307_5722715_10059_100031_10103_10624_10623_10622_5722515_10621_10620,searchweb201603_11,ppcSwitch_5&algo_expid=d553adc8-db91-4728-bc86-07cc362f026f-4&algo_pvid=d553adc8-db91-4728-bc86-07cc362f026f&transAbTest=ae803_1&priceBeautifyAB=0)
```

---
## \#1309 Posted by: ervinelin Posted at: 2018-06-07T05:41:12.358Z Reads: 242

```
My aliexpress springs took MONTHS to arrive... MONTHS...
```

---
## \#1310 Posted by: SeeTheBridges Posted at: 2018-06-07T05:42:17.254Z Reads: 238

```
I'll check how many I have left tomorrow. I should have spares leftover.

@ervinelin I KNOW RIGHT. Springs take FOREVER to arrive for some reason. I ran into the same issue earlier this year with my first round of parts
```

---
## \#1311 Posted by: clistpdx Posted at: 2018-06-07T18:53:57.319Z Reads: 246

```
[quote="solidgeek, post:1, topic:28543"]
You can find a list of all the components I used here:

[https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit?usp=sharing ](https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit?usp=sharing).
[/quote]

@solidgeek I don't see an on/off switch on your component spreadsheet. Is this just because each of us can choose our own, or is the spacing picky about what we use?
```

---
## \#1312 Posted by: rey8801 Posted at: 2018-06-07T18:59:11.387Z Reads: 241

```
It's not present but pick it up one with 3 pins and it's fine. I bought this one... They should be ok

5 Pcs 50V 0.5A 3 Pin 2 Position On/OFF 1P2T SPDT Slide Switch 3 Pin
 http://s.aliexpress.com/Y3MRrMZv?fromSns=Copy to Clipboard
```

---
## \#1313 Posted by: rey8801 Posted at: 2018-06-08T14:42:19.399Z Reads: 241

```
Guys I ordered everything, at least I hope and by the different tutorial it's clear for the remote how to build it, but not for the receiver. At least for me. Do you know whethere there is a pleasant tutorial too? I only found the schematic on @solidgeek website. I understtod that the receiver is componsed by an arduino nano + a NRF module connected basically like the remote nad the power, GND and PPM are taken from the sarvo cable, while the TX adn RX from the UART port. The part I understood less is the power filter. SO basically from the 5v of the servo i need to place the power filter in betwwen the VESC and the Arduino. The same of course for the GND. Then which capacitors should I use it? I bought this one https://www.aliexpress.com/item/1PCS-JMT-L-C-Power-Filter-1A-RTF-LC-FILTER-1-4S-LC-Module-Lllustrated-Eliminate/32841771400.html?spm=a2g0s.9042311.0.0.51554c4dLBIjh2. Is it itself enough or I need additonal capacitors? Thx a lot...looking forward to build it.
```

---
## \#1314 Posted by: clistpdx Posted at: 2018-06-08T14:52:45.670Z Reads: 235

```
I know. Solidgeek's site kind of falls apart during the receiver section. I don't think he has finished it yet. However SeeTheBridges should release his part 4 video soon which should cover it all. I just received his finished Firefly remote in the mail yesterday and took some pictures of the insides of the receiver to break it down a bit, since I'm building another one myself
```

---
## \#1315 Posted by: rey8801 Posted at: 2018-06-08T14:54:24.650Z Reads: 227

```
YEs I saw his video really nice. I am waitng for the last part too. Well at mean time if you can upload some pictures it would be awesome!
```

---
## \#1316 Posted by: Zyb Posted at: 2018-06-08T15:29:10.569Z Reads: 254

```
needing to reset issue is quite a headache. LC filter and low ESR caps were both recommended in this thread i applied both of them but it didnt help with the issue. everytime i power on my vesc i had the issue until you make a cap modification on reset-gnd pins. another good implementation will be 1000uf on 5V line for brownouts and around 10uf to 3.3v is recommended for the nrf module. tho its better to use 100uf, 10uf and 100nf in parallel. you can make your own pcb to make the whole thing more robust and you dont have to use cables at all except for the mandatory servo and tx rx leads. this my take on what i talked about. it is already rock solid as it is and you can heat shrink the whole thing. you can see the lc filter is there on servo cable. the big cap is low ESR 1000uf one rest is 100uf, 10uf and 100nf
transmitter side also made with pcb. again less cables less hassle.
![image_6483441%20(1)|592x500](upload://fGhnMd1XPBAc9uoCmoQlOK2Iw6T.JPG)![image_6483441%20(2)|590x499](upload://5Jd144K4JSSp9v9M2YfLSsUo3bt.JPG)
```

---
## \#1317 Posted by: rey8801 Posted at: 2018-06-08T15:33:17.527Z Reads: 236

```
Really nice!
So let me understand. Is someone actually using this remote up to know or it still has bugs that make it unreliable? Thx
```

---
## \#1318 Posted by: Zyb Posted at: 2018-06-08T15:37:39.140Z Reads: 241

```
there has been quite a bit issues at least i had. but the latest version is rock solid at the moment. worst was the issue with the signal for me and solved with the chip in the picture. then there was a reset issue and thats solved aswell with a cap tho im trying a mcp130 chip now you can see theres a place for it on the pcb, gonna try it to replace cap solution see if it works. @ervinelin had brownout issue and someone recommended 1000uf cap which is a thing in RC universe and thats solved too. no more problems so far.
```

---
## \#1319 Posted by: HighMasterGogo Posted at: 2018-06-08T15:49:56.142Z Reads: 233

```
Hey @solidgeek any chance of the easyeda for this?
```

---
## \#1320 Posted by: rey8801 Posted at: 2018-06-08T16:02:00.847Z Reads: 242

```
I see. Maybe I am talking only for me but I read the all thread and it's too long and of course full of "I try it but it didn't work at the end" that makes it really complicate choose the right way to build it correctly. I saw the video tutorial and the description ecc but, for instance, I do not know if they still correct anymore. Do you guys think would be possible that someone with the competence make a to do list with everything well explained? Of course he can refeer to the parts that are still correct but I think it's important to make it clear. Including the software part, since it's full of updates. For who like me started to follow this project later it's difficult to keep up to date. Just my opinion, if I am the only one who think that, then nevermind.
PS: just to be sure I bought stuffs for 3 remotes :sunglasses:
```

---
## \#1321 Posted by: SeeTheBridges Posted at: 2018-06-08T17:25:06.968Z Reads: 241

```
My guide is still up to date. I finished filming the receiver building stuff last week, I'm just trying to finish shipping my batch 1 remotes and do a couple other behind the scenes things before I get to editing it all together. Sorry about that! 🙈

The software has seen updates but it's still basically the same principle. The dev branch is pretty much perfect right now.
```

---
## \#1322 Posted by: rey8801 Posted at: 2018-06-08T18:03:55.582Z Reads: 243

```
That sounds good! I watch your video and I see a lot of effort also in editing. I can confirm that they are pretty good! Thanks for your contribution, really appreciated!
```

---
## \#1323 Posted by: clistpdx Posted at: 2018-06-09T01:44:31.546Z Reads: 267

```
[quote="rey8801, post:1315, topic:28543"]
if you can upload some pictures it would be awesome!
[/quote]

Here's what my Firefly receiver from @SeeTheBridges looks like. Case with PPM and UART cables coming out:
![receiver1|583x500](upload://1a9vFacRgTFQr5tNEf6G33vaxcm.JPG)

Inside there are just two components (Nano and NRF). No IC filter. He has added two caps. A small yellow 0.022μF (223) cap on the end bridging the GND and RESET pins and a large black A1722 (can't tell what it is? It's glued down) cap soldered between the 5V and GND pins.
![receiver2|690x294](upload://mXvOnS6vLkmDknvzmCBLMX9tQd6.JPG)

![receiver3|666x500](upload://an9Q4uONpFCmhbzGar0vEGgPzt3.JPG)
Pretty straightforward
```

---
## \#1324 Posted by: rey8801 Posted at: 2018-06-09T03:38:52.490Z Reads: 244

```
Ok that's feasible. I'm case the power filter is needed that is not difficult to add it. So I see a UART cable only for RX and TX and a servo cable for PPM, 5v and GRD. Did you already tried it out? Thx man you gave me hope :laughing:
```

---
## \#1325 Posted by: clistpdx Posted at: 2018-06-09T04:04:23.698Z Reads: 243

```
I haven't tried it out on the road. Just bench tested. It doesn't fit in my current build, but I'll be putting it into my next one, once I get my Spud from jlabs.
```

---
## \#1326 Posted by: rey8801 Posted at: 2018-06-09T04:05:58.299Z Reads: 248

```
Great man! Welcome in the Spud family.
```

---
## \#1327 Posted by: Zyb Posted at: 2018-06-09T12:57:31.042Z Reads: 255

```
for those who wants to fix the reset issue with a different approach, mcp130 chip works! i just received it today and soldered it to the pcb and problem vanished.
![04239784-7293-4A4B-ACCC-506E8B818464|297x499](upload://wFyCdfdKOZXKuNkb4fjEwTIqJUO.jpeg)
```

---
## \#1328 Posted by: clistpdx Posted at: 2018-06-09T14:34:49.318Z Reads: 244

```
Is it still possible to use the mcp130 without the PCB  approach (i.e. if we're going old school w/ just a nano and nrf24)? I'm not as familiar w/ the pinouts on the PCB. What would we bridge w/ the mcp130?
```

---
## \#1329 Posted by: Zyb Posted at: 2018-06-09T14:40:32.099Z Reads: 242

```
Yea you can get to92 package of the same chip it’s much easier to deal with than this smd component. You need to check the datasheet but it has 3 legs one goes to voltage source to watch over in our case it’s 5v  second one goes to ground and third leg goes to reset pin
```

---
## \#1330 Posted by: SeeTheBridges Posted at: 2018-06-09T15:10:19.101Z Reads: 234

```
Just looked up pricing on these, looking like ~46c per unit bought individually. The Kemet ceramic caps I've been using are 30c per unit, so not a terrible price difference too 👌
```

---
## \#1331 Posted by: Zyb Posted at: 2018-06-09T15:35:19.579Z Reads: 232

```
Also it looks like a proper solution. Tested it on the road too and no problem so far.
```

---
## \#1332 Posted by: clistpdx Posted at: 2018-06-09T15:42:20.391Z Reads: 232

```
Do you think this could replace both of your caps, or just the ceramic 223?
```

---
## \#1333 Posted by: SeeTheBridges Posted at: 2018-06-09T16:03:16.372Z Reads: 242

```
This would only replace the ceramic cap, so for my use case it doesn't make too much sense to switch to it. The electrolytic cap is to cover the less than ideal 5V line from the VESC. For how I'm understanding it, my ceramic caps just delay the Arduino startup by enough milliseconds for it not to be an issue at all so the same end result as this IC 🤷‍♀️

EDIT: I just read the data sheet, and if I'm understanding this correctly it might also be able to cover for the lack of an electrolytic cap, but I think you'd just run into momentary cutout issues. The IC sends a reset signal to the microcontroller whenever the supply voltage drops too low, so instead of the arduino freezing, you'd get a reset and feel it as a blip of connection? Totally speculating here, but I think that's what would happen
```

---
## \#1334 Posted by: wafflejock Posted at: 2018-06-09T16:30:05.672Z Reads: 249

```
FYI I had brown out type issues with a 5V (16MHz) nano when working on my remote and receiver too I went with just using 3.3V (8MHz) variant of the pro mini since the dips in voltage didn't cause the brown out resets I was seeing with the 5V nano powered off the BEC from the VESC

---

Bonus with the 3.3V ones you can power them off a 1S lipo (in the remote without boost) they can work reliably down to the cut off voltage on 1S lipos that have built in cut off circuitry.
```

---
## \#1335 Posted by: Zyb Posted at: 2018-06-09T17:03:09.163Z Reads: 248

```
In case of a brownout I think mcp130 will reset the arduino but that’s why I have I have a big ass 1000uf cap on 5v line to prevent that. So far no issues with hard acceleration braking etc just smooth as a butter
```

---
## \#1336 Posted by: solidgeek Posted at: 2018-06-10T11:47:14.169Z Reads: 246

```
@HighMasterGogo Here you go: https://easyeda.com/thesolidgeek/Firefly_Remote-d6b2c0d3979343d1ab0fd1710bf98450

@Zyb Nice addition with the MCP130, I didn't know such chips existed :D  

@willumpie82 Weird that your VESC didn't like the standard 1000-2000 PPM signal. I am curious of how you implemented the blinking battery when charging - did you add another wire to monitor if a charger is connected? :slight_smile:
```

---
## \#1337 Posted by: erod998 Posted at: 2018-06-10T13:19:30.774Z Reads: 234

```
For the receiver, should I take 5V from the VESC through UART or PWM? Does it matter?
```

---
## \#1338 Posted by: ervinelin Posted at: 2018-06-10T13:21:15.087Z Reads: 233

```
pwm just makes it easier... same 3 wires
```

---
## \#1339 Posted by: erod998 Posted at: 2018-06-10T13:29:33.058Z Reads: 233

```
I’ve seen some people use a BEC. Do you think it’s necessary? The PWM can supply up to 1 amp, and the receiver will never come close to pulling that. I guess the only advantage is no noise from the VESC, which shouldn’t be a problem if thanks to SolidGeek’s recommendation to solder the capacitors on the Vin for the Nano.
```

---
## \#1340 Posted by: ervinelin Posted at: 2018-06-10T13:36:48.947Z Reads: 229

```
You need a HUGE BEC to step down from 10/12S to 5V.... 

I just use an LC filter and a large cap to filter the noise in the 5V line...
```

---
## \#1341 Posted by: erod998 Posted at: 2018-06-10T13:48:14.231Z Reads: 231

```
Thank you.
```

---
## \#1342 Posted by: adrianlee Posted at: 2018-06-10T16:16:12.306Z Reads: 236

```
seems like i blew 3 oleds now... Did anyone else had problems with 5v boost converter? Mine is getting up to 5.85V and this is like third one I soldered on
```

---
## \#1343 Posted by: clistpdx Posted at: 2018-06-10T16:29:33.493Z Reads: 243

```
[quote="solidgeek, post:1336, topic:28543"]
Here you go: [https://easyeda.com/thesolidgeek/Firefly_Remote-d6b2c0d3979343d1ab0fd1710bf98450 ](https://easyeda.com/thesolidgeek/Firefly_Remote-d6b2c0d3979343d1ab0fd1710bf98450)
[/quote]

Is there a trick to exporting the gerber file on EasyEDA? I tried to open your design in the Editor, then clicked 'convert to PCB'. But it gives 'cant find the package' errors. Is there an easier way to export the Gerber that I'm not aware of?
```

---
## \#1344 Posted by: SeeTheBridges Posted at: 2018-06-10T17:49:41.978Z Reads: 235

```
I've made I think 8 remotes now and haven't blown a single OLED yet. I use the one with the red PCB recommended by solidgeek

EDIT. I meant the red boost converters
```

---
## \#1345 Posted by: clistpdx Posted at: 2018-06-10T18:12:02.343Z Reads: 228

```
solidgeek's spreadsheet recommends this one, w/ a **blue** PCB: https://www.aliexpress.com/item/1pcs-SAMIORE-ROBOT-0-91-inch-OLED-module-0-91-white-OLED-128X32-OLED-LCD-LED/32672229793.html
Did he post updated recommendations somewhere in this thread?
```

---
## \#1346 Posted by: HighMasterGogo Posted at: 2018-06-10T19:56:13.781Z Reads: 226

```
Awesome, thanks @solidgeek.

Any chance of the easyeda for the stand alone ATmega chip?
```

---
## \#1347 Posted by: SeeTheBridges Posted at: 2018-06-10T20:03:44.381Z Reads: 230

```
Check my edit. I meant the boost converter
```

---
## \#1348 Posted by: willumpie82 Posted at: 2018-06-10T20:24:24.556Z Reads: 226

```
I connected the oled and hall to the 3v3 rail of my Arduino. Maybe not all oleds are 5v capable?
```

---
## \#1349 Posted by: solidgeek Posted at: 2018-06-10T22:17:21.815Z Reads: 226

```
Well I only used EasyEDA to make the schematics, most parts doesn't have a footprint. So you cannot simply export the gerber files :P The receiver PCB I posted earlier is made in Altium Designer - and is more of a prototype to test the ATmega32u4 instead of the standard 328p
```

---
## \#1350 Posted by: willumpie82 Posted at: 2018-06-11T09:36:24.915Z Reads: 231

```
check out this unit, 5v 2A e-bike usbport, there is a compact PCB inside (if desired, I can post a picture later today ;) )
https://nl.aliexpress.com/item/Elektrische-Bike-USB-Charger-Output-5-V-2A-Voor-Mobiele-Telefoons-Ebike-36-V-48-V/32860737409.html
```

---
## \#1351 Posted by: Travo Posted at: 2018-06-12T01:30:07.055Z Reads: 230

```
Hey guys, I'm just getting into all this electric skateboarding stuff and would like to know if anyone has made a video or has an instructions list containing something similar to a step by step of how to do this. I am considering making this alternatively to buying a winning v2 remote.  I have a 3d printer so the case etc is no probem it's just the electronics inside that are kind of scaring me out of this. Thanks!
```

---
## \#1352 Posted by: clistpdx Posted at: 2018-06-12T03:07:06.548Z Reads: 237

```
Yep, it's all buried in the thousand threads above :) @solidgeek has a tutorial: https://solidgeek.dk/docs/firefly-remote/getting-started/
and @seethebridges has a video tutorial. The first 3 parts are out already w/ more coming: https://www.youtube.com/watch?v=N032HqxeymA
```

---
## \#1353 Posted by: adrianlee Posted at: 2018-06-12T09:32:55.645Z Reads: 241

```
My Oleds should be rated 3-5V, and they work from 5V rail when powered by usb (real measured voltage around 4.7V). I think the logic pins cant take over 5V thats why they fry when using my shitty boost converter. Or maybe because the boost converter doesn fit properly, something is pressing wrong place on it
```

---
## \#1354 Posted by: Travo Posted at: 2018-06-12T14:55:44.509Z Reads: 233

```
Thanks so much!
```

---
## \#1355 Posted by: Travo Posted at: 2018-06-12T15:03:00.569Z Reads: 230

```
One more question, I was just looking at sourcing all the parts and the nrf24 module on the parts list is "no longer available. I tried to find one but was unable to. Does anyone know where I could purchase one of these?
```

---
## \#1356 Posted by: rey8801 Posted at: 2018-06-12T15:07:52.721Z Reads: 232

```
https://www.aliexpress.com/item/SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in-stock-fast/32255233251.html?spm=a2g0s.9042311.0.0.27424c4d4V3Bdl
```

---
## \#1357 Posted by: clistpdx Posted at: 2018-06-12T15:48:27.186Z Reads: 237

```
And if you can't wait 30-50 days you can get them next week for a bit more cash: https://www.ebay.com/itm/1Pcs-2-4G-NRF24L01-PA-LNA-Wireless-Module-Ceramic-Antenna-1-27mm-For-Arduino-US/162862165321?hash=item25eb576d49:g:jrgAAOSw8d5ZRXQZ
```

---
## \#1358 Posted by: adrianlee Posted at: 2018-06-12T18:24:04.982Z Reads: 231

```
When ordering from aliexpress, I always use the aliexprees standard shipping, it costs like 2,50e and delivery time is reasonable 12-21days to Finland. And use the same shop when ordering many items so only one shipping cost is added
```

---
## \#1359 Posted by: Travo Posted at: 2018-06-13T15:27:17.357Z Reads: 231

```
I was unable to locate the code for the arduino, I've never used one before so is it just as easy as plugging it in and uploading the code? Also how does this connect to the ESC, and do I need more parts do make the connection.  Thanks again for all the help I'm really new to this skateboarding thing. Here is the link to the ESC if needed products/torque-esc-bldc-electronic-speed-controller
```

---
## \#1360 Posted by: SeeTheBridges Posted at: 2018-06-13T17:58:32.019Z Reads: 243

```
https://github.com/SolidGeek/nRF24-Esk8-Remote/

There's the code, and you'll need to get the arduino IDE and a couple more libraries
```

---
## \#1361 Posted by: Travo Posted at: 2018-06-13T21:00:44.890Z Reads: 240

```
Thanks! Appreciate it. 
Do you know how the remote connects to the board?
```

---
## \#1362 Posted by: clistpdx Posted at: 2018-06-13T21:51:27.429Z Reads: 238

```
both the remote and the receiver have an arduino on board with a microUSB jack on them. Just watch the videos. It's all in there
```

---
## \#1363 Posted by: Travo Posted at: 2018-06-14T01:01:06.102Z Reads: 231

```
Sorry for all the questions.  Are the videos on @solidgeek youtube channel as i couldn't locate them :frowning:  Is it possible you could link them?
```

---
## \#1364 Posted by: clistpdx Posted at: 2018-06-14T01:10:58.357Z Reads: 240

```
[quote="clistpdx, post:1352, topic:28543"]
Yep, it’s all buried in the thousand threads above :slight_smile: @solidgeek has a tutorial: [https://solidgeek.dk/docs/firefly-remote/getting-started/ ](https://solidgeek.dk/docs/firefly-remote/getting-started/)
and @seethebridges has a video tutorial. The first 3 parts are out already w/ more coming: [https://www.youtube.com/watch?v=N032HqxeymA ](https://www.youtube.com/watch?v=N032HqxeymA)
[/quote]
10 characters
```

---
## \#1365 Posted by: Travo Posted at: 2018-06-14T01:31:58.949Z Reads: 240

```
Thanks again so much :slight_smile: !!!
```

---
## \#1367 Posted by: Travo Posted at: 2018-06-14T23:05:33.951Z Reads: 250

```
I couldn't seem to find any of this in the thread above so here it is.  I was wondering if you could put a USB C female jack instead of the micro USB one in the remote to charge it.  I'm no electrician or anything and I know there's not a whole lot of space in that area but I'm curios if one of [these](https://www.aliexpress.com/item/2-pcs-USB-3-1-Type-C-Connector-24-Pins-Female-Socket-receptacle-adapter-to-solder/32728796345.html?ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10068_10130_5722815_10342_10547_10343_10340_5722915_10548_10341_5722615_10696_10084_10083_10618_10139_10307_5722715_10059_100031_10103_10624_10623_10622_5722515_10621_10620,searchweb201603_25,ppcSwitch_4&algo_expid=cdc03c05-7072-47b1-bbe2-6e53724f0a5b-1&algo_pvid=cdc03c05-7072-47b1-bbe2-6e53724f0a5b&transAbTest=ae803_2&priceBeautifyAB=0) would work?  If that doesn't fit could you also use one of [these](https://www.aliexpress.com/item/cltgxdd-N-400-1PCS-Type-C-micro-USB-Dock-Connector-Charging-Port-socket-jack-for-ZTE/32840351844.html?scm=1007.13338.98644.000000000000000&scm_id=1007.13338.98644.000000000000000&scm-url=1007.13338.98644.000000000000000&pvid=40f66279-13eb-4972-8125-fb72837c8fb6&_t=pvid:40f66279-13eb-4972-8125-fb72837c8fb6,scm-url:1007.13338.98644.000000000000000)? I'm not sure about the pin layout but couldn't you directly solder onto them as to reduce space?![jpg_640x640|430x430](upload://fLdR2U98Bu45SHjC6BlVWEghJ2s.jpg)![cltgxdd-N-400-1PCS-Type-C-micro-USB-Dock-Connector-Charging-Port-socket-jack-for-ZTE%20(1)|500x500](upload://b9c8kkRzneL7BDP3wRImfyoFv9S.jpg)
```

---
## \#1368 Posted by: wafflejock Posted at: 2018-06-14T23:15:40.856Z Reads: 235

```
Yup should work fine.  Only issue really is usb-c has the capability to have more than 5V supply (can go up to 20V according to Wikipedia) but so long as there is no connection to the CC pins it should default to 5V 500mA.  In theory should work fine though (plus something will be able to plug directly into a MacBook pro 2017) https://en.m.wikipedia.org/wiki/USB-C

Would just check the vbus and G pins with multimeter with it plugged into the adapter(s) you plan to use to charge.
```

---
## \#1369 Posted by: Travo Posted at: 2018-06-15T00:35:11.319Z Reads: 243

```
I would be attaching the wires to these ports correct? ![sketch-1529022830282|281x500](upload://aZpVBSa79LwVNFH2HyizIbXfKhd.jpg)
```

---
## \#1370 Posted by: SeeTheBridges Posted at: 2018-06-15T00:36:33.646Z Reads: 234

```
That USBc port is waaayyyyy too big to fit in the remote because of the PCB around it
```

---
## \#1371 Posted by: Travo Posted at: 2018-06-15T00:38:36.138Z Reads: 246

```
I was thinking of trimming all the sides off and just soldering to the gnd which I think connects directly to the side of the board. Correct me if I'm wrong on that. That would make it about the same size. ![sketch-1529023178169|281x500](upload://b6GlahLiNwCrQCRgwwp9rFnn0bk.jpg)
```

---
## \#1372 Posted by: Zyb Posted at: 2018-06-15T00:46:11.556Z Reads: 243

```
if you have something like a dremel tool i think you can make some adjustments on the shell to make it fit. just connect a usb c cable to a phone charger and see exactly which pads are 5v-gnd using a multimeter, trim the excess pcb. try to fit it if not enlarge the usb hole with a dremel.
```

---
## \#1373 Posted by: Travo Posted at: 2018-06-15T01:23:26.487Z Reads: 235

```
Good point, I'll probably have the parts in like 1-2 months I'll let you guys know how it goes down.  On a side note, will I have to change anything with the boost converter or anything?
```

---
## \#1374 Posted by: Travo Posted at: 2018-06-15T01:42:54.720Z Reads: 237

```
Hey everyone, I was looking at the Hall-Effect sensor (SS495A) and found that it costs about 24 USD to ship to Canada (My country) [This ](https://www.ebay.com/itm/1PCS-SS495A-SENSOR-SS-HALL-EFFECT-RATIOMETRC-495-SS495/192167972916?hash=item2cbe1a9034:g:A84AAOSwuspY~s0M) one costs 8.18 usd and I'm 99% sure its the exact same one as in the shopping list provided by @solidgeek above. If someone could double check that it's the same that'd be great!
```

---
## \#1375 Posted by: SeeTheBridges Posted at: 2018-06-15T01:59:12.833Z Reads: 230

```
That Hall sensor should work fine. If you Dremel that PCB on the USB C, assuming you don't short anything in the process, it might work.
```

---
## \#1376 Posted by: Travo Posted at: 2018-06-15T02:03:17.880Z Reads: 231

```
Alright, I'm ordering 2 just in case. Also keep up the videos they really help out a lot :slight_smile:
```

---
## \#1377 Posted by: SeeTheBridges Posted at: 2018-06-15T02:48:57.711Z Reads: 231

```
Glad I can help :smiley: I'm gonna try and finish the script for the next part tonight and hopefully have it up by next week!
```

---
## \#1378 Posted by: willumpie82 Posted at: 2018-06-15T06:08:30.553Z Reads: 238

```
or if we are making a pcb anyway, add this conroller:
https://www.microchip.com/wwwproducts/en/UTC2000
"Transition any existing USB Type-A design to a USB Type-CTM Downstream Facing Port or any existing Type-B design to a USB Type-C Upstream Facing Port"

and
http://www.ti.com/product/BQ25703A/

but i guess to make it safe, it can get rather complex
https://www.synopsys.com/designware-ip/technical-bulletin/converting-existing-designs.html
https://www.scorpia.co.uk/2016/03/17/using-usb-type-c-on-hobyist-projects/
```

---
## \#1379 Posted by: chinzw Posted at: 2018-06-15T17:40:25.542Z Reads: 239

```
travo , use digikey.ca for electronics components, there's no point on using ebay. Digikey has overnight shipping 8$ and free for orders over 100$. Those hall sensors are super cheap, around 5$ if you buy only one.

https://www.digikey.ca/product-detail/en/honeywell-sensing-and-productivity-solutions/SS495A/480-2005-ND/701360
```

---
## \#1380 Posted by: Travo Posted at: 2018-06-15T17:48:53.446Z Reads: 240

```
Thanks so much! Shipping isn't too important as I'm still waiting on almost every part required for the build.  But digi key is definitely more reliable.
```

---
## \#1381 Posted by: chinzw Posted at: 2018-06-15T18:01:26.115Z Reads: 250

```
When i say overnight shipping 8$, i mean that's the only shipping option they offer. So try and bulk up a few items into one order.
```

---
## \#1382 Posted by: Travo Posted at: 2018-06-18T20:51:46.685Z Reads: 256

```
Just printed the outer shell and it looks fantastic!![15293550470161770323247022675970|375x500](upload://rx37qcpEE8SuAnJqxIsjdP2ggnY.jpg)
```

---
## \#1383 Posted by: Travo Posted at: 2018-06-19T01:47:26.450Z Reads: 253

```
Not entirely related to the discussion but if anyone wants a reliable cheap 3d printer in my experience you cannot go wrong with the Anet A8 (I got mine from gearbest). I've had mine for over a year and it still works fine.( I've only replaced the heat block, nozzle and tube which is just considered regular maintenance and is super cheap to do).
```

---
## \#1384 Posted by: SeeTheBridges Posted at: 2018-06-19T02:49:30.807Z Reads: 241

```
If you get an Anet A8, just make sure to turn on the safety features in the firmware! They don't come turned on by default and I've heard stories of them catching fire because of that
```

---
## \#1385 Posted by: Travo Posted at: 2018-06-19T05:46:38.537Z Reads: 255

```
Jeez I didn't know about that?! Thanks for letting me know, I am attaching a MOSFET so that should help on safety but thanks for he heads up!!
```

---
## \#1386 Posted by: SeeTheBridges Posted at: 2018-06-19T06:41:19.527Z Reads: 268

```
Check out this guide if you need help setting up all the safety features!
https://youtu.be/tu5WD6ymEJE

EDIT: I dont wanna double post so here's part 4 of my guide btw for everyone else.
https://youtu.be/DzMGfMHYWHw
```

---
## \#1387 Posted by: Travo Posted at: 2018-06-22T01:02:55.778Z Reads: 254

```
Great, thanks. Hyped for part 5
```

---
## \#1388 Posted by: Travo Posted at: 2018-06-22T01:06:48.187Z Reads: 244

```
I ordered the ardiuno from the provided link about a week ago and the seller has still not started shipping or replied to my messages. Is anyone else having this problem?
```

---
## \#1389 Posted by: SeeTheBridges Posted at: 2018-06-22T01:22:49.819Z Reads: 242

```
I was having issues with them as well. Send them a message at the end of your processing time if they haven't shipped it, and they should ship it before the time expires. I've dealt with them thru AliExpress and directly. You'll get your arduino, don't worry
```

---
## \#1390 Posted by: erod998 Posted at: 2018-06-23T20:39:12.524Z Reads: 241

```
What is the killswitch vs cruise trigger type? I cant get mine to do anything when I change it. 
Also, who is using control over UART only? Any issues?
```

---
## \#1391 Posted by: adrianlee Posted at: 2018-06-25T14:15:45.918Z Reads: 245

```
I dont understand wtf I'm doing wrong, the oleds never work when i turn the remote on. I made new remote with new 5v regulator and new arduino nano, new oleds, work when usb powered , once turn on from battery, the oled wont work anymore, all rated for 5V.
Connecting 
5V to vcc
GND to gnd
SDA to A4
SCL to A5
UPDATE: The oled works again when powering arduino from usb, but not when battery is on
```

---
## \#1392 Posted by: SeeTheBridges Posted at: 2018-06-25T15:14:19.661Z Reads: 239

```
Can you upload pictures of your wiring?
```

---
## \#1393 Posted by: clistpdx Posted at: 2018-06-25T15:51:59.765Z Reads: 247

```
It sounds to me like the issue may exist somewhere in your booster/charger wiring, rather than near your OLED. I would want to see photos of your usb/booster/charger/switch section
```

---
## \#1394 Posted by: adrianlee Posted at: 2018-06-25T16:38:17.032Z Reads: 267

```
![10|375x500](upload://65VIKiS9zaa7S3ZiiYaxDYrURaQ.jpg)![43|375x500](upload://1JrKaEI0Djkl2iz1RwxMDxMUa1y.jpg)
```

---
## \#1395 Posted by: clistpdx Posted at: 2018-06-25T18:36:35.525Z Reads: 248

```
You are using a newer version of the TP4056 than I am, so my wiring setup looks slightly different. According to this video (https://www.youtube.com/watch?v=Qw4psECqpwI) your version of the TP4056 has a built in battery protection IC which may not allow your battery to power your OLED if it's voltage has dropped below 2.9V or so. is your battery fully charged in order to rule this out? I don't know enough about these things to say for sure, but if your battery already has a low-voltage protection circuit built in then maybe you don't need this version of the TP4056...or perhaps it's even what is causing you troubles.
```

---
## \#1396 Posted by: adrianlee Posted at: 2018-06-25T18:53:48.733Z Reads: 245

```
Thanks for trying to help. 
I tested and, battery was 3.9V, and oled vcc/gnd showed 5.19V, same as from booster out.
Doesn't make sense for the oled not to work

Charger module if it matters: https://m.aliexpress.com/item/1852201781.html?
```

---
## \#1397 Posted by: clistpdx Posted at: 2018-06-25T19:01:04.171Z Reads: 242

```
Any chance you have the more standard 4056 module on hand to try? (https://www.ebay.com/itm/Micro-USB-5V-1A-TP4056-Lithium-Li-Battery-Charging-Board-Charger-Module/182108324849?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649)
```

---
## \#1398 Posted by: adrianlee Posted at: 2018-06-25T19:09:19.009Z Reads: 246

```
No I have only one type. As the voltage to booster is fine it should work. I guess I could measure current but oleds shouldn't need much

update: 
 I changed the switch and if I reset the nano while powered the oled turns on. I guess there's some timing issue that the oled powers up too slow to register IC2 address before nano boots
```

---
## \#1399 Posted by: clistpdx Posted at: 2018-06-30T07:40:51.333Z Reads: 259

```
Does anyone know what changes should be made in the sketch to get this remote to show miles per hour (MPH) instead of kilometers per hour (KPH)? I'm guessing I need to adjust the math here:

[CODE]
        
          switch (displayData){
          case 0:
          value = ratioRpmSpeed * data.rpm;
          suffix = "KMH";
          prefix = "SPEED";
          decimals = 1;
          break;
[/code]

Has anyone already done this and would care to share their work? Would it be as simple as updating the 'value' line to read:
[code]
value = ratioRpmSpeed * data.rpm / 1.60934;
[/code]
Or do I need to make the conversation to MPH further upstream in the code?
```

---
## \#1400 Posted by: mptrs Posted at: 2018-06-30T10:37:39.074Z Reads: 257

```
Finally got to finishing the remote. Looks awesome! Now some waiting for some pieces for the receiver. And than adjusting to thumb instead of trigger. Let's see how that goes.

Thx for the great remote @solidgeek, will donate you a beer!

![IMG_4638|666x500](upload://dwgwkp6iZxjX0wJKAZrE0nk9JSw.JPG)

No the photo is not mirrored, it's build for a lefty!!
```

---
## \#1401 Posted by: Jc06505n Posted at: 2018-06-30T12:32:47.076Z Reads: 241

```
I was actually in the process of adding it myself. I was ganna do so put adding it as a settings feature and depending on which setting is selected is what’s displayed.
```

---
## \#1402 Posted by: clistpdx Posted at: 2018-06-30T15:26:55.457Z Reads: 230

```
That’s the right way to do it! Let me know what you come up with
```

---
## \#1403 Posted by: Jc06505n Posted at: 2018-06-30T15:45:06.495Z Reads: 233

```
Probably won’t touch It until next Saturday due to classes. Also seeing if I can implement a blinking battery icon upon charging, should be easy since the Bluetooth icon does the same.
```

---
## \#1404 Posted by: Andy87 Posted at: 2018-06-30T21:13:28.362Z Reads: 229

```
Relaxe they will sent it soon.
With my order it took also 7-9 days till they shipped
```

---
## \#1405 Posted by: erod998 Posted at: 2018-07-01T22:37:22.060Z Reads: 224

```
What would cause the display to be frozen at the Firefly start screen?
```

---
## \#1406 Posted by: SeeTheBridges Posted at: 2018-07-01T23:06:24.485Z Reads: 225

```
A lot of things could. It's most likely a short on your NRF board tho. Double check all your solder joints
```

---
## \#1407 Posted by: erod998 Posted at: 2018-07-01T23:12:42.428Z Reads: 227

```
Boom. 3v3 on the NRF came out. Fixed and hot glued for the future. Thanks! Now to get telemetry working..
```

---
## \#1408 Posted by: erod998 Posted at: 2018-07-02T00:30:03.162Z Reads: 244

```
Using the development branch, why do I get this error?
"Set serial port was not declared in this scope"
The error occurs in the setup function.
void setup()
{

  #ifdef DEBUG
    SetDebugSerialPort(&Serial);
    Serial.begin(115200);
    DEBUG_PRINT("** Esk8-remote receiver **");
    printf_begin();
  #else
    #ifndef FIREFLYPCB
      // Using RX and TX to get VESC data
      SetSerialPort(&Serial); ----Error here.
      Serial.begin(115200);
    #endif
  #endif
```

---
## \#1409 Posted by: SeeTheBridges Posted at: 2018-07-02T00:33:52.257Z Reads: 230

```
You're not using the VESC6 branch of the vescUART library
```

---
## \#1410 Posted by: ron Posted at: 2018-07-02T07:01:34.494Z Reads: 230

```
Hi there! Is there an easy way to revert the max/min Positions respective reverse the throttle. Because if I'm pressing the thumbwheel up I get lower throttle numbers and if I'm pushing the wheel down I get higher value readings...

So what do I need to change in the code to get this properly running?
And wouldn't it be good to implement this feature in the Settings menu to be able to switch to inverted throttle?

Thanks in advance?
```

---
## \#1411 Posted by: solodros Posted at: 2018-07-02T07:25:48.481Z Reads: 226

```
Interchange the N and S poles of the magnet
```

---
## \#1412 Posted by: ron Posted at: 2018-07-02T08:54:14.016Z Reads: 247

```
Yeah, I thought that would be the easiest way... Done that...

But another serious issue. I built this remote like many months ago, and didn't get freezes of the arduino whatsoever. 
Today I flashed the code from the developement branch and it worked first flawelessly, arduino boots up properly and it worked out of the box. Then I wen to the settings changed the ranges and exited the Settings, still no problems. Turned it of, and on again to get into the settings, then wanted to generate an adress, and then it froze up. 

Now the remote freezes up at the firefly logo or after a while on the info screen, or sometimes after pushing the throttle.

I tried to reflash the arduino with the firmware, it flashes but the problem remains with the random freezes of the Arduino. I also resoldered all pins on the arduino and the display and the NRF24 module.

I didn't set up the receiver so maybe the unavailable receiver is messing up the Arduino after a while?!

Is it a common problem? I tried to search the thread for "freeze" but didn't get any usable result.

And is there a way to reset/erase the EEPROM? Maybe it's due to the settings in the EEPROM?!

Thanks in advance.
Ron
```

---
## \#1413 Posted by: solidgeek Posted at: 2018-07-02T11:03:17.006Z Reads: 237

```
If you haven't connected a nrf module it could crash - I haven't tested it. I cant think of anything else. You can try to erase the settings by adding the function setDefaultEEPROMSettings() in the setup. However it should not be the issue :-)
```

---
## \#1414 Posted by: erod998 Posted at: 2018-07-02T17:14:00.023Z Reads: 239

```
To use the VESC 6 library do I have to have a VESC 6? I have a 4.xx. This is my current state of telemetry: New package: '0-543-0'
New package: '0-543-0'
New package: '0-557-0'
New package: '0-568-0'
New package: '0-550-0'
New package: '0-547-0'
New package: '0-557-0'
New package: '0-561-0'
New package: '0-543-0'
New package: '0-557-0'
New package: '0-561-0'
From the receiver. No data shows on the remote.
```

---
## \#1415 Posted by: ron Posted at: 2018-07-02T18:01:23.099Z Reads: 232

```
Thanks for the fast reply... I have connected all parts but still it is crashing.. witth the initial version of the firmware I didn't have such problems but after upgrading to current version even tho I downgraded to the initial firmware version I have this issue now of randomly freezing Arduino.
```

---
## \#1416 Posted by: mptrs Posted at: 2018-07-02T18:02:21.507Z Reads: 244

```
Off to buy some capacitors for the receiver. What voltage should they be?

"A good mix would be a 220uF, a 10uF and a 100nF capacitor in parallel." 16V good enough?

And is it still needed when I add the 220uF to the arduino and add a 22pF to the reset - ground. (this is from the video of @SeeTheBridges) 

Bit confused with because of the build video and the guide.
```

---
## \#1417 Posted by: erod998 Posted at: 2018-07-02T18:22:12.047Z Reads: 255

```
I am using this library for my VESC 4:
https://github.com/RollingGecko/VescUartControl/tree/imartinezl-master

No battery, and the distance and speed:
![com-optimize-3|225x400](upload://wCe7ceBtub5bUaz8J3UYJjQdrbv.gif)
```

---
## \#1418 Posted by: erod998 Posted at: 2018-07-02T18:24:08.284Z Reads: 250

```
Here are what I am using for the power filter capacitors. Voltages don't really matter as long as they are more than 6v.

https://www.mouser.com/ProductDetail/594-K104K15X7RF53H5

https://www.mouser.com/ProductDetail/140-RGA100M1VBK0511G

https://www.mouser.com/ProductDetail/140-RGA221M1EBK0811G

In case you need a power switch:
https://www.mouser.com/ProductDetail/612-EG1201

I suggest you order some spares in case you break a lead off or something. I ordered two of each especially since how cheap they are.
```

---
## \#1419 Posted by: SeeTheBridges Posted at: 2018-07-02T19:04:18.418Z Reads: 236

```
The VESC6 library is backwards compatible.

@mptrs I can't confirm whether you still need the reset cap if you're using Geeks schematic for the power filter. My remotes don't have them, so I include the reset-GND caps. You'll just have to tell us if it works without!
```

---
## \#1420 Posted by: erod998 Posted at: 2018-07-02T19:09:39.767Z Reads: 239

```
I am not using the GND to reset cap and I haven't had a problem yet, however that has been only 15 miles.
```

---
## \#1421 Posted by: junwoo091400 Posted at: 2018-07-02T19:28:05.685Z Reads: 240

```
If anyone is interested, check out my [thingiverse thing](https://www.thingiverse.com/thing:2821982) to see my nrf24_Remote mod with PCB. It's got a longer handle. I am in testing phase and have verified solid radio connection and OLED and communication with VESC and so on. Hope you guys are making awesome remotes too! This project is exciting :)
```

---
## \#1422 Posted by: mptrs Posted at: 2018-07-02T22:43:15.039Z Reads: 243

```
@SeeTheBridges you did your build after or before the guide? I think you have the 220uF to fix the power issue. And the 22pF is for fixing the arduino not getting stuck in setup I guess.

I'm not that into all the capacitor and resistor stuff hehe. But you never had any with power drops?
```

---
## \#1423 Posted by: mptrs Posted at: 2018-07-02T22:43:39.613Z Reads: 249

```
Thx for the help, will order from Ali :)
```

---
## \#1424 Posted by: SeeTheBridges Posted at: 2018-07-02T23:16:01.432Z Reads: 241

```
Which guide? I built my first remote prior to Solidgeek's written guide, but for my video series, I think all but the first part came out after the written guide from Solidgeek. I've also since that first remote switched to 100uF caps with no power issues.
```

---
## \#1425 Posted by: sofu Posted at: 2018-07-05T07:45:12.493Z Reads: 235

```
I'm also having this issue with the crazy values... I have the latest firmware from the dev branch flashed...
```

---
## \#1426 Posted by: erod998 Posted at: 2018-07-05T07:50:51.613Z Reads: 234

```
Got my working and using mph now. After I cleared the Arduono IDE of all VESC libraries, restarted nd reinstalled the libraries, and reflagged the receiver and remote.
```

---
## \#1427 Posted by: sofu Posted at: 2018-07-05T07:53:23.357Z Reads: 238

```
Was there any specific way you reinstalled the VescUartControl library or a specific way you reconnected the receiver and remote?
```

---
## \#1428 Posted by: erod998 Posted at: 2018-07-05T07:56:39.441Z Reads: 249

```
When you download the library, it should be a zip. Go to sketch then include library then add zip library or something. Then connect one of the arduinos and hit upload. Maybe unplug them after, and then make sure they both are connected to each other. The wireless icon should be solid, not flashing.
```

---
## \#1429 Posted by: clistpdx Posted at: 2018-07-05T17:53:55.823Z Reads: 264

```
Does anyone know where I would point the D-, D+, ID pins on the my external micro USB jack so that it can double as a charger AND upload code to the Nano?
Does Rx = D- and  Tx = D+ ?
![12%20AM|663x500](upload://4RKCXRS4o0uuow8O6Woc4MrNeru.jpg)
```

---
## \#1430 Posted by: SeeTheBridges Posted at: 2018-07-05T21:29:55.939Z Reads: 259

```
Unfprtunately you need to to go through the arduino USB port to do so. Unless you added another external USB to serial converter in there. But why do that when there's already a CH40g on the board haha

Sofu used a 4 pin micro USB breakout on her remote, I use the 5 pin breakouts on mine. Then you just have to match the pin outs. 

On your picture there, from left to write the pins are 1-5. The data pins just need to match pins 2 and 3 on a microUSB breakout. On my remotes though, I have to use another cable feeding pin 5 too for some reason. Sofu only needs 2 and 3.
```

---
## \#1431 Posted by: clistpdx Posted at: 2018-07-05T22:05:55.318Z Reads: 253

```
Thanks for the info. Do you have a link to the 4- or 5-pin breakouts that would work? I don't think I'm using the right search terminology and all I'm coming up with are [basic ones like these](https://www.aliexpress.com/item/10PCS-CJMCU-Breakout-Power-Supply-Module-Micro-USB-Interface-Power-Adapter-Board-USB-5V-Breakout-Module/32827910858.html?spm=2114.search0104.3.28.2b8964baiv2VTq&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10130_10068_10324_10547_10342_10325_10546_10343_10340_10548_10341_10545_10696_10084_10083_10618_10307_10059_100031_524_10103_10624_10623_10622_10621_10620,searchweb201603_31,ppcSwitch_4&algo_expid=8bc8d880-b017-4498-8d01-89bb2193e0ac-4&algo_pvid=8bc8d880-b017-4498-8d01-89bb2193e0ac&priceBeautifyAB=0). I imagine I'm looking for something with a male micro USB end on it?
```

---
## \#1432 Posted by: SeeTheBridges Posted at: 2018-07-05T22:08:26.131Z Reads: 265

```
These are the ones sofu used: https://www.amazon.com/Micro-Male-5-Pin-Solder-Connector/dp/B00OK8ELNA/ref=pd_sbs_147_2?_encoding=UTF8&pd_rd_i=B00OK8ELNA&pd_rd_r=TRC6K560GY88YB8JY6BH&pd_rd_w=QR00U&pd_rd_wg=Zeeqp&psc=1&refRID=TRC6K560GY88YB8JY6BH

They only need 2 wire apparently. I'm not gonna link mine since this appears way easier than dealing with my 3 wire solution
```

---
## \#1434 Posted by: DjamboBuksne Posted at: 2018-07-09T09:06:51.363Z Reads: 260

```
Hey @solidgeek, can I make remotes and sell them on the forum?
```

---
## \#1435 Posted by: rey8801 Posted at: 2018-07-10T06:00:28.298Z Reads: 273

```
Finally I can start. Now I just need to find the time :laughing: Really curious to see how it goes.

![IMG_20180710_075717|281x500](upload://4lgH2Mp8mKC3I3DNgyoQoIBh1qg.jpg)![IMG_20180710_075506|690x388](upload://nAgwswpHQWdZYjjUidJwmFhGo2V.jpg)![IMG_20180710_075656|690x388](upload://jj6hCdHIBeAaUJkoLpUMrfhY1fu.jpg)![IMG_20180710_075200|690x388](upload://jQ9zYPgBVyu6am4cZUtgETURBGx.jpg)
```

---
## \#1436 Posted by: Travo Posted at: 2018-07-10T16:28:40.630Z Reads: 267

```
Hey everyone, I got the usb type C female port and it works fine.  As you can see in I should be able to shave off half the board and solder directly to the G and than to the V spot to get the 4.74V ![IMG_20180710_122323|375x500](upload://4G0kF9o4ju2O2HAz639bg2dLM6j.jpg) 
Now if I really wanted to I could attempt to solder onto the tiny pins to really minimize the size but we'll see
```

---
## \#1437 Posted by: rey8801 Posted at: 2018-07-11T13:55:12.285Z Reads: 269

```
Question, when I try to uploadthe trasmitter.ino file I get this error
Arduino: 1.8.5 (Windows 7), TD: 1.41, Board: "Arduino Nano, ATmega328P"

C:\Users\Administrator\Desktop\ESkate\FireFly Remote\nRF24-Esk8-Remote-development\transmitter\transmitter.ino:15:21: fatal error: U8g2lib.h: No such file or directory

 #include <U8g2lib.h>

                     ^

compilation terminated.

exit status 1
Error compiling for board Arduino Nano.

It seems the U8g2lib.h library is missing. Do you know how to solve it?
Moreover in this sketch I do not see the raw where @SeeTheBridges advices to change the pipe sequence. Is It automatic now?
Thx
```

---
## \#1438 Posted by: Surfer Posted at: 2018-07-11T13:58:40.971Z Reads: 253

```
You have to look for the libraries of the LCD in the ide, and yes now the pipe address you can change it in settings
```

---
## \#1439 Posted by: rey8801 Posted at: 2018-07-11T14:03:29.322Z Reads: 257

```
Thx, I checked in IDE in manage libraries but I do not find it. Do you know what to search?

EDIT: I found U8g2 from Oliver for monocrome display, is it the right one?
```

---
## \#1440 Posted by: clistpdx Posted at: 2018-07-11T14:09:56.298Z Reads: 263

```
Search 'U8G2'. Be sure the change 'type' to ALL rather than 'updateable':
![59%20AM|690x292](upload://dTtgHvhFUQuYEVBd6SJ3u8CwwTH.png)
The pipe is on line 126 in my code:
![32%20AM|690x81](upload://9AnebjdqdGEFxkqZyate90CciDe.png)
```

---
## \#1441 Posted by: Surfer Posted at: 2018-07-11T14:10:25.420Z Reads: 251

```
Yeah! :) 10 chars
```

---
## \#1442 Posted by: rey8801 Posted at: 2018-07-11T14:10:58.208Z Reads: 253

```
I download the one from Oliver, I hope it is correct. Now it asks for the RF24.h one
Which one is it?

OK the U8g2 is correct, nice
```

---
## \#1443 Posted by: rey8801 Posted at: 2018-07-11T14:21:25.470Z Reads: 254

```
I installed the RF24 library from TMRh20 I hope it is correct. Then the upload succeed, although I got the message
C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-master\VescUart.cpp: In function 'int PackSendPayload(uint8_t*, int)':

C:\Users\Administrator\Documents\Arduino\libraries\VescUartControl-master\VescUart.cpp:139:21: warning: converting to non-pointer type 'uint8_t {aka unsigned char}' from NULL [-Wconversion-null]

  messageSend[count] = NULL;

                     ^
Something wrong?
```

---
## \#1444 Posted by: clistpdx Posted at: 2018-07-11T14:34:38.107Z Reads: 246

```
I think I got that same error. I just ignored it. But maybe someone here w/ more arduino knowledge can explain it
```

---
## \#1445 Posted by: halfbro Posted at: 2018-07-11T14:38:36.604Z Reads: 255

```
They are just warnings, you don't have to worry about them too much.

You can tell its a warning because of the little text in brackets at the end, `[-Wconversion-null]`. That means whatever code came before it triggered that warning. All warnings start with `-W`.
```

---
## \#1446 Posted by: rey8801 Posted at: 2018-07-11T14:41:17.850Z Reads: 257

```
@clistpdx @halfbro thx guys! And what about the RF24 library. Did I install the correct one?
```

---
## \#1447 Posted by: clistpdx Posted at: 2018-07-11T15:54:27.287Z Reads: 255

```
I don't have access to my arduino stuff right now because I'm at work, but I can look tonight.
```

---
## \#1448 Posted by: rey8801 Posted at: 2018-07-11T15:58:41.925Z Reads: 267

```
Many Thx! 10ch
```

---
## \#1449 Posted by: rey8801 Posted at: 2018-07-11T18:51:38.965Z Reads: 282

```
It looks really good! Although I am not totally sure about the the shape, I like the wheel but the whole remote it's a bit too long for my taste. Maybe is because I am use to the Nano-X. I may design a new enclosure for it. 
![IMG_20180711_204235|690x388](upload://yOt465MxW2w7H7snJQFZXCkI7vy.jpg)![IMG_20180711_204153|690x388](upload://1f8UbP0UpP80S1EsrFW70WBodDq.jpg)![IMG_20180711_204214|690x388](upload://ifik9MR3FibDFZSoVmRAeXR7MA3.jpg)

Edit: First ride went fine! This thing is really nice... I will build more in next weeks, I have part left anyway :grin:

https://youtu.be/05wjP5dEqa8
```

---
## \#1450 Posted by: mptrs Posted at: 2018-07-12T18:00:14.002Z Reads: 274

```
Yeah it was Solidgeeks guide. Got my parts, so gonna follow your video and see where I get. Thanks for the videos and all the research.
```

---
## \#1451 Posted by: DoodleDinosaur Posted at: 2018-07-15T23:21:48.863Z Reads: 269

```
First time posting here, just wanna say that @solidgeek has done an awesome job.

I started my own design the other day also modelled after the boosted board but a bit more basic than this. (Simple PWM/PPM, no feedback from the VESC) all on one board.

If anyone is interested I can share my schematic/PCB files (done in Eagle) once I'm finished. I'm hoping to design the board so that it fits in the same housing without modifying the actual mechanical design.
```

---
## \#1452 Posted by: dfairlite Posted at: 2018-07-15T23:58:58.852Z Reads: 266

```
I'm going to build a few of these if anyone is interested pm me. These things look awesome, thanks @solidgeek
```

---
## \#1453 Posted by: Deakbannok Posted at: 2018-07-17T09:25:35.284Z Reads: 270

```
![51Cx0j0ng3L|500x500](upload://gwZPiAyhICaHVzaMQjYVebTej7Z.jpg)

For anyone that want to switch to a smaller NRF24L01+ 
![NRF24-Mini-02|278x338](upload://7ZAEeNJJPmpoKfoRxYRh7gvKQL8.jpg)
It shorter than the ceramic one and less power consumption.
```

---
## \#1454 Posted by: rey8801 Posted at: 2018-07-17T10:15:15.570Z Reads: 266

```
I personally used this module on both receiver and Transmitter and I get stronger signal within 5m between walls. Didn't test outside, i guess it would be more. It's also smaller than nrf24 ceramic module. 
https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/303?u=rey8801
:grin:
```

---
## \#1455 Posted by: Deakbannok Posted at: 2018-07-17T16:41:27.287Z Reads: 257

```
adding code for auto stop to a reciever is a good idea. incase of lost connection between TX and RX. your board will slow itself to stop.
```

---
## \#1456 Posted by: mmaner Posted at: 2018-07-17T16:44:48.716Z Reads: 259

```
I'm gong to wholeheartedly disagree with that.  

The reason we all get rid of 'Limit ERPM with Negative Torque' is because you begin by flying off the board and end by looking for your teeth, same situation if you apply negative torque on disconnect :).

![image|217x70](upload://v3oevROsx6w6zLMqyYijPYqiT4D.png)
```

---
## \#1457 Posted by: Deakbannok Posted at: 2018-07-17T17:46:38.563Z Reads: 256

```
[quote="mmaner, post:1456, topic:28543"]
Limit ERPM with Negative Torque
[/quote]

What I meant is applying the negative torque slowly 10+ seconds from Neutral to stop. Enough time to brace yourself. And that is only applied when the Controller WAS connected.
```

---
## \#1458 Posted by: webst Posted at: 2018-07-17T19:07:09.043Z Reads: 246

```
I see it working but it would need more precise feedback algorithm, probably one that Benjamin is going to work on soon (as Frank says will be better than anything out there and easily better than watt mode). Hope it's true, for now I'm with @mmaner.
```

---
## \#1459 Posted by: DoodleDinosaur Posted at: 2018-07-17T22:46:10.340Z Reads: 250

```
[quote="DoodleDinosaur, post:1451, topic:28543"]
I started my own design the other day also modelled after the boosted board but a bit more basic than this. (Simple PWM/PPM, no feedback from the VESC) all on one board.
[/quote]

If anybody is interested in the schematic here's a link to the file.
You'll notice I've used a different battery to the one used by solidgeeks. If you want to use another battery you'll have to tweak the sense resistor value but that's in the datasheet for the charge controller

[Onedrive link to .sch file](https://1drv.ms/u/s!Au7zmpbmrX9Dim_PmhNqDGf-7K8f)

Like I said earlier this is a very simple design, it's based off an ATTiny85 and outputs just the PWM as personally I'm not interested in the telemetry data. I'm interested in just going and stopping :grinning:

I've ordered some boards which should arrive in a few weeks. I'd post the .brd file but until I can guarantee it works I don't want to waste anybody's time. 

Price works out to ~£25 but there's a lot of soldering involved.
Will post some pics as I go if anyone is interested
```

---
## \#1460 Posted by: Wentworth Posted at: 2018-07-25T07:45:30.159Z Reads: 244

```
Hello, I have been using it for a while. But I think its Generate address has a bit of a problem. It will switch values immediately. Sometimes there is no response, can anyone tell me why? Still my operation problem. How can I deal with this problem? I want to make it better
```

---
## \#1461 Posted by: Deakbannok Posted at: 2018-07-25T14:38:09.355Z Reads: 257

```
So is not synchronizing to the RX? because TX and have to get RX to change its address pipe and send back confirmation back to TX first before the TX can take effect. 
I have added a fix to the code. 

I also added the auto deacceleration to STOP the board from running away if the controller is disconnected whilst riding. The code will apply brake slowly until it reach a minimum throtlle. And after 30 sec the code will set the throttle back to neutral position.

3 profiles for each controller. Now you can use only one controller for 3 different boards and settings :smiley:
```

---
## \#1462 Posted by: Wentworth Posted at: 2018-07-26T01:33:19.772Z Reads: 250

```
My receiver has received a signal, but sometimes it can be changed at once, sometimes for a long time. My receiver is always on. A new address cannot be generated after using the "Generate Address" multiple times. Is it only me that one person has this problem?
```

---
## \#1463 Posted by: Deakbannok Posted at: 2018-07-26T04:23:21.385Z Reads: 249

```
Try out my code. basicly is a copy from solidgeek with a few changes. See if you are still experiencing problem.
```

---
## \#1464 Posted by: junwoo091400 Posted at: 2018-07-26T18:35:40.584Z Reads: 247

```
Hmm I don't see any links to your repository/file. Where can I find your code?
```

---
## \#1465 Posted by: Deakbannok Posted at: 2018-07-27T17:05:48.985Z Reads: 251

```
https://github.com/deakbannok/Arduino-Nano-Controller
```

---
## \#1466 Posted by: junwoo091400 Posted at: 2018-07-27T19:12:04.740Z Reads: 253

```
Very nice code. I will look more into it in the morning.
Btw, function uint64ToString is actually not properly defined... But since upper 32 bits are always 0 for this use case, it doent show any errors
```

---
## \#1467 Posted by: erod998 Posted at: 2018-07-31T22:42:11.347Z Reads: 268

```
My receiver isn't connecting now. 

Here is the serial output from the receiver:
** Esk8-remote receiver **
Settings loaded
Printing receiver details
STATUS		 = 0x00 RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=0 TX_FULL=0
RX_ADDR_P0-1	 = 0x0000000000 0x0000000000
RX_ADDR_P2-5	 = 0x00 0x00 0x00 0x00
TX_ADDR		 = 0x0000000000
RX_PW_P0-6	 = 0x00 0x00 0x00 0x00 0x00 0x00
EN_AA		 = 0x00
EN_RXADDR	 = 0x00
RF_CH		 = 0x00
RF_SETUP	 = 0x00
CONFIG		 = 0x00
DYNPD/FEATURE	 = 0x00 0x00
Data Rate	 = 1MBPS
Model		 = nRF24L01
CRC Length	 = Disabled
PA Power	 = PA_MIN
Setup complete - begin listening
New package: '0-0-0'
Getting VESC data
New package: '0-0-0'

Transmitter:
STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0
RX_ADDR_P0-1	 = 0xe8e8f0f0e1 0xc2c2c2c2c2
RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6
TX_ADDR		 = 0xe8e8f0f0e1
RX_PW_P0-6	 = 0x20 0x00 0x00 0x00 0x00 0x00
EN_AA		 = 0x3f
EN_RXADDR	 = 0x03
RF_CH		 = 0x6c
RF_SETUP	 = 0x07
CONFIG		 = 0x0e
DYNPD/FEATURE	 = 0x3f 0x06
Data Rate	 = 1MBPS
Model		 = nRF24L01+
CRC Length	 = 16 bits
PA Power	 = PA_MAX
e8e8f0f0e1: Failed transmission

Checked continuity on all the wires to the Nanos. Maybe a NRF is bad?
```

---
## \#1468 Posted by: monter_man Posted at: 2018-08-03T01:54:10.322Z Reads: 248

```
hi I tried the code for from both (solidgeek and deakbannok) and still cannot get the nrf to connect.

any pointers?

the wireless icon on the screen flashes constantly
```

---
## \#1469 Posted by: Wentworth Posted at: 2018-08-03T06:31:51.506Z Reads: 259

```
![image|690x52](upload://ywuhIBcniI9q4wNBM2dVucXLNsa.png)
![image|690x380](upload://pI3iXtkyWCRg5CdKI5FxLZMJFVC.png)
gear ratio = WheelPulley / MotorPulley.
Although the process is correct, I think your name is easy to misunderstand others.
```

---
## \#1470 Posted by: Wentworth Posted at: 2018-08-03T07:23:45.625Z Reads: 235

```
Can anyone tell me the calculation principle of speed and distance, whether there is any reference material？
```

---
## \#1471 Posted by: monter_man Posted at: 2018-08-06T16:43:50.858Z Reads: 243

```
HI, did you get yours to work.  I have 3 nrf modules and tried all interchanging all 3 without any luck, I cannot get them to connect receiver/transmitter!  spent almost half a day doing tests and rewiring...

any help is welcome.
```

---
## \#1472 Posted by: SeeTheBridges Posted at: 2018-08-06T17:04:00.991Z Reads: 242

```
Your receiver is either shorting, or not wired up properly all those 0x00's mean no information is being communicated between the NRF and the Arduino. The NRF could also just be bad.

@monter_man What do you get with debug turned on?
```

---
## \#1473 Posted by: erod998 Posted at: 2018-08-09T19:18:20.427Z Reads: 249

```

Switched the Tx's NRF...again. Still will not connect.
STATUS		 = 0xff RX_DR=1 TX_DS=1 MAX_RT=1 RX_P_NO=7 TX_FULL=1
RX_ADDR_P0-1	 = 0xffffffff7f 0xffffffffff
RX_ADDR_P2-5	 = 0x7f 0xff 0x7f 0xff
TX_ADDR		 = 0xffffffff7f
RX_PW_P0-6	 = 0xff 0x7f 0xff 0x7f 0xff 0x7f
EN_AA		 = 0xff
EN_RXADDR	 = 0x7f
RF_CH		 = 0xff
RF_SETUP	 = 0x7f
CONFIG		 = 0x7f
DYNPD/FEATURE	 = 0x7f 0xff
Data Rate	 = 1MBPS
Model		 = nRF24L01
CRC Length	 = 16 bits
PA Power	 = PA_MAX
041004b0a: Failed transmission

The Rx is:
⸮⸮<⸮⸮<** Esk8-remote receiver **
Settings loaded
Printing receiver details
STATUS		 = 0x00 RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=0 TX_FULL=0
RX_ADDR_P0-1	 = 0x0000000000 0x0000000000
RX_ADDR_P2-5	 = 0x00 0x00 0x00 0x00
TX_ADDR		 = 0x0000000000
RX_PW_P0-6	 = 0x00 0x00 0x00 0x00 0x00 0x00
EN_AA		 = 0x00
EN_RXADDR	 = 0x00
RF_CH		 = 0x00
RF_SETUP	 = 0x00
CONFIG		 = 0x00
DYNPD/FEATURE	 = 0x00 0x00
Data Rate	 = 1MBPS
Model		 = nRF24L01
CRC Length	 = Disabled
PA Power	 = PA_MIN
Setup complete - begin listening
New package: '0-0-0'
Getting VESC data

Getting completely new NRFs tommorow so I’ll try that. Maybe one of the ones I replaced is bad
```

---
## \#1474 Posted by: Deakbannok Posted at: 2018-08-11T19:26:47.646Z Reads: 248

```
Can you show us your wiring picture.


sorry I was on vacation.![20180807_145423|690x388](upload://yjoIbrGkjCJygY8KcYpuWcmSDG4.jpg)![20180806_161733|281x500](upload://d1hLe6zt45PrJJXtmrF5E91G053.jpg)

I did a over 130km across the passes from Chiang Mai to Pai. It tooks 3 charges to complete the route.
```

---
## \#1475 Posted by: neiru37 Posted at: 2018-08-13T11:45:10.696Z Reads: 232

```
Hey everyone, I can't seem to get telemetry working. How can I match my vesc's baud rate with my receiver's? How do I know what my receiver's baud rate is? I'm using a Focbox with Ackmaniac 3.102 together with an arduino nano (non firefly PCB), dev branch of solidgeek's code and master branch of rollinggecko's code.
```

---
## \#1476 Posted by: Pedrodemio Posted at: 2018-08-13T11:55:27.231Z Reads: 240

```
Probably the packet in Ackmaniac's  is different than the one in the rolling gecko library, you need to compare the bldcmeasure or mc_values struct of booth to see if they are equal

I had this problem with the newer firmwares since Vedder is always adding more things

    struct bldcMeasure {
	float tempFET;
	float tempMotor;
	float avgMotorCurrent;
	float avgInputCurrent;
	float FOCcurrentD;
	float FOCcurrentQ;
	float dutyCycleNow;
	float rpm;
	float inpVoltage;
	float ampHours;
	float ampHoursCharged;
	float wattHours;
	float wattHoursCharged;
	long tachometer;
	long tachometerAbs;
	mc_fault_code fault_code;
	float position;
```

---
## \#1477 Posted by: Pimousse Posted at: 2018-08-13T12:32:29.221Z Reads: 230

```
This structure matches FW from 3.34 to 3.39.

Until now, I always managed to have Rollinggecko's library working by adding new elements in deserialization.
However with FW3.40, by adding 1 byte more (vesc ID) in COMM_GET_VALUES packet, I encounter an issue of packet shorter than expected.

Actually, it seems that now we reach serial buffer limit of Arduino (64 bytes).
Packet is : 1 start byte + 1 size type byte + 1 length byte + 59 bytes Payload + 2 CRC bytes + 1 stop byte = 65 bytes... :confounded:
The trick to increase buffer size is to modify SERIAL_BUFFER_SIZE in internal file of Arduino core (HardwareSerial.h).
Not that hard to do, but it's not as simple as just adding a library for beginners. :confused: 

This is just a clue, I need to test. But that really makes sense.
```

---
## \#1478 Posted by: neiru37 Posted at: 2018-08-13T18:50:22.401Z Reads: 229

```
Hi, thanks for your reply

[quote="Pedrodemio, post:1476, topic:28543"]
bldcmeasure or mc_values
[/quote]

mc_values struct seems to be the same on ackmaniac's firmware:

    	float v_in;
	float temp_mos1;
	float temp_mos2;
	float temp_mos3;
	float temp_mos4;
    float temp_mos5;
    float temp_mos6;
    float temp_pcb;
    float current_motor;
    float current_in;
    float rpm;
    float duty_now;
    float amp_hours;
    float amp_hours_charged;
    float watt_hours;
    float watt_hours_charged;
    int tachometer;
    int tachometer_abs;
    mc_fault_code fault_code;

I can't seem to find the `bldcMeasure` struct within ackmaniac's firmware. Where is it usually stored? Or is ghe `bldcMeasure` struct only within the scope of rollinggecko's library?
```

---
## \#1479 Posted by: Pedrodemio Posted at: 2018-08-13T19:18:35.673Z Reads: 213

```
Only on the library, you have to see if booth of them match and probably adjust the bit size if I’m not mistaken

I have a library modified by @Pimousse that works on 3.33, if you want I can send for you to try
```

---
## \#1480 Posted by: Pimousse Posted at: 2018-08-13T19:23:58.540Z Reads: 218

```
@neiru37, which FW are you running ?
Check my librairies here :
https://drive.google.com/open?id=13ZL37tD0YRZzcL2XTEyNG4uAA-xMj4O9 

Regarding the buffer size, I'm still struggling to have it working even after had modified the Arduino core :pensive:
BTW, I opened an issue on Vedder's BLDC repo. Will see...
```

---
## \#1481 Posted by: Pedrodemio Posted at: 2018-08-13T19:26:14.455Z Reads: 218

```
Didn’t see your message first, that sucks, I get that new features have to be added, but breaking up a function by upgrading is no good

I’m still on 3.34 by fear of the library stop working again
```

---
## \#1482 Posted by: Pimousse Posted at: 2018-08-13T19:28:03.378Z Reads: 212

```
I confirm that the library (VESC_FW_from_v3.34) is fine up to FW3.39.
```

---
## \#1483 Posted by: Pedrodemio Posted at: 2018-08-13T19:30:05.914Z Reads: 210

```
Thanks, I will update it

I think the only significant change it the handbrake
```

---
## \#1484 Posted by: neiru37 Posted at: 2018-08-13T20:15:50.416Z Reads: 225

```
[quote="Pimousse, post:1480, topic:28543"]
which FW are you running ?
[/quote]

Ackmaniac 3.01, rollinggecko master, solidgeek development

[quote="Pimousse, post:1482, topic:28543, full:true"]
I confirm that the library (VESC_FW_from_v3.34) is fine up to FW3.39.
[/quote]

Fine as in it works with the firefly firmware?

EDIT: Nvm this is the firefly firmware
```

---
## \#1485 Posted by: Pimousse Posted at: 2018-08-13T20:24:14.164Z Reads: 211

```
Don't know, I don't have a Firefly.

**I finally got FW3.40 working !!!**
What a pain in the a** ! I needed to activate compilation output in Preferences then seek for the path of `HardwareSerial.h` which is actually lost in a hidden folder in the darkness of the Hard drive... :roll_eyes:

Now, buffer size 128 for RX is quite enough for a bunch of FW update I guess :smile: 
Works with my library `VESC_FW_from_v3.40`
```

---
## \#1486 Posted by: Pedrodemio Posted at: 2018-08-13T20:28:05.450Z Reads: 207

```
Nice, can you upload it for us mortals? And what I have to change in the arduino ide?
```

---
## \#1487 Posted by: Pimousse Posted at: 2018-08-13T20:36:29.988Z Reads: 223

```
Library is already in my Google drive public (link few post above).
Well, nothing to change in Arduino IDE, but in a file in hidden directory, which obviously is different regarding your OS. 
On my mac :
`/Users/User/Library/Arduino15/packages/arduino/hardware/avr/1.6.21/cores/Arduino/HardwareSerial.h`
Open this file and look for `SERIAL_RX_BUFFER_SIZE 64`.
Change 64 by 128.
Keep in mind that every Arduino project you will code will have this extended buffer, which also take more memory of course (=less for your code).
```

---
## \#1488 Posted by: Pedrodemio Posted at: 2018-08-13T20:37:51.004Z Reads: 214

```
Thanks a lot
```

---
## \#1489 Posted by: BigBrit Posted at: 2018-08-13T20:48:57.865Z Reads: 222

```
is anyone else having issues with the two halves of the cases not meeting exactly on the long edges? I have printed out two of these now in Nylon and the case isn't an exact fit which is a shame
```

---
## \#1490 Posted by: SeeTheBridges Posted at: 2018-08-13T22:13:45.946Z Reads: 224

```
The original design file has a flaw that causes this. The MicroUSB port doesn't sit flush in the bottom half for any of my prints. So every remote has a small gap down there
```

---
## \#1491 Posted by: BigBrit Posted at: 2018-08-13T22:18:14.699Z Reads: 224

```
I just downloaded the files from thingiverse, is there a more up to date file?
```

---
## \#1492 Posted by: SeeTheBridges Posted at: 2018-08-13T22:28:09.762Z Reads: 218

```
Nope. It's the only one around. It's got some other small issues too that I wanted to address with my own small revision, but I never had the chance to get to it
```

---
## \#1493 Posted by: rey8801 Posted at: 2018-08-13T22:38:42.708Z Reads: 213

```
My does fit pretty well. It's true that the micro usb doesn't sit perfectly, what I do is just put the soldering iron on top of it while I am gently pushing it down. In this way the micro usb port will melt the hal mm plastic part that needs to fit perfectly.
```

---
## \#1494 Posted by: neiru37 Posted at: 2018-08-14T00:37:33.247Z Reads: 219

```
[quote="Pimousse, post:1485, topic:28543"]
Don’t know, I don’t have a Firefly.
[/quote]

Yes you do! The remote you're writing firmware for is the firefly lol.
```

---
## \#1495 Posted by: Pimousse Posted at: 2018-08-14T04:55:36.779Z Reads: 214

```
I don't write any firmware for any remote. :smile: 
I just came on this thread because I'm using the same library and was facing an issue that you may have also facing. ;)
```

---
## \#1496 Posted by: BigBrit Posted at: 2018-08-14T08:14:19.190Z Reads: 217

```
You are right, I loaded the model into fusion 360 and it seems to fit pretty well where I am having the issues, must be because I am printing with Nylon or something.  Will try ABS and see what happens
```

---
## \#1497 Posted by: rey8801 Posted at: 2018-08-14T08:28:47.083Z Reads: 216

```
Try PETG and you won't regret
```

---
## \#1498 Posted by: BigBrit Posted at: 2018-08-14T16:13:03.576Z Reads: 211

```
I have a roll of black PETG, ill give it a go
```

---
## \#1499 Posted by: rey8801 Posted at: 2018-08-14T16:17:25.271Z Reads: 210

```
It doesn't shrink and it is rock solid
```

---
## \#1500 Posted by: BigBrit Posted at: 2018-08-14T16:17:50.829Z Reads: 206

```
you wouldn't think nylon would either tbf
```

---
## \#1501 Posted by: rey8801 Posted at: 2018-08-14T16:33:36.730Z Reads: 211

```
If you can get it print well yes it's good too. I just find PETG the easiest and the stronger material to print.
I do not know which printer you have, but it has to be a good one since you can print nylon. If you do not have experience with petg, just use your pla profile. Lower the fan (to 0 for strength, towards 100 for nice finish) ti something in the middle, like 30-50%. PETG likes to be printed slow. So I use 40mm/sec at most. Temperature depends on the filament. Usually between 220 to 240 ^C. Run a heat tower.
```

---
## \#1502 Posted by: BigBrit Posted at: 2018-08-14T16:54:59.983Z Reads: 212

```
Thanks for the tips.

I have an ultimaker S5 and a CR-10S.  I printed PETG on the CR-10S once and it was good, slightly stringy but came out nice.  I will buy some ultimaker PETG, then I don't have to worry about the settings as someone else has already worked that out for me!!!
```

---
## \#1503 Posted by: rey8801 Posted at: 2018-08-14T17:04:16.218Z Reads: 219

```
I have a CR10S too. If you need my PETG profile just ask. I use https://www.amazon.de/SUNLU-Filament-Drucker-Dimensionsgenauigkeit-Schwarz/dp/B075Q65H5D/ref=sr_1_3?ie=UTF8&qid=1534266235&sr=8-3&keywords=petg PETG and It's good.
```

---
## \#1504 Posted by: mooose Posted at: 2018-08-15T08:09:44.523Z Reads: 228

```
Wow, what a nice remote! I'm handy but not that handy to build one myself...I'll blow up sh*t before I get something soldered correctly, hahahaa! Is anyone making these to sell? If so, what would the cost be? Really interested!
```

---
## \#1505 Posted by: Deakbannok Posted at: 2018-08-15T15:38:14.214Z Reads: 236

```
I am rework on the 3d files. Hope to improve a few minors and faster printing time with 2mm screws. And try to keep it original shape.

Printed PETG but best with Nylon for more dure on event of falls.

![20180807_113356|690x388](upload://lFA6MhbMMSlzBZUgqkGGL7W5rUf.jpg)
```

---
## \#1506 Posted by: rey8801 Posted at: 2018-08-15T16:23:13.178Z Reads: 233

```
I am planning to sell few batches of them after I used it for the past months and really like it. @solidgeek was so kind to give me the permission. I will of course send him donations for each remote sold. I am based in EU but I can ship world wild. I need a bit of time to finished other stuff before have the time to embrace this way. :wink:
```

---
## \#1507 Posted by: erod998 Posted at: 2018-08-15T18:31:22.242Z Reads: 242

```
I just don't know. I traced each connection the the arduino, even to the 328p. Tried a bunch of different NRF's, still nothing. It's killing me now because I had the remote working, even rode with it, but after two weeks of not riding it did not work. Using the development branch, tried master to get same results.
TX Output:
⸮STATUS		 = 0xff RX_DR=1 TX_DS=1 MAX_RT=1 RX_P_NO=7 TX_FULL=1
RX_ADDR_P0-1	 = 0xffffffffff 0xffffffffff
RX_ADDR_P2-5	 = 0x7f 0xff 0x7f 0xff
TX_ADDR		 = 0xffffffff7f
RX_PW_P0-6	 = 0xff 0x7f 0xff 0x7f 0xff 0x7f
EN_AA		 = 0xff
EN_RXADDR	 = 0x7f
RF_CH		 = 0xff
RF_SETUP	 = 0x7f
CONFIG		 = 0x7f
DYNPD/FEATURE	 = 0x7f 0xff
Data Rate	 = 1MBPS
Model		 = nRF24L01
CRC Length	 = 16 bits
PA Power	 = PA_MAX
041004b0a: Failed transmission

Rx Output:
** Esk8-remote receiver **
Settings loaded
Printing receiver details
STATUS		 = 0x00 RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=0 TX_FULL=0
RX_ADDR_P0-1	 = 0x0000000000 0x0000000000
RX_ADDR_P2-5	 = 0x00 0x00 0x00 0x00
TX_ADDR		 = 0x0000000000
RX_PW_P0-6	 = 0x00 0x00 0x00 0x00 0x00 0x00
EN_AA		 = 0x00
EN_RXADDR	 = 0x00
RF_CH		 = 0x00
RF_SETUP	 = 0x00
CONFIG		 = 0x00
DYNPD/FEATURE	 = 0x00 0x00
Data Rate	 = 1MBPS
Model		 = nRF24L01
CRC Length	 = Disabled
PA Power	 = PA_MIN
Setup complete - begin listening
New package: '0-0-0'
Getting VESC data


![IMG_2076|374x500](upload://43y1ARhf5ebK1bjdBU2xEeMPOZL.JPG)

Serial Output of the master branch on the Tx:
STATUS		 = 0xff RX_DR=1 TX_DS=1 MAX_RT=1 RX_P_NO=7 TX_FULL=1
RX_ADDR_P0-1	 = 0xffffffffff 0xffffffffff
RX_ADDR_P2-5	 = 0x7f 0xff 0x7f 0xff
TX_ADDR		 = 0xffffffff7f
RX_PW_P0-6	 = 0xff 0x7f 0xff 0x7f 0xff 0x7f
EN_AA		 = 0xff
EN_RXADDR	 = 0x7f
RF_CH		 = 0xff
RF_SETUP	 = 0x7f
CONFIG		 = 0x7f
DYNPD/FEATURE	 = 0x7f 0xff
Data Rate	 = 1MBPS
Model		 = nRF24L01
CRC Length	 = 16 bits
PA Power	 = PA_MAX
525
Failed transmission
423
Failed transmission
359
Failed transmission
302
Failed transmission
252
Transmission succes
207
Transmission succes
164
Failed transmission
130
Failed transmission
100
Failed transmission
80
Transmission succes
63
Transmission succes
48
Transmission succes
39
Failed transmission
33
Failed transmission
32


Not sure what the numbers mean.
```

---
## \#1508 Posted by: SeeTheBridges Posted at: 2018-08-15T19:28:29.249Z Reads: 208

```
The numbers are probably your hall sensor readings. Humor me and touch the antenna while you're trying to use the transmitter. I've found some of my ceramic NRFs don't work unless I'm touching the antenna for some reason. If that ends up being the case, I usually add an extra bit of wire to the antenna when this is the case and it clears right up
```

---
## \#1509 Posted by: erod998 Posted at: 2018-08-15T22:28:47.593Z Reads: 238

```
I can't, I do not have the ceramic antenna modules.

PA Power	 = PA_MAX
529
Failed transmission
430
Failed transmission
368
Failed transmission
312
Failed transmission
260
Transmission succes
215
Transmission succes
174
Failed transmission
138
Failed transmission
107
Failed transmission
82
Transmission succes
62
Transmission succes
48
Transmission succes


Strange that it connects then loses it.

Ok it is connecting, but erratically. Re-soldering all connections.
```

---
## \#1510 Posted by: 12382 Posted at: 2018-08-17T04:05:34.290Z Reads: 243

```
Hey you guys! Long time lurker, first time poster.

But I successfully built a remote and connected it to my board! I have set up the PPM and it works just fine, but I have yet to solder on the connections to get telemetry! Hoping to get that done later today. 

Some notes that may help other builders:
- I used the default code that was located in the original github and it works very well with the new VESC tool.
- I initially could not get the hall sensor to detect the magnets that I had ordered, so rather than order stronger magnets, I put a glob of hot glue under the hall sensor, elevating it closer to the wheel! Hasnt failed yet :smiley: 
- I completed the remote and the receiver and I couldnt get them to pair. It wasnt the address that was wrong, I apparently messed up the flashing process. I reflashed the receiver and it fixed my connection issues.
- Make sure you put some sort of shielding on the ceramic antennae. I tried to test the range without shielding the rest of the chip and the range was maybe 3 meters. Once I shielded it, I was able to control it from the other side of my house. 
- I was successful in using a female Usb-C Port (Like member Travo was attempting) I attached the positive connection from the charging board to the 5v pad on the Usb-C port, and after cutting off the edges and tracing the pads, The ground is simply the metal casing of the port. So ground to ground (as per usual)
- I did have to trim off the edges of the port to get it to fit and modify the hole, but it is 100% possible. If you want to do this, make sure your 5v pad is within the center of the port and it will (probably) be usable once you trim off the edges.
- I wanted to use Usb-C because I currently use a Samsung phone that utilizes the port and theoretically, you should be able to use a lighting jack (if you can source one with breakout pads) with no issue just like USB-C. I have also been using my Samsung fast charger brick to charge the device and I have had no major issues other than the remote getting warm after charging.
- I used the board schematic provided by @ervinelin and his modified trigger version. It made the reciever so much simpler to build since not many people provided an "easy" way to set it up without having the need to reset it every time it gets restarted. The board was custom ordered from JLCPCB and came in at an amazing 5 business days.

Enough of the tips, here is my remote!

I realize now after uploading all the images that new users are limited to one image per post, so heres a link to an imgur gallery (Click the image) :

https://imgur.com/a/SBlZ2Tk

Anyway, I loved building the remote and it was a fun little weekend project! If anyone has any questions on how to make the remote or need clarification on any of my points I made above, feel free to ask!
```

---
## \#1511 Posted by: rey8801 Posted at: 2018-08-17T05:07:53.611Z Reads: 222

```
Nice man. By the size of the receiver I see you didn't use any big capacitor on between the 5v and gnd coming from the VESC.
What did you use to shield the antenna? I am using another antenna that gives me more range than the ceramic one, but it worth a try if I can further extend the range. Did you should both the NRF modules? Thx
```

---
## \#1512 Posted by: 12382 Posted at: 2018-08-17T05:20:32.194Z Reads: 215

```
I actually have a 220uf capacitor on the other side of the board as per @ervinelin 's design! To shield my antenna I did one layer of Electrical tape, then one layer of aluminum tape. I shielded both of my modules and it works pretty well! I have yet to try it in practical environments, so im not sure if there will be any additional interference in the city, but in my suburb it works great
```

---
## \#1513 Posted by: rey8801 Posted at: 2018-08-17T05:24:55.355Z Reads: 216

```
Good! I also have the 220uf capacitor. If you go further in the thread they also suggest it replace the cap with a 100uf to prevent from brownout possible during hard acceleration. I also have only the 220uf for the moment and no issue, just wanted to let you know.
I will try to shield my antennas and see if it change. For the moment I didn't have problem during riding for the past months, but always open for upgrade... Thx :wink:
```

---
## \#1514 Posted by: ervinelin Posted at: 2018-08-17T05:31:22.809Z Reads: 213

```
The better modules I do without shielding. See my diy trigger remote thread towards the end there are links to these better modules...
```

---
## \#1515 Posted by: rey8801 Posted at: 2018-08-17T05:57:36.533Z Reads: 215

```
Then I guess is the one I am using it since my receiver is the one posted at the end of your thread and we discuss about which antenna to use in the previous posts. Although I remember that you use also an external antenna while I opted for the same antenna board but without external antenna.
```

---
## \#1516 Posted by: ervinelin Posted at: 2018-08-17T06:15:24.907Z Reads: 207

```
I use external antenna for my transmitter.

Although I have one board which uses external antenna on the receiver as well... I get about 20m range
```

---
## \#1517 Posted by: rey8801 Posted at: 2018-08-17T06:18:36.604Z Reads: 206

```
Good to know thanks!
```

---
## \#1518 Posted by: mishrasubhransu Posted at: 2018-08-17T06:47:27.534Z Reads: 199

```
what do you mean by shielding the antenna?
```

---
## \#1519 Posted by: 12382 Posted at: 2018-08-17T14:45:45.886Z Reads: 205

```
By shielding the antenna, I wrapped the rest of the board (not blocking the ceramic antenna) with a metal tape, in my case aluminium. Make sure you wrap the board in a non conductive material first (like electrical tape) as to not short any connections
```

---
## \#1520 Posted by: clistpdx Posted at: 2018-08-17T15:58:33.033Z Reads: 220

```
Do you have any tips on how to solder the NRF to the through-hole connections on @ervinelin or @Zyb's custom PCBs? I got some 1.27mm header pin strips and soldered them through the board, but when I solder the pins to the NRF it tends to loosen the earlier solder that holds the pins secure. The NRF complicates the job further because it doesn't have actual holes at the attachment pads, but rather just half-moon crescent shaped divits. Is there a secret soldering trick for this type of connection?  
Here's the shielded NRF w/ external antenna that I'm using:
![49%20AM|611x500](upload://qxl7diZ5OFBzjkEnp8H1Nc9wHQ5.png)
```

---
## \#1521 Posted by: Zyb Posted at: 2018-08-17T20:39:18.701Z Reads: 225

```
Put it directly over the pcb and don’t use 1.27pins. It’s actually easier without pins. I just put a piece of kapton tape under the module for a piece of mind. Apply some paste, make sure iron is touching both pcb pad and module pad and then apply the solder. Just be careful if you apply too much it’s very easy to apply too much and bridge the connection and actually even that is easy to deal with. Here’s a picture ![image|375x500](upload://7liUvLeZUVtndN0ay3IrStHkLME.jpeg)
```

---
## \#1522 Posted by: clistpdx Posted at: 2018-08-17T21:26:14.325Z Reads: 217

```
Is this an earlier version of your PCB? The one I ordered has the NRF attachment points on the END of the board, and they are thru-holes, rather than SMD pads.
```

---
## \#1523 Posted by: Zyb Posted at: 2018-08-17T21:32:53.158Z Reads: 231

```
It’s not an smd pad. You just need to treat as if it is an smd pad 😁 cover the holes on the other side with kapton tape if needed. ![image|375x500](upload://tQhNdzcxB0IkYwd5b7W7i1UzAxw.jpg)
```

---
## \#1524 Posted by: clistpdx Posted at: 2018-08-17T21:33:59.765Z Reads: 220

```
Brilliant! Thanks
```

---
## \#1525 Posted by: Zyb Posted at: 2018-08-17T22:18:40.122Z Reads: 217

```
good luck!
```

---
## \#1526 Posted by: ervinelin Posted at: 2018-08-17T23:37:36.574Z Reads: 222

```
I solder pins to PCB first... I almost wick the solder in as opposed to apply it to the hole.

After that I place the NRF module in place and hold it there with some blutack first... Get the first one or two in then the rest will be easy.. again using a very fine tip and wicking the solder after heating the pin.

The smd style soldering sounds like a good idea too!
```

---
## \#1527 Posted by: mooose Posted at: 2018-08-18T07:10:24.793Z Reads: 221

```
Wow nice!!!! Let me know ASAP :smile:

P.S. Sorry for the delayed response, had to travel for work.
```

---
## \#1528 Posted by: 12382 Posted at: 2018-08-18T23:34:38.629Z Reads: 223

```
I cant get any of my telemetry to show up, and I followed @Dekbannok short guide posted earlier! Do you have any advice on what I might need to do to get this up and running?
```

---
## \#1529 Posted by: solidgeek Posted at: 2018-08-18T23:38:31.217Z Reads: 227

```
I just found out that one of the latests firmware releases from Vedder broke the VescUartControl library. Im not sure about the VESC 6 version, but the one for VESV 4.12 doesn't work. 

What firmware do you have installed on your VESC? If its the latest that should be the problem. I have used the entire day figuring this out, and I have rewritting the library from RollingGecko. I will be posting this and a update to the receiver soon :slight_smile:
```

---
## \#1530 Posted by: rey8801 Posted at: 2018-08-19T06:17:38.163Z Reads: 222

```
I use @Ackmaniac's firmware and it does work :wink:
```

---
## \#1531 Posted by: Flo Posted at: 2018-08-19T07:16:12.634Z Reads: 232

```
[quote="solidgeek, post:1529, topic:28543"]
he library from RollingGecko. I will be posting this and a update to the receiver soon :slight_smile:
[/quote]

will you also have a look at the vesc6 library? I couldn't get the RollingGecko library working with the newest 3.40 firmware for VESC6. If so I would be very thankful.
```

---
## \#1532 Posted by: solidgeek Posted at: 2018-08-19T10:16:49.751Z Reads: 229

```
@rey8801 thats probably because Ackmaniacs firmware is a few commits behind Vedders. 

@Flo Yeah actually I think the library I have made works with both v4.x and v6 hardware as long as you install the newest firmware (3.40).
```

---
## \#1533 Posted by: rey8801 Posted at: 2018-08-19T10:18:31.498Z Reads: 221

```
yes, I thought so. I just wanted to let you know. Also for others that might be interested.
```

---
## \#1534 Posted by: ervinelin Posted at: 2018-08-19T10:20:10.620Z Reads: 222

```
Good find... A friend was trying to figure out why he wasn't getting telemetry. Looks like this might be the reason.
```

---
## \#1535 Posted by: solidgeek Posted at: 2018-08-19T10:29:55.314Z Reads: 215

```
Yeah I was scratching my head a lot yesterday, and I figured some of you guys probably have had the same problems :-) I do not know which firmware version broke the telemetry, but it should be easy enough to roll back the updates and find a firmware that works. I will have a new update for the receiver and the new library released tonight.
```

---
## \#1536 Posted by: Flo Posted at: 2018-08-19T10:33:50.146Z Reads: 235

```
That sounds great that you will share the library with us tonight :) 
I'm a little curious if you managed to solve that problem: 
https://github.com/vedderb/bldc/issues/63
Will we have to wait for another firmware update for Vesc6 or did you get around that problem?
```

---
## \#1537 Posted by: solidgeek Posted at: 2018-08-19T10:40:19.692Z Reads: 232

```
The longer packet lenght is not an issue as long as you read the serial buffer fast enough. The old library used a delay(10) after sending the UART package to the VESC. This way some data will be lost if the buffer isn't big enough. I have made it different, such that it listens for and reads the serial data as soon as it arrives - therefor not losing any data. 

I have not tested it with my VESC 6 yet, however the newest firmware for VESC 6 is also FW3.40 right? So it should work.
```

---
## \#1538 Posted by: Flo Posted at: 2018-08-19T10:45:16.484Z Reads: 230

```
Yes FW 3.40 is the latest for VESC 6. 
Wonderful :) can't wait to get my bike running again :heart_eyes:
```

---
## \#1539 Posted by: erod998 Posted at: 2018-08-19T22:01:46.662Z Reads: 223

```
Could a "bad" or damaged Arduino cause brownouts? I do not have a reliable connection. It is constantly connecting and then disconnecting. When I fiddle with the Tx, like moving it and such it will connect....so I thought it was a bad connection. Yet all connections are soldered fine and checked.
```

---
## \#1540 Posted by: solidgeek Posted at: 2018-08-19T22:07:23.648Z Reads: 218

```
@erod998 Sounds like a power or noise related issue. Which Arduino do you use?
```

---
## \#1541 Posted by: erod998 Posted at: 2018-08-19T22:08:25.102Z Reads: 220

```
Arduino Nano. Currently Testing off USB. Previously had working but now it is not. 

If I move the NRF24l01 it will connect, but then crash and freeze.
```

---
## \#1542 Posted by: solidgeek Posted at: 2018-08-19T22:10:40.282Z Reads: 224

```
I have released the new VescUart library. It is basicly the same as RollingGecko's however cleaned up a bit and updated for the new FW3.40. The library can be found here: https://github.com/SolidGeek/VescUart

I have also updated the receiver software on the development branch to make use of the new library. It works great on a VESC 4.12 however I have not yet tested it on my VESC 6 as it powers my main board at the moment. 

Further testing is needed if anyone is up for the task :-) @Flo @ervinelin
```

---
## \#1543 Posted by: solidgeek Posted at: 2018-08-19T22:12:40.482Z Reads: 224

```
The one I recommend with a dedicated 3.3V voltage regulator? And you are sure none of your nrf24 wires aren't shorted?
```

---
## \#1544 Posted by: erod998 Posted at: 2018-08-19T22:13:34.466Z Reads: 236

```
![image|374x500](upload://dVFq7j8ZWv98Oxp2xYBFgERq1G6.jpg)

I checked them all multiple times, and tried many different NRF's.
```

---
## \#1545 Posted by: solidgeek Posted at: 2018-08-19T22:15:19.194Z Reads: 226

```
You need at least a 47uF capacitor on your 3.3V rail, on both receiver and remote. Otherwise the power is not sufficient.
```

---
## \#1546 Posted by: erod998 Posted at: 2018-08-19T22:23:14.698Z Reads: 237

```
[quote="solidgeek, post:1545, topic:28543"]

[/quote]

Strange, it worked before. I will solder it on now. Also if any one wants a modified STLs for these cheaper, and probably lower quality lol NRF's, let me know. I don't have all the stuff in the Rx or have it cleaned but whatever.

![IMG_2087|374x500](upload://vQGTEA5Q1HSDrcMSWfmK8BnG3Tk.JPG)
```

---
## \#1547 Posted by: ervinelin Posted at: 2018-08-19T23:37:32.732Z Reads: 226

```
Is this backward compatible?
```

---
## \#1550 Posted by: Pimousse Posted at: 2018-08-20T07:17:20.921Z Reads: 218

```
Thanks for sharing ! :slight_smile:
```

---
## \#1551 Posted by: Wentworth Posted at: 2018-08-20T07:55:43.493Z Reads: 215

```
Indeed, I tried again, FW3.38 can be used, FW3.40 can not be used.  I used the previous library.
```

---
## \#1552 Posted by: Pimousse Posted at: 2018-08-20T08:44:02.609Z Reads: 221

```
What library are you using with ?
```

---
## \#1554 Posted by: erod998 Posted at: 2018-08-20T18:52:33.976Z Reads: 226

```
I am getting 5v when powered from the remote not USB to the 3v3 pins…what could cause this? A blown part in the arduino? I think it is. When powered off USB, the Tx gets .68 volts. When powered from the Tx remote/boost converter, it has 4.10 volts. I am gonna replace the arduino.

EDIT: I powered the NRF off a NodeMCU....which has a 3v3 output. Boom. Instant stable connection. Something is wrong mechanically or electronically with the arduino, by differing different points of pressure on the board can change the voltage output...whatever. Sorry for blowing up this thread lol. It's fixed. Nice job to solidgeek for correctly diagnosing the power issue, thanks.
```

---
## \#1555 Posted by: Jc06505n Posted at: 2018-08-22T18:19:07.096Z Reads: 218

```
Has anyone tried letting 2 Fireflies connect to a a single receiver? So like one board can be used with any firefly with a specific address?
```

---
## \#1557 Posted by: Marksmoura Posted at: 2018-08-30T01:05:17.745Z Reads: 191

```
Why using arduino 5V plus a step up converter instead of using an arduino 3.3V and connect everything directly on the remote?
```

---
## \#1558 Posted by: Wraith Posted at: 2018-08-30T01:06:48.788Z Reads: 192

```
I asked @solidgeek and that isn't going to work out of the box. Should be possible with some upgrading or tweaking as He's told me.
```

---
## \#1559 Posted by: clistpdx Posted at: 2018-08-30T03:05:16.488Z Reads: 185

```
I know the hall sensor needs 5V to operate, and I think the arduino needs it too, so the battery voltage needs to be boosted at the beginning.
```

---
## \#1560 Posted by: solodros Posted at: 2018-08-30T06:49:14.312Z Reads: 191

```
I tried to use the SS39ET Hall sensor and the 8MHZ crystal to successfully make the remote control work in 3.3v.
```

---
## \#1561 Posted by: solidgeek Posted at: 2018-08-30T10:03:44.646Z Reads: 201

```
The only reason why I choose 5V instead of 3.3V back when I made the remote, was that the Hall sensor (SS495) didn't work with 3.3V. You can definitly make it run on 3.3V, you just need to find a appropiate hall sensor :-)
```

---
## \#1562 Posted by: Deakbannok Posted at: 2018-08-30T16:35:52.353Z Reads: 195

```
Is the new firmware for the VESC 6.xx that you were having problem with? or VESC 4.xx.
I use VESC 4.xx and have no issue with a new firmware. (I use Ackmaniac firmware)
```

---
## \#1563 Posted by: solidgeek Posted at: 2018-08-30T16:58:41.199Z Reads: 195

```
The new receiver software (and the new library) works for any VESC as long as it is updated to the newest firmware (FW3.40). The newest firmware for VESC 6 and 4.xx broke the old UART library.
```

---
## \#1564 Posted by: chinzw Posted at: 2018-08-30T21:08:47.231Z Reads: 197

```
There's plenty halls sensors which work with 3.3v or lower, and there's 3.3v arduinos.
```

---
## \#1565 Posted by: clistpdx Posted at: 2018-08-30T21:48:55.269Z Reads: 198

```
Right, I just mean that the original design called for it because some of the components required it. There's lot of ways to build this thing. I've got one where the boost converted and USB charger are all in one, to keep it a bit simpler.
```

---
## \#1566 Posted by: Wentworth Posted at: 2018-08-31T09:26:51.688Z Reads: 194

```
I found that after changing the new serial protocol, the throttle response slowed down. My V4's FW is 3.40. The library is up to date. Only I have this problem? My previous library didn't have this problem. Can anyone help me solve this problem?
```

---
## \#1567 Posted by: solidgeek Posted at: 2018-08-31T09:32:33.896Z Reads: 192

```
I will have a look into this, however I haven't experienced it. Maybe the updated UART protocal uses a sligthly longer time to process the data. I will make some measurements :-)
```

---
## \#1568 Posted by: Wentworth Posted at: 2018-08-31T09:55:07.537Z Reads: 191

```
I don't know if it is my own problem. Because I modified the code, I added a lot of features. I also deleted the cruise code of the receiver. I have no problem using the previous library in FW3.38.
```

---
## \#1569 Posted by: mishrasubhransu Posted at: 2018-08-31T10:01:02.194Z Reads: 193

```
why 8Mhz crystal?
```

---
## \#1570 Posted by: solidgeek Posted at: 2018-08-31T10:15:01.581Z Reads: 202

```
You can't reliably run an Atmega328p supplied by 3.3V at 16Mhz. You would basically be overclocking the microcontroller.
```

---
## \#1571 Posted by: StefanMe Posted at: 2018-08-31T11:56:02.448Z Reads: 211

```
Is it possible to get the STEP files from the inner plate where the arduinio is mounted? I want to modify it for my purposes... I know, I just could redraw it, but get the original file would make it much easier. 
Its only because i bought a different sent/reciver https://www.ebay.de/itm/5x-NRF24L01-2-4-GHz-Funkmodul-Transceiver-Sender-Empfänger-Arduino-Raspberry-Pi/162887194799?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649

Thanks! Awesome build. I will build one and will definitely do a donation!
```

---
## \#1572 Posted by: solidgeek Posted at: 2018-08-31T12:03:12.995Z Reads: 212

```
Glad you like the remote, and yes of course. Don't know why I haven't uploaded them someplace yet. I will drop you a PM with a link to the file :-)
```

---
## \#1573 Posted by: StefanMe Posted at: 2018-08-31T13:05:26.328Z Reads: 211

```
Thanks! It helped a lot!
```

---
## \#1574 Posted by: Pedrodemio Posted at: 2018-08-31T22:22:03.764Z Reads: 219

```
Hey @solidgeek could you PM the STEP files for me to please? I need to add a few holes for buttons

Just waiting to all the parts to arrive to assemble it

Thanks
```

---
## \#1575 Posted by: StefanMe Posted at: 2018-09-01T00:23:34.903Z Reads: 224

```
Is there any reason why u use the 5V (Out/Input) to power the Arduino instead of the VIN?

https://github.com/MrSolidGeek/nRF24-Esk8-Remote/raw/master/images/electronics_schematic_part2.png
```

---
## \#1576 Posted by: SeeTheBridges Posted at: 2018-09-01T01:02:18.251Z Reads: 222

```
The vin goes through a 5V regulator and needs I think ~6.5V before it starts out putting a stable 5V. Using the 5V pin bypasses the regulator
```

---
## \#1577 Posted by: atlas Posted at: 2018-09-02T00:18:28.431Z Reads: 226

```
Hello, so ive been watching this project for quite some time.  I just received all the necessary parts to build the remote.  everything is hooked up and ready to go, however im stuck on the software part.  I went to solidgeeks webpage and downloaded all the latest firmware as well as the libraries, thats the U8g2 library and the vesc uart new version.  I also have the latest transmitter and reciever software.  When try to verify it says:
Arduino: 1.8.6 (Windows 10), Board: "Arduino Nano, ATmega328P"

Invalid library found in C:\Users\theli\Documents\Arduino\libraries\transmitter_code: C:\Users\theli\Documents\Arduino\libraries\transmitter_code
Multiple libraries were found for "buffer.h"
transmitter:15:18: error: RF24.h: No such file or directory

 Used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-new
compilation terminated.

 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
 Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
exit status 1
RF24.h: No such file or directory

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.

It also says that when i try to upload it.  a couple of things to note, is when i try to get the board info it says:  
BN - unknown board
VID - 1A86
PID - 7523
SN - upload any sketch to obtain it

Also when i try to do the wifi101 firmware certificate/updator test connection it says: 
programmer not responding.!!!

Please help

And thank you in advance
```

---
## \#1578 Posted by: Jc06505n Posted at: 2018-09-02T00:47:35.167Z Reads: 206

```
Just do everyone knows... discourse has code blocks 

```ruby 
def hello
   puts "world"
end
```
To do so have 3 of these (`) followed immediately by your programming language of choice so python 
Then whatever code you have , and close it off with the same characters used to start it
```

---
## \#1579 Posted by: atlas Posted at: 2018-09-02T14:31:22.619Z Reads: 201

```
hello, thank you for the reply.  So im not exactly sure what you mean by that.  I put the three apostrophes in a row where it was giving me the RF24.h error but it said empty character content.  I also put it in the beginning of the entire code and at the end but still did nothing.  theirs also multiple errors?
```

---
## \#1580 Posted by: Jc06505n Posted at: 2018-09-02T14:40:41.384Z Reads: 215

```
``` 
Arduino: 1.8.6 (Windows 10), Board: “Arduino Nano, ATmega328P”

Invalid library found in C:\Users\theli\Documents\Arduino\libraries\transmitter_code: C:\Users\theli\Documents\Arduino\libraries\transmitter_code
Multiple libraries were found for “buffer.h”
transmitter:15:18: error: RF24.h: No such file or directory

Used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-new
compilation terminated.

Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-master
Not used: C:\Users\theli\Documents\Arduino\libraries\VescUartControl-0.1.5
exit status 1
RF24.h: No such file or directory

This report would have more information with
“Show verbose output during compilation”
option enabled in File -> Preferences.
```

``` BN - unknown board
VID - 1A86
PID - 7523
SN - upload any sketch to obtain it
```
```

---
## \#1581 Posted by: atlas Posted at: 2018-09-02T14:46:01.768Z Reads: 200

```
I'm not sure what im suppose to take from this, its just a copy of the error message
```

---
## \#1582 Posted by: Jc06505n Posted at: 2018-09-02T14:47:54.669Z Reads: 201

```
It’s to make it presentable so anyone who wish to help you can read it better
```

---
## \#1583 Posted by: atlas Posted at: 2018-09-02T14:50:36.756Z Reads: 198

```
Ok, i appreciate it.
```

---
## \#1584 Posted by: StefanMe Posted at: 2018-09-02T16:58:49.406Z Reads: 204

```
@solidgeek how did u calculate the pre resistor for the LEDs? 1kOhm looks much to high. 

If I calculate for a blue led:
5V digital output
3V LED through voltage
18mA current
= 111 Ohm ~ 120 Ohm

Did I miscalculate or misunderstood something?
```

---
## \#1585 Posted by: clistpdx Posted at: 2018-09-02T20:15:22.985Z Reads: 204

```
[quote="Jc06505n, post:1580, topic:28543"]
Multiple libraries were found for “buffer.h”
[/quote]

I think this error might be in part because you've installed multiple VescUart libraries. Each one contains a buffer.h but they conflict with eachother if you have more than one. Looks like you might have 'New', 'master' and one other named '0.1.5' installed. Just delete/uninstall all but the one you want.
```

---
## \#1586 Posted by: atlas Posted at: 2018-09-02T20:27:47.362Z Reads: 221

```
thank you,
I erased everything and started from scratch.  I still get this error however and it wont let me upload:  

Arduino: 1.8.6 (Windows 10), Board: "Arduino Nano, ATmega328P (Old Bootloader)"

transmitter:15:18: error: RF24.h: No such file or directory

compilation terminated.

exit status 1
RF24.h: No such file or directory

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.
```

---
## \#1587 Posted by: SeeTheBridges Posted at: 2018-09-02T20:29:44.859Z Reads: 218

```
For anyone interested in a prebuilt, I've got 1 more currently available: 
https://www.electric-skateboard.builders/t/f-s-black-firefly-remote/66781?u=seethebridges
```

---
## \#1588 Posted by: clistpdx Posted at: 2018-09-02T20:49:11.015Z Reads: 214

```
[quote="atlas, post:1586, topic:28543"]
transmitter:15:18: error: RF24.h: No such file or directory
[/quote]

Have you installed the RF24.h library? There are a few libraries you have to install other than the VESCUART one.
```

---
## \#1589 Posted by: Ashton_P Posted at: 2018-09-02T21:21:25.443Z Reads: 204

```
Hey are you still selling these things? If so, can you make different colors?
```

---
## \#1590 Posted by: SeeTheBridges Posted at: 2018-09-02T21:39:50.856Z Reads: 208

```
I'm not currently producing different colors right now
```

---
## \#1591 Posted by: atlas Posted at: 2018-09-03T01:46:11.105Z Reads: 227

```
Thank you, I did that and it work.  Transmitter is all good. So now the reciever code is giving me this error:

Arduino: 1.8.6 (Windows 10), Board: "Arduino Nano, ATmega328P (Old Bootloader)"

Reciever:127:2: error: 'VescUart' does not name a type

  VescUart UART;

  ^

C:\Users\theli\Documents\Arduino\libraries\Reciever\Reciever.ino: In function 'void setup()':

Reciever:139:7: error: 'UART' was not declared in this scope

       UART.setSerialPort(&Serial);

       ^

C:\Users\theli\Documents\Arduino\libraries\Reciever\Reciever.ino: In function 'void setCruise(bool, uint16_t)':

Reciever:453:5: error: 'UART' was not declared in this scope

     UART.nunchuck.lowerButton = cruise;

     ^

C:\Users\theli\Documents\Arduino\libraries\Reciever\Reciever.ino: In function 'void setThrottle(uint16_t)':

Reciever:488:5: error: 'UART' was not declared in this scope

     UART.nunchuck.valueY = map(throttle, 0, 1023, 0, 255);

     ^

C:\Users\theli\Documents\Arduino\libraries\Reciever\Reciever.ino: In function 'void getUartData()':

Reciever:537:10: error: 'UART' was not declared in this scope

     if ( UART.getVescValues() )

          ^

exit status 1
'VescUart' does not name a type

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.
```

---
## \#1592 Posted by: Nordle Posted at: 2018-09-03T06:49:01.240Z Reads: 208

```
Hey, i have some questions about this remote:

* is it possible to use the switch for reverse mode? (would like to keep ppm with brakes but have possibility for reverse mode)
* is it possible to use said button for cruise control?
* do i have to connect uart pins on my master vesc, or is slave also ok? because i would like to have bluetooth module on master

thanks
```

---
## \#1593 Posted by: dspx Posted at: 2018-09-03T12:17:47.130Z Reads: 203

```
Having the same issue, what are we doing wrong?
```

---
## \#1594 Posted by: atlas Posted at: 2018-09-03T13:55:26.687Z Reads: 216

```
Hello, so my first issue was that I didn't install the rf24.h library.  Now the second issue is for my reciever and it says the vescuart does not name a type. I'm not sure what that's suppose to mean, I'm a noob at coding.
Any help is appreciated. I've read that if you basically downgrade to an older version of the arduino ide, some things will upload then on the newer version. It's because when the code is made in the older version, its specific to that version.  Some things may be ok in the newer version because they havnt change, however, some other things may have. I just hope I can find a fix other then trying that.
```

---
## \#1595 Posted by: dspx Posted at: 2018-09-03T14:16:46.824Z Reads: 213

```
Ah, I guess I'll give that a try. Also having an issue getting the trigger to limit acceleration/braking in the OLED display, which is confusing because the trigger function works when booting into the settings, so I imagine my soldering connections are sound.
```

---
## \#1596 Posted by: atlas Posted at: 2018-09-03T14:18:31.443Z Reads: 216

```
It makes it super easy when you make a custom PCB. Try easyeda, itll clean up a lot of the wire clutter.
```

---
## \#1597 Posted by: atlas Posted at: 2018-09-03T22:04:08.341Z Reads: 218

```
Just seeing if anybody has found a fix for the "VescUart does not name a type" error in the receiver code.  By the way i tried an earlier version of arduino and it didn't work.
```

---
## \#1598 Posted by: mishrasubhransu Posted at: 2018-09-03T22:12:56.761Z Reads: 231

```
I got 2 of these units https://www.adafruit.com/product/3176 at $24 each
It has lipo charger, radio built in. It also operates at around 900mhz which makes the range longer(longer wavelength lower energy dissipation) also less interference from 2.4Ghz wifi networks.

Porting the code doesn't seem difficult. Let's see. 
![image|666x500](upload://7t0Ne1Muu9MNOQOx0VPUV6NIIzf.jpg)
```

---
## \#1599 Posted by: dspx Posted at: 2018-09-03T22:52:35.300Z Reads: 229

```
Did you try the VescUart fix from solidgeek?
https://github.com/SolidGeek/VescUart
I was about to try it, but I think my receiver is showing its Chinese clone colors.. doesn't allow any uploads now.. errors out with:

  `avrdude stk500_recv() programmer is not responding arduino nano`

Case of the Mondays
```

---
## \#1600 Posted by: neiru37 Posted at: 2018-09-04T01:47:17.256Z Reads: 219

```
Hi guys,

Anyone have this issue? Sometimes when I ride, the motors would register a reverse signal spike. You can see from the my video that even though I'm not engaging my remote the board would reverse by itself for literally a split second.

https://drive.google.com/file/d/1Egwbgk_t3qJdiuje9l9CiDpHQGu7bc76/preview

Sadly this has happened way too often and even one time during high speed so I opted to switch out for the time being. If I didn't have straps I would have been flown off of the board.
```

---
## \#1601 Posted by: clistpdx Posted at: 2018-09-04T04:26:16.442Z Reads: 213

```
[quote="dspx, post:1599, topic:28543"]
avrdude stk500_recv() programmer is not responding arduino nano
[/quote]

I think I got that error and had to choose 'old bootloader' when selecting your processor inside the IDE
```

---
## \#1602 Posted by: Nordle Posted at: 2018-09-04T04:47:24.722Z Reads: 205

```
please report back how this feather works. could make smallest remote ever with that all in one:)
```

---
## \#1603 Posted by: solidgeek Posted at: 2018-09-04T09:15:54.642Z Reads: 215

```
@atlas You have to use the VescUart library I released on Github, if you want to use the latest development branch.

Github.com/Solidgeek/VescUart

@neiru37 How did you configure your VESC? What firmware do you use? Which version of the receiver software do you have? Have you configured the PPM options in the Vesc? We cant help you if you dont supply any information.
```

---
## \#1604 Posted by: neiru37 Posted at: 2018-09-04T09:21:34.138Z Reads: 208

```
[quote="solidgeek, post:1603, topic:28543"]
How did you configure your VESC? What firmware do you use? Which version of the receiver software do you have? Have you configured the PPM options in the Vesc? We cant help you if you dont supply any information.
[/quote]

Woops, sorry wasn't sure what to include as supplementary information.

I'm using ackmaniac on my vesc and have calibrated ppm on the vesc tool. 

I'm not sure how I should answer your question on how I set up my vesc. 

I used the development version of your receiver firmware before the recent changes you pushed.

Here's a direct link to the video in case the preview doesn't load: [https://drive.google.com/file/d/1Egwbgk_t3qJdiuje9l9CiDpHQGu7bc76/preview](https://drive.google.com/file/d/1Egwbgk_t3qJdiuje9l9CiDpHQGu7bc76/preview)
```

---
## \#1605 Posted by: StefanMe Posted at: 2018-09-04T16:35:38.349Z Reads: 201

```
Omg this is awesome... 😍

Are u working on this?
```

---
## \#1606 Posted by: Pedrodemio Posted at: 2018-09-04T16:50:23.140Z Reads: 210

```
Any particular reason you left out the Wh reading from the vesc?

    case COMM_GET_VALUES: // Structure defined here: https://github.com/vedderb/bldc/blob/43c3bbaf91f5052a35b75c2ff17b5fe99fad94d1/commands.c#L164

			ind = 4; // Skip the first 4 bytes 
			data.avgMotorCurrent 	= buffer_get_float32(message, 100.0, &ind);
			data.avgInputCurrent 	= buffer_get_float32(message, 100.0, &ind);
			ind += 8; // Skip the next 8 bytes
			data.dutyCycleNow 		= buffer_get_float16(message, 1000.0, &ind);
			data.rpm 				= buffer_get_int32(message, &ind);
			data.inpVoltage 		= buffer_get_float16(message, 10.0, &ind);
			data.ampHours 			= buffer_get_float32(message, 10000.0, &ind);
			data.ampHoursCharged 	= buffer_get_float32(message, 10000.0, &ind);
			ind += 8; // Skip the next 8 bytes 
			data.tachometer 		= buffer_get_int32(message, &ind);
			data.tachometerAbs 		= buffer_get_int32(message, &ind);
			return true;
```

---
## \#1607 Posted by: solidgeek Posted at: 2018-09-04T17:26:16.502Z Reads: 202

```
@neiru37 Did you configure your VESC to current with brake or reverse? I cant be sure but I dont see any flucturations on the throttle (on the display). So the problem must be on the receiver side. I think you should redo the PPM settings (VESC tool) and add some more  deadband. Did you add a capasitor to your receivers 5V supply?

@Pedrodemio Well because I dont use it. If you need it I can add it no problem 😊
```

---
## \#1608 Posted by: neiru37 Posted at: 2018-09-04T17:44:59.109Z Reads: 216

```
[quote="solidgeek, post:1607, topic:28543"]
Did you configure your VESC to current with brake or reverse?
[/quote]

Yup, it's current with reverse, but with ackmaniac's special only-reverse-after-fully-braking mode.

[quote="solidgeek, post:1607, topic:28543"]
I cant be sure but I dont see any flucturations on the throttle (on the display). So the problem must be on the receiver side.
[/quote]

Yeah it's definitely on the receiver side. Could it be interference?

[quote="solidgeek, post:1607, topic:28543"]
I think you should redo the PPM settings (VESC tool) and add some more deadband.
[/quote]

The thing though is that it still does this while I'm engaging throttle. While my video showcases the brake throttle spike during idle, it has happened while I was accelerating. If I were to describe it, it feels as if I accidentally pulled back the throttle then back up again.

[quote="solidgeek, post:1607, topic:28543"]
Did you add a capasitor to your receivers 5V supply?
[/quote]

Would it matter if the spikes were happening on idle? If I remember correctly the reason for adding a cap was to compensate for voltage sag/drop that happens on the vesc 5v when accelerating hard. But if it happens on idle it seems like it's not a power issue.

Another thing to note: It only happens when the receiver is connected to the transmitter. When I turn off the transmitter the board stops engaging the brakes/reversing. The moment I turn it back on again and it connects to the receiver it does it again. This seems like it's less of a power/wiring issue and more of an interference/signal issue.
```

---
## \#1609 Posted by: Pedrodemio Posted at: 2018-09-04T19:02:48.800Z Reads: 191

```
Thanks, Will add for sure, just checking if it has anything to do with the buffer limit of the Arduino with the firmware 3.40

Just by curiosity, how did you deal with it without changing the compiler settings?
```

---
## \#1610 Posted by: mishrasubhransu Posted at: 2018-09-04T19:46:21.319Z Reads: 191

```
Yeah. When I get the boards.
```

---
## \#1611 Posted by: Nordle Posted at: 2018-09-04T21:00:52.731Z Reads: 195

```

it is so easily overlooked in this topic, but maybe some1 can answer my questions?^^ i printed the shell and would be ready to order parts:)
[quote="Nordle, post:1592, topic:28543"]
* is it possible to use the switch for reverse mode? (would like to keep ppm with brakes but have possibility for reverse mode)
* is it possible to use said button for cruise control?
* do i have to connect uart pins on my master vesc, or is slave also ok? because i would like to have bluetooth module on master

thanks
[/quote]
```

---
## \#1612 Posted by: clistpdx Posted at: 2018-09-04T21:42:43.369Z Reads: 190

```
Can anyone suggest how I might configure the firefly settings so that I get accurate readings using hub motors. Obviously the current settings ask for pulley teeth, wheel diameter, etc. Not all of this is applicable to hub motors. I'd love to use the firefly with Hummie's Hubs but I wonder if someone has already figured out the math on this?
```

---
## \#1613 Posted by: Nordle Posted at: 2018-09-04T21:49:32.519Z Reads: 192

```
gearing in a hub motor is 1:1 just take the same theeth amount for both, motor and wheel pulley, and set your wheel size to your wheel size.
```

---
## \#1614 Posted by: Jc06505n Posted at: 2018-09-04T22:06:36.017Z Reads: 218

```
[quote="Nordle, post:1611, topic:28543"]
is it possible to use the switch for reverse mode? (would like to keep ppm with brakes but have possibility for reverse mode)
[/quote]

I think you would have to do some rewriting maybe. It looks like the switch’s only responsibility is to act as a power switch and nothing more. You would need something like @Zyb’s remote that has a extra programmable button. Same said for cruise control, though CC is a setting in the developer’s branch of the code.
```

---
## \#1615 Posted by: Nordle Posted at: 2018-09-05T06:15:46.131Z Reads: 228

```
@Jc06505n  there are two switches actually? ![img_20180314_181103750-2-1024x576|690x388](upload://Ag1tA2PcFp3HbqW4nAFx8QJLDlv.jpg)

@solidgeek, can you take a look at my questions:
[^scroll up^](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/1592)
```

---
## \#1616 Posted by: solidgeek Posted at: 2018-09-05T09:12:00.847Z Reads: 230

```
@Nordle Yes you can use the trigger as reverse mode, however you would have to make a few software changes. There are two ways I can see this implemented, both require the UART connection.

1. The Nunchuck mod from Vedder, used the top button to switch direction and the lower to cruise. I use this to enable cruise control with the remote, however I never implemented reverse. This could be done by setting the valLowerButton to true I think. This method uses UART only.

2. Change the settings over UART. The VESC got a configuration called "Invert motor direction" if this could be changed by a UART package the motor direction could be changed on the fly. However has to be tested.

I am planning to add this in the future, however I am currently spending my time on a related project :-)
```

---
## \#1617 Posted by: StefanMe Posted at: 2018-09-05T09:17:53.912Z Reads: 215

```
What project? 😏 *Spoiler*
```

---
## \#1618 Posted by: Deakbannok Posted at: 2018-09-06T17:02:13.329Z Reads: 210

```
PCB *spoiled*
```

---
## \#1619 Posted by: oiitsjamesmate Posted at: 2018-09-06T19:05:09.923Z Reads: 206

```
Anyone got any Ideas on how to limit the rate the hall effect/potentiometer value can increase? Like an acceleration limiter.
```

---
## \#1620 Posted by: clistpdx Posted at: 2018-09-06T19:11:37.231Z Reads: 213

```
I don't have the code in front of me now, but I recall that in the transmitter.ino there's a section which takes the hall reading and converts them to a 1-100 scale, or something along those lines (since the hall sensor returns values roughly in the range of 200-1100). It is in this section that you could adjust the math to suit your needs, i.e. to cap how high the number can go. But maybe that would just be easier to do in the VESC Tool when you configure the remote?
```

---
## \#1621 Posted by: oiitsjamesmate Posted at: 2018-09-06T19:36:45.778Z Reads: 210

```
I don't need to limit its range, just the speed that it can increase by. So if I hold the thumb wheel down full throttle, the board will gradually accelerate.
```

---
## \#1622 Posted by: clistpdx Posted at: 2018-09-06T23:40:28.344Z Reads: 202

```
Maybe throttle curves are a simpler answer? https://www.electric-skateboard.builders/t/ackmaniacs-fw-lets-talk-throttle-curves/64173
```

---
## \#1623 Posted by: Lionpuncher Posted at: 2018-09-07T00:14:35.800Z Reads: 201

```
I would agree with you. Having played with mine a bit I can tell you with an aggressive throttle curve you can really make the acceleration gradual. Top end still gets pretty crazy tho...
```

---
## \#1624 Posted by: atlas Posted at: 2018-09-07T00:23:10.757Z Reads: 201

```
I have two questions:

1.  How can you change the logo and what it says on the opening screen?

2.  how can you change the settings from KM to MPH.  I seen you can change it in the display however does it calculate the correct value if changed?
```

---
## \#1625 Posted by: clistpdx Posted at: 2018-09-07T00:40:28.259Z Reads: 199

```
[quote="atlas, post:1624, topic:28543"]
How can you change the logo and what it says on the opening screen?
[/quote]

You have to first create your bitmap graphic, then convert it to hex so you can place it in the code. There's some free PC software that can convert for you. https://www.instructables.com/id/How-to-convert-bitmap-graphics-for-OLED-SSD1306-di/
```

---
## \#1626 Posted by: clistpdx Posted at: 2018-09-07T00:43:14.587Z Reads: 207

```
[quote="atlas, post:1624, topic:28543"]
how can you change the settings from KM to MPH. I seen you can change it in the display however does it calculate the correct value if changed?
[/quote]
I got it working by adjusting the math slightly in the code (see post #1399), then of course changing the 'KM' text to 'MPH' in the code wherever it was referenced. I think it's accurate:
https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/1399?u=clistpdx
```

---
## \#1627 Posted by: dspx Posted at: 2018-09-07T15:20:36.563Z Reads: 195

```
Anyone in the states have an extra nano v3 they wouldn't mind parting with? :pray: I'm pretty sure I've botched the receiver nano - I've gone through about every troubleshooting exercise I could find, it errors out in spite of my efforts. Ordered a few on aliexpress, but I could be dead by the time those arrive #dramatic 

I'd also be happy to trade one back once the shipment comes in. Eh? Eh?
```

---
## \#1628 Posted by: StefanMe Posted at: 2018-09-07T17:15:22.228Z Reads: 194

```
Hi Guys! I build my first remote an I am happy so far... made some modifications to it like a bigger screen, ball bearings instead of the plastic glides, extra button and a little vibration motor... At the moment I use just the basic code from the development branch, and PPM works great, BUT I cannot get any data from the VESC. Every value shows just 0.
I just wired up to RX/TX to vesc. UART worked before, because there was an HM10 connected. Baudrate is set to 115200. Do I have to do something else??
```

---
## \#1629 Posted by: SeeTheBridges Posted at: 2018-09-07T17:32:13.402Z Reads: 191

```
Did you also set your control scheme to "PPM and UART"?
```

---
## \#1630 Posted by: StefanMe Posted at: 2018-09-07T18:05:16.469Z Reads: 196

```
yes I didn't. I used an HM10 before on the same cables... worked without any issues.

Do I have to use the ground or +5V from the UART Port from the VESC? One Ground from my Ardunio is connected to - of the VESC (where normally the recover is powered) and the other ground goes to the NRF42.

Is there any chance to debug the connection? I really don't know how to solve this issue. I just get no data from the VESC.
```

---
## \#1631 Posted by: StefanMe Posted at: 2018-09-07T21:36:45.735Z Reads: 211

```
maybe this helps for debug?

    Esk8-remote receiver
    Settings loaded
    Printing receiver details
    STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0
    RX_ADDR_P0-1	 = 0xe7e7e7e7e7 0xe8e8f0f0e1
    RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6
    TX_ADDR		 = 0xe7e7e7e7e7
    RX_PW_P0-6	 = 0x00 0x20 0x00 0x00 0x00 0x00
    EN_AA		 = 0x3f
    EN_RXADDR	 = 0x02
    RF_CH		 = 0x6c
    RF_SETUP	 = 0x07
    CONFIG		 = 0x0f
    DYNPD/FEATURE	 = 0x3f 0x06
    Data Rate	 = 1MBPS
    Model		 = nRF24L01+
    CRC Length	 = 16 bits
    PA Power	 = PA_MAX
    Setup complete - begin listening
    New package: '0-527-0'
    Getting VESC data
    New package: '0-546-0'
    Getting VESC data
    New package: '0-527-0'
    Getting VESC data
    New package: '0-537-0'
    Getting VESC data
    New package: '0-563-0'
```

---
## \#1632 Posted by: solidgeek Posted at: 2018-09-07T22:53:40.151Z Reads: 204

```
It could be a simple compability issue you are facing. What firmware version are you running at the VESC? And which software version for the receiver? :-)
```

---
## \#1633 Posted by: StefanMe Posted at: 2018-09-07T23:00:20.863Z Reads: 198

```
I run 3.40 on my vesc (hw.4.10).  On the receiver Iam running `#define VERSION 2.0` from the development branch. Not good? :slight_smile:
```

---
## \#1634 Posted by: solidgeek Posted at: 2018-09-07T23:02:15.336Z Reads: 200

```
Are you using the latest commit from the development branch, and downloaded the library I released for UART communication "VescUart"?
```

---
## \#1635 Posted by: StefanMe Posted at: 2018-09-07T23:08:53.478Z Reads: 197

```
I downloaded this one [GITHUB](https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/a70a9fb09ecb110ddd1fdb40eb173e6ce42d27d9) and use this library [VescUart](https://github.com/SolidGeek/VescUart)...

Battery always show 0 on my remote. Can I check the connection in any other way?
```

---
## \#1636 Posted by: solidgeek Posted at: 2018-09-07T23:16:51.282Z Reads: 203

```
That sounds about right :-) Did you check that you connected TX and RX correctly? You should not need an extra GND wire, as long as you got GND through the PPM cable. 

If you got an Arduino Pro Mini laying around, you can use that for debugging as it got a hardware serial and a virtual serial port. I made an example in the library you could try out. Did you configure the correct baud rate for both VESC and receiver? Have you tried a lower baudrate?
```

---
## \#1637 Posted by: StefanMe Posted at: 2018-09-08T12:25:02.783Z Reads: 216

```
WAIT. Looks like its working now... I downloaded the latest commit from the branch! Looks better now! Maybe I made a mistake by downloading just the master developer branch instead of the latest commit? Thanks for your help. Everything works now as  expected. Thx a lot!

Just my signal from the hall sensor is a little bit jittering...  but I didn't have any capacitor inside at the moment. When I power the Arduino from the USB jack, it works perfectly. Is it more an issue from my 5v booster?
```

---
## \#1638 Posted by: solidgeek Posted at: 2018-09-08T14:42:46.411Z Reads: 214

```
Maybe try add a small capasitor (10uF or less) to the supply of the Hall sensor. Could be a power / noise issue.
```

---
## \#1639 Posted by: Eretron Posted at: 2018-09-09T11:18:03.281Z Reads: 209

```
Anyone selling this as a already assembled remote?
```

---
## \#1640 Posted by: boramiNYC Posted at: 2018-09-09T17:57:43.641Z Reads: 217

```
Did anyone have problem with telemetry using FOCBOX? And solved it? My focboxes are not sending over data through UART to the Firefly remote. SeeTheBridges isn't familiar with focbox. I tried baud rates 115200 and 9600. I'm lost what to look for. Please help. FW 4.12 and using BLDC Tool.
```

---
## \#1641 Posted by: StefanMe Posted at: 2018-09-10T18:59:18.705Z Reads: 218

```
Hace i tried the latest commit from the developer branch?

https://github.com/SolidGeek/VescUart?files=1
```

---
## \#1642 Posted by: HighMasterGogo Posted at: 2018-09-12T19:00:17.569Z Reads: 216

```
Just wanted to update where I'm at with my remote. I actually went back to my GT2B mod as I couldn't get a reliable, stable and non noisy pulsewidth in BLDC tool. Even when riding holding a throttle position, I could feel the signal going up and down slightly; quite unnerving!

However, this remote is so cool and I really wanted to use it! I spent some time updating the remote and going over all my connections. But, the thing that made ALL the difference was setting a higher sample rate for the smoothing or averaging of the hall sensor. Specifically this bit...

    // Hall sensor reading can be noisy, lets make an average reading.
    uint16_t total = 0;
    uint8_t samples = 20;

I changed uint8_t samples = 20; to uint8_t samples = 50; (after some experimenting with different values.

Also, be careful as the signal was stable when connected to PC USB power but not when powered from battery. I updated the value and disconnect the USB before testing.

This obviously means that the reason my hall sensor is noisy is down to a power issue. Maybe a capacitor would help?

Anyway, so happy I can use this remote for some riding! Cheers!
```

---
## \#1643 Posted by: StefanMe Posted at: 2018-09-13T01:06:13.322Z Reads: 189

```
I have exactly the same issue.. I already replaced my stepUp converter, but that doesn't help. Thx for the hint with the SAMPLE. Have u any capacitor inside your build?
```

---
## \#1644 Posted by: Wraith Posted at: 2018-09-13T01:18:17.082Z Reads: 197

```
There are a few others @BigBrit is going to be selling some from what I can recall from memory. There was another guy on the forum but can’t recall atm
```

---
## \#1645 Posted by: HighMasterGogo Posted at: 2018-09-13T07:39:37.140Z Reads: 207

```
To be fair, I’m starting to think the sample helps but didn’t solve the problem fully. 

I did a bit further investigation and a 10uf capacitor between ground and the signal pin of the hall sensor gives me a solid read out on the remote and an almost solid read out on pulsewidth on bldc tool. The percentage is steady which I believe is what the vesc uses for throttle so it should be fine. I’m going to put this together tonight and give it a go. 

So maybe try a capacitor instead?
```

---
## \#1646 Posted by: Nordle Posted at: 2018-09-13T08:03:36.638Z Reads: 202

```
do you use genuine hall sensor?
```

---
## \#1647 Posted by: HighMasterGogo Posted at: 2018-09-13T08:25:56.423Z Reads: 201

```
I have no idea. I used [this one.](https://www.ebay.co.uk/itm/HONEYWELL-S-C-SS495A-SENSOR-RATIOMETRIC-LINEAR/351163597255?epid=24012045852&hash=item51c2fb41c7:g:9bwAAOxyd8NSa73G)
```

---
## \#1648 Posted by: BigBrit Posted at: 2018-09-13T10:54:11.500Z Reads: 201

```
Still waiting for parts on the slow boat at the moment but will be selling some soon!
```

---
## \#1649 Posted by: HighMasterGogo Posted at: 2018-09-13T22:30:11.801Z Reads: 205

```
Hi guys, got an issue with vesc data that doesn't make any sense!

I've used a bluetooth module before and the data is perfect.

I'm getting nothing on battery voltage, 1539 on distance and speed bounces around 0 then 122 then 244 even when everything is stationary bench testing.

Any ideas!?
```

---
## \#1650 Posted by: HighMasterGogo Posted at: 2018-09-13T22:44:23.090Z Reads: 203

```
I'm using a Focbox and the data is showing (other than battery level) but it's making no sense to me. One thing I noticed is that you must turn debug off on the receiver else the TX/RX is used for serial monitor.
```

---
## \#1651 Posted by: HighMasterGogo Posted at: 2018-09-13T22:50:05.312Z Reads: 205

```
to add to this... if I spin the motor up the battery level shows 100% instantly and stays there until the motor stops and the reading returns to 0.
```

---
## \#1652 Posted by: StefanMe Posted at: 2018-09-14T18:25:54.014Z Reads: 203

```
Has anyone tried to use HM-10 UART Bluetooth modul together with the receiver? Is this possible?
```

---
## \#1653 Posted by: mishrasubhransu Posted at: 2018-09-16T14:44:55.729Z Reads: 206

```
@solidgeek, @JTAG, @Ackmaniac  or anyone else?. what's the best way to get 50hz odometry and current data from the vescs as fast as possible with a nonblocking call?  What I can do now is send in a packet request and wait for it to respond~20ms . Any way to make vesc constantly spit out data?
Should I be looking at can bus? Instead?
```

---
## \#1654 Posted by: solidgeek Posted at: 2018-09-17T20:31:06.270Z Reads: 214

```
@HighMasterGogo I think your problem is caused by an compability issue. Is your VESC updated to FW3.40 and are you using the latest development commit? :slight_smile:

@StefanMe This is not possible at the moment, simple because the UART port only can handle one device connected. I am planning to explore the possiblity of using a multiplexer or an analog switch IC to make an expandable UART port on the receiver. However for now you will have to use a dual VESC setup or drop telemetry for the remote :frowning:

@mishrasubhransu Yeah that is not possible unless you could enable one of the other ports on the VESC to spit out data much faster.
```

---
## \#1655 Posted by: HighMasterGogo Posted at: 2018-09-17T22:33:07.831Z Reads: 207

```
As always, you're spot on. All fixed!
```

---
## \#1656 Posted by: lockeboss Posted at: 2018-09-22T16:58:34.215Z Reads: 205

```
the howto wiki sems to be missing the last steps ( * Software
* Final assembly)?!

is there somewhere a complete instruction to find?
```

---
## \#1657 Posted by: Migro Posted at: 2018-09-22T19:07:41.750Z Reads: 201

```
@SeeTheBridges made some youtube tutorials :slight_smile:
Same name on youtube ;)
```

---
## \#1658 Posted by: KranzeKake Posted at: 2018-09-23T21:05:42.037Z Reads: 197

```
Anyone who can build a firefly remote for me? More than happy to pay a little extra
```

---
## \#1659 Posted by: Migro Posted at: 2018-09-24T12:38:12.550Z Reads: 199

```
Again i think @SeeTheBridges stil does and @Zyb. Zyb got another topic created for his remotes [WTS: PCB based Firefly Remotes](https://www.electric-skateboard.builders/t/wts-pcb-based-firefly-remotes/66349)
```

---
## \#1660 Posted by: SeeTheBridges Posted at: 2018-09-24T19:45:32.414Z Reads: 191

```
I'm not actively accepting new orders at this time unfortunately.
```

---
## \#1661 Posted by: elman Posted at: 2018-09-27T01:12:38.924Z Reads: 190

```
@solidgeek  Hi bro, it's absolutely perfect job. Do you have receiver schema?
```

---
## \#1662 Posted by: chickengun Posted at: 2018-09-28T00:03:10.764Z Reads: 195

```
do you guys think I fried my nrf24l01 by connecting Arduino 3.3V to GND on nrf24l01 and Arduino GND to 3.3V  on nrf24l01?

Arduino 3.3 V <---> nrf24l01 GND
Arduino GND <---> nrf24l01 3.3 V

The 3.3V voltage regulator got hot on the arduino, then I noticed my mistake.
```

---
## \#1663 Posted by: StefanMe Posted at: 2018-09-28T00:47:36.132Z Reads: 196

```
More likely u fried your 3.3v regulator on the Arduino instead the nrf24
```

---
## \#1664 Posted by: StefanMe Posted at: 2018-09-28T00:48:22.946Z Reads: 192

```
It’s exactly the same as the transmitter...
```

---
## \#1665 Posted by: solidgeek Posted at: 2018-09-28T14:52:01.399Z Reads: 191

```
Yeah here you go: https://solidgeek.dk/docs/firefly-remote/remote/electrical-wiring/
```

---
## \#1666 Posted by: StefanMe Posted at: 2018-09-28T15:13:34.944Z Reads: 190

```
What’s about your PCB? I took a look on your blog and it seems like i are already finished there...
```

---
## \#1667 Posted by: chickengun Posted at: 2018-09-28T22:25:29.601Z Reads: 188

```
turned out that both, my arduino and the nrf works fine ;)
```

---
## \#1668 Posted by: AxelF Posted at: 2018-09-29T11:07:09.457Z Reads: 187

```
Just build mine, is this info still accurate? Throttle up means the bar goes from left to right, brake means bar goes from right to left? I would like throttle up to be when pulling the wheel down (towards me), currently the bar then goes from right to left.
```

---
## \#1669 Posted by: skslingo21 Posted at: 2018-09-29T11:53:09.897Z Reads: 188

```
Does anyone have a reliable build log for the firefly remote? I would love to know voltage and rough distance traveled with a remote! I have the tools to build it but resources are scattered like bitcoins. 

Thank you to everyone who has helped on the firefly project, lm looking forward to assembling one someday!
```

---
## \#1670 Posted by: Nordle Posted at: 2018-09-29T12:09:08.683Z Reads: 190

```
flip your hall sensor or magnets 180 degree
```

---
## \#1671 Posted by: AxelF Posted at: 2018-09-29T12:20:27.763Z Reads: 189

```
Yea I figured, thank you :)
```

---
## \#1672 Posted by: chickengun Posted at: 2018-09-29T20:58:13.262Z Reads: 196

```
@solidgeek do you also have the schematic of your Firefly Remote PCB on easyeda?
```

---
## \#1673 Posted by: StefanMe Posted at: 2018-09-30T14:47:34.356Z Reads: 203

```
Ph boysch! This getting awesome. Final ready with headlights implementation, vibration alarm and big display with switchable main value (small button close to the display❤️

![image|375x500](upload://f604AfYrC9cOkLsw3u59AFQseOU.jpeg)
```

---
## \#1674 Posted by: rey8801 Posted at: 2018-09-30T14:49:20.567Z Reads: 196

```
Nice I like the bigger screen and the additional features.
```

---
## \#1675 Posted by: rene Posted at: 2018-09-30T15:46:04.977Z Reads: 192

```
Great - how did you design the headlight feature on the hardware side of the headlight?
```

---
## \#1676 Posted by: StefanMe Posted at: 2018-09-30T16:39:53.721Z Reads: 193

```
I didn't implemented it yet. I don have headlights. And I guess I ll never have headlights. But maybe I ll switch on something other shit with it.

Should be easy possible with some cheap transistor -> relay combination. Maybe I ll make an PCB for this too...
```

---
## \#1677 Posted by: Pedrodemio Posted at: 2018-09-30T17:15:14.093Z Reads: 194

```
Nice, I’m adding light controls to mine

Could you share the light logo? Did you draw pixel by pixel or did the conversion to hex?

And the button just turn on or off? My plan is to have just one button handle all functions, but the control scheme is already a bit complicated
```

---
## \#1678 Posted by: StefanMe Posted at: 2018-09-30T18:10:34.863Z Reads: 194

```
yes of course... just simple like this:

      u8g2.drawDisc(x , y , 5, U8G2_DRAW_UPPER_RIGHT);
      u8g2.drawDisc(x , y , 5, U8G2_DRAW_LOWER_RIGHT);
      u8g2.drawLine(x -1 , y -3, x -1, y +3);

and this for the 'shine'

      u8g2.drawLine(x -3 , y, x -5, y);
      u8g2.drawLine(x -3 , y + 3, x -5, y + 4);
      u8g2.drawLine(x -3 , y - 3, x -5, y - 4);
```

---
## \#1679 Posted by: AxelF Posted at: 2018-09-30T18:11:13.995Z Reads: 205

```
Might have a few noob questions here for you coming up in the next couple of weeks while Im figuring this out :slight_smile:
Is the status LED on the receiver supposed to change in brightness when you trottle up/brake?  Just wanna make sure everythings allright, don't wanna have anything go nuts while riding!

EDIT: Im stupid, could just have checked the code... Seems like it's supposed to :) Sorry for the code format, not sure how to do it properly on this forum

>   if(statusCode == CONNECTED){
           analogWrite(statusLedPin, map(remPackage.throttle, 0, 1023, 0, 255)); 
     }else{
           digitalWrite(statusLedPin, statusLedState);
     }  
}

EDIT 2: While Im at it, searched a bit but cant find any recent info on how the binding process works (my experience with coding is not enough to understand from the actual code)? So I found adress generator in the remote, but can't seem to change it? Does that mean all remotes with firefly OS have the same adress and will interfere?
```

---
## \#1680 Posted by: Pedrodemio Posted at: 2018-09-30T18:43:34.708Z Reads: 190

```
Thanks, will see if I can fit in the small display
```

---
## \#1681 Posted by: clistpdx Posted at: 2018-10-01T05:15:51.006Z Reads: 210

```
I built a second remote and no matter what I try, I cannot get the transmitter to connect to the receiver. The transmitter always shows the blinking connection icon. I'm running the latest development version. In debug mode the receiver shows a timeout error:
>     ** Esk8-remote receiver **
>     Settings loaded
>     Printing receiver details
>     STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0
>     RX_ADDR_P0-1	 = 0xe7e7e7e7e7 0xe8e8f0f0e1
>     RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6
>     TX_ADDR		 = 0xe7e7e7e7e7
>     RX_PW_P0-6	 = 0x00 0x20 0x00 0x00 0x00 0x00
>     EN_AA		 = 0x3f
>     EN_RXADDR	 = 0x02
>     RF_CH		 = 0x6c
>     RF_SETUP	 = 0x07
>     CONFIG		 = 0x0f
>     DYNPD/FEATURE	 = 0x3f 0x06
>     Data Rate	 = 1MBPS
>     Model		 = nRF24L01+
>     CRC Length	 = 16 bits
>     PA Power	 = PA_MAX
>     Setup complete - begin listening
>     e8e8f0f0e1 - Timeout
>     e8e8f0f0e1 - Timeout
>     e8e8f0f0e1 - Timeout
>     e8e8f0f0e1 - Timeout

But the transmitter shows a 'failed transmission' error:
> STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0
> RX_ADDR_P0-1	 = 0xe8e8f0f0e1 0xc2c2c2c2c2
> RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6
> TX_ADDR		 = 0xe8e8f0f0e1
> RX_PW_P0-6	 = 0x20 0x00 0x00 0x00 0x00 0x00
> EN_AA		 = 0x3f
> EN_RXADDR	 = 0x03
> RF_CH		 = 0x6c
> RF_SETUP	 = 0x07
> CONFIG		 = 0x0e
> DYNPD/FEATURE	 = 0x3f 0x06
> Data Rate	 = 1MBPS
> Model		 = nRF24L01+
> CRC Length	 = 16 bits
> PA Power	 = PA_MAX
> e8e8f0f0e1: Failed transmission
> e8e8f0f0e1: Failed transmission
> e8e8f0f0e1: Failed transmission
> e8e8f0f0e1: Failed transmission

Am I missing something really obvious? What are the most obvious culprits? I haven't had this issue before. I appreciate the advice.
```

---
## \#1682 Posted by: chickengun Posted at: 2018-10-01T20:26:11.413Z Reads: 181

```
Is the receiver working when you use your first remote? If so the receiver is ok and I would check all your solder joints on the transmitter (nothing shorted?). Double check the connection is right. Also you might want to take it out of the printed shell and keep it away from the 5v booster to avoid interference.
```

---
## \#1683 Posted by: clistpdx Posted at: 2018-10-01T20:31:17.720Z Reads: 186

```
I checked all the solder points on both NRF's and nothing was shorted. But that's a good idea to swap out a different receiver and try that. How does the dev code know which receiver to pair with, since the pipe address is dynamically generated (unlike the master version where it's hard coded)?
```

---
## \#1684 Posted by: chickengun Posted at: 2018-10-01T20:38:15.774Z Reads: 187

```
[Transmitter.ino Line 168 and 169](https://github.com/SolidGeek/nRF24-Esk8-Remote/blob/development/transmitter/transmitter.ino).
If you haven't changed the defaultAddress and defaultChannel it's the same for both of your remotes
```

---
## \#1685 Posted by: clistpdx Posted at: 2018-10-02T02:57:17.447Z Reads: 191

```
I kept playing with the defaultAddress and noticed that it would never actually update on the transmitter. I then reset the EEPROM (at least I think that's what I did, on accident) on the transmitter and it basically flushed out whatever was causing the conflict and BOOM I have a connection :grinning:
```

---
## \#1686 Posted by: clistpdx Posted at: 2018-10-02T03:11:51.717Z Reads: 196

```
[quote="Deakbannok, post:1004, topic:28543"]
You need to clear out the EEPROM on both tx and rx
[/quote]

Is there an easy way to clear out the EEPROM on our tx or rx? I see it mentioned in the arduino code, but I'm not sure what's the best way to initiate the clear out
```

---
## \#1687 Posted by: erod998 Posted at: 2018-10-02T16:11:11.488Z Reads: 185

```
What size screen is that? I really like it.
```

---
## \#1688 Posted by: StefanMe Posted at: 2018-10-02T16:19:50.820Z Reads: 185

```
0.9inch something
```

---
## \#1689 Posted by: erod998 Posted at: 2018-10-02T16:35:10.926Z Reads: 187

```
Would it be possible to keep the motor and MOSFET temp in there as well?
```

---
## \#1690 Posted by: Deakbannok Posted at: 2018-10-03T01:43:09.512Z Reads: 190

```
@clistpdx You have to modify the code. Or wire a reset switch to your arduino.
  and If you dont get connetion between your tx and rx reason being that is your address is not declared or somehow is not registered.
```

---
## \#1691 Posted by: powerlego Posted at: 2018-10-03T18:26:57.948Z Reads: 195

```
@solidgeek I was wondering if you can add a setting for lights, to turn them on or off and maybe a dimming option?
```

---
## \#1692 Posted by: lockeboss Posted at: 2018-10-03T18:30:50.792Z Reads: 203

```
Hi
I'm trying to upload the code for the receiver but get this errormesssge:

Adruini.h is not included in the vesc uart library


![1538591411468695110392623898205|666x500](upload://8cMhugcIJtVeUEp0D1RM4o49swA.jpeg)
```

---
## \#1693 Posted by: clistpdx Posted at: 2018-10-03T18:35:42.426Z Reads: 186

```
you need to use solidgeek's updated VESCUart library, instead of the older rolling gecko ones. https://github.com/SolidGeek/VescUart?files=1
And you need your Vesc/s on 3.40 firmware
```

---
## \#1694 Posted by: lockeboss Posted at: 2018-10-03T18:37:29.982Z Reads: 182

```
I took the updated one. Does it need to  be connected to the vesc while programming?
```

---
## \#1695 Posted by: clistpdx Posted at: 2018-10-03T18:37:57.603Z Reads: 182

```
No it doesn't need to be connected while programming
```

---
## \#1696 Posted by: lockeboss Posted at: 2018-10-03T18:42:11.883Z Reads: 179

```
OK I downloaded the one from your link. Same error
```

---
## \#1697 Posted by: clistpdx Posted at: 2018-10-03T18:45:51.529Z Reads: 186

```
If you've added the new VescUart library, you may need to remove any older libraries that are still installed. They can interfere with eachother because they all have .h files of the same names
```

---
## \#1698 Posted by: clistpdx Posted at: 2018-10-03T18:46:46.125Z Reads: 188

```
Also, you should use the latest commit on the development version, rather than the master one.
```

---
## \#1699 Posted by: lockeboss Posted at: 2018-10-03T18:50:43.830Z Reads: 195

```
Deleted the old ones. I'll try the dev again but the arduini.h is missing in the uart library says ide
```

---
## \#1700 Posted by: rey8801 Posted at: 2018-10-03T18:55:49.527Z Reads: 186

```
I also see that the new library has to be modified before use it. @clistpdx could you elaborate a bit more about it?
```

---
## \#1701 Posted by: lockeboss Posted at: 2018-10-03T19:05:22.325Z Reads: 181

```
OK I have solved this error but now I get bldc measured values has incomplete type and cannot be defined
```

---
## \#1702 Posted by: rey8801 Posted at: 2018-10-03T19:07:51.195Z Reads: 175

```
you first need to adjust the throttle at the remote level. Did you went inside the setting?
```

---
## \#1703 Posted by: lockeboss Posted at: 2018-10-03T19:08:48.831Z Reads: 171

```
I'm programming the receiver. Does the remote has to be connected to it first?
```

---
## \#1704 Posted by: rey8801 Posted at: 2018-10-03T19:09:45.355Z Reads: 168

```
no it will connect only when both of the part are loaded with the scripts. Now do the receiver. remember to use the same address
```

---
## \#1705 Posted by: lockeboss Posted at: 2018-10-03T19:10:40.821Z Reads: 170

```
OK. But I'm stuck at the receiver with the bldc error
```

---
## \#1706 Posted by: rey8801 Posted at: 2018-10-03T19:11:29.039Z Reads: 173

```
ah ok, didn't have that error. Are you using the last develp branch?
```

---
## \#1707 Posted by: clistpdx Posted at: 2018-10-03T19:23:31.872Z Reads: 173

```
I didn't have to adjust any code. I think solidgeek's note there is trying to say that if you've branched off and are using your own code you will have to make adjustments to it accordingly. I had no issue using dev version with his new VescUart library, on 4.3 firmware. Only trouble I've encountered are weak NRF connections. Trying now to isolate all the other components with copper tape. I'm also building zyb's trigger remote which uses shielded NRFs and external whip antennas. Hoping to have better luck with that model.
```

---
## \#1708 Posted by: lockeboss Posted at: 2018-10-03T19:25:11.902Z Reads: 175

```
Yeah.

I tried every version its all the same
```

---
## \#1709 Posted by: rey8801 Posted at: 2018-10-03T19:25:40.960Z Reads: 169

```
Ah ok thanks for the clarification! Up to know I always used Ackmaniac's firmware. In that case should I keep use the old library or the new ones works also for the older firmware version? I guess not
```

---
## \#1710 Posted by: clistpdx Posted at: 2018-10-03T19:26:39.009Z Reads: 167

```
That I'm not certain about. I haven't tried ackmaniac's firmware personally.
```

---
## \#1711 Posted by: lockeboss Posted at: 2018-10-03T19:34:39.972Z Reads: 165

```
OK receiver seems to be done but nobody here knows why xD
Trying the remote now
```

---
## \#1712 Posted by: rey8801 Posted at: 2018-10-03T19:35:37.971Z Reads: 170

```
ahahaha that's normal some time!
```

---
## \#1713 Posted by: lockeboss Posted at: 2018-10-03T19:38:15.853Z Reads: 173

```
Remote worked first try🤣😂😂
```

---
## \#1714 Posted by: StefanMe Posted at: 2018-10-03T19:39:29.739Z Reads: 177

```
That’s so true
```

---
## \#1715 Posted by: lockeboss Posted at: 2018-10-03T19:41:04.855Z Reads: 173

```
But I can't change the pages in the settings
```

---
## \#1716 Posted by: rey8801 Posted at: 2018-10-03T19:42:19.528Z Reads: 171

```
I hope you insert the magnets correctly in the thumb wheel, otherwise is the hall sensor probably
```

---
## \#1717 Posted by: lockeboss Posted at: 2018-10-03T19:44:04.570Z Reads: 177

```
When I use the thump wheel in the normal mode is see bar going up and down so it seems to work
```

---
## \#1718 Posted by: rey8801 Posted at: 2018-10-03T19:51:27.030Z Reads: 180

```
ah ok then it's weird.
```

---
## \#1719 Posted by: clistpdx Posted at: 2018-10-03T19:59:34.498Z Reads: 180

```
The bar will still go up and down even if the magnets are in backwards. The bar just moves in the opposite direction. Try editing the min/max/center and see if min is a number between 0 and 200 ish. That's roughly where it should be
```

---
## \#1720 Posted by: lockeboss Posted at: 2018-10-03T20:00:20.872Z Reads: 172

```
Ahhh I think one magnet is wrong. In normal position I can switch up the pages but to switch down I have to turn the wheel upside down. So I think I have to change one magnet?
Also the double Nummer for pages like 11 won't fit in the rectangular frame
```

---
## \#1721 Posted by: lockeboss Posted at: 2018-10-03T20:03:36.120Z Reads: 175

```
Min is 0
Max is 1023center is 512
```

---
## \#1722 Posted by: rey8801 Posted at: 2018-10-03T20:03:56.104Z Reads: 173

```
in mine max is 865 I think so almost there.
```

---
## \#1723 Posted by: lockeboss Posted at: 2018-10-03T20:07:23.835Z Reads: 178

```
So are specific values for min max center which I adjust or how does it work? I need to switch one magnet I think :(
```

---
## \#1724 Posted by: rey8801 Posted at: 2018-10-03T20:08:37.736Z Reads: 177

```
no no the values are subjective tot the magnets you have, impossible to have same magnets strength. IF the wheels move correctly in both the direction should be ok.
```

---
## \#1725 Posted by: lockeboss Posted at: 2018-10-03T20:10:55.115Z Reads: 179

```
OK. So it's just the magnet I have too change. Man building this remote was an adventure😁
```

---
## \#1726 Posted by: rey8801 Posted at: 2018-10-03T20:17:12.874Z Reads: 174

```
it's a learning curve. Well took you two days, not to bad.
```

---
## \#1727 Posted by: StefanMe Posted at: 2018-10-03T20:26:17.131Z Reads: 174

```
That’s the problem. U just build the remote without understand how the components work together and how the code is implemented. 😉 but u ll get it after a few tries.
```

---
## \#1728 Posted by: clistpdx Posted at: 2018-10-03T20:32:11.909Z Reads: 187

```
[quote="lockeboss, post:1721, topic:28543, full:true"]
Min is 0
Max is 1023center is 512
[/quote]

Those are the default values. If you're running the dev code the OLED screen will display the ACTUAL hall sensor values while allowing you to adjust your min/max/center. If you're running the master code, you won't see these on screen. You'll have to enter debug mode inside arduino software and view the output there.
```

---
## \#1729 Posted by: lockeboss Posted at: 2018-10-03T20:32:59.760Z Reads: 187

```
Yeah I'm more the mechanical guy. But even my two IT guys where confused (but they heard of vesc and e skate the first time)

It's really good to experience how helpful people in this forum are :) 

Without rey8801 I would even have a remote or motors 😁
```

---
## \#1730 Posted by: lockeboss Posted at: 2018-10-04T21:06:56.589Z Reads: 197

```
So I used the dev version with the latest uart...
Is it normal that I don't have written words in the settings just can change the values via 1 2 3 etc

And the doubled numbers won't fit in the frame. 

Or is it because of the dev version??? 

![IMG_20181004_230305|689x239](upload://uRSbv2xSPMILQtZPHG4EFdHPft7.jpeg) 

![IMG_20181004_230136|375x500](upload://obqH69792jX2IJEMOYHqBTItLog.jpeg)
```

---
## \#1731 Posted by: Ryguy_MyGuy Posted at: 2018-10-04T21:20:40.451Z Reads: 189

```
Is there a way to make this remote able to change modes?  Maybe some programming?
```

---
## \#1732 Posted by: solidgeek Posted at: 2018-10-04T22:40:14.429Z Reads: 197

```
That is not the newest development branch. You have to update the remote to the latest version.

https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development
```

---
## \#1733 Posted by: lockeboss Posted at: 2018-10-04T22:58:09.334Z Reads: 197

```
Ah damn. Thank you
```

---
## \#1734 Posted by: chickengun Posted at: 2018-10-05T16:50:12.288Z Reads: 211

```
I just found [this](https://de.aliexpress.com/item/Free-Shipping-New-Pro-Micro-for-arduino-ATmega32U4-5V-16MHz-Module-with-2-row-pin-header/1804917596.html) arduino pro mini clone. There is a 3.3V/8MHz version for $3.42, so price range similar to arduino nano ATmega328p ($2).

For the esk8 remote this is interesting because if we use this arduino we don't need a 5v booster anymore + less noise when using the nrf transceiver.

![](https://cdn.sparkfun.com/r/600-600/assets/9/c/3/c/4/523a1765757b7f5c6e8b4567.png)

RAW is the unregulated voltage input (up to 12 V) and VCC is the voltage supplied to the on-board ATmega32U4 (3.3V, 8MHz). A supply going into the ‘RAW’ pin will be regulated down to the correct operating voltage of 3.3V which means the lipo/tp4056 can be attached directly without a 5v booster. I should try this for the next esk8 remote I build.
```

---
## \#1735 Posted by: StefanMe Posted at: 2018-10-05T16:59:56.531Z Reads: 194

```
BUT u ll only run in 8Mhz... do u know that’s enough? Or just make a try and error?
```

---
## \#1736 Posted by: chickengun Posted at: 2018-10-05T17:13:46.230Z Reads: 193

```
I think it will work, but have to do more research.
```

---
## \#1737 Posted by: marcgermany Posted at: 2018-10-05T17:36:58.937Z Reads: 204

```
Hey first i will say i love your work very great remote! i read much here about it and try to build it.all worked  but i have a little problem the throttle value is very small. now i saw this post and i am thinking maybe i am wrong because i used a 3,3v arduino pro mini but i used the raw pin for power it (there goes 5v) and the oled + the hall sensor too, but maybe thats wrong ? what can make a problem like mine? the remote show throttle value 50% too 99% when i rotate the wheelknob. regards from germany marc ;)
```

---
## \#1738 Posted by: StefanMe Posted at: 2018-10-05T19:48:13.215Z Reads: 203

```
How did u put the magnets together? One is normal way and the other one is upside down. In the settings menu u can adjust everything u need
Regards from Munich 😬
```

---
## \#1739 Posted by: solidgeek Posted at: 2018-10-05T20:43:33.558Z Reads: 201

```
As @StefanMe points out, maybe you didn't invert the polarity of the magnets? Another issue I can think of is that the SS495 hall sensor min voltage is 4.5V, so a 3.3V supply wont work. If you supply it from the 5V you wil be having issues as the OUTPUT voltage of the hall sensor will be to high for your 3.3V Arduino.
```

---
## \#1740 Posted by: moon Posted at: 2018-10-05T20:44:45.897Z Reads: 192

```
Hey, could you respond to my message?
```

---
## \#1741 Posted by: marcgermany Posted at: 2018-10-05T22:25:33.447Z Reads: 196

```
Thank you for the Info ;) i just put 2 magnets in the 2 holes at this moment i dont think about the direction, so i think thats my fault but i will test it tomorrow and let you know 
Regards from kreuzwertheim :wink:
```

---
## \#1742 Posted by: marcgermany Posted at: 2018-10-05T22:33:32.467Z Reads: 196

```
Thank you for the fast answer. :slight_smile: thought falsely wise that the digital pins 5v would be tolerant. I test everything tomorrow and give feedback. is it actually possible to exchange gas and brake? I'm used to it (gas forward / brake backwards). Regards from germany :wink:
```

---
## \#1743 Posted by: StefanMe Posted at: 2018-10-05T22:55:33.127Z Reads: 191

```
Just put the magnet in the wrong way in... ;) then everything is inverted.
Or invert the values in VESC...
```

---
## \#1744 Posted by: StefanMe Posted at: 2018-10-09T07:35:45.551Z Reads: 188

```
What is the best component for building at the moment. Did someone found a solution for an all power up/charge combination with 100 or 200ma charge current? 

Did anyone work on the feather M0?
```

---
## \#1745 Posted by: PaFe Posted at: 2018-10-09T09:09:11.915Z Reads: 182

```
Damn that was huge amount of wholesome information. Thank you all for your effort!
```

---
## \#1746 Posted by: tnschro Posted at: 2018-10-09T09:19:33.606Z Reads: 188

```
hello every one im about to build my own long board i just have a question what type of reciever you can control with this remote all 2.4ghz or is a specific one??
```

---
## \#1747 Posted by: StefanMe Posted at: 2018-10-09T11:04:38.200Z Reads: 193

```
@tnschro U use an Arduino with RF24 2.4gh board. U cannot use some kind of other receiver...

@PaFe ??
```

---
## \#1748 Posted by: PaFe Posted at: 2018-10-09T11:22:09.272Z Reads: 189

```
@StefanMe sorry I'm new to the forum and just red the whole history. Just wanted to say thanks to all of you for this great effort - it's insane.
```

---
## \#1749 Posted by: tnschro Posted at: 2018-10-09T13:55:22.564Z Reads: 179

```
So you need 2 RF24 2.4gh one for receiver and one for transmitter right??
```

---
## \#1750 Posted by: StefanMe Posted at: 2018-10-09T15:35:07.716Z Reads: 191

```
Correct. U have two times the same setup. Arduino with NRF24l01. Both send and receive information. One is in your remote and the other at your VESC
```

---
## \#1751 Posted by: marcgermany Posted at: 2018-10-13T13:22:15.631Z Reads: 186

```
now it works with 5v arduino pro mini and 2 magnets but in diff directions thank you for the help :)
```

---
## \#1752 Posted by: Scream Posted at: 2018-10-17T21:26:31.518Z Reads: 190

```
I'm having an issue where my transmitter won't boot correctly unless I push the reset button on the nano. 

It won't boot from just turning on the power switch. I get green and blue lights on the nano, but the lcd doesn't turn on.

It boots correctly 100% of the time when I push the reset button on the nano.

Any likely culprits here? I've tried the 10k resister from RX to GND as suggested by @HighMasterGogo... no change. I've tried turning it on and wiggling all wires to see if it might be a loose connection or short somewhere - nothing. Transmitter appears to be functioning as expected once the reset button is pressed, so wiring fault seems unlikely.

It may be relevant that the transmitter isn't 100% completed yet... I'm still waiting on the Hall effect sensor.
```

---
## \#1753 Posted by: SeeTheBridges Posted at: 2018-10-17T21:53:42.050Z Reads: 179

```
Get your hands on a really small ceramic cap to go between reset and ground. I use 22pF caps on all mine
```

---
## \#1754 Posted by: Scream Posted at: 2018-10-18T01:36:10.388Z Reads: 185

```
Hmmm... so I just soldered a ceramic capacitor between the RST and GND but it hasn't fixed the issue.

Just double checking I bought the right thing:

https://www.jaycar.co.nz/22pf-50vdc-ceramic-capacitors-pack-of-2/p/RC5316

Is there anything I should have done with the Arduino out of the box to prepare it? (Other than upload the two/three libraries and flash the code). I'm wondering if there's some code I'm missing which resets the Arduino when it's turned on?
```

---
## \#1755 Posted by: SeeTheBridges Posted at: 2018-10-18T02:27:57.089Z Reads: 187

```
Hmm, yeah. Those should work. If it's still freezing, you're gonna want to check the wiring on your NRF. If there's a short there, it can freeze up the whole nano.
```

---
## \#1756 Posted by: Scream Posted at: 2018-10-18T02:41:31.828Z Reads: 205

```
Yeah, that's something I'd be pretty worried about... soldering that NRF was a real MF.

Further information for diagnostic purposes:

- Remote boots correctly when micro usb connected directly to nano, but not from battery
- Battery is fully charged
- Boots every time after reset button pressed 
- Once remote has booted correctly (screen turns on) it pairs with the receiver every time (suggests NRF modules wired correctly?)
- Receiver doesn't seem to need any rebooting, gets straight into it every time. But then the receiver doesn't have an lcd screen, which is the main symptom of the problem with the remote.

Here’s a list of things I’ve tried:

Added 10K resistor from RX to GND

Added 22pF capacitor from RST to GND

Moved 10K resistor, so now from RX to TX

Jumped TX to GND, with 10K resistor between RX and TX

Checked resistance between all points on the NRF chip - confirmed no shorts

Double checked wiring schematic for NRF - confirmed wired correctly.

Checked battery voltage - 4.5V

Checked voltage from boost converter - 5.6V

Tried alternative battery (LG HG2 - 4V) - identical behaviour from remote (won’t boot from turning on switch, boots from pressing reset)

Interesting observation - if I open the circuit by disconnecting the battery, then reconnect the battery, the remote boots correctly. This is leading me to believe the issue is with the switch or the 10K resistor wired to Analog 2 (I’ve connected this to the switch).

EDIT

Can confirm the fault was with the 10K resistor and switch. I had wired the resistor to the side of the switch going to the charging board/battery. This meant the resistor was closing the circuit between the battery and analog pin 2.

I switched the resistor to the other leg of the switch, and everything is working perfectly.

Now the question is whether I should remove the RX resistor and RST capacitor? Any harm having them there if I’m not using them?
```

---
## \#1759 Posted by: rey8801 Posted at: 2018-10-20T18:36:31.170Z Reads: 200

```
ok now I feel a bit confused. I made already other remotes for VESC 4.12. Now on one of min board I moved to Flipsky 6.6 and the remote was working but I didn't get any real data on the remote. I read that I need to update the library. So I deleted the old VESC library and install the new one  https://github.com/SolidGeek/VescUart?files=1. I then dowload the last developer branch https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development. I opened them up add the library as usual for receiver and transmitter. Change the address on both of them and uploaded

(I wanted to upload a picture but the forum give me error message, please check the links)  https://www.dropbox.com/s/2tlu0djbvm7yxgu/IMG_20181020_202301.jpg?dl=0
https://www.dropbox.com/s/hle84j6bbdr7rby/IMG_20181020_202218.jpg?dl=0

All went fine but if I simply test to turn pair the remote with the receiver doesn't work anymore. Do you know what I am missing? Every time there is something new :laughing:
I tested the remote and receiver just by powered the receiver with the PC. Before was working like that.

ah BTW on the VESC 6.6 I am using Ackmaniac firmware, did someone tried with his firmware already the new vesc library?

Thanks guys!


EDIT: @clistpdx man could you give me your opinion. Sorry to bother :grin: I would like to have back the remote in working condition as before
```

---
## \#1760 Posted by: MrHappy Posted at: 2018-10-21T00:18:32.771Z Reads: 185

```
Im having an issue where the reciever wont connect to the remote unless i unplug and replug the PWM cable. It doesnt matter the order I boot up the Board or remotes. Its strange. My only idea is to have a push button on the outside of the case that lets me reboot the nano, but thats a silly solution.
```

---
## \#1761 Posted by: rey8801 Posted at: 2018-10-21T00:26:15.252Z Reads: 175

```
In that case seems like the receiver is freezing. Did you tried to add a mcp130 chip to the receiver? It takes care of the voltage drops. A small 22uF cap should also help in case is easier to find it. You can search for both in the thread.
```

---
## \#1762 Posted by: MrHappy Posted at: 2018-10-21T00:29:06.508Z Reads: 176

```
I followed @SeeTheBridges tutorial, ill have to find how to add that thanks. Which version of the Mcp130 chip should i get?
I'm a Mechanical Engineer, electronics are not my best friend
```

---
## \#1763 Posted by: dth2m5 Posted at: 2018-10-21T00:42:21.157Z Reads: 181

```
@solidgeek Great work! I didn't see it in the thread, but I did read that you have some connectivity issues.

Have you noticed and iterated on the position of the Bluetooth Antenna relative to your hand? Bluetooth signal is attenuated due to water and your hand is a big source of water.

Doug
```

---
## \#1764 Posted by: rey8801 Posted at: 2018-10-21T07:28:38.997Z Reads: 191

```
I used this one 10pcs/lot MCP130T-450I / TT MCP130 SOT23-3 new original
 https://s.click.aliexpress.com/e/bQluJSjO
```

---
## \#1765 Posted by: StefanMe Posted at: 2018-10-21T08:23:28.441Z Reads: 201

```
That’s strange... I never used any capacitors or something and it always works. I don’t know what unsre doing different. I also just use cheap Chinese nano clones ect. 

Now I just use an capacitor to make the hall sensor more stable, but that’s it. 

Maybe my software is a bit different? I use my own fork...
I developed an version of this remote to use the Adafruit Feather M0 with build in Lipo control and telemetry. An all in one solution.

![](https://cdn-shop.adafruit.com/1200x900/3177-00.jpg)
https://www.adafruit.com/product/3177

 This shit works awesome. U can even pair new receivers and switch between different boards... solidgerk is not working anymore on this branch. He has some other project at the moment.
```

---
## \#1766 Posted by: Livid Posted at: 2018-10-21T22:31:26.466Z Reads: 187

```
I'm having 2 types of disconnects riding my board with this remote, and frankly both terrify me. most often the board just returns to neutral, i improved this by adding an lc filter onto the rx power supply and some caps onto the nrf power on the receiver, still happens a bit though. the second variety locks the board in it's set power for 2-5 sec, which once nearly resulted in me going under a bus, but there seems to be no way to predict which one will happen, anyone have any ideas short of just adding more caps?
```

---
## \#1767 Posted by: StefanMe Posted at: 2018-10-22T10:53:15.409Z Reads: 184

```
What components are u using? I never had this issue...
```

---
## \#1768 Posted by: Livid Posted at: 2018-10-22T12:04:00.787Z Reads: 181

```
I'm using a chinese arduino nano, nrf24 module, got 4 capacitors on the power pads for the nrf24 and another on the power for the arduino
```

---
## \#1769 Posted by: rey8801 Posted at: 2018-10-22T12:50:25.709Z Reads: 182

```
Hi sorry to bother you but seems you are active on this topic, could you please check my previous post?https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/1759?u=rey8801
I basically moved to VESC 6.6 and so I used the new library for the UART port. Since there the remote doesn't pair with the receiver anymore. Am I missing something?
Thank you!
```

---
## \#1770 Posted by: Nordle Posted at: 2018-10-22T13:10:59.076Z Reads: 177

```
the one from the bom, cause there are many chinese ones with bad voltage regulators?
```

---
## \#1771 Posted by: StefanMe Posted at: 2018-10-22T14:24:42.494Z Reads: 178

```
Has nothing todo with the VESC. The UART is completely separated from the paring or anything else.

tune both, remote and receiver into DEBUG by uncommenting the //  from // define DEBUG and check the address. Could only be an address issue. Do u use the latest development commit?
```

---
## \#1772 Posted by: rey8801 Posted at: 2018-10-22T14:47:40.758Z Reads: 173

```
You are right about the UART library, cna not be that. It's just becuase is the only thing different compare to before. I used the last delevopment commit as I linked in the post https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development. Is it right? Do I still have to add the library or once they are installed in the arduino IDE they will be uploaded automatically? Here the picture of how I did it [https://www.dropbox.com/s/2tlu0djbvm7yxgu/IMG_20181020_202301.jpg?dl=0 ](https://www.dropbox.com/s/2tlu0djbvm7yxgu/IMG_20181020_202301.jpg?dl=0)
[https://www.dropbox.com/s/hle84j6bbdr7rby/IMG_20181020_202218.jpg?dl=0 ](https://www.dropbox.com/s/hle84j6bbdr7rby/IMG_20181020_202218.jpg?dl=0)

Thank you a lot!
```

---
## \#1773 Posted by: StefanMe Posted at: 2018-10-22T14:58:08.216Z Reads: 190

```
 Ahhhhh ok, at first remove all the things u added manually. Or simply just delete your sketch and download a new untouched version from the link u posted before. Open the sketch from the transmitter and upload the code without adding anything. Just open the stecht. Adjust the port and push upload.

U added accidentally some code to your sketch 
![image|281x500](upload://xOTgnO3iPaImJ5VuuPuxiYvKYEg.jpeg)


All this at least is wrong :slight_smile:
```

---
## \#1774 Posted by: rey8801 Posted at: 2018-10-22T15:35:28.223Z Reads: 170

```
Ok perfect. It actually it was what had to be done in the previous version. Those ones are the libraries. Anyhow I will try that, thanks.
```

---
## \#1775 Posted by: StefanMe Posted at: 2018-10-22T15:43:43.207Z Reads: 173

```
Yes, I have to add the library’s to the Arduino IDE but not add them manually to your sketch. All the code I have marked is not needed, because the libarys u need are written below. So what u did, was to add it in the code and add a lot of unessassery code above the main #include code. Give it a try and then we can see what’s next.
```

---
## \#1776 Posted by: rey8801 Posted at: 2018-10-22T17:32:26.823Z Reads: 184

```
Ok tried like that. Downloaded the development files again. Didn't add anything manually. Only Change the address in both receiver and trasmitter. Upload all fine. The remote and receiver still don't pair.
I didn't change my nrf24 and U8g2 libraries. Are you also using these ones
![IMG_20181022_192955|690x388](upload://lJrtWrK1G5Bw9iddTDp1icJpfoi.jpeg)
```

---
## \#1777 Posted by: StefanMe Posted at: 2018-10-22T21:23:09.844Z Reads: 177

```
I have a newer version of the u8g2 but this should not matter... 

open TOOLS - SERIAL MONITOR
uncomment // #define DEBUG 

upload code and show us what's going on on the first lines... there should be a problem with the address or the transmission.
```

---
## \#1778 Posted by: Livid Posted at: 2018-10-22T21:57:17.155Z Reads: 169

```
No, I used whatever i could find on ebay, looking at it now it doesn't have the extra voltage regulator, god dammit. Oh well, i'll keep slapping caps on to see if that fixes it
```

---
## \#1779 Posted by: sharky Posted at: 2018-10-23T07:36:09.157Z Reads: 175

```
Hy Guys!
Has anybody the Firefly remote and a Smartphone app in use?
SO my question is is it possible to get the Vesc data on the Remote and similar to the Smartphone (bluetooth module) ?
Can the Signal pins / on the VESC/Focbox  be connected to the Bluetooth module for the App and the receiver for the Firefly all in one?
For example on a single Focbox setup?
KR
```

---
## \#1780 Posted by: StefanMe Posted at: 2018-10-23T08:05:45.554Z Reads: 174

```
No. It’s not possible yet. Maybe in the future. It’s only possible in dual VESC setup
```

---
## \#1781 Posted by: sharky Posted at: 2018-10-23T08:14:41.531Z Reads: 169

```
ok thx for the reply
so in a dual setup one vesc will have the bluetooth module connected for the app an the other one will (probably the master) will get the remote commands and sends the info to the firefly
think ill try this when ive finished my firefly
Let you know if it worked out for me
KR
```

---
## \#1782 Posted by: StefanMe Posted at: 2018-10-23T08:29:06.007Z Reads: 172

```
It’s not a secret. It works ;)
```

---
## \#1783 Posted by: sharky Posted at: 2018-10-23T08:44:22.324Z Reads: 170

```
nice thx for the info
```

---
## \#1784 Posted by: rey8801 Posted at: 2018-10-23T11:15:11.825Z Reads: 199

```
ok so. Here the trasmitter (it sends the right address)

![image|546x500](upload://tVAJY2tSxQDlf1uM1w61EcH4JmH.png) 

here the receiver

![image|690x361](upload://5ypWoIv8QM6iskhKeCG3jLsqvlZ.png)
:weary: why these simbols at the receiver side?

Thanks for the help.
```

---
## \#1785 Posted by: StefanMe Posted at: 2018-10-23T11:40:49.078Z Reads: 173

```
U can choose the baudrate on the bottom left. Compare it to the baudrate in the code. Should be 115200
```

---
## \#1786 Posted by: rey8801 Posted at: 2018-10-23T11:45:17.452Z Reads: 202

```
If I check the code in the receiver is 115200
![image|516x500](upload://59TGrXO7lm2rEkrHCXAPcP8pCxm.png) 

While in the transmitter is 9600
![image|608x500](upload://3x7KBW7blP6U1IOY85YkVWWYVGx.png) 

Do you know why are they different? should I change the transmitter to 115200?

Now I understood what you meant. I am going now to try to change the baudrate during serial monitor at the receiver side.

Indeed it is sending wrong address!
![image|452x500](upload://cLiNQYNsNaiIywwB8ynWCedosHD.png) 

Why since I changed it in the code?
```

---
## \#1787 Posted by: rey8801 Posted at: 2018-10-23T12:01:41.976Z Reads: 178

```
Ok perfect. Apparently the receiver doesn't accept a new address. Do you know why?
I changed the address on the transmitter side to match the receiver and now they pair. That's so weird.
Do you know if it is normal that the transmitter is 9600 baud rate and the receiver is 115200? Thank you for the help. I learnt a new things, never rely just on code, always check...why it doesn't change the address remain a mystery to me.
```

---
## \#1788 Posted by: StefanMe Posted at: 2018-10-23T12:55:03.198Z Reads: 181

```
The different Serial baudrates are ok. Doesn’t matter...

No i am not to much into the normal code, because my code is handling the address in a totally different way. 

I guess I have to reset the address from the remote in the menu or something to force a new pairing... not shure. For now I ll not go in with the development on the Arduino Nano. I switched to the feather and short before finishing this code.
```

---
## \#1789 Posted by: rey8801 Posted at: 2018-10-23T13:02:17.665Z Reads: 180

```
ok no problem. Indeed in the remote you have to force to switch to the new default code but it won't change on the receiver. Weird because the code there was the one I used in the past with the previous development version. So I was able to change it before and now with the new version if I upload whatever address doens't change anything. Weird, Thanks for the help!
```

---
## \#1790 Posted by: clistpdx Posted at: 2018-10-23T15:42:47.493Z Reads: 185

```
[quote="rey8801, post:1789, topic:28543"]
So I was able to change it before and now with the new version if I upload whatever address doens’t change anything.
[/quote]
I had the same thing happen to me. I think it was storing the incorrect/old address in PRAM and the Nano and I couldn't fix it until I was able to flush the PRAM (or go back to using the default address). I'm not sure how I got the PRAM deleted but I eventually did and then it accepted my custom address
```

---
## \#1791 Posted by: rey8801 Posted at: 2018-10-23T16:18:17.803Z Reads: 181

```
yes exactly, @StefanMe helped me to figure it out. Indeed the receiver doesn't accept the new address but keeps the old one. Well It was already modified by me the first time so at least is not the real default one. Would be nice to correct this issue in the code.
```

---
## \#1792 Posted by: StefanMe Posted at: 2018-10-23T20:53:58.939Z Reads: 172

```
resetAddressPin = 4;

U can reset the address on the receiver by connecting pin 4 to ground for a second. ;) then everything should pair as before...
```

---
## \#1793 Posted by: Deakbannok Posted at: 2018-10-24T05:57:48.821Z Reads: 177

```
When first you have uploaded the code to your controller and receiver.  Your receiver RX default address is assigned (void). Thats why your address on receiver shows 0xe7e7e7..... I did fork an addictional code to the Receiver to have that assigns the value by default if is not validated.
```

---
## \#1794 Posted by: rey8801 Posted at: 2018-10-24T06:50:33.789Z Reads: 175

```
That's a cool trick! Thanks.
BTW I want to report back that now the remote works again and I am using Flibsky 6.6. And Ackmaniac firmware.
The only problem is that Flipsky voltage sensor is crap and does read 1-1.5V less theb real. On my 12s at 49.4V it reads 47.9V.
```

---
## \#1795 Posted by: StefanMe Posted at: 2018-10-24T07:54:19.236Z Reads: 172

```
Is the difference between real voltage and Vesc voltage always at the same value or does it increase by higher voltage? I can build on an factor for the voltage...
```

---
## \#1796 Posted by: rey8801 Posted at: 2018-10-24T08:30:30.019Z Reads: 178

```
Well it is a known behavior from Flipsky 6.6. I think is constant but I still have to go at lower voltage. For the moment ai decrease the cut out of 1V
```

---
## \#1797 Posted by: sofu Posted at: 2018-10-24T09:56:45.239Z Reads: 197

```
As @StefanMe said, the baudrate doesn't actually matter for connecting your transmitter to receiver. You're pointing to two different things. `#ifdef` is a preprocessor conditional macro. How `setup()` in receiver.ino reads is actually:

```
if you have the DEBUG macro on,
    set uart debug port append serial
    begin serial at baud rate 115200
    start printing in run loop
otherwise
    if firefly pcb macro on,
        set uart serial port append serial
        begin serial at baud rate 115200
```

This only has to do with serial output to uart, not communication with the transmitter. 

Just an explainer if you're still wondering :smiley:
```

---
## \#1798 Posted by: rey8801 Posted at: 2018-10-24T09:58:25.377Z Reads: 183

```
I see, thank you for the clarification!
```

---
## \#1799 Posted by: rey8801 Posted at: 2018-10-24T21:58:03.358Z Reads: 186

```
Hi! So you know our every tried to connect the UART jst from the receiver to the UART port of the slave VESC while the PPM signal is one the master? I mean the remote works with out the UART port (of course with out real time data). In this way the UART data comes from the slave vesc which should be the same anyway.
```

---
## \#1800 Posted by: tardyparty7 Posted at: 2018-10-25T04:28:04.736Z Reads: 187

```
Hi guys, for my school project I am going to make this remote. Unfortunately, I cannot find any parts that won't take **30-40 days to ship**. I have a limited time and I don't have enough time to find another project. Do you guys have any other places where I could by these without needing to pay upwards of **50 dollars for shipping in 13 - 15 days or pay none and have 30-40 day shipping**? Thanks!!
```

---
## \#1801 Posted by: StefanMe Posted at: 2018-10-25T05:27:34.515Z Reads: 185

```
It should work perfect. At least it should work in PPM split mode. I don’t run a dual motor system at the moment, so i can’t test it... maybe in the future.
Running the remote without real-time data is no option 😂 I mean... it would not give me that unique feeling
```

---
## \#1802 Posted by: StefanMe Posted at: 2018-10-25T05:29:20.557Z Reads: 183

```
I can buy everything working a few days from eBay in Europe... it would be strange if u could do this in USA or where ever u live.
```

---
## \#1803 Posted by: rey8801 Posted at: 2018-10-25T05:38:36.212Z Reads: 179

```
The remote works PPM only. Of course without the real time data doesn't make sense. That's why I was wondering to get this data from the slave Vesc instead so that I remove a bit of load from the master VESC. Otherwise now he has to sent data both to UART for the remote and to can for the Bluetooth on the slave. Thanks I might give it a try.
```

---
## \#1804 Posted by: StefanMe Posted at: 2018-10-25T06:08:18.899Z Reads: 178

```
I ll add an option to double the amps ect... I think we need it for a double setup without CAN
```

---
## \#1805 Posted by: walleywalker Posted at: 2018-10-25T06:15:04.788Z Reads: 193

```
What about a group buy for all the components listed?
```

---
## \#1806 Posted by: Blix Posted at: 2018-10-25T07:00:17.717Z Reads: 208

```
I would be in but only with the upgrades from @zyb :smiley:
Maybe @Zyb even has the parts and could send them to you...
```

---
## \#1807 Posted by: DroidSector Posted at: 2018-10-25T07:24:21.837Z Reads: 215

```
Almost finished a version of this great remote, it's based on Adafruit Feather M0 RFM69HCW:
![IMG_20181019_235919|332x500](upload://65qChTql8fyOmgus1SMjccwL48I.jpeg)
![Capture|690x394](upload://tB9IQrukhtojaqtxPm0wbQK4q0k.jpeg) 

I'll share the code and .stl files soon. The parts are more expensive but the delivery should be quicker:
[docs.google.com/spreadsheets/d/13rUPX8BsSac1AdnFAXx4dwR3XoQiU4FAKbunFaeW-oY](https://docs.google.com/spreadsheets/d/13rUPX8BsSac1AdnFAXx4dwR3XoQiU4FAKbunFaeW-oY/edit?usp=sharing)
```

---
## \#1808 Posted by: rey8801 Posted at: 2018-10-25T07:32:39.267Z Reads: 208

```
Really nice! I was wondering what are the improvement in using Adafruit instead of an Arduino? Just out of curiosity
```

---
## \#1809 Posted by: StefanMe Posted at: 2018-10-25T07:43:07.249Z Reads: 210

```
Are u kidding me 😂 I work also ok the feather and I am short before of releasing 😂
```

---
## \#1810 Posted by: DroidSector Posted at: 2018-10-25T07:43:17.928Z Reads: 212

```
It's just less wires to solder, as it has built-in battery charger and radio. On the receiver side Arduino + RFM69HCW Transceiver could be used to save $20, but did not tested it yet.
```

---
## \#1811 Posted by: StefanMe Posted at: 2018-10-25T07:45:08.808Z Reads: 219

```
![image|375x500](upload://mpH9RwR43vAvm3n5ZK1nQowfSoi.jpeg) lol exactly the same on my plan. What is your cycle time in best and worst case including transmissions?
```

---
## \#1812 Posted by: DroidSector Posted at: 2018-10-25T07:49:47.080Z Reads: 217

```
Yeah, saw your post only yesterday. Did not measure it yet, but managed to improve the response using this code:

    // update every half second
    if (millis() - lastScreenUpdate > 500) {
       u8g2.clearBuffer();

       drawPage();
       drawBatteryLevel();
       drawSignal();    
          
       lastScreenUpdate = millis();
    }

    u8g2.sendBuffer();
```

---
## \#1813 Posted by: StefanMe Posted at: 2018-10-25T07:51:33.325Z Reads: 201

```
That’s much to slow... my cycle time is 63ms including update display and send and revive all data. Worst case <100ms on bad transmissions...

Transmission time is 10ms - update display is around 55ms. If u drawing the display only every 500ms not smooth, doesn’t it?
```

---
## \#1814 Posted by: DroidSector Posted at: 2018-10-25T07:57:41.171Z Reads: 207

```
I originally used Feather 32u4, it struggled to draw all the data :)
```

---
## \#1815 Posted by: StefanMe Posted at: 2018-10-25T08:02:04.312Z Reads: 214

```
I like your stl. I wanna try them out!

Please try to measure your cycle time, transmission time and worst case cycle time to have a benchmark. With full GUI on OLED Of course.
```

---
## \#1816 Posted by: Fabialbo Posted at: 2018-10-25T12:27:32.678Z Reads: 228

```
wouldn't it be a great idea to fork the software to an Esp32/Lora/oled board? 

They a ridiculously cheap (15$ on AliExpress) and combine everything on one board: 
Lipo charger, OLED-Display, MCU with  WiFi/Bluetooth, low power wireless transmission without any range/bandwidth problems.
you can transmit well over 2 km if you don't restrict the transmission power. 
and they are way smaller which means more battery or smaller controller :)

You just have to use a 3V analog hall effect sensor. If there is any interest I could search and test a couple of them. allegro has a lot of hall-sensors in the already used to-92 flat package.

do some of you already have experience with the Lora chips?

I can offer to make new parts lists as well as new fitting enclosures for the Esp32/Lora board. 
I just have to little experience in C++ to fork the software.

these are the ones I would buy because they even have an onboard switch, but there are a lot of nearly identical boards for 15$

![a4615332c25dd5b92857eaaa9ec65d229c0449d0|690x236](upload://nsaP1zzFO2cL6l9sEsKfeWRGIGQ.png) 

[2pcs Lora Esp32 boards with OLED Aliexpress](https://www.aliexpress.com/item/2-Pcs-TTGO-LORA32-V2-0-433-868-915Mhz-ESP32-LoRa-OLED-0-96-Inch-SD/32844889787.html?ws_ab_test=searchweb0_0,searchweb201602_5_10320_10065_10068_318_10547_319_10548_317_10696_450_10084_10083_10618_452_535_534_10304_10307_533_5025915_10820_532_10821_10302_204_10843_10059_10884_323_10887_100031_5728715_10319_320_321_322_10103_448_449,searchweb201603_55,ppcSwitch_0&algo_expid=1df496d8-3af1-4a7a-b178-d7a2c9dee12d-2&algo_pvid=1df496d8-3af1-4a7a-b178-d7a2c9dee12d)
```

---
## \#1817 Posted by: DroidSector Posted at: 2018-10-25T13:41:22.987Z Reads: 225

```
This is a good find, I didn't know about this board. Will order and test the transmission speed. I used DRV5053OAQLPG 3.3v sensor, which was recommended in this thread, and it works fine.
```

---
## \#1818 Posted by: StefanMe Posted at: 2018-10-25T14:25:27.866Z Reads: 217

```
Haha we both use a 3.3 hall sensor. Mine worked great.  
OH49E SS49E from Honeywell 

I also didn’t know about this board. Looks awesome!
```

---
## \#1819 Posted by: tardyparty7 Posted at: 2018-10-25T18:27:48.645Z Reads: 211

```
Hey, does anyone have pictures for the inside of the remote?
```

---
## \#1820 Posted by: neiru37 Posted at: 2018-10-25T18:31:28.176Z Reads: 217

```
The ESP stack is kinda buggy, I've used these before and they'd just die out on me when I use them for a long time, forcing me to reset them.
```

---
## \#1821 Posted by: rey8801 Posted at: 2018-10-25T18:31:36.058Z Reads: 216

```
Check the several tutorials or scroll in the thread. You will find a lot of pics of the inside. You can also check my posts and you find one or two
```

---
## \#1822 Posted by: Fabialbo Posted at: 2018-10-25T18:47:16.568Z Reads: 216

```
cool :grinning: I think I just can't keep up with all the cool threads on this forum...
They are both exactly what I searched for (under 3V to over 5V support). The DRV5053 is even more efficient and only uses around 2-3mA compared 4-6mA of the Honeywell. Don't get me wrong they are both awesome, I just wanted to compare the sensors for others who have to decide. They are both a little bit over 1$ :+1:

If you want to know more about Lora i can just recommend [Andreas Spiess](https://www.youtube.com/channel/UCu7_D0o48KbfhpEohoP7YSQ/videos) he made tons of videos about the Lora boards and has a crazy amount of knowledge. yea the speed could be an issue. I had mixed up something in my head in the last comment. Apparently, they are quite slow...
```

---
## \#1823 Posted by: Fabialbo Posted at: 2018-10-25T18:54:43.206Z Reads: 224

```
mhh doesn't sound good...
how long ago was it? maybe Arduino bootloaders/compiler improved. i have its predecessor the ESP8266 in a small project of mine. for 3 years it ran without problems
```

---
## \#1824 Posted by: sharky Posted at: 2018-10-27T15:58:35.118Z Reads: 229

```
Just finished my first firefly remote sobi want to thank solidgeek for all the files and the know how and special thx to seethebridges and of course to this great forum.  I followed your how to vids on youtube got the remote running on the 1st try (still have to make the receiver and the final settings so im looking forward for the last vieo 😁)  Are there any instructions how to set up the remote in the remote settings?
Really like the remote so far i sprayed it with plast dip to make it more grippy and it fits soo good to my board
![IMG_5790|375x500](upload://A4N95TPdTdJXtNH2tdJcxlRgK5V.jpeg) ![IMG_5566|375x500](upload://aKZEapVsykcfX2WWRUE09fHaKT.JPG)
```

---
## \#1825 Posted by: chickengun Posted at: 2018-10-27T16:26:10.812Z Reads: 218

```
perfect match ;)
```

---
## \#1826 Posted by: Livid Posted at: 2018-10-29T22:12:09.559Z Reads: 215

```
hmm, a new antenna and linear regs installed on tx and rx and the dropouts are gone, but i'm still having an unusual failure where the throttle locks up for a few seconds randomly
```

---
## \#1827 Posted by: Yegmesh Posted at: 2018-10-30T02:01:07.300Z Reads: 222

```
I've remixed the top part of the remote with a larger screen for people who were interested.

[Remote Top With Larger Screen](https://www.thingiverse.com/thing:3184630)
```

---
## \#1828 Posted by: DroidSector Posted at: 2018-10-30T13:08:22.001Z Reads: 231

```
Just uploaded .stl files and code to GitHub:
https://www.thingiverse.com/thing:3185093

There is no settings menu yet, all parameters are in the code. It's also smaller, so please print it before ordering electronic components. 

![IMG_20181030_235402|619x500](upload://yOWtUX9b84V2b1iXYQERwgMiutT.jpeg) 

Just got RFM69HCW transceiver (~$2), will try to use it with Arduino Nano to make receiver cheaper. Also ordered TIGO LoRa32 board.
```

---
## \#1829 Posted by: StefanMe Posted at: 2018-10-30T14:01:34.741Z Reads: 227

```
Thanks... what’s about your times? 

Cycle time
Display refresh time
Transmission time...
Worst case cycle time over 15 minutes or something... 

That’s super important.
```

---
## \#1830 Posted by: MrHappy Posted at: 2018-11-02T02:33:06.927Z Reads: 221

```
So ive got some MCP chips on hand now. I dont have the PCB for the reciever, what pins should i connect to the chip.
```

---
## \#1831 Posted by: DjamboBuksne Posted at: 2018-11-02T16:54:27.754Z Reads: 219

```
I can do, If you're still interested.
```

---
## \#1832 Posted by: willumpie82 Posted at: 2018-11-05T07:40:57.793Z Reads: 211

```
I like your design, (bit like the other micro remotes from china) I'm thinking of going with one of these [boards](https://nl.aliexpress.com/item/TTGO-SX1276-SX1278-LoRa-ESP32-868-915-mhz-433-mhz-Bluetooth-WI-FI-Internet-Antenne-Development/32844017936.html) (esp32 + sx1278) from alixpress (also available with mounted oled), imo the feathers from adafruit are a bit to expensive at 25$,
```

---
## \#1833 Posted by: DroidSector Posted at: 2018-11-05T08:01:53.587Z Reads: 208

```
Please see my [post](https://www.electric-skateboard.builders/t/firefly-nano-remote/72916/38?u=droidsector). I'll update STL files to accommodate esp32 board after testing, it's almost the same size.
```

---
## \#1834 Posted by: Scream Posted at: 2018-11-06T04:35:52.300Z Reads: 212

```
Does anyone have a vector file for the firefly logo used in this rendering?

https://www.electric-skateboard.builders/uploads/db1493/original/3X/3/d/3d175c9a45adba6b5b793992130610435e6ec4c6.png

I want to engrave my scream logo on a wood and aluminium version of this remote, but I'd feel better about doing that if it had the firefly logo as well to pay homage.
```

---
## \#1835 Posted by: StefanMe Posted at: 2018-11-06T08:31:41.299Z Reads: 204

```
i got it as DXF... if it helps
```

---
## \#1836 Posted by: Scream Posted at: 2018-11-06T09:07:51.090Z Reads: 206

```
Yeah that’d be cool. Just any graphic file I can work with.
```

---
## \#1837 Posted by: StefanMe Posted at: 2018-11-06T09:16:50.012Z Reads: 207

```
Give me your email... i cannot upload DXF here
```

---
## \#1838 Posted by: bevilacqua Posted at: 2018-11-06T09:30:29.662Z Reads: 210

```
Best way is sharing a dropbox/GDrive (or any cloud) link. That way you share it only once and everyone can acces it ;)
```

---
## \#1839 Posted by: SynteX Posted at: 2018-11-11T20:42:24.279Z Reads: 204

```
I'm using the latest development code from github but my remote won't bind with the receiver? What can go wrong? I checked the soldering and it all looks great.
```

---
## \#1840 Posted by: clistpdx Posted at: 2018-11-12T16:45:04.331Z Reads: 203

```
[quote="SynteX, post:1839, topic:28543"]
my remote won’t bind with the receiver?
[/quote]

I had the same symptoms and found that it was interference that the transmitter was receiving from other components in the remote. I solved it by masking everything but the antenna with copper tape, and also soldering a 3 inch wire antenna to the ends of the ceramic antenna.  If you place your finger on the ceramic antenna do you temporarily get a connection? I would, which is how I diagnosed the issue.
```

---
## \#1841 Posted by: SynteX Posted at: 2018-11-12T20:59:45.601Z Reads: 195

```
I'll try Thanks!!!
```

---
## \#1842 Posted by: StefanMe Posted at: 2018-11-12T21:02:33.178Z Reads: 193

```
That sounds so scary :rofl:

@SynteX make sure u have on both devices the same ADDRESS set... AND MAKE IT UNIQUE PLEASE
```

---
## \#1843 Posted by: SynteX Posted at: 2018-11-12T22:01:24.930Z Reads: 193

```
Both are running stock development branche gor test mode. Also i can't find any adress variable anymore.
```

---
## \#1844 Posted by: SynteX Posted at: 2018-11-12T22:03:29.675Z Reads: 192

```
Still can't get it to bind i'm using the nrf chips from the order list.
The remote signal icon keeps flashing the signals...
```

---
## \#1845 Posted by: StefanMe Posted at: 2018-11-12T22:03:30.367Z Reads: 208

```
![36|402x500](upload://mHViprLq62YhPNkyyjfW5Y1F7v0.png)
```

---
## \#1846 Posted by: SynteX Posted at: 2018-11-12T22:06:18.344Z Reads: 194

```
found it but first need to solve the binding issue but i have no clue at all!!!
```

---
## \#1847 Posted by: StefanMe Posted at: 2018-11-12T22:10:42.369Z Reads: 198

```
Did u tried the debug mode and check remote and reciever?
```

---
## \#1848 Posted by: SynteX Posted at: 2018-11-12T22:19:57.054Z Reads: 201

```
Will do that tomorrow evening. Is there something i can notice with debug mode? something i have to look for?

(I know how to enable it)
```

---
## \#1849 Posted by: StefanMe Posted at: 2018-11-12T22:29:57.505Z Reads: 200

```
U will see if the transmitters are working properly
```

---
## \#1850 Posted by: SeeTheBridges Posted at: 2018-11-13T00:16:28.699Z Reads: 201

```
So judging but what you've said so far, it sounds like you haven't cleared your EEPROM. When you reflash anything you need to clear the EEPROM first so that the address will take and everything can connect. If you go into the example sketches in the arduino IDE, there's an EEPROM clear sketch that'll run, then turn on the blue LED when it's done. Do that to both the remote and receiver, THEN flash the dev branch again. If you want to change the connection address, you'll need to clear the EEPROM again before flashing the code with the new address. Otherwise, the new address won't take.
```

---
## \#1851 Posted by: tardyparty7 Posted at: 2018-11-13T01:25:40.509Z Reads: 187

```
Have u made the five video yet?
```

---
## \#1852 Posted by: SeeTheBridges Posted at: 2018-11-13T02:52:26.065Z Reads: 189

```
Script was finished before the semster started, but unfortunately I haven't had access to any of my other gear while at school. So no, not yet. I'll hopefully be home next week and can finish up the series then.
```

---
## \#1854 Posted by: SynteX Posted at: 2018-11-17T14:53:46.046Z Reads: 184

```
It seems that this indeed was the issue! I'm only wondering how to change the adress? Is there a place we're i can generate a new one or can i just smash my keyboard?
```

---
## \#1855 Posted by: ShutterShock Posted at: 2018-11-23T03:32:21.542Z Reads: 178

```
Hey guys has anyone had issues with their computer not detecting their Arduino at all?  I have been looking around and I can't seem to figure it out.  It powers on from the usb power but for some reason it is not detected by the Arduino IDE and I can't seem to find it in device manager to even try to force install a driver.

For reference I have the exact boards that were suggested to buy.  Black with the resonators on them and enhanced voltage control stuff
```

---
## \#1856 Posted by: Scream Posted at: 2018-11-23T03:37:00.039Z Reads: 178

```
Using a Mac by any chance? I had to fluff about downloading a new driver. Something to do with it not being a genuine Arduino and the knock offs use a cheaper usb module or something...
```

---
## \#1857 Posted by: ShutterShock Posted at: 2018-11-23T03:40:18.190Z Reads: 182

```
No I am using a PC. I do believe that you are required to download a new driver for the C340G communication chip.  I am not sure that cheaper board is the correct term considering it is built better than the original from my standpoint haha

Anyway I haven't gotten it to work yet.  Did you have success with your own?
```

---
## \#1858 Posted by: Scream Posted at: 2018-11-23T03:46:37.125Z Reads: 189

```
Yeah I managed to get mine working - muddled my way through. That’s good to know about the chip - it works which is all I care about.

Only other thing I guess is the settings in the Arduino interface... but then you probably know how to use an interface.
```

---
## \#1859 Posted by: ShutterShock Posted at: 2018-11-23T03:47:52.706Z Reads: 200

```
Yeah haha I know how to use the interface.  I haven't figured out how to install the driver without selecting the device though because for whatever reason the nano doesn't even show up as an unknown usb serial interface or anything.

Did yours show up in device manager or are you on MAC

Here's the chip in question![20181122_195003|375x500](upload://f8VXMyIeaa2SN9atXbdFM79DdkY.jpeg)

You can see it in the middle
```

---
## \#1860 Posted by: Scream Posted at: 2018-11-23T03:51:11.659Z Reads: 192

```
That does sound a lot like the issue I was having until I downloaded the driver for that chip... I don’t know the technical terms but there wasn’t even showing up as connected when I checked devices in “about this Mac”. So my extremely noob diagnosis would be that you don’t have the right driver correctly installed...
```

---
## \#1861 Posted by: ShutterShock Posted at: 2018-11-23T03:51:41.520Z Reads: 190

```
Yeah that is what it is seeming like to me.  I guess I shall continue to try and install haha

Man I call myself an expert and I just now tried a different usb cable -_- 

Guess what.  I did install the driver properly, the usb cable just didn't work.
```

---
## \#1862 Posted by: ShutterShock Posted at: 2018-11-24T09:02:22.724Z Reads: 199

```
Okay so I am further along in my progress now, but have hit another sticky point.

The remote and receiver are both finished (soldered and everything) and I managed to get the code on both the receiver and remote.  The remote boots up fine and I can enter into config mode when I use the trigger and stuff, so I think that is all good.

I have no idea how to actually get the receiver to connect to the remote, I turn both on and it just stays blinking.  I made sure to change my pipe to another compatible hex number, on both sides.  I don't know what else to do at this point and I have basically read this entire post, all 1800 of them, and I don't know what to do now.

I entered the debug mode on the transmitter side and it said failed transmission 512 over and over again, looking around it seems like other people had this issue when their board wasn't soldered right, but I double checked mine and eveything looks right.  I have the capacitors on the receiver board as well as suggested by @SeeTheBridges 

Also weird thing to note, you cannot program the receiver once you put the small cap between the gnd and rst pins.  That was an annoying one to figure out.  Also it seems that when the receiver is powered on, the L light stays lit constantly and the rx light consistently blinks.  I do not know if this is normal or not, as the lights on the transmitter show differently. 

If anyone has ideas here, I know there are many people who have sucessfully completed this and I am almost there, just need a little more help.
```

---
## \#1863 Posted by: Zyb Posted at: 2018-11-24T09:38:07.925Z Reads: 186

```
first of all dont just solder cap between reset and ground. i suggest you do it following way and you shouldnt have problems with uploading a sketch. connect reset to positive end of the cap(10uF) and negative end of the cap goes to 470 ohm resistor and the other leg of the resistor goes to the ground this way you wont damage anything and you shouldnt have issues with uploading a sketch. like this RESET --- (+)Cap(-)---470ohm---Gnd :) crappy illustration. for the other issue you have i would check again the wiring of the nrf and the solder job. try another sketch etc..
```

---
## \#1864 Posted by: Scream Posted at: 2018-11-24T09:51:05.524Z Reads: 186

```
I also had the same issues - couple of things...

I wrapped both nrf modules in copper tape, leaving only the antenna exposed. Pretty sure that’s what fixed it for me.

But also, I read that the receiver doesn’t get enough power to run the nrf chip when it’s powered by usb. So I wasn’t too worried about not getting a great connection when desk testing.

All the same, mine connects fine with the receiver powered by usb since I did the shielding.
```

---
## \#1865 Posted by: Zyb Posted at: 2018-11-24T10:00:19.799Z Reads: 174

```
oh yes and theres the power issue if you are using those blue arduinos they wont be able to feed required current to nrf. copper tape is a good idea too just make sure to put something non conductive like kapton tape underneath
```

---
## \#1866 Posted by: ShutterShock Posted at: 2018-11-24T16:41:54.711Z Reads: 173

```
Interesting I'll try this, the capacitor I'm using for the reset issue isn't polarized but I'll try putting the 470 ohm resistor and see if that helps.
```

---
## \#1867 Posted by: ShutterShock Posted at: 2018-11-24T16:43:30.269Z Reads: 179

```
I can see that making sense, USB is only 500mA on a standard port, but mine is plugged into my VESC so I don't think that was the issue. I will try shielding the nrf modules and report back about that.

Do you have to do anything to connect the rwo or is it just supposed to be automatic?
```

---
## \#1868 Posted by: ShutterShock Posted at: 2018-11-24T16:44:06.307Z Reads: 175

```
I'm actually using the nice black ones that the original maker used for mine
```

---
## \#1869 Posted by: Zyb Posted at: 2018-11-24T16:58:44.357Z Reads: 187

```
when pipes are matching they should connect automatically and yes non polarised caps like ceramic ones work too
```

---
## \#1870 Posted by: sharky Posted at: 2018-11-28T14:53:01.791Z Reads: 197

```
Hey Guys!
Just saw the possibility to turn on and off the lights by using an Turnigy receiver switch
https://www.amazon.de/Hobby-King-Turnigy-Receiver-Controlled/dp/B012W6RJ5I/ref=sr_1_6?ie=UTF8&qid=1543414701&sr=8-6&keywords=receiver+switch
there fore a 2nd channel is needed on the remote would this be possible with the firefly?
what has to be changed?
KR
```

---
## \#1871 Posted by: SimonVoss Posted at: 2018-11-28T16:46:19.314Z Reads: 195

```
Hey @SolidGeek jeg har svært ved at finde delene billigt i danmark/EU...
Gør du dig i at sælge et komplet sæt, en færdiglavet remote og receiver eller bare nogen af delene?
Jeg søger specielt en UIOTEC SMD NRF24L01 billigere end 26€ det står til på amazon
```

---
## \#1872 Posted by: solidgeek Posted at: 2018-11-28T21:23:39.906Z Reads: 192

```
Actually a second channel is not needed. You just have to add a boolean variable to the datastructure that is being sent with the RF24 library. You will have to update the structure on both receiver and transmitter site
```

---
## \#1873 Posted by: Scream Posted at: 2018-11-30T10:49:29.787Z Reads: 203

```
I know you guys probably feel like this has been explained a few times already... but how does the calibration process work? The throttle/brake in my remote seems to jump from 0 to 100% and I can't navigate the menus.

I have managed to work out what is meant by "uncomment #define DEBUG...", and get the following output from serial monitor:

![06%20PM|690x353](upload://lFcId2EE0CA3yUFi8jkRlWzm3Gt.png) 

I can't see anything in the output about maxHallValue or minHallValue... what should I be looking for?

EDIT:

[quote="solidgeek, post:418, topic:28543"]
**The polarity isn’t opposite** . Check the polarity of the magnets, they have to be opposite (one being north and the other being south). If they aren’t opposite, drill a small hole beneath each magnet and push them out.
[/quote]

Durrr... This explains my troubles navigating the settings menu... will rectify this tomorrow!
```

---
## \#1874 Posted by: Scream Posted at: 2018-12-03T03:21:41.408Z Reads: 196

```
Hahaha I’ve just realised why I’ve had so many issues getting this remote working. I was getting only 100% or nil throttle, and I couldn’t get any brake. I’d switch the magnets and I got all brake, no throttle.

My hall effect sensors from ali express basically just never showed up, so I bought what I thought was a suitable replacement from a local electronics store.

Turns out I bought a hall effect switch. It either outputs a voltage or it doesn’t. No amount of tweaking the software or fiddling with the magnets was going to fix it. 

So yeah... don’t do that guys.
```

---
## \#1875 Posted by: Pete75 Posted at: 2018-12-04T05:56:24.254Z Reads: 202

```
Just a quick question the remote seems to turn on maybe one out of 7 times. When the blue and green light on arduino come on it will not turn on. I have to cycle the switch a few times. But if I turn it on and press the reset button it fires up every time. What have I stuffed up. Do I need a cap somewhere?![15439028287853142593687591262988|281x500](upload://tfb2RH5oUWnYznPbZheuFAA6ra9.jpeg) ![15439028941583716398239756517937|281x500](upload://jEA0BJvrWYTFc6fDHCgiFOg6Dr8.jpeg)
```

---
## \#1876 Posted by: Pete75 Posted at: 2018-12-04T23:49:04.964Z Reads: 194

```
Never mind. Placed a cap between reset and ground. Problem fixed.
```

---
## \#1877 Posted by: sharky Posted at: 2018-12-05T17:40:37.938Z Reads: 198

```
Thx @solidgeek and @SeeTheBridges for all the know how to build the remote
Any way to donate this? Let me know😉
Kr sharky
```

---
## \#1878 Posted by: SeeTheBridges Posted at: 2018-12-05T18:37:52.669Z Reads: 199

```
SolidGeeks has a donation link here! 
https://www.paypal.me/solidgeek
```

---
## \#1879 Posted by: sharky Posted at: 2018-12-05T22:07:28.804Z Reads: 194

```
Thx money is on the way
```

---
## \#1880 Posted by: Scream Posted at: 2018-12-06T00:49:31.657Z Reads: 200

```
Just be aware that a cap wired this way may cause issues for your Arduino when using the IDE (for debugging or updates). You may need to remove it to get it to work.

When I had some trouble getting my transmitter working, I tried a bunch of things including wiring a cap in this way. 

Turns out my issue was actually that my battery voltage wire was connected on the wrong side of the switch so my transmitter wasn’t properly rebooting when it was switched on. I left all the other stuff wired up (cap between reset and ground, resistor between RX and TX), because I figured it wasn’t doing any harm.

When it came time to debug my transmitter I found it wasn’t playing nice with the Arduino IDE - something to do with not being in sync or something. Once I removed all the extra stuff it returned to working flawlessly.

The reason I think it’s the cap is because the error messages I was getting were apparently to do with the Arduino reset not being in sync with the IDE... the IDE expects the board to reset at certain times during the writing process. I suspect the cap was interfering with this and causing the board and IDE to be out of sync.
```

---
## \#1881 Posted by: Chupacabra Posted at: 2018-12-06T06:56:24.382Z Reads: 190

```
@SeeTheBridges Are you taking any orders for complete builds ?
```

---
## \#1882 Posted by: SeeTheBridges Posted at: 2018-12-06T07:47:57.184Z Reads: 195

```
Not at this time. I can take limited parts only orders, but I'm not home enough to assemble completes
```

---
## \#1883 Posted by: StefanMe Posted at: 2018-12-06T08:32:47.323Z Reads: 203

```
Its a good idea to put hot glue on all the solder joints where wires come out. its so easy to get a loose wire while using this thing hard. This is why i prefer a PCB... looks much safer. 

![](https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/5/5/5547572784f3b0d9ca03bd08aa147a5b556c3171_1_375x500.jpeg)
```

---
## \#1885 Posted by: Pete75 Posted at: 2018-12-09T09:43:10.168Z Reads: 192

```
Ok Guys. I have built the remote and receiver with the Development codes for both. I am using FOCBOX running version 2.18. I am getting no movement in the BLDC ppm monitor.  How do I check if the TX and RX are really talking. Do I need to update the focbox firmware to something else?  Any Advice appreciated
```

---
## \#1886 Posted by: Pete75 Posted at: 2018-12-09T11:57:15.384Z Reads: 196

```
Done the debug and me moving the wheel changes the value but not in Ack maniac esc tool (updated my Focbox to latest FW). tried both ppm and ppm and uart.![Untitled|690x388](upload://gKlcTTrgtrzRSf8fKyLlLC3P7VQ.jpeg)
Oh BTW this debug was done with the receiver unplugged from the vesc
```

---
## \#1887 Posted by: Nordle Posted at: 2018-12-09T14:07:12.766Z Reads: 187

```
is the code for feather chip, same as for arduino?
```

---
## \#1888 Posted by: Pete75 Posted at: 2018-12-10T00:48:28.340Z Reads: 187

```
Solved Issue was a unfiltered 5v that was stuffing it up added some filtering and problem was fixed.
```

---
## \#1889 Posted by: ervinelin Posted at: 2018-12-10T06:56:33.862Z Reads: 189

```
Only if you use the 328P feathers and do some custom re-mapping of the pins and such...
```

---
## \#1890 Posted by: elman Posted at: 2018-12-12T10:06:34.215Z Reads: 188

```
Why solidgeek.dk doesn't work?
```

---
## \#1891 Posted by: Zyb Posted at: 2018-12-12T11:48:14.848Z Reads: 191

```
Nrf24 chip doesn’t like the voltage changes at all. It is not a problem but rather a drawback in feather boards. In order to maintain 3.3v on the system they use a linear voltage regulator and it can’t keep it up when battery drops to around 3.5v depending on the diode they use to switch between usb and battery power. So having a big battery helps to keep the voltage higher for longer so the voltage regulator can do it’s job properly. Battery in the original firefly Bom is good enough but only if you charge it after every ride.
Probably using 5v switching regulator is the best to use the battery to its fullest potential and drop the voltage only for the nrf. That is actually how original design works.
Another option is to use 2s battery to keep the voltage input high enough but that just complicates the charging system.
```

---
## \#1892 Posted by: swimmydude Posted at: 2018-12-12T15:46:25.295Z Reads: 192

```
Yea, it gave me issues when I tried to go on there for a reference last night. It's back up now. If it happens again, you can at least go to a cache page to see the information you need.
```

---
## \#1894 Posted by: lukasilestam Posted at: 2018-12-20T00:40:41.094Z Reads: 181

```
anyone knows how to increase the power of the NRF? I have set PA_MAX and when the hand covers the remote control, NRF lost connection :confused:
```

---
## \#1895 Posted by: ervinelin Posted at: 2018-12-20T03:10:57.645Z Reads: 185

```
Which NRF module and how did you position it?

I find the module (and antenna if you have one) are extremely fussy when it comes to placement within the remote itself.
```

---
## \#1896 Posted by: lukasilestam Posted at: 2018-12-20T15:44:59.694Z Reads: 195

```
Here:
![IMG_0629|382x500](upload://1Dfu3ekypQpLAg6BRnB3ibhnqXs.jpeg) 

I have this nrf:
![nrf24-fig1|596x469](upload://j09CssYbi37cx80AjZuNJQxFiOw.jpeg)
```

---
## \#1897 Posted by: ervinelin Posted at: 2018-12-20T15:59:16.731Z Reads: 190

```
Yeah this one is not the best module to get... I am using these now..

[E01-ML01S SPI nRF24L01P 2.4Ghz 1mW PCB Antenna IoT uhf Wireless Transceiver nRF24L01 PA LNA Transmitter Receiver rf Module  http://s.aliexpress.com/InYjyEze](E01-ML01S SPI nRF24L01P 2.4Ghz 1mW PCB Antenna IoT uhf Wireless Transceiver nRF24L01 PA LNA Transmitter Receiver rf Module  http://s.aliexpress.com/InYjyEze)
```

---
## \#1898 Posted by: lukasilestam Posted at: 2018-12-20T17:08:30.235Z Reads: 188

```
thank you!
what do you think about this: https://aliexpress.com/item/2-4GHz-rf-Wireless-uhf-Module-Power-Amplifier-E01-ML01SP4-Original-SENET-1-8km-2-4g/32806320077.html
I ordered a week ago
```

---
## \#1899 Posted by: ervinelin Posted at: 2018-12-20T17:41:28.389Z Reads: 189

```
I use this too.. but you'll need an external antenna.

The antenna position within the remote is very sensitive, having it in the wrong place means zero signal for some weird reason.
```

---
## \#1900 Posted by: Sascha_stevenson Posted at: 2018-12-23T19:19:38.756Z Reads: 193

```
does this have a 3.3v regulator??

https://www.dx.com/p/RobotDyn-Nano-V3-ATmega328CH340G-Micro-USB-Pin-headers-NOT-Soldered-Compatible-for-Arduino-Nano-V30--2061744#.XB_fPC2cYWo
```

---
## \#1901 Posted by: sanderfu Posted at: 2018-12-23T19:26:47.381Z Reads: 192

```
Yes, it takes 6-12V (5V over usb) in and output 3.3V it says on the website so it appears this has a voltage regulator as would also be likely as a seperate regulator for 3.3V is not mentioned in the parts lists.

I think this is the RobotDyn one that Solidgeek also has linked on Aliexpress.
```

---
## \#1902 Posted by: Sascha_stevenson Posted at: 2018-12-23T19:27:47.280Z Reads: 193

```
thank you!
```

---
## \#1903 Posted by: BigBrit Posted at: 2018-12-23T19:43:33.613Z Reads: 198

```
where can you buy those PCB's bud?
```

---
## \#1904 Posted by: StefanMe Posted at: 2018-12-23T19:46:08.849Z Reads: 203

```
I created them by my own... but these are with totally different hardware.

https://www.electric-skateboard.builders/t/featherremote-and-smartremote/74084
```

---
## \#1905 Posted by: Sascha_stevenson Posted at: 2018-12-24T11:54:55.519Z Reads: 193

```
would this hall sensor work? [https://www.ebay.co.uk/itm/HONEYWELL-S-C-SS495A-SENSOR-RATIOMETRIC-LINEAR-/351163597255 ](https://www.ebay.co.uk/itm/HONEYWELL-S-C-SS495A-SENSOR-RATIOMETRIC-LINEAR-/351163597255)
```

---
## \#1907 Posted by: StefanMe Posted at: 2018-12-24T12:04:00.995Z Reads: 194

```
Its the sensor from the BOM... so of course it will work if u stick to the basic 5V Arduino nano
```

---
## \#1908 Posted by: Deakbannok Posted at: 2018-12-26T00:29:49.553Z Reads: 200

```
@StefanMe I will try out your controller. Despite it Is hard to buy adafruit in Europe.

I am still using Firefly controller at moment and still keep my firefly code up to date.
```

---
## \#1910 Posted by: Sascha_stevenson Posted at: 2018-12-26T13:29:00.685Z Reads: 205

```
@solidgeek @StefanMe 
anyone used this module? or know if it works
https://www.banggood.com/GT-24-Digital-Wireless-Module-2_4G-NRF24L01-PA-LNA-Industrial-Grade-1100M-Long-Distance-With-Welding-p-1361359.html?gmcCountry=GB&currency=GBP&createTmp=1&utm_source=googleshopping&utm_medium=cpc_elc&utm_content=zouzou&utm_campaign=pla-uk-ele-pc&gclid=Cj0KCQiAgf3gBRDtARIsABgdL3nA-F3WFS0UNnHmD-NEbE9Lo_xnKTuM0pyMwJSdUC7HTi_w13HWmJYaAlE0EALw_wcB&cur_warehouse=CN
```

---
## \#1911 Posted by: StefanMe Posted at: 2018-12-26T13:32:38.965Z Reads: 196

```
Looks like it’s a combined SMD and TH module... should work. It’s just a bit bigger than the regular one. Why u wanna use it? Just take the normal one. Or a high quality one...
```

---
## \#1912 Posted by: Sascha_stevenson Posted at: 2018-12-26T13:35:12.789Z Reads: 192

```
because it is another 40 days wait for the one listed on the build :joy:
but would it work as a temporary one?
```

---
## \#1913 Posted by: StefanMe Posted at: 2018-12-26T13:36:26.054Z Reads: 196

```
Yes module should work... u can use SMD or TH to connect it.
```

---
## \#1914 Posted by: Scream Posted at: 2018-12-27T08:59:52.557Z Reads: 203

```
Any Firefly geeks keen to work on getting telemetry working with the Focbox Unity?

Here's the post from Jeff (Deodand) where he talks about the change he made to the UART protocol for the Unity.

https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/121?u=scream

Am I correct that we would need to make changes to the datatypes.h code in the VescUartControl-new file?
```

---
## \#1915 Posted by: KranzeKake Posted at: 2018-12-27T12:35:49.447Z Reads: 196

```
I just ordered a firefly and a unity. Let me know if I can help
```

---
## \#1916 Posted by: Zyb Posted at: 2018-12-28T11:42:02.498Z Reads: 194

```
Yes this particular nano has dedicated 3.3v regulator underside of the board.
```

---
## \#1917 Posted by: Scream Posted at: 2018-12-29T09:07:50.353Z Reads: 203

```
Sorry cbf reading through every solution on this thread - any quick fixes for intermittent cutouts?

I have built the remote and receiver according to this tutorial:
https://solidgeek.dk/docs/firefly-remote/

It’s plugged into a unity. 
I added the power filtering to the receiver today but it didn’t fix the issue. In my skim through this topic I saw a few mentions of adding caps to the receiver Arduino between 5v and gnd. Is that the solution?
```

---
## \#1918 Posted by: totalgeek9224 Posted at: 2018-12-29T10:04:55.956Z Reads: 191

```
Im no expert, but when you say power filtering to the receiver (if u used something like a LC filter), i believe that would have the same effect as the capacitor
```

---
## \#1919 Posted by: Zyb Posted at: 2018-12-29T10:54:16.657Z Reads: 199

```
If you don’t have a cap on 5v sure add it and see if it helps other than that it could be fluctuations on 3.3v
```

---
## \#1920 Posted by: Deakbannok Posted at: 2018-12-30T01:57:17.418Z Reads: 213

```
![TEST|690x431](upload://9E6Skx3oGpTanQe6zQqqPuemkac.jpeg) 
Making it more compact and durable. Nothing change on parts.
```

---
## \#1921 Posted by: Sascha_stevenson Posted at: 2018-12-30T23:34:08.257Z Reads: 209

```
@Deakbannok search for firefly nano. :wink:
```

---
## \#1922 Posted by: StefanMe Posted at: 2018-12-31T00:00:11.351Z Reads: 217

```
or FeatherRemote or TriggerRemote or...... all the remotes are smaller then the firefly. Firefly was a great start for all! I think no diy remote would there if soldigeek didn't start with the firefly!

![FeatherRemoteOverview|461x499](upload://vmZw2KuDjgHnrdER7Bo3C1f5Zo9.png)
```

---
## \#1923 Posted by: Deakbannok Posted at: 2018-12-31T01:45:15.195Z Reads: 212

```
@StefanMe @Sascha_stevenson  Yes I am following those. But this one is using old list "Arduino Nano and NRF ". Those origin parts are easy to buy than the adafruit stuffs.... if you live outside the states.
It is not as compact as your adafruit controller. But I am sure this will be useful to some user here that wanted to switch their old part to a new case.
```

---
## \#1924 Posted by: Sascha_stevenson Posted at: 2018-12-31T01:48:35.550Z Reads: 200

```
I live in the UK and it is so much easier to get Adafruit parts than 40 other parts each from somewhere else
```

---
## \#1925 Posted by: kotman333 Posted at: 2019-01-04T21:12:46.786Z Reads: 206

```
how about something like this ? 
https://www.ebay.co.uk/itm/5V-2-1A-Charge-Discharge-boost-Power-Module-3-7V-4-2V-li-ion-18650-LED-battery/142888931306?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m1438.l2649
```

---
## \#1926 Posted by: fabu Posted at: 2019-01-04T21:45:40.808Z Reads: 215

```
Hello @all
I have alread read the whole 1902 posts in this very interesting topic.
First of all a big WOW ;-) really impressive.
A few words to my motivation...I have developed 3 jet surfboards but the big deal is still the remote.
A few years ago the first prototype was controlled by a nunchuck and a teensy 3.1.
All the software / codes have been written down by a friend of mine.
Now I have seen your lovely remote controls - really nice.
And .... a few days later I have build up a working one.
Now the big BUT is coming, when I try to use the receiver to control a stupid PWM ESC it doesn`t work.
By checking with the oszi the are really strange curves...
I have tried everything, starting with solidgeeks data from mid 2017 over solidgeeks data from mid 2018 up to deadbannoks software - with your software it is impossible to get a connection - I am to stupid ;-)
All the same issue - what could it be?

Enclosed I will try to load up data from the nunchuck version and one from the solidgeek....

Bye and thanks in advance
Fabian!
the version of solidgeek:
![esk8|690x371](upload://3TXc6O0THozgFrfkunEeYdONHNl.jpeg) 

and the old nunchuck version:
I will post it in a few seconds....
```

---
## \#1927 Posted by: fabu Posted at: 2019-01-04T21:47:25.063Z Reads: 196

```
![ard8|690x371](upload://p2f7pPJqD8dWtKr0Z64kjENENFN.jpeg)
```

---
## \#1928 Posted by: fabu Posted at: 2019-01-04T22:10:10.561Z Reads: 204

```
okay....I have found the mistake - I have forgotten to solder the pins 5 and 6 :frowning:
3 evenings of searching the mistake - and now 15 seconds of soldering and it is done.
The signal is still a little noisy - any ideas?
![esk8_omg|690x371](upload://dUR80WsMWvMkihi4VNzbZFxjkrC.jpeg)

One more question why is the signal on PIN6 for status LED smoother than on PIN5 for PWM?
```

---
## \#1929 Posted by: StefanMe Posted at: 2019-01-04T22:37:02.702Z Reads: 198

```
Should be the same... both Pins share the same clock. Maybe this is a quality issue from clones? Or a overall issue? 

Is this so important for u? The PWM looks quiet ok for a average receiver. Have I tried another board with different chip for sience? Maybe the ESP32 or SAMD21?
```

---
## \#1930 Posted by: Surfer Posted at: 2019-01-04T23:21:43.179Z Reads: 196

```
A bit of derail, Stefan do you know if your remote will work with the normal receiver of solidgeek, adjusting the address pipe?
```

---
## \#1931 Posted by: StefanMe Posted at: 2019-01-04T23:25:00.259Z Reads: 199

```
No chance... total different transmitter/Frequency. :frowning:
```

---
## \#1932 Posted by: fabu Posted at: 2019-01-07T20:44:44.821Z Reads: 198

```
Hi StefanMe
The problem is the little noisy signal - for the MGM controller it is a little hard to follow a clean ramp up for exapmle.
I will try to improve a little - anyone else there using it with an normal ESC?
```

---
## \#1933 Posted by: whiteflight Posted at: 2019-01-10T15:14:25.324Z Reads: 196

```
I've just started building this cool remote, I've got the arduinos all soldered up and would like to test the communication of the nrfs to see if I did everything right, is there anything I have to do to the default code to get them to recognize each other? or is it just upload the code and turn them on? I've got a pretty basic knowledge of arduino, so could somebody explain how the address thing works? How does the receiver know to talk to my transmitter not another and vice versa?
```

---
## \#1934 Posted by: StefanMe Posted at: 2019-01-10T15:21:25.401Z Reads: 194

```
Take a look to the code... make shure u got the same address ect.

    Defining variables for NRF24 communication
    const uint64_t defaultAddress = 0xE8E8F0F0E1LL;
    const uint8_t defaultChannel = 108;
```

---
## \#1935 Posted by: Migro Posted at: 2019-01-10T15:22:19.758Z Reads: 193

```
Basically it should be plug n play with the code to test. But in the future u should get your own address since this remote has become pretty popular.  And you may run into another person using it with stock address.
```

---
## \#1936 Posted by: whiteflight Posted at: 2019-01-10T15:28:56.995Z Reads: 189

```
I see, so if I were to change the address, what possibilities can I write in for the address and what values can I write for the channel?
```

---
## \#1937 Posted by: StefanMe Posted at: 2019-01-10T15:34:14.372Z Reads: 184

```
for the address 0-F (hex  for example... 0x**92F83A329B**LL ). Keep the channel how it is for now.
```

---
## \#1938 Posted by: StefanMe Posted at: 2019-01-10T15:35:26.057Z Reads: 183

```
There is no option to switch off the regulator... i dont like it.
```

---
## \#1939 Posted by: whiteflight Posted at: 2019-01-10T15:40:50.546Z Reads: 188

```
Awesome, that is super helpful! Thanks!
```

---
## \#1940 Posted by: Sascha_stevenson Posted at: 2019-01-10T20:16:29.031Z Reads: 207

```
@StefanMe @solidgeek  

I'm having trouble uploading the code?!
![22|431x500](upload://dim1Il1QK7rR61pMNtvmZO8gsUT.png)
```

---
## \#1941 Posted by: StefanMe Posted at: 2019-01-10T20:28:00.012Z Reads: 200

```
U have to include libaries... just google for Arduino IDE install libraries.
```

---
## \#1942 Posted by: Sascha_stevenson Posted at: 2019-01-10T20:33:26.540Z Reads: 204

```
@StefanMe is it the VescUart.cpp from RollingGecko i need to install?
```

---
## \#1943 Posted by: StefanMe Posted at: 2019-01-10T21:08:47.544Z Reads: 210

```
some libs...

-u8g2
-nrf24
-vescUart

then it should work :slight_smile: just play around a bit.

SKETCH->include Library->manage library
```

---
## \#1944 Posted by: ervinelin Posted at: 2019-01-11T01:18:40.121Z Reads: 196

```
Anyone knows how to get this to work with ackmanics firmware?
```

---
## \#1945 Posted by: sofu Posted at: 2019-01-11T05:37:31.214Z Reads: 199

```
yes

10char
```

---
## \#1946 Posted by: ervinelin Posted at: 2019-01-11T05:38:33.723Z Reads: 197

```
Hm.. what am I missing? Telemetry works with latest standard VESC but not with ackmanics.
```

---
## \#1947 Posted by: sofu Posted at: 2019-01-11T05:39:34.946Z Reads: 193

```
baud rate? uart enabled? if vesc 6, use vesc 6 library instead?
```

---
## \#1948 Posted by: ervinelin Posted at: 2019-01-11T05:41:23.974Z Reads: 195

```
Let me go check again.... It shouldn't need some other special library right?
```

---
## \#1949 Posted by: sofu Posted at: 2019-01-11T05:42:05.680Z Reads: 187

```
If you've installed the necessary libraries specified in the instructions and it compiles, then you don't need anything else...
```

---
## \#1950 Posted by: ervinelin Posted at: 2019-01-11T05:43:01.753Z Reads: 196

```
Yup.. like I said. Works for regular VESC firmware... Maybe baud rate or something wasn't set up on default... I will go check, thanks!
```

---
## \#1951 Posted by: StefanMe Posted at: 2019-01-11T05:43:28.089Z Reads: 198

```
If u want i can send u the new LIB for UNITY support... :wink:
```

---
## \#1952 Posted by: ervinelin Posted at: 2019-01-11T05:54:12.473Z Reads: 203

```
Haha thanks but I don't have a set of unities yet... Drooling for one... But not yet...
```

---
## \#1953 Posted by: Scream Posted at: 2019-01-11T06:58:10.304Z Reads: 207

```
[quote="StefanMe, post:1951, topic:28543"]
If u want i can send u the new LIB for UNITY support… :wink:
[/quote]

Ooooh yes please! Is it in the thread for your remote?
```

---
## \#1954 Posted by: StefanMe Posted at: 2019-01-11T07:15:07.059Z Reads: 207

```
Yeah i added it in the manual in the UPDATE section... There are all libs.
```

---
## \#1955 Posted by: Arek Posted at: 2019-01-11T23:50:22.191Z Reads: 213

```
Can I use this nrf24l01l module?:
https://i.ebayimg.com/images/g/GxgAAOSw5ZBWKoWV/s-l500.jpg
```

---
## \#1956 Posted by: Sascha_stevenson Posted at: 2019-01-12T00:04:36.448Z Reads: 207

```
Not sure, if you are in the UK I can get you the ones listed in the build for free, u just need to pay for postage I have some that at just collecting dust :wink:
```

---
## \#1957 Posted by: Arek Posted at: 2019-01-12T00:14:12.476Z Reads: 199

```
Thanks for the offer, will think about it.
```

---
## \#1958 Posted by: tardyparty7 Posted at: 2019-01-13T17:32:25.462Z Reads: 205

```
90% sure u can. it looks like the on i used, do u have a link?
```

---
## \#1959 Posted by: Arek Posted at: 2019-01-13T17:36:10.750Z Reads: 214

```
https://www.ebay.co.uk/itm/161867582052
```

---
## \#1961 Posted by: Moment_Films Posted at: 2019-01-16T05:15:20.804Z Reads: 208

```
how can I change the bootup screen on the controller to my own logo or something and could I use a bigger OLED display?
```

---
## \#1962 Posted by: tardyparty7 Posted at: 2019-01-16T05:18:45.586Z Reads: 209

```
yeah u can use ur own logo, change the code.
```

---
## \#1963 Posted by: solidgeek Posted at: 2019-01-16T07:54:41.413Z Reads: 218

```
It is a little complicated but sure you can. You will have to draw your logo in black and white, and generate a XBM type file from the image. Open this file with some test editor and insert/replace this directly in the source code. The XBM format is simple an array of hexadecimals describing the individual pixels

https://en.m.wikipedia.org/wiki/X_BitMap
```

---
## \#1964 Posted by: StefanMe Posted at: 2019-01-16T07:59:08.092Z Reads: 212

```
Much easier and works great.

http://javl.github.io/image2cpp/
```

---
## \#1965 Posted by: fabu Posted at: 2019-01-16T19:18:56.058Z Reads: 221

```
You can also use gimp to create the logo.
Important 1bit (black and white), the right size for example 128x32 pixel and lust but not least save as xbm format.
https://sandhansblog.wordpress.com/2017/04/16/interfacing-displaying-a-custom-graphic-on-an-0-96-i2c-oled/
here it si described really nice :slight_smile:
one question, I have tried to build it up with a teensy 3.1 - the nrf24L01 is not working....has anyone else tried this?
```

---
## \#1966 Posted by: fabu Posted at: 2019-01-22T19:51:51.836Z Reads: 213

```
I have found the solution for the teensy issue.
The **#pragma pack** has to be applied to the code to work together with a teensy...
next step is to apply a 128x128 pixel display - for my eyes ;-)
```

---
## \#1967 Posted by: kotman333 Posted at: 2019-02-04T21:52:13.080Z Reads: 209

```
Anyone can help me please ?
I'm trying to load receiver sketch to Arduino and this what comes out:
,,VescUart" does not name a type. 

should I change anything in the code?
![Bez%C2%A0tytu%C5%82u|690x387](upload://eIkp87gqZpnfjNai3I2AUH3iPCB.png)
```

---
## \#1968 Posted by: StefanMe Posted at: 2019-02-05T04:48:58.442Z Reads: 200

```
U have to install the VESC lib... just search here in the thread
```

---
## \#1969 Posted by: kotman333 Posted at: 2019-02-05T20:46:00.800Z Reads: 197

```
[quote="solidgeek, post:1542, topic:28543"]
found here: [https://github.com/SolidGeek/VescUart ](https://github.com/SolidGeek/VescUart)
[/quote]

had this same problem. try this found here: [https://github.com/SolidGeek/VescUart ](https://github.com/SolidGeek/VescUart)
```

---
## \#1970 Posted by: kotman333 Posted at: 2019-02-05T20:46:38.824Z Reads: 189

```
fixed it than you!
```

---
## \#1971 Posted by: swimmydude Posted at: 2019-02-09T00:37:28.509Z Reads: 203

```
So I been working on this for a while now and finishing this remote is what is bottle-necking me from completing my build. I can't figure out the problem. I even made a prototype remote on a breadboard with extra parts I got. Still couldn't get it running. I've checked the connection and wiring multiple times. While the soldering and such is not amazing, it is satisfactory enough for a first build. I've used my multimeter to see if the connections were working and they were. While I can't say with 100% certainty that none of the pieces are defective, I believe they all work. Which leads me to believe it is something with the coding or how I approached the Arduino factor. I do have experience with Arduino, I'm technically only a novice since I've only messed around with it for several school projects. Software isn't my strong suit and even doing some of the leg work for this project was a bit confusing, even though it shouldn't have been for me. 

My actual remote will turn on and go to the Firefly logo screen but then nothing more. I can go to the settings and tinker with the settings. I can even go to the settings from startup, then exit the setting using the last option and go to the normal UI. I can't do anything there though and I get no readings. I can't connect to the receiver either. On my prototype, I can't even get the nano or the screen to light up. Only the 5v converter lights up. So the problem on the prototype may just be a completely different problem. Any ideas on what my issue may be?

Here's a couple of my prototype. I can post pictures of the actual remote, but not sure how much that would help.
![PrototypeRemote|666x500](upload://rM5IR2H88PsD5PmQjy1qdCiVbvt.jpeg) 
![PrototypeRemote2|375x500](upload://dgoBBvIU59kO6gV7BkChFzzk99T.jpeg)
```

---
## \#1972 Posted by: solidgeek Posted at: 2019-02-09T01:41:12.105Z Reads: 194

```
Sorry to hear that you cannoy get it working. Which version of the software are you using? If you are using the newest version of the development branch the software should work just fine. To me it sounds like some error with the nRF24 module, as you describe that the remotes crashes when the nRF24 tries to transmit. Please double check that the nRF24 is connected correctly. Have you tried enabling debugging by uncommenting the #DEFINE debug?
```

---
## \#1973 Posted by: swimmydude Posted at: 2019-02-09T23:09:59.552Z Reads: 193

```
It's okay, I still love the remote and refuse to try another one right now because I simply just want this design. So part of that is on me. I should be using the latest version. I simply downloaded the most recent one and went from there. 

You stating that you think it's the nRF24 module at least gives me something to work with, so I will try to go from there. I've already isolated the module with aluminum foil, but that only solves the problem if the problem is not transmitting well. I doubt it is even doing that. I'll double check all the connections once again. I am also going to try the debugging. I honestly did not know what that was until now, even though I saw things here and there while going through this topic.
```

---
## \#1974 Posted by: solidgeek Posted at: 2019-02-09T23:31:06.069Z Reads: 195

```
Let me know the output og the Serial monitor after enabling debugging. Also make sure you isolate the nRF24 module and the aluminium foil with some plastic or paper inbetween such that you dont short anything (aluminium is conducting)
Just making sure, this is the version you are using?: 
https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development
```

---
## \#1975 Posted by: swimmydude Posted at: 2019-02-09T23:54:02.719Z Reads: 199

```
Yep, that's the one I used. Now I did everything manually and didn't just download the zip file from that page. Should I have? This was before I realized I could because I haven't really messed much with GitHub. 

I do have the module wrapped with kapton tape then wrapped with aluminium, but not covering the ceramic antenna. But I may have found the problem. It seems I have switched the wire up for CS->D10 and CE->D9. What I don't understand is how I didn't catch that before because I traced every wire and should have already checked this. -_-
Lol, well now I can start working on it. Going to take a minute since after I soldered everything and apparently "double checked," I covered the connections with silicone.
This may be the issue because I couldn't even get a reading with the serial monitor using the debug.
```

---
## \#1976 Posted by: swimmydude Posted at: 2019-02-10T03:13:22.635Z Reads: 188

```
I got it working. It loads and goes to the normal screen and I see stuff happening. I couldn't get the serial monitor to show any outputs, on the 115xxx baud rate. I don't remember the number but I know that is the one you said you used. Now I still couldn't get the remote to make the wheels move or actually connect to the receiver. But I'll be working on that now. Thanks for the help thus far @solidgeek, it's been helpful to get me going again.
```

---
## \#1977 Posted by: solidgeek Posted at: 2019-02-10T19:53:01.041Z Reads: 195

```
@swimmydude Glad to hear you got it working. To read anything on the serial monitor from the remote you have to use 9600 baud, as this is used for debugging - a baud of 115200 is used for the receiver debug and VESC UART communication :slight_smile:  (actually this should maybe be the same in the future)... Now regarding the connection between remote and receiver, if the nrf24 module is connected corretly and code is uploaded it should work right out of the box.  The most common problem regarding receiver is bad power supply, and can often be fixed by adding a big electrolytic capacitor (220uF-470uF) on the 5V input rail.
```

---
## \#1978 Posted by: SynteX Posted at: 2019-02-24T19:30:44.567Z Reads: 187

```
A friend of my has a little issue. When he clears the EPROM the firefly connects with the receiver. But only the first time. If the turns them off and on again they won't bind. Only after clearing EPROM again. This is impossible to work with ofcours :stuck_out_tongue:
```

---
## \#1979 Posted by: solidgeek Posted at: 2019-02-24T21:48:50.667Z Reads: 189

```
How does he clear the EPROM? :-)
```

---
## \#1980 Posted by: Parafodas Posted at: 2019-02-25T00:55:54.661Z Reads: 185

```
(Oldbotlouder)
```

---
## \#1981 Posted by: ervinelin Posted at: 2019-02-25T01:48:35.024Z Reads: 195

```
Does anyone know what's the correct way to create a new pipe address?

I had a remote which would connect to the receiver and the throttle works but no telemetry.

After troubleshooting it. It turns out there was something wrong with the pipe. Adjusted it and suddenly both throttle and telemetry work. Nothing else was changed.

Any ideas?
```

---
## \#1982 Posted by: SynteX Posted at: 2019-02-25T06:38:52.133Z Reads: 186

```
Using the default sketch in arduino studio.
```

---
## \#1983 Posted by: solidgeek Posted at: 2019-02-25T07:42:24.604Z Reads: 186

```
That does not clear the EEPROM it only reflashes the firmware. You can try uploading this sketch: https://www.arduino.cc/en/Tutorial/EEPROMClear
```

---
## \#1984 Posted by: ervinelin Posted at: 2019-02-27T06:51:16.699Z Reads: 185

```
Anyone knows if the telemetry works with the new VESCtool just recently released?
```

---
## \#1985 Posted by: TSJ Posted at: 2019-02-27T18:50:08.006Z Reads: 189

```
I am planning to start building one of these remotes and have a couple of questions.  I am in the US and have not found an Arduino nano with 3.3V regulator.  Any US source for this?  If not, I see that a few people have used the Pro Mini and I was wondering if this works with the current code and wiring, or if there are any modifications that need to be done.  Also, is the development branch of the code still the one to use?  Thanks for your help.
```

---
## \#1986 Posted by: solidgeek Posted at: 2019-02-27T23:32:29.292Z Reads: 192

```
@ervinelin Have not tried it out, didnt know about the new update. Any changes? 

@TSJ Well the Nano I recommend is just nice because it fixes many power related issues. If you makes sure that the nrf24 module is well supplied and you filter the supply voltage from VESC then any Arduino should work 😊
```

---
## \#1987 Posted by: ervinelin Posted at: 2019-02-28T02:43:12.102Z Reads: 186

```
Seems like lots of changes actually... That's why I was considering upgrading...
```

---
## \#1988 Posted by: swimmydude Posted at: 2019-03-02T20:28:50.507Z Reads: 199

```
I should have completed my build before February. But I been busy and putting this off, but I'm determined to stop procrastinating. -_-

Anyway I discovered my capacitors were wired to gnd and 5v pins, opposed to gnd and rst pins. So I got that fixed but still no dice. I will mess around with the capacitance. See if that will solve it. Meanwhile I'm gonna mess around with settings and stuff too. I've noticed that since the last update or so, the settings changed a bit. It's a bit more streamlined, but the options are now numbers rather than stating what the options are. I can't seem to find a guide or a list anywhere that states what each number means. Like what are option 1, 2, and 3 mean for the trigger setting. I can only assume option 0 for battery is Li-Ion and 1 is lipo? Maybe it's somewhere obvious, but I can't find it.

I also did serial monitor for the remote and it just kept stating failed transmission. I did it with and without the receiver being on/connected. It did seem to be giving accurate readings of the throttle though. Gave me numbers ~100-700 or so. I'm going to guess that it's still a problem with the remote rather than the receiver due to these results?
```

---
## \#1989 Posted by: Surfer Posted at: 2019-03-02T20:53:31.979Z Reads: 191

```
Hi I'm curious if you have plans to upgrade the firmware to work with nrf 51, it seem like Benjamin did a nice work on the last firmware update, short history, now is no needed receiver anymore, we can use a external nrf51 to connect the remote and the phone app, all trough UART. I know you tried before but it was not a lot of documention.
http://www.trampaboards.com/vesc-connect-nrf-wireless-dongle-p-25516.html
```

---
## \#1990 Posted by: krazor Posted at: 2019-03-06T07:40:37.872Z Reads: 181

```
im interested in building my own remote since im a programmer. funny enough i have my own 3D printer so i would love to venture on and tackle a project like this myself. if you dont mind me asking where you started. i was thinking about using arduino to build the transmitter and reciever but my biggest question is what libraries did you use and where did you find the appropriate info to cover for the variety of available vescs. wouldn't each vesc supply its own data?
```

---
## \#1991 Posted by: solidgeek Posted at: 2019-03-06T19:39:16.761Z Reads: 188

```
@Surfer Well that is quite interesting, however I do not have any nrf51 laying around and I do not have the income to try it out. The interesting part is that you can replace the Arduino Nano and nrf24 with an nrf51 as it includes a microprocessor (actually programmable from Arduino IDE)... I smell much more features and faster / bigger displays :wink: 

@krazor Well I began with an Arduino and a PPM signal to a speed controller. I have since developed it a little further, with a library made to communicate with a VESC over UART. As long as the VESC is updated, each VESC has the same communication protocol. If you are interested you can check out my github for the source code :)
```

---
## \#1992 Posted by: krazor Posted at: 2019-03-06T23:26:01.178Z Reads: 181

```
thanks, i would love to make one for myself =)
```

---
## \#1993 Posted by: krazor Posted at: 2019-03-10T02:14:18.032Z Reads: 185

```
i was looking over your github but the tutorial section doenst seem to be finished. is there an update coming along. i dont want to go ordering parts and start the printing process if the documentation is unfinished.
```

---
## \#1994 Posted by: ervinelin Posted at: 2019-03-10T04:17:20.831Z Reads: 185

```
I shall answer my own question... Yes it works with the new vesctool.
```

---
## \#1995 Posted by: solidgeek Posted at: 2019-03-10T10:00:13.607Z Reads: 188

```
This should help you: https://solidgeek.dk/docs/firefly-remote/getting-started/
```

---
## \#1996 Posted by: chickengun Posted at: 2019-03-10T15:03:13.265Z Reads: 183

```
@solidgeek
I would like to add an option to activate/deactivate a led strip with your remote. I was thinking of having another option in the settings menu to set a GPIO pin on the receiver arduino board either to HIGH or LOW. I would use a moset and +42V from the battery pack to power on the led strip.
Can you tell me which adjustments to make at the transmitter.ino/receiver.ino file (development branch)? That would be awesome.
```

---
## \#1997 Posted by: solidgeek Posted at: 2019-03-10T15:32:47.256Z Reads: 190

```
If you aren't familiar with mosfet I would use a small relay instead, as HIGH voltage switching MOSFETs can be difficult and dangerous for your electronics if you do something wrong. Regarding the software, it can be done in multiple ways, and I cannot tell you all the things you need to do - you will have to figure that out yourself :)
```

---
## \#1998 Posted by: krazor Posted at: 2019-03-11T07:26:41.500Z Reads: 176

```
thanks for the link, for some reason i couldnt find this on the github page.
```

---
## \#1999 Posted by: krazor Posted at: 2019-03-12T08:00:10.538Z Reads: 176

```
is there a custom PCB designed for this project yet?
```

---
## \#2000 Posted by: hanyelkomy Posted at: 2019-03-14T16:45:54.416Z Reads: 177

```
Hi there, did u manage to sort out the no real data on the remote, i am also not able to get any data like speed, range and battery!!!
```

---
## \#2001 Posted by: hanyelkomy Posted at: 2019-03-14T16:55:26.935Z Reads: 191

```
Hi, thanks for your awesome remote, but i have an issue with real data as its not shown on the remote, i am using flipsky dual 6.6 controller and have followed all your instruction but no real date. Another thing it will be really great if u can some how add speed control in the remote code, like slow, med and fast... is that possible ?

edit: i am using the latest dev code
```

---
## \#2002 Posted by: legend27 Posted at: 2019-03-17T15:35:41.892Z Reads: 189

```
SOLVED: You have to hold the dead man switch down... lol

Hey everyone!

So as im putting the remote together and testing the hall sensor, I noticed that the battery bar is moving instead of the throttle bar. Does anyone know how to fix it?

https://www.youtube.com/watch?v=NMr9FM0bOaQ
```

---
## \#2003 Posted by: Migro Posted at: 2019-03-18T14:27:18.060Z Reads: 179

```
I would assume that you wired something wrong :slight_smile:
Like A2 and A3 switched or something
```

---
## \#2004 Posted by: legend27 Posted at: 2019-03-18T14:58:31.835Z Reads: 178

```
[quote="legend27, post:2002, topic:28543"]
SOLVED: You have to hold the dead man switch down… lol
[/quote]

:no_mouth:
```

---
## \#2005 Posted by: Migro Posted at: 2019-03-18T15:15:34.206Z Reads: 174

```
Was the wiring wrong?
```

---
## \#2006 Posted by: legend27 Posted at: 2019-03-18T16:35:26.731Z Reads: 174

```
No. You just had to hold down the dead man switch
```

---
## \#2007 Posted by: Migro Posted at: 2019-03-18T16:40:56.901Z Reads: 169

```
ohh i see. But how come you could control the battery then?
```

---
## \#2008 Posted by: legend27 Posted at: 2019-03-18T16:43:15.389Z Reads: 170

```
The battery wasn't connected. It got power from my computer via usb.

Connected the battery and now everything is working like it should.
```

---
## \#2009 Posted by: Migro Posted at: 2019-03-18T16:46:40.401Z Reads: 170

```
Ahh okay :+1:
```

---
## \#2010 Posted by: TSJ Posted at: 2019-03-19T19:16:13.243Z Reads: 171

```
I think I have seen this in a previous post, but finding stuff is a little overwhelming sometimes, Does this board effectively replace the battery charge board and boost board in the design?  Has anyone used something similar?

[Onyehn 5Pcs 5V Boost Step Up Power Supply Module Lithium Battery Charge Protection Board 134N3P DIY Charger LED Display USB and Micro Port 5 Pack](https://www.amazon.com/gp/product/B07D3SQYKJ/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)

![image|242x353](upload://c8ATAbC6hjIZfoGFK9Q4GLSIv49.jpeg)
```

---
## \#2011 Posted by: solidgeek Posted at: 2019-03-19T20:35:55.899Z Reads: 174

```
Yeah it should work, however I have not tried it myself. The only thing that I dont like is that the 5V regulator is always on (draining the battery), unless you cut the battery power directly, making it impossible to charge unless the remote is turned on.

I have seen some new charging boards lately that is a lot smaller than the old I used. https://www.seeedstudio.io/Li-Po-Battery-Charger-p-2656.html
```

---
## \#2012 Posted by: Deakbannok Posted at: 2019-03-19T23:27:32.341Z Reads: 172

```
@solidgeek and to all.
Arduino nano intrgated with rf24. :slight_smile:
will make this more compact and easier to work with.


 https://s.click.aliexpress.com/e/K7yU42H
```

---
## \#2013 Posted by: Reills Posted at: 2019-03-20T01:18:02.652Z Reads: 169

```
Im looking at building this project for a school project! I was just wondering if there is any turuorials or help for actually connecting the remote to the board i cant seem to find any. And is there anyone selling this remote ?

Cheers
```

---
## \#2014 Posted by: KranzeKake Posted at: 2019-03-20T08:22:51.418Z Reads: 165

```
@Zyb is selling the remote:)
```

---
## \#2015 Posted by: sami Posted at: 2019-03-20T14:30:33.009Z Reads: 165

```
will I need to change something in the code for it to work?
```

---
## \#2016 Posted by: TSJ Posted at: 2019-03-20T16:16:44.808Z Reads: 162

```
Thanks @solidgeek for the design and help and @SeeTheBridges for the awesome videos.  I have built the electronics and printed the parts and am hopefully in the final stages of assembling.  I have a few of questions:
How do you afix the hall sensor, hot glue?  It does not seem to hold with the recess in the 3D print.
For a unique address, from what I have read, I need to change the existing in both the remote and receiver and I need to clear the eprom before uploading the new code? Are there any restrictions on the address, or can I just change a few of the digits? 
For the kill switch, is the spring force provided by the limit switch?  It seems to stick sometimes, but I may just need to clean up my print a little more.  Has anyone added an lubricant to the parts to make it smoother?
```

---
## \#2017 Posted by: StefanMe Posted at: 2019-03-20T16:32:22.863Z Reads: 170

```
I added some bearings... smooth as hell 

But I have to modifie the prints...

https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084
```

---
## \#2018 Posted by: Deakbannok Posted at: 2019-03-20T22:35:15.321Z Reads: 171

```
I am not sure. I havent get a hand on it yet.
```

---
## \#2019 Posted by: Deakbannok Posted at: 2019-03-21T10:43:21.996Z Reads: 181

```
 this was i have been working on before. a new printed controller. when I get back home i will order that new arduino nano with integrated with rf24.![IMG_20190321_124543|375x500](upload://nCnEhQ7vQfzSPRqcpRdm96wVvPW.jpeg)
```

---
## \#2020 Posted by: captclearleft Posted at: 2019-03-21T12:16:14.696Z Reads: 175

```
Hey @hanyelkomy, 
Did you get a response on your question about:

>   ...flipsky dual 6.6 controller and have followed all your instruction but no real date. Another thing it will be really great if u can some how add speed control in the remote code, like slow, med and fast… is that possible ?

I am interested in trying the flipsky dual 6.6 but was not sure if there were communicability issues with the firefly remote.
Thanks
```

---
## \#2021 Posted by: sami Posted at: 2019-03-21T13:34:52.595Z Reads: 170

```
Let me know how it goes. I really like the bottom design... If I could fit the Same remote inside that design that would be great
```

---
## \#2022 Posted by: auveele Posted at: 2019-03-21T17:01:54.806Z Reads: 172

```
I'm remodeling the remote to change somethings and add some buttons (lights and turnlights) and maybe cruise control. I'm doing it in Solidworks.

I haven't finished it yet, but i'm in it :slight_smile:

What software are you using for modeling?
```

---
## \#2023 Posted by: Deakbannok Posted at: 2019-03-21T17:08:50.627Z Reads: 177

```
no the bottom one is not my design. this is from Nano adafruit controller. The middle one is mine
```

---
## \#2024 Posted by: Deakbannok Posted at: 2019-03-21T17:09:38.467Z Reads: 179

```
Fusion 360
```

---
## \#2025 Posted by: wafflejock Posted at: 2019-03-26T14:36:06.469Z Reads: 178

```
Fantastic I was thinking of doing this myself but nice if I can just buy it somewhere :) . Have my own trigger version here I just updated too if anyone prefers triggers https://www.thingiverse.com/thing:1864536 I like it for riding with light gloves in the fall/winter but have to admit I still haven't tried a wheel remote.  I'll probably grab one of those boards and update my code/design to work around it too thanks for sharing!
```

---
## \#2026 Posted by: frekk1 Posted at: 2019-03-28T20:29:52.535Z Reads: 190

```
![11|690x372](upload://lxCgcHLwxs7vTdMcwio8G1UNrrI.png) ![43|690x381](upload://qDyw8nlCphhvt8hrcPNBxLF8wgZ.png) 
What am I doing wrong?
I had no problem uploading the software for the transmitter.
But when I try to upload the receiver I get: VescUart does not name a type.
I include VescUartControl from RollingGecko in the script.
Is it something Im missing? I am new to this Arduino:sweat::sweat::sweat:
Hope someone can help me. I am very eager to make it work
Thanks
```

---
## \#2027 Posted by: Michaelj1 Posted at: 2019-03-29T04:05:07.122Z Reads: 174

```
hey guys, so I'm trying to build this remote with the bigger display mod, is there any code I need to change to accommodate for that and if so what? if anyone has code or just tips for the 128x64 OLED display it would be greatly appreciated!
```

---
## \#2028 Posted by: solidgeek Posted at: 2019-03-29T06:05:38.755Z Reads: 178

```
Maybe you have installed wrong library? Download my VescUart library om github, https://github.com/SolidGeek/VescUart/tree/development and delete any other
```

---
## \#2029 Posted by: StefanMe Posted at: 2019-03-29T07:49:19.026Z Reads: 185

```
There are several codes out with a bigger screen but different boards. The nano is just not that powerfull to run the code on a bigger screen with additional features.

https://www.electric-skateboard.builders/t/featherremote-and-smartremote-files-in-post-577/74084

or 

https://www.electric-skateboard.builders/t/firefly-nano-remote/72916

for example
```

---
## \#2030 Posted by: Michaelj1 Posted at: 2019-03-29T12:04:40.296Z Reads: 180

```
Shoot, I wish I would’ve known that before I ordered the parts, oh well haha
```

---
## \#2031 Posted by: Deakbannok Posted at: 2019-03-29T20:53:13.858Z Reads: 189

```
If you are looking to build a simple controller, with arduino is fine, cheap to replace and cost less for parts. But to run a bigger OLED are a few futuristic options are required more memo. which arduino is limited. I also have adafruit on hands. With a small 182x32 screen is enough room for indicators FETs temp and Voltage, Speed, Distance. 
https://www.instagram.com/p/Bt0Su2LgMOW/?utm_source=ig_web_button_share_sheet
```

---
## \#2032 Posted by: StefanMe Posted at: 2019-03-29T21:07:53.014Z Reads: 181

```
What has the picture to do with the remote? Fishing for compliments?
```

---
## \#2033 Posted by: solidgeek Posted at: 2019-03-29T22:26:55.255Z Reads: 183

```
For a bigger screen you just need a more powerfull microcontroller. I just received a SAMD21 M0-Mini (Arduino compatible 32-bit microcontroller) through the mail, and if everything compiles/works reliable it would be a neat replacement for the nano as it has almost the same form-factor.
```

---
## \#2034 Posted by: Deakbannok Posted at: 2019-03-30T18:00:54.002Z Reads: 182

```
Comes with 256k is not bad to punch more code. :) 
Having a cruise control + kick cruise mode, limit ERMP.
```

---
## \#2035 Posted by: StefanMe Posted at: 2019-03-30T19:03:46.359Z Reads: 188

```
The main thing is to replace the eeprom with the flash storage. Check my code from the FeatherRemote to see how it works. 

The rest works quite plug and play...
```

---
## \#2036 Posted by: chickengun Posted at: 2019-03-30T23:47:05.134Z Reads: 188

```
Quick question for receiver wiring in conbination with vanda vesc 4: Is it correct that I just need the RX and TX pins for communication (5V and GND not needed)? On this picture I drew how I would do the wiring. PPM signal in red, green and purple. RX and TX in black.

![image|690x259](upload://vxlTrpOvB5KZ7n9BYChq175QMjt.jpeg)
```

---
## \#2037 Posted by: StefanMe Posted at: 2019-03-30T23:51:32.331Z Reads: 187

```
Yes. U can use the 5v and ground from the PPM or the UART port. Doesn’t matter. Is the same regulator.
```

---
## \#2038 Posted by: Deakbannok Posted at: 2019-03-31T00:02:17.630Z Reads: 191

```
Yes, or u can just use a ppm pin and connect other power pins to UART pins. that is my preference to keep organizing all the wires ![51089071_1253315748149449_2354312273494802432_n|669x499](upload://m07UsltKd0RcpKrciD3k5YaxHnw.jpeg)
```

---
## \#2039 Posted by: frekk1 Posted at: 2019-04-03T16:42:21.236Z Reads: 179

```
Thanks solidgeek. Now I was able to install the reciver. And it bind to the remote without any problem.
Thanks for a fantastic remote. Keep ut the good work 👍
```

---
## \#2040 Posted by: niel5046 Posted at: 2019-04-07T18:08:46.426Z Reads: 173

```
Can someone help me? I just ordered the all the stuff i need to build this remote. But how do I connect the receiver to the ECS?
```

---
## \#2041 Posted by: StefanMe Posted at: 2019-04-07T18:41:02.175Z Reads: 177

```
    PLUS - PLUS
    MINUS - MINUS
    TX - RX
    RX - TX
    PPM - PPM

10 char
```

---
## \#2042 Posted by: niel5046 Posted at: 2019-04-07T18:57:40.576Z Reads: 169

```
Then i kind of have a problem i can only find a GND, W, V, U, 5V

I have this esc https://www.ebay.com/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute/302812941839?hash=item46810ece0f:m:mEjYlp9id5UtRAwhPmlchiw
```

---
## \#2043 Posted by: Mich21050 Posted at: 2019-04-07T19:51:12.177Z Reads: 164

```
This esc won't work. It's proprietary. This remote is only compatible with vesc's.
```

---
## \#2044 Posted by: niel5046 Posted at: 2019-04-08T04:21:12.832Z Reads: 163

```
What kind of vesc, is the best for this remote ?


Or can i use this one https://www.aliexpress.com/item/Maytech-Dual-VESC-based-controller-electric-skateboard-longboard-dual-ESC-based-on-VESC-vedder-Pcb-BLDC/32948876329.html
```

---
## \#2045 Posted by: StefanMe Posted at: 2019-04-08T08:09:27.599Z Reads: 168

```
Then the FIREFLY REMOTE makes no sensor for u. The Remote is specially made to receive specified data from the ESC (VESC compatible). 

[quote="niel5046, post:2044, topic:28543"]
for this remote ?
[/quote]

Dont choose the VESC for your remote... choose the VESC for your board/motors....

Any VESC based ESC will work.

@Mich21050
It will work... but not live data. Thats what i told him in the post before... EDIT: Lol the post is missing... strange. Sorry
```

---
## \#2046 Posted by: niel5046 Posted at: 2019-04-08T08:32:34.062Z Reads: 165

```
Now, this is starting to confuse me. I have this ESC https://www.ebay.com/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute/302812941839?hash=item46810ece0f:m:mEjYlp9id5UtRAwhPmlchiw the belt one 

But I can only find GND, W, V, U, 5V on the ESC. and what do you mean with live data, like I cant see how fast i am going??

Btw this is my second board i am building. But first controller :)
```

---
## \#2047 Posted by: Mich21050 Posted at: 2019-04-08T08:34:45.888Z Reads: 158

```
How? As far as I know this esc hasn't got a pwm (ppm) input. @niel5046 you won't get live data, like speed and so on.
```

---
## \#2048 Posted by: niel5046 Posted at: 2019-04-08T08:39:11.502Z Reads: 157

```
Okay. My build is 2 belt motors. And what kind of vesc, do i need to buy to get live data :)
```

---
## \#2049 Posted by: Mich21050 Posted at: 2019-04-08T08:40:24.200Z Reads: 152

```
It doesn't matter. Your esc just needs to be vesc based.
```

---
## \#2050 Posted by: niel5046 Posted at: 2019-04-08T08:47:25.633Z Reads: 164

```
Okay now i understand. I am just gonna buy this one https://www.aliexpress.com/item/Maytech-Dual-VESC-based-controller-electric-skateboard-longboard-dual-ESC-based-on-VESC-vedder-Pcb-BLDC/32948876329.html?spm=2114.search0104.3.84.4e7a7ac9HsTVcN&amp;ws_ab_test=searchweb0_0,searchweb201602_6_10065_10068_319_10059_10884_317_10887_10696_321_322_10084_453_10083_454_10103_10618_10304_10307_10820_10821_537_10302_536,searchweb201603_70,ppcSwitch_0&amp;algo_expid=7bb6c018-0fcd-4e51-b0b6-9e859e360fd1-13&amp;algo_pvid=7bb6c018-0fcd-4e51-b0b6-9e859e360fd1 when i get the datasheet. :smile:
```

---
## \#2051 Posted by: Mich21050 Posted at: 2019-04-08T08:50:14.940Z Reads: 157

```
This one would work but it's not really reliable.
```

---
## \#2052 Posted by: niel5046 Posted at: 2019-04-08T09:03:23.030Z Reads: 161

```
How do you know its not really reliable ?
```

---
## \#2053 Posted by: Winkelmann Posted at: 2019-04-08T18:01:25.969Z Reads: 165

```
what do you guys think of my project so far?
Its a work in progress that i hope can get even better with all of your thoughts 

https://www.electric-skateboard.builders/t/project-board-better-than-boosted/89825?u=winkelmann
```

---
## \#2054 Posted by: niel5046 Posted at: 2019-04-10T18:58:21.628Z Reads: 154

```
?
[quote="Mich21050, post:2051, topic:28543, full:true"]
This one would work but it’s not really reliable
[/quote]


How do you know that it's not reliable
```

---
## \#2055 Posted by: Surfer Posted at: 2019-04-10T19:24:07.957Z Reads: 154

```
Maytech vesc is know to cheap out in essential components, most probably will not run on FOC
```

---
## \#2056 Posted by: captclearleft Posted at: 2019-04-11T04:21:22.139Z Reads: 167

```
I am sure it has been asked an answered, but I cant seem to find it in the thread - 
After building the remote.  Is the throttle bar supposed to deflect to fill the entire bar (for throttle and brake)?  If so, how do I calibrate that.?  ![ffremote1|375x500](upload://emV3RVIamKW2yiTfyMoq3S5ITCx.jpeg) 

How do I get into the settings (holding the throttle full without the trigger does not work)?

Is there a wiki where we can start adding all the answers we find? 

Thanks
```

---
## \#2057 Posted by: StefanMe Posted at: 2019-04-11T05:20:02.340Z Reads: 158

```
Jodel trigger kn start up the remote.

U ll find some settings to calibrate the throttle.
```

---
## \#2058 Posted by: Mitkah Posted at: 2019-04-11T08:06:50.988Z Reads: 159

```
Short question which spring is recommended? Which springdimensions do you use
```

---
## \#2059 Posted by: StefanMe Posted at: 2019-04-11T08:23:37.654Z Reads: 156

```
15mm x 0.4mm is best (0.4-0.6 depends on how strong u want the feedback)
```

---
## \#2060 Posted by: Mitkah Posted at: 2019-04-11T09:24:47.458Z Reads: 153

```
But in the Google list stands 20mm
```

---
## \#2061 Posted by: StefanMe Posted at: 2019-04-11T09:58:08.196Z Reads: 163

```
[quote="Mitkah, post:2060, topic:28543"]
t stands 20mm
[/quote]

Yeah, for me is 15 mm better...  go for both. just a few cents.
```

---
## \#2062 Posted by: captclearleft Posted at: 2019-04-11T16:38:19.676Z Reads: 179

```
Thanks @StefanMe ...  That helped.  
How do I get into the settings menu on firefly remote?  Hold trigger while powering on remote.

For those in my situation: throttle does not reach Max - I opened up the remote.  
And noticed that the spring was preventing the throttle movement to go max either direction.  ![IMG_20190411_090228008%20-%20Copy|666x500](upload://orhr4L8nqiCK5vdu3vmhdmVuZ7v.jpeg) 

So I filed down lever that the spring attaches to.  Then re-bent spring to make more clearance.  I also filed the remote housing a little to allow the throttle wheel to move a little more forward and a little more back (just a tiny bit).  

Then I opened up the code. Uncomment 
#define DEBUG

Then added this right after throttle variable is populated

  #ifdef DEBUG

  Serial.println(throttle);

  #endif

Then plugged in the remote to the computer and opened up serial monitor.  Then watch the serial output while moving the throttle.  Then I filed down the previously mentioned pieces till I got 1000 on full throttle, and 0 on Full Brake.  

![ffremote_file_1|666x500](upload://tW8EC9P73QhzI1FFf3yOEQwUI4X.jpeg) 

tags:
throttle does not reach max, how do i enter the settings menu, firefly remote settings
```

---
## \#2063 Posted by: StefanMe Posted at: 2019-04-11T16:40:11.971Z Reads: 167

```
hmm no u don't have to.. just go into settings where u can calibrate the min, max and center value for the hall sensor...

Hold the trigger on startup until the menu appears to join the settings menu
```

---
## \#2064 Posted by: robthebuilder Posted at: 2019-04-11T19:52:18.932Z Reads: 167

```
Damn I wanna build this.. But import taxes in Sweden is about $10 per part if I buy them from different sites. :disappointed_relieved:

Does anyone know if I can buy them all in one place and have it sent in the same package? At least as few packages as possible.. Thanks :slight_smile:
```

---
## \#2065 Posted by: niel5046 Posted at: 2019-04-11T20:25:58.362Z Reads: 163

```
Are you sure about that, because we don't have that in Denmark? We only get in an import taxes if one package comes over 14 dollars then we get taxes and moms.

But If you want it I can buy it for you and send it to you?
```

---
## \#2066 Posted by: robthebuilder Posted at: 2019-04-12T05:49:53.605Z Reads: 166

```
Yup, Sweden has changed the import-laws as of last year so it's quite horrible now.. That is really nice of you! :smiley:

I just read the rules again and if I order from within the EU, the shipper is responsible for including the taxes in my total so, It might be alright if I find something inside the EU. But everything is so much more expensive here then in China for example :P 

Do you guys know any good electronics sellers in the EU?
```

---
## \#2067 Posted by: niel5046 Posted at: 2019-04-12T12:35:32.007Z Reads: 163

```
You can try hoppy king or Amazon.de
```

---
## \#2068 Posted by: solidgeek Posted at: 2019-04-12T15:23:54.391Z Reads: 162

```
I got some spare parts I can send you if you would like, I got everything (electronics, springs etc.) however I am not sure if postnord will allow me to ship the battery, so maybe you will have to source that yourself 👍 Send me a PM if you still need parts
```

---
## \#2069 Posted by: robthebuilder Posted at: 2019-04-12T15:47:34.463Z Reads: 165

```
That would be awesome! I'll send you a PM :smiley:
```

---
## \#2070 Posted by: captclearleft Posted at: 2019-04-15T16:05:50.174Z Reads: 174

```
Hello, 
Just need a little clarification. Thanks in advance. :slight_smile:

What is the current  - VescUartControl Library (VESC 4.12/latest firmware).  ???
I am using the VescUartControl-new from this link:
https://solidgeek.dk/docs/firefly-remote/software/

I get the error (while uploading to the receiver) (NANO v3):
'SERIALIO' was not declared in this scope.  

After reading the VescUart.h and some of the threads.  I deduced that I must add these lines to the receiver code????



    #define SERIALIO Serial  //  Originally not in receiver code NEW!

    void setup() {
      SetSerialPort(&SERIALIO);  //  Originally not in receiver code NEW!
      SERIALIO.begin(115200);



Is this correct???

The github wiki refers to using this library:
https://github.com/RollingGecko/VescUartControl

Then there is a VESC6 library...  Can someone confirm which is the most current library, and am I correctly handling the 'SERIALIO' was not declared in this scope ERROR???
Thanks so much.
```

---
## \#2071 Posted by: solidgeek Posted at: 2019-04-15T21:49:26.849Z Reads: 166

```
You should use my updated version of the library if you use newest version of the remote.

https://github.com/SolidGeek/VescUart
```

---
## \#2072 Posted by: ABSKnut Posted at: 2019-04-15T22:09:49.212Z Reads: 162

```
Is the remote model the same exact size as a boosted remote? Basically, will it fit in the new flatland 3d rubber cover for boosted?
```

---
## \#2073 Posted by: captclearleft Posted at: 2019-04-15T22:33:25.092Z Reads: 158

```
Thank You!! That worked.  I am now getting consistent connection, and telemetry.  Awesome.
```

---
## \#2074 Posted by: adrianlee Posted at: 2019-04-16T15:25:26.224Z Reads: 171

```
Just updated remote to latest version as with vesc fw 3.52 it was not showing telemetry data anymore. While I got the data now to remote, ppm control vanished! 

The remote and receiver both works, I even measured speedPin output from receiver and it was showing correct voltage changes to throttle. In Vesc tool I can control motor with arrows, so vesc and motor is working, but ppm data is not showing there also. I tried resetting "app to use" setting to Off and back to PPM and UART again , rebooting between, but no success. 

Any ideas how to fix or what happened?

updates:
* I tested also voltage from ppm pin from vesc and it shows correct values
* the vesc is a focbox 4.12

I reflashed firmware on vesc and got it working now. The input still seems a bit unstable, like if you accelerate or brake fast the value stops halfway to max. Could this be power issues? I have recommended power filtering but maybe its damaged
```

---
## \#2075 Posted by: solidgeek Posted at: 2019-04-16T18:39:33.405Z Reads: 163

```
Which version of the remote do you use? It sounds to me like you use the analogWrite function indstead of the Servo.write. Have you used the Vesc tool to calibrate your min and more PPM values?
```

---
## \#2076 Posted by: adrianlee Posted at: 2019-04-16T20:10:04.495Z Reads: 164

```
@solidgeek I'm using version from here, is it not the latest? https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/master

It is using indeed analogWrite so i guess its old version, do you have link to the latest?

edit: 
Okay so it must be the development branch that has latest version..
Yes that did it! Data and ppm working properly now.
```

---
## \#2077 Posted by: Petja Posted at: 2019-04-18T20:45:01.402Z Reads: 179

```
Hello everybody. Thank you, SolidGeek, for sharing this project!

But I can't connect remote with VESC (I have VESC 4).
When I power receiver through USB, should transmitter see receiver? Because now, when I connect receiver to USB, symbol of antenna still blinking on lcd.
I use 220uF 10V tantalic capacitor between 5V and GND, 22pF ceramic capacitor between RST and GND on receiver.
Should I use capacitor between RST and GND on transmitter?
I clean EEPROM every time before uploading code on arduino (for transmiter and receiver). Is it normal, if I use RF24-1.3.2 library? Or should I use older release?
https://www.arduinolibraries.info/libraries/rf24
Which library VESC-UART should I use: from SolidGeek
https://github.com/SolidGeek/VescUart/tree/development
or from RollingGecko for VESC4
https://github.com/RollingGecko/VescUartControl/tree/imartinezl-master
Where did I make mistake?
![IMG_3107|690x304](upload://zArBBkabP3euQAgnAd6xYL2cUKw.jpeg) ![IMG_3105|690x361](upload://78T7Dji4A8robv5Tq0xVsb925XI.jpeg)
```

---
## \#2078 Posted by: curtis Posted at: 2019-04-19T02:56:11.910Z Reads: 173

```
You tube bro.
https://www.youtube.com/watch?v=N032HqxeymA&t=169s This guy has done 4 video's on it.
```

---
## \#2079 Posted by: curtis Posted at: 2019-04-19T03:01:24.950Z Reads: 178

```
https://www.youtube.com/watch?v=N032HqxeymA&t=169s
```

---
## \#2080 Posted by: Petja Posted at: 2019-04-19T18:22:30.288Z Reads: 178

```
I saw all videos made by SeeTheBridges. And also saw his posts in thread. Problem is not in assembling, problem is connection between receiver and transmitter. He didn't make video about it.![IMG_3057|690x459](upload://l9aYY7B4mJQRyxeQ7pFAzvtdoP2.jpeg)
```

---
## \#2081 Posted by: SeeTheBridges Posted at: 2019-04-19T19:00:13.500Z Reads: 180

```
Honestly getting the receiver and remote connected has always been my most fiddly part. Took me almost a half day on average to get every remote I built working properly. My recommendations are kinda strange, but first start out by touching the antenna on the remote while it's on. I've found sometimes for some reason the antenna was the wonky part and when I touched the ceramic, the remote would begin transmitting properly. If that's the case, I had 2 fixes with varying degrees of success. The first was to add an additional piece of wire to either side of the antenna about the full length of the arduino. I usually tried to tuck this behind my PCBs. If that didn't work, I'd remove the ceramic antenna entirely. That worked on a few occasions and didn't really effect connectivity range in my regular testing. Removing the ceramic was always my last ditch effort tho. I'd double check he continuity on all the NRF pads on both parts and then reflow them before attempting it.
```

---
## \#2082 Posted by: curtis Posted at: 2019-04-19T21:42:30.192Z Reads: 180

```
https://www.youtube.com/watch?v=C8n8ceZM9qY&t=228s
Pryside I think he is on the forums wrote some code for the remote that used different signals. Watch his video at 13:49. He goes over all of the problems.

curtis
```

---
## \#2083 Posted by: chickengun Posted at: 2019-04-19T21:44:23.493Z Reads: 179

```
This is his thread: https://www.electric-skateboard.builders/t/3d-printed-boosted-board-killer/88803
```

---
## \#2084 Posted by: solidgeek Posted at: 2019-04-19T23:03:46.068Z Reads: 184

```
First of all, you should use the development version for the Remote and receiver (newest version) https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development. If that doesnt solve the problem I would try erasing the EEPROM (overriding any bad settings) by changing the firmware version and reupload everything.

![Screenshot_20190420-010034__01__01|690x433](upload://vJSlczQV6WWgv2W9atDgFDcADsP.jpeg) 

The problem usually is bad connections (please double check all nrf24 connections) or wrong software. I havent had any hardware issues ever. But I might have been lucky.
```

---
## \#2085 Posted by: shupeste Posted at: 2019-04-21T11:34:29.602Z Reads: 177

```
Are you still selling the remotes? i would like to buy one if you are. thanks.
```

---
## \#2086 Posted by: huntercasillas Posted at: 2019-04-21T13:52:16.596Z Reads: 175

```
I don’t think anyone is right now, you’d have to make one yourself. I could be wrong though 🤷🏻‍♂️
```

---
## \#2087 Posted by: chickengun Posted at: 2019-04-22T17:29:39.701Z Reads: 181

```
For anyone those who experienced connection issues. It's no secret that the power filter on the receiver is important but today I found out something about the nrf module on the remote. For a reliable connection the wires coming from the nrf module need to be parallel to each other for around 1 cm, like shown here:
![image|690x265](upload://6FSwZGC1uKuZz5SMe5XKNwQY0Jq.jpeg) 
If they are soldered well but cross each other early (no short but not parallel to each other from pin direction) than I don't get a good connection. They have to be parallel for 1 cm, I used kapton tape to keep it in place and ever since didn't had any connection problems. Anyone can confirm this?
```

---
## \#2088 Posted by: chickengun Posted at: 2019-04-22T22:35:42.211Z Reads: 171

```
How can I invert acceleration/brake in the transmitter.ino ? One solution is of course to just flip the magnets but I have them already glued so I need to change it in the arduino file. Anyone knows how? @solidgeek
```

---
## \#2089 Posted by: willumpie82 Posted at: 2019-04-23T10:11:10.389Z Reads: 170

```
I build this remote a while ago, but I noticed a lot of noise on the throttle shown on the bar on the display. Since i upgraded my board to 150mm air tires, I also noticed this noise while driving.

any clue how to improve this?
```

---
## \#2090 Posted by: landonkun Posted at: 2019-04-23T23:45:16.979Z Reads: 176

```
I just got in my nano with integrated rf24. Has anyone tested this out yet?

![IMG_20190423_184442|666x500](upload://gL6A3pbnJlG7pZ6lkRwD4TPUar4.jpeg)
```

---
## \#2091 Posted by: Deakbannok Posted at: 2019-04-24T18:04:30.718Z Reads: 169

```
:) Just point the CSN and CE pins.
>>>> RF24 radio(10,9);
```

---
## \#2092 Posted by: balerion Posted at: 2019-05-02T11:26:15.274Z Reads: 164

```
I was thinking of getting the same. Did you get a chance to test it?
```

---
## \#2093 Posted by: niuva Posted at: 2019-05-04T00:15:33.098Z Reads: 162

```
If I'm not mistaken, the UART protocol changed for the Focbox Unity and the telemetry on the Firefly is broken. I'm highly sceptical my board can go 1000km/h.. or that's at least what the telemetry tells me. :laughing:

Did some digging on the forums and came across @StefanMe FeatherRemote and his updated VescUartUnity library. 
https://github.com/StefanMeGit/VescUartUnity

How to fix it for Unity users:
- Download and include the Unity lib into Arduino IDE
- comment out the old **#include "VescUart.h"** on line 5 in **reciever.ino**
- on the next line, paste the new Unity lib: **#include <VescUartUnity.h>**
- comment out **VescUart UART;** on line 116.
- paste **VescUartUnity UART;** on the next line 

Should be good to go, unless I forgot something.
```

---
## \#2094 Posted by: Michaelj1 Posted at: 2019-05-04T01:45:05.968Z Reads: 161

```
Has anybody had the issue with the remote where it freezes/ glitches out on startup? I thought maybe I had a tiny shirt somewhere but it seems to happen randomly. When the hall sensor was soldered on it would turn on and the RX light would light up, but with the hall sensor desoldered it just has the power light on. Normally on a successful boot up the L light blinks for a second. It’s really frustrating can someone help me?
```

---
## \#2095 Posted by: Michaelj1 Posted at: 2019-05-04T01:45:34.427Z Reads: 154

```
For clarification it fixes itself when I hit the reset button on the Arduino
```

---
## \#2096 Posted by: SeeTheBridges Posted at: 2019-05-04T03:29:29.576Z Reads: 160

```
Generally this happened when I had either a short or a bad solder joint somewhere on the remote. Typically though this was an issue I'd have on my receivers before I added a ceramic cap on the GND and reset pins. That might work for you in this instance as well but it'd only be a bandaid fix
```

---
## \#2097 Posted by: Michaelj1 Posted at: 2019-05-04T03:37:08.123Z Reads: 156

```
Ok, I’m gonna try and re solder all my pins, and see if that does anything. I’ll admit I’m not all the good at soldering as I’m relatively new to it (or at least new to doing it the RIGHT way😅)
```

---
## \#2098 Posted by: Michaelj1 Posted at: 2019-05-04T03:44:54.737Z Reads: 160

```
![image|375x500](upload://xFaA5VngMNn10tNrfoA5W5mFjdR.jpeg) 

As you can see I’m relatively new to this haha. I took the best picture I could, but let me know if anything stands out
```

---
## \#2099 Posted by: Michaelj1 Posted at: 2019-05-04T03:45:35.488Z Reads: 155

```
The loose wire is for the hall sensor, I ended up breaking mine so I had to order a new one
```

---
## \#2100 Posted by: niuva Posted at: 2019-05-04T11:20:16.709Z Reads: 158

```
Also a note for those who are not aware:
Placing a cap on the GND and Reset in some cases will not allow you to upload sketches to your Arduino, so placing a cap is recommended after the software is installed.

You say it's a 'bandaid' fix? What would you recommend as a more 'serious' fix? :slight_smile:
```

---
## \#2101 Posted by: SeeTheBridges Posted at: 2019-05-04T14:11:04.726Z Reads: 157

```
I'll let you know if I ever figure one out 😓 I said bandaid because like you said, some people have had issues with not being able to upload after placing the ceramic cap. I haven't run into that issue personally yet, but I do recognize that I have the luxury of a surplus of consistent hardware from the same manufacturer.
```

---
## \#2102 Posted by: sami Posted at: 2019-05-05T11:54:59.257Z Reads: 157

```
@SeeTheBridges @solidgeek  
I can't navigate in the menu, it's on "Trigger use" it only changes the value from Killswitch and Cruise. 
am I missing something?
all my wires are correct

EDIT: my magnet were reversed :sweat_smile: all good :smile:
```

---
## \#2105 Posted by: Michaelj1 Posted at: 2019-05-08T16:29:26.560Z Reads: 155

```
Edit/ update: Just tried shielding the NRF antennas and resoldering the one on the transmitter. Also plugged it into my VESC for power to see if that was the issue. It still pairs for just a second and then disconnects. I’m gonna guess that it’s code related then. I’ll keep you guys posted, sorry for the spam😬

last edit: fixed it. had the wrong UART library installed. cleared EEPROM, flashed devbranch of solidgeeks code, and everything seems to be working perfect! anybody know how to get UART info to show up?
```

---
## \#2106 Posted by: niuva Posted at: 2019-05-13T23:05:37.942Z Reads: 149

```
Decided to tweak my trusty Firefly Controller a bit and added vibration feedback to it.
- Buzzes during startup to let you know when it's operational without you having to look at the screen
- When the connection is lost to the receiver it will let you know by going into a rapid vibration frenzy. (Only when the deadmans switch is held down tho, to avoid pointless buzzing)
- The harder you brake the harder it will buzz in your hand. (If you are above 1KM/H)

Let's see how fast this will drain the tiny 500mah battery my Firefly has.

All it took was a [2N7000 Mosfet](https://www.aliexpress.com/item/20PCS-LOT-2N7000-TO92-Small-Signal-MOSFET-200-mAmps-60-Volts-N-Channel-TO-92-New/32907177045.html?spm=a2g0s.9042311.0.0.27424c4diPo3cS), a [5v flat 10mm motor](https://www.aliexpress.com/item/1pcs-Brand-new-Flat-10-2-7MM-button-motor-10mm-vibrating-motor-2V-5V-micro-DC/32899371784.html?spm=2114.search0104.3.8.53e71fefNVpc5V&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_319_10059_10884_317_10887_10696_321_322_10084_453_10083_454_10103_10618_10304_10307_10820_10821_537_10302_536,searchweb201603_52,ppcSwitch_0&algo_expid=4130c2e1-1f7a-4f1f-8adb-b431c4b28d32-1&algo_pvid=4130c2e1-1f7a-4f1f-8adb-b431c4b28d32&transAbTest=ae803_4) and a [few lines of code](https://pastebin.com/cFw3Bdwf).

Hopefully you can hear the buzzing in the video.

https://www.youtube.com/watch?v=pJavyScmKig
```

---
## \#2107 Posted by: farnamweb Posted at: 2019-05-14T10:46:53.693Z Reads: 149

```
The battery in the part list cuts the voltage at 2.7V. This damages the battery. 
I think we should just use a cheaper battery and add a board that cuts the voltage at 3.2V
```

---
## \#2108 Posted by: farnamweb Posted at: 2019-05-14T11:05:41.538Z Reads: 146

```
I'm thinking of building a few remotes for $115/each. Free shipping for US.

Would anyone be interested in buying?
```

---
## \#2109 Posted by: Flouw Posted at: 2019-05-19T18:41:59.696Z Reads: 134

```
Hey guys i have a bit of trouble with the code. I tried the library from solidgeek but i cant even compile the example sketch. It says that Serial1 is not declared. I am using an arduino nano and i am not sure how to fix this. Anyone an idea ? :frowning:
```

---
## \#2110 Posted by: solidgeek Posted at: 2019-05-19T19:46:15.969Z Reads: 132

```
Serial1 does not work in Nano. The example sketch is made using a Micro Pro which has a seperate UART for serial data. You cannot use a Nano and get debug/telemetry text out in Serial monitor, unless you use SoftwareSerial as the VESC UART port ☺️
```

---
## \#2111 Posted by: Flouw Posted at: 2019-05-19T20:21:00.787Z Reads: 131

```
Hey thanks for the answer :slight_smile:
i am a bit confused know because i dont know exacly how the serial port on my nano is named and sadly i am not so good at programming :frowning: i dont want to bother you but do you know what i have to change in the code to make it work ? 
P.s. thanks for this great remote design <3
```

---
## \#2112 Posted by: solidgeek Posted at: 2019-05-19T20:40:29.586Z Reads: 127

```
You will have to include the SoftwareSerial library and replace the Serial1 with a SoftwareSerial object. The SoftwareSerial works on most pins I quess, but you have to connect the VESC to the pins you define as RX and TX. You should be able to figure this out by looking at the documentation for the SoftwareSerial library 🙂🙄
```

---
## \#2113 Posted by: solidgeek Posted at: 2019-05-19T21:13:37.441Z Reads: 136

```
Actually if you download the development version it supports software Serial, and there is an example 🙃

https://github.com/SolidGeek/VescUart/tree/development
```

---
## \#2114 Posted by: Jeefberky Posted at: 2019-05-20T19:43:41.044Z Reads: 135

```
Hi,

I'm having trouble getting this setup to work again. I had setup the receiver and transmitter a long time ago and all was working well (did not install it in my longboard or remote). Now I have updated my vesc (hw version 4.12) to firmware 3.57 because vesctool otherwise did not work. After that the receiver/transmitter setup did not work.

I have updated the transmitter and receiver arduino sketch to the latest version from this url:
https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development

I also have removed the old vesc-uart library and changed it out with the following:
https://github.com/SolidGeek/VescUart/tree/development

(also tried this one:)
https://github.com/SolidGeek/VescUart

If I enable the debug feature on the receiver, I can see the trigger button being pressed and also see the position change of the throttle wheel. But i do not get telemetry data back from the vesc nor am I able to control the vesc via uart.

Maybe I have setup vesctool wrong, my settings for uart are:
App settings --> General: App to use: UART
App settings --> UART: Baudrate: 19200 bps

Could somebody help me how to get this working? 

Kind regards,
```

---
## \#2115 Posted by: solidgeek Posted at: 2019-05-20T21:54:48.353Z Reads: 124

```
Unless you are using the Firefly PCB receiver I made a few of, the baud for telemetry should be 115200.
```

---
## \#2116 Posted by: Jeefberky Posted at: 2019-05-21T07:35:01.776Z Reads: 130

```
Thanks. I will look at it later today. I'm using Arduino nano's for both the receiver and transmitter.

I'm already glad the two arduino's at least talk to each other.
```

---
## \#2117 Posted by: Jeefberky Posted at: 2019-05-21T15:55:50.927Z Reads: 132

```
I am able to control the vesc via the arduino's. Only telemetry is not working. Is there some setting I have missed?

Edit: With nog working telemetry, I meant I'm not getting vesc battery information to show on the screen.
```

---
## \#2118 Posted by: solidgeek Posted at: 2019-05-21T16:24:30.325Z Reads: 134

```
It sounds like a version issue. Which VESC firmware are you running?
```

---
## \#2119 Posted by: Jeefberky Posted at: 2019-05-21T16:37:41.465Z Reads: 135

```
I'm running firmware version 3.57 on hardware version 4.12.
```

---
## \#2120 Posted by: Falcon1651 Posted at: 2019-05-22T13:52:04.500Z Reads: 128

```
Hi how do i connect the nrf24 module to the vesc?
```

---
## \#2121 Posted by: solidgeek Posted at: 2019-05-22T15:39:08.851Z Reads: 113

```
And which software for the receiver are you using? And which VescUart library?
```

---
## \#2122 Posted by: Jeefberky Posted at: 2019-05-22T16:06:54.657Z Reads: 120

```
It is solved. All is working..... 

In the previous versions of your controller, you had battery voltage displayed on the oled. Now it shows the percentage. I was testing my vesc with a low cell count battery while the in settings it was configured as 8s. I was expecting it to still show voltage, instead it showed 00.0% (I just noticed the % symbol on the screen).

But to answer your question: 
I'm using the development build of the vescuart library and development build of the receiver and transmitter sketches.

Thanks anyway for the help!!!
```

---
## \#2123 Posted by: solidgeek Posted at: 2019-05-22T16:23:56.772Z Reads: 122

```
Glad you got it working 😊
```

---
## \#2124 Posted by: rice Posted at: 2019-05-25T10:57:43.399Z Reads: 127

```
Hello, I was wondering if anyone can help with my problem 
While i am compiling the receiver code, i get the error:

receiver:29:3: error: 'SERIALIO' was not declared in this scope

   SERIALIO.begin(115200);

Im using a clone arduino Nano with the ch340 Chip, but i had no problems uploading the transmitter code onto the same board.

Any help is appreciated thanks
```

---
## \#2125 Posted by: farnamweb Posted at: 2019-05-27T13:58:13.261Z Reads: 129

```
Please help me pair my Firefly NRF remote. 

The receiver  ( arduino + nrf24l01 ) is connected to the VESC TX/RX.  
The remote is powered on and I can see the throttle value changes on the LCD. 
I have configured FOC and I can move the motor with the PC keyboard. 

1) I selected "Setup Input" > NRF  
2) Turned off the remote and selected Next. 
3) Turned on the remote and restarted the timer.
4) Pressed the remote trigger button during the countdown. 
5) Timer finished and nothing appears on the screen


TWO OF THE WIRES WERE SWITCHED :)
```

---
## \#2126 Posted by: Jeefberky Posted at: 2019-05-27T15:11:58.761Z Reads: 133

```
You have to select UART in vesctool as communication protocol. And in UART settings you have to use a baud rate of 115200. This is because Arduino is talking to the vesc via UART at a default speed of 115200 baud.
```

---
## \#2127 Posted by: farnamweb Posted at: 2019-05-28T11:36:16.855Z Reads: 132

```
@solidgeek Are you still selling the PCB ? 
https://solidgeek.dk/produkt/firefly-receiver/
```

---
## \#2128 Posted by: farnamweb Posted at: 2019-05-28T12:08:41.425Z Reads: 135

```
I can't get the remote working. I have uploaded the firmware for RX and TX.TX LCD lights up but I see the Voltage as 0. I also can't control the motors. 

1) I have selected UART under "APP to Use" and UART is set to 115200 under the UART tab. Do I still need to follow the "Input Setup Wizard" ? If not, how do I pair TX and RX ? 
2) I can enter the remote menu by holding down the switch and powering on the remote, but I don't know how to change settings there.
3) Do I need to power on the TX first and RX second? 

Vesc : 4.12 with FW3.40  
firmware : https://github.com/Pryside/FireFly-Esk8-NRF24/blob/master/libraries  
VescUart Lib : https://github.com/SolidGeek/VescUart
```

---
## \#2129 Posted by: farnamweb Posted at: 2019-05-30T01:54:22.943Z Reads: 122

```
anyone? :frowning:
```

---
## \#2130 Posted by: Jeefberky Posted at: 2019-05-30T08:53:26.945Z Reads: 124

```
You could try to enable the debug feature on the transmitter or receiver, and use the serial monitor in the Arduino IDE to see if the transmitter and receiver are talking to each other.

If you enable the debug feature on the transmitter, you can only see if the connection with the receiver is successful.

If you enable the debug feature on the receiver, you have to disconnect the Arduino from the vesc. Then in serial monitor you can see the throttle value and if the trigger is being pressed.

Also, make sure you have connected rx-tx right on the vesc and receiver. Arduino Rx -> vesc tx / Arduino Tx -> vesc Rx.

I think someone mentioned, a few posts back, that the development build is the latest build of the firmware, and is optimised for vesc 3.xx firmwares (correct me if I'm wrong).
The debug feature for the receiver is available in the development build.
```

---
## \#2131 Posted by: farnamweb Posted at: 2019-05-31T06:07:36.058Z Reads: 120

```
You are a life saver. 
I had a terrible problem. I had to swap an NRF and also erase the EEPROM. 
Debugger was showing the same address "e8e8f0f0e1" even though I changed it and re-uploaded it.
I erased the EEPROM using the below sktech. Feel free to message me if you need help setting this up. 

Here is the sketch 

    #include <EEPROM.h>

    void setup()
    {
      // write a 0 to all 512 bytes of the EEPROM
      for (int i = 0; i < 512; i++)
        EEPROM.write(i, 255); 
     // turn the LED on when we're done
        digitalWrite(13, HIGH);
      }

    void loop()
     {
     }
```

---
## \#2132 Posted by: Gpole Posted at: 2019-05-31T16:49:13.330Z Reads: 115

```
First of all the brackets are missing in the for loop, and you will turn on the LED immidetly
should be
```
for (int i = 0; i < 512; i++) {
    EEPROM.write(i, 255);
}
digitalWrite(13, HIGH);
```
```

---
## \#2133 Posted by: wafflejock Posted at: 2019-05-31T16:53:21.099Z Reads: 118

```
https://stackoverflow.com/questions/26289546/what-does-a-for-loop-without-curly-braces-do

Although stylistically I agree add braces for clarity don't need a GOTO fail bug :)

https://nakedsecurity.sophos.com/2014/02/24/anatomy-of-a-goto-fail-apples-ssl-bug-explained-plus-an-unofficial-patch/
```

---
## \#2134 Posted by: Gpole Posted at: 2019-05-31T18:23:40.317Z Reads: 109

```
Wow diddnt know that, great info !
```

---
## \#2135 Posted by: farnamweb Posted at: 2019-06-01T01:32:35.095Z Reads: 110

```
The code runs without the braces too.
```

---
## \#2136 Posted by: farnamweb Posted at: 2019-06-04T05:26:03.874Z Reads: 103

```
I got the remote working but why does the connection Icon on the remote LCD keep blinking? 

Isn't it supposed to not blink when the connection is established ?
```

---
## \#2137 Posted by: Jeefberky Posted at: 2019-06-04T07:36:53.690Z Reads: 102

```
I think the nrf24 is not getting enough power. Powering the Arduino via a pc usb port is limiting the current. It is also advised to place a small capacitor over the power terminals (watch the polarity) of the nrf24 to make sure there is always sufficient power available for the nrf24.
```

---
## \#2138 Posted by: farnamweb Posted at: 2019-06-04T07:43:37.476Z Reads: 104

```
both RX and TX are connected to battery and not USB. I have installed a capacitor to filter the 5V input to RX. There is already a 3.3V regulator on Arduino. Do you think the cap is necessary on the nrf ?
```

---
## \#2139 Posted by: Jeefberky Posted at: 2019-06-04T07:49:40.186Z Reads: 108

```
I think the cap is useful to prevent packet loss. I still think the nrf is getting not enough power delivered by the Arduino. Because If I'm powering the the Arduino via pc usb, the connection icons keeps blinking, although I can control the vesc.
```

---
## \#2140 Posted by: farnamweb Posted at: 2019-06-04T07:52:21.733Z Reads: 106

```
good to know. What size cap do you use?
```

---
## \#2141 Posted by: Jeefberky Posted at: 2019-06-04T15:46:24.816Z Reads: 98

```
I'm using a 10 nanofarad cap that I have salvaged from an old motherbord. Probably a bit overkill.
```

---
## \#2145 Posted by: farnamweb Posted at: 2019-06-13T01:58:09.106Z Reads: 110

```
WTF!!
My new remote loses connection left and right. I have shielded both TX and RX and installed a giant capacitor (470UF) on both NRFs. RX has a 100MF capacitor on the 5V rail. 
1) Do I need to install a cap on the TX's 5v? 
2) Could it be a bad NRF ? I'm using these 
https://de.aliexpress.com/item/SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in-stock-fast/32367254718.html
3) Can I use these modules instead? Are these modules compatible with the code? 
https://www.amazon.com/dp/B00O9O868G/ref=twister_B07434GZWL?_encoding=UTF8&amp;psc=1
```

---
## \#2146 Posted by: solidgeek Posted at: 2019-06-13T07:06:10.388Z Reads: 111

```
Its important that you do not Shield the antenne, only the electronics. And yes a capacitor om the receivers 5V is essentiel as the VESCs 5V power supply can be a little unstable.
```

---
## \#2147 Posted by: matiller Posted at: 2019-06-13T16:24:57.123Z Reads: 118

```
So, I have problem with receiving data here is receiver:
![1|403x272](upload://3FCiIpySadhu2bRQAqRy0dctD8t.png) 
transmitter:
![22|690x383](upload://bXlXlIAO4IFTYdyKJj0yV31VpFT.png) 

when I restart the transmitter it sends data... unfortunately just one package. Already have cap on 5v receiver 3.3v receiver antena. (GettingStarted.ino code works great when added radio.setAutoAck(false); //also tried adding it in firefly remote code -- didnt help//, both arduinos are receiving and sending) (I connected Hall data to 5v that is why it is 1023 (if you are wondering)
```

---
## \#2149 Posted by: farnamweb Posted at: 2019-06-14T10:29:01.965Z Reads: 102

```
I’m using these NRF modules [https://de.aliexpress.com/item/SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in-stock-fast/32367254718.html ](https://de.aliexpress.com/item/SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in-stock-fast/32367254718.html)
Can I use these modules instead? Do I need to change anything in the code?[https://www.amazon.com/dp/B00O9O868G/ref=twister_B07434GZWL?_encoding=UTF8&amp;psc=1 ](https://www.amazon.com/dp/B00O9O868G/ref=twister_B07434GZWL?_encoding=UTF8&amp;psc=1)
```

---
## \#2150 Posted by: Jeefberky Posted at: 2019-06-14T10:33:11.340Z Reads: 103

```
You can use them. I am also using the modules from the second URL.
```

---
## \#2151 Posted by: niuva Posted at: 2019-06-14T11:57:06.989Z Reads: 104

```
I recommend these. Already shielded and allows for external antenna.
https://s.click.aliexpress.com/e/b9vobc5K
```

---
## \#2152 Posted by: farnamweb Posted at: 2019-06-15T05:12:45.882Z Reads: 106

```
Thank you guys for helping out. I switched my NRFs with the ones from Amazon and the connection  is flawless now. Rode 5 miles without a single connection drop. I did use 100UF capacitors on both NRFs but I didn't use shielding. 

https://www.amazon.com/dp/B00O9O868G/ref=twister_B07434GZWL?_encoding=UTF8&psc=1
```

---
## \#2153 Posted by: farnamweb Posted at: 2019-06-15T11:22:17.379Z Reads: 107

```
1) What is the point of using this battery with the built in BMS? It cuts power at 2.7V. LIPOs usually die around 3V and sometimes can't be recovered. 
https://de.aliexpress.com/store/product/502535-3-7V-300mAh-lithium-polymer-battery-for-MP3-player/818305_32215795542.html

2) The NRFs that I'm using accept 5V. I assume I don't need to buy the 3.3V Arduino. correct? 
https://www.amazon.com/dp/B00O9O868G/ref=twister_B07434GZWL?_encoding=UTF8&amp;psc=1
```

---
## \#2154 Posted by: Petja Posted at: 2019-06-17T21:43:37.142Z Reads: 116

```
I upload the newest version (version 2) into transmitter and receiver. Also I erase the EEPROM every time before I upload the sketch.

But I found some bugs:

1. In menu setting I can’t choose “Cruise”. Only “Killswitch”. The same situation with control mode. I can use only “PPM and UART”.
2. After exit from settigs, throttle is working without involved trigger.

Video about it:
https://vimeo.com/342838556
```

---
## \#2155 Posted by: Petja Posted at: 2019-06-21T22:48:23.750Z Reads: 113

```
Is it normal that throttle working without involved trigger in firmware version 2? Is anybody here?
```

---
## \#2156 Posted by: sami Posted at: 2019-06-23T06:10:07.884Z Reads: 112

```
I have the same issue... Calling @solidgeek
```

---
## \#2157 Posted by: niuva Posted at: 2019-06-23T10:42:13.871Z Reads: 110

```
The throttle/braking indicator should move, even without the killswitch being held down. 
But it should not transmit the throttle values to the receiver until the killswitch is held down. Braking should work even without the killswitch.

Cruise control has not been implemented yet nor UART control (Telemetry is sent over UART and throttle/braking via PPM). I think @Pryside 's firmware works via UART so you can ditch PPM, if you need that. Not tried his firmware, so I can't recommend it personally, but I know he did some changes to get control working over UART as well.
```

---
## \#2158 Posted by: Elmar04 Posted at: 2019-06-26T11:53:52.904Z Reads: 105

```
I have tried building this remote but it doesn't connect. I used a slightly different transceiver module.
This one: https://www.aliexpress.com/item/32599246022.html?spm=a2g0s.9042311.0.0.77b94c4d7xKxhn (the small one)
the receiver turns on and all but it gives that moving connecting logo.
What should i do?
```

---
## \#2159 Posted by: Petja Posted at: 2019-07-02T05:22:44.427Z Reads: 106

```
@niuva, thank you for answer! I think, it will be better talk about Solidgeek’s firmware. But I still didn’t decide problem with connection transmitter and receiver.
Maybe I use incorrect library for nRF24L01. I downloaded this one from here:
https://www.arduinolibraries.info/libraries/rf24
As I can see, SPI bus pins are 7 – CE, 8 – CSn.
In @SolidGeek's sketch are using 9 – CE, 10 – CSn.
What library do you use?
Should transmitter see receiver (symbol of antenna will not blinking), if I will power receiver by USB?
```

---
## \#2160 Posted by: Daniel_Kievit Posted at: 2019-07-03T15:42:55.368Z Reads: 108

```
Hi, I've made the esk8 remote, but i have two little problems. Maybe anyone can help me fix them?

1. The throttle bar in the screen only goes until the middle of the throttle bar. This also happens when I push the throttle completely forward. I ordered the same magnets as in the spreadsheet, but maybe they are not strong enough? Or is it maybe something about the hall sensor? Or have I mounted the wheel incorrect? When I bring a single magnet (without the throttle wheel) very close to the hall sensor it does go to the full throttle in the screen.

Edit: I think I have mounted the hall sensor incorrectly. When i bring it closer up to the wheel it the throttle value goes to zero and to 249. But 249 isn't completely full either. This only happens with the 249 side and not with the 0 side. Does anybody have a clue why this happens? 

2. The connectivity symbol in the screen does not show up when I have both the receiver and the transmitter on. It only blinks. Would it be connected? I can't test it yet, because i don't have a vesc yet. 



Has anyone else had these problems before? Does anybody know how to solve this? 

I'd really appreciate your help!!
```

---
## \#2161 Posted by: solidgeek Posted at: 2019-07-04T21:07:43.593Z Reads: 96

```
Looks like something is causing the settings to reset every time you try to change a setting. To change the "Control mode" you have to be connected to the receiver, I can't remember if this is the case for "Trigger type" also. Have you tried connecting the receiver at the same time?
```

---
## \#2162 Posted by: solidgeek Posted at: 2019-07-05T09:51:54.784Z Reads: 95

```
You have to calibrate the hall sensor, this can be done in the settings menu.
```

---
## \#2163 Posted by: matiller Posted at: 2019-07-05T19:27:10.459Z Reads: 91

```
Does anyone have schematic for updateabble arduino using charger usb? If I want to do that I have to connect Charging and Discharging pins or how can I do it?(I am thinking of diodes, but hoping there is better way as they reduce voltage) Thanks.
```

---
## \#2164 Posted by: matiller Posted at: 2019-07-05T19:28:29.937Z Reads: 91

```
It will not work if it blinks...
```

---
## \#2165 Posted by: Daniel_Kievit Posted at: 2019-07-06T18:54:46.219Z Reads: 92

```
Thanks,

It really worked!! Do you also know how to solve the connectivity issue? The connection icon on my oled screen keeps blinking, while I have turned the power on of both the receiver and the transmitter. Of course I have uploaded the code and I haven't changed the pipe. 

Maybe it is because I don't have a VESC connected to my receiver? 

Help would really be appreciated!
```

---
## \#2166 Posted by: Parafodas Posted at: 2019-07-08T06:45:36.980Z Reads: 87

```
You you click on the resect boton in the ardoino you dont have conection?( Reciver)
```

---
## \#2167 Posted by: solidgeek Posted at: 2019-07-08T22:24:08.896Z Reads: 87

```
Have you tried running the debug to see if the nrf24 modules are connected correctly and working? :-) Just uncomment #DEBUG
```

---
## \#2168 Posted by: farnamweb Posted at: 2019-07-09T01:21:01.052Z Reads: 88

```
I'd like to report a serious SAFETY issue!!!!!!!!!!!!!! :open_mouth::open_mouth::open_mouth::open_mouth::open_mouth:   
Today, the remote lost the connection for a second and when it came back the throttle remained on the same value.The remote was unresponsive to any commands.
It threw me off the board and the board continued moving forward, finally the board hit the curb and I was able to lift it and power it down. power cycled both the remote and the board and everything went back to normal, I even rode it for another 15km and I didn't experience any connection loss. 
@solidgeek, we should review the code to find the issue. This can be really dangerous :(
```

---
## \#2169 Posted by: solidgeek Posted at: 2019-07-09T01:30:23.024Z Reads: 93

```
Sorry to hear mate, hope you are alright :grimacing:! It sounds weird though, nothing I have experienced before. Have you been able to reproduce this issue? Would be great to eliminate hardware problems such as the throttle getting stuck, which could explain the behavior.

The receiver got a fail-safe that cuts the throttle if the connection is lost for more than a few packages: https://github.com/SolidGeek/nRF24-Esk8-Remote/blob/a70a9fb09ecb110ddd1fdb40eb173e6ce42d27d9/receiver/receiver.ino#L233

What version of the firefly software are you using? :slight_smile: And have you made any changes to the remote, such as extra capacitors or added some features?
```

---
## \#2170 Posted by: farnamweb Posted at: 2019-07-09T01:46:21.686Z Reads: 91

```
Thanks man. Thankfully nothing happened to me or the board. I'm using v2.0 and I haven't been able to reproduce the issue.
There is only one extra 22 nF ceramic cap on the receiver RST/GND and I haven't edited the code. 
I'm sure the connection was lost. The connection icon was blinking right before the board went crazy.
Good to mention that I rode the board in the small puddle of water right before the accident. It's possible that water got into the VESC case where the RX is mounted, It's unlikely though.
```

---
## \#2171 Posted by: solidgeek Posted at: 2019-07-09T10:03:20.214Z Reads: 85

```
Glad to hear! I have newer liked the addition of that capacitor as it fiddles with the Arduinos boot-cycle, however it should not cause such issues. The more I think about it, the only possible answer I can come up with is some sort of hardware problem, as the software should perform as always... Are you sure that the throttle didn't get stuck? :face_with_raised_eyebrow: Because it is not possible for the remote to keep sending the same throttle if it crashed or somehow got inside an infinite loop. Are you using PPM or UART?
```

---
## \#2172 Posted by: StefanMe Posted at: 2019-07-09T10:19:46.817Z Reads: 81

```
Make shure the OLED display is propperbly conencted. Squeeze the shell ect. I found some issues on unstable OLEDs there. Add an 10K pull up resistor to SCL and SDA. This should help a lot.
```

---
## \#2173 Posted by: niuva Posted at: 2019-07-09T10:20:03.285Z Reads: 88

```
[quote="solidgeek, post:2171, topic:28543"]
I have newer liked the addition of that capacitor as it fiddles with the Arduinos boot-cycle, however it should not cause such issues.
[/quote]

Personally, I've never managed to get any of my Firefly receivers working without the cap on GND and RST and I've built like 10. All of them crash on boot without it when powered by the VESC. Ceramic cap gets applied after the firmware upload.
I also have a 220uF cap on the 5V in. Never have I had any issues with Fireflys and I've been running them for a solid year.
```

---
## \#2174 Posted by: Daniel_Kievit Posted at: 2019-07-09T12:11:50.783Z Reads: 96

```
**If I uncomment DEBUG in the transmitter code, I get this on my serial monitor:**

⸮⸮STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0

RX_ADDR_P0-1	 = 0xe8e8f0f0e1 0xc2c2c2c2c2

RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6

TX_ADDR		 = 0xe8e8f0f0e1

RX_PW_P0-6	 = 0x20 0x00 0x00 0x00 0x00 0x00

EN_AA		 = 0x3f

EN_RXADDR	 = 0x03

RF_CH		 = 0x6c

RF_SETUP	 = 0x07

CONFIG		 = 0x0e

DYNPD/FEATURE	 = 0x3f 0x06

Data Rate	 = 1MBPS

Model		 = nRF24L01+

CRC Length	 = 16 bits

PA Power	 = PA_MAX

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

and then it keeps going on.

The connection icon on the OLED screen also keeps blinking.

And can someone tell me what the ResetButton is for? And what does the led indicate, because it blinks 3x slow and then 3x fast.

**When I uncomment debug on the transmitter, I found this on the serial monitor:**

STATUS		 = 0x0e RX_DR=0 TX_DS=0 MAX_RT=0 RX_P_NO=7 TX_FULL=0

RX_ADDR_P0-1	 = 0xe8e8f0f0e1 0xc2c2c2c2c2

RX_ADDR_P2-5	 = 0xc3 0xc4 0xc5 0xc6

TX_ADDR		 = 0xe8e8f0f0e1

RX_PW_P0-6	 = 0x20 0x00 0x00 0x00 0x00 0x00

EN_AA		 = 0x3f

EN_RXADDR	 = 0x03

RF_CH		 = 0x6c

RF_SETUP	 = 0x07

CONFIG		 = 0x0e

DYNPD/FEATURE	 = 0x3f 0x06

Data Rate	 = 1MBPS

Model		 = nRF24L01+

CRC Length	 = 16 bits

PA Power	 = PA_MAX

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Failed transmission

Sometimes it says "transmission succes one or two times, when I move the throttle:

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Transmission succes

e8e8f0f0e1: Failed transmission

e8e8f0f0e1: Transmission succes

e8e8f0f0e1: Failed transmission

**My questions:**
- Can the remote be connected to the receiver, while the connection icon on the OLED blinks?
- What does the blinking(3x slow, 3x fast) led on the receiver mean?
- What is the function of the ResetButton on the receiver?
- Can you guys make up a problem of the text on my serial monitor?
- Is it ok, when there only is a "transmission succes" on the serial monitor, when I move the throttle? 

I really hope anybody can answer my questions!!!!
```

---
## \#2175 Posted by: farnamweb Posted at: 2019-07-10T19:47:23.711Z Reads: 88

```
While I was running after the board, I turned off the remote and it didn't stop the motors. I think water got into the VESC case and caused that.not sure how but that's the only explanation.     
Even if the throttle was stuck, the killswitch had to be stuck at the same time. 

I'm using PPM and UART. Time to waterproof the case and the electronics. 

I'm thinking of adding a few features like vibration alert and one LED slot to show when the LIPO is charging/charged. Do you accept code commit?
```

---
## \#2176 Posted by: solidgeek Posted at: 2019-07-10T21:16:02.278Z Reads: 90

```
Thanks for the explanation, well that means the remote being faulty is out of the question. The issue was between the receiver and the VESC, and most likely caused by some faulty PPM signal. The PPM signal is an analog protocol, making it impossible for the VESC to know if the throttle signal is corrupt. To eliminate this possibility I would recommend using "UART only" instead, as the digital protocol uses CRC to validate the integrity of the signal. Furthermore, the UART packages has to be generated and sent at a given internal, thus if the receiver crashes the VESC simple stops. 

I accept code commits if they are well done, while adding some cool features :slight_smile:
```

---
## \#2177 Posted by: solidgeek Posted at: 2019-07-10T21:25:27.187Z Reads: 94

```
Hey Daniel,

As to answer your questions first:

- No
- Probably just getting some packages while losing some
- To reset the settings
- No problem from the log other than bad connection
- No it should stay on (not blinking) if there is a stable connection

From the log it is clear that the nRF24 modules are connected correctly, and works. I am pretty sure you are dealing with a hardware problem. You can try setting the nRF24 power level a little lower. Instead of setPALevel(RF24_PA_HIGH) in the setup, write setPALevel(RF24_PA_LOW). If it works after this, you need to add some capacitance (220uF) to the 3.3V power rail (both remote and receiver).

The problem could also be caused by some bad RF isolation, try to cover your nRF24 modules in some isolation, and wrap them in tinfoil (not the antenna of course :stuck_out_tongue:)

Let me know what you find out!
```

---
## \#2178 Posted by: farnamweb Posted at: 2019-07-11T00:37:27.943Z Reads: 88

```
I thought your code only supports PPM for signal.What else do I need to do besides selecting UART only in Vesctool?
```

---
## \#2179 Posted by: solidgeek Posted at: 2019-07-11T01:25:05.558Z Reads: 89

```
Select the correct baud rate, and change the Control mode on the remote. Should work 👍
```

---
## \#2180 Posted by: farnamweb Posted at: 2019-07-11T01:44:48.120Z Reads: 90

```
The signal cable is still connected to PPM on the VESC. Can I just unplug that cable after selecting UART only?
```

---
## \#2181 Posted by: solidgeek Posted at: 2019-07-11T09:48:49.633Z Reads: 90

```
The signal cable (PPM) is no longer needed, just RX, TX, GND and 5V :-)
```

---
## \#2182 Posted by: Daniel_Kievit Posted at: 2019-07-12T12:46:13.772Z Reads: 93

```
Thanks a lot!

It really worked and i got it connected. 

I do still have a few little problems:

* One problem is that when I move the throttle, the led on the receiver flashes 3 times slow and then 3 times fast. The connection icon on the remote also flashes. Is this normal or not?

* Another problem is that, when I move the throttle, the battery level goes up, while I haven't connected anything to pin A2. I also didn't short pin A3 and A2. Does anyone know why this happens?

* I also have my doubts about the connection of the NRF's, because the led on the receiver sometimes just blinks a few times and sometimes it loses connection completely. Has anybody got a solution for this?

Thanks everybody, it's really nice to be able to ask my questions to you guys!
```

---
## \#2183 Posted by: solidgeek Posted at: 2019-07-12T17:46:02.318Z Reads: 89

```
If you haven't connected anything to A2, the analog port floats around, meaning it picks up the slightest variations in the surrounding noise, e.g. the A3 wire right next to it. Why not connect A2 as it should? 

Please supply some images of your setup, of both the remote and receiver. Did you build it exactly as I showcased in my tutorials?
```

---
## \#2184 Posted by: Daniel_Kievit Posted at: 2019-07-13T13:33:59.283Z Reads: 93

```
I cant do that yet, because I don't have the parts yet.
```

---
## \#2185 Posted by: farnamweb Posted at: 2019-07-13T15:23:53.254Z Reads: 96

```
I can't find a alternative for this arduino board anywhere in US? please let me know if there is one. 
https://de.aliexpress.com/item/32664577152.html
```

---
## \#2186 Posted by: SeeTheBridges Posted at: 2019-07-13T15:52:58.578Z Reads: 95

```
You can buy the robotdyn V3s straight from robotdyn last time I checked their website. They're the exact same ones recommended from AliExpress unless the parts list has changed. 

https://robotdyn.com/nano-v3-atmega-328-usb-ttl-ch340g-micro-usb-with-cable-not-soldered.html

Or if you don't want to trust them with payment info, I've got a box of them available too
```

---
## \#2187 Posted by: farnamweb Posted at: 2019-07-14T04:50:14.810Z Reads: 94

```
I sent you a PM. Please reply there :slight_smile:
```

---
## \#2188 Posted by: ShutterShock Posted at: 2019-07-15T14:46:52.964Z Reads: 89

```
I got mine from here too, they delivered late but they did arrive.
```

---
## \#2189 Posted by: Philipp6 Posted at: 2019-07-15T16:52:15.375Z Reads: 92

```
Must I use the SS495A hall sensor or can I use a other one??
```

---
## \#2190 Posted by: Daniel_Kievit Posted at: 2019-07-19T09:25:32.125Z Reads: 94

```
Try the one you have. Mine worked with another one. Just make sure to check the pinout in the datasheet, otherwise you could fuck up your hall sensor. It should have 3 pins: a 5v pin, GND pin and a signal pin.
```

---
## \#2191 Posted by: mark_c Posted at: 2019-07-22T07:33:50.645Z Reads: 91

```
Hello, 

Im trying to get this code uploaded onto my Firefly remote build but cannot seem to get past the VescUart does not name a type issue. If anyone could help me out, I would be very much appreciative.

![34%20AM|690x388](upload://9nz55i0XBcCjfb1G1AnUNGxAbV0.png)
```

---
## \#2192 Posted by: mark_c Posted at: 2019-07-22T07:38:33.680Z Reads: 89

```
![IMG_1331|375x500](upload://8N2pTB8njF8GEqgpPgOtO9KMTJS.jpeg)
```

---
## \#2193 Posted by: solidgeek Posted at: 2019-07-22T12:15:57.178Z Reads: 83

```
You need to use my VescUart library: https://github.com/SolidGeek/VescUart
```

---
## \#2194 Posted by: mark_c Posted at: 2019-07-22T13:15:55.437Z Reads: 80

```
Thank you, Ive just started with Arduino about a week ago so still a noob :) I had your library but had to go through and delete the older ones. Its working now!

Another issue ive run into is I cant get the ESC and motor to start without following the process below.

So the receiver and transmitter connect shown when the LED lights up solid (the motor chirps twice and then follows with a series of chirps, it does not "arm")
Next I have to hold the trigger in, then adding reverse on the thumb wheel, only then do I get the distinct chirp that the motor is "armed" and then it proceeds to spin unless I put maximum reverse,

What am I doing wrong?
```

---
## \#2195 Posted by: solidgeek Posted at: 2019-07-22T19:06:31.294Z Reads: 78

```
Well that's hard to tell... But have you calibrated your hall-sensor through the remote settings?
```

---
## \#2196 Posted by: TomBE Posted at: 2019-07-22T20:07:24.189Z Reads: 85

```
Hi,
First of all i followed this thread for a while now and @solidgeek it's amazing that you still respond after 2 years. You da best! :wink:

That being said i build it myself and i ran into 1 issue so far. My triggerbutton won't work. I have connected it to D3 and changed it in the code (maybe d4 is somehow broken) but that doesn't solve it.
Nothing happened when i press/hold the button.

Followed the instructions on your website.
```

---
## \#2197 Posted by: solidgeek Posted at: 2019-07-22T20:34:46.986Z Reads: 83

```
I do my best to support :-) Do you have a multi-meter? It could be the switch that is broken. Measure the resistance between the two terminals you selected, and press the switch. If the resistance goes to zero, everything should be good. Maybe you chose the wrong terminal points?
```

---
## \#2198 Posted by: TomBE Posted at: 2019-07-22T20:54:54.381Z Reads: 83

```
The button is brand new and working fine. Tried to make a connection with just a jumper wire connecting D4 straight to GND. Didn't do anything either
```

---
## \#2199 Posted by: solidgeek Posted at: 2019-07-22T20:57:58.052Z Reads: 81

```
Hmm, sounds weird. You use the development branch right? Can you use the trigger within the settings?
```

---
## \#2200 Posted by: TomBE Posted at: 2019-07-22T21:05:11.178Z Reads: 80

```
What do you mean with development branch?
I can't do anything with the trigger.
I wanted to open the menu but couldn't.
```

---
## \#2201 Posted by: mark_c Posted at: 2019-07-22T21:21:18.997Z Reads: 83

```
Im not currently using a hall sensor, Im using a small rc plane hobby esc and motor ( Im not even sure if it works in reverse), this was a simple way to test if it all worked. Next I will be adding an Arc 200 ESC and 6384 Motor. Thanks for the response, it is much appreciated, the simple matter of fact is that i have no idea what im doing yet but ive got this far and wont stop. I think the remote you have built and open sourced is fantastic and it seems the community are very appreciative.
```

---
## \#2202 Posted by: mark_c Posted at: 2019-07-22T22:24:48.140Z Reads: 85

```
Ah I am using a hall sensor, I thought you meant in the motor itself, no, I haven't calibrated it, I presume I can find the the instructions on your wiki page?
```

---
## \#2203 Posted by: solidgeek Posted at: 2019-07-22T22:50:53.407Z Reads: 89

```
Oh! glad to hear, makes much more sense now :P Well it is straight forward, just enter the Settings menu, and scroll to the "Throttle" settings. Then change the min, max and center values, to your sensors min, max and center output. 

![image|632x185,75%](upload://bC72dXidhYgi577Ij3Rma5iIsEO.jpeg)
```

---
## \#2204 Posted by: TomBE Posted at: 2019-07-28T15:26:55.716Z Reads: 90

```
So i managed to get into the settings. I just didn't know how. I tried to hold the trigger for a few seconds etc. But i didn't try to hold it while starting up the remote. So now i know.

Second issue now: my remote won't connect to the receiver anymore. I resoldered everything and made sure the wires are parallel to each other for over 1cm like someone said here but didn't help. Maybe one of the rf24l01 is broken but that would be very fast. Any idea's?
The connection icon just keeps flickering.

EDIT: would it be possible to make it a wired remote till i have a new rf24l01?
```

---
## \#2205 Posted by: captclearleft Posted at: 2019-07-29T17:45:46.671Z Reads: 96

```
Hey @solidgeek - You have done a FANTASTIC! job. Thanks SO MUCH!  Love this remote!

I am updating my firefly transmitter and receiver to the latest...  
OK... So I am reading through this thread "backwards", and am a little lost as to what happened while I was away...  
Sooooo - Three questions here: 

Are we still able to use the Arduino NANO?

Is this still the [valid working schematic](https://solidgeek.dk/docs/firefly-remote/receiver/schematic/) ?

![reciever-schematic|690x417,75%](upload://1nC4DRwxq4EBhEAZxxbRwfySHBN.png) 

AND... We are no longer using the RollingGecko Library - Is that correct?  
We are now using [your custom VescUart Library](https://github.com/SolidGeek/VescUart/tree/development) .

I am updated with my VESCs (4.12) to the latest firmware. And I do want to use UART as opposed to the PPM signal that was used on the old firefly version.
Thanks so much.
```

---
## \#2206 Posted by: Parafodas Posted at: 2019-07-30T09:21:15.558Z Reads: 83

```
Hello im usinhg the vesc 4.12 it fw3.57 and i dont get any data form the pins tx ,rx
```

---
## \#2207 Posted by: Parafodas Posted at: 2019-07-30T09:23:39.968Z Reads: 81

```
But the ppm signal its ok .  Only worcks it fw3.40?
```

---
## \#2208 Posted by: Petja Posted at: 2019-08-01T05:41:11.309Z Reads: 84

```
It's been a long time coming, but I maked remote. I used RF-Nano and changed CE, CS pins (after looking schematic). I tried to connect two VESC 4.12 via CAN. And I saw that transmitter didn't take data. I recieved data when used only one VESC. Can remote work with two VESC with taking data?
```

---
## \#2209 Posted by: Parafodas Posted at: 2019-08-01T05:51:41.569Z Reads: 82

```
I gess not . It only gets telemetry of 1 vesc
```

---
## \#2210 Posted by: Petja Posted at: 2019-08-01T05:57:24.088Z Reads: 82

```
I thought that master VESC accumulate all information and send it on transmitter.
```

---
## \#2211 Posted by: Parafodas Posted at: 2019-08-01T06:01:31.271Z Reads: 83

```
Hey im not a expert , i havinhg some problems to . 😂😂😂
```

---
## \#2212 Posted by: bukl Posted at: 2019-08-01T09:12:46.441Z Reads: 86

```
Hey, does the code work with the nrf51 Firmware included in the VESC-Tool?
```

---
## \#2213 Posted by: solidgeek Posted at: 2019-08-01T21:17:14.214Z Reads: 93

```
@captclearleft Glad you like the remote :-) Yes the remote is still compatible with Arduino Nano, and it is the correct schematics. The VescUart library I made is compatible with FW3.40, I have not tested any newer versions. I know that @Pimousse has updated the library to newer versions of the VESC firmware, download here: https://github.com/Peemouse/VescUart/

@Parafodas and @Petja Try the updated version from https://github.com/Peemouse/VescUart/
 
@bukl I am not sure what you mean. The Firefly needs its own receiver at the moment, it cannot connect directly to the VESC NRF51 receiver unless changed dramatic.
```

---
## \#2214 Posted by: Petja Posted at: 2019-08-01T23:37:38.907Z Reads: 94

```
@solidgeek Ok, I will try to update. But I use PPM splitter today (assembled like attached picture). All is good! Both motors are spinning and I'm getting telemetry on transmitter.
But I notice that motor connecting to slave VESC starts to rotate late than motor connecting to master VESC (on CAN bus and PPM splitter). What should I do?
![Twin-VESC-wiring|690x370,100%](upload://giJtlGEEVhmc0f03XU9xlB4MxCw.jpeg)
```

---
## \#2215 Posted by: captclearleft Posted at: 2019-08-03T17:33:17.751Z Reads: 93

```
@Petja : NOTE: I don't know your exact setup, and I don't understand the ppm splitter with theCAN bus.  

I "think" a motor spinning late is normal (unless you are running them as FOC).  The motors are not perfectly matched to spin the same rpm (unless hooked up FOC).  Its just like any other BLDC motor.  Each motor gets a pulse signal from the motor controller to spin the motor...   

Its kinda like an open differential on a pickup truck...  Lightly hold (and I mean just a touch) the wheel that spins first...  You will notice the other wheel spin...  Its hard to match your belt tensions perfectly, and your motors are not wound exactly the same.  

Further.  I believe you should run the "Motor Setup" on both VESCs (I did, but I am not entirely sure.)

Hope this helps...  Someone else - Please correct me if I am wrong... Thanks
```

---
## \#2216 Posted by: captclearleft Posted at: 2019-08-05T19:15:22.701Z Reads: 92

```
As always - Thanks so much for the help.  Fantastic.  
I think I will use FM3.4 for my VESCs. and your VescUART library.
```

---
## \#2217 Posted by: Quezacotl Posted at: 2019-08-07T17:46:32.408Z Reads: 97

```
Hello!

I built the transmitter and all seems to be OK. Now when i'm building the receiver, i encountered some different compiling errors. Tried different libraries and codes, but nothing seems to work.

So what is the current working code for both sender and receiver and all that is needed with it?
And i think i have the hardware ok, but to be sure. Any link to the most recent hardware?

Okay, so now i found this site through solidgeek's github profile: https://solidgeek.dk/docs/firefly-remote/software/

I followed things on the site, and it didn't compile. Became a bunch of errors. Finally i found out "https://github.com/SolidGeek/VescUart" with "https://github.com/SolidGeek/nRF24-Esk8-Remote/tree/development" are compiling without problems. Now i have used those for receiver and transmitter.

Even if those are the combination that should work, i still don't know what settings i need to do and in what VESC version those are supposed to work? And is there any special pairing thing?

EDIT: Okay. I got it to work :slight_smile:
```

---
## \#2218 Posted by: Jonisonvespa Posted at: 2019-08-08T16:03:21.424Z Reads: 99

```
hello
really interested in building one of these, i dont have a printer, could someone please sell me the latest version of the shell ?
thanks very much
```

---
## \#2219 Posted by: captclearleft Posted at: 2019-08-11T14:33:03.913Z Reads: 94

```
Hey @Jonisonvespa - Has someone gotten back to you yet?  What part of the word are you in?
```

---
## \#2220 Posted by: captclearleft Posted at: 2019-08-11T14:36:21.155Z Reads: 93

```
@Quezacotl - You got it to work ok?  Glad to hear it.
```

---
## \#2221 Posted by: Jonisonvespa Posted at: 2019-08-11T15:02:12.734Z Reads: 90

```
hello im in the uk, no no one yet would really like to make this if i can get hold of a shell
thank you
```

---
## \#2222 Posted by: captclearleft Posted at: 2019-08-11T15:17:47.452Z Reads: 93

```
@Jonisonvespa OK, I'm in the US. 
I just looked up the cost of shipping to the UK...  The cost is so high to ship, I would recommend you post a separate thread - Such as: "UK Firefly Remote Print Needed" or something...  Maybe there is an electric skateboard group on Facebook in your area you could reach out too.  
At $37 USD to ship a $5 part, does not seem worth it.  I will be happy to ship one to ya...  Just let me know.
```

---
## \#2223 Posted by: Jonisonvespa Posted at: 2019-08-11T16:33:32.037Z Reads: 88

```
hi thansk very much i will ask on the general section, very nivce of you to offer
```

---
## \#2224 Posted by: Quezacotl Posted at: 2019-08-11T20:25:31.092Z Reads: 90

```
Yea. Once the code is uploaded, it works straight away. I have latest VESC firmware, so it works atleast with that.
```

---
## \#2225 Posted by: Jonisonvespa Posted at: 2019-08-12T15:32:32.473Z Reads: 92

```
hi 
is there a reciever part toi this cant seem to find it
```

---
## \#2226 Posted by: captclearleft Posted at: 2019-08-13T15:09:15.866Z Reads: 98

```
INTERFERENCE ---  So I run a group ride and have found that Boosted boards particularly cause my board to glitch (like a very quick power on, power off... Or a stutter)...  I have done several rides without anyone around - No glitches...  

I know that some 2.4g addresses are susceptible to interference more than others.  I am researching that. 
I also am not on the latest version of Arduino firmware/software as developed by @solidgeek.  
I plan on updating everything this week.  

**Has anyone else seen this issue?**  

**Does anyone have a good idea of how to create an address that is more robust?**

Thanks.
```

---
## \#2227 Posted by: Qrob Posted at: 2019-08-13T23:00:01.988Z Reads: 90

```
@solidgeek can you make me one i would pay!
```

---
## \#2228 Posted by: KranzeKake Posted at: 2019-08-18T15:14:50.139Z Reads: 87

```
Anybody that is willing to make one for me?
More than happy to pay a little extra :))
```

---
## \#2229 Posted by: captclearleft Posted at: 2019-08-24T14:47:43.928Z Reads: 82

```
@Quezacotl , Which VescUart library did you use?  The SolidGeek/VescUart, or the Peemouse?  
And
Did you use the nRF24-Esk8-Remote "Developement branch" transmitter.ino sketch, or the "Master Branch" transmitter.ino sketch?  

I just updated my VESCs to the lasted firmware(3.58), and updated my sketches (with the peemouse / VescUart, and the Developement Branch version of the sketches, but now I am having issues...  

Just curious, thanks
```

---
## \#2230 Posted by: Quezacotl Posted at: 2019-08-24T15:08:27.219Z Reads: 75

```
You can see the links in my post...
```

---
## \#2231 Posted by: captclearleft Posted at: 2019-08-24T15:13:25.025Z Reads: 79

```
Ah, Indeed.  my bad. lol, Thanks!  **Have you had any connectivity issues, or disconnects**?  I am going to change my address back to the default address to see if that fixes the glitches.
```

---
## \#2232 Posted by: Quezacotl Posted at: 2019-08-24T15:32:10.748Z Reads: 83

```
My 3D-printed case is so bad quality that the throttle suffers from it and feels like connection problems. But so far no problems.
I designed a new pcb with all electronics, including battery within about 50x27x8mm area. Then i'll try to design a small casing for it also. I'll post pictures when i get it done when the pcbs arrive.
```

---
## \#2233 Posted by: captclearleft Posted at: 2019-08-27T03:58:53.537Z Reads: 83

```
Not sure if anyone is still using the Firefly remote - This thread has gotten real silent...  
Anyway, 
**Does anyone know how to setup the VESC with the vesc tool to take input from UART Only setting.**

I selected UART for "App to Use" in the VESC Tool.  Selected UART Only in the Settings on the remote...  Now I get nothing.  Not sure what to do from here.
Thanks
```

---
## \#2234 Posted by: solidgeek Posted at: 2019-08-27T20:51:12.585Z Reads: 80

```
You have to make sure that the VescUart-library version matches the firmware version of your VESC, otherwise it won't work. Benjamin didn't do a great job making anything backwards compatible.
```

---
## \#2235 Posted by: captclearleft Posted at: 2019-08-27T21:40:16.495Z Reads: 79

```
Interesting - Thank You.  I am right now using your (@solidgeek) [VescUart Lib](https://github.com/SolidGeek/VescUart/tree/development).  I tried the [Peemouse VescUART Lib](https://github.com/Peemouse/VescUart)  .  

I am using the VESC 4.12 with firmware v3.58.  So.. It looks like the SolidGeek v is good for Vesc firmware 3.51, and the PeeMouse is good for version 3.4.  

Thanks.  I think I get it.
```

---
## \#2236 Posted by: captclearleft Posted at: 2019-09-09T16:37:15.106Z Reads: 74

```
UNCOMMANDED FULL THROTTLE ???

Ok. So, I was cruising at a pretty slow speed and next thing you know - I am on my butt, and the board is full throttle into a ravine...  I look up, and board is upside down still at full throttle.  I try to hit the brake (pull back on throttle wheel) and nothing...  I look at the remote.  It is off. (switch must have gotten turned off by wrist strap during fall).  I turn on remote...  and try again.  Not sure if it connected as I was running into the ravine to turn off the board.  

Has anyone experienced this?
I am not sure why the VESC would get a full throttle command.

Specs:
Dual VESCs over CAN 4.12 Firmware 3.58
Current Firefly code with @solidgeek VESCUART lib 
Communicating over PPM (could not get UART to work).

Any suggestions would be appreciated. 
Thanks
```

---
## \#2237 Posted by: wallable Posted at: 2019-09-20T22:28:09.317Z Reads: 79

```
Hi guys,
I have recently been building an electric skateboard with @solidgeeks remote. I have completed the remote and receiver, and have uploaded the development version of the remote code and the development version of @solidgeeks VESC-UART library. When i power the remote and board up, the remote connects with the receiver and the percentage of the skateboard battery is displayed on the remote. However, when i press the deadman switch and move the accelerator on the remote, nothing happens.
I have tried the master version of @solidgeeks VESC-UART and the PEEMOUSE library also with no luck.
I have just downloaded the code and added the libraries, only changing the baud rate in the code if necessary, The address and channel are just the default values. I always make sure to clear the eeprom before uploading code.  Is there something i need to change with the receiver or remote code to get this to work? im a coding noob btw haha. 
in the vesc tool, i have the app settings on UART and the baud rate on 115200.
In the settings in the remote, i cannot change the type of communication from PPM and UART to solely UART.

My specs are, single Vanda vesc 4.12,  FW 3.58

Does anyone have an idea of what im missing? Cheers

EDIT: Got it sorted, I had a problem with not being able to change the remote to only UART, but was able to do it. then went through and paired the remote on the vesc tool and it worked.
Now my only problem is that the remote connects sometimes and sometimes i restart it and it doesnt connect with the reciever. it also freezes as soon as i press the deadman switch. im pretty sure this is a connection issue in the remote so will resolder the arduino pins and see how i go.
```

---
## \#2238 Posted by: Winkelmann Posted at: 2019-11-06T02:21:16.562Z Reads: 65

```
@solidgeek

Arduino: 1.8.9 (Windows Store 1.8.21.0) (Windows 10), Board: "Arduino Nano, ATmega328P (Old Bootloader)"

In function 'global constructors keyed to 65535_0_transmitter.ino.cpp.o':

lto1.exe: internal compiler error: Segmentation fault

Please submit a full bug report,

with preprocessed source if appropriate.

See <http://gcc.gnu.org/bugs.html> for instructions.

lto-wrapper.exe: fatal error: C:\Program Files\WindowsApps\ArduinoLLC.ArduinoIDE_1.8.21.0_x86__mdqgnx93n4wtt\hardware\tools\avr/bin/avr-gcc returned 1 exit status

compilation terminated.

c:/program files/windowsapps/arduinollc.arduinoide_1.8.21.0_x86__mdqgnx93n4wtt/hardware/tools/avr/bin/../lib/gcc/avr/5.4.0/../../../../avr/bin/ld.exe: error: lto-wrapper failed

collect2.exe: error: ld returned 1 exit status

exit status 1
Error compiling for board Arduino Nano.

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.
 
What do i do?

I tried the master branch to and then it gave me a null warning but then uploaded but the screen didnt light up... :confused:
```

---
## \#2239 Posted by: julian_esk8 Posted at: 2019-11-11T15:16:44.714Z Reads: 55

```
Hello, I experienced comparable issues with my remote. Running on stock development software. Whenever I tried to run my board with my DJI Mavic, nothing happens. The board is not responding in any way. 
Maybe you got some new knowledge in 2.4 GHz adresses. Let me know what you thing.

Best Regards 
Julian
```

---
## \#2240 Posted by: captclearleft Posted at: 2019-11-11T18:08:07.659Z Reads: 58

```
@julian_esk8 , Not sure waht you mean by:  

" run my board with my DJI Mavic, nothing happens"  ??

I ended up pulling the receiver out, and going back to riding with a regular remote. 

Summer is pretty short here in Colorado, and I wanted to ride.  Plus, I wanted to weed out any other components that may have caused the issue.  

So far.  The board runs fine, no glitches - So, I am assuming that my VESCs are fine, and were not the cause of the issue.  

Right now - I am thinking that my setup (NRF remote, and receiver) was the culprit.  
I am thinking maybe what happened was while riding the remote shut off, and turned back on or something, and when it did, the receiver got an incorrect signal... Or maybe the receiver board (cheep Chinese Arduino NANO) was tired of being rattled around in the battery case on the skateboard, and glitched.  

During the winter I will build another remote based on this remote, but there are other versions that are still being supported.  I think @solidgeek did a FANTASTIC job with this, but I think he has moved on to other things. 

What exactly is happening with your setup?
```

---
## \#2241 Posted by: Deakbannok Posted at: 2019-11-23T12:10:54.750Z Reads: 59

```
Here is what I have been picked up after him. My deployment and field time were carried me down to finish this.
I have changed a few things, additional wiring, resistor, and newer code. I prefer to stay with arduino nano controller because it is cheap, easy to find, and compact. The code will be post up sometime later once I get home in Thailand.

The controller supports multiple profile and address. You can use one controller 3+ different board. !![IMG_20191120_012346|375x500](upload://uCYU2xgJM2sKVsivFmdKIi8AWAe.jpeg) [IMG_20191123_121623|375x500](upload://a1EvTGXZTjZWd9dJujkYylwk1Ya.jpeg) 

![IMG_20191123_123149|375x500](upload://mtxshoEcrOJ3yDQ7JLA9kKUj6Sc.jpeg)
```

---
## \#2243 Posted by: Petja Posted at: 2019-12-16T23:02:18.950Z Reads: 47

```
Hi! Can you say, how to decrease  noise of throttle (I'm using version 2 (development))?
https://youtu.be/e6tgKDJsH3U
I need this for using "Control type - Duty" in PPM Configuration in VESC Tool.
And about your upgrade: can remote work with two receivers?
```

---
## \#2244 Posted by: luckyjacky Posted at: 2019-12-19T04:14:56.844Z Reads: 42

```
Hello, anyone can help with a screen remote for hobbywing ESC?
```

---
## \#2245 Posted by: Deakbannok Posted at: 2019-12-29T17:04:42.224Z Reads: 40

```
Yes, you can designate a different address on each profile for different receiver.
I do not have to create a wiring diagram. I will post up a wiring photo later in a few days.
```

---
## \#2246 Posted by: Deakbannok Posted at: 2020-01-11T16:40:59.625Z Reads: 33

```
This is final preview.
![featured_preview_IMG_20200111_171448|628x472](upload://oxgN7aMbNh8sN0fN4XwNw3tSqDV.jpeg)
```

---
## \#2247 Posted by: cchiou Posted at: 2020-02-11T09:39:01.863Z Reads: 10

```
hi guys, i was just reading through this post and was totally blown away how long this conversation has been ongoing.  Just a quick query, are you guys in the same country? same state? or area?  if so, have you guys ever thought of getting together to meet up and solve this error code?  if not, then it would make sense seeing how long this convo has been ongoing.  Great team work though... so impress by the work done, trial and error attempts and without failure, you will never succeed.  
Just out of curiosity where abouts are you guys based? I'm in australia melbourne.
```

---
